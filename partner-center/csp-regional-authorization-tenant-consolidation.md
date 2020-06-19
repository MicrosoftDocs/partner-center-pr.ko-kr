---
title: CSP 지역 권한 부여 테 넌 트 통합
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이러한 지침을 사용 하 여 다른 국가/지역에 대 한 테 넌 트를 통합할 수 있습니다. 여기에는 고객 계정 및 고객 구독을 마이그레이션하는 단계가 포함 됩니다.
author: LauraBrenner
ms.author: labrenne
keywords: 고객 마이그레이션, 프로 비전 및 테 넌 트 계정, 테 넌 트 통합
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2e3c0bd9b50e91e02952a690cc7cbfe1601ad550
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991471"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="fa416-105">CSP 지역 권한 부여 테넌트 통합에 대한 지침</span><span class="sxs-lookup"><span data-stu-id="fa416-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="fa416-106">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="fa416-106">**Applies to**</span></span>

-  <span data-ttu-id="fa416-107">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="fa416-107">Partner Center</span></span>
-  <span data-ttu-id="fa416-108">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="fa416-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="fa416-109">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="fa416-109">**Appropriate roles**</span></span>

- <span data-ttu-id="fa416-110">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="fa416-110">Global admin</span></span>
- <span data-ttu-id="fa416-111">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="fa416-111">Admin agent</span></span>

<span data-ttu-id="fa416-112">\[일부 정보는 상업적으로 출시 되기 전에 대폭 수정 될 수 있는 미리 릴리스된 제품과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="fa416-113">Microsoft는 여기에 제공된 정보와 관련하여 명시적이거나 묵시적인 어떤 보증도 하지 않습니다.\]</span><span class="sxs-lookup"><span data-stu-id="fa416-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="fa416-114">이러한 지침을 사용 하 여 다른 국가/지역에 대 한 테 넌 트를 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="fa416-115">전환 계정에서 프로 비전 된 고객의 모든 구독 및 사용자 수를 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-115">You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="fa416-116">마이그레이션 프로세스의 일부로 새 중앙 CSP 계정에서 동일한 사용자 수를 사용 하 여 동일한 정확한 구독을 다시 프로 비전 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="fa416-117">목록 내보내기 기능을 사용 하 여 중앙 테 넌 트로 이동 하는 고객의 목록을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="fa416-118">파트너 테 넌 트 통합을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="fa416-119">통합이 완료 되 면 파트너는 이전 상태로 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="fa416-120">고객 동작도 필요할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-120">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="fa416-121">마이그레이션 준비</span><span class="sxs-lookup"><span data-stu-id="fa416-121">Prepare for migration</span></span>

- <span data-ttu-id="fa416-122">**전환 (기존** ) 계정 (기존 계정)을 사용 하 여 **파트너 센터** 에 로그인 하 고 해당 고객에 대해 프로 비전 된 모든 고객 및 모든 서비스를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-122">Sign in to **Partner Center**  with the **Transitioning** (existing) account (the one you will transition) and review of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="지역별 고객 목록":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="fa416-124">고객 계정 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="fa416-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="fa416-125">**전환 (신규** ) 계정 (전환 하려는 계정)을 사용 하 여 **파트너 센터** 에 로그인 하 고 **고객**목록으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="fa416-126">고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-126">Select Customers.</span></span>

3. <span data-ttu-id="fa416-127">**대리점 관계 요청을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="fa416-128">고객에 게 제공 되는 기본 전자 메일 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="fa416-129">이 메시지에는 새 파트너 센터 계정에 고유한 조직 ID를 포함 하는 URL이 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="fa416-130">**고객 작업:** 마이그레이션하려는 각 활성 고객이이 URL을 방문 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="fa416-131">URL을 열면 고객에게 Office 365 포털에 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="fa416-132">고객은 Azure 및 Office 365 관리 포털에 액세스 하는 데 사용 하는 것과 동일한 조직 ID를 사용 하 여 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="fa416-133">로그인 한 후 고객 계정에 대 한 전역 관리자에 게 새 CSP 계정에 위임 된 관리자 권한을 부여 하는 규약을 전송 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="fa416-134">동의 하면 고객이 확인란을 선택 하 고 관계에 대 한 권한을 부여 하는 데 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="fa416-135">고객은 계약을 제출한 후 파트너의 고객 목록에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="fa416-136">Office 365 및 비 Azure 사용 기반 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="fa416-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="fa416-137">고객이 규약에 서명 하면 중앙 파트너 테 넌 트에서 구독을 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="fa416-138">**파트너 센터** 에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-138">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="fa416-139">마이그레이션하려는 고객의 회사 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="fa416-140">**구독 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-140">Select **Add subscription**.</span></span>

