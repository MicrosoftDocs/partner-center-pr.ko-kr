---
title: report queries API Insights 데이터 삭제
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용 하 여 파트너 센터 정보에서 사용자 정의 쿼리를 삭제 합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375886"
---
# <a name="delete-report-queries-api"></a>보고서 쿼리 API 삭제

이 API는 사용자 정의 쿼리를 삭제 합니다.

**요청 구문**

|    방법    |    요청 URI    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**요청 헤더**

|    헤더    |    유형    |    Description    |
|    ----    |    ----    |    ----    |
|    권한 부여    |    문자열    |    필수 요소. 형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`    |
|    콘텐츠 형식    |    문자열    |    `Application/JSON`    |
|        |        |        |

**경로 매개 변수**

|    매개 변수 이름    |    유형    |    필수    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    문자열     |    No    |    인수에 지정된 ID를 가진 쿼리만 세부 정보를 가져오는 필터     |
|        |        |        |        |

**쿼리 매개 변수**

없음

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
|    QueryId     |    삭제 된 쿼리의 고유 UUID    |
|    이름     |    삭제 된 쿼리의 이름    |
|    Description     |    삭제 된 쿼리에 대 한 설명     |
|    쿼리     |    삭제 된 쿼리의 보고서 쿼리 문자열    |
|    유형     |    사용자가 만든 쿼리의 사용자 정의로 설정     |
|    사용자     |    쿼리를 만든 사용자 ID     |
|    CreatedTime     |    쿼리를 만든 시간     |
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    메시지     |    API 실행의 상태 메시지     |
|    StatusCode     |    결과 코드입니다. 가능한 값은 200, 400, 401, 403, 500입니다.     |
|        |        |
