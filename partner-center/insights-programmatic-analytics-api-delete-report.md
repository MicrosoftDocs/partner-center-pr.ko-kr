---
title: 보고서 API-Insights 데이터 삭제
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용 하 여 파트너 센터 정보에서 보고서를 삭제 합니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376140"
---
# <a name="delete-report-api"></a><span data-ttu-id="ead3a-103">보고서 API 삭제</span><span class="sxs-lookup"><span data-stu-id="ead3a-103">Delete report API</span></span>

<span data-ttu-id="ead3a-104">실행 시 이 API는 모든 보고서 및 보고서 실행 레코드를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="ead3a-105">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="ead3a-105">**Request syntax**</span></span>

|    <span data-ttu-id="ead3a-106">방법</span><span class="sxs-lookup"><span data-stu-id="ead3a-106">Method</span></span>    |    <span data-ttu-id="ead3a-107">요청 URI</span><span class="sxs-lookup"><span data-stu-id="ead3a-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ead3a-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="ead3a-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="ead3a-109">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="ead3a-109">**Request header**</span></span>

|    <span data-ttu-id="ead3a-110">헤더</span><span class="sxs-lookup"><span data-stu-id="ead3a-110">Header</span></span>    |    <span data-ttu-id="ead3a-111">유형</span><span class="sxs-lookup"><span data-stu-id="ead3a-111">Type</span></span>    |    <span data-ttu-id="ead3a-112">Description</span><span class="sxs-lookup"><span data-stu-id="ead3a-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ead3a-113">권한 부여</span><span class="sxs-lookup"><span data-stu-id="ead3a-113">Authorization</span></span>    |    <span data-ttu-id="ead3a-114">문자열</span><span class="sxs-lookup"><span data-stu-id="ead3a-114">string</span></span>    |    <span data-ttu-id="ead3a-115">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="ead3a-115">Required.</span></span> <span data-ttu-id="ead3a-116">형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ead3a-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ead3a-117">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="ead3a-117">Content-Type</span></span>    |    <span data-ttu-id="ead3a-118">문자열</span><span class="sxs-lookup"><span data-stu-id="ead3a-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ead3a-119">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="ead3a-119">**Path parameter**</span></span>

|    <span data-ttu-id="ead3a-120">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="ead3a-120">Parameter Name</span></span>    |    <span data-ttu-id="ead3a-121">유형</span><span class="sxs-lookup"><span data-stu-id="ead3a-121">Type</span></span>    |    <span data-ttu-id="ead3a-122">필수</span><span class="sxs-lookup"><span data-stu-id="ead3a-122">Required</span></span>    |    <span data-ttu-id="ead3a-123">Description</span><span class="sxs-lookup"><span data-stu-id="ead3a-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ead3a-124">reportId</span><span class="sxs-lookup"><span data-stu-id="ead3a-124">reportId</span></span>     |    <span data-ttu-id="ead3a-125">문자열</span><span class="sxs-lookup"><span data-stu-id="ead3a-125">string</span></span>    |    <span data-ttu-id="ead3a-126">예</span><span class="sxs-lookup"><span data-stu-id="ead3a-126">No</span></span>    |    <span data-ttu-id="ead3a-127">삭제할 보고서의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="ead3a-128">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="ead3a-128">**Query parameter**</span></span>

<span data-ttu-id="ead3a-129">없음</span><span class="sxs-lookup"><span data-stu-id="ead3a-129">None</span></span>

<span data-ttu-id="ead3a-130">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="ead3a-130">**Request payload**</span></span>

<span data-ttu-id="ead3a-131">없음</span><span class="sxs-lookup"><span data-stu-id="ead3a-131">None</span></span>

<span data-ttu-id="ead3a-132">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="ead3a-132">**Glossary**</span></span>

<span data-ttu-id="ead3a-133">없음</span><span class="sxs-lookup"><span data-stu-id="ead3a-133">None</span></span>

<span data-ttu-id="ead3a-134">**응답**</span><span class="sxs-lookup"><span data-stu-id="ead3a-134">**Response**</span></span>

<span data-ttu-id="ead3a-135">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="ead3a-136">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ead3a-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ead3a-137">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="ead3a-137">Response payload example:</span></span>

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

<span data-ttu-id="ead3a-138">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="ead3a-138">**Glossary**</span></span>

