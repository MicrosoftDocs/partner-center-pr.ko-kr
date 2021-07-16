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
# <a name="get-report-queries-api"></a><span data-ttu-id="b6e7c-103">보고서 쿼리 API 가져오기</span><span class="sxs-lookup"><span data-stu-id="b6e7c-103">Get report queries API</span></span>

<span data-ttu-id="b6e7c-104">보고서 쿼리 가져오기 API는 보고서에서 사용할 수 있는 모든 쿼리를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="b6e7c-105">기본값으로 모든 시스템 및 사용자 정의 쿼리를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="b6e7c-106">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-106">**Request syntax**</span></span>

|    <span data-ttu-id="b6e7c-107">방법</span><span class="sxs-lookup"><span data-stu-id="b6e7c-107">Method</span></span>    |    <span data-ttu-id="b6e7c-108">요청 URI</span><span class="sxs-lookup"><span data-stu-id="b6e7c-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b6e7c-109">GET</span><span class="sxs-lookup"><span data-stu-id="b6e7c-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="b6e7c-110">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-110">**Request header**</span></span>

|    <span data-ttu-id="b6e7c-111">헤더</span><span class="sxs-lookup"><span data-stu-id="b6e7c-111">Header</span></span>    |    <span data-ttu-id="b6e7c-112">유형</span><span class="sxs-lookup"><span data-stu-id="b6e7c-112">Type</span></span>    |    <span data-ttu-id="b6e7c-113">Description</span><span class="sxs-lookup"><span data-stu-id="b6e7c-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="b6e7c-114">권한 부여</span><span class="sxs-lookup"><span data-stu-id="b6e7c-114">Authorization</span></span>    |    <span data-ttu-id="b6e7c-115">문자열</span><span class="sxs-lookup"><span data-stu-id="b6e7c-115">string</span></span>    |    <span data-ttu-id="b6e7c-116">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-116">Required.</span></span> <span data-ttu-id="b6e7c-117">형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="b6e7c-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="b6e7c-118">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="b6e7c-118">Content-Type</span></span>    |    <span data-ttu-id="b6e7c-119">문자열</span><span class="sxs-lookup"><span data-stu-id="b6e7c-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="b6e7c-120">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-120">**Path parameter**</span></span>

<span data-ttu-id="b6e7c-121">없음</span><span class="sxs-lookup"><span data-stu-id="b6e7c-121">None</span></span>

<span data-ttu-id="b6e7c-122">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-122">**Query parameter**</span></span>

|    <span data-ttu-id="b6e7c-123">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="b6e7c-123">Parameter Name</span></span>    |    <span data-ttu-id="b6e7c-124">유형</span><span class="sxs-lookup"><span data-stu-id="b6e7c-124">Type</span></span>    |    <span data-ttu-id="b6e7c-125">필수</span><span class="sxs-lookup"><span data-stu-id="b6e7c-125">Required</span></span>    |    <span data-ttu-id="b6e7c-126">Description</span><span class="sxs-lookup"><span data-stu-id="b6e7c-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="b6e7c-127">queryId</span><span class="sxs-lookup"><span data-stu-id="b6e7c-127">queryId</span></span>     |    <span data-ttu-id="b6e7c-128">문자열</span><span class="sxs-lookup"><span data-stu-id="b6e7c-128">string</span></span>     |    <span data-ttu-id="b6e7c-129">No</span><span class="sxs-lookup"><span data-stu-id="b6e7c-129">No</span></span>    |    <span data-ttu-id="b6e7c-130">인수에 지정된 ID를 가진 쿼리만 세부 정보를 가져오는 필터</span><span class="sxs-lookup"><span data-stu-id="b6e7c-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="b6e7c-131">queryName</span><span class="sxs-lookup"><span data-stu-id="b6e7c-131">queryName</span></span>     |    <span data-ttu-id="b6e7c-132">문자열</span><span class="sxs-lookup"><span data-stu-id="b6e7c-132">string</span></span>     |    <span data-ttu-id="b6e7c-133">No</span><span class="sxs-lookup"><span data-stu-id="b6e7c-133">No</span></span>    |    <span data-ttu-id="b6e7c-134">인수에 지정된 이름을 가진 쿼리만 세부 정보를 가져오는 필터</span><span class="sxs-lookup"><span data-stu-id="b6e7c-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="b6e7c-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="b6e7c-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="b6e7c-136">boolean</span><span class="sxs-lookup"><span data-stu-id="b6e7c-136">boolean</span></span>     |    <span data-ttu-id="b6e7c-137">예</span><span class="sxs-lookup"><span data-stu-id="b6e7c-137">No</span></span>    |    <span data-ttu-id="b6e7c-138">응답에 미리 정의된 시스템 쿼리 포함</span><span class="sxs-lookup"><span data-stu-id="b6e7c-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="b6e7c-139">Includeonly Systemqueries</span><span class="sxs-lookup"><span data-stu-id="b6e7c-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="b6e7c-140">boolean</span><span class="sxs-lookup"><span data-stu-id="b6e7c-140">boolean</span></span>     |    <span data-ttu-id="b6e7c-141">예</span><span class="sxs-lookup"><span data-stu-id="b6e7c-141">No</span></span>    |    <span data-ttu-id="b6e7c-142">응답에 시스템 쿼리만 포함</span><span class="sxs-lookup"><span data-stu-id="b6e7c-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="b6e7c-143">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-143">**Request payload**</span></span>