5. <span data-ttu-id="fa416-141">카탈로그에서 올바른 구독과 좌석 수를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="fa416-142">파트너 계정 **에서 전환** 에 제공 된 정보를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="고객 목록":::

6. <span data-ttu-id="fa416-144">**제출을 클릭 합니다.**</span><span class="sxs-lookup"><span data-stu-id="fa416-144">Click **Submit.**</span></span>

   <span data-ttu-id="fa416-145">이제 서비스는 파트너 계정 **으로 전환** 하 여 고객에 게 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="fa416-146">이러한 단계를 반복 하 여 모든 추가 고객에 대 한 구독을 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="fa416-147">다음 섹션으로 진행 하기 전에 파트너 계정으로 **전환** 하는 동안 기존 모든 고객 구독이 파트너 계정 **으로 전환** 하 여 다시 프로 비전 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="fa416-148">파트너는 파트너 센터의 파트너 테 넌 트 계정 **전환** 에 대 한 구독을 일시 중단 해야 합니다 .이는 파트너 센터의 파트너 테 넌 트 계정 **으로 전환** 하 여 이중 청구가 발생 하지 않도록 하는 것과 동일 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="fa416-149">구독에서 사용 안 함으로의 **전환을** 올바르게 설정 하지 않아 발생 하는 청구의 겹치는 부분으로 인해 크레딧에 대 한 지원 요청이 거부 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="fa416-150">파트너 계정에서 전환 하는 경우 Office 365 구독을 사용 하지 않도록 설정</span><span class="sxs-lookup"><span data-stu-id="fa416-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="fa416-151">파트너 계정 **에서 전환** 하는 동안 CSP 구독을 사용 하지 않도록 설정 하면 이후 청구도 중지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="fa416-152">Azure 구독은 마이그레이션 프로세스 중에 자동으로 사용 하지 않도록 설정 되므로 Azure 구독을 수동으로 사용 하지 않도록 설정할 필요는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="fa416-153">CSP 계정 **에서 전환** 하 여 **파트너 센터** 에 로그인 하 고 고객 목록으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="fa416-154">사용 하지 않도록 설정 하려는 구독을 사용 하 여 고객을 열고 비활성화할 첫 번째 제품을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="fa416-155">구독을 **일시 중단 됨**으로 설정 하 고 **제출**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="fa416-156">구독을 일시 중단 하면 이중 청구가 발생 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="fa416-157">구독 목록에서 구독이 **일시 중단** 된 상태로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="fa416-158">고객의 모든 구독에 대해 이러한 단계를 반복 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="fa416-159">모든 show **suspended를 확인 합니다.**</span><span class="sxs-lookup"><span data-stu-id="fa416-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="fa416-160">목록에서 다음 고객을 선택 하 고 모든 구독을 사용 하지 않도록 설정 하는 프로세스를 반복 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="fa416-161">Azure 사용량 기반 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="fa416-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="fa416-162">Azure, 사용 기반 CSP 구독은 Office 365 CSP 구독을 사용 하는 경우와 마찬가지로 수동으로 마이그레이션할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="fa416-163">Microsoft Azure 지원을 통해 csp 재판매인 계정에서 **csp 재판매인 계정으로 전환 하** 는 것으로 **전환** 될 때까지 Azure 구독 및 배포 된 모든 서비스 또는 리소스를 마이그레이션할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="fa416-164">이 전환 중에는 고객에 게 서비스가 중단 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="fa416-165">Azure 구독을 마이그레이션해야 하는 고객 계정에 새 **전환** CSP 계정에 연결할 수 있는 계약을 수락 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="fa416-166">파트너는 Azure 구독을 보유 하 고 있는 고객 계정에 대해 Microsoft에 알리고 해당 고객의 회사 이름을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="fa416-167">Microsoft는 Azure 사용량 기반 구독을 마이그레이션하고 마이그레이션이 완료 되 면 파트너에 게 알립니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="fa416-168">파트너는 이제 CSP 재판매인 계정 **에서 전환** 중인 Azure 구독이 고객 구독 섹션의 파트너 센터에서 일시 중단 됨으로 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="fa416-169">파트너는 이제 CSP 재판매인 계정 **으로 전환** 중인 Azure 구독이 고객 구독 섹션의 파트너 센터에서 **활성** 상태를 표시 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="fa416-170">고객에서 구독을 사용 하지 않도록 설정 해도 고객 목록에 있는 고객의 모양은 변경 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="fa416-171">현재 목록에서 고객을 제거 하는 옵션은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="fa416-172">파트너는 나중에 계정을 **전환** 하 여 해당 고객에 게 다시 구독을 추가 하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="fa416-173">모든 고객의 모든 구독에 대해 이러한 단계를 반복 하 여 계정 **전환** 에 대 한 향후 요금을 중지 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="fa416-174">파트너는 취소 날짜와 청구 기간의 마지막 날 사이에 사용 되지 않은 일 수에 대 한 크레딧이 있는 최종 송장을 하나씩 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="fa416-175">최종 청구 기간이 끝난 후에는 이후 송장이 생성 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-175">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="fa416-176">추가 정보</span><span class="sxs-lookup"><span data-stu-id="fa416-176">Additional information</span></span>

