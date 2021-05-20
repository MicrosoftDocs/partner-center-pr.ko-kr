---
title: 간접 재판매인 성과 분석
description: 분석을 사용 하 여 간접 재판매인이 수행 하는 작업을 파악 하 고, 성공 및 영역에서 더 많은 주의가 필요할 수 있습니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh
ms.author: shganesh
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/13/2020
ms.openlocfilehash: 50a527f8fd3690ff73b198e572b356706889e72b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150185"
---
# <a name="use-analytics-to-analyze-the-performance-of-your-indirect-resellers"></a><span data-ttu-id="342ce-103">분석을 사용 하 여 간접 대리점의 성능 분석</span><span class="sxs-lookup"><span data-stu-id="342ce-103">Use analytics to analyze the performance of your indirect resellers</span></span>

<span data-ttu-id="342ce-104">**적절 한 역할**: 전역 관리자 | 사용자 관리 관리자</span><span class="sxs-lookup"><span data-stu-id="342ce-104">**Appropriate roles**: Global admin | User management admin</span></span>


<span data-ttu-id="342ce-105">데이터는 비즈니스 의사 결정을 유도 합니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-105">Data drives business decisions.</span></span> <span data-ttu-id="342ce-106">**재판매인 분석** 페이지의 메트릭을 사용 하 여 성공, 간접 재판매인의 성공 및 주의가 필요한 영역을 식별할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-106">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="342ce-107">새 비즈니스 목표를 계획할 때이 정보를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-107">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="342ce-108">간접 재판매인 분석은 클라우드 솔루션 공급자 프로그램의 간접 공급자에 대해서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-108">Indirect reseller analytics is available only for Indirect providers in the Cloud Solution Provider program.</span></span>

## <a name="types-of-reseller-analytics-metrics-you-can-view"></a><span data-ttu-id="342ce-109">볼 수 있는 재판매인 분석 메트릭 유형</span><span class="sxs-lookup"><span data-stu-id="342ce-109">Types of reseller analytics metrics you can view</span></span>

<span data-ttu-id="342ce-110">다음 메트릭을 추적 합니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-110">We are tracking the following metrics:</span></span>

<span data-ttu-id="342ce-111">**요약**</span><span class="sxs-lookup"><span data-stu-id="342ce-111">**Summary**</span></span>  
 - <span data-ttu-id="342ce-112">**총 대리점**: 구독의 마지막 날에 활성화 된 대리점 수</span><span class="sxs-lookup"><span data-stu-id="342ce-112">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="342ce-113">**새 대리점**: 지정 된 기간에 대 한 새 간접 대리점 수</span><span class="sxs-lookup"><span data-stu-id="342ce-113">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="342ce-114">**활성 대리점**: MPNID이 하나 이상의 구독 이며 구독 상태가 프로 비전 해제이 아닌 간접 대리점의 수</span><span class="sxs-lookup"><span data-stu-id="342ce-114">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="342ce-115">**거래** 재판매인: 지정 된 기간에 판매 된 구독이 있는 간접 대리점의 수</span><span class="sxs-lookup"><span data-stu-id="342ce-115">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="342ce-116">**시장의 대리점**</span><span class="sxs-lookup"><span data-stu-id="342ce-116">**Resellers by market**</span></span>  
 - <span data-ttu-id="342ce-117">지리적 위치별 총 대리점</span><span class="sxs-lookup"><span data-stu-id="342ce-117">Total resellers by geographic location</span></span>  

