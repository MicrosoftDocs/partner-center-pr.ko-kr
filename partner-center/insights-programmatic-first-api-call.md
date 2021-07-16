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
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a><span data-ttu-id="c7274-103">파트너 insights 분석 데이터에 액세스 하기 위한 첫 번째 API 호출 만들기</span><span class="sxs-lookup"><span data-stu-id="c7274-103">Make your first API call to access partner insights analytics data</span></span>

<span data-ttu-id="c7274-104">파트너 insights 분석 데이터에 액세스 하기 위한 Api 목록은 [partner insights 분석 데이터에 액세스 하기 위한 api](insights-programmatic-analytics-available-api.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c7274-104">For a list of the APIs for accessing partner insights analytics data, see [APIs for accessing partner insights analytics data](insights-programmatic-analytics-available-api.md).</span></span> <span data-ttu-id="c7274-105">첫 번째 API 호출을 수행 하기 전에 파트너 Insights 분석 데이터에 프로그래밍 방식으로 액세스 하기 위한 [필수](insights-programmatic-prerequisites.md) 구성 요소를 충족 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-105">Before you make your first API call, make sure that you met the [pre-requisites](insights-programmatic-prerequisites.md) to programmatically access Partner Insights analytics data.</span></span>

## <a name="token-generation"></a><span data-ttu-id="c7274-106">토큰 생성</span><span class="sxs-lookup"><span data-stu-id="c7274-106">Token generation</span></span>

<span data-ttu-id="c7274-107">메서드를 호출 하기 전에 먼저 AAD (Azure Active Directory) 액세스 토큰을 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-107">Before calling any of the methods, you must first obtain an Azure Active Directory (AAD) access token.</span></span> <span data-ttu-id="c7274-108">API에서 각 메서드의 인증 헤더에 Azure AD 액세스 토큰을 전달해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-108">You need to pass the Azure AD access token to the Authorization header of each method in the API.</span></span> <span data-ttu-id="c7274-109">액세스 토큰을 얻은 후 만료되기 전에 60분 동안 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-109">After obtaining an access token, you have 60 minutes to use it before it expires.</span></span> <span data-ttu-id="c7274-110">토큰이 만료 되 면 토큰을 새로 고칠 수 있으며 API에 대 한 추가 호출에 토큰을 계속 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-110">After the token expires, you can refresh the token and can continue to use it for further calls to the API.</span></span>

<span data-ttu-id="c7274-111">토큰을 생성하는 방법에 관한 샘플 요청은 아래를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c7274-111">Refer to a sample request below for generating a token.</span></span> <span data-ttu-id="c7274-112">토큰을 생성하는 데 필요한 세 가지 값은 `clientId`, `clientSecret` 및 `tenantId`입니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-112">The three values that are required to generate the token are `clientId`, `clientSecret`, and `tenantId`.</span></span> <span data-ttu-id="c7274-113">리소스 매개 변수를로 설정 해야 합니다. `https://api.partnercenter.microsoft.com`</span><span class="sxs-lookup"><span data-stu-id="c7274-113">The resource parameter should be set to `https://api.partnercenter.microsoft.com`</span></span>

#### <a name="request-example"></a><span data-ttu-id="c7274-114">요청 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-114">Request example</span></span>

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

#### <a name="response-example"></a><span data-ttu-id="c7274-115">응답 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-115">Response example</span></span>

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

<span data-ttu-id="c7274-116">응용 프로그램에 대 한 Azure AD 토큰을 얻는 방법에 대 한 자세한 내용은 [스토어 서비스를 사용 하 여 분석 데이터 액세스](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c7274-116">For more information about how to obtain an Azure AD token for your application, see [Access analytics data using Store services.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span></span>

## <a name="programmatic-api-call"></a><span data-ttu-id="c7274-117">프로그래매틱 API 호출</span><span class="sxs-lookup"><span data-stu-id="c7274-117">Programmatic API call</span></span>

<span data-ttu-id="c7274-118">이전 섹션에 설명 된 대로 AAD 토큰을 가져온 후에는 다음 단계에 따라 첫 번째 프로그래밍 방식 액세스 보고서를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-118">After you obtain the AAD Token as described in the previous section, follow these steps to create your first programmatic access report.</span></span>

<span data-ttu-id="c7274-119">다음 데이터 세트(datasetName)에서 데이터를 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-119">Data can be downloaded from the following datasets (datasetName):</span></span>

- <span data-ttu-id="c7274-120">CustomersAndTenants</span><span class="sxs-lookup"><span data-stu-id="c7274-120">CustomersAndTenants</span></span>
- <span data-ttu-id="c7274-121">SeatsSubscriptionsAndRevenue</span><span class="sxs-lookup"><span data-stu-id="c7274-121">SeatsSubscriptionsAndRevenue</span></span>
- <span data-ttu-id="c7274-122">Azureusage.xls</span><span class="sxs-lookup"><span data-stu-id="c7274-122">AzureUsage</span></span>
- <span data-ttu-id="c7274-123">MSLearn</span><span class="sxs-lookup"><span data-stu-id="c7274-123">MSLearn</span></span>
- <span data-ttu-id="c7274-124">인 오피스 사용</span><span class="sxs-lookup"><span data-stu-id="c7274-124">OfficeUsage</span></span>
- <span data-ttu-id="c7274-125">프로필</span><span class="sxs-lookup"><span data-stu-id="c7274-125">Profile</span></span>
- <span data-ttu-id="c7274-126">TrainingCompletions</span><span class="sxs-lookup"><span data-stu-id="c7274-126">TrainingCompletions</span></span>
- <span data-ttu-id="c7274-127">DynamicsUsage</span><span class="sxs-lookup"><span data-stu-id="c7274-127">DynamicsUsage</span></span>
- <span data-ttu-id="c7274-128">CompetencySummaryHistory</span><span class="sxs-lookup"><span data-stu-id="c7274-128">CompetencySummaryHistory</span></span>
- <span data-ttu-id="c7274-129">PowerBIUsage</span><span class="sxs-lookup"><span data-stu-id="c7274-129">PowerBIUsage</span></span>
- <span data-ttu-id="c7274-130">EMSUsage</span><span class="sxs-lookup"><span data-stu-id="c7274-130">EMSUsage</span></span>
- <span data-ttu-id="c7274-131">CompetencyPeformanceRequirement</span><span class="sxs-lookup"><span data-stu-id="c7274-131">CompetencyPeformanceRequirement</span></span>
- <span data-ttu-id="c7274-132">ResellerPerformance</span><span class="sxs-lookup"><span data-stu-id="c7274-132">ResellerPerformance</span></span>
- <span data-ttu-id="c7274-133">CLASAgreementRenewalsPropensity</span><span class="sxs-lookup"><span data-stu-id="c7274-133">CLASAgreementRenewalsPropensity</span></span>
- <span data-ttu-id="c7274-134">CLASAzurePropensity</span><span class="sxs-lookup"><span data-stu-id="c7274-134">CLASAzurePropensity</span></span>
- <span data-ttu-id="c7274-135">CLASD365Propensity</span><span class="sxs-lookup"><span data-stu-id="c7274-135">CLASD365Propensity</span></span>
- <span data-ttu-id="c7274-136">CLASM365Propensity</span><span class="sxs-lookup"><span data-stu-id="c7274-136">CLASM365Propensity</span></span>
- <span data-ttu-id="c7274-137">TeamsUsage3PApps</span><span class="sxs-lookup"><span data-stu-id="c7274-137">TeamsUsage3PApps</span></span>
- <span data-ttu-id="c7274-138">TeamsUsageWorkload</span><span class="sxs-lookup"><span data-stu-id="c7274-138">TeamsUsageWorkload</span></span>
- <span data-ttu-id="c7274-139">TeamsUsageMeetingsAndCalls</span><span class="sxs-lookup"><span data-stu-id="c7274-139">TeamsUsageMeetingsAndCalls</span></span>

<span data-ttu-id="c7274-140">다음 섹션에서는 `SubscriptionId` DynamicsUsage 데이터 집합에서 프로그래밍 방식으로 액세스 하는 방법에 대 한 예제를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-140">In the following section, we will see examples of how to programmatically access `SubscriptionId` from the DynamicsUsage dataset.</span></span>

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a><span data-ttu-id="c7274-141">1 단계: 데이터 집합 가져오기 API를 사용 하 여 REST 호출</span><span class="sxs-lookup"><span data-stu-id="c7274-141">Step 1: Make a REST call using the get datasets API</span></span>

<span data-ttu-id="c7274-142">API 응답은 보고서를 다운로드할 수 있는 데이터 세트 이름을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-142">The API response provides the dataset name from where you can download the report.</span></span> <span data-ttu-id="c7274-143">특정 데이터 세트의 경우 API 응답은 사용자 지정 보고서 템플릿에 사용할 수 있는 선택 가능한 열 목록도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-143">For the specific dataset, the API response also provides the list of selectable columns that can be used for your custom report template.</span></span> <span data-ttu-id="c7274-144">[데이터 정의](insights-data-definitions.md) 를 참조 하 여 열의 이름을 가져올 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-144">You can also refer to the [Data Definitions](insights-data-definitions.md) to get the names of the columns.</span></span>

#### <a name="request-example"></a><span data-ttu-id="c7274-145">요청 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-145">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="c7274-146">응답 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-146">Response example</span></span>

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

### <a name="step-2-create-the-custom-query"></a><span data-ttu-id="c7274-147">2 단계: 사용자 지정 쿼리 만들기</span><span class="sxs-lookup"><span data-stu-id="c7274-147">Step 2: Create the Custom Query</span></span>

<span data-ttu-id="c7274-148">이 단계에서는 DynamicsUsage 데이터 집합에서 SubscriptionId를 사용 하 여 원하는 보고서에 대 한 사용자 지정 쿼리를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-148">In this step, we will use SubscriptionId from the DynamicsUsage dataset to create a custom query for the report we want.</span></span> <span data-ttu-id="c7274-149">쿼리에 지정 되지 않은 경우 기본 timespan은 6 개월입니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-149">The default timespan if not specified in the query is 6 months.</span></span>

#### <a name="request-example"></a><span data-ttu-id="c7274-150">요청 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-150">Request example</span></span>

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

#### <a name="response-example"></a><span data-ttu-id="c7274-151">응답 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-151">Response example</span></span>

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

<span data-ttu-id="c7274-152">쿼리가 성공적으로 실행되면 보고서를 생성하는 데 사용해야 하는 `queryId`가 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-152">On successful execution of the query, a `queryId` is generated that needs to be used to generate the report.</span></span>

### <a name="step-3-execute-test-query-api"></a><span data-ttu-id="c7274-153">3단계: 테스트 쿼리 API 실행</span><span class="sxs-lookup"><span data-stu-id="c7274-153">Step 3: Execute test query API</span></span>

<span data-ttu-id="c7274-154">이 단계에서는 테스트 쿼리 API를 사용 하 여 생성 된 쿼리에 대 한 상위 100 행을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-154">In this step, we will use the test query API to get the top 100 rows for the query that was created.</span></span>

#### <a name="request-example"></a><span data-ttu-id="c7274-155">요청 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-155">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="c7274-156">응답 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-156">Response example</span></span>

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

### <a name="step-4-create-the-report"></a><span data-ttu-id="c7274-157">4단계: 보고서 만들기</span><span class="sxs-lookup"><span data-stu-id="c7274-157">Step 4: Create the report</span></span>

<span data-ttu-id="c7274-158">이 단계에서는 이전에 생성 된 QueryId를 사용 하 여 보고서를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-158">In this step, we will use the previously generated QueryId to create the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="c7274-159">요청 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-159">Request example</span></span>

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

#### <a name="response-example"></a><span data-ttu-id="c7274-160">응답 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-160">Response example</span></span>

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

<span data-ttu-id="c7274-161">성공적으로 실행되면 보고서의 다운로드를 예약하는 데 사용해야 하는 `reportId`가 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-161">On successful execution, a `reportId` is generated that needs to be used to schedule a download of the report.</span></span>

### <a name="step-5-execute-report-executions-api"></a><span data-ttu-id="c7274-162">5단계: 보고서 실행 API 실행</span><span class="sxs-lookup"><span data-stu-id="c7274-162">Step 5: Execute Report Executions API</span></span>

<span data-ttu-id="c7274-163">이 단계에서는 보고서 실행 API를 사용 하 여 보고서의 보안 위치 (URL)를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c7274-163">In this step, we will use the Report Executions API to get the secure location (URL) of the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="c7274-164">요청 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-164">Request example</span></span>

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a><span data-ttu-id="c7274-165">응답 예제</span><span class="sxs-lookup"><span data-stu-id="c7274-165">Response example</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="c7274-166">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c7274-166">Next steps</span></span>

- <span data-ttu-id="c7274-167">[SWAGGER API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) 을 통해 api 사용해 보기</span><span class="sxs-lookup"><span data-stu-id="c7274-167">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>