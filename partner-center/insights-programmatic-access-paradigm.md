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
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="2a4f9-104">프로그래밍 방식 액세스 페러다임</span><span class="sxs-lookup"><span data-stu-id="2a4f9-104">Programmatic access paradigm</span></span>

<span data-ttu-id="2a4f9-105">이 다이어그램에서는 새 보고서 템플릿을 만들고, 사용자 지정 보고서를 예약 하 고, 오류 데이터를 검색 하는 데 사용 되는 API 호출 패턴을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="상위 수준 흐름":::
<span data-ttu-id="2a4f9-107">***그림 1: API 호출 패턴의 높은 수준 흐름***</span><span class="sxs-lookup"><span data-stu-id="2a4f9-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="2a4f9-108">이 목록에는 그림 1에 대한 자세한 내용이 나와 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="2a4f9-109">클라이언트 애플리케이션은 [보고서 쿼리 만들기 API](#create-report-query-api)를 호출하여 사용자 지정 보고서 스키마/템플릿을 정의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="2a4f9-110">또는 여기에 나열 된 보고서 템플릿 라이브러리 샘플에서 보고서 템플릿 (QueryId)을 선택할 수 있습니다 [.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="2a4f9-111">성공 하면 보고서 만들기 쿼리 API가 QueryId를 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="2a4f9-112">그런 다음 클라이언트 응용 프로그램은 보고서 시작 날짜, 반복 간격, 되풀이 및 선택적 콜백 URI와 함께 QueryId를 사용 하 여 [보고서 만들기 API](#create-report-api) 를 호출 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="2a4f9-113">성공 하면 [보고서 만들기 API](#create-report-api) 가 보고서 id를 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="2a4f9-114">클라이언트 응용 프로그램은 보고서 데이터를 다운로드할 준비가 되는 즉시 콜백 URL에 대 한 알림 메시지를 받습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="2a4f9-115">그러면 클라이언트 응용 프로그램에서 보고서 [실행 API 가져오기 API](#get-report-execution-api) 를 사용 하 여 보고서 ID 및 날짜 범위로 보고서 상태를 쿼리 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="2a4f9-116">성공 시 보고서 다운로드 링크가 반환되고 애플리케이션에서 데이터 다운로드를 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="2a4f9-117">보고서 쿼리 언어 사양</span><span class="sxs-lookup"><span data-stu-id="2a4f9-117">Report query language specification</span></span>

