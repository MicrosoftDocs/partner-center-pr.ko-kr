---
title: Insights 데이터에 대 한 프로그래밍 방식 액세스 패러다임
description: 프로그래밍 분석을 위한 API 호출 패턴의 대략적인 흐름을 이해합니다. 파트너 insights 분석 보고서에 액세스 하는 Api에 대해서도 설명 합니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375887"
---
# <a name="programmatic-access-paradigm"></a>프로그래밍 방식 액세스 페러다임

이 다이어그램에서는 새 보고서 템플릿을 만들고, 사용자 지정 보고서를 예약 하 고, 오류 데이터를 검색 하는 데 사용 되는 API 호출 패턴을 보여 줍니다.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="상위 수준 흐름":::
***그림 1: API 호출 패턴의 높은 수준 흐름***

이 목록에는 그림 1에 대한 자세한 내용이 나와 있습니다.

1. 클라이언트 애플리케이션은 [보고서 쿼리 만들기 API](#create-report-query-api)를 호출하여 사용자 지정 보고서 스키마/템플릿을 정의할 수 있습니다. 또는 여기에 나열 된 보고서 템플릿 라이브러리 샘플에서 보고서 템플릿 (QueryId)을 선택할 수 있습니다 [.](insights-programmatic-system-queries.md)
2. 성공 하면 보고서 만들기 쿼리 API가 QueryId를 반환 합니다.
3. 그런 다음 클라이언트 응용 프로그램은 보고서 시작 날짜, 반복 간격, 되풀이 및 선택적 콜백 URI와 함께 QueryId를 사용 하 여 [보고서 만들기 API](#create-report-api) 를 호출 해야 합니다.
4. 성공 하면 [보고서 만들기 API](#create-report-api) 가 보고서 id를 반환 합니다.
5. 클라이언트 응용 프로그램은 보고서 데이터를 다운로드할 준비가 되는 즉시 콜백 URL에 대 한 알림 메시지를 받습니다.
6. 그러면 클라이언트 응용 프로그램에서 보고서 [실행 API 가져오기 API](#get-report-execution-api) 를 사용 하 여 보고서 ID 및 날짜 범위로 보고서 상태를 쿼리 합니다.
7. 성공 시 보고서 다운로드 링크가 반환되고 애플리케이션에서 데이터 다운로드를 시작할 수 있습니다.

## <a name="report-query-language-specification"></a>보고서 쿼리 언어 사양

보고서를 만드는 데 사용할 수 있는 [시스템 쿼리](insights-programmatic-system-queries.md) 를 제공 하지만 비즈니스 요구 사항에 따라 고유한 쿼리를 만들 수도 있습니다. 사용자 지정 쿼리에 대 한 자세한 내용은 [사용자 지정 쿼리 사양](insights-programmatic-custom-query.md)을 참조 하세요.

## <a name="create-report-query-api"></a>보고서 쿼리 만들기 API

API를 사용 하면 열과 메트릭을 내보내야 하는 데이터 집합을 정의 하는 사용자 지정 쿼리를 만들 수 있습니다. 이 API는 비즈니스 요구에 따라 새 보고 템플릿을 만들 수 있는 유연성을 제공합니다.  

기본 제공되는 [시스템 쿼리](insights-programmatic-system-queries.md)를 사용할 수도 있습니다. 사용자 지정 보고서 템플릿이 필요 하지 않은 경우 제공 된 시스템 쿼리의 QueryIds를 사용 하 여 직접 [Create REPORT API](#create-report-api) 를 호출할 수 있습니다.  

다음 예에서는 지난 달의 수익을 기준으로 상위 10 명의 고객을 가져오는 사용자 지정 쿼리를 만드는 방법을 보여 줍니다.

### <a name="request-syntax"></a>요청 구문

|    방법     |    요청 URI     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>요청 헤더

|    헤더     |    유형     |    Description     |
|-------|-----|------|
|    권한 부여     |    문자열 |필수 요소. Azure AD(Azure Active Directory) 액세스 토큰입니다. 형식은  `Bearer <token>` 입니다.|
|    콘텐츠 형식     |문자열 |`Application/JSON` |
||||

### <a name="path-parameter"></a>경로 매개 변수

None

### <a name="query-parameter"></a>쿼리 매개 변수

None

### <a name="sample-request-payload"></a>샘플 요청 페이로드

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>용어

이 표에는 요청 페이로드에 있는 요소의 주요 정의가 나열되어 있습니다.

|매개 변수|    필수     |    Description     |    허용되는 값     |
|-----|    -----    |    -----    |    -----    |
|이름 |    예     |    쿼리의 식별 이름     |    문자열     |
|    설명     |    아니요     |    쿼리가 반환하는 내용에 대한 설명     |    문자열     |
|    쿼리     |    예     |    보고서 쿼리 문자열     |    데이터 형식: 문자열 <br> 비즈니스 요구 사항에 따른 [사용자 지정 쿼리](insights-programmatic-custom-query.md) |
|        |        |        |        |

> [!Note]
> 사용자 지정 쿼리 예제는 [샘플 쿼리 예제](insights-programmatic-sample-queries.md) 를 참조 하세요.

### <a name="sample-response"></a>샘플 응답

응답 페이로드는 다음과 같이 구성됩니다.

응답 코드: 200, 400, 401, 403, 500

응답 페이로드 예제:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>용어

이 표에는 요청 페이로드에 있는 요소의 주요 정의가 나열되어 있습니다.

|    매개 변수     |    Description     |
|    ----    |    ----    |
|    QueryId     |    만든 쿼리의 UUID(범용 고유 식별자)     |
|    이름     |    요청 페이로드의 쿼리에 지정된 식별 이름     |
|    Description     |    쿼리를 만드는 동안 제공된 설명     |
|    쿼리     |    쿼리를 만드는 동안 입력으로 전달된 보고서 쿼리     |
|    유형     |    `userDefined`     |
|    사용자     |    쿼리를 만드는 데 사용 되는 사용자 ID     |
|    CreatedTime     |    쿼리가 생성된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)     |
|    TotalCount     |    값 배열의 데이터 세트 수     |
|    StatusCode     |    결과 코드 <br> 가능한 값은 200, 400, 401, 403, 500입니다.     |
|    message     |    API 실행의 상태 메시지     |
|        |        |

## <a name="create-report-api"></a>보고서 만들기 API

[보고서 쿼리 응답 만들기](#create-report-query-api) 의 일부로 사용자 지정 보고서 템플릿을 만들고 QueryID를 수신 하는 경우이 API를 호출 하 여 정기적으로 실행 되도록 쿼리를 예약할 수 있습니다. 보고서가 배달되는 빈도 및 일정을 설정할 수 있습니다.
기본 제공되는 시스템 쿼리의 경우 [QueryId](insights-programmatic-system-queries.md)를 사용하여 보고서 만들기 API를 호출할 수도 있습니다.

### <a name="callback-url"></a>콜백 URL

보고서 만들기 API는 콜백 URL을 허용 합니다. 이 URL은 보고서 생성에 성공하면 호출됩니다. 콜백 URL은 공개적으로 연결할 수 있어야 합니다. URL 외에도 콜백 메서드를 지정할 수 있습니다. 콜백 메서드는 "GET" 또는 "POST"만 될 수 있습니다. 값이 전달되지 않는 경우 기본 메서드는 "POST"입니다. 생성이 완료된 reportId는 콜백 중에 항상 다시 전달됩니다.

POST 콜백: 전달된 URL이 `https://www.contosso.com/callback` 이면 호출된 URL은 입니다. `https://www.contosso.com/callback/<reportID>` 

GET 콜백: 전달된 URL이 `https://www.contosso.com/callback` 이면 호출된 URL은 입니다. `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow 보고서

예약하지 않고 보고서를 생성하는 프로비전이 있습니다. 보고서 만들기 API 페이로드는 매개 변수 를 수락할 수 있습니다. 이 매개 `ExecuteNow` 변수는 API가 호출되는 즉시 생성되는 보고서를 시차로 립니다. `ExecuteNow`이 true로 설정되면 `StartTime` , `RecurrenceCount` , `RecurrenceInterval` 필드가 무시됩니다. 이러한 보고서는 예약되지 않습니다.

가 true인 경우 두 개의 추가 필드 및 를 전달할 수 `ExecuteNow` `QueryStartTime` `QueryEndTime` 있습니다. 이러한 두 필드는 `TIMESPAN` 쿼리의 필드를 재정의합니다. 이러한 필드는 데이터가 변경되지 않는 고정된 기간 동안 지속적으로 생성되기 때문에 예약된 보고서에는 적용되지 않습니다.

### <a name="request-syntax"></a>요청 구문

|    방법     |    요청 URI     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>요청 헤더

|    헤더     |    유형     |    Description     |
|-------|-----|------|
|    권한 부여     |    문자열 |필수 요소. Azure AD(Azure Active Directory) 액세스 토큰입니다. 형식은  `Bearer <token>` 입니다.|
|    콘텐츠 형식     |문자열 |`Application/JSON` |

### <a name="path-parameter"></a>경로 매개 변수

None

### <a name="query-parameter"></a>쿼리 매개 변수

None

### <a name="sample-request-payload"></a>샘플 요청 페이로드

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>용어

요청 페이로드의 요소에 대한 주요 정의는 다음과 같습니다.

|    매개 변수     |    필수     |    Description     |    허용되는 값     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    예     |    보고서에 할당할 이름     |    문자열     |
|    설명     |    아니요     |    생성된 보고서에 대한 설명     |    문자열     |
|    QueryId     |    예     |    보고서 쿼리 ID     |    문자열     |
|    StartTime     |    예     |    보고서 생성이 시작되는 UTC 타임스탬프입니다. <br> yyyy-MM-ddTHH:mm:ssZ 형식이어야 합니다.       |    문자열     |
|    ExecuteNow     |    아니요     |    이 매개 변수는 한 번만 실행되는 보고서를 만드는 데 사용해야 합니다. `StartTime`, `RecurrenceInterval` 및 `RecurrenceCount` 는 true로 설정된 경우 무시됩니다. 보고서는 비동기 방식으로 즉시 실행됩니다.     |    true/false     |
|    QueryStartTime     |    아니요     |    필요에 따라 데이터를 추출하는 쿼리의 시작 시간을 지정합니다. 이 매개 변수는 true로 설정된 일회성 실행 보고서에만 `ExecuteNow` 적용됩니다. 이 매개 변수를 설정 하면 `TIMESPAN` 쿼리에 지정 된 재정의 합니다. yyyy-MM-ddTHH:mm:ssZ 형식이어야 합니다.     |    문자열 타임스탬프     |
|    QueryEndTime     |    아니요     |    필요에 따라 데이터를 추출하는 쿼리의 종료 시간을 지정합니다. 이 매개 변수는 true로 설정된 일회성 실행 보고서에만 `ExecuteNow` 적용됩니다. 이 매개 변수를 설정 하면 `TIMESPAN` 쿼리에 지정 된 재정의 합니다. yyyy-MM-ddTHH:mm:ssZ 형식이어야 합니다.     |    문자열 타임스탬프     |
|    RecurrenceInterval     |    예     |    보고서가 생성되어야 하는 빈도(시간)입니다. <br> 최소값은 4이고 최대값은 2160입니다.      |    integer     |
|    RecurrenceCount     |    아니요     |    생성할 보고서 수입니다.     |    정수     |
|    형식     |    아니요     |    내보낸 파일의 파일 형식입니다. <br> 기본값은 CSV입니다.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    아니요     |    선택적으로 콜백 대상으로 구성할 수 있는 공개적으로 연결할 수 있는 URL     |    문자열(http URL)     |
|    CallbackMethod     |    아니요     |    콜백에 사용할 메서드     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>샘플 응답

응답 페이로드는 다음과 같이 구성됩니다.

응답 코드: 200, 400, 401, 403, 404, 500

응답 페이로드 예제:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>용어

응답의 요소에 대 한 주요 정의는 아래와 같습니다.

|    매개 변수     |    Description     |
|    ----    |    ----    |
|    ReportId     |    만든 보고서의 UUID(범용 고유 식별자)     |
|    ReportName     |    요청 페이로드의 보고서에 지정된 이름     |
|    Description     |    보고서를 만드는 동안 제공된 설명     |
|    QueryId     |    보고서를 만들 때 전달된 쿼리 ID     |
|    쿼리     |    이 보고서에 대해 실행되는 쿼리 텍스트     |
|    사용자     |    보고서를 만드는 데 사용되는 사용자 ID     |
|    CreatedTime     |    보고서가 생성된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)     |
|    ModifiedTime     |    보고서가 마지막으로 수정된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)     |
|    ExecuteNow     |    `ExecuteNow` 보고서를 만들 때 설정 되는 플래그입니다.     |
|    StartTime     |    보고서 실행이 시작되는 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)     |
|    ReportStatus     |    보고서 실행 상태입니다. 가능한 값은 `Paused` , `Active` 및입니다. `Inactive`     |
|    RecurrenceInterval     |    보고서를 만드는 동안 제공된 되풀이 간격     |
|    RecurrenceCount     |    보고서를 만드는 동안 제공된 되풀이 수입니다.      |
|    콜백 url     |    요청에 제공된 콜백 URL     |
|    CallbackMethod     |    요청에 제공 된 콜백 메서드입니다.     |
|    서식     |    보고서 파일의 형식입니다. 가능한 값은 `CSV` 또는 `TSV` 입니다.     |
|    TotalCount     |    값 배열에 있는 레코드 수     |
|    StatusCode     |    결과 코드     |
|    message     |    가능한 값은 200, 400, 401, 403, 500입니다. API 실행의 상태 메시지     |
|        |        |

## <a name="get-report-execution-api"></a>보고서 실행 API 가져오기

이 메서드를 사용 하 여 [보고서 만들기 API](#create-report-api)에서 받은 보고서 id를 사용 하 여 보고서 실행 상태를 쿼리할 수 있습니다. 이 메서드는 보고서를 다운로드할 준비가 된 경우 보고서 다운로드 링크를 반환합니다. 그렇지 않으면 메서드가 상태를 반환합니다. 또한 이 API를 사용하여 특정 보고서에 대해 발생한 모든 실행을 가져올 수도 있습니다.  

>[!IMPORTANT]
>이 API에는 및에 대해 설정 된 기본 쿼리 매개 변수가 있습니다 `executionStatus=Completed` `getLatestExecution=true` . 따라서 보고서 실행이 처음으로 성공하기 전에 API를 호출하면 404가 반환됩니다. `executionStatus=Pending`을 설정하여 보류 중인 실행을 가져올 수 있습니다.

### <a name="request-syntax"></a>요청 구문

|    방법     |    요청 URI     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>요청 헤더

|    헤더     |    유형     |    Description     |
|-------|-----|------|
|    권한 부여     |    문자열 |필수 요소. Azure AD(Azure Active Directory) 액세스 토큰입니다. 형식은  `Bearer <token>` 입니다.|
|    콘텐츠 형식     |문자열 |`Application/JSON` |

### <a name="path-parameter"></a>경로 매개 변수

|    매개 변수 이름    |    필수    |    Type    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    예    |    문자열    |    이 인수에 지정 된 보고서 id를 사용 하는 보고서의 실행 세부 정보를 가져오려면 필터를 사용 합니다. 여러 reportIds를 세미콜론 ";"으로 구분 하 여 지정할 수 있습니다.    |
|        |        |        |        |

### <a name="query-parameter"></a>쿼리 매개 변수

|    매개 변수 이름    |    필수    |    Type    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    예    |    문자열    |    이 인수에 지정 된 executionId를 사용 하 여 보고서의 세부 정보만 가져오도록 필터링 합니다. 여러 executionIds는 세미콜론 ";"으로 구분 하 여 지정할 수 있습니다.    |
|    executionStatus    |    아니요    |    문자열/열거형    |    이 인수에 지정 된 executionStatus를 사용 하 여 보고서의 세부 정보만 가져오도록 필터링 합니다. <br> 유효한 값은 `Pending` , `Running` `Paused` 및 `Completed` 입니다. <br> 기본값은 `Completed`입니다. <br> 여러 상태를 세미콜론 (";")으로 구분 하 여 지정할 수 있습니다.    |
|    getLatestExecution    |    아니요    |    boolean    |    API는 최신 실행에 대 한 세부 정보를 반환 합니다. 이 매개 변수는 기본적으로 true로 설정 됩니다.<br> 이 매개 변수 값을 false로 전달 하도록 선택 하면 API는 최근 90 일 실행 인스턴스를 반환 합니다.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>샘플 요청 페이로드

None

### <a name="sample-response"></a>샘플 응답

응답 페이로드는 다음과 같이 구성됩니다.

응답 코드: 200, 400, 401, 403, 404, 500

응답 페이로드 예제:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

보고서 실행이 완료되면 실행 상태 `Completed`가 표시됩니다. `reportAccessSecureLink`에서 URL을 선택하여 보고서를 다운로드할 수 있습니다.

### <a name="glossary"></a>용어

응답에 있는 요소의 주요 정의입니다.

|    매개 변수    |    Description    |
|    ----    |    ----    |
|    ExecutionId    |    실행 인스턴스의 UUID(범용 고유 식별자)    |
|    ReportId    |    실행 인스턴스와 연결된 보고서 ID    |
|    RecurrenceInterval    |    보고서를 만드는 동안 제공된 되풀이 간격    |
|    RecurrenceCount    |    보고서를 만드는 동안 제공된 되풀이 수    |
|    콜백 url    |    실행 인스턴스와 연결된 콜백 URL    |
|    CallbackMethod    |    실행 인스턴스와 연결 된 콜백 메서드입니다.    |
|    서식    |    실행이 끝날 때 생성된 파일의 형식    |
|    ExecutionStatus    |    보고서 실행 인스턴스의 상태입니다. <br> 유효한 값은 `Pending`, `Running`, `Paused` 및 `Completed`입니다.    |
|    ReportAccessSecureLink    |보고서에 안전하게 액세스하는 데 사용할 수 있는 링크        |
|    ReportExpiryTime    |    보고서 링크가 만료되는 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)    |
|    ReportGeneratedTime    |    보고서가 생성된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)    |
|    TotalCount    |    값 배열의 데이터 세트 수    |
|    StatusCode    |    결과 코드 <br> 가능한 값은 200, 400, 401, 403, 404 및 500입니다.    |
|    message    |    API 실행의 상태 메시지    |
|        |        |

## <a name="next-steps"></a>다음 단계

- [SWAGGER API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) 을 통해 api 사용해 보기
- [첫 번째 API 호출 만들기](insights-programmatic-first-api-call.md)