- <span data-ttu-id="fa416-177">구독을 사용 하지 않도록 설정 하기 전에 csp 계정 **에서** 구독을 사용 하지 않도록 설정 하는 것은 서비스를 Csp 계정 **으로 전환** 하는 동안 최종 고객의 서비스에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="fa416-178">고객은 구독을 사용할 수 없으며 일시 중단 또는 취소 시에는 요금이 생성 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="fa416-179">현재 고객 목록에서 고객을 완전히 제거할 수 있는 방법은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

    >[!Note]
    > <span data-ttu-id="fa416-180">파트너는 파트너 센터 **의 파트너 테** 넌 트 계정 전환에 대 한 구독을 일시 중단 하 고 파트너 센터의 파트너 테 넌 트 계정 **으로 전환** 하 여 이중 청구가 발생 하지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="fa416-181">Microsoft는 구독에서 일시 중단으로의 **전환을** 올바르게 설정 하지 않아 발생 하는 청구의 겹치는 부분으로 인해 크레딧 요청을 지원 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="fa416-182">내보내기를 사용 하 여 마이그레이션 간소화</span><span class="sxs-lookup"><span data-stu-id="fa416-182">Simplify migration using Export</span></span>

<span data-ttu-id="fa416-183">**Export 함수**를 사용 하 여 새 통합 구조에서 사용 해야 하는 구독을 캡처할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="fa416-184">파트너 센터에서 **고객** 을 클릭 하 여 기존 구조에 있는 고객 목록을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="fa416-185">원하는 고객 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="fa416-186">**구독 페이지에서** 구독 **내보내기** 를 클릭 하 여 구독 정보를 Excel 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="fa416-187">이 목록을 사용 하 여 새 통합 된 테 넌 트에 구독을 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fa416-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="fa416-188">API 등록</span><span class="sxs-lookup"><span data-stu-id="fa416-188">API registration</span></span>

<span data-ttu-id="fa416-189">API 등록에 대 한 자세한 내용은 [파트너 센터에서 api 액세스 설정](https://go.microsoft.com/fwlink/?linkid=847990)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="fa416-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
