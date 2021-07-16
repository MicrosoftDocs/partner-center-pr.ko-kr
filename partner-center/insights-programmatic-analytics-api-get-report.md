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
# <a name="get-report-api"></a><span data-ttu-id="2941d-103">보고서 API 가져오기</span><span class="sxs-lookup"><span data-stu-id="2941d-103">Get report API</span></span>

<span data-ttu-id="2941d-104">이 API는 예약된 모든 보고서를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="2941d-105">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="2941d-105">**Request syntax**</span></span>

|    <span data-ttu-id="2941d-106">방법</span><span class="sxs-lookup"><span data-stu-id="2941d-106">Method</span></span>    |    <span data-ttu-id="2941d-107">요청 URI</span><span class="sxs-lookup"><span data-stu-id="2941d-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2941d-108">GET</span><span class="sxs-lookup"><span data-stu-id="2941d-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="2941d-109">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="2941d-109">**Request header**</span></span>

|    <span data-ttu-id="2941d-110">헤더</span><span class="sxs-lookup"><span data-stu-id="2941d-110">Header</span></span>    |    <span data-ttu-id="2941d-111">유형</span><span class="sxs-lookup"><span data-stu-id="2941d-111">Type</span></span>    |    <span data-ttu-id="2941d-112">Description</span><span class="sxs-lookup"><span data-stu-id="2941d-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="2941d-113">권한 부여</span><span class="sxs-lookup"><span data-stu-id="2941d-113">Authorization</span></span>    |    <span data-ttu-id="2941d-114">문자열</span><span class="sxs-lookup"><span data-stu-id="2941d-114">string</span></span>    |    <span data-ttu-id="2941d-115">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="2941d-115">Required.</span></span> <span data-ttu-id="2941d-116">양식의 AAD(Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="2941d-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="2941d-117">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="2941d-117">Content-Type</span></span>    |    <span data-ttu-id="2941d-118">문자열</span><span class="sxs-lookup"><span data-stu-id="2941d-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="2941d-119">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="2941d-119">**Path parameter**</span></span>

<span data-ttu-id="2941d-120">없음</span><span class="sxs-lookup"><span data-stu-id="2941d-120">None</span></span>

<span data-ttu-id="2941d-121">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="2941d-121">**Query parameter**</span></span>

|    <span data-ttu-id="2941d-122">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="2941d-122">Parameter Name</span></span>    |    <span data-ttu-id="2941d-123">유형</span><span class="sxs-lookup"><span data-stu-id="2941d-123">Type</span></span>    |    <span data-ttu-id="2941d-124">필수</span><span class="sxs-lookup"><span data-stu-id="2941d-124">Required</span></span>    |    <span data-ttu-id="2941d-125">Description</span><span class="sxs-lookup"><span data-stu-id="2941d-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2941d-126">reportId</span><span class="sxs-lookup"><span data-stu-id="2941d-126">reportId</span></span>     |    <span data-ttu-id="2941d-127">문자열</span><span class="sxs-lookup"><span data-stu-id="2941d-127">string</span></span>    |    <span data-ttu-id="2941d-128">예</span><span class="sxs-lookup"><span data-stu-id="2941d-128">No</span></span>    |    <span data-ttu-id="2941d-129">이 인수에 지정된 reportId가 있는 보고서만 자세히 보기 위한 필터</span><span class="sxs-lookup"><span data-stu-id="2941d-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="2941d-130">reportName</span><span class="sxs-lookup"><span data-stu-id="2941d-130">reportName</span></span>     |    <span data-ttu-id="2941d-131">문자열</span><span class="sxs-lookup"><span data-stu-id="2941d-131">string</span></span>    |    <span data-ttu-id="2941d-132">예</span><span class="sxs-lookup"><span data-stu-id="2941d-132">No</span></span>    |    <span data-ttu-id="2941d-133">이 인수에 지정된 reportName이 있는 보고서만 자세히 보기 위한 필터</span><span class="sxs-lookup"><span data-stu-id="2941d-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="2941d-134">queryId</span><span class="sxs-lookup"><span data-stu-id="2941d-134">queryId</span></span>     |    <span data-ttu-id="2941d-135">문자열</span><span class="sxs-lookup"><span data-stu-id="2941d-135">string</span></span>    |    <span data-ttu-id="2941d-136">예</span><span class="sxs-lookup"><span data-stu-id="2941d-136">No</span></span>    |    <span data-ttu-id="2941d-137">이 인수에 지정된 queryId를 사용하여 보고서 세부 정보만 가져오기 위한 필터</span><span class="sxs-lookup"><span data-stu-id="2941d-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="2941d-138">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="2941d-138">**Request payload**</span></span>

<span data-ttu-id="2941d-139">없음</span><span class="sxs-lookup"><span data-stu-id="2941d-139">None</span></span>

<span data-ttu-id="2941d-140">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="2941d-140">**Glossary**</span></span>

