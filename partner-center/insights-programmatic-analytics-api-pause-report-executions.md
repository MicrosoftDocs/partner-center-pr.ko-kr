---
title: 보고서 실행 API 일시 중지 - 데이터 Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용하여 파트너 센터 인사이트에서 보고서의 실행을 일시 중지합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376117"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="a8412-103">보고서 실행 API 일시 중지</span><span class="sxs-lookup"><span data-stu-id="a8412-103">Pause report executions API</span></span>

<span data-ttu-id="a8412-104">실행에서 이 API는 예약된 보고서 실행을 일시 중지합니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="a8412-105">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="a8412-105">**Request syntax**</span></span>

|    <span data-ttu-id="a8412-106">방법</span><span class="sxs-lookup"><span data-stu-id="a8412-106">Method</span></span>    |    <span data-ttu-id="a8412-107">요청 URI</span><span class="sxs-lookup"><span data-stu-id="a8412-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a8412-108">PUT</span><span class="sxs-lookup"><span data-stu-id="a8412-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="a8412-109">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="a8412-109">**Request header**</span></span>

|    <span data-ttu-id="a8412-110">헤더</span><span class="sxs-lookup"><span data-stu-id="a8412-110">Header</span></span>    |    <span data-ttu-id="a8412-111">유형</span><span class="sxs-lookup"><span data-stu-id="a8412-111">Type</span></span>    |    <span data-ttu-id="a8412-112">Description</span><span class="sxs-lookup"><span data-stu-id="a8412-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="a8412-113">권한 부여</span><span class="sxs-lookup"><span data-stu-id="a8412-113">Authorization</span></span>    |    <span data-ttu-id="a8412-114">문자열</span><span class="sxs-lookup"><span data-stu-id="a8412-114">string</span></span>    |    <span data-ttu-id="a8412-115">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="a8412-115">Required.</span></span> <span data-ttu-id="a8412-116">양식의 AAD(Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="a8412-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="a8412-117">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="a8412-117">Content-Type</span></span>    |    <span data-ttu-id="a8412-118">문자열</span><span class="sxs-lookup"><span data-stu-id="a8412-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="a8412-119">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="a8412-119">**Path parameter**</span></span>

|    <span data-ttu-id="a8412-120">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="a8412-120">Parameter Name</span></span>    |    <span data-ttu-id="a8412-121">유형</span><span class="sxs-lookup"><span data-stu-id="a8412-121">Type</span></span>    |    <span data-ttu-id="a8412-122">필수</span><span class="sxs-lookup"><span data-stu-id="a8412-122">Required</span></span>    |    <span data-ttu-id="a8412-123">Description</span><span class="sxs-lookup"><span data-stu-id="a8412-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a8412-124">reportId</span><span class="sxs-lookup"><span data-stu-id="a8412-124">reportId</span></span>     |    <span data-ttu-id="a8412-125">문자열</span><span class="sxs-lookup"><span data-stu-id="a8412-125">string</span></span>    |    <span data-ttu-id="a8412-126">예</span><span class="sxs-lookup"><span data-stu-id="a8412-126">No</span></span>    |    <span data-ttu-id="a8412-127">수정 중인 보고서의 ID</span><span class="sxs-lookup"><span data-stu-id="a8412-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="a8412-128">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="a8412-128">**Query parameter**</span></span>

<span data-ttu-id="a8412-129">없음</span><span class="sxs-lookup"><span data-stu-id="a8412-129">None</span></span>

<span data-ttu-id="a8412-130">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="a8412-130">**Request payload**</span></span>

<span data-ttu-id="a8412-131">없음</span><span class="sxs-lookup"><span data-stu-id="a8412-131">None</span></span>

<span data-ttu-id="a8412-132">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="a8412-132">**Glossary**</span></span>

<span data-ttu-id="a8412-133">없음</span><span class="sxs-lookup"><span data-stu-id="a8412-133">None</span></span>

<span data-ttu-id="a8412-134">**응답**</span><span class="sxs-lookup"><span data-stu-id="a8412-134">**Response**</span></span>

<span data-ttu-id="a8412-135">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="a8412-136">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a8412-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a8412-137">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="a8412-137">Response payload example:</span></span>

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

<span data-ttu-id="a8412-138">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="a8412-138">**Glossary**</span></span>

