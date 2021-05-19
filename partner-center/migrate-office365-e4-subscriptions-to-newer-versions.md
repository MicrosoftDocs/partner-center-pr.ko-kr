---
title: Office 365 E4 구독 마이그레이션
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 edition은 2017 년 4 월 7 일에 사용 중지 됩니다. 최신 버전의 Office 365로 고객 구독을 마이그레이션하는 방법에 대해 알아봅니다.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151562"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="c261a-104">Office 365 E4 구독을 최신 Office 365 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="c261a-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="c261a-105">**적절 한 역할**: 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트 | 판매 에이전트</span><span class="sxs-lookup"><span data-stu-id="c261a-105">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="c261a-106">Office 365 Enterprise E4 요금제는 2017 년 4 월 7 일부 터 사용 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-106">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="c261a-107">이 날짜 이후에는 새 Office 365 E4 구독을 더 이상 구매할 수 없으며 기존 E4 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-107">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="c261a-108">E4 구독이 종료 되 면 취소 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-108">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="c261a-109">고객의 연속성을 보장 하려면 다음에 나열 된 지원 되는 SKU 옵션을 만료 하는 E4 구독이 있는 고객을 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-109">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="c261a-110">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="c261a-111">Office 365 Enterprise E4 상용 및 정부 Sku는 모두 사용이 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-111">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="c261a-112">구독의 세부 정보 페이지에서 E4 구독 상태가 "[date]에 대 한 자동 갱신 [date]"에서 "Expires on [date]"로 변경 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-112">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="c261a-113">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-113">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="c261a-114">E4 구독은 2017 년 4 월 7 일에 자동 갱신 = False로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-114">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="c261a-115">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-115">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="c261a-116">Office 365 Enterprise E4 버전 교체 계획</span><span class="sxs-lookup"><span data-stu-id="c261a-116">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="c261a-117">E4와 동일한 기능을 유지 하거나 고객이 Office 365 및 비즈니스용 Skype Online에서 최신 기능과 기능을 활용할 수 있도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-117">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="c261a-118">가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-118">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="c261a-119">Office 365 Enterprise E3 또는 Office 365 Enterprise E5의 다음 옵션에서는 보안 제품 Enterprise E3 또는 안전한 생산적인 Enterprise E5를 각각 대체할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-119">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="c261a-120">옵션 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="c261a-120">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="c261a-121">옵션 2: Office 365 Enterprise E3 + 비즈니스용 Skype 클라우드 PBX</span><span class="sxs-lookup"><span data-stu-id="c261a-121">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="c261a-122">옵션 3: Office 365 Enterprise E3 + 비즈니스용 Skype Plus CAL(E4의 가격 및 기능 패리티)</span><span class="sxs-lookup"><span data-stu-id="c261a-122">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="c261a-123">옵션 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="c261a-123">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="c261a-124">기능</span><span class="sxs-lookup"><span data-stu-id="c261a-124">Feature</span></span> | <span data-ttu-id="c261a-125">옵션 1</span><span class="sxs-lookup"><span data-stu-id="c261a-125">Option 1</span></span> | <span data-ttu-id="c261a-126">옵션 2</span><span class="sxs-lookup"><span data-stu-id="c261a-126">Option 2</span></span> | <span data-ttu-id="c261a-127">옵션 3</span><span class="sxs-lookup"><span data-stu-id="c261a-127">Option 3</span></span> | <span data-ttu-id="c261a-128">옵션 4</span><span class="sxs-lookup"><span data-stu-id="c261a-128">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="c261a-129">Office 365 Enterprise E4에 포함된 모든 기능을 사용하세요?</span><span class="sxs-lookup"><span data-stu-id="c261a-129">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="c261a-130">예</span><span class="sxs-lookup"><span data-stu-id="c261a-130">Yes</span></span> | <span data-ttu-id="c261a-131">예</span><span class="sxs-lookup"><span data-stu-id="c261a-131">Yes</span></span> | <span data-ttu-id="c261a-132">예</span><span class="sxs-lookup"><span data-stu-id="c261a-132">Yes</span></span> | <span data-ttu-id="c261a-133">예</span><span class="sxs-lookup"><span data-stu-id="c261a-133">No</span></span> |
| <span data-ttu-id="c261a-134">Office 365에서 관리되는 전화 번호</span><span class="sxs-lookup"><span data-stu-id="c261a-134">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="c261a-135">예</span><span class="sxs-lookup"><span data-stu-id="c261a-135">Yes</span></span> | <span data-ttu-id="c261a-136">예</span><span class="sxs-lookup"><span data-stu-id="c261a-136">Yes</span></span> | <span data-ttu-id="c261a-137">예</span><span class="sxs-lookup"><span data-stu-id="c261a-137">No</span></span> | <span data-ttu-id="c261a-138">예</span><span class="sxs-lookup"><span data-stu-id="c261a-138">No</span></span> |
| <span data-ttu-id="c261a-139">온-프레미스와 Office 365(하이브리드 배포)에서 모두 관리되는 전화 번호는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="c261a-139">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="c261a-140">예</span><span class="sxs-lookup"><span data-stu-id="c261a-140">Yes</span></span> | <span data-ttu-id="c261a-141">예</span><span class="sxs-lookup"><span data-stu-id="c261a-141">Yes</span></span> | <span data-ttu-id="c261a-142">예</span><span class="sxs-lookup"><span data-stu-id="c261a-142">No</span></span> | <span data-ttu-id="c261a-143">예</span><span class="sxs-lookup"><span data-stu-id="c261a-143">No</span></span> |
| <span data-ttu-id="c261a-144">PSTN 음성 통화 계획을 추가하는 옵션</span><span class="sxs-lookup"><span data-stu-id="c261a-144">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="c261a-145">예</span><span class="sxs-lookup"><span data-stu-id="c261a-145">Yes</span></span> | <span data-ttu-id="c261a-146">예</span><span class="sxs-lookup"><span data-stu-id="c261a-146">Yes</span></span> | <span data-ttu-id="c261a-147">예</span><span class="sxs-lookup"><span data-stu-id="c261a-147">No</span></span> | <span data-ttu-id="c261a-148">예</span><span class="sxs-lookup"><span data-stu-id="c261a-148">No</span></span> |
| <span data-ttu-id="c261a-149">PSTN 회의?</span><span class="sxs-lookup"><span data-stu-id="c261a-149">PSTN Conferencing?</span></span> | <span data-ttu-id="c261a-150">예</span><span class="sxs-lookup"><span data-stu-id="c261a-150">Yes</span></span> | <span data-ttu-id="c261a-151">예</span><span class="sxs-lookup"><span data-stu-id="c261a-151">No</span></span> | <span data-ttu-id="c261a-152">예</span><span class="sxs-lookup"><span data-stu-id="c261a-152">No</span></span> | <span data-ttu-id="c261a-153">예</span><span class="sxs-lookup"><span data-stu-id="c261a-153">No</span></span> |
| <span data-ttu-id="c261a-154">협업, 분석 및 보안을 위한 고급 도구는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="c261a-154">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="c261a-155">예</span><span class="sxs-lookup"><span data-stu-id="c261a-155">Yes</span></span> | <span data-ttu-id="c261a-156">예</span><span class="sxs-lookup"><span data-stu-id="c261a-156">No</span></span> | <span data-ttu-id="c261a-157">예</span><span class="sxs-lookup"><span data-stu-id="c261a-157">No</span></span> | <span data-ttu-id="c261a-158">예</span><span class="sxs-lookup"><span data-stu-id="c261a-158">No</span></span> |
| <span data-ttu-id="c261a-159">대화형 보고서, 대시보드 및 데이터 시각화</span><span class="sxs-lookup"><span data-stu-id="c261a-159">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="c261a-160">예</span><span class="sxs-lookup"><span data-stu-id="c261a-160">Yes</span></span> | <span data-ttu-id="c261a-161">예</span><span class="sxs-lookup"><span data-stu-id="c261a-161">No</span></span> | <span data-ttu-id="c261a-162">예</span><span class="sxs-lookup"><span data-stu-id="c261a-162">No</span></span> | <span data-ttu-id="c261a-163">예</span><span class="sxs-lookup"><span data-stu-id="c261a-163">No</span></span> | 
| <span data-ttu-id="c261a-164">기본 제공 개인 정보 보호, 투명성 및 구체화된 사용자 정의 컨트롤을 통해 데이터 보안 및 규정 준수를 더 자세히 제어할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="c261a-164">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="c261a-165">예</span><span class="sxs-lookup"><span data-stu-id="c261a-165">Yes</span></span> | <span data-ttu-id="c261a-166">예</span><span class="sxs-lookup"><span data-stu-id="c261a-166">No</span></span> | <span data-ttu-id="c261a-167">예</span><span class="sxs-lookup"><span data-stu-id="c261a-167">No</span></span> | <span data-ttu-id="c261a-168">예</span><span class="sxs-lookup"><span data-stu-id="c261a-168">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c261a-169">고객을 새 제품 플랜으로 전환</span><span class="sxs-lookup"><span data-stu-id="c261a-169">Transition customers to new product plans</span></span>

