---
title: 보고서 API 업데이트
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 정보에서이 API를 사용 하 여 보고서 매개 변수를 업데이트 합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376092"
---
# <a name="update-report-api"></a><span data-ttu-id="3bc38-103">보고서 API 업데이트</span><span class="sxs-lookup"><span data-stu-id="3bc38-103">Update report API</span></span>

<span data-ttu-id="3bc38-104">이 API는 보고서 매개 변수를 수정하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="3bc38-105">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="3bc38-105">**Request syntax**</span></span>

|    <span data-ttu-id="3bc38-106">방법</span><span class="sxs-lookup"><span data-stu-id="3bc38-106">Method</span></span>    |    <span data-ttu-id="3bc38-107">요청 URI</span><span class="sxs-lookup"><span data-stu-id="3bc38-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3bc38-108">PUT</span><span class="sxs-lookup"><span data-stu-id="3bc38-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="3bc38-109">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="3bc38-109">**Request header**</span></span>

|    <span data-ttu-id="3bc38-110">헤더</span><span class="sxs-lookup"><span data-stu-id="3bc38-110">Header</span></span>    |    <span data-ttu-id="3bc38-111">유형</span><span class="sxs-lookup"><span data-stu-id="3bc38-111">Type</span></span>    |    <span data-ttu-id="3bc38-112">Description</span><span class="sxs-lookup"><span data-stu-id="3bc38-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="3bc38-113">권한 부여</span><span class="sxs-lookup"><span data-stu-id="3bc38-113">Authorization</span></span>    |    <span data-ttu-id="3bc38-114">문자열</span><span class="sxs-lookup"><span data-stu-id="3bc38-114">string</span></span>    |    <span data-ttu-id="3bc38-115">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="3bc38-115">Required.</span></span> <span data-ttu-id="3bc38-116">형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="3bc38-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="3bc38-117">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="3bc38-117">Content-Type</span></span>    |    <span data-ttu-id="3bc38-118">문자열</span><span class="sxs-lookup"><span data-stu-id="3bc38-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="3bc38-119">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="3bc38-119">**Path parameter**</span></span>

|    <span data-ttu-id="3bc38-120">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="3bc38-120">Parameter Name</span></span>    |    <span data-ttu-id="3bc38-121">유형</span><span class="sxs-lookup"><span data-stu-id="3bc38-121">Type</span></span>    |    <span data-ttu-id="3bc38-122">필수</span><span class="sxs-lookup"><span data-stu-id="3bc38-122">Required</span></span>    |    <span data-ttu-id="3bc38-123">Description</span><span class="sxs-lookup"><span data-stu-id="3bc38-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3bc38-124">reportId</span><span class="sxs-lookup"><span data-stu-id="3bc38-124">reportId</span></span>     |    <span data-ttu-id="3bc38-125">문자열</span><span class="sxs-lookup"><span data-stu-id="3bc38-125">string</span></span>    |    <span data-ttu-id="3bc38-126">예</span><span class="sxs-lookup"><span data-stu-id="3bc38-126">No</span></span>    |    <span data-ttu-id="3bc38-127">수정 중인 보고서의 ID</span><span class="sxs-lookup"><span data-stu-id="3bc38-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="3bc38-128">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="3bc38-128">**Query parameter**</span></span>

<span data-ttu-id="3bc38-129">없음</span><span class="sxs-lookup"><span data-stu-id="3bc38-129">None</span></span>

<span data-ttu-id="3bc38-130">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="3bc38-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="3bc38-131">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="3bc38-131">**Glossary**</span></span>