<span data-ttu-id="2a4f9-118">보고서를 만드는 데 사용할 수 있는 [시스템 쿼리](insights-programmatic-system-queries.md) 를 제공 하지만 비즈니스 요구 사항에 따라 고유한 쿼리를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="2a4f9-119">사용자 지정 쿼리에 대 한 자세한 내용은 [사용자 지정 쿼리 사양](insights-programmatic-custom-query.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="2a4f9-120">보고서 쿼리 만들기 API</span><span class="sxs-lookup"><span data-stu-id="2a4f9-120">Create report query API</span></span>

<span data-ttu-id="2a4f9-121">API를 사용 하면 열과 메트릭을 내보내야 하는 데이터 집합을 정의 하는 사용자 지정 쿼리를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="2a4f9-122">이 API는 비즈니스 요구에 따라 새 보고 템플릿을 만들 수 있는 유연성을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="2a4f9-123">기본 제공되는 [시스템 쿼리](insights-programmatic-system-queries.md)를 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="2a4f9-124">사용자 지정 보고서 템플릿이 필요 하지 않은 경우 제공 된 시스템 쿼리의 QueryIds를 사용 하 여 직접 [Create REPORT API](#create-report-api) 를 호출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="2a4f9-125">다음 예에서는 지난 달의 수익을 기준으로 상위 10 명의 고객을 가져오는 사용자 지정 쿼리를 만드는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="2a4f9-126">요청 구문</span><span class="sxs-lookup"><span data-stu-id="2a4f9-126">Request syntax</span></span>

|    <span data-ttu-id="2a4f9-127">방법</span><span class="sxs-lookup"><span data-stu-id="2a4f9-127">Method</span></span>     |    <span data-ttu-id="2a4f9-128">요청 URI</span><span class="sxs-lookup"><span data-stu-id="2a4f9-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="2a4f9-129">POST</span><span class="sxs-lookup"><span data-stu-id="2a4f9-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="2a4f9-130">요청 헤더</span><span class="sxs-lookup"><span data-stu-id="2a4f9-130">Request header</span></span>

|    <span data-ttu-id="2a4f9-131">헤더</span><span class="sxs-lookup"><span data-stu-id="2a4f9-131">Header</span></span>     |    <span data-ttu-id="2a4f9-132">유형</span><span class="sxs-lookup"><span data-stu-id="2a4f9-132">Type</span></span>     |    <span data-ttu-id="2a4f9-133">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="2a4f9-134">권한 부여</span><span class="sxs-lookup"><span data-stu-id="2a4f9-134">Authorization</span></span>     |    <span data-ttu-id="2a4f9-135">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-135">string</span></span> |<span data-ttu-id="2a4f9-136">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-136">Required.</span></span> <span data-ttu-id="2a4f9-137">Azure AD(Azure Active Directory) 액세스 토큰입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="2a4f9-138">형식은  `Bearer <token>` 입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="2a4f9-139">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-139">Content-Type</span></span>     |<span data-ttu-id="2a4f9-140">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="2a4f9-141">경로 매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-141">Path parameter</span></span>

<span data-ttu-id="2a4f9-142">None</span><span class="sxs-lookup"><span data-stu-id="2a4f9-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="2a4f9-143">쿼리 매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-143">Query parameter</span></span>

<span data-ttu-id="2a4f9-144">None</span><span class="sxs-lookup"><span data-stu-id="2a4f9-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="2a4f9-145">샘플 요청 페이로드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="2a4f9-146">용어</span><span class="sxs-lookup"><span data-stu-id="2a4f9-146">Glossary</span></span>

<span data-ttu-id="2a4f9-147">이 표에는 요청 페이로드에 있는 요소의 주요 정의가 나열되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="2a4f9-148">매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-148">Parameter</span></span>|    <span data-ttu-id="2a4f9-149">필수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-149">Required</span></span>     |    <span data-ttu-id="2a4f9-150">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-150">Description</span></span>     |    <span data-ttu-id="2a4f9-151">허용되는 값</span><span class="sxs-lookup"><span data-stu-id="2a4f9-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="2a4f9-152">이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-152">Name</span></span> |    <span data-ttu-id="2a4f9-153">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-153">Yes</span></span>     |    <span data-ttu-id="2a4f9-154">쿼리의 식별 이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-154">Friendly name of the query</span></span>     |    <span data-ttu-id="2a4f9-155">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-155">string</span></span>     |
|    <span data-ttu-id="2a4f9-156">설명</span><span class="sxs-lookup"><span data-stu-id="2a4f9-156">Description</span></span>     |    <span data-ttu-id="2a4f9-157">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-157">No</span></span>     |    <span data-ttu-id="2a4f9-158">쿼리가 반환하는 내용에 대한 설명</span><span class="sxs-lookup"><span data-stu-id="2a4f9-158">Description of what the query returns</span></span>     |    <span data-ttu-id="2a4f9-159">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-159">string</span></span>     |
|    <span data-ttu-id="2a4f9-160">쿼리</span><span class="sxs-lookup"><span data-stu-id="2a4f9-160">Query</span></span>     |    <span data-ttu-id="2a4f9-161">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-161">Yes</span></span>     |    <span data-ttu-id="2a4f9-162">보고서 쿼리 문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-162">Report query string</span></span>     |    <span data-ttu-id="2a4f9-163">데이터 형식: 문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-163">Data type: string</span></span> <br> <span data-ttu-id="2a4f9-164">비즈니스 요구 사항에 따른 [사용자 지정 쿼리](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="2a4f9-165">사용자 지정 쿼리 예제는 [샘플 쿼리 예제](insights-programmatic-sample-queries.md) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="2a4f9-166">샘플 응답</span><span class="sxs-lookup"><span data-stu-id="2a4f9-166">Sample response</span></span>

<span data-ttu-id="2a4f9-167">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="2a4f9-168">응답 코드: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="2a4f9-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="2a4f9-169">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="2a4f9-169">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="2a4f9-170">용어</span><span class="sxs-lookup"><span data-stu-id="2a4f9-170">Glossary</span></span>

<span data-ttu-id="2a4f9-171">이 표에는 요청 페이로드에 있는 요소의 주요 정의가 나열되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="2a4f9-172">매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-172">Parameter</span></span>     |    <span data-ttu-id="2a4f9-173">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="2a4f9-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-174">QueryId</span></span>     |    <span data-ttu-id="2a4f9-175">만든 쿼리의 UUID(범용 고유 식별자)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="2a4f9-176">이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-176">Name</span></span>     |    <span data-ttu-id="2a4f9-177">요청 페이로드의 쿼리에 지정된 식별 이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="2a4f9-178">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-178">Description</span></span>     |    <span data-ttu-id="2a4f9-179">쿼리를 만드는 동안 제공된 설명</span><span class="sxs-lookup"><span data-stu-id="2a4f9-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="2a4f9-180">쿼리</span><span class="sxs-lookup"><span data-stu-id="2a4f9-180">Query</span></span>     |    <span data-ttu-id="2a4f9-181">쿼리를 만드는 동안 입력으로 전달된 보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="2a4f9-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="2a4f9-182">유형</span><span class="sxs-lookup"><span data-stu-id="2a4f9-182">Type</span></span>     |    <span data-ttu-id="2a4f9-183">`userDefined`</span><span class="sxs-lookup"><span data-stu-id="2a4f9-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="2a4f9-184">사용자</span><span class="sxs-lookup"><span data-stu-id="2a4f9-184">User</span></span>     |    <span data-ttu-id="2a4f9-185">쿼리를 만드는 데 사용 되는 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="2a4f9-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="2a4f9-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-186">CreatedTime</span></span>     |    <span data-ttu-id="2a4f9-187">쿼리가 생성된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2a4f9-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2a4f9-188">TotalCount</span></span>     |    <span data-ttu-id="2a4f9-189">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="2a4f9-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2a4f9-190">StatusCode</span></span>     |    <span data-ttu-id="2a4f9-191">결과 코드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-191">Result Code</span></span> <br> <span data-ttu-id="2a4f9-192">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="2a4f9-193">message</span><span class="sxs-lookup"><span data-stu-id="2a4f9-193">message</span></span>     |    <span data-ttu-id="2a4f9-194">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="2a4f9-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="2a4f9-195">보고서 만들기 API</span><span class="sxs-lookup"><span data-stu-id="2a4f9-195">Create report API</span></span>

<span data-ttu-id="2a4f9-196">[보고서 쿼리 응답 만들기](#create-report-query-api) 의 일부로 사용자 지정 보고서 템플릿을 만들고 QueryID를 수신 하는 경우이 API를 호출 하 여 정기적으로 실행 되도록 쿼리를 예약할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="2a4f9-197">보고서가 배달되는 빈도 및 일정을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="2a4f9-198">기본 제공되는 시스템 쿼리의 경우 [QueryId](insights-programmatic-system-queries.md)를 사용하여 보고서 만들기 API를 호출할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="2a4f9-199">콜백 URL</span><span class="sxs-lookup"><span data-stu-id="2a4f9-199">Callback URL</span></span>

<span data-ttu-id="2a4f9-200">보고서 만들기 API는 콜백 URL을 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="2a4f9-201">이 URL은 보고서 생성에 성공하면 호출됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="2a4f9-202">콜백 URL은 공개적으로 연결할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="2a4f9-203">URL 외에도 콜백 메서드를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="2a4f9-204">콜백 메서드는 "GET" 또는 "POST"만 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="2a4f9-205">값이 전달되지 않는 경우 기본 메서드는 "POST"입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="2a4f9-206">생성이 완료된 reportId는 콜백 중에 항상 다시 전달됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="2a4f9-207">POST 콜백: 전달된 URL이 `https://www.contosso.com/callback` 이면 호출된 URL은 입니다. `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="2a4f9-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="2a4f9-208">GET 콜백: 전달된 URL이 `https://www.contosso.com/callback` 이면 호출된 URL은 입니다. `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="2a4f9-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="2a4f9-209">ExecuteNow 보고서</span><span class="sxs-lookup"><span data-stu-id="2a4f9-209">ExecuteNow reports</span></span>

<span data-ttu-id="2a4f9-210">예약하지 않고 보고서를 생성하는 프로비전이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="2a4f9-211">보고서 만들기 API 페이로드는 매개 변수 를 수락할 수 있습니다. 이 매개 `ExecuteNow` 변수는 API가 호출되는 즉시 생성되는 보고서를 시차로 립니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="2a4f9-212">`ExecuteNow`이 true로 설정되면 `StartTime` , `RecurrenceCount` , `RecurrenceInterval` 필드가 무시됩니다. 이러한 보고서는 예약되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="2a4f9-213">가 true인 경우 두 개의 추가 필드 및 를 전달할 수 `ExecuteNow` `QueryStartTime` `QueryEndTime` 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="2a4f9-214">이러한 두 필드는 `TIMESPAN` 쿼리의 필드를 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="2a4f9-215">이러한 필드는 데이터가 변경되지 않는 고정된 기간 동안 지속적으로 생성되기 때문에 예약된 보고서에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="2a4f9-216">요청 구문</span><span class="sxs-lookup"><span data-stu-id="2a4f9-216">Request syntax</span></span>

|    <span data-ttu-id="2a4f9-217">방법</span><span class="sxs-lookup"><span data-stu-id="2a4f9-217">Method</span></span>     |    <span data-ttu-id="2a4f9-218">요청 URI</span><span class="sxs-lookup"><span data-stu-id="2a4f9-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="2a4f9-219">POST</span><span class="sxs-lookup"><span data-stu-id="2a4f9-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="2a4f9-220">요청 헤더</span><span class="sxs-lookup"><span data-stu-id="2a4f9-220">Request header</span></span>

|    <span data-ttu-id="2a4f9-221">헤더</span><span class="sxs-lookup"><span data-stu-id="2a4f9-221">Header</span></span>     |    <span data-ttu-id="2a4f9-222">유형</span><span class="sxs-lookup"><span data-stu-id="2a4f9-222">Type</span></span>     |    <span data-ttu-id="2a4f9-223">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="2a4f9-224">권한 부여</span><span class="sxs-lookup"><span data-stu-id="2a4f9-224">Authorization</span></span>     |    <span data-ttu-id="2a4f9-225">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-225">string</span></span> |<span data-ttu-id="2a4f9-226">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-226">Required.</span></span> <span data-ttu-id="2a4f9-227">Azure AD(Azure Active Directory) 액세스 토큰입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="2a4f9-228">형식은  `Bearer <token>` 입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="2a4f9-229">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-229">Content-Type</span></span>     |<span data-ttu-id="2a4f9-230">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="2a4f9-231">경로 매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-231">Path Parameter</span></span>

<span data-ttu-id="2a4f9-232">None</span><span class="sxs-lookup"><span data-stu-id="2a4f9-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="2a4f9-233">쿼리 매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-233">Query Parameter</span></span>

<span data-ttu-id="2a4f9-234">None</span><span class="sxs-lookup"><span data-stu-id="2a4f9-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="2a4f9-235">샘플 요청 페이로드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-235">Sample request payload</span></span>

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

### <a name="glossary"></a><span data-ttu-id="2a4f9-236">용어</span><span class="sxs-lookup"><span data-stu-id="2a4f9-236">Glossary</span></span>

<span data-ttu-id="2a4f9-237">요청 페이로드의 요소에 대한 주요 정의는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="2a4f9-238">매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-238">Parameter</span></span>     |    <span data-ttu-id="2a4f9-239">필수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-239">Required</span></span>     |    <span data-ttu-id="2a4f9-240">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-240">Description</span></span>     |    <span data-ttu-id="2a4f9-241">허용되는 값</span><span class="sxs-lookup"><span data-stu-id="2a4f9-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2a4f9-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="2a4f9-242">ReportName</span></span>     |    <span data-ttu-id="2a4f9-243">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-243">Yes</span></span>     |    <span data-ttu-id="2a4f9-244">보고서에 할당할 이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="2a4f9-245">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-245">string</span></span>     |
|    <span data-ttu-id="2a4f9-246">설명</span><span class="sxs-lookup"><span data-stu-id="2a4f9-246">Description</span></span>     |    <span data-ttu-id="2a4f9-247">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-247">No</span></span>     |    <span data-ttu-id="2a4f9-248">생성된 보고서에 대한 설명</span><span class="sxs-lookup"><span data-stu-id="2a4f9-248">Description of the created report</span></span>     |    <span data-ttu-id="2a4f9-249">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-249">string</span></span>     |
|    <span data-ttu-id="2a4f9-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-250">QueryId</span></span>     |    <span data-ttu-id="2a4f9-251">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-251">Yes</span></span>     |    <span data-ttu-id="2a4f9-252">보고서 쿼리 ID</span><span class="sxs-lookup"><span data-stu-id="2a4f9-252">Report query ID</span></span>     |    <span data-ttu-id="2a4f9-253">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-253">string</span></span>     |
|    <span data-ttu-id="2a4f9-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-254">StartTime</span></span>     |    <span data-ttu-id="2a4f9-255">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-255">Yes</span></span>     |    <span data-ttu-id="2a4f9-256">보고서 생성이 시작되는 UTC 타임스탬프입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="2a4f9-257">yyyy-MM-ddTHH:mm:ssZ 형식이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="2a4f9-258">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-258">string</span></span>     |
|    <span data-ttu-id="2a4f9-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2a4f9-259">ExecuteNow</span></span>     |    <span data-ttu-id="2a4f9-260">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-260">No</span></span>     |    <span data-ttu-id="2a4f9-261">이 매개 변수는 한 번만 실행되는 보고서를 만드는 데 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="2a4f9-262">`StartTime`, `RecurrenceInterval` 및 `RecurrenceCount` 는 true로 설정된 경우 무시됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="2a4f9-263">보고서는 비동기 방식으로 즉시 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="2a4f9-264">true/false</span><span class="sxs-lookup"><span data-stu-id="2a4f9-264">true/false</span></span>     |
|    <span data-ttu-id="2a4f9-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-265">QueryStartTime</span></span>     |    <span data-ttu-id="2a4f9-266">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-266">No</span></span>     |    <span data-ttu-id="2a4f9-267">필요에 따라 데이터를 추출하는 쿼리의 시작 시간을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="2a4f9-268">이 매개 변수는 true로 설정된 일회성 실행 보고서에만 `ExecuteNow` 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="2a4f9-269">이 매개 변수를 설정 하면 `TIMESPAN` 쿼리에 지정 된 재정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="2a4f9-270">yyyy-MM-ddTHH:mm:ssZ 형식이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="2a4f9-271">문자열 타임스탬프</span><span class="sxs-lookup"><span data-stu-id="2a4f9-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="2a4f9-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-272">QueryEndTime</span></span>     |    <span data-ttu-id="2a4f9-273">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-273">No</span></span>     |    <span data-ttu-id="2a4f9-274">필요에 따라 데이터를 추출하는 쿼리의 종료 시간을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="2a4f9-275">이 매개 변수는 true로 설정된 일회성 실행 보고서에만 `ExecuteNow` 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="2a4f9-276">이 매개 변수를 설정 하면 `TIMESPAN` 쿼리에 지정 된 재정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="2a4f9-277">yyyy-MM-ddTHH:mm:ssZ 형식이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="2a4f9-278">문자열 타임스탬프</span><span class="sxs-lookup"><span data-stu-id="2a4f9-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="2a4f9-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2a4f9-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="2a4f9-280">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-280">Yes</span></span>     |    <span data-ttu-id="2a4f9-281">보고서가 생성되어야 하는 빈도(시간)입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="2a4f9-282">최소값은 4이고 최대값은 2160입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="2a4f9-283">integer</span><span class="sxs-lookup"><span data-stu-id="2a4f9-283">integer</span></span>     |
|    <span data-ttu-id="2a4f9-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2a4f9-284">RecurrenceCount</span></span>     |    <span data-ttu-id="2a4f9-285">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-285">No</span></span>     |    <span data-ttu-id="2a4f9-286">생성할 보고서 수입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="2a4f9-287">정수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-287">integer</span></span>     |
|    <span data-ttu-id="2a4f9-288">형식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-288">Format</span></span>     |    <span data-ttu-id="2a4f9-289">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-289">No</span></span>     |    <span data-ttu-id="2a4f9-290">내보낸 파일의 파일 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-290">File format of the exported file.</span></span> <br> <span data-ttu-id="2a4f9-291">기본값은 CSV입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-291">Default is CSV.</span></span>    |    <span data-ttu-id="2a4f9-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="2a4f9-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="2a4f9-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="2a4f9-293">CallbackUrl</span></span>     |    <span data-ttu-id="2a4f9-294">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-294">No</span></span>     |    <span data-ttu-id="2a4f9-295">선택적으로 콜백 대상으로 구성할 수 있는 공개적으로 연결할 수 있는 URL</span><span class="sxs-lookup"><span data-stu-id="2a4f9-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="2a4f9-296">문자열(http URL)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-296">String (http URL)</span></span>     |
|    <span data-ttu-id="2a4f9-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2a4f9-297">CallbackMethod</span></span>     |    <span data-ttu-id="2a4f9-298">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-298">No</span></span>     |    <span data-ttu-id="2a4f9-299">콜백에 사용할 메서드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-299">The method to be used for callback</span></span>     |    <span data-ttu-id="2a4f9-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="2a4f9-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="2a4f9-301">샘플 응답</span><span class="sxs-lookup"><span data-stu-id="2a4f9-301">Sample response</span></span>

<span data-ttu-id="2a4f9-302">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="2a4f9-303">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2a4f9-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2a4f9-304">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="2a4f9-304">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="2a4f9-305">용어</span><span class="sxs-lookup"><span data-stu-id="2a4f9-305">Glossary</span></span>

<span data-ttu-id="2a4f9-306">응답의 요소에 대 한 주요 정의는 아래와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="2a4f9-307">매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-307">Parameter</span></span>     |    <span data-ttu-id="2a4f9-308">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="2a4f9-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-309">ReportId</span></span>     |    <span data-ttu-id="2a4f9-310">만든 보고서의 UUID(범용 고유 식별자)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="2a4f9-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="2a4f9-311">ReportName</span></span>     |    <span data-ttu-id="2a4f9-312">요청 페이로드의 보고서에 지정된 이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="2a4f9-313">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-313">Description</span></span>     |    <span data-ttu-id="2a4f9-314">보고서를 만드는 동안 제공된 설명</span><span class="sxs-lookup"><span data-stu-id="2a4f9-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="2a4f9-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-315">QueryId</span></span>     |    <span data-ttu-id="2a4f9-316">보고서를 만들 때 전달된 쿼리 ID</span><span class="sxs-lookup"><span data-stu-id="2a4f9-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="2a4f9-317">쿼리</span><span class="sxs-lookup"><span data-stu-id="2a4f9-317">Query</span></span>     |    <span data-ttu-id="2a4f9-318">이 보고서에 대해 실행되는 쿼리 텍스트</span><span class="sxs-lookup"><span data-stu-id="2a4f9-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="2a4f9-319">사용자</span><span class="sxs-lookup"><span data-stu-id="2a4f9-319">User</span></span>     |    <span data-ttu-id="2a4f9-320">보고서를 만드는 데 사용되는 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="2a4f9-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="2a4f9-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-321">CreatedTime</span></span>     |    <span data-ttu-id="2a4f9-322">보고서가 생성된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2a4f9-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-323">ModifiedTime</span></span>     |    <span data-ttu-id="2a4f9-324">보고서가 마지막으로 수정된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2a4f9-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2a4f9-325">ExecuteNow</span></span>     |    <span data-ttu-id="2a4f9-326">`ExecuteNow` 보고서를 만들 때 설정 되는 플래그입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="2a4f9-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-327">StartTime</span></span>     |    <span data-ttu-id="2a4f9-328">보고서 실행이 시작되는 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2a4f9-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="2a4f9-329">ReportStatus</span></span>     |    <span data-ttu-id="2a4f9-330">보고서 실행 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-330">Status of the report execution.</span></span> <span data-ttu-id="2a4f9-331">가능한 값은 `Paused` , `Active` 및입니다. `Inactive`</span><span class="sxs-lookup"><span data-stu-id="2a4f9-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="2a4f9-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2a4f9-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="2a4f9-333">보고서를 만드는 동안 제공된 되풀이 간격</span><span class="sxs-lookup"><span data-stu-id="2a4f9-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="2a4f9-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2a4f9-334">RecurrenceCount</span></span>     |    <span data-ttu-id="2a4f9-335">보고서를 만드는 동안 제공된 되풀이 수입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="2a4f9-336">콜백 url</span><span class="sxs-lookup"><span data-stu-id="2a4f9-336">CallbackUrl</span></span>     |    <span data-ttu-id="2a4f9-337">요청에 제공된 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="2a4f9-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="2a4f9-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2a4f9-338">CallbackMethod</span></span>     |    <span data-ttu-id="2a4f9-339">요청에 제공 된 콜백 메서드입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="2a4f9-340">서식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-340">Format</span></span>     |    <span data-ttu-id="2a4f9-341">보고서 파일의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-341">Format of the report files.</span></span> <span data-ttu-id="2a4f9-342">가능한 값은 `CSV` 또는 `TSV` 입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="2a4f9-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2a4f9-343">TotalCount</span></span>     |    <span data-ttu-id="2a4f9-344">값 배열에 있는 레코드 수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="2a4f9-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2a4f9-345">StatusCode</span></span>     |    <span data-ttu-id="2a4f9-346">결과 코드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-346">Result Code</span></span>     |
|    <span data-ttu-id="2a4f9-347">message</span><span class="sxs-lookup"><span data-stu-id="2a4f9-347">message</span></span>     |    <span data-ttu-id="2a4f9-348">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="2a4f9-349">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="2a4f9-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="2a4f9-350">보고서 실행 API 가져오기</span><span class="sxs-lookup"><span data-stu-id="2a4f9-350">Get report execution API</span></span>

<span data-ttu-id="2a4f9-351">이 메서드를 사용 하 여 [보고서 만들기 API](#create-report-api)에서 받은 보고서 id를 사용 하 여 보고서 실행 상태를 쿼리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="2a4f9-352">이 메서드는 보고서를 다운로드할 준비가 된 경우 보고서 다운로드 링크를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="2a4f9-353">그렇지 않으면 메서드가 상태를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="2a4f9-354">또한 이 API를 사용하여 특정 보고서에 대해 발생한 모든 실행을 가져올 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="2a4f9-355">이 API에는 및에 대해 설정 된 기본 쿼리 매개 변수가 있습니다 `executionStatus=Completed` `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="2a4f9-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="2a4f9-356">따라서 보고서 실행이 처음으로 성공하기 전에 API를 호출하면 404가 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="2a4f9-357">`executionStatus=Pending`을 설정하여 보류 중인 실행을 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="2a4f9-358">요청 구문</span><span class="sxs-lookup"><span data-stu-id="2a4f9-358">Request syntax</span></span>

|    <span data-ttu-id="2a4f9-359">방법</span><span class="sxs-lookup"><span data-stu-id="2a4f9-359">Method</span></span>     |    <span data-ttu-id="2a4f9-360">요청 URI</span><span class="sxs-lookup"><span data-stu-id="2a4f9-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="2a4f9-361">GET</span><span class="sxs-lookup"><span data-stu-id="2a4f9-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="2a4f9-362">요청 헤더</span><span class="sxs-lookup"><span data-stu-id="2a4f9-362">Request header</span></span>

|    <span data-ttu-id="2a4f9-363">헤더</span><span class="sxs-lookup"><span data-stu-id="2a4f9-363">Header</span></span>     |    <span data-ttu-id="2a4f9-364">유형</span><span class="sxs-lookup"><span data-stu-id="2a4f9-364">Type</span></span>     |    <span data-ttu-id="2a4f9-365">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="2a4f9-366">권한 부여</span><span class="sxs-lookup"><span data-stu-id="2a4f9-366">Authorization</span></span>     |    <span data-ttu-id="2a4f9-367">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-367">string</span></span> |<span data-ttu-id="2a4f9-368">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-368">Required.</span></span> <span data-ttu-id="2a4f9-369">Azure AD(Azure Active Directory) 액세스 토큰입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="2a4f9-370">형식은  `Bearer <token>` 입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="2a4f9-371">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-371">Content-Type</span></span>     |<span data-ttu-id="2a4f9-372">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="2a4f9-373">경로 매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-373">Path parameter</span></span>

|    <span data-ttu-id="2a4f9-374">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-374">Parameter Name</span></span>    |    <span data-ttu-id="2a4f9-375">필수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-375">Required</span></span>    |    <span data-ttu-id="2a4f9-376">Type</span><span class="sxs-lookup"><span data-stu-id="2a4f9-376">Type</span></span>    |    <span data-ttu-id="2a4f9-377">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2a4f9-378">reportId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-378">reportId</span></span>    |    <span data-ttu-id="2a4f9-379">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-379">Yes</span></span>    |    <span data-ttu-id="2a4f9-380">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-380">string</span></span>    |    <span data-ttu-id="2a4f9-381">이 인수에 지정 된 보고서 id를 사용 하는 보고서의 실행 세부 정보를 가져오려면 필터를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="2a4f9-382">여러 reportIds를 세미콜론 ";"으로 구분 하 여 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="2a4f9-383">쿼리 매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-383">Query parameter</span></span>

|    <span data-ttu-id="2a4f9-384">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="2a4f9-384">Parameter Name</span></span>    |    <span data-ttu-id="2a4f9-385">필수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-385">Required</span></span>    |    <span data-ttu-id="2a4f9-386">Type</span><span class="sxs-lookup"><span data-stu-id="2a4f9-386">Type</span></span>    |    <span data-ttu-id="2a4f9-387">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2a4f9-388">executionId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-388">executionId</span></span>    |    <span data-ttu-id="2a4f9-389">예</span><span class="sxs-lookup"><span data-stu-id="2a4f9-389">No</span></span>    |    <span data-ttu-id="2a4f9-390">문자열</span><span class="sxs-lookup"><span data-stu-id="2a4f9-390">string</span></span>    |    <span data-ttu-id="2a4f9-391">이 인수에 지정 된 executionId를 사용 하 여 보고서의 세부 정보만 가져오도록 필터링 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="2a4f9-392">여러 executionIds는 세미콜론 ";"으로 구분 하 여 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="2a4f9-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="2a4f9-393">executionStatus</span></span>    |    <span data-ttu-id="2a4f9-394">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-394">No</span></span>    |    <span data-ttu-id="2a4f9-395">문자열/열거형</span><span class="sxs-lookup"><span data-stu-id="2a4f9-395">String/enum</span></span>    |    <span data-ttu-id="2a4f9-396">이 인수에 지정 된 executionStatus를 사용 하 여 보고서의 세부 정보만 가져오도록 필터링 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="2a4f9-397">유효한 값은 `Pending` , `Running` `Paused` 및 `Completed` 입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="2a4f9-398">기본값은 `Completed`입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="2a4f9-399">여러 상태를 세미콜론 (";")으로 구분 하 여 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="2a4f9-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="2a4f9-400">getLatestExecution</span></span>    |    <span data-ttu-id="2a4f9-401">아니요</span><span class="sxs-lookup"><span data-stu-id="2a4f9-401">No</span></span>    |    <span data-ttu-id="2a4f9-402">boolean</span><span class="sxs-lookup"><span data-stu-id="2a4f9-402">boolean</span></span>    |    <span data-ttu-id="2a4f9-403">API는 최신 실행에 대 한 세부 정보를 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="2a4f9-404">이 매개 변수는 기본적으로 true로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="2a4f9-405">이 매개 변수 값을 false로 전달 하도록 선택 하면 API는 최근 90 일 실행 인스턴스를 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="2a4f9-406">샘플 요청 페이로드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-406">Sample Request Payload</span></span>

<span data-ttu-id="2a4f9-407">None</span><span class="sxs-lookup"><span data-stu-id="2a4f9-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="2a4f9-408">샘플 응답</span><span class="sxs-lookup"><span data-stu-id="2a4f9-408">Sample Response</span></span>

<span data-ttu-id="2a4f9-409">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="2a4f9-410">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2a4f9-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2a4f9-411">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="2a4f9-411">Response payload example:</span></span>

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

<span data-ttu-id="2a4f9-412">보고서 실행이 완료되면 실행 상태 `Completed`가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="2a4f9-413">`reportAccessSecureLink`에서 URL을 선택하여 보고서를 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="2a4f9-414">용어</span><span class="sxs-lookup"><span data-stu-id="2a4f9-414">Glossary</span></span>

<span data-ttu-id="2a4f9-415">응답에 있는 요소의 주요 정의입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="2a4f9-416">매개 변수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-416">Parameter</span></span>    |    <span data-ttu-id="2a4f9-417">Description</span><span class="sxs-lookup"><span data-stu-id="2a4f9-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2a4f9-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-418">ExecutionId</span></span>    |    <span data-ttu-id="2a4f9-419">실행 인스턴스의 UUID(범용 고유 식별자)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="2a4f9-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="2a4f9-420">ReportId</span></span>    |    <span data-ttu-id="2a4f9-421">실행 인스턴스와 연결된 보고서 ID</span><span class="sxs-lookup"><span data-stu-id="2a4f9-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="2a4f9-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2a4f9-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="2a4f9-423">보고서를 만드는 동안 제공된 되풀이 간격</span><span class="sxs-lookup"><span data-stu-id="2a4f9-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="2a4f9-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2a4f9-424">RecurrenceCount</span></span>    |    <span data-ttu-id="2a4f9-425">보고서를 만드는 동안 제공된 되풀이 수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="2a4f9-426">콜백 url</span><span class="sxs-lookup"><span data-stu-id="2a4f9-426">CallbackUrl</span></span>    |    <span data-ttu-id="2a4f9-427">실행 인스턴스와 연결된 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="2a4f9-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="2a4f9-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2a4f9-428">CallbackMethod</span></span>    |    <span data-ttu-id="2a4f9-429">실행 인스턴스와 연결 된 콜백 메서드입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="2a4f9-430">서식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-430">Format</span></span>    |    <span data-ttu-id="2a4f9-431">실행이 끝날 때 생성된 파일의 형식</span><span class="sxs-lookup"><span data-stu-id="2a4f9-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="2a4f9-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="2a4f9-432">ExecutionStatus</span></span>    |    <span data-ttu-id="2a4f9-433">보고서 실행 인스턴스의 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="2a4f9-434">유효한 값은 `Pending`, `Running`, `Paused` 및 `Completed`입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="2a4f9-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="2a4f9-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="2a4f9-436">보고서에 안전하게 액세스하는 데 사용할 수 있는 링크</span><span class="sxs-lookup"><span data-stu-id="2a4f9-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="2a4f9-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="2a4f9-438">보고서 링크가 만료되는 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="2a4f9-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="2a4f9-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="2a4f9-440">보고서가 생성된 UTC 시간(yyyy-MM-ddTHH:mm:ssZ 형식)</span><span class="sxs-lookup"><span data-stu-id="2a4f9-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="2a4f9-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2a4f9-441">TotalCount</span></span>    |    <span data-ttu-id="2a4f9-442">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="2a4f9-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="2a4f9-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2a4f9-443">StatusCode</span></span>    |    <span data-ttu-id="2a4f9-444">결과 코드</span><span class="sxs-lookup"><span data-stu-id="2a4f9-444">Result Code</span></span> <br> <span data-ttu-id="2a4f9-445">가능한 값은 200, 400, 401, 403, 404 및 500입니다.</span><span class="sxs-lookup"><span data-stu-id="2a4f9-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="2a4f9-446">message</span><span class="sxs-lookup"><span data-stu-id="2a4f9-446">message</span></span>    |    <span data-ttu-id="2a4f9-447">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="2a4f9-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="2a4f9-448">다음 단계</span><span class="sxs-lookup"><span data-stu-id="2a4f9-448">Next steps</span></span>

- <span data-ttu-id="2a4f9-449">[SWAGGER API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) 을 통해 api 사용해 보기</span><span class="sxs-lookup"><span data-stu-id="2a4f9-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="2a4f9-450">첫 번째 API 호출 만들기</span><span class="sxs-lookup"><span data-stu-id="2a4f9-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)