---
title: Office 365 E4 구독을 Office 365 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 버전은 2017년 4월 7일부로 사용 중지되었습니다. 고객 구독을 Office 365 최신 버전으로 마이그레이션하는 방법을 알아보세요.
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: ead92169ce7b3f1c2e697b6d4e983603c17d39fc
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390882"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="b423d-104">Office 365 E4 구독을 Office 365 최신 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="b423d-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="b423d-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="b423d-105">**Applies to**</span></span>

-  <span data-ttu-id="b423d-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b423d-106">Partner Center</span></span>

<span data-ttu-id="b423d-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="b423d-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="b423d-108">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="b423d-108">Global admin</span></span>
-   <span data-ttu-id="b423d-109">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="b423d-109">User admin</span></span>
-   <span data-ttu-id="b423d-110">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="b423d-110">Admin agent</span></span>
-   <span data-ttu-id="b423d-111">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="b423d-111">Sales agent</span></span>

<span data-ttu-id="b423d-112">Office 365 Enterprise E4 요금제가 2017년 4월 7일부로 사용 중지되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="b423d-113">이 날짜 이후로는 더 이상 새 Office 365 E4 구독을 구입할 수 없으며, 기존 E4 구독은 만료 시 자동으로 갱신되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="b423d-114">E4 구독이 만료되면 구독이 취소됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="b423d-115">고객에게 연속성을 보장하기 위해, E4 구독이 곧 만료되는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="b423d-116">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="b423d-117">Office 365 Enterprise E4 상용 및 정부 Sku는 모두 사용이 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="b423d-118">구독의 세부 정보 페이지에서 E4 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="b423d-119">API(CREST 또는 파트너 센터)를 사용하는 경우 auto renew = False 속성과 함께 구독의 종료 날짜를 확인하여 곧 만료되는 구독을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="b423d-120">E4 구독은 2017년 4월 7일에 auto renew=False로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="b423d-121">언제든지 고객을 새 요금제로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="b423d-122">Office 365 Enterprise E4 버전 교체 요금제</span><span class="sxs-lookup"><span data-stu-id="b423d-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="b423d-123">E4와 같은 기능을 그대로 유지할 수도 있고 고객이 Office 365 및 비즈니스용 Skype Online의 새로운 기능을 활용하게 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="b423d-124">가격 정보는 가격 목록에서 찾을 수 있으며 파트너 센터에 목록표가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="b423d-125">Secure Product Enterprise E3 또는 Secure Productive Enterprise E5는 각각 Office 365 Enterprise E3 또는 Office 365 Enterprise E5에 대한 다음 옵션에서 대체될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="b423d-126">옵션 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="b423d-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="b423d-127">옵션 2: Office 365 Enterprise E3 + 비즈니스용 Skype 클라우드 PBX</span><span class="sxs-lookup"><span data-stu-id="b423d-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="b423d-128">옵션 3: Office 365 Enterprise E3 + 비즈니스용 Skype Plus CAL(E4와 가격 및 기능이 동일)</span><span class="sxs-lookup"><span data-stu-id="b423d-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="b423d-129">옵션 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="b423d-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="b423d-130">기능</span><span class="sxs-lookup"><span data-stu-id="b423d-130">Feature</span></span> | <span data-ttu-id="b423d-131">옵션 1</span><span class="sxs-lookup"><span data-stu-id="b423d-131">Option 1</span></span> | <span data-ttu-id="b423d-132">옵션 2</span><span class="sxs-lookup"><span data-stu-id="b423d-132">Option 2</span></span> | <span data-ttu-id="b423d-133">옵션 3</span><span class="sxs-lookup"><span data-stu-id="b423d-133">Option 3</span></span> | <span data-ttu-id="b423d-134">옵션 4</span><span class="sxs-lookup"><span data-stu-id="b423d-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="b423d-135">Office 365 Enterprise E4의 모든 기능을 제공하나요?</span><span class="sxs-lookup"><span data-stu-id="b423d-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="b423d-136">예</span><span class="sxs-lookup"><span data-stu-id="b423d-136">Yes</span></span> | <span data-ttu-id="b423d-137">예</span><span class="sxs-lookup"><span data-stu-id="b423d-137">Yes</span></span> | <span data-ttu-id="b423d-138">예</span><span class="sxs-lookup"><span data-stu-id="b423d-138">Yes</span></span> | <span data-ttu-id="b423d-139">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-139">No</span></span> |
| <span data-ttu-id="b423d-140">전화 번호를 Office 365에서 관리하나요?</span><span class="sxs-lookup"><span data-stu-id="b423d-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="b423d-141">예</span><span class="sxs-lookup"><span data-stu-id="b423d-141">Yes</span></span> | <span data-ttu-id="b423d-142">예</span><span class="sxs-lookup"><span data-stu-id="b423d-142">Yes</span></span> | <span data-ttu-id="b423d-143">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-143">No</span></span> | <span data-ttu-id="b423d-144">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-144">No</span></span> |
| <span data-ttu-id="b423d-145">전화 번호를 온-프레미스와 Office 365 모두에서 관리하나요(하이브리드 배포)?</span><span class="sxs-lookup"><span data-stu-id="b423d-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="b423d-146">예</span><span class="sxs-lookup"><span data-stu-id="b423d-146">Yes</span></span> | <span data-ttu-id="b423d-147">예</span><span class="sxs-lookup"><span data-stu-id="b423d-147">Yes</span></span> | <span data-ttu-id="b423d-148">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-148">No</span></span> | <span data-ttu-id="b423d-149">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-149">No</span></span> |
| <span data-ttu-id="b423d-150">PSTN 음성 통화 요금제를 추가할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="b423d-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="b423d-151">예</span><span class="sxs-lookup"><span data-stu-id="b423d-151">Yes</span></span> | <span data-ttu-id="b423d-152">예</span><span class="sxs-lookup"><span data-stu-id="b423d-152">Yes</span></span> | <span data-ttu-id="b423d-153">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-153">No</span></span> | <span data-ttu-id="b423d-154">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-154">No</span></span> |
| <span data-ttu-id="b423d-155">PSTN 회의가 가능한가요?</span><span class="sxs-lookup"><span data-stu-id="b423d-155">PSTN Conferencing?</span></span> | <span data-ttu-id="b423d-156">예</span><span class="sxs-lookup"><span data-stu-id="b423d-156">Yes</span></span> | <span data-ttu-id="b423d-157">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-157">No</span></span> | <span data-ttu-id="b423d-158">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-158">No</span></span> | <span data-ttu-id="b423d-159">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-159">No</span></span> |
| <span data-ttu-id="b423d-160">공동 작업, 분석 및 보안을 위한 고급 도구가 제공되나요?</span><span class="sxs-lookup"><span data-stu-id="b423d-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="b423d-161">예</span><span class="sxs-lookup"><span data-stu-id="b423d-161">Yes</span></span> | <span data-ttu-id="b423d-162">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-162">No</span></span> | <span data-ttu-id="b423d-163">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-163">No</span></span> | <span data-ttu-id="b423d-164">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-164">No</span></span> |
| <span data-ttu-id="b423d-165">대화형 보고서, 대시보드 및 데이터 시각화가 제공되나요?</span><span class="sxs-lookup"><span data-stu-id="b423d-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="b423d-166">예</span><span class="sxs-lookup"><span data-stu-id="b423d-166">Yes</span></span> | <span data-ttu-id="b423d-167">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-167">No</span></span> | <span data-ttu-id="b423d-168">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-168">No</span></span> | <span data-ttu-id="b423d-169">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-169">No</span></span> | 
| <span data-ttu-id="b423d-170">기본 프라이버시, 투명성 및 정교한 사용자 컨트롤로 데이터 보안과 규정 준수를 보다 철저하게 제어할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="b423d-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="b423d-171">예</span><span class="sxs-lookup"><span data-stu-id="b423d-171">Yes</span></span> | <span data-ttu-id="b423d-172">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-172">No</span></span> | <span data-ttu-id="b423d-173">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-173">No</span></span> | <span data-ttu-id="b423d-174">아니요</span><span class="sxs-lookup"><span data-stu-id="b423d-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b423d-175">새 제품 계획으로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="b423d-175">Transition customers to new product plans</span></span>

