---
title: report queries API Insights 데이터 삭제
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용 하 여 파트너 센터 정보에서 사용자 정의 쿼리를 삭제 합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375886"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="8ad7e-103">보고서 쿼리 API 삭제</span><span class="sxs-lookup"><span data-stu-id="8ad7e-103">Delete report queries API</span></span>

<span data-ttu-id="8ad7e-104">이 API는 사용자 정의 쿼리를 삭제 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ad7e-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="8ad7e-105">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-105">**Request syntax**</span></span>

|    <span data-ttu-id="8ad7e-106">방법</span><span class="sxs-lookup"><span data-stu-id="8ad7e-106">Method</span></span>    |    <span data-ttu-id="8ad7e-107">요청 URI</span><span class="sxs-lookup"><span data-stu-id="8ad7e-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8ad7e-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="8ad7e-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="8ad7e-109">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-109">**Request header**</span></span>

|    <span data-ttu-id="8ad7e-110">헤더</span><span class="sxs-lookup"><span data-stu-id="8ad7e-110">Header</span></span>    |    <span data-ttu-id="8ad7e-111">유형</span><span class="sxs-lookup"><span data-stu-id="8ad7e-111">Type</span></span>    |    <span data-ttu-id="8ad7e-112">Description</span><span class="sxs-lookup"><span data-stu-id="8ad7e-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="8ad7e-113">권한 부여</span><span class="sxs-lookup"><span data-stu-id="8ad7e-113">Authorization</span></span>    |    <span data-ttu-id="8ad7e-114">문자열</span><span class="sxs-lookup"><span data-stu-id="8ad7e-114">string</span></span>    |    <span data-ttu-id="8ad7e-115">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="8ad7e-115">Required.</span></span> <span data-ttu-id="8ad7e-116">형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="8ad7e-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="8ad7e-117">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="8ad7e-117">Content-Type</span></span>    |    <span data-ttu-id="8ad7e-118">문자열</span><span class="sxs-lookup"><span data-stu-id="8ad7e-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="8ad7e-119">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-119">**Path parameter**</span></span>

|    <span data-ttu-id="8ad7e-120">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="8ad7e-120">Parameter Name</span></span>    |    <span data-ttu-id="8ad7e-121">유형</span><span class="sxs-lookup"><span data-stu-id="8ad7e-121">Type</span></span>    |    <span data-ttu-id="8ad7e-122">필수</span><span class="sxs-lookup"><span data-stu-id="8ad7e-122">Required</span></span>    |    <span data-ttu-id="8ad7e-123">Description</span><span class="sxs-lookup"><span data-stu-id="8ad7e-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="8ad7e-124">queryId</span><span class="sxs-lookup"><span data-stu-id="8ad7e-124">queryId</span></span>     |    <span data-ttu-id="8ad7e-125">문자열</span><span class="sxs-lookup"><span data-stu-id="8ad7e-125">string</span></span>     |    <span data-ttu-id="8ad7e-126">No</span><span class="sxs-lookup"><span data-stu-id="8ad7e-126">No</span></span>    |    <span data-ttu-id="8ad7e-127">인수에 지정된 ID를 가진 쿼리만 세부 정보를 가져오는 필터</span><span class="sxs-lookup"><span data-stu-id="8ad7e-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="8ad7e-128">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-128">**Query parameter**</span></span>

<span data-ttu-id="8ad7e-129">없음</span><span class="sxs-lookup"><span data-stu-id="8ad7e-129">None</span></span>

<span data-ttu-id="8ad7e-130">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-130">**Request payload**</span></span>

<span data-ttu-id="8ad7e-131">없음</span><span class="sxs-lookup"><span data-stu-id="8ad7e-131">None</span></span>

<span data-ttu-id="8ad7e-132">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-132">**Glossary**</span></span>

<span data-ttu-id="8ad7e-133">없음</span><span class="sxs-lookup"><span data-stu-id="8ad7e-133">None</span></span>

<span data-ttu-id="8ad7e-134">**응답**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-134">**Response**</span></span>

<span data-ttu-id="8ad7e-135">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ad7e-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="8ad7e-136">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="8ad7e-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="8ad7e-137">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="8ad7e-137">Response payload example:</span></span>

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

<span data-ttu-id="8ad7e-138">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="8ad7e-138">**Glossary**</span></span>

<span data-ttu-id="8ad7e-139">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="8ad7e-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="8ad7e-140">매개 변수</span><span class="sxs-lookup"><span data-stu-id="8ad7e-140">Parameter</span></span>    |    <span data-ttu-id="8ad7e-141">Description</span><span class="sxs-lookup"><span data-stu-id="8ad7e-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8ad7e-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="8ad7e-142">QueryId</span></span>     |    <span data-ttu-id="8ad7e-143">삭제 된 쿼리의 고유 UUID</span><span class="sxs-lookup"><span data-stu-id="8ad7e-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="8ad7e-144">이름</span><span class="sxs-lookup"><span data-stu-id="8ad7e-144">Name</span></span>     |    <span data-ttu-id="8ad7e-145">삭제 된 쿼리의 이름</span><span class="sxs-lookup"><span data-stu-id="8ad7e-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="8ad7e-146">Description</span><span class="sxs-lookup"><span data-stu-id="8ad7e-146">Description</span></span>     |    <span data-ttu-id="8ad7e-147">삭제 된 쿼리에 대 한 설명</span><span class="sxs-lookup"><span data-stu-id="8ad7e-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="8ad7e-148">쿼리</span><span class="sxs-lookup"><span data-stu-id="8ad7e-148">Query</span></span>     |    <span data-ttu-id="8ad7e-149">삭제 된 쿼리의 보고서 쿼리 문자열</span><span class="sxs-lookup"><span data-stu-id="8ad7e-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="8ad7e-150">유형</span><span class="sxs-lookup"><span data-stu-id="8ad7e-150">Type</span></span>     |    <span data-ttu-id="8ad7e-151">사용자가 만든 쿼리의 사용자 정의로 설정</span><span class="sxs-lookup"><span data-stu-id="8ad7e-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="8ad7e-152">사용자</span><span class="sxs-lookup"><span data-stu-id="8ad7e-152">User</span></span>     |    <span data-ttu-id="8ad7e-153">쿼리를 만든 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="8ad7e-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="8ad7e-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="8ad7e-154">CreatedTime</span></span>     |    <span data-ttu-id="8ad7e-155">쿼리를 만든 시간</span><span class="sxs-lookup"><span data-stu-id="8ad7e-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="8ad7e-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="8ad7e-156">TotalCount</span></span>     |    <span data-ttu-id="8ad7e-157">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="8ad7e-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="8ad7e-158">메시지</span><span class="sxs-lookup"><span data-stu-id="8ad7e-158">Message</span></span>     |    <span data-ttu-id="8ad7e-159">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="8ad7e-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="8ad7e-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="8ad7e-160">StatusCode</span></span>     |    <span data-ttu-id="8ad7e-161">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="8ad7e-161">Result Code.</span></span> <span data-ttu-id="8ad7e-162">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="8ad7e-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
