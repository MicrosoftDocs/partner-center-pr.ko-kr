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
# <a name="custom-query-specification"></a><span data-ttu-id="63d63-103">사용자 지정 쿼리 사양</span><span class="sxs-lookup"><span data-stu-id="63d63-103">Custom query specification</span></span>

<span data-ttu-id="63d63-104">파트너는 이 쿼리 사양을 통해 분석 테이블에서 데이터를 추출하기 위한 사용자 지정 쿼리를 쉽게 작성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="63d63-105">쿼리를 사용하여 특정 조건과 일치하는 열과 메트릭만 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="63d63-106">언어 사양의 핵심은 사용자 지정 쿼리를 작성할 수 있는 데이터 세트 정의입니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="63d63-107">데이터 세트</span><span class="sxs-lookup"><span data-stu-id="63d63-107">Datasets</span></span>

<span data-ttu-id="63d63-108">사용자 지정 쿼리는 테이블과 열을 포함하는 데이터베이스에 대해 일부 쿼리를 실행하는 것과 동일한 방식으로 열과 메트릭이 포함된 데이터 세트에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="63d63-109">쿼리 작성에 사용할 수 있는 데이터 세트의 전체 목록은 데이터 세트 API를 사용하여 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="63d63-110">다음은 JSON으로 표시 되는 데이터 집합의 예입니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="63d63-111">데이터 세트의 구성</span><span class="sxs-lookup"><span data-stu-id="63d63-111">Parts of a dataset</span></span>

- <span data-ttu-id="63d63-112">데이터 세트 이름은 데이터베이스 테이블 이름과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="63d63-113">예:.</span><span class="sxs-lookup"><span data-stu-id="63d63-113">For example, OfficeUsage.</span></span> <span data-ttu-id="63d63-114">데이터 집합에는 CustomerTenantId와 같이 선택할 수 있는 열 목록이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="63d63-115">데이터 세트에는 데이터베이스의 집계 함수와 같은 메트릭도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="63d63-116">예: TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="63d63-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="63d63-117">데이터를 내보낼 수 있는 고정된 시간 범위가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="63d63-118">데이터 세트에 대한 쿼리 작성</span><span class="sxs-lookup"><span data-stu-id="63d63-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="63d63-119">다음은 다양한 유형의 데이터를 추출하는 방법을 보여주는 몇 가지 샘플 쿼리입니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="63d63-120">쿼리</span><span class="sxs-lookup"><span data-stu-id="63d63-120">Query</span></span>|    <span data-ttu-id="63d63-121">Description</span><span class="sxs-lookup"><span data-stu-id="63d63-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="63d63-122">**선택** CustomerTenantId, 다음 **에서 Paid부터 시작** 되는 단위</span><span class="sxs-lookup"><span data-stu-id="63d63-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="63d63-123">LAST_MONTH 사용 **TIMESPAN**</span><span class="sxs-lookup"><span data-stu-id="63d63-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="63d63-124">이 쿼리는 지난 1 달 동안 모든 CusotmerTenantID 및 해당 하는 Paid 단위를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="63d63-125">**선택** CustomerTenantId, 다음 **에서 Paid부터 시작** 되는 단위</span><span class="sxs-lookup"><span data-stu-id="63d63-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="63d63-126">**Paid사용이** 제한 된 단위 **제한** 10</span><span class="sxs-lookup"><span data-stu-id="63d63-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="63d63-127">이 쿼리는 사용 가능한 유료 단위 수의 내림차순으로 상위 10 개 고객 테 넌 트를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="63d63-128">**선택** CustomerTenantId, **Paid사용 가능** 단위, Monthlyactiveusers **에서** monthlyactiveusers > 10만 **ORDER By** monthlyactiveusers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="63d63-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="63d63-129">이 쿼리는 MonthlyActiveUsers가 10만 보다 큰 모든 고객의 Paid사용할 수 있는 단위 및 MonthlyActiveUsers를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="63d63-130">**선택** CustomerTenantId, Month, MonthlyActiveUsers </span><span class="sxs-lookup"><span data-stu-id="63d63-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="63d63-131">(' 2a31c234-1f4e-4c60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-b378-0242ac130002 ')에서 customertpid를 사용 하 **는 경우**</span><span class="sxs-lookup"><span data-stu-id="63d63-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="63d63-132">이 쿼리는 "2a31c234-1f4e-4c60-909e-76d234f93161 ' 및 ' 80780748-3f9a-11eb-b378-0242ac130002 ' 이라는 두 CustomerTpId 값을 기준으로 매월의 CustomerTenantId 및 월별 활성 사용자를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="63d63-133">쿼리 사양</span><span class="sxs-lookup"><span data-stu-id="63d63-133">Query specification</span></span>

<span data-ttu-id="63d63-134">이 섹션에서는 쿼리 정의와 구조에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="63d63-135">문법 참조</span><span class="sxs-lookup"><span data-stu-id="63d63-135">Grammar reference</span></span>

<span data-ttu-id="63d63-136">이 표에서는 쿼리에 사용되는 기호에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="63d63-137">쿼리</span><span class="sxs-lookup"><span data-stu-id="63d63-137">Query</span></span>    |    <span data-ttu-id="63d63-138">Description</span><span class="sxs-lookup"><span data-stu-id="63d63-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="63d63-139">선택 사항</span><span class="sxs-lookup"><span data-stu-id="63d63-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="63d63-140">없거나 1개 이상</span><span class="sxs-lookup"><span data-stu-id="63d63-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="63d63-141">1개 이상</span><span class="sxs-lookup"><span data-stu-id="63d63-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="63d63-142">또는/목록 중 하나</span><span class="sxs-lookup"><span data-stu-id="63d63-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="63d63-143">쿼리 정의</span><span class="sxs-lookup"><span data-stu-id="63d63-143">Query definition</span></span>

