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
# <a name="try-report-queries-api"></a><span data-ttu-id="665c7-103">보고서 쿼리 API 사용해 보기</span><span class="sxs-lookup"><span data-stu-id="665c7-103">Try report queries API</span></span>

<span data-ttu-id="665c7-104">이 API는 보고서 쿼리 문을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-104">This API executes a Report query statement.</span></span> <span data-ttu-id="665c7-105">API는 파트너가 데이터를 예상한 대로 확인하는 데 사용할 수 있는 레코드를 100개만 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="665c7-106">이 API의 쿼리 실행 제한 시간은 100초입니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="665c7-107">API에 100초 이상이 소요될 경우 쿼리가 구문상 정확할 가능성이 높습니다. 그렇지 않으면 200 이외의 오류 코드를 수신하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="665c7-108">쿼리 구문이 올바르면 실제 보고서 생성이 성공합니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="665c7-109">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="665c7-109">**Request syntax**</span></span>

|    <span data-ttu-id="665c7-110">방법</span><span class="sxs-lookup"><span data-stu-id="665c7-110">Method</span></span>    |    <span data-ttu-id="665c7-111">요청 URI</span><span class="sxs-lookup"><span data-stu-id="665c7-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="665c7-112">GET</span><span class="sxs-lookup"><span data-stu-id="665c7-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="665c7-113">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="665c7-113">**Request header**</span></span>

|    <span data-ttu-id="665c7-114">헤더</span><span class="sxs-lookup"><span data-stu-id="665c7-114">Header</span></span>    |    <span data-ttu-id="665c7-115">유형</span><span class="sxs-lookup"><span data-stu-id="665c7-115">Type</span></span>    |    <span data-ttu-id="665c7-116">Description</span><span class="sxs-lookup"><span data-stu-id="665c7-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="665c7-117">권한 부여</span><span class="sxs-lookup"><span data-stu-id="665c7-117">Authorization</span></span>    |    <span data-ttu-id="665c7-118">문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-118">string</span></span>    |    <span data-ttu-id="665c7-119">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="665c7-119">Required.</span></span> <span data-ttu-id="665c7-120">양식의 AAD(Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="665c7-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="665c7-121">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="665c7-121">Content-Type</span></span>    |    <span data-ttu-id="665c7-122">문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="665c7-123">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="665c7-123">**Path parameter**</span></span>

<span data-ttu-id="665c7-124">없음</span><span class="sxs-lookup"><span data-stu-id="665c7-124">None</span></span>

<span data-ttu-id="665c7-125">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="665c7-125">**Query parameter**</span></span>

|    <span data-ttu-id="665c7-126">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="665c7-126">Parameter Name</span></span>    |    <span data-ttu-id="665c7-127">유형</span><span class="sxs-lookup"><span data-stu-id="665c7-127">Type</span></span>    |    <span data-ttu-id="665c7-128">필수</span><span class="sxs-lookup"><span data-stu-id="665c7-128">Required</span></span>    |    <span data-ttu-id="665c7-129">Description</span><span class="sxs-lookup"><span data-stu-id="665c7-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="665c7-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="665c7-130">exportQuery</span></span>     |    <span data-ttu-id="665c7-131">문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-131">string</span></span>    |    <span data-ttu-id="665c7-132">예</span><span class="sxs-lookup"><span data-stu-id="665c7-132">No</span></span>    |    <span data-ttu-id="665c7-133">실행해야 하는 보고서 쿼리 문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="665c7-134">queryId</span><span class="sxs-lookup"><span data-stu-id="665c7-134">queryId</span></span>     |    <span data-ttu-id="665c7-135">문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-135">string</span></span>    |    <span data-ttu-id="665c7-136">예</span><span class="sxs-lookup"><span data-stu-id="665c7-136">No</span></span>    |    <span data-ttu-id="665c7-137">유효한 기존 쿼리 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-137">A valid existing query ID.</span></span> <span data-ttu-id="665c7-138">exportQuery 매개 변수에 지정된 쿼리 문자열과 함께 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="665c7-139">startTime</span><span class="sxs-lookup"><span data-stu-id="665c7-139">startTime</span></span>     |    <span data-ttu-id="665c7-140">문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-140">string</span></span>    |    <span data-ttu-id="665c7-141">예</span><span class="sxs-lookup"><span data-stu-id="665c7-141">No</span></span>    |    <span data-ttu-id="665c7-142">데이터를 원하는 시작 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-142">Start time from which we want the data.</span></span> <span data-ttu-id="665c7-143">쿼리에 지정된 시간 간격을 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="665c7-144">endTime</span><span class="sxs-lookup"><span data-stu-id="665c7-144">endTime</span></span>     |    <span data-ttu-id="665c7-145">문자열</span><span class="sxs-lookup"><span data-stu-id="665c7-145">string</span></span>    |    <span data-ttu-id="665c7-146">예</span><span class="sxs-lookup"><span data-stu-id="665c7-146">No</span></span>    |    <span data-ttu-id="665c7-147">데이터를 원하는 시간까지의 종료 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-147">End time till which we want the data.</span></span> <span data-ttu-id="665c7-148">쿼리에 지정된 시간 간격을 재정의합니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="665c7-149">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="665c7-149">**Request payload**</span></span>

<span data-ttu-id="665c7-150">없음</span><span class="sxs-lookup"><span data-stu-id="665c7-150">None</span></span>

<span data-ttu-id="665c7-151">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="665c7-151">**Glossary**</span></span>

<span data-ttu-id="665c7-152">없음</span><span class="sxs-lookup"><span data-stu-id="665c7-152">None</span></span>

<span data-ttu-id="665c7-153">**응답**</span><span class="sxs-lookup"><span data-stu-id="665c7-153">**Response**</span></span>

<span data-ttu-id="665c7-154">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="665c7-155">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="665c7-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="665c7-156">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="665c7-156">Response payload example:</span></span>

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

<span data-ttu-id="665c7-157">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="665c7-157">**Glossary**</span></span>

<span data-ttu-id="665c7-158">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="665c7-159">매개 변수</span><span class="sxs-lookup"><span data-stu-id="665c7-159">Parameter</span></span>    |    <span data-ttu-id="665c7-160">Description</span><span class="sxs-lookup"><span data-stu-id="665c7-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="665c7-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="665c7-161">TotalCount</span></span>     |    <span data-ttu-id="665c7-162">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="665c7-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="665c7-163">메시지</span><span class="sxs-lookup"><span data-stu-id="665c7-163">Message</span></span>     |    <span data-ttu-id="665c7-164">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="665c7-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="665c7-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="665c7-165">StatusCode</span></span>     |    <span data-ttu-id="665c7-166">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-166">Result Code.</span></span> <span data-ttu-id="665c7-167">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="665c7-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
