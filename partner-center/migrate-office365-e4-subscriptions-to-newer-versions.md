---
title: Office 365 E4 구독을 Office 365 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: Microsoft Office 365 Enterprise E4 버전은 2017년 4월 7일부로 사용 중지되었습니다. 고객 구독을 Office 365 최신 버전으로 마이그레이션하는 방법을 알아보세요.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 381b4c5dda7486737ef010d7fa22e65710b5e5bf
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587796"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="2fae6-104">Office 365 E4 구독을 Office 365 최신 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="2fae6-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="2fae6-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="2fae6-105">**Applies to**</span></span>

-  <span data-ttu-id="2fae6-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="2fae6-106">Partner Center</span></span>

<span data-ttu-id="2fae6-107">Office 365 Enterprise E4 요금제가 2017년 4월 7일부로 사용 중지되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-107">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="2fae6-108">이 날짜 이후로는 더 이상 새 Office 365 E4 구독을 구입할 수 없으며, 기존 E4 구독은 만료 시 자동으로 갱신되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-108">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="2fae6-109">E4 구독이 만료되면 구독이 취소됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-109">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="2fae6-110">고객에게 연속성을 보장하기 위해, E4 구독이 곧 만료되는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-110">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="2fae6-111">고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-111">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="2fae6-112">Office 365 Enterprise E4 상용 및 government Sku 사용이 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-112">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="2fae6-113">구독의 세부 정보 페이지에서 E4 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-113">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2fae6-114">API(CREST 또는 파트너 센터)를 사용하는 경우 auto renew = False 속성과 함께 구독의 종료 날짜를 확인하여 곧 만료되는 구독을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-114">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="2fae6-115">E4 구독은 2017년 4월 7일에 auto renew=False로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-115">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="2fae6-116">언제든지 고객을 새 요금제로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-116">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="2fae6-117">Office 365 Enterprise E4 버전 교체 요금제</span><span class="sxs-lookup"><span data-stu-id="2fae6-117">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="2fae6-118">E4와 같은 기능을 그대로 유지할 수도 있고 고객이 Office 365 및 비즈니스용 Skype Online의 새로운 기능을 활용하게 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-118">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="2fae6-119">가격 정보는 가격 목록에서 찾을 수 있으며 파트너 센터에 목록표가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-119">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="2fae6-120">Secure Product Enterprise E3 또는 Secure Productive Enterprise E5는 각각 Office 365 Enterprise E3 또는 Office 365 Enterprise E5에 대한 다음 옵션에서 대체될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-120">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="2fae6-121">옵션 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="2fae6-121">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="2fae6-122">옵션 2: Office 365 Enterprise E3 + 비즈니스 클라우드 PBX Skype</span><span class="sxs-lookup"><span data-stu-id="2fae6-122">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="2fae6-123">옵션 3: Office 365 Enterprise E3 + Skype for Business 및 CAL (E4 사용 하 여 가격 및 기능 패리티)</span><span class="sxs-lookup"><span data-stu-id="2fae6-123">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="2fae6-124">옵션 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="2fae6-124">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="2fae6-125">기능</span><span class="sxs-lookup"><span data-stu-id="2fae6-125">Feature</span></span> | <span data-ttu-id="2fae6-126">옵션 1</span><span class="sxs-lookup"><span data-stu-id="2fae6-126">Option 1</span></span> | <span data-ttu-id="2fae6-127">옵션 2</span><span class="sxs-lookup"><span data-stu-id="2fae6-127">Option 2</span></span> | <span data-ttu-id="2fae6-128">옵션 3</span><span class="sxs-lookup"><span data-stu-id="2fae6-128">Option 3</span></span> | <span data-ttu-id="2fae6-129">옵션 4</span><span class="sxs-lookup"><span data-stu-id="2fae6-129">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="2fae6-130">Office 365 Enterprise E4의 모든 기능을 제공하나요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-130">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="2fae6-131">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-131">Yes</span></span> | <span data-ttu-id="2fae6-132">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-132">Yes</span></span> | <span data-ttu-id="2fae6-133">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-133">Yes</span></span> | <span data-ttu-id="2fae6-134">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-134">No</span></span> |
| <span data-ttu-id="2fae6-135">전화 번호를 Office 365에서 관리하나요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-135">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="2fae6-136">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-136">Yes</span></span> | <span data-ttu-id="2fae6-137">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-137">Yes</span></span> | <span data-ttu-id="2fae6-138">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-138">No</span></span> | <span data-ttu-id="2fae6-139">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-139">No</span></span> |
| <span data-ttu-id="2fae6-140">전화 번호를 온-프레미스와 Office 365 모두에서 관리하나요(하이브리드 배포)?</span><span class="sxs-lookup"><span data-stu-id="2fae6-140">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="2fae6-141">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-141">Yes</span></span> | <span data-ttu-id="2fae6-142">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-142">Yes</span></span> | <span data-ttu-id="2fae6-143">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-143">No</span></span> | <span data-ttu-id="2fae6-144">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-144">No</span></span> |
| <span data-ttu-id="2fae6-145">PSTN 음성 통화 요금제를 추가할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-145">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="2fae6-146">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-146">Yes</span></span> | <span data-ttu-id="2fae6-147">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-147">Yes</span></span> | <span data-ttu-id="2fae6-148">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-148">No</span></span> | <span data-ttu-id="2fae6-149">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-149">No</span></span> |
| <span data-ttu-id="2fae6-150">PSTN 회의가 가능한가요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-150">PSTN Conferencing?</span></span> | <span data-ttu-id="2fae6-151">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-151">Yes</span></span> | <span data-ttu-id="2fae6-152">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-152">No</span></span> | <span data-ttu-id="2fae6-153">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-153">No</span></span> | <span data-ttu-id="2fae6-154">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-154">No</span></span> |
| <span data-ttu-id="2fae6-155">공동 작업, 분석 및 보안을 위한 고급 도구가 제공되나요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-155">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="2fae6-156">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-156">Yes</span></span> | <span data-ttu-id="2fae6-157">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-157">No</span></span> | <span data-ttu-id="2fae6-158">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-158">No</span></span> | <span data-ttu-id="2fae6-159">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-159">No</span></span> |
| <span data-ttu-id="2fae6-160">대화형 보고서, 대시보드 및 데이터 시각화가 제공되나요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-160">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="2fae6-161">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-161">Yes</span></span> | <span data-ttu-id="2fae6-162">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-162">No</span></span> | <span data-ttu-id="2fae6-163">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-163">No</span></span> | <span data-ttu-id="2fae6-164">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-164">No</span></span> | 
| <span data-ttu-id="2fae6-165">기본 프라이버시, 투명성 및 정교한 사용자 컨트롤로 데이터 보안과 규정 준수를 보다 철저하게 제어할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="2fae6-165">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="2fae6-166">예</span><span class="sxs-lookup"><span data-stu-id="2fae6-166">Yes</span></span> | <span data-ttu-id="2fae6-167">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-167">No</span></span> | <span data-ttu-id="2fae6-168">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-168">No</span></span> | <span data-ttu-id="2fae6-169">아니오</span><span class="sxs-lookup"><span data-stu-id="2fae6-169">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2fae6-170">새 제품 계획으로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="2fae6-170">Transition customers to new product plans</span></span>

