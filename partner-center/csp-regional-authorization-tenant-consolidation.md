---
title: CSP 지역 권한 설정 테넌트 통합 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 다양한 국가/지역에 대한 테넌트를 통합하려면 다음 지침을 사용하세요.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: 고객 마이그레이션, 프로비저닝, 테넌트 계정, 테넌트 통합
ms.localizationpriority: medium
ms.openlocfilehash: 183b5f518a57fdaf27badce5927a2ea09a5ec89c
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587556"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="ebbff-104">CSP 지역 권한 설정 테넌트 통합</span><span class="sxs-lookup"><span data-stu-id="ebbff-104">CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="ebbff-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="ebbff-105">**Applies to**</span></span>

-  <span data-ttu-id="ebbff-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="ebbff-106">Partner Center</span></span>
-  <span data-ttu-id="ebbff-107">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="ebbff-107">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="ebbff-108">\[일부 정보는 정식으로 발표 되기 전에 대폭 수정 될 수 있는 사전 릴리스된 제품과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="ebbff-109">Microsoft는 명시적이 든 여기에 제공 된 정보에 따라 묵시적 보증도 하지 않습니다.\]</span><span class="sxs-lookup"><span data-stu-id="ebbff-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="ebbff-110">다양한 국가/지역에 대한 테넌트를 통합하려면 다음 지침을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="ebbff-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="ebbff-111">**참고** 고객이 전환 계정에서 프로비전한 모든 구독 및 실제 사용자 수를 알고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="ebbff-112">마이그레이션 프로세스의 일부로 새 중앙 CSP 계정에서 같은 실제 사용자 수가 포함된 정확히 같은 구독을 다시 프로비전합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-112">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="ebbff-113">목록 내보내기 기능을 사용하여 중앙 집중식 테넌트로 이동할 고객의 목록을 만드세요.</span><span class="sxs-lookup"><span data-stu-id="ebbff-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="ebbff-114">파트너가 테넌트를 통합하도록 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="ebbff-115">통합이 완료되면 파트너는 이전 상태로 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="ebbff-116">고객 작업도 필요할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-116">Note that customer action may also be required.</span></span>



## <a name="prepare-for-migration"></a><span data-ttu-id="ebbff-117">마이그레이션 준비</span><span class="sxs-lookup"><span data-stu-id="ebbff-117">Prepare for migration</span></span>


-   <span data-ttu-id="ebbff-118">에 로그인 하 여 **파트너 센터** 사용 하 여를 **Transitioning** 모든 고객의 메모 (기존) 계정 (계정 전환 됩니다) 및 수행 및 고객에 대 한 프로 비전 된 모든 서비스.</span><span class="sxs-lookup"><span data-stu-id="ebbff-118">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![지역 고객 목록](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="ebbff-120">고객 계정 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="ebbff-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="ebbff-121">에 로그인 하 여 **파트너 센터** 사용 하 여는 **Transitioning** (으로 전환 하는 하나)를 계정 (신규) 및 고객 목록으로 이동 **고객**.</span><span class="sxs-lookup"><span data-stu-id="ebbff-121">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="ebbff-122">고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-122">Select Customers.</span></span>

3.  <span data-ttu-id="ebbff-123">**재판매인 관계 요청**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="ebbff-124">고객에게 제공할 기본 메일 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="ebbff-125">이 메시지는 새 파트너 센터 계정에 고유한 조직 ID가 포함된 URL을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="ebbff-126">**고객 작업:** 이 URL를 방문할 각 마이그레이션할 활성 고객을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="ebbff-127">URL을 열면 고객에게 Office 365 포털에 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="ebbff-128">고객은 Azure 및 Office 365 관리 포털에 액세스하는 데 사용하는 것과 같은 조직 ID를 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="ebbff-129">로그인한 후 고객 계정의 전역 관리자에게 새 CSP 계정에 위임된 관리 권한을 부여하는 것에 대한 동의를 제출하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="ebbff-130">동의하는 경우 고객은 확인란을 선택하고 관계에 권한을 부여하는 것에 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="ebbff-131">고객이 동의를 제출하고 나면 고객이 하나씩 파트너의 고객 목록에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="ebbff-132">Office 365 및 비 Azure 사용량 기준 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="ebbff-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="ebbff-133">고객이 계약에 서명하고 나면, 중앙 집중식 파트너 테넌트에서 해당 구독을 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="ebbff-134">**파트너 센터** 선택 **고객**합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-134">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="ebbff-135">마이그레이션할 고객의 회사 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="ebbff-136">**구독 추가**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="ebbff-137">카탈로그에서 올바른 구독 및 실제 사용자 수를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="ebbff-138">**Transitioning From**(전환 원본) 파트너 계정에 제공된 정보로 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

![고객 목록](images/regionalcustomer2.png)

6.  <span data-ttu-id="ebbff-140">**제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-140">Click **Submit.**</span></span>

<span data-ttu-id="ebbff-141">이제 서비스가 **Transitioning To**(전환 대상) 파트너 계정의 고객에게 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ebbff-142">모든 추가 고객에 대해 구독을 마이그레이션하려면 이러한 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="ebbff-143">다음 섹션을 계속하기 전에 **전환 원본** 파트너 계정 아래에 있는 모든 고객 구독이 **전환 대상** 파트너 계정 아래에 다시 프로비전되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ebbff-144">**참고** 파트너는 파트너 센터에서 **전환 대상** 파트너 테넌트 계정 아래에 구독이 전환 및 설정되는 날과 같은 날에 파트너 센터의 **전환 원본** 파트너 테넌트 계정에서 해당 구독을 일시 중단하여 이중 청구가 발생하지 않도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ebbff-145">**전환 원본** 구독을 사용 안 함으로 올바르게 설정하지 않아 발생하는 청구의 겹침으로 인해 크레딧에 대한 지원 요청이 거부됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="ebbff-146">전환 원본 파트너 계정에서 Office 365 구독을 사용하지 않도록 설정</span><span class="sxs-lookup"><span data-stu-id="ebbff-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="ebbff-147">**전환 원본** 파트너 계정에서 CSP 구독을 사용하지 않도록 설정하면 이후 청구가 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="ebbff-148">Azure 구독은 마이그레이션 프로세스 동안 자동으로 사용하지 않도록 설정되므로 수동으로 Azure 구독을 사용하지 않도록 설정할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="ebbff-149">에 로그인 합니다 **파트너 센터** 사용 하 여 합니다 **전환에서** CSP 계정 및 고객 목록으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-149">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="ebbff-150">사용하지 않도록 설정할 구독이 포함된 고객을 연 다음 사용하지 않도록 설정할 첫 번째 제품을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="ebbff-151">구독을 **일시 중단됨**으로 설정한 다음 **제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

 >[! **참고**]<span data-ttu-id="ebbff-152"> 요금이 이중으로 청구 없는 하면 구독을 일시 중단 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-152"> Suspending the subscription ensures double billing does not occur.</span></span>



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  <span data-ttu-id="ebbff-153">고객의 모든 구독에 대해 이러한 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="ebbff-154">모든 구독이 **일시 중단됨**으로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-154">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="ebbff-155">목록에서 다음 고객을 선택하고 모든 구독을 사용하지 않도록 설정하는 프로세스를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="ebbff-156">Azure 사용량 기준 구독 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="ebbff-156">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="ebbff-157">Office 365 CSP 구독의 경우와 마찬가지로 Azure 사용량 기준 CSP 구독은 수동으로 마이그레이션할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-157">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="ebbff-158">Microsoft Azure 지원에서는 **Transitioning From**(전환 원본) CSP 재판매인 계정의 모든 배포된 서비스 또는 리소스뿐만 아니라 Azure 구독을 **Transitioning To**(전환 대상) CSP 재판매인 계정으로 마이그레이션할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-158">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="ebbff-159">이 전환 동안 고객에게 서비스 중단이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-159">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="ebbff-160">Azure 구독을 마이그레이션해야 하는 고객 계정이 새 **Transitioning To**(전환 대상) CSP 계정과 연결하기 위한 계약에 동의했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-160">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="ebbff-161">파트너는 Microsoft에 Azure 구독을 마이그레이션할 준비가 된 고객 계정을 알리고 해당 고객의 회사 이름을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-161">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="ebbff-162">Microsoft는 Azure 사용량 기준 구독을 마이그레이션하고 마이그레이션이 완료되면 파트너에게 알립니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-162">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="ebbff-163">파트너는 **Transitioning From**(전환 원본) CSP 재판매인 계정의 Azure 구독이 이제 파트너 센터의 고객 구독 섹션에서 일시 중단됨으로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-163">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="ebbff-164">파트너는 **Transitioning To**(전환 대상) CSP 재판매인 계정의 Azure 구독이 이제 파트너 센터의 고객 구독 섹션에서 **활성** 상태로 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-164">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

>[! **참고**]<span data-ttu-id="ebbff-165"> 고객 구독을 사용 하지 않도록 설정 해도 고객 목록에 있는 고객의 모양을 변경 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-165"> Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="ebbff-166">현재 목록에서 고객을 제거하는 옵션은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="ebbff-167">파트너는 나중에 **전환 원본** 계정에서 이러한 고객에 구독을 다시 추가하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>



6.  <span data-ttu-id="ebbff-168">모든 고객의 모든 구독에 대해 이러한 단계를 반복하여 이후 **Transitioning From**(전환 원본) 계정에 요금이 청구되지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="ebbff-169">파트너는 취소일과 청구 기간의 마지막 날 사이에 사용되지 않은 일수에 대한 크레딧이 포함된 최종 송장을 하나 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="ebbff-170">해당 최종 청구 기간 이후 더는 송장이 생성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-170">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="ebbff-171">참고</span><span class="sxs-lookup"><span data-stu-id="ebbff-171">Notes</span></span>

-   <span data-ttu-id="ebbff-172">**Transitioning From**(전환 원본) CSP 계정의 구독을 사용하지 않도록 설정해도, 이렇게 사용하지 않도록 설정하기 전에 서비스가 **Transitioning To**(전환 대상) CSP 계정에서 프로비전된 경우 최종 고객의 서비스에는 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="ebbff-173">고객은 구독을 사용할 수 없으며 구독이 일시 중단되거나 취소된 경우 청구 요금이 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="ebbff-174">현재 고객 목록에서 고객을 완전히 제거하는 방법은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-174">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="ebbff-175">**참고** 파트너는 파트너 센터에서 **전환 대상** 파트너 테넌트 계정 아래에 구독이 전환 및 설정되는 날과 같은 날에 파트너 센터의 **전환 원본** 파트너 테넌트 계정에서 해당 구독을 일시 중단하여 이중 청구가 발생하지 않도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-175">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ebbff-176">Microsoft는 **전환 원본** 구독을 일시 중단됨으로 올바르게 설정하지 않아 발생하는 청구의 겹침으로 인한 크레딧에 대한 요청은 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-176">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>



### <a name="simplify-migration-using-export"></a><span data-ttu-id="ebbff-177">내보내기를 사용하여 마이그레이션 간소화</span><span class="sxs-lookup"><span data-stu-id="ebbff-177">Simplify migration using Export</span></span>

<span data-ttu-id="ebbff-178">**내보내기 기능**을 사용하여 새 통합 구조에서 사용해야 하는 구독을 캡처할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="ebbff-179">클릭 **고객** 기존 구조에 있는 고객의 목록을 보려면 파트너 센터에서.</span><span class="sxs-lookup"><span data-stu-id="ebbff-179">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="ebbff-180">원하는 고객 이름을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-180">Open the desired customer name.</span></span>

3.  <span data-ttu-id="ebbff-181">**구독** 페이지에서 **구독 내보내기**를 클릭하여 구독 세부 정보를 Excel 파일로 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-181">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="ebbff-182">이 목록을 사용하여 새 통합 테넌트에서 구독을 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ebbff-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="ebbff-183">API 등록</span><span class="sxs-lookup"><span data-stu-id="ebbff-183">API registration</span></span>

<span data-ttu-id="ebbff-184">API 등록에 대한 자세한 내용은 [이 페이지를 참조](https://go.microsoft.com/fwlink/?linkid=847990)하세요.</span><span class="sxs-lookup"><span data-stu-id="ebbff-184">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>