<span data-ttu-id="b6e7c-144">없음</span><span class="sxs-lookup"><span data-stu-id="b6e7c-144">None</span></span>

<span data-ttu-id="b6e7c-145">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-145">**Glossary**</span></span>

<span data-ttu-id="b6e7c-146">없음</span><span class="sxs-lookup"><span data-stu-id="b6e7c-146">None</span></span>

<span data-ttu-id="b6e7c-147">**응답**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-147">**Response**</span></span>

<span data-ttu-id="b6e7c-148">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="b6e7c-149">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="b6e7c-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="b6e7c-150">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="b6e7c-150">Response payload example:</span></span>

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

<span data-ttu-id="b6e7c-151">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="b6e7c-151">**Glossary**</span></span>

<span data-ttu-id="b6e7c-152">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="b6e7c-153">매개 변수</span><span class="sxs-lookup"><span data-stu-id="b6e7c-153">Parameter</span></span>    |    <span data-ttu-id="b6e7c-154">Description</span><span class="sxs-lookup"><span data-stu-id="b6e7c-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b6e7c-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="b6e7c-155">QueryId</span></span>     |    <span data-ttu-id="b6e7c-156">쿼리의 고유 UUID</span><span class="sxs-lookup"><span data-stu-id="b6e7c-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="b6e7c-157">이름</span><span class="sxs-lookup"><span data-stu-id="b6e7c-157">Name</span></span>     |    <span data-ttu-id="b6e7c-158">쿼리를 만들 때 쿼리에 지정된 이름</span><span class="sxs-lookup"><span data-stu-id="b6e7c-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="b6e7c-159">Description</span><span class="sxs-lookup"><span data-stu-id="b6e7c-159">Description</span></span>     |    <span data-ttu-id="b6e7c-160">쿼리를 만드는 동안 제공된 설명</span><span class="sxs-lookup"><span data-stu-id="b6e7c-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="b6e7c-161">쿼리</span><span class="sxs-lookup"><span data-stu-id="b6e7c-161">Query</span></span>     |    <span data-ttu-id="b6e7c-162">보고서 쿼리 문자열</span><span class="sxs-lookup"><span data-stu-id="b6e7c-162">Report query string</span></span>     |
|    <span data-ttu-id="b6e7c-163">유형</span><span class="sxs-lookup"><span data-stu-id="b6e7c-163">Type</span></span>     |    <span data-ttu-id="b6e7c-164">미리 정의 된 시스템 쿼리를 위해 사용자가 만든 쿼리 및 시스템에 대 한 사용자 정의로 설정</span><span class="sxs-lookup"><span data-stu-id="b6e7c-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="b6e7c-165">사용자</span><span class="sxs-lookup"><span data-stu-id="b6e7c-165">User</span></span>     |    <span data-ttu-id="b6e7c-166">쿼리를 만든 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="b6e7c-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="b6e7c-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="b6e7c-167">CreatedTime</span></span>     |    <span data-ttu-id="b6e7c-168">쿼리를 만든 시간</span><span class="sxs-lookup"><span data-stu-id="b6e7c-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="b6e7c-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b6e7c-169">TotalCount</span></span>     |    <span data-ttu-id="b6e7c-170">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="b6e7c-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="b6e7c-171">메시지</span><span class="sxs-lookup"><span data-stu-id="b6e7c-171">Message</span></span>     |    <span data-ttu-id="b6e7c-172">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="b6e7c-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="b6e7c-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="b6e7c-173">StatusCode</span></span>     |    <span data-ttu-id="b6e7c-174">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-174">Result Code.</span></span> <span data-ttu-id="b6e7c-175">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="b6e7c-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
