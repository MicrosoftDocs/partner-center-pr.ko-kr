---
title: 보고서 API - 데이터 Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용하여 파트너 센터 인사이트에서 사용 가능한 모든 보고서 ID를 얻을 수 있습니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376124"
---
# <a name="get-report-api"></a>보고서 API 가져오기

이 API는 예약된 모든 보고서를 가져옵니다.

**요청 구문**

|    방법    |    요청 URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**요청 헤더**

|    헤더    |    유형    |    Description    |
|    ----    |    ----    |    ----    |
|    권한 부여    |    문자열    |    필수 요소. 양식의 AAD(Azure Active Directory) 액세스 토큰`Bearer <token>`    |
|    콘텐츠 형식    |    문자열    |    `Application/JSON`    |
|        |        |        |

**경로 매개 변수**

없음

**쿼리 매개 변수**

|    매개 변수 이름    |    유형    |    필수    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    문자열    |    예    |    이 인수에 지정된 reportId가 있는 보고서만 자세히 보기 위한 필터     |
|    reportName     |    문자열    |    예    |    이 인수에 지정된 reportName이 있는 보고서만 자세히 보기 위한 필터     |
|    queryId     |    문자열    |    예    |    이 인수에 지정된 queryId를 사용하여 보고서 세부 정보만 가져오기 위한 필터     |
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
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**용어 설명**

다음 표에서는 응답의 주요 요소를 정의합니다.

|    매개 변수    |    Description    |
|    ----    |    ----    |
|    ReportId     |    생성된 보고서의 고유 UUID     |
|    ReportName     |    요청 페이로드의 보고서에 지정된 이름     |
|    Description     |    보고서를 만들 때 지정된 설명     |
|    QueryId     |    보고서를 만들 때 전달된 쿼리 ID     |
|    쿼리     |    이 보고서에 대해 실행되는 쿼리 텍스트     |
|    사용자     |    보고서를 만드는 데 사용되는 사용자 ID     |
|    CreatedTime     |    보고서가 생성된 시간입니다. 시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.     |
|    ModifiedTime     |    보고서를 마지막으로 수정한 시간입니다. 시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.     |
|    executeNow     |    보고서를 만들 때 설정된 ExecuteNow 플래그    |
|    StartTime     |    시간 실행이 시작됩니다. 시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.     |
|    ReportStatus     |    보고서 실행 상태입니다. 가능한 값은 일시 중지, 활성 및 비활성입니다.     |
|    RecurrenceInterval     |    보고서를 만드는 동안 제공된 되풀이 간격     |
|    RecurrenceCount     |    보고서를 만드는 동안 제공된 되풀이 수     |
|    CallbackUrl     |    요청에 제공된 콜백 URL     |
|    CallbackMethod    |    요청에 제공된 콜백 메서드    |
|    서식     |    보고서 파일 형식     |
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    메시지     |    API 실행의 상태 메시지     |
|    StatusCode     |    결과 코드입니다. 가능한 값은 200, 400, 401, 403, 500입니다.     |
|        |        |