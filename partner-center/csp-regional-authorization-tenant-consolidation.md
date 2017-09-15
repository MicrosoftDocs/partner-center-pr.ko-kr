---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="88c06-103">CSP regional authorization tenant consolidation</span><span class="sxs-lookup"><span data-stu-id="88c06-103">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="88c06-104">Applies to</span><span class="sxs-lookup"><span data-stu-id="88c06-104">Applies to</span></span>**

-  <span data-ttu-id="88c06-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="88c06-105">Partner Center</span></span>
-  <span data-ttu-id="88c06-106">Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="88c06-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="88c06-107">Partner Center for Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="88c06-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="88c06-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span><span class="sxs-lookup"><span data-stu-id="88c06-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="88c06-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span><span class="sxs-lookup"><span data-stu-id="88c06-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="88c06-110">Use these instructions to consolidate tenants for different country/regions.</span><span class="sxs-lookup"><span data-stu-id="88c06-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="88c06-111">**참고** 고객이 전환 계정에서 프로비전한 모든 구독 및 실제 사용자 수를 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="88c06-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span><span class="sxs-lookup"><span data-stu-id="88c06-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="88c06-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span><span class="sxs-lookup"><span data-stu-id="88c06-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="88c06-114">Partners choose to consolidate their tenants.</span><span class="sxs-lookup"><span data-stu-id="88c06-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="88c06-115">Once consolidation is complete, Partners cannot revert to their previous state.</span><span class="sxs-lookup"><span data-stu-id="88c06-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="88c06-116">Note that customer action is also be required.</span><span class="sxs-lookup"><span data-stu-id="88c06-116">Note that customer action is also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="88c06-117">Prepare for migration</span><span class="sxs-lookup"><span data-stu-id="88c06-117">Prepare for migration</span></span>


-   <span data-ttu-id="88c06-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span><span class="sxs-lookup"><span data-stu-id="88c06-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="88c06-120">Migrate customer accounts</span><span class="sxs-lookup"><span data-stu-id="88c06-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="88c06-121">전환(새) 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 파트너 센터 대시보드에서 고객 목록으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-121">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="88c06-122">Select Customer.</span><span class="sxs-lookup"><span data-stu-id="88c06-122">Select Customer.</span></span>

3.  <span data-ttu-id="88c06-123">**재판매인 관계 요청**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="88c06-124">You are presented with a default email message to present to your customers.</span><span class="sxs-lookup"><span data-stu-id="88c06-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="88c06-125">This message contains a URL with the org ID unique to your new Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="88c06-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="88c06-126">**고객 작업:** 마이그레이션할 각 활성 고객이 이 URL을 방문하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="88c06-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span><span class="sxs-lookup"><span data-stu-id="88c06-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="88c06-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span><span class="sxs-lookup"><span data-stu-id="88c06-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="88c06-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span><span class="sxs-lookup"><span data-stu-id="88c06-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="88c06-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span><span class="sxs-lookup"><span data-stu-id="88c06-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="88c06-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span><span class="sxs-lookup"><span data-stu-id="88c06-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="88c06-132">Migrating Office 365 and non-Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="88c06-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="88c06-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span><span class="sxs-lookup"><span data-stu-id="88c06-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="88c06-134">파트너 센터 대시보드의 왼쪽 탐색에서 **고객**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-134">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="88c06-135">Open the company name for the customer you want to migrate.</span><span class="sxs-lookup"><span data-stu-id="88c06-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="88c06-136">**구독 추가**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="88c06-137">Add the correct subscriptions and seat counts from the catalog.</span><span class="sxs-lookup"><span data-stu-id="88c06-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="88c06-138">**전환 원본** 파트너 계정에 제공된 정보로 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  <span data-ttu-id="88c06-140">**제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-140">Click **Submit.**</span></span>

<span data-ttu-id="88c06-141">이제 서비스가 **전환 대상** 파트너 계정의 고객에게 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="88c06-142">Repeat these steps to migrate subscriptions for all additional customers.</span><span class="sxs-lookup"><span data-stu-id="88c06-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="88c06-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span><span class="sxs-lookup"><span data-stu-id="88c06-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="88c06-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="88c06-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="88c06-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span><span class="sxs-lookup"><span data-stu-id="88c06-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="88c06-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span><span class="sxs-lookup"><span data-stu-id="88c06-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="88c06-147">**전환 원본** 파트너 계정에서 CSP 구독을 사용하지 않도록 설정하면 이후 청구가 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="88c06-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span><span class="sxs-lookup"><span data-stu-id="88c06-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="88c06-149">**전환 원본** CSP 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 고객 목록으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-149">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="88c06-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span><span class="sxs-lookup"><span data-stu-id="88c06-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="88c06-151">구독을 **일시 중단됨**으로 설정한 다음 **제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="88c06-152">**참고** 구독을 일시 중단하면 이중 청구가 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-152">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="88c06-153">구독이 구독 목록에서 **일시 중단됨**으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="88c06-154">Repeat these steps for all subscriptions under the customer.</span><span class="sxs-lookup"><span data-stu-id="88c06-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="88c06-155">모든 구독이 **일시 중단됨**으로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="88c06-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span><span class="sxs-lookup"><span data-stu-id="88c06-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="88c06-157">Migrating Azure usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="88c06-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="88c06-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span><span class="sxs-lookup"><span data-stu-id="88c06-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="88c06-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span><span class="sxs-lookup"><span data-stu-id="88c06-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="88c06-160">There will be no disruption of service to the customer during this transition.</span><span class="sxs-lookup"><span data-stu-id="88c06-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="88c06-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span><span class="sxs-lookup"><span data-stu-id="88c06-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="88c06-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span><span class="sxs-lookup"><span data-stu-id="88c06-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="88c06-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span><span class="sxs-lookup"><span data-stu-id="88c06-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="88c06-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="88c06-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="88c06-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span><span class="sxs-lookup"><span data-stu-id="88c06-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="88c06-166">**참고** 고객의 구독을 사용하지 않도록 설정해도 고객 목록에서 고객의 모양이 변경되지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-166">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="88c06-167">There is currently no option to remove customers from the list.</span><span class="sxs-lookup"><span data-stu-id="88c06-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="88c06-168">파트너는 나중에 **전환 원본** 계정에서 이러한 고객에 구독을 다시 추가하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="88c06-169">모든 고객의 모든 구독에 대해 이러한 단계를 반복하여 이후 **전환 원본** 계정에 요금이 청구되지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="88c06-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span><span class="sxs-lookup"><span data-stu-id="88c06-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="88c06-171">No future invoices will generate after that final billing period.</span><span class="sxs-lookup"><span data-stu-id="88c06-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="88c06-172">Notes</span><span class="sxs-lookup"><span data-stu-id="88c06-172">Notes</span></span>

-   <span data-ttu-id="88c06-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span><span class="sxs-lookup"><span data-stu-id="88c06-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="88c06-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span><span class="sxs-lookup"><span data-stu-id="88c06-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="88c06-175">There is currently no way to remove a customer from the Customers list completely.</span><span class="sxs-lookup"><span data-stu-id="88c06-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="88c06-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span><span class="sxs-lookup"><span data-stu-id="88c06-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="88c06-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span><span class="sxs-lookup"><span data-stu-id="88c06-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="88c06-178">Simplify migration using Export</span><span class="sxs-lookup"><span data-stu-id="88c06-178">Simplify migration using Export</span></span>

<span data-ttu-id="88c06-179">**내보내기 기능**을 사용하여 새 통합 구조에서 사용해야 하는 구독을 캡처할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="88c06-180">대시보드에서 **고객**을 클릭하여 기존 구조에서 고객 목록을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-180">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="88c06-181">Open the desired customer name.</span><span class="sxs-lookup"><span data-stu-id="88c06-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="88c06-182">**구독** 페이지에서 **구독 내보내기**를 클릭하여 구독 세부 정보를 Excel 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="88c06-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span><span class="sxs-lookup"><span data-stu-id="88c06-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="88c06-184">API registration</span><span class="sxs-lookup"><span data-stu-id="88c06-184">API registration</span></span>

<span data-ttu-id="88c06-185">API 등록에 대한 자세한 내용은 [이 페이지를 참조](https://go.microsoft.com/fwlink/?linkid=847990)하세요.</span><span class="sxs-lookup"><span data-stu-id="88c06-185">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="88c06-186">Partner Center Activity log</span><span class="sxs-lookup"><span data-stu-id="88c06-186">Partner Center Activity log</span></span>


<span data-ttu-id="88c06-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span><span class="sxs-lookup"><span data-stu-id="88c06-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="88c06-188">This helps partners track changes on a customer tenant.</span><span class="sxs-lookup"><span data-stu-id="88c06-188">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="88c06-189">View the Activity log</span><span class="sxs-lookup"><span data-stu-id="88c06-189">View the Activity log</span></span>**

1.  <span data-ttu-id="88c06-190">파트너 센터 대시보드에서 **활동 로그** 링크를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-190">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="88c06-191">**활동 로그** 페이지에서 고객 계정에 수행된 변경 내용을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-191">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="88c06-192">날짜를 기준으로 활동 로그를 필터링하려면 **시작일** 및 **종료일**을 선택하여 로그에서 선택되는 레코드 범위를 좁힙니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-192">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="88c06-193">**활동 로그**에서 고객을 기준으로 필터링하려면 검색 상자를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-193">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="88c06-194">Export the Activity log</span><span class="sxs-lookup"><span data-stu-id="88c06-194">Export the Activity log</span></span>**

-   <span data-ttu-id="88c06-195">**로그 내보내기**를 클릭하여 활동 로그 데이터를 CSV 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="88c06-195">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="88c06-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span><span class="sxs-lookup"><span data-stu-id="88c06-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



