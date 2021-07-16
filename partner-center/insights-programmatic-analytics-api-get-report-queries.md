---
title: 보고서 쿼리 API Insights 데이터 가져오기
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용 하 여 보고서 API에서 사용할 수 있는 모든 쿼리를 가져올 수 있습니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376125"
---
# <a name="get-report-queries-api"></a>보고서 쿼리 API 가져오기

보고서 쿼리 가져오기 API는 보고서에서 사용할 수 있는 모든 쿼리를 가져옵니다. 기본값으로 모든 시스템 및 사용자 정의 쿼리를 가져옵니다.

**요청 구문**

|    방법    |    요청 URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**요청 헤더**

|    헤더    |    유형    |    Description    |
|    ----    |    ----    |    ----    |
|    권한 부여    |    문자열    |    필수 요소. 형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`    |
|    콘텐츠 형식    |    문자열    |    `Application/JSON`    |
|        |        |        |

**경로 매개 변수**

없음

**쿼리 매개 변수**

|    매개 변수 이름    |    유형    |    필수    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    문자열     |    No    |    인수에 지정된 ID를 가진 쿼리만 세부 정보를 가져오는 필터     |
|    queryName     |    문자열     |    No    |    인수에 지정된 이름을 가진 쿼리만 세부 정보를 가져오는 필터     |
|    IncludeSystemQueries     |    boolean     |    예    |    응답에 미리 정의된 시스템 쿼리 포함     |
|    Includeonly Systemqueries     |    boolean     |    예    |    응답에 시스템 쿼리만 포함     |
|        |        |        |        |


**요청 페이로드**

없음

**용어 설명**

없음

**응답**

응답 페이로드는 다음과 같이 구성됩니다.

응답 코드: 200, 400, 401, 403, 404, 500

응답 페이로드 예제:

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

**용어 설명**

다음 표에서는 응답의 주요 요소를 정의합니다.

|    매개 변수    |    Description    |
|    ----    |    ----    |
|    QueryId     |    쿼리의 고유 UUID     |
|    이름     |    쿼리를 만들 때 쿼리에 지정된 이름     |
|    Description     |    쿼리를 만드는 동안 제공된 설명     |
|    쿼리     |    보고서 쿼리 문자열     |
|    유형     |    미리 정의 된 시스템 쿼리를 위해 사용자가 만든 쿼리 및 시스템에 대 한 사용자 정의로 설정     |
|    사용자     |    쿼리를 만든 사용자 ID     |
|    CreatedTime     |    쿼리를 만든 시간     |
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    메시지     |    API 실행의 상태 메시지     |
|    StatusCode     |    결과 코드입니다. 가능한 값은 200, 400, 401, 403, 500입니다.     |
|        |        |
