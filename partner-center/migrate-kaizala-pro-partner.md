---
title: Microsoft 365로 Kaizala Pro 구독 마이그레이션
description: Microsoft 365 또는 Office 365 버전으로 Kaizala Pro 구독을 마이그레이션하는 방법에 대해 알아봅니다. 고객 전환에 대 한 자세한 내용은이 문서를 참조 하세요.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172407"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="63214-104">Microsoft 365 또는 Office 365 버전으로 Kaizala Pro 독립 실행형 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="63214-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="63214-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="63214-105">**Appropriate roles**</span></span>

- <span data-ttu-id="63214-106">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="63214-106">Sales agent</span></span>

<span data-ttu-id="63214-107">2020 년 7 월 1 일부 터 Microsoft는 Kaizala Pro 독립 실행형 서비스의 판매를 종료 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="63214-108">이 날짜 이후에는 고객이 새 Kaizala Pro 구독을 더 이상 구매할 수 없으며 기존 Kaizala Pro 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="63214-109">고객의 연속성을 보장 하려면 Kaizala Pro 독립 실행형 구독이 만료 된 고객을 아래에 나열 된 지원 되는 SKU 옵션으로 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="63214-110">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="63214-111">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 속성과 false로 설정 된 구독의 종료 날짜를 평가 하 여 만료 된 구독을 검색할 수 있습니다 `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="63214-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="63214-112">E4 구독은 `auto renew=False` 2020 년 7 월 1 일에 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63214-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="63214-113">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="63214-114">Kaizala Pro 독립 실행형 교체 계획</span><span class="sxs-lookup"><span data-stu-id="63214-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="63214-115">새로운 요금제를 사용 하 여 고객은 Microsoft 365의 새로운 기능을 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="63214-116">가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="63214-117">다음을 포함 한 [**비즈니스 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)</span><span class="sxs-lookup"><span data-stu-id="63214-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="63214-118">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="63214-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="63214-119">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="63214-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="63214-120">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="63214-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="63214-121">[**Frontline에 대 한 Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)다음을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="63214-122">Microsoft 365 F3(이전의 Microsoft 365 F1) 및 Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="63214-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="63214-123">다음을 포함 한 [**Enterprise Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)</span><span class="sxs-lookup"><span data-stu-id="63214-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="63214-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="63214-124">Office 365 E1</span></span>
   - <span data-ttu-id="63214-125">Microsoft 365 E3 및 Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="63214-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="63214-126">Microsoft 365 E5 및 Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="63214-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="63214-127">다음을 포함 하 여 [**교육용 Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365)</span><span class="sxs-lookup"><span data-stu-id="63214-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="63214-128">Microsoft 365 A1 및 Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="63214-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="63214-129">Microsoft 365 A3 및 Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="63214-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="63214-130">Microsoft 365 A5 및 Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="63214-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="63214-131">고객을 새 제품 요금제로 전환</span><span class="sxs-lookup"><span data-stu-id="63214-131">Transition customers to new product plans</span></span>

<span data-ttu-id="63214-132">Microsoft는 파트너에 게 새로운 제품과 서비스를 지속적으로 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="63214-133">이러한 경우 고객을 새 서비스로 업그레이드 하거나 결국 종료 될 Sku에서 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="63214-134">사용 중지 된 Sku에서 최신 버전으로 고객을 마이그레이션하려면 다음 단계를 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="63214-135">A.</span><span class="sxs-lookup"><span data-stu-id="63214-135">A.</span></span> <span data-ttu-id="63214-136">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="63214-136">Purchase the new subscription</span></span>

<span data-ttu-id="63214-137">B.</span><span class="sxs-lookup"><span data-stu-id="63214-137">B.</span></span> <span data-ttu-id="63214-138">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="63214-138">Reassign current user licenses</span></span>

<span data-ttu-id="63214-139">C.</span><span class="sxs-lookup"><span data-stu-id="63214-139">C.</span></span> <span data-ttu-id="63214-140">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="63214-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="63214-141">고객을 새 요금제로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="63214-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="63214-142">A.</span><span class="sxs-lookup"><span data-stu-id="63214-142">A.</span></span> <span data-ttu-id="63214-143">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="63214-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="63214-144">새 구독을 구입 하려면 **파트너 센터** 메뉴에서 **고객** 을 선택 하 고 이동할 고객을 선택한 다음 **구독 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="63214-145">카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="63214-146">이제 고객에 게 이전 구독과 새 구독, 이전 Kaizala Pro 독립 실행형 구독 및 새로운 ' 대상 ' 구독이 모두 포함 되어 있어야 합니다 (예: 옵션 1-Office 365 Enterprise F1).</span><span class="sxs-lookup"><span data-stu-id="63214-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="63214-147">B.</span><span class="sxs-lookup"><span data-stu-id="63214-147">B.</span></span> <span data-ttu-id="63214-148">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="63214-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="63214-149">고객의 사용자 라이선스를 재할당 하려면 **파트너 센터** 메뉴에서 **고객** 을 선택 하 고 이동 하는 고객을 선택한 다음 **사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="63214-150">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="63214-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="63214-151">사용자 라이선스를 다시 할당 하려면 재할당할 사용자를 선택한 다음 **라이선스 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="63214-152">**라이선스 관리** 페이지에서 Kaizala Pro 독립 실행형 라이선스 확인란의 선택을 취소 하 고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="63214-153">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-153">Select **Submit**.</span></span> <span data-ttu-id="63214-154">확인 페이지에 새 라이선스 할당이 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63214-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="63214-155">라이선스를 할당 해야 하는 다른 사용자에 대해 동일한 프로세스를 계속 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="63214-156">C.</span><span class="sxs-lookup"><span data-stu-id="63214-156">C.</span></span> <span data-ttu-id="63214-157">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="63214-157">Cancel old subscription</span></span>

<span data-ttu-id="63214-158">사용자 라이선스를 새 서비스로 이동한 후에는 고객 수준에서 사용 중지 된 구독을 안전 하 게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63214-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="63214-159">**파트너 센터** 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="63214-160">취소할 구독이 있는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="63214-161">구독 세부 정보 페이지에서 구독을 **일시 중단 됨** 으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="63214-162">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-162">Select **Submit**.</span></span>

<span data-ttu-id="63214-163">이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="63214-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="63214-164">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63214-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="63214-165">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="63214-165">The customer incurs no additional costs for the old subscription.</span></span>
