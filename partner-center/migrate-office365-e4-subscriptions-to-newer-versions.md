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
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949043"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="d7c5b-104">Office 365 E4 구독을 최신 Office 365 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="d7c5b-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="d7c5b-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="d7c5b-105">**Applies to**</span></span>

-  <span data-ttu-id="d7c5b-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="d7c5b-106">Partner Center</span></span>

<span data-ttu-id="d7c5b-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="d7c5b-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="d7c5b-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="d7c5b-108">Global admin</span></span>
-   <span data-ttu-id="d7c5b-109">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="d7c5b-109">User admin</span></span>
-   <span data-ttu-id="d7c5b-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="d7c5b-110">Admin agent</span></span>
-   <span data-ttu-id="d7c5b-111">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="d7c5b-111">Sales agent</span></span>

<span data-ttu-id="d7c5b-112">Office 365 Enterprise E4 요금제는 2017 년 4 월 7 일부 터 사용 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="d7c5b-113">이 날짜 이후에는 새 Office 365 E4 구독을 더 이상 구매할 수 없으며 기존 E4 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="d7c5b-114">E4 구독이 종료 되 면 취소 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="d7c5b-115">고객의 연속성을 보장 하려면 다음에 나열 된 지원 되는 SKU 옵션을 만료 하는 E4 구독이 있는 고객을 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="d7c5b-116">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="d7c5b-117">Office 365 Enterprise E4 상용 및 정부 Sku는 모두 사용이 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="d7c5b-118">구독의 세부 정보 페이지에서 E4 구독 상태가 "[date]에 대 한 자동 갱신 [date]"에서 "Expires on [date]"로 변경 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="d7c5b-119">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="d7c5b-120">E4 구독은 2017 년 4 월 7 일에 자동 갱신 = False로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="d7c5b-121">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="d7c5b-122">Office 365 Enterprise E4 버전 교체 계획</span><span class="sxs-lookup"><span data-stu-id="d7c5b-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="d7c5b-123">E4와 동일한 기능을 유지 하거나 고객이 Office 365 및 비즈니스용 Skype Online에서 최신 기능과 기능을 활용할 수 있도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="d7c5b-124">가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="d7c5b-125">Office 365 Enterprise E3 또는 Office 365 Enterprise E5의 다음 옵션에서는 보안 제품 Enterprise E3 또는 안전한 생산적인 Enterprise E5를 각각 대체할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="d7c5b-126">옵션 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="d7c5b-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="d7c5b-127">옵션 2: Office 365 Enterprise E3 + 비즈니스용 Skype 클라우드 PBX</span><span class="sxs-lookup"><span data-stu-id="d7c5b-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="d7c5b-128">옵션 3: Office 365 Enterprise E3 + 비즈니스용 Skype Plus CAL (E4를 사용 하는 가격 및 기능 패리티)</span><span class="sxs-lookup"><span data-stu-id="d7c5b-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="d7c5b-129">옵션 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="d7c5b-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="d7c5b-130">기능</span><span class="sxs-lookup"><span data-stu-id="d7c5b-130">Feature</span></span> | <span data-ttu-id="d7c5b-131">옵션 1</span><span class="sxs-lookup"><span data-stu-id="d7c5b-131">Option 1</span></span> | <span data-ttu-id="d7c5b-132">옵션 2</span><span class="sxs-lookup"><span data-stu-id="d7c5b-132">Option 2</span></span> | <span data-ttu-id="d7c5b-133">옵션 3</span><span class="sxs-lookup"><span data-stu-id="d7c5b-133">Option 3</span></span> | <span data-ttu-id="d7c5b-134">옵션 4</span><span class="sxs-lookup"><span data-stu-id="d7c5b-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="d7c5b-135">Office 365 Enterprise E4에 포함 된 모든 기능을 다운로드 하세요.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="d7c5b-136">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-136">Yes</span></span> | <span data-ttu-id="d7c5b-137">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-137">Yes</span></span> | <span data-ttu-id="d7c5b-138">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-138">Yes</span></span> | <span data-ttu-id="d7c5b-139">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-139">No</span></span> |
| <span data-ttu-id="d7c5b-140">Office 365에서 관리 되는 전화 번호</span><span class="sxs-lookup"><span data-stu-id="d7c5b-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="d7c5b-141">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-141">Yes</span></span> | <span data-ttu-id="d7c5b-142">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-142">Yes</span></span> | <span data-ttu-id="d7c5b-143">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-143">No</span></span> | <span data-ttu-id="d7c5b-144">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-144">No</span></span> |
| <span data-ttu-id="d7c5b-145">온-프레미스와 Office 365에서 모두 관리 되는 전화 번호 (하이브리드 배포)</span><span class="sxs-lookup"><span data-stu-id="d7c5b-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="d7c5b-146">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-146">Yes</span></span> | <span data-ttu-id="d7c5b-147">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-147">Yes</span></span> | <span data-ttu-id="d7c5b-148">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-148">No</span></span> | <span data-ttu-id="d7c5b-149">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-149">No</span></span> |
| <span data-ttu-id="d7c5b-150">PSTN 음성 호출 계획을 추가 하는 옵션</span><span class="sxs-lookup"><span data-stu-id="d7c5b-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="d7c5b-151">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-151">Yes</span></span> | <span data-ttu-id="d7c5b-152">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-152">Yes</span></span> | <span data-ttu-id="d7c5b-153">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-153">No</span></span> | <span data-ttu-id="d7c5b-154">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-154">No</span></span> |
| <span data-ttu-id="d7c5b-155">PSTN 회의</span><span class="sxs-lookup"><span data-stu-id="d7c5b-155">PSTN Conferencing?</span></span> | <span data-ttu-id="d7c5b-156">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-156">Yes</span></span> | <span data-ttu-id="d7c5b-157">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-157">No</span></span> | <span data-ttu-id="d7c5b-158">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-158">No</span></span> | <span data-ttu-id="d7c5b-159">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-159">No</span></span> |
| <span data-ttu-id="d7c5b-160">공동 작업, 분석 및 보안을 위한 고급 도구</span><span class="sxs-lookup"><span data-stu-id="d7c5b-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="d7c5b-161">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-161">Yes</span></span> | <span data-ttu-id="d7c5b-162">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-162">No</span></span> | <span data-ttu-id="d7c5b-163">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-163">No</span></span> | <span data-ttu-id="d7c5b-164">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-164">No</span></span> |
| <span data-ttu-id="d7c5b-165">대화형 보고서, 대시보드 및 데이터 시각화</span><span class="sxs-lookup"><span data-stu-id="d7c5b-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="d7c5b-166">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-166">Yes</span></span> | <span data-ttu-id="d7c5b-167">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-167">No</span></span> | <span data-ttu-id="d7c5b-168">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-168">No</span></span> | <span data-ttu-id="d7c5b-169">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-169">No</span></span> | 
| <span data-ttu-id="d7c5b-170">기본 제공 개인 정보, 투명성 및 구체화 된 사용자 정의 컨트롤에 대 한 데이터 보안 및 규정 준수 제어 강화</span><span class="sxs-lookup"><span data-stu-id="d7c5b-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="d7c5b-171">예</span><span class="sxs-lookup"><span data-stu-id="d7c5b-171">Yes</span></span> | <span data-ttu-id="d7c5b-172">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-172">No</span></span> | <span data-ttu-id="d7c5b-173">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-173">No</span></span> | <span data-ttu-id="d7c5b-174">아니요</span><span class="sxs-lookup"><span data-stu-id="d7c5b-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d7c5b-175">고객을 새 제품 요금제로 전환</span><span class="sxs-lookup"><span data-stu-id="d7c5b-175">Transition customers to new product plans</span></span>

