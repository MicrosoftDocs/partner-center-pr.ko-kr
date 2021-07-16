---
title: 보고서 쿼리 API 사용해 보기
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용하여 쿼리를 테스트하고 파트너 센터 인사이트에서 결과의 유효성을 검사합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376093"
---
# <a name="try-report-queries-api"></a>보고서 쿼리 API 사용해 보기

이 API는 보고서 쿼리 문을 실행합니다. API는 파트너가 데이터를 예상한 대로 확인하는 데 사용할 수 있는 레코드를 100개만 반환합니다.

> [!IMPORTANT]
> 이 API의 쿼리 실행 제한 시간은 100초입니다. API에 100초 이상이 소요될 경우 쿼리가 구문상 정확할 가능성이 높습니다. 그렇지 않으면 200 이외의 오류 코드를 수신하게 됩니다. 쿼리 구문이 올바르면 실제 보고서 생성이 성공합니다.

**요청 구문**

|    방법    |    요청 URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
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
|    exportQuery     |    문자열    |    예    |    실행해야 하는 보고서 쿼리 문자열     |
|    queryId     |    문자열    |    예    |    유효한 기존 쿼리 ID입니다. exportQuery 매개 변수에 지정된 쿼리 문자열과 함께 사용할 수 없습니다.    |
|    startTime     |    문자열    |    예    |    데이터를 원하는 시작 시간입니다. 쿼리에 지정된 시간 간격을 재정의합니다.    |
|    endTime     |    문자열    |    예    |    데이터를 원하는 시간까지의 종료 시간입니다. 쿼리에 지정된 시간 간격을 재정의합니다.    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    메시지     |    API 실행의 상태 메시지     |
|    StatusCode     |    결과 코드입니다. 가능한 값은 200, 400, 401, 403, 500입니다.     |
|        |        |
