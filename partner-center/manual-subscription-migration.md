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
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132743"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="d4ad3-103">Dynamics 365 및 Customer Engagement 플랜을 기본(제한된 제품)에서 새 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="d4ad3-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="d4ad3-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="d4ad3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d4ad3-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="d4ad3-105">Global admin</span></span>
- <span data-ttu-id="d4ad3-106">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="d4ad3-106">User management admin</span></span>
- <span data-ttu-id="d4ad3-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="d4ad3-107">Admin agent</span></span>
- <span data-ttu-id="d4ad3-108">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="d4ad3-108">Sales agent</span></span>

<span data-ttu-id="d4ad3-109">2019 년 1 월 1 일부 터 기본 (우량 제안) 구독의 판매/고객 참여 요금제에 대 한 Dynamics 365이 있는 고객은 이러한 레거시 제안을 더 이상 갱신할 수 없습니다. 기존 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="d4ad3-110">구독의 세부 정보 페이지에서 구독 상태는 "[date]에 대 한 자동 갱신 [날짜]"에서 "만료 날짜 [날짜]"로 변경 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="d4ad3-111">고객의 연속성을 보장 하려면 구독 만료를 포함 하는 항목을 아래 나열 된 지원 되는 옵션으로 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="d4ad3-112">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="d4ad3-113">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="d4ad3-114">문제의 구독은 2019 년 1 월 1 일에 자동 갱신 = False로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="d4ad3-115">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="d4ad3-116">Dynamics 365 제공이 사용 중지 됨</span><span class="sxs-lookup"><span data-stu-id="d4ad3-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="d4ad3-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-118">교직원 용 Dynamics 365 for Sales Enterprise Edition CRMOL 기본 (우량 제안)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4ad3-119">학생을 위한 Dynamics 365 for Sales Enterprise Edition CRMOL Basic (우량 제안)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4ad3-120">Dynamics 365 for Sales Enterprise Edition (정부 가격) CRMOL 기본 (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-121">CRM Basic (정규화 된 제품)의 경우 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d4ad3-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-122">교직원 용 Dynamics 365 for CRM Basic (우량 제안) for 교직원</span><span class="sxs-lookup"><span data-stu-id="d4ad3-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4ad3-123">학생의 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise 버전용 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d4ad3-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4ad3-124">CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 for Sales Enterprise Edition (정부 가격)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-125">CRM Basic (정규화 된 제품)에 대 한 Dynamics 365 for Sales Enterprise Edition Add-On</span><span class="sxs-lookup"><span data-stu-id="d4ad3-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-126">교직원 용 Dynamics 365 for Sales Enterprise Edition Add-On (교직원 용 정식 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4ad3-127">학생용 CRM Basic (정규화 된 제품)에 대 한 Dynamics 365 for Sales Enterprise Edition Add-On</span><span class="sxs-lookup"><span data-stu-id="d4ad3-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4ad3-128">CRM Basic (정규화 된 제품)에 대 한 Dynamics 365 for Sales Enterprise Edition (정부 가격) Add-On</span><span class="sxs-lookup"><span data-stu-id="d4ad3-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (정부 가격) CRMOL 기본 (적격 제안)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-131">학생용 Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (우량 제안)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4ad3-132">교직원 용 Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (적격 제안)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4ad3-133">Dynamics 365 Customer Engagement Plan for SA에서 CRM Basic (정규화 된 제품)에 대 한 엔터프라이즈 버전</span><span class="sxs-lookup"><span data-stu-id="d4ad3-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-134">CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 요금제 Enterprise Edition (정부 가격)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-135">Dynamics 365 Customer Engagement Plan for SA에서 학생용 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4ad3-136">Dynamics 365 고객 Engagement 요금제의 SA에서 교직원 용 CRM Basic (정규화 된 제품)에 대 한 엔터프라이즈 버전</span><span class="sxs-lookup"><span data-stu-id="d4ad3-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d4ad3-137">Dynamics 365 고객 Engagement 계획 Enterprise Edition Add-On CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-138">Dynamics 365 CRM Basic (정규화 된 제품)에 대 한 Dynamics 고객 Engagement 계획 Enterprise Edition (정부 가격) Add-On</span><span class="sxs-lookup"><span data-stu-id="d4ad3-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-139">Dynamics 365 Customer Engagement Plan for 학생에 대 한 CRM Basic (우량 제안)의 경우 Enterprise Edition Add-On</span><span class="sxs-lookup"><span data-stu-id="d4ad3-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d4ad3-140">Dynamics 365 고객 Engagement 계획 Enterprise Edition Add-On 교직원 용 CRM Basic (정규화 된 제품)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="d4ad3-141">기본 (우량 제안) 대체 요금제에서 판매/고객 참여 요금제에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d4ad3-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="d4ad3-142">**사용 중지 된 제안**</span><span class="sxs-lookup"><span data-stu-id="d4ad3-142">**Retired offers**</span></span>   