<span data-ttu-id="d7c5b-176">Microsoft는 파트너에 게 새로운 제품과 서비스를 지속적으로 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="d7c5b-177">이러한 경우 고객을 새 서비스로 업그레이드 하거나 결국 종료 될 Sku에서 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="d7c5b-178">사용 중지 된 Sku에서 최신 버전으로 고객을 마이그레이션하려면 다음 단계를 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="d7c5b-179">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="d7c5b-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="d7c5b-180">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="d7c5b-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="d7c5b-181">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="d7c5b-181">Cancel the old subscription</span></span>

<span data-ttu-id="d7c5b-182">위의 표에 있는 옵션 중 하나로 고객의 Office 365 Enterprise E4 구독을 마이그레이션하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="d7c5b-183">1 단계-새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="d7c5b-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="d7c5b-184">**파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동할 고객을 선택한 다음 **구독 추가**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="d7c5b-185">카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="d7c5b-186">이제 고객에 게 이전 구독과 새 구독, 이전 Office 365 Enterprise E4 구독 및 새 ' 대상 ' 구독 (예: 1-Office 365 Enterprise E5)이 모두 포함 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="d7c5b-187">2 단계-고객의 사용자 라이선스 재할당</span><span class="sxs-lookup"><span data-stu-id="d7c5b-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="d7c5b-188">**파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동할 고객을 선택한 후 **사용자 및 라이선스**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="d7c5b-189">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="d7c5b-190">사용자 라이선스를 다시 할당 하려면 재할당할 사용자를 선택한 다음 **라이선스 관리**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="d7c5b-191">**라이선스 관리** 페이지에서 **Office 365 Enterprise E4** 라이선스 확인란의 선택을 취소 하 고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="d7c5b-192">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-192">Select **Submit**.</span></span> <span data-ttu-id="d7c5b-193">확인 페이지에 새 라이선스 할당이 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="d7c5b-194">라이선스를 다시 할당 해야 하는 다른 고객 사용자와 동일한 단계를 계속 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="d7c5b-195">사용자 라이선스를 새 서비스로 이동한 후에는 상위 고객 수준에서 사용 중지 된 구독을 안전 하 게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="d7c5b-196">3 단계-이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="d7c5b-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="d7c5b-197">**파트너 센터** 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="d7c5b-198">이동할 고객을 선택 하 고 취소 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="d7c5b-199">구독 정보 페이지에서 구독 상태를 **일시 중지 됨**으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="d7c5b-200">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-200">Select **Submit**.</span></span>

<span data-ttu-id="d7c5b-201">이전 구독이 일시 중단 되 고 새 구독이 활성 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="d7c5b-202">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d7c5b-203">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="d7c5b-203">The customer incurs no additional costs for the old subscription.</span></span>



 



