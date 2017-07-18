---
title: "CSP 지역 권한 설정 테넌트 통합 | 파트너 센터"
description: "다양한 국가/지역에 대한 테넌트를 통합하려면 다음 지침을 사용하세요."
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: fe08fcfbb555b4913fa747d538abf08a18658e09
ms.sourcegitcommit: 0b00306bfb0b406e64ad857cb360de4533740e6a
ms.translationtype: HT
ms.contentlocale: ko-KR
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="4324c-103">CSP 지역 권한 설정 테넌트 통합</span><span class="sxs-lookup"><span data-stu-id="4324c-103">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="4324c-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="4324c-104">Applies to</span></span>**

-  <span data-ttu-id="4324c-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4324c-105">Partner Center</span></span>
-  <span data-ttu-id="4324c-106">미국 정부용 Microsoft 클라우드 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4324c-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="4324c-107">Microsoft 클라우드 독일 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4324c-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="4324c-108">\[일부 정보는 상업용으로 출시되기 전에 상당 부분 수정될 수 있는 시험판 제품과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="4324c-109">Microsoft는 여기에 제공된 정보에 대해 명시적 또는 묵시적 보증을 하지 않습니다.\]</span><span class="sxs-lookup"><span data-stu-id="4324c-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="4324c-110">다양한 국가/지역에 대한 테넌트를 통합하려면 다음 지침을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="4324c-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="4324c-111">**참고** 고객이 전환 계정에서 프로비전한 모든 구독 및 실제 사용자 수를 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="4324c-112">파트너는 마이그레이션 프로세스의 일부로 새 중앙 CSP 계정에서 같은 실제 사용자 수가 포함된 정확히 같은 구독을 다시 프로비전합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-112">Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="4324c-113">목록 내보내기 기능을 사용하여 중앙 집중식 테넌트로 이동할 고객의 목록을 만드세요.</span><span class="sxs-lookup"><span data-stu-id="4324c-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="4324c-114">파트너가 테넌트를 통합하도록 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="4324c-115">통합이 완료되면 파트너는 이전 상태로 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="4324c-116">고객 작업도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-116">Note that customer action is also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="4324c-117">마이그레이션 준비</span><span class="sxs-lookup"><span data-stu-id="4324c-117">Prepare for migration</span></span>