<span data-ttu-id="2fae6-171">Microsoft는 지속적으로 파트너에게 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-171">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="2fae6-172">다음과 같은 경우 파트너는 고객을 새 서비스로 업그레이드하거나 결국 종료될 SKU의 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-172">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="2fae6-173">사용 중지된 SKU에서 새 SKU로 고객을 마이그레이션하려면 다음 단계를 따라야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-173">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="2fae6-174">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="2fae6-174">Purchase the new subscription</span></span>
-   <span data-ttu-id="2fae6-175">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="2fae6-175">Reassign current user licenses</span></span>
-   <span data-ttu-id="2fae6-176">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="2fae6-176">Cancel the old subscription</span></span>

<span data-ttu-id="2fae6-177">다음 단계에 따라 고객의 Office 365 Enterprise E4 구독을 아래 표의 옵션 중 하나로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-177">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="2fae6-178">1단계 - 새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="2fae6-178">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="2fae6-179">**파트너 센터** 메뉴에서 **고객**, 이동 및 선택 하려는 고객을 선택 **구독 추가**.</span><span class="sxs-lookup"><span data-stu-id="2fae6-179">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="2fae6-180">카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-180">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="2fae6-181">이제 고객은 기존 구독과 새 구독, 다시 말해서 기존 Office 365 엔터프라이즈 E4 구독과 새로운 '대상' 구독(예: 옵션 1 - Office 365 Enterprise E5)을 모두 갖고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-181">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new ‘target’ subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="2fae6-182">2단계 - 고객의 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="2fae6-182">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="2fae6-183">**파트너 센터** 메뉴에서 **고객**, 이동 및 선택 하려는 고객을 선택 **사용자 및 라이선스**합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-183">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="2fae6-184">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-184">The customer’s Users and Licenses page opens.</span></span>

2. <span data-ttu-id="2fae6-185">사용자 라이선스를 다시 할당하려면 다시 할당할 사용자를 선택한 다음 **라이선스 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-185">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="2fae6-186">**라이선스 관리** 페이지에서 **Office 365 Enterprise E4** 라이선스 확인란의 선택을 취소한 다음 고객을 이동할 구독의 새로운 서비스 요금제를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-186">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="2fae6-187">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-187">Select **Submit**.</span></span> <span data-ttu-id="2fae6-188">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-188">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="2fae6-189">라이선스 다시 할당이 필요한 다른 모든 고객 사용자에 대해 같은 단계를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-189">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="2fae6-190">사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-190">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="2fae6-191">3단계 - 이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="2fae6-191">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="2fae6-192">**파트너 센터** 메뉴에서 **고객**합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-192">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2fae6-193">이동하려는 고객을 선택하고, 취소할 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-193">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="2fae6-194">구독 세부 정보 페이지에서 구독 상태를 **일시 중단됨**으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-194">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="2fae6-195">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-195">Select **Submit**.</span></span>

<span data-ttu-id="2fae6-196">이전 구독이 일시 중단되고 새 구독이 활성화됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-196">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="2fae6-197">일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-197">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2fae6-198">이전 구독에 대해서는 고객에게 추가 비용이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2fae6-198">The customer incurs no additional costs for the old subscription.</span></span>



 



