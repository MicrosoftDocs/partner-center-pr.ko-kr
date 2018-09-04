---
title: Dynamics AX 구독을 Dynamics 365로 마이그레이션 | 파트너 센터
description: Microsoft에서는 조직이 성장, 발전 및 변혁을 통해 고객의 요구 사항을 충족하고 새로운 기회를 포착할 수 있게 해주는 차세대 지능형 비즈니스 응용 프로그램인 Dynamics 365를 소개합니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 8a8aaf2591b6a67114da7d2226dde7bf94dd06b0
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876303"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a><span data-ttu-id="8ce46-103">Dynamics AX 구독을 Dynamics 365로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="8ce46-103">Migrate Dynamics AX subscriptions to Dynamics 365</span></span>

**<span data-ttu-id="8ce46-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="8ce46-104">Applies to</span></span>**

-  <span data-ttu-id="8ce46-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="8ce46-105">Partner Center</span></span>

<span data-ttu-id="8ce46-106">Microsoft에서는 조직이 성장, 발전 및 변혁을 통해 고객의 요구 사항을 충족하고 새로운 기회를 포착할 수 있게 해주는 차세대 지능형 비즈니스 응용 프로그램인 Dynamics 365를 소개합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-106">Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.</span></span> <span data-ttu-id="8ce46-107">새 제품의 일부로 Microsoft에서는 2016년 11월 1일 고객을 위한 새로운 Microsoft Dynamics 구독 계획을 소개합니다. 이 계획은 현재 계획과 유사하지만 같지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-107">As part of the new product, Microsoft introduced new Microsoft Dynamics subscription plans for customers on November 1st, 2016, that are similar but not identical to your current plans.</span></span>

<span data-ttu-id="8ce46-108">이 문서의 지침에서는 간접 공급자가 고객의 기존 Microsoft Dynamics AX 구독 및 Microsoft Dymanics CRM Online 구독을 새 Microsoft Dynamics 365로 전환하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-108">The instructions in this document describe how indirect providers can switch customers’ existing Microsoft Dynamics AX subscriptions and Microsoft Dymanics CRM Online subscriptions to Microsoft Dynamics 365.</span></span> <span data-ttu-id="8ce46-109">이 지침은 공급자가 고객의 구독을 새 SKU로 마이그레이션해야 하는 새 버전으로 업데이트하는 다른 Microsoft 제품에도 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-109">The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.</span></span>

<span data-ttu-id="8ce46-110">Microsoft Dynamics CRM Online 및 AX 계획은 사용 중지되었습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-110">The Microsoft Dynamics CRM Online and AX plans are retired.</span></span>  <span data-ttu-id="8ce46-111">2017년 7월 1일부터 더 이상 예전 계획으로 갱신할 수 없으며 기존 E4 구독은 만료될 때 자동으로 갱신되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-111">Effective July 1, 2017, you can no longer renew into the legacy plans, also existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="8ce46-112">CRM Online 및 AX 구독은 종료 시 취소됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-112">When CRM Online and AX subscriptions end, they will be canceled.</span></span> <span data-ttu-id="8ce46-113">고객에게 연속성을 보장하기 위해 구독이 곧 만료되는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-113">To ensure continuity for customers, plan to transition customers with expiring subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="8ce46-114">고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-114">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span> 

<span data-ttu-id="8ce46-115">구독의 세부 정보 페이지에서 만료되는 구독에 대한 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경된 것을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-115">On the subscription's detail page, you will see that for these expiring subscriptions, the subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="8ce46-116">API(CREST 또는 파트너 센터)를 사용하는 경우 auto renew = False 속성과 함께 구독의 종료 날짜를 확인하여 곧 만료되는 구독을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-116">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.The subscriptions were set to auto renew=False on July 1, 2017.</span></span> <span data-ttu-id="8ce46-117">언제든지 고객을 새 요금제로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-117">You can move customers to a new plan at any time.</span></span> 

**<span data-ttu-id="8ce46-118">Microsoft Dynamics AX 라이선싱 변경</span><span class="sxs-lookup"><span data-stu-id="8ce46-118">Microsoft Dynamics AX licensing changes</span></span>**

<span data-ttu-id="8ce46-119">Microsoft Dynamics AX 제품군은 2016년 11월 1일부터 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-119">The Microsoft Dynamics AX product line was retired, effective November 1st, 2016.</span></span> <span data-ttu-id="8ce46-120">Dynamics 365의 새 라이선싱 옵션에 대한 자세한 내용을 알아보려면 [라이선싱 가이드](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="8ce46-120">To learn more about the new licensing options for Dynamics 365, review the [Licensing Guide](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).</span></span>

 <span data-ttu-id="8ce46-121">라이선스 매핑에 대한 자세한 내용은 다음 표를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8ce46-121">Refer to the following table for details on license mapping:</span></span>

|**<span data-ttu-id="8ce46-122">사용 중지된 SKU</span><span class="sxs-lookup"><span data-stu-id="8ce46-122">Retired SKU</span></span>**   |**<span data-ttu-id="8ce46-123">Dynamics 365 SKU</span><span class="sxs-lookup"><span data-stu-id="8ce46-123">Dynamics 365 SKU</span></span>**   |
|-------------------|:----------------------|
|<span data-ttu-id="8ce46-124">Enterprise SKU</span><span class="sxs-lookup"><span data-stu-id="8ce46-124">Enterprise SKU</span></span>|<span data-ttu-id="8ce46-125">Microsoft Dynamics 365 for Unified Operations 또는 Microsoft Dynamics 365 계획</span><span class="sxs-lookup"><span data-stu-id="8ce46-125">Microsoft Dynamics 365 for Unified Operations or Microsoft Dynamics 365 Plan</span></span> |
|<span data-ttu-id="8ce46-126">작업</span><span class="sxs-lookup"><span data-stu-id="8ce46-126">Task</span></span>|<span data-ttu-id="8ce46-127">Microsoft Dynamics 365 for Activity</span><span class="sxs-lookup"><span data-stu-id="8ce46-127">Microsoft Dynamics 365 for Activity</span></span>
|<span data-ttu-id="8ce46-128">작업/셀프 서비스</span><span class="sxs-lookup"><span data-stu-id="8ce46-128">Task/self service</span></span>|<span data-ttu-id="8ce46-129">Microsoft Dynamics 365 for Team Members</span><span class="sxs-lookup"><span data-stu-id="8ce46-129">Microsoft Dynamics 365 for Team Members</span></span>|
|<span data-ttu-id="8ce46-130">장치</span><span class="sxs-lookup"><span data-stu-id="8ce46-130">Device</span></span>|<span data-ttu-id="8ce46-131">Microsoft Dynamics 365 for Operations Device</span><span class="sxs-lookup"><span data-stu-id="8ce46-131">Microsoft Dynamics 365 for Operations Device</span></span>|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a><span data-ttu-id="8ce46-132">Microsoft Dynamics CRM Online 라이선싱 변경</span><span class="sxs-lookup"><span data-stu-id="8ce46-132">Microsoft Dynamics CRM Online licensing changes</span></span> 

**<span data-ttu-id="8ce46-133">Microsoft Dynamics CRM Online</span><span class="sxs-lookup"><span data-stu-id="8ce46-133">Microsoft Dynamics CRM Online</span></span>**

