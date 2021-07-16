---
title: 모든 데이터 집합 API 가져오기-Insights 데이터
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 API를 사용 하 여 파트너 센터 정보에서 사용 가능한 모든 데이터 집합에 대 한 세부 정보를 가져옵니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375869"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="89337-103">모든 데이터 세트 API 가져오기</span><span class="sxs-lookup"><span data-stu-id="89337-103">Get all datasets API</span></span>

<span data-ttu-id="89337-104">모든 데이터 세트 API 가져오기는 사용 가능한 데이터 세트를 모두 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="89337-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="89337-105">데이터 세트는 테이블, 열, 메트릭, 시간 범위를 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="89337-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="89337-106">**요청 구문**</span><span class="sxs-lookup"><span data-stu-id="89337-106">**Request syntax**</span></span>

|    <span data-ttu-id="89337-107">방법</span><span class="sxs-lookup"><span data-stu-id="89337-107">Method</span></span>    |    <span data-ttu-id="89337-108">요청 URI</span><span class="sxs-lookup"><span data-stu-id="89337-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="89337-109">GET</span><span class="sxs-lookup"><span data-stu-id="89337-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="89337-110">**요청 헤더**</span><span class="sxs-lookup"><span data-stu-id="89337-110">**Request header**</span></span>

|    <span data-ttu-id="89337-111">헤더</span><span class="sxs-lookup"><span data-stu-id="89337-111">Header</span></span>    |    <span data-ttu-id="89337-112">유형</span><span class="sxs-lookup"><span data-stu-id="89337-112">Type</span></span>    |    <span data-ttu-id="89337-113">Description</span><span class="sxs-lookup"><span data-stu-id="89337-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="89337-114">권한 부여</span><span class="sxs-lookup"><span data-stu-id="89337-114">Authorization</span></span>    |    <span data-ttu-id="89337-115">문자열</span><span class="sxs-lookup"><span data-stu-id="89337-115">string</span></span>    |    <span data-ttu-id="89337-116">필수 요소.</span><span class="sxs-lookup"><span data-stu-id="89337-116">Required.</span></span> <span data-ttu-id="89337-117">형식의 AAD (Azure Active Directory) 액세스 토큰`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="89337-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="89337-118">콘텐츠 형식</span><span class="sxs-lookup"><span data-stu-id="89337-118">Content-Type</span></span>    |    <span data-ttu-id="89337-119">문자열</span><span class="sxs-lookup"><span data-stu-id="89337-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="89337-120">**경로 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="89337-120">**Path parameter**</span></span>

<span data-ttu-id="89337-121">없음</span><span class="sxs-lookup"><span data-stu-id="89337-121">None</span></span>

<span data-ttu-id="89337-122">**쿼리 매개 변수**</span><span class="sxs-lookup"><span data-stu-id="89337-122">**Query parameter**</span></span>

|    <span data-ttu-id="89337-123">매개 변수 이름</span><span class="sxs-lookup"><span data-stu-id="89337-123">Parameter Name</span></span>    |    <span data-ttu-id="89337-124">유형</span><span class="sxs-lookup"><span data-stu-id="89337-124">Type</span></span>    |    <span data-ttu-id="89337-125">필수</span><span class="sxs-lookup"><span data-stu-id="89337-125">Required</span></span>    |    <span data-ttu-id="89337-126">Description</span><span class="sxs-lookup"><span data-stu-id="89337-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="89337-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="89337-127">datasetName</span></span>    |    <span data-ttu-id="89337-128">문자열</span><span class="sxs-lookup"><span data-stu-id="89337-128">string</span></span>    |    <span data-ttu-id="89337-129">No</span><span class="sxs-lookup"><span data-stu-id="89337-129">No</span></span>    |    <span data-ttu-id="89337-130">하나의 데이터 세트에 대한 세부 정보만 가져오도록 필터링</span><span class="sxs-lookup"><span data-stu-id="89337-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="89337-131">**요청 페이로드**</span><span class="sxs-lookup"><span data-stu-id="89337-131">**Request payload**</span></span>

<span data-ttu-id="89337-132">없음</span><span class="sxs-lookup"><span data-stu-id="89337-132">None</span></span>

<span data-ttu-id="89337-133">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="89337-133">**Glossary**</span></span>

<span data-ttu-id="89337-134">없음</span><span class="sxs-lookup"><span data-stu-id="89337-134">None</span></span>

<span data-ttu-id="89337-135">**응답**</span><span class="sxs-lookup"><span data-stu-id="89337-135">**Response**</span></span>

<span data-ttu-id="89337-136">응답 페이로드는 다음과 같이 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="89337-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="89337-137">응답 코드: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="89337-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="89337-138">응답 페이로드 예제:</span><span class="sxs-lookup"><span data-stu-id="89337-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="89337-139">**용어 설명**</span><span class="sxs-lookup"><span data-stu-id="89337-139">**Glossary**</span></span>

<span data-ttu-id="89337-140">다음 표에서는 응답의 주요 요소를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="89337-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="89337-141">매개 변수</span><span class="sxs-lookup"><span data-stu-id="89337-141">Parameter</span></span>    |    <span data-ttu-id="89337-142">Description</span><span class="sxs-lookup"><span data-stu-id="89337-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="89337-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="89337-143">DatasetName</span></span>     |    <span data-ttu-id="89337-144">이 배열 개체가 정의하는 데이터 세트의 이름</span><span class="sxs-lookup"><span data-stu-id="89337-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="89337-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="89337-145">SelectableColumns</span></span>     |    <span data-ttu-id="89337-146">선택 열에서 지정할 수 있는 원시 열</span><span class="sxs-lookup"><span data-stu-id="89337-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="89337-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="89337-147">AvailableMetrics</span></span>     |    <span data-ttu-id="89337-148">선택 열에서 지정할 수 있는 집계/메트릭 열 이름</span><span class="sxs-lookup"><span data-stu-id="89337-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="89337-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="89337-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="89337-150">데이터 세트에 대한 보고서 쿼리에서 사용할 수 있는 날짜 범위</span><span class="sxs-lookup"><span data-stu-id="89337-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="89337-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="89337-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="89337-152">되풀이 간격의 최 솟 값</span><span class="sxs-lookup"><span data-stu-id="89337-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="89337-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="89337-153">TotalCount</span></span>     |    <span data-ttu-id="89337-154">값 배열의 데이터 세트 수</span><span class="sxs-lookup"><span data-stu-id="89337-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="89337-155">메시지</span><span class="sxs-lookup"><span data-stu-id="89337-155">Message</span></span>     |    <span data-ttu-id="89337-156">API 실행의 상태 메시지</span><span class="sxs-lookup"><span data-stu-id="89337-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="89337-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="89337-157">StatusCode</span></span>     |    <span data-ttu-id="89337-158">결과 코드입니다.</span><span class="sxs-lookup"><span data-stu-id="89337-158">Result Code.</span></span> <span data-ttu-id="89337-159">가능한 값은 200, 400, 401, 403, 500입니다.</span><span class="sxs-lookup"><span data-stu-id="89337-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
