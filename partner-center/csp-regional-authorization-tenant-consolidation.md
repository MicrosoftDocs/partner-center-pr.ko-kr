---
title: CSP 지역 권한 부여 테 넌 트 통합
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이러한 지침을 사용 하 여 다른 국가/지역에 대 한 테 넌 트를 통합할 수 있습니다. 여기에는 고객 계정 및 고객 구독을 마이그레이션하는 단계가 포함 됩니다.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147584"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="307a4-104">CSP 지역 권한 부여 테넌트 통합에 대한 지침</span><span class="sxs-lookup"><span data-stu-id="307a4-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="307a4-105">**적용 대상**: 파트너 센터 | 미국 정부에 대 한 파트너 센터 Microsoft 클라우드</span><span class="sxs-lookup"><span data-stu-id="307a4-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="307a4-106">**적절 한 역할**: 전역 관리자 | 관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="307a4-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="307a4-107">\[일부 정보는 상업적으로 출시 되기 전에 대폭 수정 될 수 있는 미리 릴리스된 제품과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="307a4-108">Microsoft는 여기에 제공된 정보에 대해 어떠한 명시적이거나 묵시적인 보증도 하지 않습니다.\]</span><span class="sxs-lookup"><span data-stu-id="307a4-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="307a4-109">비즈니스에 대 한 테 넌 트를 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="307a4-110">이러한 지침을 사용 하 여 다른 국가/지역에 대 한 테 넌 트를 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="307a4-111">전환 하려는 계정에서 각 고객의 프로 비전 된 구독 및 라이선스 수를 모두 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="307a4-112">마이그레이션 프로세스의 일부로 새 중앙 CSP 계정의 라이선스 수가 동일한 동일한 정확한 구독을 다시 프로 비전 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="307a4-113">목록 내보내기 기능을 사용 하 여 중앙 테 넌 트로 이동 하는 고객의 목록을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="307a4-114">통합이 완료 되 면 이전 테 넌 트 상태로 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="307a4-115">고객 동작도 필요할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="307a4-116">마이그레이션 준비</span><span class="sxs-lookup"><span data-stu-id="307a4-116">Prepare for migration</span></span>

- <span data-ttu-id="307a4-117">**전환** 계정 (새 계정으로 전환 하는 계정)을 사용 하 여 **파트너 센터** 에 로그인 하 고 해당 고객에 대해 프로 비전 된 모든 고객 및 모든 서비스를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="307a4-118">이 계정에서 로그 아웃 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="307a4-119">고객 계정 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="307a4-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="307a4-120">**전환** (신규) 계정 (고객을 전환 하는 계정)으로 **파트너 센터** 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="307a4-121">**고객** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-121">Select **Customers**.</span></span>

3. <span data-ttu-id="307a4-122">**대리점 관계 요청을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="307a4-123">고객에 게 보낼 기본 전자 메일 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="307a4-124">이 메시지에는 새 파트너 센터 계정에 고유한 조직 ID를 포함 하는 URL이 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="307a4-125">**고객 작업:** 마이그레이션하려는 각 활성 고객이 이 URL을 방문하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="307a4-126">URL을 열면 고객에게 Office 365 포털에 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="307a4-127">고객은 Azure 및 Office 365 관리 포털에 액세스하는 데 사용하는 것과 동일한 조직 ID를 사용하여 서명합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="307a4-128">로그인하면 **고객 계정의** 전역 관리자에게 위임된 관리자 권한을 새 CSP 계정에 부여하는 계약을 제출하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="307a4-129">동의하면 고객은 확인란을 선택하고 관계에 대한 권한을 부여하는 데 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="307a4-130">고객이 계약을 제출한 후 하나씩 파트너의 고객 목록에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="307a4-131">Office 365 및 비 Azure 사용량 기반 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="307a4-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="307a4-132">고객이 계약에 서명하면 중앙 집중식 파트너 테넌트에서 구독을 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="307a4-133">**파트너 센터** 에서 **고객을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="307a4-134">마이그레이션하려는 고객의 회사 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="307a4-135">**구독 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="307a4-136">카탈로그에서 올바른 구독 및 라이선스 수를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="307a4-137">파트너 **계정에서 전환에** 제공된 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="고객 목록":::

