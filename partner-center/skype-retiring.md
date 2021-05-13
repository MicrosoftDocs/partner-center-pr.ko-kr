---
title: 비즈니스용 Skype 구독 마이그레이션
description: 비즈니스용 Skype Online 요금제 1 구독을 만료 하는 특정 고객을 새 Office 365 버전으로 마이그레이션하는 방법 및 시기에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854828"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="83acd-103">비즈니스용 Skype Online 계획 1 구독을 최신 Office 365 버전으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="83acd-103">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="83acd-104">**적절 한 역할**: 판매 에이전트</span><span class="sxs-lookup"><span data-stu-id="83acd-104">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="83acd-105">비즈니스용 Skype Online 요금제 1은 2018 년 8 월 1 일부 터 사용이 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-105">The Skype for Business Online Plan 1 will be retired, effective August 1, 2018.</span></span> <span data-ttu-id="83acd-106">이 날짜 이후에는 고객이 새 비즈니스용 Skype 요금제 1 구독을 더 이상 구매할 수 없으며 기존 구독은 만료 될 때 자동으로 갱신 되지 않으며 갱신 옵션을 제공 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-106">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="83acd-107">구독의 세부 정보 페이지에서 비즈니스용 Skype Online 계획 1 구독 상태가 "만료 날짜 [날짜]"로 변경 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-107">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="83acd-108">고객의 연속성을 보장 하려면 아래에 나열 된 지원 되는 SKU 옵션에 대해 비즈니스용 Skype Online 요금제 1 구독을 만료 하는 고객을 전환 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-108">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="83acd-109">고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="83acd-110">비즈니스용 Skype Online 요금제 1 상용 및 정부 Sku는 모두 사용이 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-110">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="83acd-111">API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-111">If you use the API (either CREST or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="83acd-112">비즈니스용 Skype Online 계획 1 구독은 2018 년 9 월 1 일에 자동 갱신 = False로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-112">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="83acd-113">언제 든 지 새 요금제로 고객을 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-113">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="83acd-114">비즈니스용 Skype Online 요금제 1 교체 계획</span><span class="sxs-lookup"><span data-stu-id="83acd-114">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="83acd-115">새로운 요금제를 사용 하 여 고객이 Office 365의 새로운 기능과 기능을 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-115">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="83acd-116">가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="83acd-117">옵션 1: Office 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="83acd-117">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="83acd-118">옵션 2: Microsoft 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="83acd-118">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="83acd-119">옵션 3: 다른 Office 365 요금제</span><span class="sxs-lookup"><span data-stu-id="83acd-119">Option 3: Other Office 365 plans</span></span>

|<span data-ttu-id="83acd-120">**기능**</span><span class="sxs-lookup"><span data-stu-id="83acd-120">**Feature**</span></span>    |<span data-ttu-id="83acd-121">**옵션 1**</span><span class="sxs-lookup"><span data-stu-id="83acd-121">**Option 1**</span></span>   |<span data-ttu-id="83acd-122">**옵션 2**</span><span class="sxs-lookup"><span data-stu-id="83acd-122">**Option 2**</span></span>   |<span data-ttu-id="83acd-123">**옵션 3**</span><span class="sxs-lookup"><span data-stu-id="83acd-123">**Option 3**</span></span>   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="83acd-124">비즈니스용 Skype Online 요금제 1에 포함 된 모든 기능을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-124">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="83acd-125">예</span><span class="sxs-lookup"><span data-stu-id="83acd-125">Yes</span></span>   |<span data-ttu-id="83acd-126">예</span><span class="sxs-lookup"><span data-stu-id="83acd-126">Yes</span></span>   |<span data-ttu-id="83acd-127">예</span><span class="sxs-lookup"><span data-stu-id="83acd-127">Yes</span></span>   |
|<span data-ttu-id="83acd-128">IM 및 현재 상태</span><span class="sxs-lookup"><span data-stu-id="83acd-128">IM and presence</span></span> |<span data-ttu-id="83acd-129">예</span><span class="sxs-lookup"><span data-stu-id="83acd-129">Yes</span></span>   |<span data-ttu-id="83acd-130">예</span><span class="sxs-lookup"><span data-stu-id="83acd-130">Yes</span></span>   |<span data-ttu-id="83acd-131">예</span><span class="sxs-lookup"><span data-stu-id="83acd-131">Yes</span></span>   |
|<span data-ttu-id="83acd-132">IP를 통해 피어 투 피어 오디오 및 비디오</span><span class="sxs-lookup"><span data-stu-id="83acd-132">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="83acd-133">예</span><span class="sxs-lookup"><span data-stu-id="83acd-133">Yes</span></span>   |<span data-ttu-id="83acd-134">예</span><span class="sxs-lookup"><span data-stu-id="83acd-134">Yes</span></span>   |<span data-ttu-id="83acd-135">예</span><span class="sxs-lookup"><span data-stu-id="83acd-135">Yes</span></span>   
|<span data-ttu-id="83acd-136">인증된 사용자로 모임 참가</span><span class="sxs-lookup"><span data-stu-id="83acd-136">Join meetings as an authenticated user</span></span>| <span data-ttu-id="83acd-137">예</span><span class="sxs-lookup"><span data-stu-id="83acd-137">Yes</span></span>   |<span data-ttu-id="83acd-138">예</span><span class="sxs-lookup"><span data-stu-id="83acd-138">Yes</span></span>   |<span data-ttu-id="83acd-139">예</span><span class="sxs-lookup"><span data-stu-id="83acd-139">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="83acd-140">고객을 새 제품 플랜으로 전환</span><span class="sxs-lookup"><span data-stu-id="83acd-140">Transition customers to new product plans</span></span>

<span data-ttu-id="83acd-141">Microsoft는 파트너에게 지속적으로 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-141">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="83acd-142">이러한 경우 고객을 새 서비스로 업그레이드하거나 최종적으로 종료될 S SKU에서 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-142">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="83acd-143">사용 중지된 S SKU에서 최신 S SKU로 고객을 마이그레이션하려면 다음 단계가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-143">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="83acd-144">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="83acd-144">Purchase the new subscription</span></span>
- <span data-ttu-id="83acd-145">현재 사용자 라이선스 재할당</span><span class="sxs-lookup"><span data-stu-id="83acd-145">Reassign current user licenses</span></span>
- <span data-ttu-id="83acd-146">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="83acd-146">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="83acd-147">고객을 새 플랜으로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="83acd-147">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="83acd-148">새 구독을 구매하려면 **파트너 센터 메뉴에서** **고객을** 선택하고 이동하려는 고객을 선택한 다음 **구독 추가를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="83acd-148">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="83acd-149">카탈로그에서 구매할 구독(이 경우 위의 옵션 중 하나)을 선택하고 라이선스 수를 입력한 다음 **제출을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-149">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="83acd-150">이제 고객에게 이전 및 새 구독, 이전 비즈니스용 Skype Online 플랜 1 구독 및 새 '대상' 구독(예: 옵션 1 - Office 365 Enterprise F1)이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-150">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="83acd-151">고객의 라이선스를 다시 할당하려면 **파트너 센터** 메뉴에서 **고객을** 선택하고 이동 중인 고객을 선택한 다음 사용자 **및 라이선스를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-151">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="83acd-152">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-152">The customer's Users and Licenses page opens.</span></span>

4. <span data-ttu-id="83acd-153">사용자 라이선스를 다시 할당하려면 재할당할 사용자를 선택한 **다음, 라이선스 관리를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="83acd-153">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="83acd-154">라이선스 **관리** 페이지에서 비즈니스용 Skype Online 플랜 1 라이선스 확인란의 선택을 취소하고 고객이 이동하는 구독에 대한 새 서비스 계획을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-154">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="83acd-155">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-155">Select **Submit**.</span></span> <span data-ttu-id="83acd-156">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-156">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="83acd-157">라이선스 할당이 필요한 다른 사용자에 대해 이 동일한 프로세스를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-157">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="83acd-158">사용자 라이선스를 새 서비스로 이동한 후에는 고객 수준에서 사용 중지 된 구독을 안전 하 게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="83acd-159">**파트너 센터** 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="83acd-160">취소할 구독이 있는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-160">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="83acd-161">구독 세부 정보 페이지에서 구독을 **일시 중단 됨** 으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="83acd-162">**제출을 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="83acd-162">Select **Submit.**</span></span>

<span data-ttu-id="83acd-163">이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="83acd-164">일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="83acd-165">고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="83acd-165">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="83acd-166">다음 단계</span><span class="sxs-lookup"><span data-stu-id="83acd-166">Next steps</span></span>

- [<span data-ttu-id="83acd-167">Advisor: 클라이언트에서 Office 365을 사용해 볼 수 있는 평가판 초대 만들기 및 보내기</span><span class="sxs-lookup"><span data-stu-id="83acd-167">Advisors: Create and send a trial invitation for clients to try Office 365</span></span>](advisors-create-a-trial-invitation.md)
- [<span data-ttu-id="83acd-168">Advisor: Office 365 평가판 초대 및 구매 제안을 사용 하 여 클라이언트 기반 빌드</span><span class="sxs-lookup"><span data-stu-id="83acd-168">Advisors: Build your client base with Office 365 trial invitations and purchase offers</span></span>](advisors-build-your-business.md)
- [<span data-ttu-id="83acd-169">관리자: 구매 제안 만들기</span><span class="sxs-lookup"><span data-stu-id="83acd-169">Advisors: Create a purchase offer</span></span>](advisor-create-a-purchase-offer.md)