<span data-ttu-id="63d63-144">쿼리 문에는 SelectClause, FromClause, WhereClause, OrderClause, 절 및 TimeSpan 절이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="63d63-145">**Selectclause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="63d63-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="63d63-146">**ColumOrMetricName**: 데이터 세트 내에 정의된 열 및 메트릭</span><span class="sxs-lookup"><span data-stu-id="63d63-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="63d63-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="63d63-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="63d63-148">**DatasetName**: 데이터 세트 내에 정의된 데이터 세트 이름</span><span class="sxs-lookup"><span data-stu-id="63d63-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="63d63-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="63d63-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="63d63-150">**FilterCondition**: ColumOrMetricName Operator 값</span><span class="sxs-lookup"><span data-stu-id="63d63-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="63d63-151">**연산자**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="63d63-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="63d63-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="63d63-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="63d63-153">**숫자**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="63d63-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="63d63-154">**Stringliteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="63d63-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="63d63-155">**MultiNumberList**: `(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="63d63-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="63d63-156">**Multistringlist**: `(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="63d63-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="63d63-157">**Orderclause**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="63d63-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="63d63-158">**Ordercondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="63d63-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="63d63-159">대만 **절**:`LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="63d63-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="63d63-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="63d63-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="63d63-161">쿼리 구조</span><span class="sxs-lookup"><span data-stu-id="63d63-161">Query Structure</span></span>

<span data-ttu-id="63d63-162">보고서 쿼리는 여러 부분으로 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="63d63-163">각 파트에 대한 설명은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="63d63-164">쿼리의 이 부분은 내보낼 열을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="63d63-165">선택할 수 있는 열은 데이터 집합의 *selectableColumns* 및 *availableMetrics* 섹션에 나열 된 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="63d63-166">선택적으로 `DISTINCT` 키워드는 뒤에 지정할 수 있습니다 `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="63d63-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="63d63-167">을 `DISTINCT` 지정 하면 내보낸 마지막 행에는 항상 선택한 열에 대 한 고유 값이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="63d63-168">선택 된 열의 각 고유 조합에 대해 메트릭이 계산 되므로 `DISTINCT` 메트릭 열이 열 선택 목록에 포함 된 경우에는 키워드가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="63d63-169">**예:**</span><span class="sxs-lookup"><span data-stu-id="63d63-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="63d63-170">쿼리의 이 부분은 데이터를 내보내야 하는 데이터 세트를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="63d63-171">여기에 지정된 데이터 세트 이름은 데이터 세트 API에서 반환되는 유효한 데이터 세트 이름이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="63d63-172">**예:**</span><span class="sxs-lookup"><span data-stu-id="63d63-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="63d63-173">쿼리의 이 부분은 데이터 세트에 대한 필터 조건을 지정하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="63d63-174">최종적으로 내보낸 파일에는 이 절에 나열된 모든 조건과 일치하는 행만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="63d63-175">필터 조건은 *selectableColumns* 및 *availableMetrics* 에 나열 된 열 중 하나에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="63d63-176">필터 조건에 지정되는 값은 연산자가 `IN` 또는 `NOT IN`인 경우에만 숫자 목록 또는 문자열 목록일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="63d63-177">값은 항상 리터럴 문자열로 주어질 수 있으며, 이러한 값은 기본 형식의 열로 변환됩니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="63d63-178">여러 필터 조건을 AND 작업으로 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="63d63-179">**예:**</span><span class="sxs-lookup"><span data-stu-id="63d63-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="63d63-180">쿼리의 이 부분은 내보낸 행의 정렬 조건을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="63d63-181">순서를 정의할 수 있는 열은 데이터 집합의 *selectableColumns* 및 *availableMetrics* 에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="63d63-182">지정 된 순서 방향이 없으면 열에 대해 기본적으로 DESC로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="63d63-183">정렬은 여러 열에 대해 정의할 수 있으며, 쉼표로 구분합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="63d63-184">**예:**</span><span class="sxs-lookup"><span data-stu-id="63d63-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="63d63-185">쿼리의 이 부분은 내보낼 행의 수를 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="63d63-186">지정하려는 숫자는 0이 아닌 양의 정수여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="63d63-187">쿼리의 이 부분은 데이터를 내보내고자 하는 기간을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="63d63-188">데이터 집합 정의의 *availableDateRanges* 필드에서 가능한 값을 지정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="63d63-189">쿼리 사양의 대/소문자 구분</span><span class="sxs-lookup"><span data-stu-id="63d63-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="63d63-190">쿼리 사양은 대/소문자를 구분하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="63d63-191">미리 정의된 키워드, 열 이름 및 값은 대문자나 소문자를 사용하여 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63d63-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="63d63-192">다음 단계</span><span class="sxs-lookup"><span data-stu-id="63d63-192">Next steps</span></span>

- [<span data-ttu-id="63d63-193">시스템 쿼리 목록</span><span class="sxs-lookup"><span data-stu-id="63d63-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="63d63-194">샘플 쿼리 목록</span><span class="sxs-lookup"><span data-stu-id="63d63-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)