-   <span data-ttu-id="4324c-118">전환(기존) 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 모든 고객 및 해당 고객에 대해 프로비전된 모든 서비스를 기록해 둡니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![지역 고객 목록](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="4324c-120">고객 계정 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="4324c-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="4324c-121">전환(새) 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 파트너 센터 대시보드에서 고객 목록으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-121">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="4324c-122">고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-122">Select Customer.</span></span>

3.  <span data-ttu-id="4324c-123">**재판매인 관계 요청**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="4324c-124">고객에게 제공할 기본 메일 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="4324c-125">이 메시지는 새 파트너 센터 계정에 고유한 조직 ID가 포함된 URL을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="4324c-126">**고객 작업:** 마이그레이션할 각 활성 고객이 이 URL을 방문하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="4324c-127">URL을 열면 고객에게 Office 365 포털에 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="4324c-128">고객은 Azure 및 Office 365 관리 포털에 액세스하는 데 사용하는 것과 같은 조직 ID를 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="4324c-129">로그인한 후 고객 계정의 전역 관리자에게 새 CSP 계정에 위임된 관리 권한을 부여하는 것에 대한 동의를 제출하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="4324c-130">동의하는 경우 고객은 확인란을 선택하고 관계에 권한을 부여하는 것에 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="4324c-131">고객이 동의를 제출하고 나면 고객이 하나씩 파트너의 고객 목록에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="4324c-132">Office 365 및 비 Azure 사용량 기준 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="4324c-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="4324c-133">고객이 계약에 서명하고 나면, 중앙 집중식 파트너 테넌트에서 해당 구독을 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="4324c-134">파트너 센터 대시보드의 왼쪽 탐색에서 **고객**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-134">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="4324c-135">마이그레이션할 고객의 회사 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="4324c-136">**구독 추가**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="4324c-137">카탈로그에서 올바른 구독 및 실제 사용자 수를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="4324c-138">**전환 원본** 파트너 계정에 제공된 정보로 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![고객 목록의 스크린샷](images/regionalcustomer2.png)

6.  <span data-ttu-id="4324c-140">**제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-140">Click **Submit.**</span></span>

<span data-ttu-id="4324c-141">이제 서비스가 **전환 대상** 파트너 계정의 고객에게 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="4324c-142">모든 추가 고객에 대해 구독을 마이그레이션하려면 이러한 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="4324c-143">다음 섹션을 계속하기 전에 **전환 원본** 파트너 계정 아래에 있는 모든 고객 구독이 **전환 대상** 파트너 계정 아래에 다시 프로비전되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="4324c-144">**참고** 파트너는 파트너 센터에서 **전환 대상** 파트너 테넌트 계정 아래에 구독이 전환 및 설정되는 날과 같은 날에 파트너 센터의 **전환 원본** 파트너 테넌트 계정에서 해당 구독을 일시 중단하여 이중 청구가 발생하지 않도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="4324c-145">**전환 원본** 구독을 사용 안 함으로 올바르게 설정하지 않아 발생하는 청구의 겹침으로 인해 크레딧에 대한 지원 요청이 거부됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="4324c-146">전환 원본 파트너 계정에서 Office 365 구독을 사용하지 않도록 설정</span><span class="sxs-lookup"><span data-stu-id="4324c-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="4324c-147">**전환 원본** 파트너 계정에서 CSP 구독을 사용하지 않도록 설정하면 이후 청구가 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="4324c-148">Azure 구독은 마이그레이션 프로세스 동안 자동으로 사용하지 않도록 설정되므로 수동으로 Azure 구독을 사용하지 않도록 설정할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="4324c-149">**전환 원본** CSP 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 고객 목록으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-149">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="4324c-150">사용하지 않도록 설정할 구독이 포함된 고객을 연 다음 사용하지 않도록 설정할 첫 번째 제품을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="4324c-151">구독을 **일시 중단됨**으로 설정한 다음 **제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="4324c-152">**참고** 구독을 일시 중단하면 이중 청구가 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-152">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="4324c-153">구독이 구독 목록에서 **일시 중단됨**으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="4324c-154">고객의 모든 구독에 대해 이러한 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="4324c-155">모든 구독이 **일시 중단됨**으로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="4324c-156">목록에서 다음 고객을 선택하고 모든 구독을 사용하지 않도록 설정하는 프로세스를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="4324c-157">Azure 사용량 기준 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="4324c-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="4324c-158">Office 365 CSP 구독의 경우와 마찬가지로 Azure 사용량 기준 CSP 구독은 수동으로 마이그레이션할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="4324c-159">Microsoft Azure 지원에서는 **전환 원본** CSP 재판매인 계정의 모든 배포된 서비스 또는 리소스뿐만 아니라 Azure 구독을 **전환 대상** CSP 재판매인 계정으로 마이그레이션할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="4324c-160">이 전환 동안 고객에게 서비스 중단이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="4324c-161">Azure 구독을 마이그레이션해야 하는 고객 계정이 새 **전환 대상** CSP 계정과 연결하기 위한 계약에 동의했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="4324c-162">파트너는 Microsoft에 Azure 구독을 마이그레이션할 준비가 된 고객 계정을 알리고 해당 고객의 회사 이름을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="4324c-163">Microsoft는 Azure 사용량 기준 구독을 마이그레이션하고 마이그레이션이 완료되면 파트너에게 알립니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="4324c-164">파트너는 **전환 원본** CSP 재판매인 계정의 Azure 구독이 이제 파트너 센터의 고객 구독 섹션에서 일시 중단됨으로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="4324c-165">파트너는 **전환 대상** CSP 재판매인 계정의 Azure 구독이 이제 파트너 센터의 고객 구독 섹션에서 **활성** 상태로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="4324c-166">**참고** 고객의 구독을 사용하지 않도록 설정해도 고객 목록에서 고객의 모양이 변경되지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-166">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="4324c-167">현재 목록에서 고객을 제거하는 옵션은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="4324c-168">파트너는 나중에 **전환 원본** 계정에서 이러한 고객에 구독을 다시 추가하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="4324c-169">모든 고객의 모든 구독에 대해 이러한 단계를 반복하여 이후 **전환 원본** 계정에 요금이 청구되지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="4324c-170">파트너는 취소일과 청구 기간의 마지막 날 사이에 사용되지 않은 일수에 대한 크레딧이 포함된 최종 송장을 하나 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="4324c-171">해당 최종 청구 기간 이후 더는 송장이 생성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="4324c-172">참고</span><span class="sxs-lookup"><span data-stu-id="4324c-172">Notes</span></span>

-   <span data-ttu-id="4324c-173">**전환 원본** CSP 계정의 구독을 사용하지 않도록 설정해도, 이렇게 사용하지 않도록 설정하기 전에 서비스가 **전환 대상** CSP 계정에서 프로비전된 경우 최종 고객의 서비스에는 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="4324c-174">고객은 구독을 사용할 수 없으며 구독이 일시 중단되거나 취소된 경우 청구 요금이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="4324c-175">현재 고객 목록에서 고객을 완전히 제거하는 방법은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="4324c-176">**참고** 파트너는 파트너 센터에서 **전환 대상** 파트너 테넌트 계정 아래에 구독이 전환 및 설정되는 날과 같은 날에 파트너 센터의 **전환 원본** 파트너 테넌트 계정에서 해당 구독을 일시 중단하여 이중 청구가 발생하지 않도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="4324c-177">Microsoft는 **전환 원본** 구독을 일시 중단됨으로 올바르게 설정하지 않아 발생하는 청구의 겹침으로 인한 크레딧에 대한 요청은 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="4324c-178">내보내기를 사용하여 마이그레이션 간소화</span><span class="sxs-lookup"><span data-stu-id="4324c-178">Simplify migration using Export</span></span>

<span data-ttu-id="4324c-179">**내보내기 기능**을 사용하여 새 통합 구조에서 사용해야 하는 구독을 캡처할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="4324c-180">대시보드에서 **고객**을 클릭하여 기존 구조에서 고객 목록을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-180">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="4324c-181">원하는 고객 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="4324c-182">**구독** 페이지에서 **구독 내보내기**를 클릭하여 구독 세부 정보를 Excel 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="4324c-183">이 목록을 사용하여 새 통합 테넌트에서 구독을 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="4324c-184">API 등록</span><span class="sxs-lookup"><span data-stu-id="4324c-184">API registration</span></span>

<span data-ttu-id="4324c-185">API 등록에 대한 자세한 내용은 [이 페이지를 참조](https://msdn.microsoft.com/en-us/library/partnercenter/mt267552.aspx)하세요.</span><span class="sxs-lookup"><span data-stu-id="4324c-185">For more information about API registration, [see this page](https://msdn.microsoft.com/en-us/library/partnercenter/mt267552.aspx).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="4324c-186">파트너 센터 활동 로그</span><span class="sxs-lookup"><span data-stu-id="4324c-186">Partner Center Activity log</span></span>


<span data-ttu-id="4324c-187">활동 로그를 사용하여 파트너는 해당 테넌트에서 수행된, 고객에게 영향을 미치는 모든 변경 내용 레코드를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="4324c-188">이 기능을 통해 파트너는 고객 테넌트의 변경 내용을 추적할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-188">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="4324c-189">활동 로그 보기</span><span class="sxs-lookup"><span data-stu-id="4324c-189">View the Activity log</span></span>**

1.  <span data-ttu-id="4324c-190">파트너 센터 대시보드에서 **활동 로그** 링크를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-190">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="4324c-191">**활동 로그** 페이지에서 고객 계정에 수행된 변경 내용을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-191">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="4324c-192">날짜를 기준으로 활동 로그를 필터링하려면 **시작일** 및 **종료일**을 선택하여 로그에서 선택되는 레코드 범위를 좁힙니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-192">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="4324c-193">**활동 로그**에서 고객을 기준으로 필터링하려면 검색 상자를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-193">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="4324c-194">활동 로그 내보내기</span><span class="sxs-lookup"><span data-stu-id="4324c-194">Export the Activity log</span></span>**

-   <span data-ttu-id="4324c-195">**로그 내보내기**를 클릭하여 활동 로그 데이터를 CSV 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="4324c-195">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="4324c-196">고객 목록 및 단일 고객의 구독 목록을 내보낼 수도 있습니다(고객의 구독 페이지에서).</span><span class="sxs-lookup"><span data-stu-id="4324c-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



