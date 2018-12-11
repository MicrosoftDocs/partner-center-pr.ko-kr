---
title: 비즈니스용 Skype Online 플랜 1 구독을 새로운 Office 365 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
Description: Transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option. We recommend moving customers to new subscriptions before the subscription’s yearly end date.
author: labrenne
ms.author: labrenne
keywords: 비즈니스용 Skype 플랜, Skype 사용 중지, Office 365
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: c1e4f4611c6fe3c317339af1a036194031f3d095
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917625"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="b1688-103">비즈니스용 Skype Online 플랜 1 구독을 새로운 Office 365 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="b1688-103">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

**<span data-ttu-id="b1688-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="b1688-104">Applies to</span></span>**

- <span data-ttu-id="b1688-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b1688-105">Partner Center</span></span>

<span data-ttu-id="b1688-106">비즈니스용 Skype Online 플랜 1은 2018년 8월 1일 기준으로 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-106">The Skype for Business Online Plan 1 will be retired, effective August 1 2018.</span></span> <span data-ttu-id="b1688-107">이 날짜 이후에 고객은 더 이상 새로운 비즈니스용 Skype Online 플랜 1 구독을 구입할 수 없으며 기존 구독이 만료되면 자동으로 갱신되지 않고 갱신 옵션도 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-107">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="b1688-108">비즈니스용 Skype Online 플랜 1 구독의 세부 정보 페이지에서 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-108">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="b1688-109">고객에게 연속성을 보장하기 위해, 비즈니스용 Skype Online 플랜 1 구독이 곧 만료되는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-109">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="b1688-110">고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="b1688-111">비즈니스용 Skype Online 플랜 1 상용 및 정부 SKU는 모두 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-111">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="b1688-112">API(CREST 또는 파트너 센터)를 사용하는 경우 auto renew = False 속성과 함께 구독의 종료 날짜를 확인하여 곧 만료되는 구독을 검색하세요.</span><span class="sxs-lookup"><span data-stu-id="b1688-112">If you use the API (either CREST or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b1688-113">비즈니스용 Skype Online 플랜 1 구독은 2018년 9월 1일에 auto renew=False로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-113">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="b1688-114">언제든지 고객을 새 요금제로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-114">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="b1688-115">비즈니스용 Skype Online 플랜 1 사용 중지 계획</span><span class="sxs-lookup"><span data-stu-id="b1688-115">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="b1688-116">새로운 요금제를 통해 고객은 Office 365의 새로운 기능을 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-116">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="b1688-117">가격 정보는 가격 목록에서 찾을 수 있으며 파트너 센터에 목록표가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-117">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="b1688-118">옵션 1: Office 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="b1688-118">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="b1688-119">옵션 2: Microsoft 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="b1688-119">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="b1688-120">옵션 3: Other Office 365 플랜</span><span class="sxs-lookup"><span data-stu-id="b1688-120">Option 3: Other Office 365 plans</span></span>

|**<span data-ttu-id="b1688-121">기능</span><span class="sxs-lookup"><span data-stu-id="b1688-121">Feature</span></span>**    |**<span data-ttu-id="b1688-122">옵션 1</span><span class="sxs-lookup"><span data-stu-id="b1688-122">Option 1</span></span>**   |**<span data-ttu-id="b1688-123">옵션 2</span><span class="sxs-lookup"><span data-stu-id="b1688-123">Option 2</span></span>**   |**<span data-ttu-id="b1688-124">옵션 3</span><span class="sxs-lookup"><span data-stu-id="b1688-124">Option 3</span></span>**   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="b1688-125">비즈니스용 Skype Online 플랜 1에 포함된 모든 기능 사용</span><span class="sxs-lookup"><span data-stu-id="b1688-125">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="b1688-126">예</span><span class="sxs-lookup"><span data-stu-id="b1688-126">Yes</span></span>   |<span data-ttu-id="b1688-127">예</span><span class="sxs-lookup"><span data-stu-id="b1688-127">Yes</span></span>   |<span data-ttu-id="b1688-128">예</span><span class="sxs-lookup"><span data-stu-id="b1688-128">Yes</span></span>   |
|<span data-ttu-id="b1688-129">IM 및 상태 확인</span><span class="sxs-lookup"><span data-stu-id="b1688-129">IM and presence</span></span> |<span data-ttu-id="b1688-130">예</span><span class="sxs-lookup"><span data-stu-id="b1688-130">Yes</span></span>   |<span data-ttu-id="b1688-131">예</span><span class="sxs-lookup"><span data-stu-id="b1688-131">Yes</span></span>   |<span data-ttu-id="b1688-132">예</span><span class="sxs-lookup"><span data-stu-id="b1688-132">Yes</span></span>   |
|<span data-ttu-id="b1688-133">IP를 통한 피어 투 피어 오디오 및 비디오</span><span class="sxs-lookup"><span data-stu-id="b1688-133">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="b1688-134">예</span><span class="sxs-lookup"><span data-stu-id="b1688-134">Yes</span></span>   |<span data-ttu-id="b1688-135">예</span><span class="sxs-lookup"><span data-stu-id="b1688-135">Yes</span></span>   |<span data-ttu-id="b1688-136">예</span><span class="sxs-lookup"><span data-stu-id="b1688-136">Yes</span></span>   
|<span data-ttu-id="b1688-137">인증된 사용자로 회의 참여</span><span class="sxs-lookup"><span data-stu-id="b1688-137">Join meetings as an authenticated user</span></span>| <span data-ttu-id="b1688-138">예</span><span class="sxs-lookup"><span data-stu-id="b1688-138">Yes</span></span>   |<span data-ttu-id="b1688-139">예</span><span class="sxs-lookup"><span data-stu-id="b1688-139">Yes</span></span>   |<span data-ttu-id="b1688-140">예</span><span class="sxs-lookup"><span data-stu-id="b1688-140">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b1688-141">새 제품 요금제로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="b1688-141">Transition customers to new product plans</span></span>

<span data-ttu-id="b1688-142">Microsoft는 지속적으로 파트너에게 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-142">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="b1688-143">다음과 같은 경우 파트너는 고객을 새 서비스로 업그레이드하거나 결국 종료될 SKU의 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-143">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="b1688-144">사용 중지된 SKU에서 새 SKU로 고객을 마이그레이션하려면 다음 단계를 따라야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-144">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="b1688-145">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="b1688-145">Purchase the new subscription</span></span>
- <span data-ttu-id="b1688-146">현재 사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="b1688-146">Reassign current user licenses</span></span>
- <span data-ttu-id="b1688-147">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="b1688-147">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="b1688-148">고객을 새 플랜으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="b1688-148">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="b1688-149">**파트너 센터 메뉴**에서 새 구독을 구매, **고객**을 선택 하 고 이동 하려는 고객을 선택한 다음 **구독 추가**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-149">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="b1688-150">카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-150">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b1688-151">이제 고객은 기존 구독과 새 구독, 다시 말해서 기존 비즈니스용 Skype Online 플랜 1 구독과 새로운 '대상' 구독(예: 옵션 1 - Office 365 Enterprise F1)을 모두 갖고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-151">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new ‘target’ subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="b1688-152">**파트너 센터** 메뉴에서 고객의 사용자 라이선스를 할당 하는 **고객**을 선택, 이동, 하 고 **사용자 및 라이선스를**선택 하면 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-152">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="b1688-153">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-153">The customer’s Users and Licenses page opens.</span></span>

4. <span data-ttu-id="b1688-154">사용자 라이선스를 다시 할당하려면 다시 할당할 사용자를 선택한 다음 **라이선스 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-154">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="b1688-155">**라이선스 관리** 페이지에서 비즈니스용 Skype Online 플랜 1 라이선스 확인란의 선택을 취소한 다음 고객을 이동할 구독의 새로운 서비스 요금제를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-155">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="b1688-156">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-156">Select **Submit**.</span></span> <span data-ttu-id="b1688-157">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-157">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="b1688-158">라이센스 할당이 필요한 다른 사용자에 대해 이 프로세스를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-158">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="b1688-159">사용자 라이선스를 새 서비스로 이동한 후 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-159">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="b1688-160">**파트너 센터** 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-160">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="b1688-161">구독 취소 중인 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-161">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="b1688-162">구독 세부 정보 페이지에서 구독을 **일시 중단됨**으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-162">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="b1688-163">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-163">Select **Submit.**</span></span>

<span data-ttu-id="b1688-164">이전 구독이 일시 중단되고 새 구독이 활성화됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-164">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="b1688-165">일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-165">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b1688-166">이전 구독에 대해서는 고객에게 추가 비용이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1688-166">The customer incurs no additional costs for the old subscription.</span></span>