6. <span data-ttu-id="307a4-139">**제출을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="307a4-139">Select **Submit.**</span></span>

   <span data-ttu-id="307a4-140">이제 파트너 계정으로 **전환에서** 고객에게 서비스가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="307a4-141">이러한 단계를 반복하여 모든 추가 고객에 대한 구독을 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="307a4-142">다음 섹션으로 진행하기 전에 파트너 **계정에서 전환** 아래에 있는 모든 고객 구독이 파트너 계정으로 **전환에서** 다시 프로비전되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="307a4-143">파트너는 이중 청구가  발생하지 않도록 파트너 센터 파트너 테넌트로 전환 계정에서 해당 구독이 전환되고 설정된 날인 파트너 센터 **파트너** 테넌트 계정에서 구독을 일시 중단해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="307a4-144">구독에서 전환을 올바르게 비활성화하지 않아 발생하는 청구 중첩으로 인해 크레딧에 대한 지원 **요청이** 거부됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="307a4-145">파트너 계정에서 전환에서 Office 365 구독 비활성화</span><span class="sxs-lookup"><span data-stu-id="307a4-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="307a4-146">파트너 계정 **에서 전환** 하는 동안 CSP 구독을 사용 하지 않도록 설정 하면 이후 청구도 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="307a4-147">Azure 구독은 마이그레이션 프로세스 중에 자동으로 사용 하지 않도록 설정 되므로 Azure 구독을 수동으로 사용 하지 않도록 설정할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="307a4-148">CSP 계정 **에서 전환** 하 여 **파트너 센터** 에 로그인 하 고 고객 목록으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="307a4-149">사용 하지 않도록 설정 하려는 구독을 사용 하 여 고객을 열고 비활성화할 첫 번째 제품을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="307a4-150">구독을 **일시 중단 됨** 으로 설정 하 고 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="307a4-151">구독을 일시 중단 하면 이중 청구가 발생 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="307a4-152">구독 목록에서 구독이 **일시 중단** 된 상태로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="307a4-153">고객의 모든 구독에 대해 이러한 단계를 반복 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="307a4-154">모든 show **suspended를 확인 합니다.**</span><span class="sxs-lookup"><span data-stu-id="307a4-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="307a4-155">목록에서 다음 고객을 선택 하 고 모든 구독을 사용 하지 않도록 설정 하는 프로세스를 반복 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="307a4-156">Azure 사용량 기반 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="307a4-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="307a4-157">Office 365 CSP 구독과 달리 Azure는 사용 빈도 기반 CSP 구독을 수동으로 마이그레이션할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="307a4-158">Microsoft Azure 지원에서는 Azure 구독 및 모든 배포 된 서비스 또는 리소스를 csp 재판매인 계정 **에서** csp 재판매인 계정 **으로** 전환 하 여 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="307a4-159">이 전환 중에는 고객에 게 서비스가 중단 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="307a4-160">Azure 구독이 마이그레이션되는 고객 계정에 새 **전환** CSP 계정에 연결할 수 있는 계약을 수락 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="307a4-161">Microsoft에서 마이그레이션할 준비가 된 고객 계정을 알리고 해당 고객의 회사 이름을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="307a4-162">Microsoft는 Azure 사용량 기반 구독을 마이그레이션하고 마이그레이션이 완료 되 면 사용자에 게 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="307a4-163">이제 CSP 재판매인 계정 **에서 전환** 중인 Azure 구독이 파트너 센터의 고객 구독 섹션에서 **일시 중단** 됨으로 표시 되어 있는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="307a4-164">CSP로 **전환** 대리점 계정 아래의 Azure 구독에 이제 고객 구독 섹션 아래의 파트너 센터 **활성** 상태가 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="307a4-165">고객에서 구독을 비활성화해도 고객 목록에서 고객의 모양은 변경되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="307a4-166">현재 목록에서 고객을 제거하는 옵션은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="307a4-167">파트너는 나중에 전환 계정에서 이러한 고객에게 **구독을** 다시 추가하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="307a4-168">모든 고객의 모든 구독에 대해 이 단계를 반복하여 **계정에서 전환에서** 향후 요금을 중지합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="307a4-169">파트너는 취소일과 청구 기간의 마지막 날 사이의 사용되지 않은 일 수에 대한 크레딧이 있는 최종 청구서를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="307a4-170">최종 청구 기간 이후에는 향후 청구서가 생성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="307a4-171">추가 정보</span><span class="sxs-lookup"><span data-stu-id="307a4-171">Additional information</span></span>

- <span data-ttu-id="307a4-172">CSP **계정에서 전환 계정에서 구독을** 비활성화해도 구독을 비활성화하기 전에 CSP로 **전환** 계정에서 서비스가 프로비전된 경우 최종 고객의 서비스에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="307a4-173">구독은 고객이 사용할 수 없으며 일시 중단되거나 취소될 때 요금이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="307a4-174">현재 고객 **목록에서** 고객을 완전히 제거할 수 있는 방법은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="307a4-175">파트너는 이중 청구가 발생하지 않도록 해당 구독이 전환되는 날 파트너 센터 파트너 테넌트 **계정에서** 전환 계정에서 **구독을** 일시 중단하고 전환 계정으로 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="307a4-176">Microsoft는 **구독에서 전환** 을 일시 중단으로 올바르게 설정하지 않아 발생하는 청구 중첩으로 인해 크레딧 요청을 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="307a4-177">내보내기를 사용하여 마이그레이션 간소화</span><span class="sxs-lookup"><span data-stu-id="307a4-177">Simplify migration using Export</span></span>

<span data-ttu-id="307a4-178">**내보내기 함수** 를 사용하여 새 통합 구조에서 사용해야 하는 구독을 캡처할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="307a4-179">파트너 센터 **고객을** 선택하여 고객 목록을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="307a4-180">원하는 고객 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="307a4-181">**구독 페이지에서** 구독 **내보내기** 를 선택 하 여 구독 정보를 Excel 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="307a4-182">이 목록을 사용 하 여 새 통합 된 테 넌 트에 구독을 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="307a4-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="307a4-183">API 등록</span><span class="sxs-lookup"><span data-stu-id="307a4-183">API registration</span></span>

<span data-ttu-id="307a4-184">API 등록에 대 한 자세한 내용은 [파트너 센터에서 api 액세스 설정](/partner-center/develop/set-up-api-access-in-partner-center)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="307a4-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="307a4-185">다음 단계</span><span class="sxs-lookup"><span data-stu-id="307a4-185">Next steps</span></span>

- [<span data-ttu-id="307a4-186">CSP 제품을 판매할 수 있는 클라우드 솔루션 공급자 프로그램 지역 시장 및 통화</span><span class="sxs-lookup"><span data-stu-id="307a4-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