<span data-ttu-id="3bc38-132">다음 표에서는 응답의 요소에 대 한 주요 정의를 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="3bc38-133">매개 변수</span><span class="sxs-lookup"><span data-stu-id="3bc38-133">Parameter</span></span>    |    <span data-ttu-id="3bc38-134">필수</span><span class="sxs-lookup"><span data-stu-id="3bc38-134">Required</span></span>    |    <span data-ttu-id="3bc38-135">Description</span><span class="sxs-lookup"><span data-stu-id="3bc38-135">Description</span></span>    |    <span data-ttu-id="3bc38-136">허용되는 값</span><span class="sxs-lookup"><span data-stu-id="3bc38-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3bc38-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="3bc38-137">ReportName</span></span>     |    <span data-ttu-id="3bc38-138">예</span><span class="sxs-lookup"><span data-stu-id="3bc38-138">Yes</span></span>     |    <span data-ttu-id="3bc38-139">보고서에 할당할 이름</span><span class="sxs-lookup"><span data-stu-id="3bc38-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="3bc38-140">String</span><span class="sxs-lookup"><span data-stu-id="3bc38-140">String</span></span>     |
|    <span data-ttu-id="3bc38-141">설명</span><span class="sxs-lookup"><span data-stu-id="3bc38-141">Description</span></span>     |    <span data-ttu-id="3bc38-142">아니요</span><span class="sxs-lookup"><span data-stu-id="3bc38-142">No</span></span>     |    <span data-ttu-id="3bc38-143">생성된 보고서에 대한 설명</span><span class="sxs-lookup"><span data-stu-id="3bc38-143">Description of the created report</span></span>     |    <span data-ttu-id="3bc38-144">문자열</span><span class="sxs-lookup"><span data-stu-id="3bc38-144">String</span></span>     |
|    <span data-ttu-id="3bc38-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="3bc38-145">StartTime</span></span>     |    <span data-ttu-id="3bc38-146">예</span><span class="sxs-lookup"><span data-stu-id="3bc38-146">Yes</span></span>    |    <span data-ttu-id="3bc38-147">보고서 생성이 시작되는 타임스탬프</span><span class="sxs-lookup"><span data-stu-id="3bc38-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="3bc38-148">문자열</span><span class="sxs-lookup"><span data-stu-id="3bc38-148">String</span></span>     |
|    <span data-ttu-id="3bc38-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="3bc38-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="3bc38-150">No</span><span class="sxs-lookup"><span data-stu-id="3bc38-150">No</span></span>     |    <span data-ttu-id="3bc38-151">보고서가 생성되어야 하는 빈도(시간)입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="3bc38-152">최솟값은 4입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-152">Minimum value is 4</span></span>     |    <span data-ttu-id="3bc38-153">정수</span><span class="sxs-lookup"><span data-stu-id="3bc38-153">Integer</span></span>     |
|    <span data-ttu-id="3bc38-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="3bc38-154">RecurrenceCount</span></span>     |    <span data-ttu-id="3bc38-155">아니요</span><span class="sxs-lookup"><span data-stu-id="3bc38-155">No</span></span>     |    <span data-ttu-id="3bc38-156">생성할 보고서 수입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-156">Numbers of report to be generated.</span></span> <span data-ttu-id="3bc38-157">기본값은 무한입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-157">Default is indefinite.</span></span>     |    <span data-ttu-id="3bc38-158">정수</span><span class="sxs-lookup"><span data-stu-id="3bc38-158">Integer</span></span>     |
|    <span data-ttu-id="3bc38-159">형식</span><span class="sxs-lookup"><span data-stu-id="3bc38-159">Format</span></span>     |    <span data-ttu-id="3bc38-160">아니요</span><span class="sxs-lookup"><span data-stu-id="3bc38-160">No</span></span>    |    <span data-ttu-id="3bc38-161">내보낸 파일의 파일 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-161">File format of the exported file.</span></span> <span data-ttu-id="3bc38-162">기본값은 CSV입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-162">Default is CSV</span></span>     |    <span data-ttu-id="3bc38-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="3bc38-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="3bc38-164">콜백 URL</span><span class="sxs-lookup"><span data-stu-id="3bc38-164">CallbackURL</span></span>     |    <span data-ttu-id="3bc38-165">아니요</span><span class="sxs-lookup"><span data-stu-id="3bc38-165">No</span></span>     |    <span data-ttu-id="3bc38-166">보고서 생성 시 호출할 https 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="3bc38-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="3bc38-167">문자열</span><span class="sxs-lookup"><span data-stu-id="3bc38-167">String</span></span>     |
|    <span data-ttu-id="3bc38-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="3bc38-168">CallbackMethod</span></span>    |    <span data-ttu-id="3bc38-169">아니요</span><span class="sxs-lookup"><span data-stu-id="3bc38-169">No</span></span>    |    <span data-ttu-id="3bc38-170">콜백에 사용할 Http 메서드입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="3bc38-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="3bc38-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="3bc38-172">**응답**</span><span class="sxs-lookup"><span data-stu-id="3bc38-172">**Response**</span></span>

<span data-ttu-id="3bc38-173">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="3bc38-174">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="3bc38-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="3bc38-175">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="3bc38-175">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="3bc38-176">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="3bc38-176">**Glossary**</span></span>