<span data-ttu-id="ead3a-139">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ead3a-140">매개 변수</span><span class="sxs-lookup"><span data-stu-id="ead3a-140">Parameter</span></span>    |    <span data-ttu-id="ead3a-141">Description</span><span class="sxs-lookup"><span data-stu-id="ead3a-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ead3a-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="ead3a-142">ReportId</span></span>     |    <span data-ttu-id="ead3a-143">삭제 보고서의 UUID(범용 고유 식별자)</span><span class="sxs-lookup"><span data-stu-id="ead3a-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="ead3a-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="ead3a-144">ReportName</span></span>     |    <span data-ttu-id="ead3a-145">만드는 동안 보고서에 지정된 이름</span><span class="sxs-lookup"><span data-stu-id="ead3a-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="ead3a-146">Description</span><span class="sxs-lookup"><span data-stu-id="ead3a-146">Description</span></span>     |    <span data-ttu-id="ead3a-147">보고서를 만드는 동안 제공된 설명</span><span class="sxs-lookup"><span data-stu-id="ead3a-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="ead3a-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="ead3a-148">QueryId</span></span>     |    <span data-ttu-id="ead3a-149">보고서를 만들 때 전달된 쿼리 ID</span><span class="sxs-lookup"><span data-stu-id="ead3a-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="ead3a-150">쿼리</span><span class="sxs-lookup"><span data-stu-id="ead3a-150">Query</span></span>     |    <span data-ttu-id="ead3a-151">이 보고서에 대해 실행되는 쿼리 텍스트</span><span class="sxs-lookup"><span data-stu-id="ead3a-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="ead3a-152">사용자</span><span class="sxs-lookup"><span data-stu-id="ead3a-152">User</span></span>     |    <span data-ttu-id="ead3a-153">보고서를 만드는 데 사용되는 사용자 ID</span><span class="sxs-lookup"><span data-stu-id="ead3a-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="ead3a-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ead3a-154">CreatedTime</span></span>     |    <span data-ttu-id="ead3a-155">보고서가 생성된 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-155">Time the report was created.</span></span> <span data-ttu-id="ead3a-156">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ead3a-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ead3a-157">ModifiedTime</span></span>     |    <span data-ttu-id="ead3a-158">보고서를 마지막으로 수정한 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-158">Time the report was last modified.</span></span> <span data-ttu-id="ead3a-159">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ead3a-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ead3a-160">ExecuteNow</span></span>     |    <span data-ttu-id="ead3a-161">보고서를 만들 때 설정 되는 ExecuteNow 플래그</span><span class="sxs-lookup"><span data-stu-id="ead3a-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="ead3a-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="ead3a-162">StartTime</span></span>     |    <span data-ttu-id="ead3a-163">보고서 실행이 시작되는 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-163">Time the report execution will begin.</span></span> <span data-ttu-id="ead3a-164">시간 형식은 yyyy-MM-ddTHH:mm:ssZ입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ead3a-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="ead3a-165">ReportStatus</span></span>     |    <span data-ttu-id="ead3a-166">보고서 실행 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-166">Status of the report execution.</span></span> <span data-ttu-id="ead3a-167">가능한 값은 일시 중지, 활성 및 비활성입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="ead3a-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="ead3a-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="ead3a-169">보고서를 만드는 동안 제공된 되풀이 간격</span><span class="sxs-lookup"><span data-stu-id="ead3a-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="ead3a-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="ead3a-170">RecurrenceCount</span></span>     |    <span data-ttu-id="ead3a-171">보고서를 만드는 동안 제공된 되풀이 수</span><span class="sxs-lookup"><span data-stu-id="ead3a-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="ead3a-172">콜백 url</span><span class="sxs-lookup"><span data-stu-id="ead3a-172">CallbackUrl</span></span>     |    <span data-ttu-id="ead3a-173">요청에 제공된 콜백 URL</span><span class="sxs-lookup"><span data-stu-id="ead3a-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="ead3a-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="ead3a-174">CallbackMethod</span></span>    |    <span data-ttu-id="ead3a-175">요청에 제공 된 콜백 메서드입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="ead3a-176">서식</span><span class="sxs-lookup"><span data-stu-id="ead3a-176">Format</span></span>     |    <span data-ttu-id="ead3a-177">보고서 파일 형식</span><span class="sxs-lookup"><span data-stu-id="ead3a-177">Format of the report files</span></span>     |
|    <span data-ttu-id="ead3a-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ead3a-178">TotalCount</span></span>     |    <span data-ttu-id="ead3a-179">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="ead3a-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ead3a-180">메시지</span><span class="sxs-lookup"><span data-stu-id="ead3a-180">Message</span></span>     |    <span data-ttu-id="ead3a-181">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="ead3a-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ead3a-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="ead3a-182">StatusCode</span></span>     |    <span data-ttu-id="ead3a-183">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-183">Result Code.</span></span> <span data-ttu-id="ead3a-184">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="ead3a-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
