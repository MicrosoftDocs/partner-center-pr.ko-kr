---
title: 파트너 insights 프로그래밍 방식 액세스에 대 한 일반적인 질문
description: API를 통해 파트너 정보 데이터에 액세스 하는 방법에 대 한 일반적인 질문에 대 한 답을 가져옵니다.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376060"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>분석 데이터에 대한 프로그래밍 방식의 액세스 일반적인 질문

이 문서에서는 파트너 센터에서 프로그래밍 방식으로 파트너 정보 데이터에 액세스 하는 방법에 대 한 질문과 대답을 다룹니다.

## <a name="api-responses"></a>API 응답

200 (성공) 이외의 API 응답을 받을 수 있는 다양 한 시나리오는 무엇 인가요?

이 표에서는 API 응답 및이를 수신할 경우 수행할 작업을 설명 합니다.

|    오류 설명     |    오류 코드     |    문제 해결     |
|    ----    |    ----    |    ----    |
|    권한 없음     |    401     |    이는 인증 예외입니다. AAD (Azure Active Directory) 토큰이 올바른지 확인 합니다. AAD 토큰은 60 분 동안 유효 하며,이 시간 후에는 AAD 토큰을 다시 생성 해야 합니다.     |
|    테이블 이름이 잘못 되었습니다.     |    400     |    데이터 집합 이름이 잘못 되었습니다. "모든 데이터 집합 가져오기" API를 호출 하 여 데이터 집합 이름을 다시 확인 합니다.     |
|    열 이름이 잘못 되었습니다.     |    400     |    쿼리의 열 이름이 잘못 되었습니다. "모든 데이터 집합 가져오기" API를 호출 하거나 데이터 정의의 열 이름을 참조 하 여 열 이름을 다시 확인 합니다.    |
|    Null 또는 누락 값     |    400     |    API의 요청 페이로드의 일부로 필수 매개 변수가 없을 수 있습니다.     |
|    잘못 된 보고서 매개 변수     |    400     |    보고서 매개 변수가 올바른지 확인 하십시오. 예를 들어 RecurrenceInterval 매개 변수의 값을 4 미만으로 지정할 수 있습니다.     |
|    되풀이 간격은 4에서 2160 사이 여야 합니다.     |    400     |    RecurrenceInterval request 매개 변수의 값이 4에서 2160 사이 인지 확인 합니다.     |
|    잘못 된 QueryId     |    400     |    생성 된 QueryId를 다시 확인 합니다.     |
|    보고서 생성 시작 시간에 대 한 잘못 된 보고서 매개 변수는 현재 UTC 시간 으로부터 4 시간 이상 이어야 합니다.     |    400     |    요청 페이로드의 일부로 시작 시간 매개 변수는 과거 일 수 없습니다. 보고서의 시작 시간은 현재 UTC 시간에서 4 시간 이상 이어야 합니다.     |
|    요청 된 값 ' string '을 찾을 수 없습니다.     |    400     |    요청 매개 변수 또는 형식을 업데이트 했는지 확인 `callbackurl` 합니다.     |
|    지정 된 필터를 사용 하 여 항목을 찾을 수 없습니다.     |    404     |    보고서 실행 API 가져오기에 사용 된 보고서 id 매개 변수를 확인 합니다.     |
|    지정 된 필터 조건에 대 한 실행이 발생 하지 않았습니다. 보고서 id 또는 executionId를 다시 확인 하 고 보고서의 예약 된 실행 시간 후에 API를 다시 시도 합니다.     |    404     |    보고서 id이 올바른지 확인 합니다. 요청 페이로드에 지정 된 대로 보고서의 예약 된 실행 시간 이후에 API를 다시 시도 합니다.     |
|    보고서를 만드는 동안 내부 오류가 발생 했습니다. 상관 관계 ID <>     |    500     |    *StartTime*, *Querystarttime* 및 *querystarttime* 필드의 날짜 형식이 올바른지 확인 합니다.     |
|    서비스를 사용할 수 없음    |    500     |    계속 해 서 서비스를 사용할 수 없는 경우 (5xx 오류) 지원 티켓을 엽니다.    |
|        |        |        |

## <a name="no-records"></a>레코드 없음

보안 위치에서 보고서를 다운로드 하면 API 응답 200이 수신 됩니다. 레코드가 없는 이유는 무엇입니까?
쿼리의 문자열에 열 머리글에 대해 허용 되는 값 중 하나가 있는지 확인 합니다. 예를 들어이 쿼리는 0 개의 결과를 반환 합니다.

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

이 예제에서에 허용 되는 값은 `IsDuplicateRowForPGA` 0 또는 1입니다. 다양 한 열에 대해 가능한 모든 값에 대 한 [데이터 정의](insights-data-definitions.md) 를 참조 하세요.