<span data-ttu-id="3bc38-177">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="3bc38-178">매개 변수</span><span class="sxs-lookup"><span data-stu-id="3bc38-178">Parameter</span></span>    |    <span data-ttu-id="3bc38-179">Description</span><span class="sxs-lookup"><span data-stu-id="3bc38-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3bc38-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="3bc38-180">ReportId</span></span>     |    <span data-ttu-id="3bc38-181">업데이트 중인 보고서의 UUID(범용 고유 식별자)</span><span class="sxs-lookup"><span data-stu-id="3bc38-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="3bc38-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="3bc38-182">ReportName</span></span>     |    <span data-ttu-id="3bc38-183">요청 페이로드의 보고서에 지정된 이름</span><span class="sxs-lookup"><span data-stu-id="3bc38-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="3bc38-184">Description</span><span class="sxs-lookup"><span data-stu-id="3bc38-184">Description</span></span>     |    <span data-ttu-id="3bc38-185">요청 페이로드의 보고서에 지정 된 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="3bc38-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="3bc38-186">QueryId</span></span>     |    <span data-ttu-id="3bc38-187">보고서를 만들 때 전달된 쿼리 ID</span><span class="sxs-lookup"><span data-stu-id="3bc38-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="3bc38-188">쿼리</span><span class="sxs-lookup"><span data-stu-id="3bc38-188">Query</span></span>     |    <span data-ttu-id="3bc38-189">이 보고서에 대해 실행되는 쿼리 텍스트</span><span class="sxs-lookup"><span data-stu-id="3bc38-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="3bc38-190">사용자</span><span class="sxs-lookup"><span data-stu-id="3bc38-190">User</span></span>     |    <span data-ttu-id="3bc38-191">보고서를 만드는 데 사용되는 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="3bc38-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="3bc38-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="3bc38-192">CreatedTime</span></span>     |    <span data-ttu-id="3bc38-193">보고서가 생성된 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-193">Time the report was created.</span></span> <span data-ttu-id="3bc38-194">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3bc38-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="3bc38-195">ModifiedTime</span></span>     |    <span data-ttu-id="3bc38-196">보고서를 마지막으로 수정한 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-196">Time the report was last modified.</span></span> <span data-ttu-id="3bc38-197">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3bc38-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="3bc38-198">ExecuteNow</span></span>     |    <span data-ttu-id="3bc38-199">보고서를 만들 때 설정 되는 ExecuteNow 플래그</span><span class="sxs-lookup"><span data-stu-id="3bc38-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="3bc38-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="3bc38-200">StartTime</span></span>     |    <span data-ttu-id="3bc38-201">보고서 실행이 시작되는 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-201">Time the report execution will begin.</span></span> <span data-ttu-id="3bc38-202">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="3bc38-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="3bc38-203">ReportStatus</span></span>     |    <span data-ttu-id="3bc38-204">보고서 실행 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-204">Status of the report execution.</span></span> <span data-ttu-id="3bc38-205">가능한 값은 일시 중지, 활성 및 비활성입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="3bc38-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="3bc38-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="3bc38-207">요청 페이로드에 제공 된 되풀이 간격</span><span class="sxs-lookup"><span data-stu-id="3bc38-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="3bc38-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="3bc38-208">RecurrenceCount</span></span>     |    <span data-ttu-id="3bc38-209">요청 페이로드에 제공 된 되풀이 횟수</span><span class="sxs-lookup"><span data-stu-id="3bc38-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="3bc38-210">콜백 url</span><span class="sxs-lookup"><span data-stu-id="3bc38-210">CallbackUrl</span></span>     |    <span data-ttu-id="3bc38-211">요청에 제공된 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="3bc38-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="3bc38-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="3bc38-212">CallbackMethod</span></span>    |    <span data-ttu-id="3bc38-213">요청에 제공 된 콜백 메서드입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="3bc38-214">서식</span><span class="sxs-lookup"><span data-stu-id="3bc38-214">Format</span></span>     |    <span data-ttu-id="3bc38-215">보고서 파일 형식</span><span class="sxs-lookup"><span data-stu-id="3bc38-215">Format of the report files</span></span>     |
|    <span data-ttu-id="3bc38-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="3bc38-216">TotalCount</span></span>     |    <span data-ttu-id="3bc38-217">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="3bc38-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="3bc38-218">메시지</span><span class="sxs-lookup"><span data-stu-id="3bc38-218">Message</span></span>     |    <span data-ttu-id="3bc38-219">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="3bc38-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="3bc38-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="3bc38-220">StatusCode</span></span>     |    <span data-ttu-id="3bc38-221">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-221">Result Code.</span></span> <span data-ttu-id="3bc38-222">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="3bc38-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |