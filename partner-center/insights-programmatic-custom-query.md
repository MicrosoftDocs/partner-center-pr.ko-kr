---
title: 사용자 지정 쿼리 사양
description: 분석 테이블에서 데이터를 추출 하는 사용자 지정 쿼리를 만드는 방법에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376069"
---
# <a name="custom-query-specification"></a>사용자 지정 쿼리 사양

파트너는 이 쿼리 사양을 통해 분석 테이블에서 데이터를 추출하기 위한 사용자 지정 쿼리를 쉽게 작성할 수 있습니다. 쿼리를 사용하여 특정 조건과 일치하는 열과 메트릭만 선택할 수 있습니다. 언어 사양의 핵심은 사용자 지정 쿼리를 작성할 수 있는 데이터 세트 정의입니다.

## <a name="datasets"></a>데이터 세트

사용자 지정 쿼리는 테이블과 열을 포함하는 데이터베이스에 대해 일부 쿼리를 실행하는 것과 동일한 방식으로 열과 메트릭이 포함된 데이터 세트에서 작동합니다. 쿼리 작성에 사용할 수 있는 데이터 세트의 전체 목록은 데이터 세트 API를 사용하여 가져올 수 있습니다.

다음은 JSON으로 표시 되는 데이터 집합의 예입니다.

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>데이터 세트의 구성

- 데이터 세트 이름은 데이터베이스 테이블 이름과 같습니다. 예:. 데이터 집합에는 CustomerTenantId와 같이 선택할 수 있는 열 목록이 있습니다.
- 데이터 세트에는 데이터베이스의 집계 함수와 같은 메트릭도 있습니다. 예: TotalMonthlyActiveUsers.
- 데이터를 내보낼 수 있는 고정된 시간 범위가 있습니다.

## <a name="formulating-a-query-on-a-dataset"></a>데이터 세트에 대한 쿼리 작성

다음은 다양한 유형의 데이터를 추출하는 방법을 보여주는 몇 가지 샘플 쿼리입니다.

|쿼리|    Description    |
|----|    ----    |
|**선택** CustomerTenantId, 다음 **에서 Paid부터 시작** 되는 단위 <br>LAST_MONTH 사용 **TIMESPAN**|    이 쿼리는 지난 1 달 동안 모든 CusotmerTenantID 및 해당 하는 Paid 단위를 가져옵니다.    |
|**선택** CustomerTenantId, 다음 **에서 Paid부터 시작** 되는 단위 <br>**Paid사용이** 제한 된 단위 **제한** 10|    이 쿼리는 사용 가능한 유료 단위 수의 내림차순으로 상위 10 개 고객 테 넌 트를 가져옵니다.     |
|**선택** CustomerTenantId, **Paid사용 가능** 단위, Monthlyactiveusers **에서** monthlyactiveusers > 10만 **ORDER By** monthlyactiveusers **TIMESPAN** LAST_6_MONTHS |    이 쿼리는 MonthlyActiveUsers가 10만 보다 큰 모든 고객의 Paid사용할 수 있는 단위 및 MonthlyActiveUsers를 가져옵니다.     |
|**선택** CustomerTenantId, Month, MonthlyActiveUsers  <br>(' 2a31c234-1f4e-4c60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-b378-0242ac130002 ')에서 customertpid를 사용 하 **는 경우** |    이 쿼리는 "2a31c234-1f4e-4c60-909e-76d234f93161 ' 및 ' 80780748-3f9a-11eb-b378-0242ac130002 ' 이라는 두 CustomerTpId 값을 기준으로 매월의 CustomerTenantId 및 월별 활성 사용자를 가져옵니다.     |
|        |        |

## <a name="query-specification"></a>쿼리 사양

이 섹션에서는 쿼리 정의와 구조에 대해 설명합니다.

## <a name="grammar-reference"></a>문법 참조

이 표에서는 쿼리에 사용되는 기호에 대해 설명합니다.

|    쿼리    |    Description    |
|    ----    |    ----    |
|    `?`    |    선택 사항    |
|    `*`    |    없거나 1개 이상    |
|    `+`    |    1개 이상    |
|    `\|`    |    또는/목록 중 하나    |
|        |        |

