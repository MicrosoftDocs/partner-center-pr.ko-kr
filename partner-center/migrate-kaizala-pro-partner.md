---
title: Microsoft365로 Kaizala Pro 구독 마이그레이션
description: Microsoft365 또는 Office 365 버전으로 Kaizala Pro 구독을 마이그레이션하는 방법에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611239"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="5456b-103">Microsoft365 또는 Office 365 버전으로 Kaizala Pro 독립 실행형 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="5456b-103">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="5456b-104">2020 년 7 월 1 일부 터 Microsoft는 Kaizala Pro 독립 실행형 서비스의 판매를 종료 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-104">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="5456b-105">이 날짜 이후에는 고객이 새 Kaizala Pro 구독을 더 이상 구매할 수 없으며 기존 Kaizala Pro 구독은 만료 될 때 자동으로 갱신 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-105">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="5456b-106">고객의 연속성을 보장 하려면 Kaizala Pro 독립 실행형 구독이 만료 된 고객을 아래에 나열 된 지원 되는 SKU 옵션으로 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-106">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="5456b-107">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-107">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="5456b-108">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 속성과 false로 설정 된 구독의 종료 날짜를 평가 하 여 만료 된 구독을 검색할 수 있습니다 `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="5456b-108">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="5456b-109">E4 구독은 `auto renew=False` 2020 년 7 월 1 일에 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-109">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="5456b-110">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-110">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="5456b-111">Kaizala Pro 독립 실행형 교체 계획</span><span class="sxs-lookup"><span data-stu-id="5456b-111">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="5456b-112">새로운 요금제를 사용 하 여 고객은 Microsoft 365의 새로운 기능을 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-112">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="5456b-113">가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-113">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="5456b-114">다음을 포함 한 [**비즈니스 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)</span><span class="sxs-lookup"><span data-stu-id="5456b-114">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="5456b-115">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="5456b-115">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="5456b-116">Microsoft 365 Business 표준</span><span class="sxs-lookup"><span data-stu-id="5456b-116">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="5456b-117">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="5456b-117">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="5456b-118">[**Frontline에 대 한 Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)다음을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-118">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="5456b-119">Microsoft 365 F3 (이전의 Microsoft 365 F1) 및 Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="5456b-119">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="5456b-120">다음을 포함 한 [**Enterprise Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)</span><span class="sxs-lookup"><span data-stu-id="5456b-120">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="5456b-121">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="5456b-121">Office 365 E1</span></span>
   - <span data-ttu-id="5456b-122">Microsoft 365 E3 및 Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="5456b-122">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="5456b-123">Microsoft 365 E5 및 Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="5456b-123">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="5456b-124">다음을 포함 하 여 [**교육용 Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365)</span><span class="sxs-lookup"><span data-stu-id="5456b-124">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="5456b-125">Microsoft 365 A1 및 Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="5456b-125">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="5456b-126">Microsoft 365 A3 및 Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="5456b-126">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="5456b-127">Microsoft 365 A5 및 Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="5456b-127">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5456b-128">고객을 새 제품 요금제로 전환</span><span class="sxs-lookup"><span data-stu-id="5456b-128">Transition customers to new product plans</span></span>

<span data-ttu-id="5456b-129">Microsoft는 파트너에 게 새로운 제품과 서비스를 지속적으로 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-129">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="5456b-130">이러한 경우 고객을 새 서비스로 업그레이드 하거나 결국 종료 될 Sku에서 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-130">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="5456b-131">사용 중지 된 Sku에서 최신 버전으로 고객을 마이그레이션하려면 다음 단계를 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-131">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="5456b-132">A.</span><span class="sxs-lookup"><span data-stu-id="5456b-132">A.</span></span> <span data-ttu-id="5456b-133">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="5456b-133">Purchase the new subscription</span></span>

<span data-ttu-id="5456b-134">B.</span><span class="sxs-lookup"><span data-stu-id="5456b-134">B.</span></span> <span data-ttu-id="5456b-135">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="5456b-135">Reassign current user licenses</span></span>

<span data-ttu-id="5456b-136">C.</span><span class="sxs-lookup"><span data-stu-id="5456b-136">C.</span></span> <span data-ttu-id="5456b-137">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="5456b-137">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="5456b-138">고객을 새 요금제로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="5456b-138">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="5456b-139">A.</span><span class="sxs-lookup"><span data-stu-id="5456b-139">A.</span></span> <span data-ttu-id="5456b-140">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="5456b-140">Purchase the new subscription</span></span>

1. <span data-ttu-id="5456b-141">새 구독을 구입 하려면 **파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동할 고객을 선택한 다음 **구독 추가**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-141">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="5456b-142">카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-142">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="5456b-143">이제 고객에 게 이전 구독과 새 구독, 이전 Kaizala Pro 독립 실행형 구독 및 새로운 ' 대상 ' 구독이 모두 포함 되어 있어야 합니다 (예: 옵션 1-Office 365 Enterprise F1).</span><span class="sxs-lookup"><span data-stu-id="5456b-143">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="5456b-144">B.</span><span class="sxs-lookup"><span data-stu-id="5456b-144">B.</span></span> <span data-ttu-id="5456b-145">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="5456b-145">Reassign current user licenses</span></span>

1. <span data-ttu-id="5456b-146">고객의 사용자 라이선스를 재할당 하려면 **파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동 하는 고객을 선택한 다음 **사용자 및 라이선스**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-146">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="5456b-147">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-147">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="5456b-148">사용자 라이선스를 다시 할당 하려면 재할당할 사용자를 선택한 다음 **라이선스 관리**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-148">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="5456b-149">**라이선스 관리** 페이지에서 Kaizala Pro 독립 실행형 라이선스 확인란의 선택을 취소 하 고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-149">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="5456b-150">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-150">Select **Submit**.</span></span> <span data-ttu-id="5456b-151">확인 페이지에 새 라이선스 할당이 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-151">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="5456b-152">라이선스를 할당 해야 하는 다른 사용자에 대해 동일한 프로세스를 계속 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-152">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="5456b-153">C.</span><span class="sxs-lookup"><span data-stu-id="5456b-153">C.</span></span> <span data-ttu-id="5456b-154">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="5456b-154">Cancel old subscription</span></span>

<span data-ttu-id="5456b-155">사용자 라이선스를 새 서비스로 이동한 후에는 고객 수준에서 사용 중지 된 구독을 안전 하 게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-155">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="5456b-156">**파트너 센터** 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-156">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="5456b-157">취소할 구독이 있는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-157">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="5456b-158">구독 세부 정보 페이지에서 구독을 **일시 중단 됨**으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-158">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="5456b-159">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-159">Select **Submit**.</span></span>

<span data-ttu-id="5456b-160">이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-160">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="5456b-161">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-161">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="5456b-162">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="5456b-162">The customer incurs no additional costs for the old subscription.</span></span>
