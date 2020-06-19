---
title: Dynamics 365 Business Edition 마이그레이션
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 정식 Dynamics 365 Business Edition 제품을 최신 버전으로 마이그레이션하는 방법에 대해 알아봅니다.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 제안, 갱신 제안, 새 Dynamics 365 Sku
ms.openlocfilehash: 9675f607d183c5d427371de4f09f088fd267c573
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992076"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="0be76-104">Dynamics 365 Business Edition 제품을 최신 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="0be76-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="0be76-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="0be76-105">**Applies to**</span></span>

- <span data-ttu-id="0be76-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="0be76-106">Partner Center</span></span>

<span data-ttu-id="0be76-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="0be76-107">**Appropriate roles**</span></span>
- <span data-ttu-id="0be76-108">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="0be76-108">Global admin</span></span>
- <span data-ttu-id="0be76-109">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="0be76-109">User admin</span></span>
- <span data-ttu-id="0be76-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="0be76-110">Admin agent</span></span>
- <span data-ttu-id="0be76-111">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="0be76-111">Sales agent</span></span>

<span data-ttu-id="0be76-112">2019 년 1 월 1 일부 터 Dynamics 365 Business Edition 구독이 있는 고객은 더 이상 이러한 레거시 제품으로 갱신할 수 없습니다. 기존 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="0be76-113">구독의 세부 정보 페이지에서 구독 상태는 "[date]에 대 한 자동 갱신 [날짜]"에서 "만료 날짜 [날짜]"로 변경 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="0be76-114">고객의 연속성을 보장 하려면 구독 만료를 포함 하는 항목을 아래 나열 된 지원 되는 옵션으로 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="0be76-115">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="0be76-116">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="0be76-117">문제의 구독은 1 월 1 일 2019에 자동 갱신 = False로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="0be76-118">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="0be76-119">Dynamics 365 비즈니스 버전이 사용 중지 됨</span><span class="sxs-lookup"><span data-stu-id="0be76-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="0be76-120">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="0be76-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="0be76-121">Team Members, Business edition 용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="0be76-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="0be76-122">Dynamics Business Central-Dynamics 365 비즈니스 버전 새 제품</span><span class="sxs-lookup"><span data-stu-id="0be76-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="0be76-123">새 Dynamics Business Central 제품을 통해 고객은 financials, 영업, 서비스 및 작업을 연결 하 여 비즈니스 프로세스를 간소화 하 고 고객 상호 작용을 개선 하 고 더 나은 결정을 내릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="0be76-124">Dynamics 365 비즈니스 중부는 클라우드를 기반으로 하며, CSP (클라우드 솔루션 공급자) 프로그램 파트너를 통해서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="0be76-125">Dynamics 365 Business Edition 고객은 2020 30 년 6 월 30 일까 지 새로운 비즈니스 중앙 제품에 대해 할인 된 전환 가격을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="0be76-126">고객을 새 제품 요금제로 전환</span><span class="sxs-lookup"><span data-stu-id="0be76-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="0be76-127">사용 중지 된 Sku에서 최신 버전으로 고객을 이동 하려면 다음 단계를 순서 대로 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="0be76-128">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="0be76-128">Purchase the new subscription</span></span>
- <span data-ttu-id="0be76-129">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="0be76-129">Reassign current user licenses</span></span>
- <span data-ttu-id="0be76-130">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="0be76-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="0be76-131">고객에 대 한 새 요금제 구매</span><span class="sxs-lookup"><span data-stu-id="0be76-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="0be76-132">왼쪽 탐색 창에서 **고객** 을 선택한 다음 새 구독으로 이동할 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="0be76-133">**구독 추가**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="0be76-134">카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="0be76-135">이제 고객에 게 이전 구독과 새 구독이 모두 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="0be76-136">다음 단계는 고객의 사용자에 게 라이선스를 다시 할당 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="0be76-137">왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="0be76-138">**사용자 및 라이선스**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="0be76-139">사용자에 게 라이선스를 재할당 하려면 사용자를 선택한 다음 **라이선스 관리**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="0be76-140">**라이선스 관리** 페이지에서 기본 (우량 제안) 라이선스에서 판매/고객 지원 계획에 대 한 Dynamics 365을 지우고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="0be76-141">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-141">Select **Submit**.</span></span> <span data-ttu-id="0be76-142">새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="0be76-143">새 구독으로 라이선스를 이동한 후에는 이전 구독을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="0be76-144">왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="0be76-145">구독 정보 페이지에서 이전 구독을 **일시 중단 됨** 으로 설정 하 고 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="0be76-146">이제 이전 구독이 일시 중단 되 고 새 구독이 활성화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="0be76-147">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="0be76-148">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="0be76-148">Your customer will incur no additional costs for the old subscription.</span></span>