<span data-ttu-id="2941d-141">없음</span><span class="sxs-lookup"><span data-stu-id="2941d-141">None</span></span>

<span data-ttu-id="2941d-142">**응답**</span><span class="sxs-lookup"><span data-stu-id="2941d-142">**Response**</span></span>

<span data-ttu-id="2941d-143">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="2941d-144">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2941d-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2941d-145">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="2941d-145">Response payload example:</span></span>

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

<span data-ttu-id="2941d-146">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="2941d-146">**Glossary**</span></span>

<span data-ttu-id="2941d-147">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="2941d-148">매개 변수</span><span class="sxs-lookup"><span data-stu-id="2941d-148">Parameter</span></span>    |    <span data-ttu-id="2941d-149">Description</span><span class="sxs-lookup"><span data-stu-id="2941d-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2941d-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="2941d-150">ReportId</span></span>     |    <span data-ttu-id="2941d-151">생성된 보고서의 고유 UUID</span><span class="sxs-lookup"><span data-stu-id="2941d-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="2941d-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="2941d-152">ReportName</span></span>     |    <span data-ttu-id="2941d-153">요청 페이로드의 보고서에 지정된 이름</span><span class="sxs-lookup"><span data-stu-id="2941d-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="2941d-154">Description</span><span class="sxs-lookup"><span data-stu-id="2941d-154">Description</span></span>     |    <span data-ttu-id="2941d-155">보고서를 만들 때 지정된 설명</span><span class="sxs-lookup"><span data-stu-id="2941d-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="2941d-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="2941d-156">QueryId</span></span>     |    <span data-ttu-id="2941d-157">보고서를 만들 때 전달된 쿼리 ID</span><span class="sxs-lookup"><span data-stu-id="2941d-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="2941d-158">쿼리</span><span class="sxs-lookup"><span data-stu-id="2941d-158">Query</span></span>     |    <span data-ttu-id="2941d-159">이 보고서에 대해 실행되는 쿼리 텍스트</span><span class="sxs-lookup"><span data-stu-id="2941d-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="2941d-160">사용자</span><span class="sxs-lookup"><span data-stu-id="2941d-160">User</span></span>     |    <span data-ttu-id="2941d-161">보고서를 만드는 데 사용되는 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="2941d-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="2941d-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2941d-162">CreatedTime</span></span>     |    <span data-ttu-id="2941d-163">보고서가 생성된 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-163">Time the report was created.</span></span> <span data-ttu-id="2941d-164">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2941d-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2941d-165">ModifiedTime</span></span>     |    <span data-ttu-id="2941d-166">보고서를 마지막으로 수정한 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-166">Time the report was last modified.</span></span> <span data-ttu-id="2941d-167">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2941d-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="2941d-168">executeNow</span></span>     |    <span data-ttu-id="2941d-169">보고서를 만들 때 설정된 ExecuteNow 플래그</span><span class="sxs-lookup"><span data-stu-id="2941d-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="2941d-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="2941d-170">StartTime</span></span>     |    <span data-ttu-id="2941d-171">시간 실행이 시작됩니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-171">Time execution will begin.</span></span> <span data-ttu-id="2941d-172">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2941d-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="2941d-173">ReportStatus</span></span>     |    <span data-ttu-id="2941d-174">보고서 실행 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-174">Status of the report execution.</span></span> <span data-ttu-id="2941d-175">가능한 값은 일시 중지, 활성 및 비활성입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="2941d-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2941d-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="2941d-177">보고서를 만드는 동안 제공된 되풀이 간격</span><span class="sxs-lookup"><span data-stu-id="2941d-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="2941d-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2941d-178">RecurrenceCount</span></span>     |    <span data-ttu-id="2941d-179">보고서를 만드는 동안 제공된 되풀이 수</span><span class="sxs-lookup"><span data-stu-id="2941d-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="2941d-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="2941d-180">CallbackUrl</span></span>     |    <span data-ttu-id="2941d-181">요청에 제공된 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="2941d-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="2941d-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2941d-182">CallbackMethod</span></span>    |    <span data-ttu-id="2941d-183">요청에 제공된 콜백 메서드</span><span class="sxs-lookup"><span data-stu-id="2941d-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="2941d-184">서식</span><span class="sxs-lookup"><span data-stu-id="2941d-184">Format</span></span>     |    <span data-ttu-id="2941d-185">보고서 파일 형식</span><span class="sxs-lookup"><span data-stu-id="2941d-185">Format of the report files</span></span>     |
|    <span data-ttu-id="2941d-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2941d-186">TotalCount</span></span>     |    <span data-ttu-id="2941d-187">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="2941d-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="2941d-188">메시지</span><span class="sxs-lookup"><span data-stu-id="2941d-188">Message</span></span>     |    <span data-ttu-id="2941d-189">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="2941d-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="2941d-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2941d-190">StatusCode</span></span>     |    <span data-ttu-id="2941d-191">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-191">Result Code.</span></span> <span data-ttu-id="2941d-192">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="2941d-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |