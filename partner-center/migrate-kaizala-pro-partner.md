---
title: Microsoft 365로 Kaizala Pro 구독 마이그레이션
description: Kaizala Pro 구독을 Microsoft 365 또는 Office 365 버전으로 마이그레이션하는 방법을 알아봅니다. 고객 전환에 대한 자세한 내용은 이 문서를 읽어보세요.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146428"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="32092-104">Kaizala Pro 독립 실행형 구독을 Microsoft 365 또는 Office 365 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="32092-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="32092-105">**적절한 역할:** 영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="32092-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="32092-106">2020년 7월 1일부터 Microsoft는 Kaizala Pro 독립 실행형 서비스의 판매를 종료합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="32092-107">고객은 이 날짜 이후에 더 이상 새 Kaizala Pro 구독을 구매할 수 없으며 기존 Kaizala Pro 구독은 만료되면 자동으로 갱신되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="32092-108">고객의 연속성을 보장하려면 만료된 Kaizala Pro 독립 실행형 구독이 있는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="32092-109">고객의 서비스 중단을 방지하려면 구독의 연간 종료 날짜 이전에 고객을 새 구독으로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="32092-110">API(CREST 또는 파트너 센터)를 사용하는 경우 false로 설정된 자동 갱신 속성과 함께 구독의 종료 날짜를 평가하여 만료되는 구독을 검색할 수 `auto renew = False` 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="32092-111">E4 구독은 `auto renew=False` 2020년 7월 1일에 로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="32092-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="32092-112">언제든지 고객을 새 플랜으로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="32092-113">Kaizala Pro 독립 실행형 교체 계획</span><span class="sxs-lookup"><span data-stu-id="32092-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="32092-114">새 플랜을 통해 고객은 Microsoft 365 새로운 기능과 기능을 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="32092-115">가격 책정 세부 정보는 파트너 센터 가격표 및 제품 목록 매트릭스에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="32092-116">[**다음을 포함하여 비즈니스용 Microsoft 365.**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)</span><span class="sxs-lookup"><span data-stu-id="32092-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="32092-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="32092-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="32092-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="32092-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="32092-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="32092-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="32092-120">[**다음을 포함하여 Frontline에 대한 Microsoft 365.**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)</span><span class="sxs-lookup"><span data-stu-id="32092-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="32092-121">Microsoft 365 F3(이전의 Microsoft 365 F1) 및 Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="32092-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="32092-122">[**엔터프라이즈용 Microsoft 365:**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)</span><span class="sxs-lookup"><span data-stu-id="32092-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="32092-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="32092-123">Office 365 E1</span></span>
   - <span data-ttu-id="32092-124">Microsoft 365 E3 및 Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="32092-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="32092-125">Microsoft 365 E5 및 Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="32092-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="32092-126">[**교육용 Microsoft 365:**](https://www.microsoft.com/education/buy-license/microsoft365)</span><span class="sxs-lookup"><span data-stu-id="32092-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="32092-127">Microsoft 365 A1 및 Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="32092-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="32092-128">Microsoft 365 A3 및 Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="32092-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="32092-129">Microsoft 365 A5 및 Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="32092-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="32092-130">고객을 새 제품 플랜으로 전환</span><span class="sxs-lookup"><span data-stu-id="32092-130">Transition customers to new product plans</span></span>

<span data-ttu-id="32092-131">Microsoft는 파트너에게 지속적으로 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="32092-132">이러한 경우 고객을 새 서비스로 업그레이드하거나 최종적으로 종료될 S SKU에서 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="32092-133">사용 중지된 S SKU에서 최신 S SKU로 고객을 마이그레이션하려면 다음 단계가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="32092-134">A.</span><span class="sxs-lookup"><span data-stu-id="32092-134">A.</span></span> <span data-ttu-id="32092-135">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="32092-135">Purchase the new subscription</span></span>

<span data-ttu-id="32092-136">B.</span><span class="sxs-lookup"><span data-stu-id="32092-136">B.</span></span> <span data-ttu-id="32092-137">현재 사용자 라이선스 재할당</span><span class="sxs-lookup"><span data-stu-id="32092-137">Reassign current user licenses</span></span>

<span data-ttu-id="32092-138">C.</span><span class="sxs-lookup"><span data-stu-id="32092-138">C.</span></span> <span data-ttu-id="32092-139">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="32092-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="32092-140">고객을 새 플랜으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="32092-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="32092-141">A.</span><span class="sxs-lookup"><span data-stu-id="32092-141">A.</span></span> <span data-ttu-id="32092-142">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="32092-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="32092-143">새 구독을 구매하려면 **파트너 센터** 메뉴에서 **고객을** 선택하고 이동하려는 고객을 선택한 다음 구독 **추가를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="32092-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="32092-144">카탈로그에서 구매할 구독(이 경우 위의 옵션 중 하나)을 선택하고 라이선스 수를 입력한 다음, **제출을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="32092-145">이제 고객에게 이전 및 새 구독, 이전 Kaizala Pro 독립 실행형 구독 및 새 '대상' 구독(예: 옵션 1 - Office 365 Enterprise F1)이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="32092-146">B.</span><span class="sxs-lookup"><span data-stu-id="32092-146">B.</span></span> <span data-ttu-id="32092-147">현재 사용자 라이선스 재할당</span><span class="sxs-lookup"><span data-stu-id="32092-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="32092-148">고객의 라이선스를 다시 할당하려면 **파트너 센터** 메뉴에서 **고객을** 선택하고 이동 중인 고객을 선택한 다음 사용자 **및 라이선스를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="32092-149">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="32092-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="32092-150">사용자 라이선스를 다시 할당하려면 재할당할 사용자를 선택한 **다음, 라이선스 관리를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="32092-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="32092-151">라이선스 **관리** 페이지에서 Kaizala Pro 독립 실행형 라이선스 확인란의 선택을 취소하고 고객이 이동하는 구독에 대한 새 서비스 계획을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="32092-152">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-152">Select **Submit**.</span></span> <span data-ttu-id="32092-153">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="32092-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="32092-154">라이선스 할당이 필요한 다른 사용자에 대해 동일한 프로세스를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="32092-155">C.</span><span class="sxs-lookup"><span data-stu-id="32092-155">C.</span></span> <span data-ttu-id="32092-156">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="32092-156">Cancel old subscription</span></span>

<span data-ttu-id="32092-157">사용자 라이선스를 새 서비스로 이동한 후 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="32092-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="32092-158">**파트너 센터** 메뉴에서 **고객을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="32092-159">취소할 구독이 있는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="32092-160">구독 세부 정보 페이지에서 구독을 **일시 중단 됨** 으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="32092-161">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-161">Select **Submit**.</span></span>

<span data-ttu-id="32092-162">이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="32092-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="32092-163">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="32092-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="32092-164">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="32092-164">The customer incurs no additional costs for the old subscription.</span></span>
