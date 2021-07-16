---
title: 보고서 API 업데이트
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 정보에서이 API를 사용 하 여 보고서 매개 변수를 업데이트 합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376092"
---
# <a name="update-report-api"></a>보고서 API 업데이트

이 API는 보고서 매개 변수를 수정하는 데 도움이 됩니다.

**요청 구문**

|    방법    |    요청 URI    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    문자열    |    예    |    수정 중인 보고서의 ID     |
|        |        |        |        |

**쿼리 매개 변수**

없음

**요청 페이로드**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**용어 설명**

다음 표에서는 응답의 요소에 대 한 주요 정의를 보여 줍니다.

|    매개 변수    |    필수    |    Description    |    허용되는 값    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    예     |    보고서에 할당할 이름     |    String     |
|    설명     |    아니요     |    생성된 보고서에 대한 설명     |    문자열     |
|    StartTime     |    예    |    보고서 생성이 시작되는 타임스탬프     |    문자열     |
|    RecurrenceInterval     |    No     |    보고서가 생성되어야 하는 빈도(시간)입니다. 최솟값은 4입니다.     |    정수     |
|    RecurrenceCount     |    아니요     |    생성할 보고서 수입니다. 기본값은 무한입니다.     |    정수     |
|    형식     |    아니요    |    내보낸 파일의 파일 형식입니다. 기본값은 CSV입니다.     |    CSV/TSV     |
|    콜백 URL     |    아니요     |    보고서 생성 시 호출할 https 콜백 URL     |    문자열     |
|    CallbackMethod    |    아니요    |    콜백에 사용할 Http 메서드입니다.    |    GET/POST    |
|        |        |        |        |


**응답**

응답 페이로드는 다음과 같이 구성됩니다.

응답 코드: 200, 400, 401, 403, 404, 500

응답 페이로드 예제:

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
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
|    ReportId     |    업데이트 중인 보고서의 UUID(범용 고유 식별자)     |
|    ReportName     |    요청 페이로드의 보고서에 지정된 이름     |
|    Description     |    요청 페이로드의 보고서에 지정 된 설명입니다.     |
|    QueryId     |    보고서를 만들 때 전달된 쿼리 ID     |
|    쿼리     |    이 보고서에 대해 실행되는 쿼리 텍스트     |
|    사용자     |    보고서를 만드는 데 사용되는 사용자 ID     |
|    CreatedTime     |    보고서가 생성된 시간입니다. 시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.     |
|    ModifiedTime     |    보고서를 마지막으로 수정한 시간입니다. 시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.     |
|    ExecuteNow     |    보고서를 만들 때 설정 되는 ExecuteNow 플래그    |
|    StartTime     |    보고서 실행이 시작되는 시간입니다. 시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.     |
|    ReportStatus     |    보고서 실행 상태입니다. 가능한 값은 일시 중지, 활성 및 비활성입니다.     |
|    RecurrenceInterval     |    요청 페이로드에 제공 된 되풀이 간격     |
|    RecurrenceCount     |    요청 페이로드에 제공 된 되풀이 횟수     |
|    콜백 url     |    요청에 제공된 콜백 URL     |
|    CallbackMethod    |    요청에 제공 된 콜백 메서드입니다.    |
|    서식     |    보고서 파일 형식     |
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    메시지     |    API 실행의 상태 메시지     |
|    StatusCode     |    결과 코드입니다. 가능한 값은 200, 400, 401, 403, 500입니다.     |
|        |        |