<span data-ttu-id="8ce46-134">현재 Microsoft Dynamics CRM Online 계획은 2016년 11월 1일부터 사용 중지되었습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-134">The current Microsoft Dynamics CRM Online plan was retired effective November 1, 2016.</span></span> <span data-ttu-id="8ce46-135">Microsoft Dynamics 365의 새 라이선싱 옵션에 대한 자세한 내용을 알아보려면 [라이선싱 가이드](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="8ce46-135">To learn more about the new licensing options for microsoft Dynaics 365, review the [licensing guide](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).</span></span> <span data-ttu-id="8ce46-136">새 라이선싱 옵션에 대한 자세한 내용은 [Important information for CRM Online customers](https://go.microsoft.com/fwlink/?linkid=831667)(CRM Online 고객에 대한 중요 정보)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8ce46-136">See [Important information for CRM Online customers](https://go.microsoft.com/fwlink/?linkid=831667) to find out more about new licensing options.</span></span>

<span data-ttu-id="8ce46-137">라이선스 매핑에 대한 자세한 내용은 다음 표를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8ce46-137">Refer to the following table for details on license mapping:</span></span>

|**<span data-ttu-id="8ce46-138">사용 중지된 SKU</span><span class="sxs-lookup"><span data-stu-id="8ce46-138">Retired SKU</span></span>**   |**<span data-ttu-id="8ce46-139">Dynamics 365 SKU</span><span class="sxs-lookup"><span data-stu-id="8ce46-139">Dynamics 365 SKU</span></span>**   |
|-------------------|:----------------------|
|<span data-ttu-id="8ce46-140">Enterprise</span><span class="sxs-lookup"><span data-stu-id="8ce46-140">Enterprise</span></span>|<span data-ttu-id="8ce46-141">Dynamics 365 엔터프라이즈 고객 참여 계획</span><span class="sxs-lookup"><span data-stu-id="8ce46-141">Dynamics 365 Enterprise Customer Engagement Plan</span></span> |
|<span data-ttu-id="8ce46-142">Professional</span><span class="sxs-lookup"><span data-stu-id="8ce46-142">Professional</span></span>|<span data-ttu-id="8ce46-143">Dynamics 365 엔터프라이즈 고객 참여 계획, Dynamics 365 for Sales 또는 Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="8ce46-143">Dynamics 365 Enterprise Customer Engagement Plan, Dynamics 365 for Sales, or Dynamics 365 for Customer Service</span></span>|
|<span data-ttu-id="8ce46-144">Basic</span><span class="sxs-lookup"><span data-stu-id="8ce46-144">Basic</span></span>|<span data-ttu-id="8ce46-145">Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service 또는 Dynamics 365 엔터프라이즈 고객 참여 계획</span><span class="sxs-lookup"><span data-stu-id="8ce46-145">Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service, or Dynamics 365 Enterprise Customer Engagement Plan</span></span>|
|<span data-ttu-id="8ce46-146">Essential</span><span class="sxs-lookup"><span data-stu-id="8ce46-146">Essential</span></span>|<span data-ttu-id="8ce46-147">Dynamics 365 for Team Members</span><span class="sxs-lookup"><span data-stu-id="8ce46-147">Dynamics 365 for Team Members</span></span>|
|<span data-ttu-id="8ce46-148">Field Service 추가 기능</span><span class="sxs-lookup"><span data-stu-id="8ce46-148">Field service add-on</span></span>|<span data-ttu-id="8ce46-149">Dynamics 365 엔터프라이즈 고객 참여 계획 또는 Dynamics 365 for Field Service</span><span class="sxs-lookup"><span data-stu-id="8ce46-149">Dynamics 365 Enterprise Customer Engagement Plan or Dynamics 365 for Field Service</span></span>|
|<span data-ttu-id="8ce46-150">Project Service Authomation 추가 기능</span><span class="sxs-lookup"><span data-stu-id="8ce46-150">Project Service Authomation Add-on</span></span>|<span data-ttu-id="8ce46-151">Dynamics 365 엔터프라이즈 고객 참여 계획 또는 Dynamics 365 for Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="8ce46-151">Dynamics 365 Customer Engagement Plan or Dynamics 365 for Project Service Automation</span></span>|



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8ce46-152">새 제품 요금제로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="8ce46-152">Transition customers to new product plans</span></span>


<span data-ttu-id="8ce46-153">Microsoft는 지속적으로 재판매인 및 공급자에 새 제품 및 서비스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-153">Microsoft continuously offers new products and services to resellers and providers.</span></span> <span data-ttu-id="8ce46-154">이러한 경우 재판매인은 고객을 새 서비스로 업그레이드하거나 결국 종료될 SKU의 구독을 마이그레이션해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-154">In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="8ce46-155">이전 SKU에서 새 SKU로 고객을 마이그레이션하려면 다음 순서가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-155">Migrating customers from old SKUs to newer ones requires the following sequence:</span></span>

-   <span data-ttu-id="8ce46-156">[새 구독 구매](#manual-subscription-migration-purchasenewsubsc)</span><span class="sxs-lookup"><span data-stu-id="8ce46-156">[Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);</span></span>
-   <span data-ttu-id="8ce46-157">[현재 사용자 라이선스 다시 할당](#manual-subscription-migration-reassignlicenses)</span><span class="sxs-lookup"><span data-stu-id="8ce46-157">[Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);</span></span>
-   <span data-ttu-id="8ce46-158">[이전 구독 취소](#manual-subscription-migration-cancelsubscriptions).</span><span class="sxs-lookup"><span data-stu-id="8ce46-158">[Cancel the old subscription](#manual-subscription-migration-cancelsubscriptions).</span></span>

<span data-ttu-id="8ce46-159">다음 절차에서는 Microsoft Dynamics AX 또는 CRM Online에서 Dynamics 365로 고객을 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-159">In the following procedures, you move a customer from Microsoft Dynamics AX or CRM Online to Dynamics 365.</span></span>

<span data-ttu-id="8ce46-160">재판매인은 Dynamics AX Enterprise에 대한 기존 구독이 있는 고객을 Dynamics 365 for Operations로 이동해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-160">In this example, the reseller needs to move a customer with an existing subscription for Dynamics AX Enterprise to Dynamics 365 for Operations.</span></span> <span data-ttu-id="8ce46-161">첫 번째 단계는 Dynamics 365 for Operations를 구매하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-161">Your first step is to purchase Dynamics 365 for Operations.</span></span>  <span data-ttu-id="8ce46-162">Microsoft Dynamics 365로 이동하는 CRM Online 고객에 대해 이러한 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-162">Repeat these steps for a CRM Online customer moving to Microsoft Dynamics 365.</span></span>

<a href="" id="purchasenewsubsc"></a>

**<span data-ttu-id="8ce46-163">새 구독 구매</span><span class="sxs-lookup"><span data-stu-id="8ce46-163">Purchase the new subscription</span></span>**

1.  <span data-ttu-id="8ce46-164">**대시보드** 메뉴에서 **고객**을 선택하고 이동하려는 고객을 선택한 다음 **구독 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-164">From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.</span></span>
2.  <span data-ttu-id="8ce46-165">카탈로그에서 구매할 구독을 선택하고(이 경우 Dynamics 365 for Operations, Enterprise Edition) 라이선스 수를 입력한 다음 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-165">Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.</span></span>

    <span data-ttu-id="8ce46-166">이제 고객은 이전 구독과 새 구독이 둘 다 있어야 합니다. 이 예제에서는 이전 Dynamics AX Enterprise와 새 '대상' 구독인 Dynamics 365 for Operations, Enterprise Edition이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-166">Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.</span></span>

<a href="" id="reassignlicenses"></a> <span data-ttu-id="8ce46-167">다음 단계는 새 구독에 모든 기존 사용자 라이선스를 다시 할당하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-167">The next step is to reassign all existing user licenses to the new subscription.</span></span>

**<span data-ttu-id="8ce46-168">사용자 라이선스 다시 할당</span><span class="sxs-lookup"><span data-stu-id="8ce46-168">Reassign user licenses</span></span>**

1.  <span data-ttu-id="8ce46-169">**대시보드** 메뉴에서 **고객**을 선택하고 이동하려는 고객을 선택한 다음 **사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-169">From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**.</span></span> <span data-ttu-id="8ce46-170">고객의 사용자 및 라이선스 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-170">The customer’s Users and Licenses page opens.</span></span>
2.  <span data-ttu-id="8ce46-171">사용자 라이선스를 다시 할당하려면 다시 할당할 사용자를 선택한 다음 **라이선스 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-171">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>
3.  <span data-ttu-id="8ce46-172">**라이선스 관리** 페이지에서 **Dynamics AX Enterprise** 라이선스 확인란을 선택 취소하고 **Dynamics 365 for Operations** 라이선스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-172">On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.</span></span>
4.  <span data-ttu-id="8ce46-173">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-173">Select **Submit**.</span></span> <span data-ttu-id="8ce46-174">확인 페이지에 새 라이선스 할당이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-174">A confirmation page lists the new license assignments.</span></span>
5.  <span data-ttu-id="8ce46-175">라이선스 다시 할당이 필요한 다른 모든 고객 사용자에 대해 같은 단계를 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-175">Continue the same steps with any other customer users that need license reassignment.</span></span>

<a href="" id="cancelsubscriptions"></a> <span data-ttu-id="8ce46-176">사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 이전 구독을 안전하게 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-176">After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.</span></span>

**<span data-ttu-id="8ce46-177">이전 구독 취소</span><span class="sxs-lookup"><span data-stu-id="8ce46-177">Cancel the old subscription</span></span>**

1.  <span data-ttu-id="8ce46-178">**대시보드** 메뉴에서 **고객**을 선택하고 이동하려는 고객을 선택한 다음 취소할 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-178">From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.</span></span>
2.  <span data-ttu-id="8ce46-179">구독 세부 정보 페이지에서 구독 **상태**를 **일시 중단됨**으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-179">In the subscription details page, set the subscription **Status** to **Suspended**.</span></span>
3.  <span data-ttu-id="8ce46-180">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-180">Select **Submit**.</span></span>

<span data-ttu-id="8ce46-181">이전 구독이 일시 중단되고 새 구독이 활성화됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-181">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="8ce46-182">일시 중단된 구독은 자동으로 120일 후 프로비전이 해제됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-182">The suspended subscription will automatically be de-provisioned after 120 days.</span></span> <span data-ttu-id="8ce46-183">이전 구독에 대해서는 고객에게 추가 비용이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-183">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="additional-considerations"></a><span data-ttu-id="8ce46-184">추가 고려 사항</span><span class="sxs-lookup"><span data-stu-id="8ce46-184">Additional considerations</span></span>


<span data-ttu-id="8ce46-185">이후 구독 프로비전을 위해 고객이 개방형 채널에서 클라우드 서비스 프로그램으로 이전하는 경우 기존 구독도 마이그레이션해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-185">If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:</span></span>

-   <span data-ttu-id="8ce46-186">고객이 개방형 채널을 통해 이전 구독을 받은 경우 새 SKU의 CSP로 이동하는 작업은 간단합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-186">If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.</span></span>
-   <span data-ttu-id="8ce46-187">고객이 귀하의 고객으로 아직 설정되지 않은 경우 고객을 초대할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-187">If the customer is not yet established as your customer, you can invite them.</span></span> <span data-ttu-id="8ce46-188">자세한 내용은 [고객과의 관계 요청](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) 도움말 항목을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8ce46-188">For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.</span></span>

<span data-ttu-id="8ce46-189">고객이 귀하를 간접 공급자로 수락한 후 프로비전 단계는 대개 위에 설명된 내용과 같습니다. 즉, 새 구독을 구매한 다음 사용자 라이선스를 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-189">After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses.</span></span> <span data-ttu-id="8ce46-190">유일한 차이점은 이전 구독 취소가 수반된다는 점입니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-190">The only difference involves cancellation of old subscription(s).</span></span> <span data-ttu-id="8ce46-191">새 공급자는 다른 채널을 통해 취득한 구독을 일시 중단/취소할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-191">A new provider cannot cancel suspend/cancel subscriptions acquired via other channels.</span></span> <span data-ttu-id="8ce46-192">고객이 다른 판매 채널(예: 개방형 채널)을 통해 이전 구독을 취득한 경우 고객은 해당 채널을 통해 이전 구독을 직접 취소해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ce46-192">If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.</span></span>

 

 



