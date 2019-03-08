---
title: Basic (정규화 된 제품)에서 Dynamics 365 Customer Engagement 계획 하 고를 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Basic (정규화 된 제공) 구독에서 고객 참여 계획 갱신할 수 없습니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 제품의 제품에 새 Dynamics 365 Sku 갱신
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586946"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="28225-104">Dynamics 365 및 Customer Engagement Plan을 기본 (정규화된 제안)에서 새 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="28225-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="28225-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="28225-105">**Applies to**</span></span>

-  <span data-ttu-id="28225-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="28225-106">Partner Center</span></span>

<span data-ttu-id="28225-107">Dynamics 365 for Sales 사용 하 여 효과적인 2019 년 1 월 1 일 고객 / Basic (정규화 된 제공) 구독에서 고객 참여 계획 수 이러한 레거시 제품; 갱신할 이상 만료 시 기존 구독을 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="28225-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="28225-108">구독 세부 정보 페이지에서 구독 상태를 "[date]에 자동 갱신"에서 "[date]에 만료"에 변경 됩니다.</span><span class="sxs-lookup"><span data-stu-id="28225-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="28225-109">고객에 대 한 연속성을 위해 아래에 나열 된 지원 되는 옵션에 대 한 구독을 만료를 사용 하 여 해당 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="28225-110">고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="28225-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="28225-111">자동 함께 구독 종료 날짜를 평가 하 여 만료 구독을 갱신 찾을 수 있습니다 (CREST 또는 파트너 센터) API를 사용 하는 경우 = False 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="28225-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="28225-112">해당 구독이 자동으로 설정 됩니다 갱신 2019 년 1 월 1 일에서 = False.</span><span class="sxs-lookup"><span data-stu-id="28225-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="28225-113">언제든지 고객을 새 요금제로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="28225-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="28225-114">Dynamics 365 사용이 중지 되는 제공</span><span class="sxs-lookup"><span data-stu-id="28225-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="28225-115">Dynamics 365 for Sales Enterprise Edition CRMOL 기본 (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-116">교직원 용 판매 Enterprise Edition CRMOL Basic (정규화 된 제품)에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="28225-117">학생을 위한 판매 Enterprise Edition CRMOL Basic (정규화 된 제품)에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="28225-118">Dynamics 365 for Sales Enterprise Edition (정부 기관용 가격 책정) CRMOL 기본 (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-119">CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise Edition 용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-120">교직원 용 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise Edition 용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="28225-121">학생을 위한 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise Edition 용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="28225-122">CRM Basic (정규화 된 제품)에 대 한 SA의 (정부 기관용 가격 책정) 판매 Enterprise Edition 용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-123">CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-124">교직원 용 CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="28225-125">학생을 위한 CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="28225-126">CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition (정부 기관용 가격 책정) 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="28225-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-127">Dynamics 365 Customer Engagement 계획 Enterprise Edition CRMOL Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-128">Dynamics 365 Customer Engagement 계획 Enterprise Edition (정부 기관용 가격 책정) CRMOL Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-129">Dynamics 365 Customer Engagement 계획 Enterprise Edition CRMOL Basic (정규화 된 제품) 학생용</span><span class="sxs-lookup"><span data-stu-id="28225-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="28225-130">Dynamics 365 Customer Engagement 계획 Enterprise Edition CRMOL Basic (정규화 된 제품) 교직원 용</span><span class="sxs-lookup"><span data-stu-id="28225-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="28225-131">CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 계획 Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="28225-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-132">Dynamics 365 Customer Engagement 계획 Enterprise Edition (정부 기관용 가격 책정) CRM Basic (정규화 된 제품)에 대 한 SA의</span><span class="sxs-lookup"><span data-stu-id="28225-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-133">학생을 위한 CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 계획 Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="28225-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="28225-134">교직원 용 CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 계획 Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="28225-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="28225-135">Dynamics 365 Customer Engagement 계획 Enterprise Edition 용 추가 기능 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-136">Dynamics 365 Customer Engagement 계획 Enterprise Edition (정부 기관용 가격 책정) 용 추가 기능 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-137">Dynamics 365 Customer Engagement 계획 Enterprise Edition 용 추가 기능 학생용 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="28225-138">Dynamics 365 Customer Engagement 계획 Enterprise Edition 용 추가 기능 교직원 용 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="28225-139">Dynamics 365 for Sales / 계획 (정규화 된 제공) 하는 기본 대체에서 고객 참여 계획</span><span class="sxs-lookup"><span data-stu-id="28225-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="28225-140">**중단된 제안**</span><span class="sxs-lookup"><span data-stu-id="28225-140">**Retired offers**</span></span>   

- <span data-ttu-id="28225-141">Dynamics 365 판매 CRM Basic 또는 CRMOL Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="28225-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="28225-142">CRM Basic 또는 CRMOL Basic (정규화 된 제품)에서 Dynamics 365 Customer Engagement 요금제</span><span class="sxs-lookup"><span data-stu-id="28225-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="28225-143">**대체 옵션**</span><span class="sxs-lookup"><span data-stu-id="28225-143">**Replacement options**</span></span>
- <span data-ttu-id="28225-144">Dynamics 365 판매 professional (신규)</span><span class="sxs-lookup"><span data-stu-id="28225-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="28225-145">Dynamics 365 판매 professional (신규)</span><span class="sxs-lookup"><span data-stu-id="28225-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="28225-146">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="28225-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="28225-147">Dynamics 365 Customer Engagement 요금제 또는</span><span class="sxs-lookup"><span data-stu-id="28225-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="28225-148">Dynamics 365 팀 멤버</span><span class="sxs-lookup"><span data-stu-id="28225-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="28225-149">새 제품 계획으로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="28225-149">Transition customers to new product plans</span></span>

<span data-ttu-id="28225-150">사용 중지 된 Sku에서 새 버전을 고객에 게 이동이 순서로 다음 단계를 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="28225-151">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="28225-151">Purchase the new subscription</span></span>
- <span data-ttu-id="28225-152">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="28225-152">Reassign current user licenses</span></span>
- <span data-ttu-id="28225-153">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="28225-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="28225-154">고객을 위해 새 계획을 구입</span><span class="sxs-lookup"><span data-stu-id="28225-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="28225-155">선택 **고객** 왼쪽된 탐색 창에서 새 구독으로 이동 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="28225-156">선택 **구독 추가**합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="28225-157">카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="28225-158">이전 구독 및 새 고객에 게 이제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="28225-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="28225-159">다음 단계 고객에 게 라이선스를 다시 할당 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="28225-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="28225-160">선택 **고객** 왼쪽된 탐색 창에서 선택 된 고객 이동 하는 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="28225-161">**사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="28225-162">사용자에 게 라이선스를 할당할 사용자를 선택 하 고 선택한 **라이선스 관리**합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="28225-163">에 **라이선스 관리** 페이지, Dynamics 365 for Sales 지우기 / Basic (정규화 된 제공)에서 Customer Engagement 요금제 확인란 라이선스,로 이동 하는 고객 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="28225-164">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-164">Select **Submit**.</span></span> <span data-ttu-id="28225-165">새 라이선스를 필요로 하는 각 사용자에 대 한이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="28225-166">새 구독에 라이선스를 통해 이동한 후에 이전 구독을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="28225-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="28225-167">선택 **고객** 왼쪽된 탐색 창에서 선택 된 고객 이동 하는 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="28225-168">구독 세부 정보 페이지에서 이전 구독을 설정 **Suspended** 선택한 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="28225-169">이전 구독 이제 일시 중단 및 새 구독이 활성화 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="28225-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="28225-170">일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="28225-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="28225-171">고객에 게 기존 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="28225-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



