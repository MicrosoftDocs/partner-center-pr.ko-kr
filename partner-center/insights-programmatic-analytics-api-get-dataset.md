---
title: 모든 데이터 집합 API 가져오기-Insights 데이터
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용 하 여 파트너 센터 정보에서 사용 가능한 모든 데이터 집합에 대 한 세부 정보를 가져옵니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375869"
---
# <a name="get-all-datasets-api"></a>모든 데이터 세트 API 가져오기

모든 데이터 세트 API 가져오기는 사용 가능한 데이터 세트를 모두 가져옵니다. 데이터 세트는 테이블, 열, 메트릭, 시간 범위를 나열합니다.

**요청 구문**

|    방법    |    요청 URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName    |    문자열    |    No    |    하나의 데이터 세트에 대한 세부 정보만 가져오도록 필터링    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**용어 설명**

다음 표에서는 응답의 주요 요소를 정의합니다.

|    매개 변수    |    Description    |
|    ----    |    ----    |
|    DatasetName     |    이 배열 개체가 정의하는 데이터 세트의 이름     |
|    SelectableColumns     |    선택 열에서 지정할 수 있는 원시 열     |
|    AvailableMetrics     |    선택 열에서 지정할 수 있는 집계/메트릭 열 이름     |
|    AvailableDateRanges     |    데이터 세트에 대한 보고서 쿼리에서 사용할 수 있는 날짜 범위     |
|    minimumRecurrenceInterval     |    되풀이 간격의 최 솟 값     |
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    메시지     |    API 실행의 상태 메시지     |
|    StatusCode     |    결과 코드입니다. 가능한 값은 200, 400, 401, 403, 500입니다.     |
|        |        |