<span data-ttu-id="342ce-118">**판매 된 구독의 상위 대리점**</span><span class="sxs-lookup"><span data-stu-id="342ce-118">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="342ce-119">판매 된 구독 수를 기준으로 정렬 된 대리점 목록</span><span class="sxs-lookup"><span data-stu-id="342ce-119">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="342ce-120">**구독 수 별 상위 제품**</span><span class="sxs-lookup"><span data-stu-id="342ce-120">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="342ce-121">**Dynamics 365**: 판매 된 구독 별로 정렬 된 dynamics 365 제품</span><span class="sxs-lookup"><span data-stu-id="342ce-121">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="342ce-122">**EMS**: 판매 된 엔터프라이즈 관리 서비스 구독 수</span><span class="sxs-lookup"><span data-stu-id="342ce-122">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="342ce-123">**Microsoft 365:** 판매된 Microsoft 365 구독 수</span><span class="sxs-lookup"><span data-stu-id="342ce-123">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="342ce-124">**Office 365:** 판매된 구독별로 정렬된 Office 365 제품</span><span class="sxs-lookup"><span data-stu-id="342ce-124">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="342ce-125">**새 구독**</span><span class="sxs-lookup"><span data-stu-id="342ce-125">**New subscriptions**</span></span>  
 - <span data-ttu-id="342ce-126">날짜별로 추가된 새 구독 수</span><span class="sxs-lookup"><span data-stu-id="342ce-126">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="342ce-127">**구독 변동**</span><span class="sxs-lookup"><span data-stu-id="342ce-127">**Subscription churn**</span></span>  
 - <span data-ttu-id="342ce-128">**새 구독:** 날짜별로 추가된 새 구독 수</span><span class="sxs-lookup"><span data-stu-id="342ce-128">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="342ce-129">**프로비전 해제된 구독:** 날짜별로 프로비전 해제되거나 일시 중단된 구독 수</span><span class="sxs-lookup"><span data-stu-id="342ce-129">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="342ce-130">**새 대리점 세부 정보**</span><span class="sxs-lookup"><span data-stu-id="342ce-130">**New reseller details**</span></span>  
 - <span data-ttu-id="342ce-131">**Reseller name:** 간접 대리점의 이름</span><span class="sxs-lookup"><span data-stu-id="342ce-131">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="342ce-132">**위치:** 간접 대리점이 운영하는 시장</span><span class="sxs-lookup"><span data-stu-id="342ce-132">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="342ce-133">**구독:** 대리점에서 판매한 구독 수</span><span class="sxs-lookup"><span data-stu-id="342ce-133">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="342ce-134">**라이선스:** 대리점이 모든 구독에서 판매한 총 라이선스 수</span><span class="sxs-lookup"><span data-stu-id="342ce-134">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  

<span data-ttu-id="342ce-135">**MPA 서명 상태**</span><span class="sxs-lookup"><span data-stu-id="342ce-135">**MPA signed status**</span></span>

<span data-ttu-id="342ce-136">이 섹션에서는 CSP 간접 대리점의 MPA 서명 상태 상태를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-136">This section provides the status of MPA signed status of the CSP Indirect Resellers.</span></span>

 - <span data-ttu-id="342ce-137">**대리점 이름:** CSP 간접 대리점의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-137">**Reseller name**: Name of the CSP indirect reseller</span></span>
 - <span data-ttu-id="342ce-138">**MPN ID:** 간접 대리점의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="342ce-138">**MPN ID**: MPN ID of the indirect reseller</span></span>
 - <span data-ttu-id="342ce-139">**지역:** 간접 대리점이 작동하는 지역</span><span class="sxs-lookup"><span data-stu-id="342ce-139">**Region**: Region where the indirect reseller operates</span></span>
 - <span data-ttu-id="342ce-140">**MPN 심사 상태:** 간접 대리점의 심사 상태</span><span class="sxs-lookup"><span data-stu-id="342ce-140">**MPN vetting status**: Vetting status of the indirect reseller</span></span>
 - <span data-ttu-id="342ce-141">**MPA 서명 상태:** 간접 대리점에 대한 MPA 서명 상태</span><span class="sxs-lookup"><span data-stu-id="342ce-141">**MPA signed status**: MPA signing status for the indirect reseller</span></span>

<span data-ttu-id="342ce-142">차트에서 다운로드 아이콘을 클릭하여 추가 차원이 있는 MPA 서명된 상태 데이터를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="342ce-142">Click on the download icon in the chart to download MPA signed status data with additional dimensions</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="342ce-143">다음 단계</span><span class="sxs-lookup"><span data-stu-id="342ce-143">Next steps</span></span>

- [<span data-ttu-id="342ce-144">비즈니스 의사 결정을 내리는 데 도움이 되는 구독 및 라이선스 분석</span><span class="sxs-lookup"><span data-stu-id="342ce-144">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)