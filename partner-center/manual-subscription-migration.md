---
title: 정규화 된 Dynamics 365 구독 마이그레이션
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 기존 구독이 만료 되기 전에 정규화 된 기본 Dynamics 365 구독에서 새 구독으로 마이그레이션하는 방법에 대해 알아봅니다.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 제안, 갱신 제안, 새 Dynamics 365 Sku
ms.openlocfilehash: 5225ff60399cd491009ecb16e4c17b4fc05c0052
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949642"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="74e04-104">Dynamics 365 및 Customer Engagement 플랜을 기본(제한된 제품)에서 새 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="74e04-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="74e04-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="74e04-105">**Applies to**</span></span>

-  <span data-ttu-id="74e04-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="74e04-106">Partner Center</span></span>

<span data-ttu-id="74e04-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="74e04-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="74e04-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="74e04-108">Global admin</span></span>
-   <span data-ttu-id="74e04-109">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="74e04-109">User admin</span></span>
-   <span data-ttu-id="74e04-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="74e04-110">Admin agent</span></span>
-   <span data-ttu-id="74e04-111">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="74e04-111">Sales agent</span></span>

<span data-ttu-id="74e04-112">2019 년 1 월 1 일부 터 기본 (우량 제안) 구독의 판매/고객 참여 요금제에 대 한 Dynamics 365이 있는 고객은 이러한 레거시 제안을 더 이상 갱신할 수 없습니다. 기존 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="74e04-113">구독의 세부 정보 페이지에서 구독 상태는 "[date]에 대 한 자동 갱신 [날짜]"에서 "만료 날짜 [날짜]"로 변경 됩니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="74e04-114">고객의 연속성을 보장 하려면 구독 만료를 포함 하는 항목을 아래 나열 된 지원 되는 옵션으로 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="74e04-115">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="74e04-116">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="74e04-117">문제의 구독은 1 월 1 일 2019에 자동 갱신 = False로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="74e04-118">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="74e04-119">Dynamics 365 제공이 사용 중지 됨</span><span class="sxs-lookup"><span data-stu-id="74e04-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="74e04-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="74e04-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-121">교직원 용 Dynamics 365 for Sales Enterprise Edition CRMOL 기본 (우량 제안)</span><span class="sxs-lookup"><span data-stu-id="74e04-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="74e04-122">학생을 위한 Dynamics 365 for Sales Enterprise Edition CRMOL Basic (우량 제안)</span><span class="sxs-lookup"><span data-stu-id="74e04-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="74e04-123">Dynamics 365 for Sales Enterprise Edition (정부 가격) CRMOL 기본 (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="74e04-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-124">CRM Basic (정규화 된 제품)의 경우 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="74e04-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-125">교직원 용 Dynamics 365 for CRM Basic (우량 제안) for 교직원</span><span class="sxs-lookup"><span data-stu-id="74e04-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="74e04-126">학생의 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise 버전용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="74e04-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="74e04-127">CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 for Sales Enterprise Edition (정부 가격)</span><span class="sxs-lookup"><span data-stu-id="74e04-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-128">CRM Basic (정규화 된 제품) 용 Dynamics 365 for Sales Enterprise Edition 추가 기능</span><span class="sxs-lookup"><span data-stu-id="74e04-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-129">교직원 용 Dynamics 365 for CRM Basic (우량 제안) for 교직원</span><span class="sxs-lookup"><span data-stu-id="74e04-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="74e04-130">학생용 CRM Basic (우량 제안) 용 Dynamics 365 for Sales Enterprise Edition 추가 기능</span><span class="sxs-lookup"><span data-stu-id="74e04-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="74e04-131">CRM Basic (정규화 된 제품) 용 Dynamics 365 for Sales Enterprise Edition (정부 가격) 추가 기능</span><span class="sxs-lookup"><span data-stu-id="74e04-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="74e04-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (정부 가격) CRMOL 기본 (적격 제안)</span><span class="sxs-lookup"><span data-stu-id="74e04-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-134">학생용 Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (우량 제안)</span><span class="sxs-lookup"><span data-stu-id="74e04-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="74e04-135">교직원 용 Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (적격 제안)</span><span class="sxs-lookup"><span data-stu-id="74e04-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="74e04-136">Dynamics 365 Customer Engagement Plan for SA에서 CRM Basic (정규화 된 제품)에 대 한 엔터프라이즈 버전</span><span class="sxs-lookup"><span data-stu-id="74e04-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-137">CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 요금제 Enterprise Edition (정부 가격)</span><span class="sxs-lookup"><span data-stu-id="74e04-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-138">Dynamics 365 Customer Engagement Plan for SA에서 학생용 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="74e04-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="74e04-139">Dynamics 365 고객 Engagement 요금제의 SA에서 교직원 용 CRM Basic (정규화 된 제품)에 대 한 엔터프라이즈 버전</span><span class="sxs-lookup"><span data-stu-id="74e04-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="74e04-140">CRM Basic (정규화 된 제품) 용 Dynamics 365 Customer Engagement Plan Enterprise Edition 추가 기능</span><span class="sxs-lookup"><span data-stu-id="74e04-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-141">CRM Basic (정규화 된 제품) 용 Dynamics 365 고객 Engagement 계획 Enterprise Edition (정부 가격) 추가 기능</span><span class="sxs-lookup"><span data-stu-id="74e04-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-142">학생용 CRM Basic (정규화 된 제품) 용 Dynamics 365 고객 Engagement 계획 Enterprise Edition 추가 기능</span><span class="sxs-lookup"><span data-stu-id="74e04-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="74e04-143">교직원 용 Dynamics 365 Customer Engagement 계획 Enterprise Edition 추가 기능 (교직원 용 정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="74e04-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="74e04-144">기본 (우량 제안) 대체 요금제에서 판매/고객 참여 요금제에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="74e04-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="74e04-145">**사용 중지 된 제안**</span><span class="sxs-lookup"><span data-stu-id="74e04-145">**Retired offers**</span></span>   

- <span data-ttu-id="74e04-146">CRM Basic 또는 CRMOL Basic (정규화 된 제안)에서 판매에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="74e04-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="74e04-147">CRM Basic 또는 CRMOL Basic (정규화 된 제품)의 Dynamics 365 Customer Engagement 계획</span><span class="sxs-lookup"><span data-stu-id="74e04-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="74e04-148">**대체 옵션**</span><span class="sxs-lookup"><span data-stu-id="74e04-148">**Replacement options**</span></span>
- <span data-ttu-id="74e04-149">Dynamics 365 for Sales Professional (신규)</span><span class="sxs-lookup"><span data-stu-id="74e04-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="74e04-150">Dynamics 365 for Sales Professional (신규)</span><span class="sxs-lookup"><span data-stu-id="74e04-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="74e04-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="74e04-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="74e04-152">Dynamics 365 Customer Engagement 요금제 또는</span><span class="sxs-lookup"><span data-stu-id="74e04-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="74e04-153">Dynamics 365 팀 멤버</span><span class="sxs-lookup"><span data-stu-id="74e04-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="74e04-154">고객을 새 제품 요금제로 전환</span><span class="sxs-lookup"><span data-stu-id="74e04-154">Transition customers to new product plans</span></span>

<span data-ttu-id="74e04-155">사용 중지 된 Sku에서 최신 버전으로 고객을 이동 하려면 다음 단계를 순서 대로 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="74e04-156">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="74e04-156">Purchase the new subscription</span></span>
- <span data-ttu-id="74e04-157">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="74e04-157">Reassign current user licenses</span></span>
- <span data-ttu-id="74e04-158">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="74e04-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="74e04-159">고객에 대 한 새 요금제 구매</span><span class="sxs-lookup"><span data-stu-id="74e04-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="74e04-160">왼쪽 탐색 창에서 **고객** 을 선택한 다음 새 구독으로 이동할 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="74e04-161">**구독 추가**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="74e04-162">카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="74e04-163">이제 고객에 게 이전 구독과 새 구독이 모두 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="74e04-164">다음 단계는 고객의 사용자에 게 라이선스를 다시 할당 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="74e04-165">왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="74e04-166">**사용자 및 라이선스**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="74e04-167">사용자에 게 라이선스를 재할당 하려면 사용자를 선택한 다음 **라이선스 관리**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="74e04-168">**라이선스 관리** 페이지에서 기본 (우량 제안) 라이선스에서 판매/고객 지원 계획에 대 한 Dynamics 365을 지우고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="74e04-169">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-169">Select **Submit**.</span></span> <span data-ttu-id="74e04-170">새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="74e04-171">새 구독으로 라이선스를 이동한 후에는 이전 구독을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="74e04-172">왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="74e04-173">구독 정보 페이지에서 이전 구독을 **일시 중단 됨** 으로 설정 하 고 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="74e04-174">이제 이전 구독이 일시 중단 되 고 새 구독이 활성화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="74e04-175">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="74e04-176">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e04-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