<span data-ttu-id="a8412-139">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="a8412-140">매개 변수</span><span class="sxs-lookup"><span data-stu-id="a8412-140">Parameter</span></span>    |    <span data-ttu-id="a8412-141">Description</span><span class="sxs-lookup"><span data-stu-id="a8412-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a8412-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="a8412-142">ReportId</span></span>     |    <span data-ttu-id="a8412-143">일시 중지된 보고서의 UUID(범용 고유 식별자)</span><span class="sxs-lookup"><span data-stu-id="a8412-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="a8412-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="a8412-144">ReportName</span></span>     |    <span data-ttu-id="a8412-145">만드는 동안 보고서에 지정된 이름</span><span class="sxs-lookup"><span data-stu-id="a8412-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="a8412-146">Description</span><span class="sxs-lookup"><span data-stu-id="a8412-146">Description</span></span>     |    <span data-ttu-id="a8412-147">보고서를 만드는 동안 제공된 설명</span><span class="sxs-lookup"><span data-stu-id="a8412-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="a8412-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="a8412-148">QueryId</span></span>     |    <span data-ttu-id="a8412-149">보고서를 만들 때 전달된 쿼리 ID</span><span class="sxs-lookup"><span data-stu-id="a8412-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="a8412-150">쿼리</span><span class="sxs-lookup"><span data-stu-id="a8412-150">Query</span></span>     |    <span data-ttu-id="a8412-151">이 보고서에 대해 실행되는 쿼리 텍스트</span><span class="sxs-lookup"><span data-stu-id="a8412-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="a8412-152">사용자</span><span class="sxs-lookup"><span data-stu-id="a8412-152">User</span></span>     |    <span data-ttu-id="a8412-153">보고서를 만드는 데 사용되는 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="a8412-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="a8412-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a8412-154">CreatedTime</span></span>     |    <span data-ttu-id="a8412-155">보고서가 생성된 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-155">Time the report was created.</span></span> <span data-ttu-id="a8412-156">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8412-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a8412-157">ModifiedTime</span></span>     |    <span data-ttu-id="a8412-158">보고서를 마지막으로 수정한 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-158">Time the report was last modified.</span></span> <span data-ttu-id="a8412-159">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8412-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="a8412-160">ExecuteNow</span></span>     |    <span data-ttu-id="a8412-161">보고서를 만들 때 설정된 ExecuteNow 플래그</span><span class="sxs-lookup"><span data-stu-id="a8412-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="a8412-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="a8412-162">StartTime</span></span>     |    <span data-ttu-id="a8412-163">보고서 실행이 시작되는 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-163">Time the report execution will begin.</span></span> <span data-ttu-id="a8412-164">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8412-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="a8412-165">ReportStatus</span></span>     |    <span data-ttu-id="a8412-166">보고서 실행 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-166">Status of the report execution.</span></span> <span data-ttu-id="a8412-167">가능한 값은 일시 중지, 활성 및 비활성입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="a8412-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="a8412-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="a8412-169">보고서를 만드는 동안 제공된 되풀이 간격</span><span class="sxs-lookup"><span data-stu-id="a8412-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="a8412-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="a8412-170">RecurrenceCount</span></span>     |    <span data-ttu-id="a8412-171">보고서를 만드는 동안 제공된 되풀이 수</span><span class="sxs-lookup"><span data-stu-id="a8412-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="a8412-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a8412-172">CallbackUrl</span></span>     |    <span data-ttu-id="a8412-173">요청에 제공된 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="a8412-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="a8412-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a8412-174">CallbackMethod</span></span>    |    <span data-ttu-id="a8412-175">요청에 제공된 콜백 메서드</span><span class="sxs-lookup"><span data-stu-id="a8412-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="a8412-176">서식</span><span class="sxs-lookup"><span data-stu-id="a8412-176">Format</span></span>     |    <span data-ttu-id="a8412-177">보고서 파일 형식</span><span class="sxs-lookup"><span data-stu-id="a8412-177">Format of the report files</span></span>     |
|    <span data-ttu-id="a8412-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a8412-178">TotalCount</span></span>     |    <span data-ttu-id="a8412-179">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="a8412-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="a8412-180">메시지</span><span class="sxs-lookup"><span data-stu-id="a8412-180">Message</span></span>     |    <span data-ttu-id="a8412-181">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="a8412-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="a8412-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="a8412-182">StatusCode</span></span>     |    <span data-ttu-id="a8412-183">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-183">Result Code.</span></span> <span data-ttu-id="a8412-184">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="a8412-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