- <span data-ttu-id="d4ad3-143">CRM Basic 또는 CRMOL Basic (정규화 된 제안)에서 판매에 대 한 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d4ad3-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d4ad3-144">CRM Basic 또는 CRMOL Basic (정규화 된 제품)의 Dynamics 365 Customer Engagement 계획</span><span class="sxs-lookup"><span data-stu-id="d4ad3-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="d4ad3-145">**대체 옵션**</span><span class="sxs-lookup"><span data-stu-id="d4ad3-145">**Replacement options**</span></span>
- <span data-ttu-id="d4ad3-146">Dynamics 365 for Sales Professional (신규)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d4ad3-147">Dynamics 365 for Sales Professional (신규)</span><span class="sxs-lookup"><span data-stu-id="d4ad3-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d4ad3-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="d4ad3-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="d4ad3-149">Dynamics 365 Customer Engagement 요금제 또는</span><span class="sxs-lookup"><span data-stu-id="d4ad3-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="d4ad3-150">Dynamics 365 팀 멤버</span><span class="sxs-lookup"><span data-stu-id="d4ad3-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d4ad3-151">고객을 새 제품 요금제로 전환</span><span class="sxs-lookup"><span data-stu-id="d4ad3-151">Transition customers to new product plans</span></span>

<span data-ttu-id="d4ad3-152">사용 중지 된 Sku에서 최신 버전으로 고객을 이동 하려면 다음 단계를 순서 대로 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="d4ad3-153">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="d4ad3-153">Purchase the new subscription</span></span>
- <span data-ttu-id="d4ad3-154">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="d4ad3-154">Reassign current user licenses</span></span>
- <span data-ttu-id="d4ad3-155">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="d4ad3-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="d4ad3-156">고객에 대 한 새 요금제 구매</span><span class="sxs-lookup"><span data-stu-id="d4ad3-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="d4ad3-157">왼쪽 탐색 창에서 **고객** 을 선택한 다음 새 구독으로 이동할 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="d4ad3-158">**구독 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="d4ad3-159">카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="d4ad3-160">이제 고객에 게 이전 구독과 새 구독이 모두 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="d4ad3-161">다음 단계는 고객의 사용자에 게 라이선스를 다시 할당 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="d4ad3-162">왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d4ad3-163">**사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="d4ad3-164">사용자에 게 라이선스를 재할당 하려면 사용자를 선택한 다음 **라이선스 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="d4ad3-165">**라이선스 관리** 페이지에서 기본 (우량 제안) 라이선스에서 판매/고객 지원 계획에 대 한 Dynamics 365을 지우고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="d4ad3-166">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-166">Select **Submit**.</span></span> <span data-ttu-id="d4ad3-167">새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="d4ad3-168">새 구독으로 라이선스를 이동한 후에는 이전 구독을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="d4ad3-169">왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d4ad3-170">구독 정보 페이지에서 이전 구독을 **일시 중단 됨** 으로 설정 하 고 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="d4ad3-171">이제 이전 구독이 일시 중단 되 고 새 구독이 활성화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="d4ad3-172">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d4ad3-173">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4ad3-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