<span data-ttu-id="c261a-170">Microsoft는 파트너에게 지속적으로 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-170">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="c261a-171">이러한 경우 고객을 새 서비스로 업그레이드하거나 최종적으로 종료될 S SKU에서 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-171">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="c261a-172">사용 중지된 S SKU에서 최신 S SKU로 고객을 마이그레이션하려면 다음 단계가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-172">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="c261a-173">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="c261a-173">Purchase the new subscription</span></span>
-   <span data-ttu-id="c261a-174">현재 사용자 라이선스 재할당</span><span class="sxs-lookup"><span data-stu-id="c261a-174">Reassign current user licenses</span></span>
-   <span data-ttu-id="c261a-175">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="c261a-175">Cancel the old subscription</span></span>

<span data-ttu-id="c261a-176">다음 단계에 따라 고객의 Office 365 Enterprise E4 구독을 위 표의 옵션 중 하나로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-176">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="c261a-177">1단계 - 새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="c261a-177">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="c261a-178">**파트너 센터** 메뉴에서 **고객을** 선택하고 이동하려는 고객을 선택한 다음 구독 **추가를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="c261a-179">카탈로그에서 구매할 구독(이 경우 위의 옵션 중 하나)을 선택하고 라이선스 수를 입력한 다음, **제출을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-179">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="c261a-180">이제 고객에게 이전 및 새 구독, 이전 Office 365 Enterprise E4 구독 및 새 '대상' 구독(예: 옵션 1 - Office 365 Enterprise E5)이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-180">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="c261a-181">2단계 - 고객의 사용자 라이선스 재할당</span><span class="sxs-lookup"><span data-stu-id="c261a-181">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="c261a-182">**파트너 센터** 메뉴에서 **고객을** 선택하고 이동하려는 고객을 선택한 다음, 사용자 및 **라이선스를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="c261a-183">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-183">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="c261a-184">사용자 라이선스를 다시 할당하려면 재할당할 사용자를 선택한 **다음, 라이선스 관리를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="c261a-184">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="c261a-185">라이선스 **관리** 페이지에서 **Office 365 Enterprise E4** 라이선스 확인란의 선택을 취소하고 고객이 이동하는 구독에 대한 새 서비스 계획을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-185">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="c261a-186">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-186">Select **Submit**.</span></span> <span data-ttu-id="c261a-187">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-187">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="c261a-188">라이선스 재할당이 필요한 다른 고객 사용자와 동일한 단계를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-188">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="c261a-189">사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-189">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="c261a-190">3단계 - 이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="c261a-190">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="c261a-191">**파트너 센터** 메뉴에서 **고객을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-191">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="c261a-192">이동하려는 고객을 선택하고 취소할 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-192">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="c261a-193">구독 세부 정보 페이지에서 구독 상태를 **일시 중단 으로** 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-193">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="c261a-194">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-194">Select **Submit**.</span></span>

<span data-ttu-id="c261a-195">이전 구독이 일시 중단되고 새 구독이 활성 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-195">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="c261a-196">일시 중단된 구독은 120일 후에 자동으로 프로비저닝이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-196">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c261a-197">고객은 이전 구독에 대한 추가 비용이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c261a-197">The customer incurs no additional costs for the old subscription.</span></span>



 



