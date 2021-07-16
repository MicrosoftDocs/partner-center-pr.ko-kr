---
title: 파트너 insights 분석 데이터에 액세스 하기 위한 첫 번째 API 호출 만들기
description: API를 사용 하 여 파트너 insights 분석 데이터에 액세스 하는 방법을 배울 수 있는 예입니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375868"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>파트너 insights 분석 데이터에 액세스 하기 위한 첫 번째 API 호출 만들기

파트너 insights 분석 데이터에 액세스 하기 위한 Api 목록은 [partner insights 분석 데이터에 액세스 하기 위한 api](insights-programmatic-analytics-available-api.md)를 참조 하세요. 첫 번째 API 호출을 수행 하기 전에 파트너 Insights 분석 데이터에 프로그래밍 방식으로 액세스 하기 위한 [필수](insights-programmatic-prerequisites.md) 구성 요소를 충족 하는지 확인 합니다.

## <a name="token-generation"></a>토큰 생성

메서드를 호출 하기 전에 먼저 AAD (Azure Active Directory) 액세스 토큰을 가져와야 합니다. API에서 각 메서드의 인증 헤더에 Azure AD 액세스 토큰을 전달해야 합니다. 액세스 토큰을 얻은 후 만료되기 전에 60분 동안 사용할 수 있습니다. 토큰이 만료 되 면 토큰을 새로 고칠 수 있으며 API에 대 한 추가 호출에 토큰을 계속 사용할 수 있습니다.

토큰을 생성하는 방법에 관한 샘플 요청은 아래를 참조하세요. 토큰을 생성하는 데 필요한 세 가지 값은 `clientId`, `clientSecret` 및 `tenantId`입니다. 리소스 매개 변수를로 설정 해야 합니다. `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>요청 예제

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>응답 예제

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

응용 프로그램에 대 한 Azure AD 토큰을 얻는 방법에 대 한 자세한 내용은 [스토어 서비스를 사용 하 여 분석 데이터 액세스](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token) 를 참조 하세요.

## <a name="programmatic-api-call"></a>프로그래매틱 API 호출

이전 섹션에 설명 된 대로 AAD 토큰을 가져온 후에는 다음 단계에 따라 첫 번째 프로그래밍 방식 액세스 보고서를 만듭니다.

다음 데이터 세트(datasetName)에서 데이터를 다운로드할 수 있습니다.

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- Azureusage.xls
- MSLearn
- 인 오피스 사용
- 프로필
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

다음 섹션에서는 `SubscriptionId` DynamicsUsage 데이터 집합에서 프로그래밍 방식으로 액세스 하는 방법에 대 한 예제를 제공 합니다.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>1 단계: 데이터 집합 가져오기 API를 사용 하 여 REST 호출

API 응답은 보고서를 다운로드할 수 있는 데이터 세트 이름을 제공합니다. 특정 데이터 세트의 경우 API 응답은 사용자 지정 보고서 템플릿에 사용할 수 있는 선택 가능한 열 목록도 제공합니다. [데이터 정의](insights-data-definitions.md) 를 참조 하 여 열의 이름을 가져올 수도 있습니다.

#### <a name="request-example"></a>요청 예제

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>응답 예제

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>2 단계: 사용자 지정 쿼리 만들기

이 단계에서는 DynamicsUsage 데이터 집합에서 SubscriptionId를 사용 하 여 원하는 보고서에 대 한 사용자 지정 쿼리를 만듭니다. 쿼리에 지정 되지 않은 경우 기본 timespan은 6 개월입니다.

#### <a name="request-example"></a>요청 예제

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>응답 예제

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

쿼리가 성공적으로 실행되면 보고서를 생성하는 데 사용해야 하는 `queryId`가 생성됩니다.

### <a name="step-3-execute-test-query-api"></a>3단계: 테스트 쿼리 API 실행

이 단계에서는 테스트 쿼리 API를 사용 하 여 생성 된 쿼리에 대 한 상위 100 행을 가져옵니다.

#### <a name="request-example"></a>요청 예제

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>응답 예제

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>4단계: 보고서 만들기

이 단계에서는 이전에 생성 된 QueryId를 사용 하 여 보고서를 만듭니다.

#### <a name="request-example"></a>요청 예제

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>응답 예제

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
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

성공적으로 실행되면 보고서의 다운로드를 예약하는 데 사용해야 하는 `reportId`가 생성됩니다.

### <a name="step-5-execute-report-executions-api"></a>5단계: 보고서 실행 API 실행

이 단계에서는 보고서 실행 API를 사용 하 여 보고서의 보안 위치 (URL)를 가져옵니다.

#### <a name="request-example"></a>요청 예제

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>응답 예제

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>다음 단계

- [SWAGGER API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) 을 통해 api 사용해 보기