## <a name="query-definition"></a>쿼리 정의

쿼리 문에는 SelectClause, FromClause, WhereClause, OrderClause, 절 및 TimeSpan 절이 있습니다.

- **Selectclause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName**: 데이터 세트 내에 정의된 열 및 메트릭
- **FromClause**: `FROM DatasetName`
    - **DatasetName**: 데이터 세트 내에 정의된 데이터 세트 이름
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition**: ColumOrMetricName Operator 값
        - **연산자**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Value**: Number | StringLiteral | MultiNumberList | MultiStringList
            - **숫자**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **Stringliteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList**: `(Number (,Number)*)`
            - **Multistringlist**: `(StringLiteral (,StringLiteral)*)`
- **Orderclause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **Ordercondition**: `ColumOrMetricName (ASC | DESC)*`
- 대만 **절**:`LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>쿼리 구조

보고서 쿼리는 여러 부분으로 구성됩니다.
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

각 파트에 대한 설명은 다음과 같습니다.

### `SELECT`

쿼리의 이 부분은 내보낼 열을 지정합니다. 선택할 수 있는 열은 데이터 집합의 *selectableColumns* 및 *availableMetrics* 섹션에 나열 된 필드입니다.

선택적으로 `DISTINCT` 키워드는 뒤에 지정할 수 있습니다 `SELECT` . 을 `DISTINCT` 지정 하면 내보낸 마지막 행에는 항상 선택한 열에 대 한 고유 값이 포함 됩니다. 선택 된 열의 각 고유 조합에 대해 메트릭이 계산 되므로 `DISTINCT` 메트릭 열이 열 선택 목록에 포함 된 경우에는 키워드가 필요 하지 않습니다.

**예:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

쿼리의 이 부분은 데이터를 내보내야 하는 데이터 세트를 나타냅니다. 여기에 지정된 데이터 세트 이름은 데이터 세트 API에서 반환되는 유효한 데이터 세트 이름이어야 합니다.

**예:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

쿼리의 이 부분은 데이터 세트에 대한 필터 조건을 지정하는 데 사용됩니다. 최종적으로 내보낸 파일에는 이 절에 나열된 모든 조건과 일치하는 행만 표시됩니다. 필터 조건은 *selectableColumns* 및 *availableMetrics* 에 나열 된 열 중 하나에 있을 수 있습니다. 필터 조건에 지정되는 값은 연산자가 `IN` 또는 `NOT IN`인 경우에만 숫자 목록 또는 문자열 목록일 수 있습니다. 값은 항상 리터럴 문자열로 주어질 수 있으며, 이러한 값은 기본 형식의 열로 변환됩니다. 여러 필터 조건을 AND 작업으로 구분 해야 합니다.

**예:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

쿼리의 이 부분은 내보낸 행의 정렬 조건을 지정합니다. 순서를 정의할 수 있는 열은 데이터 집합의 *selectableColumns* 및 *availableMetrics* 에 있어야 합니다. 지정 된 순서 방향이 없으면 열에 대해 기본적으로 DESC로 설정 됩니다. 정렬은 여러 열에 대해 정의할 수 있으며, 쉼표로 구분합니다.

**예:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

쿼리의 이 부분은 내보낼 행의 수를 지정합니다. 지정하려는 숫자는 0이 아닌 양의 정수여야 합니다.

### `TIMESPAN`

쿼리의 이 부분은 데이터를 내보내고자 하는 기간을 지정합니다. 데이터 집합 정의의 *availableDateRanges* 필드에서 가능한 값을 지정 해야 합니다.

### <a name="case-sensitivity-in-query-specification"></a>쿼리 사양의 대/소문자 구분

쿼리 사양은 대/소문자를 구분하지 않습니다. 미리 정의된 키워드, 열 이름 및 값은 대문자나 소문자를 사용하여 지정할 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [시스템 쿼리 목록](insights-programmatic-system-queries.md)
- [샘플 쿼리 목록](insights-programmatic-sample-queries.md)