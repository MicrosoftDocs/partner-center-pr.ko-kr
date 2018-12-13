---
title: Dynamics 365 고객 참여 계획 하 고 기본 (자격 갖춘된 제공)을 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / 고객 참여 계획 (자격을 갖춘 제공)는 기본 구독에서 더 이상 갱신할 수 없습니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968273"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="b8bc6-103">Dynamics 365 고객 참여 계획 하 고 기본 (자격 갖춘된 제공)을 최신 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="b8bc6-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="b8bc6-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="b8bc6-104">Applies to</span></span>**

-  <span data-ttu-id="b8bc6-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b8bc6-105">Partner Center</span></span>

<span data-ttu-id="b8bc6-106">Dynamics 365 for Sales 사용 하 여 유효 2019 년 1 월 1 일, 고객 / 고객 참여 계획 (자격을 갖춘 제공)는 기본 구독에서 이러한 레거시 제품; 더 이상 갱신할 수 기존 구독 만료 시 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="b8bc6-107">구독의 세부 정보 페이지에서 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="b8bc6-108">고객에 대 한 연속성을 보장 하려면 아래에 나열 된 지원 되는 옵션으로 구독이 곧 만료 되 있는 사용자를 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="b8bc6-109">고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b8bc6-110">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 함께 구독의 종료 날짜를 확인 하 여 곧 만료 되 구독 찾을 수 = False 속성과 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b8bc6-111">해당 구독을 자동으로 설정 됩니다 갱신 2019 년 1 월 1 일에 = False입니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="b8bc6-112">언제든지 고객을 새 요금제로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="b8bc6-113">Dynamics 365 사용 중지 되 고 제공</span><span class="sxs-lookup"><span data-stu-id="b8bc6-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="b8bc6-114">Dynamics 365 판매 Enterprise Edition CRMOL basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-115">Dynamics 365 교직원에 대 한 판매 Enterprise Edition CRMOL basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8bc6-116">Dynamics 365 학생에 대 한 판매 Enterprise Edition CRMOL basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8bc6-117">Dynamics 365 판매 Enterprise Edition (정부 가격) CRMOL basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-118">CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-119">교직원 용 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8bc6-120">학생 들을 위한 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8bc6-121">CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise Edition (정부 가격)에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-122">CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-123">교직원 용 CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8bc6-124">학생 들을 위한 CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8bc6-125">CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition (정부 가격) 추가 기능에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b8bc6-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-126">Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-127">Dynamics 365 고객 참여 계획 Enterprise Edition (정부 가격) CRMOL Basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-128">Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic (자격 갖춘된 제품) 학생</span><span class="sxs-lookup"><span data-stu-id="b8bc6-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8bc6-129">Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic (자격 갖춘된 제품) 교직원</span><span class="sxs-lookup"><span data-stu-id="b8bc6-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8bc6-130">CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="b8bc6-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-131">Dynamics 365 고객 참여 계획 Enterprise Edition (정부 가격)에서 SA CRM basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-132">학생 들을 위한 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="b8bc6-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8bc6-133">교직원 용 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="b8bc6-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8bc6-134">Dynamics 365 고객 참여 계획 Enterprise Edition의 추가 기능 CRM Basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-135">Dynamics 365 고객 참여 계획 Enterprise Edition (정부 가격) 추가 기능 CRM basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-136">Dynamics 365 고객 참여 계획 Enterprise Edition의 추가 기능 학생에 대 한 CRM Basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8bc6-137">Dynamics 365 고객 참여 계획 Enterprise Edition의 추가 기능 교직원 용 CRM Basic (자격 갖춘된 제품)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="b8bc6-138">Dynamics 365 for Sales / 계획 (자격을 갖춘 제공) 기본 대체에서 고객 참여 계획</span><span class="sxs-lookup"><span data-stu-id="b8bc6-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="b8bc6-139">사용 중지 된 제품</span><span class="sxs-lookup"><span data-stu-id="b8bc6-139">Retired offers</span></span>**   

- <span data-ttu-id="b8bc6-140">Dynamics 365 for Sales CRM Basic 또는 CRMOL (자격 갖춘된 제품)에서</span><span class="sxs-lookup"><span data-stu-id="b8bc6-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8bc6-141">CRM Basic 또는 CRMOL (자격 갖춘된 제품)에서 Dynamics 365 고객 참여 계획</span><span class="sxs-lookup"><span data-stu-id="b8bc6-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="b8bc6-142">대체 옵션</span><span class="sxs-lookup"><span data-stu-id="b8bc6-142">Replacement options</span></span>**
- <span data-ttu-id="b8bc6-143">Dynamics 365 판매 professional (신규)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="b8bc6-144">Dynamics 365 판매 professional (신규)</span><span class="sxs-lookup"><span data-stu-id="b8bc6-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="b8bc6-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="b8bc6-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="b8bc6-146">Dynamics 365 고객 참여 계획 또는</span><span class="sxs-lookup"><span data-stu-id="b8bc6-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="b8bc6-147">Dynamics 365 팀 구성원</span><span class="sxs-lookup"><span data-stu-id="b8bc6-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b8bc6-148">새 제품 요금제로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="b8bc6-148">Transition customers to new product plans</span></span>

<span data-ttu-id="b8bc6-149">고객에 게 사용 중지 된 Sku에서 최신 패키지로 이동 순서로 다음 단계를 따라야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="b8bc6-150">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="b8bc6-150">Purchase the new subscription</span></span>
- <span data-ttu-id="b8bc6-151">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="b8bc6-151">Reassign current user licenses</span></span>
- <span data-ttu-id="b8bc6-152">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="b8bc6-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="b8bc6-153">구매 고객에 대 한 새 계획</span><span class="sxs-lookup"><span data-stu-id="b8bc6-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="b8bc6-154">왼쪽된 탐색에서 **고객** 을 선택 하 고 새 구독으로 이동 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="b8bc6-155">**구독 추가**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="b8bc6-156">카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b8bc6-157">이전 구독와 새 고객에 게 이제 생깁니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="b8bc6-158">다음 단계는 고객의 사용자에 게 라이선스 할당 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="b8bc6-159">왼쪽된 탐색에서 **고객** 을 선택 하 고 이동 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b8bc6-160">**사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="b8bc6-161">사용자에 게 라이선스를 할당 하는 사용자를 선택 하 고 **라이선스 관리를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="b8bc6-162">**라이선스 관리** 페이지에서 Dynamics 365 for Sales의 선택을 취소/고객 참여 계획 (자격을 갖춘 제공) 기본에서 라이선스 확인란을 선택 하 고 고객을 이동할 구독의 새로운 서비스 요금제를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="b8bc6-163">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-163">Select **Submit**.</span></span> <span data-ttu-id="b8bc6-164">새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="b8bc6-165">새 구독에 라이선스를 이동한 후에 이전 구독을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="b8bc6-166">왼쪽된 탐색에서 **고객** 을 선택 하 고 이동 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b8bc6-167">구독 세부 정보 페이지에서 이전 구독 **일시 중단 됨** 을 설정 하 고 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="b8bc6-168">이전 구독이 이제 일시 중단 하 고 새 구독이 활성화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="b8bc6-169">일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b8bc6-170">고객에 게 이전 구독에 대 한 추가 비용 없이 발생 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b8bc6-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



