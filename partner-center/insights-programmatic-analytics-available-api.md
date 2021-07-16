---
title: 파트너 insights 데이터에 액세스 하기 위한 API 목록
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 insights 데이터에 액세스 하기 위한 API 목록입니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376077"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="6a1a0-103">파트너 통찰력 분석에 사용할 수 있는 Api</span><span class="sxs-lookup"><span data-stu-id="6a1a0-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="6a1a0-104">다음은 파트너 insights 분석과 관련 기능에 대 한 Api 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="6a1a0-105">데이터 세트 풀하기 API</span><span class="sxs-lookup"><span data-stu-id="6a1a0-105">Dataset pull APIs</span></span>

<span data-ttu-id="6a1a0-106">***표 1: 데이터 세트 풀하기 API***</span><span class="sxs-lookup"><span data-stu-id="6a1a0-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="6a1a0-107">**API**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-107">**API**</span></span> | <span data-ttu-id="6a1a0-108">**기능**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="6a1a0-109">모든 데이터 세트 가져오기</span><span class="sxs-lookup"><span data-stu-id="6a1a0-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="6a1a0-110">사용 가능한 데이터 세트를 모두 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-110">Gets all the available datasets.</span></span> <span data-ttu-id="6a1a0-111">데이터 세트는 테이블, 열, 메트릭, 시간 범위를 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="6a1a0-112">쿼리 관리 API</span><span class="sxs-lookup"><span data-stu-id="6a1a0-112">Query management APIs</span></span>

<span data-ttu-id="6a1a0-113">***표 2: 쿼리 관리 API***</span><span class="sxs-lookup"><span data-stu-id="6a1a0-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="6a1a0-114">**API**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-114">**API**</span></span> | <span data-ttu-id="6a1a0-115">**기능**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="6a1a0-116">보고서 쿼리 만들기</span><span class="sxs-lookup"><span data-stu-id="6a1a0-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="6a1a0-117">열과 메트릭을 내보내야 하는 데이터 세트를 정의하는 사용자 지정 쿼리를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="6a1a0-118">보고서 쿼리 가져오기</span><span class="sxs-lookup"><span data-stu-id="6a1a0-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="6a1a0-119">보고서에서 사용할 수 있는 모든 쿼리를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="6a1a0-120">기본적으로 모든 시스템 및 사용자 정의 쿼리를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="6a1a0-121">보고서 쿼리 삭제</span><span class="sxs-lookup"><span data-stu-id="6a1a0-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="6a1a0-122">사용자 정의 쿼리를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="6a1a0-123">보고서 관리 API</span><span class="sxs-lookup"><span data-stu-id="6a1a0-123">Report management APIs</span></span>

<span data-ttu-id="6a1a0-124">***표 3: 보고서 관리 API***</span><span class="sxs-lookup"><span data-stu-id="6a1a0-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="6a1a0-125">**API**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-125">**API**</span></span> | <span data-ttu-id="6a1a0-126">**기능**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="6a1a0-127">보고서 만들기</span><span class="sxs-lookup"><span data-stu-id="6a1a0-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="6a1a0-128">정기적으로 쿼리를 실행하도록 예약합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="6a1a0-129">보고서 쿼리 시도</span><span class="sxs-lookup"><span data-stu-id="6a1a0-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="6a1a0-130">보고서 쿼리 문을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-130">Executes a Report query statement.</span></span> <span data-ttu-id="6a1a0-131">데이터가 예상한 대로인지 확인하는 데 파트너가 사용할 수 있는 10개의 레코드만 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="6a1a0-132">보고서 가져오기</span><span class="sxs-lookup"><span data-stu-id="6a1a0-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="6a1a0-133">예약된 모든 보고서를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="6a1a0-134">보고서 업데이트</span><span class="sxs-lookup"><span data-stu-id="6a1a0-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="6a1a0-135">보고서 매개 변수를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="6a1a0-136">보고서 삭제</span><span class="sxs-lookup"><span data-stu-id="6a1a0-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="6a1a0-137">모든 보고서 및 보고서 실행 레코드를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="6a1a0-138">보고서 실행 일시 중지</span><span class="sxs-lookup"><span data-stu-id="6a1a0-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="6a1a0-139">예약된 보고서 실행을 일시 중지합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="6a1a0-140">보고서 실행 계속</span><span class="sxs-lookup"><span data-stu-id="6a1a0-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="6a1a0-141">일시 중지된 보고서의 예약된 실행을 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="6a1a0-142">보고서 실행 풀하기 API</span><span class="sxs-lookup"><span data-stu-id="6a1a0-142">Report execution pull APIs</span></span>

<span data-ttu-id="6a1a0-143">***표 4: 보고서 실행 풀하기 API***</span><span class="sxs-lookup"><span data-stu-id="6a1a0-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="6a1a0-144">**API**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-144">**API**</span></span> | <span data-ttu-id="6a1a0-145">**기능**</span><span class="sxs-lookup"><span data-stu-id="6a1a0-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="6a1a0-146">보고서 실행 가져오기</span><span class="sxs-lookup"><span data-stu-id="6a1a0-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="6a1a0-147">지정된 보고서에 대해 발생한 모든 실행을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="6a1a0-148">다음 단계</span><span class="sxs-lookup"><span data-stu-id="6a1a0-148">Next steps</span></span>

- <span data-ttu-id="6a1a0-149">[Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)을 통해 API를 사용해 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a0-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>