<span data-ttu-id="b423d-176">Microsoft는 지속적으로 파트너에게 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="b423d-177">다음과 같은 경우 파트너는 고객을 새 서비스로 업그레이드하거나 결국 종료될 SKU의 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="b423d-178">사용 중지된 SKU에서 새 SKU로 고객을 마이그레이션하려면 다음 단계를 따라야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="b423d-179">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="b423d-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="b423d-180">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="b423d-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="b423d-181">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="b423d-181">Cancel the old subscription</span></span>

<span data-ttu-id="b423d-182">다음 단계에 따라 고객의 Office 365 Enterprise E4 구독을 아래 표의 옵션 중 하나로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="b423d-183">1단계 - 새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="b423d-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="b423d-184">**파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동할 고객을 선택한 다음 **구독 추가**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="b423d-185">카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="b423d-186">이제 고객에 게 이전 구독과 새 구독, 이전 Office 365 Enterprise E4 구독 및 새 ' 대상 ' 구독 (예: 1-Office 365 Enterprise E5)이 모두 포함 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="b423d-187">2단계 - 고객의 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="b423d-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="b423d-188">**파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동할 고객을 선택한 후 **사용자 및 라이선스**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="b423d-189">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="b423d-190">사용자 라이선스를 다시 할당하려면 다시 할당할 사용자를 선택한 다음 **라이선스 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="b423d-191">**라이선스 관리** 페이지에서 **Office 365 Enterprise E4** 라이선스 확인란의 선택을 취소한 다음 고객을 이동할 구독의 새로운 서비스 요금제를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="b423d-192">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-192">Select **Submit**.</span></span> <span data-ttu-id="b423d-193">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="b423d-194">라이선스 다시 할당이 필요한 다른 모든 고객 사용자에 대해 같은 단계를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="b423d-195">사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="b423d-196">3단계 - 이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="b423d-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="b423d-197">**파트너 센터** 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="b423d-198">이동하려는 고객을 선택하고, 취소할 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="b423d-199">구독 세부 정보 페이지에서 구독 상태를 **일시 중단됨**으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="b423d-200">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-200">Select **Submit**.</span></span>

<span data-ttu-id="b423d-201">이전 구독이 일시 중단되고 새 구독이 활성화됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="b423d-202">일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b423d-203">이전 구독에 대해서는 고객에게 추가 비용이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b423d-203">The customer incurs no additional costs for the old subscription.</span></span>



 



