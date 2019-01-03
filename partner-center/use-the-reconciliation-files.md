---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 청구 주기에서 각 요금의 자세한 품목 보기에 대 한 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 50af14ab0e8edf6cd4576be6615cd7238b23bd99
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990995"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="940c8-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="940c8-103">Use the reconciliation files</span></span>

**<span data-ttu-id="940c8-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="940c8-104">Applies to</span></span>**

-  <span data-ttu-id="940c8-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="940c8-105">Partner Center</span></span>
-  <span data-ttu-id="940c8-106">미국 정부용 Microsoft 클라우드 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="940c8-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="940c8-107">청구 주기에서 각 요금의 자세한 품목 보기에 대 한 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="940c8-108">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="940c8-109">파트너를 기준으로 항목별로 구분</span><span class="sxs-lookup"><span data-stu-id="940c8-109">Itemize by partner</span></span>


<span data-ttu-id="940c8-110">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="940c8-111">MPN ID</span><span class="sxs-lookup"><span data-stu-id="940c8-111">MPN ID</span></span></th>
<th><span data-ttu-id="940c8-112">설명</span><span class="sxs-lookup"><span data-stu-id="940c8-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="940c8-113">MPN ID</span><span class="sxs-lookup"><span data-stu-id="940c8-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="940c8-114">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="940c8-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-115">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="940c8-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="940c8-116">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="940c8-117">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="940c8-118">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="940c8-119">보거나 업데이트 파트너 센터 메뉴에서 재판매인을 <strong>고객</strong>을 선택한 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="940c8-120">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="940c8-121"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="940c8-122">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="940c8-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="940c8-123">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="940c8-124">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="940c8-125">라이선스 기준 파일 필드</span><span class="sxs-lookup"><span data-stu-id="940c8-125">License-based file fields</span></span>


<span data-ttu-id="940c8-126">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="940c8-127">열</span><span class="sxs-lookup"><span data-stu-id="940c8-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="940c8-128">설명</span><span class="sxs-lookup"><span data-stu-id="940c8-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="940c8-129">샘플 값</span><span class="sxs-lookup"><span data-stu-id="940c8-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-130">PartnerID</span><span class="sxs-lookup"><span data-stu-id="940c8-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="940c8-131">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="940c8-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="940c8-132">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="940c8-133">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="940c8-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="940c8-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="940c8-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="940c8-136">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID.</span><span class="sxs-lookup"><span data-stu-id="940c8-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="940c8-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="940c8-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="940c8-138">OrderID</span></span></td>
<td><p><span data-ttu-id="940c8-139">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="940c8-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="940c8-140">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="940c8-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="940c8-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="940c8-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="940c8-143">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="940c8-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="940c8-144">지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="940c8-145">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="940c8-146">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="940c8-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="940c8-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="940c8-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="940c8-149">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="940c8-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="940c8-150">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="940c8-151">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="940c8-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="940c8-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="940c8-153">OfferID</span></span></td>
<td><p><span data-ttu-id="940c8-154">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="940c8-154">Unique offer ID.</span></span> <span data-ttu-id="940c8-155">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="940c8-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="940c8-156"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="940c8-157">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="940c8-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="940c8-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="940c8-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="940c8-160">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="940c8-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="940c8-161"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="940c8-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="940c8-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="940c8-163">OfferName</span></span></td>
<td><p><span data-ttu-id="940c8-164">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="940c8-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="940c8-165">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="940c8-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="940c8-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="940c8-167">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="940c8-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="940c8-168">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="940c8-169">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="940c8-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="940c8-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="940c8-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="940c8-172">구독 종료 날짜: 12개월 + 시작 날짜 이후 x일(파트너 청구 날짜에 맞추기 위해) 또는 갱신 날짜로부터 12개월.</span><span class="sxs-lookup"><span data-stu-id="940c8-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="940c8-173">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="940c8-174">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="940c8-175">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="940c8-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="940c8-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="940c8-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="940c8-178">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="940c8-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="940c8-179">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="940c8-180">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="940c8-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="940c8-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="940c8-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="940c8-183">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="940c8-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="940c8-184">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="940c8-185">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="940c8-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="940c8-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="940c8-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="940c8-188">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="940c8-188">The type of charge or adjustment.</span></span> <span data-ttu-id="940c8-189"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="940c8-190"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="940c8-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="940c8-192">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="940c8-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="940c8-193">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="940c8-194">6.82</span><span class="sxs-lookup"><span data-stu-id="940c8-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="940c8-195">Quantity</span></span></td>
<td><p><span data-ttu-id="940c8-196">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="940c8-196">Number of seats.</span></span> <span data-ttu-id="940c8-197">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="940c8-198">2</span><span class="sxs-lookup"><span data-stu-id="940c8-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-199">Amount</span><span class="sxs-lookup"><span data-stu-id="940c8-199">Amount</span></span></td>
<td><p><span data-ttu-id="940c8-200">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="940c8-200">Total of price for quantity.</span></span> <span data-ttu-id="940c8-201">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="940c8-202">13.32</span><span class="sxs-lookup"><span data-stu-id="940c8-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="940c8-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="940c8-204">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="940c8-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="940c8-205">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="940c8-206">2.32</span><span class="sxs-lookup"><span data-stu-id="940c8-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="940c8-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="940c8-208">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="940c8-208">Total before tax.</span></span> <span data-ttu-id="940c8-209">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="940c8-210">11</span><span class="sxs-lookup"><span data-stu-id="940c8-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-211">Tax</span><span class="sxs-lookup"><span data-stu-id="940c8-211">Tax</span></span></td>
<td><p><span data-ttu-id="940c8-212">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="940c8-212">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="940c8-213">0</span><span class="sxs-lookup"><span data-stu-id="940c8-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="940c8-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="940c8-215">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="940c8-215">Total after tax.</span></span> <span data-ttu-id="940c8-216">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="940c8-217">11</span><span class="sxs-lookup"><span data-stu-id="940c8-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-218">Currency</span><span class="sxs-lookup"><span data-stu-id="940c8-218">Currency</span></span></td>
<td><p><span data-ttu-id="940c8-219">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="940c8-219">Currency type.</span></span> <span data-ttu-id="940c8-220">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="940c8-221">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="940c8-222">EUR</span><span class="sxs-lookup"><span data-stu-id="940c8-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="940c8-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="940c8-224">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="940c8-224">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="940c8-225">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="940c8-226">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="940c8-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="940c8-227">MPNID</span></span></td>
<td><p><span data-ttu-id="940c8-228">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="940c8-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="940c8-229">4390934</span><span class="sxs-lookup"><span data-stu-id="940c8-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="940c8-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="940c8-231">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="940c8-232">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-232">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="940c8-233">4390934</span><span class="sxs-lookup"><span data-stu-id="940c8-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="940c8-234">DomainName</span></span></td>
<td><p><span data-ttu-id="940c8-235">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-235">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="940c8-236">와 고객/파트너 O365 포털을 통해 베 니 티/기본 도메인을 업데이트할 수 있는 고객을 고유 하 게 식별 하 하지 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="940c8-237">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="940c8-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="940c8-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="940c8-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="940c8-240">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="940c8-240">Subscription nickname.</span></span> <span data-ttu-id="940c8-241">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="940c8-242">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="940c8-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="940c8-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="940c8-244">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="940c8-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="940c8-245">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="940c8-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="940c8-246">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="940c8-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="940c8-247">사용량 기준 파일 필드</span><span class="sxs-lookup"><span data-stu-id="940c8-247">Usage-based file fields</span></span>


<span data-ttu-id="940c8-248">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="940c8-249">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="940c8-250">열</span><span class="sxs-lookup"><span data-stu-id="940c8-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="940c8-251">설명</span><span class="sxs-lookup"><span data-stu-id="940c8-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="940c8-252">샘플 값</span><span class="sxs-lookup"><span data-stu-id="940c8-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="940c8-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="940c8-254">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="940c8-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="940c8-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="940c8-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="940c8-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="940c8-257">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="940c8-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="940c8-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="940c8-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="940c8-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="940c8-260">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="940c8-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="940c8-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="940c8-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="940c8-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="940c8-263">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="940c8-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="940c8-264">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="940c8-265">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="940c8-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="940c8-266">MPNID</span></span></td>
<td><p><span data-ttu-id="940c8-267">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="940c8-268">4390934</span><span class="sxs-lookup"><span data-stu-id="940c8-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="940c8-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="940c8-270">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="940c8-271">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="940c8-272">4390934</span><span class="sxs-lookup"><span data-stu-id="940c8-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="940c8-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="940c8-274">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="940c8-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="940c8-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="940c8-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="940c8-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="940c8-277">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="940c8-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="940c8-278">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="940c8-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="940c8-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="940c8-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="940c8-281">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="940c8-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="940c8-282">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="940c8-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="940c8-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="940c8-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="940c8-285">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="940c8-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="940c8-286">지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="940c8-287">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="940c8-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="940c8-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="940c8-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="940c8-290">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="940c8-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="940c8-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="940c8-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="940c8-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="940c8-293">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="940c8-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="940c8-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="940c8-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="940c8-295">OrderID</span></span></td>
<td><p><span data-ttu-id="940c8-296">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="940c8-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="940c8-297">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="940c8-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="940c8-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="940c8-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="940c8-300">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="940c8-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="940c8-301">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="940c8-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="940c8-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="940c8-303">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="940c8-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="940c8-304">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="940c8-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="940c8-305">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="940c8-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="940c8-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="940c8-307">모든 서비스 데이터 및 가격 책정 구조에 대한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="940c8-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="940c8-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="940c8-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="940c8-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="940c8-310">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="940c8-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="940c8-311">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="940c8-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="940c8-312">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="940c8-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-313">Region</span><span class="sxs-lookup"><span data-stu-id="940c8-313">Region</span></span></td>
<td><p><span data-ttu-id="940c8-314">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-314">The region the usage applies to.</span></span> <span data-ttu-id="940c8-315">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="940c8-316">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="940c8-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-317">SKU</span><span class="sxs-lookup"><span data-stu-id="940c8-317">SKU</span></span></td>
<td><p><span data-ttu-id="940c8-318">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="940c8-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="940c8-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="940c8-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="940c8-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="940c8-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="940c8-321">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="940c8-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="940c8-322">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="940c8-323">1</span><span class="sxs-lookup"><span data-stu-id="940c8-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="940c8-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="940c8-325">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="940c8-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="940c8-326">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="940c8-327">11</span><span class="sxs-lookup"><span data-stu-id="940c8-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="940c8-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="940c8-329">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="940c8-329">Units included as part of the offer.</span></span> <span data-ttu-id="940c8-330">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="940c8-331">0</span><span class="sxs-lookup"><span data-stu-id="940c8-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="940c8-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="940c8-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="940c8-333">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="940c8-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="940c8-334">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="940c8-335">11</span><span class="sxs-lookup"><span data-stu-id="940c8-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="940c8-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="940c8-337">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="940c8-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="940c8-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="940c8-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="940c8-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="940c8-340">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="940c8-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="940c8-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="940c8-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="940c8-343">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="940c8-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="940c8-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="940c8-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="940c8-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="940c8-346">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="940c8-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="940c8-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="940c8-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-348">Currency</span><span class="sxs-lookup"><span data-stu-id="940c8-348">Currency</span></span></td>
<td><p><span data-ttu-id="940c8-349">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="940c8-349">Currency type.</span></span> <span data-ttu-id="940c8-350">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="940c8-351">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="940c8-352">EUR</span><span class="sxs-lookup"><span data-stu-id="940c8-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="940c8-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="940c8-354">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="940c8-354">Pretax price per unit.</span></span> <span data-ttu-id="940c8-355">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="940c8-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="940c8-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="940c8-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="940c8-358">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="940c8-358">Post tax price per unit.</span></span> <span data-ttu-id="940c8-359">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="940c8-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="940c8-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="940c8-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="940c8-362">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="940c8-362">The type of charge or adjustment.</span></span> <span data-ttu-id="940c8-363"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="940c8-364"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="940c8-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="940c8-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="940c8-366">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="940c8-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="940c8-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="940c8-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="940c8-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="940c8-369">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="940c8-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="940c8-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="940c8-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="940c8-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="940c8-372">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="940c8-373">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="940c8-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="940c8-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="940c8-375">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="940c8-376">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="940c8-377">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="940c8-378">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="940c8-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="940c8-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="940c8-380">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="940c8-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="940c8-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="940c8-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-382">Project</span><span class="sxs-lookup"><span data-stu-id="940c8-382">Project</span></span></td>
<td><p><span data-ttu-id="940c8-383">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="940c8-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="940c8-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="940c8-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="940c8-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="940c8-386">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="940c8-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="940c8-387">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="940c8-388">25팩 ServiceBus 연결 하나를 프로비전하고 해당 날짜에 연결 1개를 사용한 경우 해당 날짜의 일일 사용 내역서는 "25개 연결/30일 - 사용됨: 1.000000"으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="940c8-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="940c8-390">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID.</span><span class="sxs-lookup"><span data-stu-id="940c8-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="940c8-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="940c8-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="940c8-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="940c8-392">DomainName</span></span></td>
<td><p><span data-ttu-id="940c8-393">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="940c8-394">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="940c8-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="940c8-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="940c8-396">단위</span><span class="sxs-lookup"><span data-stu-id="940c8-396">Unit</span></span></td>
<td><p><span data-ttu-id="940c8-397">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="940c8-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="940c8-398">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="940c8-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="940c8-399">일회성구입 파일 필드</span><span class="sxs-lookup"><span data-stu-id="940c8-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="940c8-400">필드</span><span class="sxs-lookup"><span data-stu-id="940c8-400">Field</span></span>** |**<span data-ttu-id="940c8-401">정의</span><span class="sxs-lookup"><span data-stu-id="940c8-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="940c8-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="940c8-402">PartnerId</span></span> |<span data-ttu-id="940c8-403">GUID 형식의 파트너 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="940c8-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="940c8-404">CustomerId</span></span> |<span data-ttu-id="940c8-405">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="940c8-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="940c8-406">CustomerName</span></span> |<span data-ttu-id="940c8-407">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="940c8-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="940c8-408">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="940c8-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="940c8-409">CustomerDomainName</span></span> |<span data-ttu-id="940c8-410">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="940c8-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="940c8-411">CustomerCountry</span></span> |<span data-ttu-id="940c8-412">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="940c8-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="940c8-413">InvoiceNumber</span></span> |<span data-ttu-id="940c8-414">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="940c8-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="940c8-415">MpnId</span></span> |<span data-ttu-id="940c8-416">CSP 파트너(직접 또는 간접)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="940c8-417">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="940c8-417">Reseller MPN ID</span></span> |<span data-ttu-id="940c8-418">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="940c8-419">예약에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="940c8-420">파트너 센터에서 특정 예약에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="940c8-421">CSP 파트너가 고객에게 직접 예약을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="940c8-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="940c8-422">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="940c8-423">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="940c8-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="940c8-424">OrderId</span></span> |<span data-ttu-id="940c8-425">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="940c8-426">지원 팀에 문의할 때는 Azure 예약을 식별하는 것이 유용할 수 있지만, 조정에서는 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="940c8-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="940c8-427">OrderDate</span></span> |<span data-ttu-id="940c8-428">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-428">The date the order was placed.</span></span> |
|<span data-ttu-id="940c8-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="940c8-429">ProductId</span></span> |<span data-ttu-id="940c8-430">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-430">The ID for the product.</span></span> |
|<span data-ttu-id="940c8-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="940c8-431">SkuId</span></span>  |<span data-ttu-id="940c8-432">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="940c8-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="940c8-433">AvailabilityId</span></span> |<span data-ttu-id="940c8-434">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-434">The ID for a particular Availability.</span></span> <span data-ttu-id="940c8-435">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="940c8-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="940c8-436">SkuName</span></span>  |<span data-ttu-id="940c8-437">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="940c8-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="940c8-438">ProductName</span></span> |<span data-ttu-id="940c8-439">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-439">The name of the product.</span></span> |
|<span data-ttu-id="940c8-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="940c8-440">ChargeType</span></span> |<span data-ttu-id="940c8-441">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="940c8-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="940c8-442">UnitPrice</span></span> |<span data-ttu-id="940c8-443">주문한 각 제품의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-443">Price per product ordered.</span></span> |
|<span data-ttu-id="940c8-444">수량</span><span class="sxs-lookup"><span data-stu-id="940c8-444">Quantity</span></span> |<span data-ttu-id="940c8-445">주문한 제품의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-445">Number of products ordered.</span></span> |
|<span data-ttu-id="940c8-446">소계</span><span class="sxs-lookup"><span data-stu-id="940c8-446">Subtotal</span></span> |<span data-ttu-id="940c8-447">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="940c8-447">Total before tax.</span></span> <span data-ttu-id="940c8-448">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="940c8-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="940c8-449">TaxTotal</span></span> |<span data-ttu-id="940c8-450">적용 가능한 모든 세금의 총액입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="940c8-451">총액</span><span class="sxs-lookup"><span data-stu-id="940c8-451">Total</span></span> |<span data-ttu-id="940c8-452">총 구입 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="940c8-453">통화</span><span class="sxs-lookup"><span data-stu-id="940c8-453">Currency</span></span> |<span data-ttu-id="940c8-454">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="940c8-454">Currency type.</span></span> <span data-ttu-id="940c8-455">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="940c8-456">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="940c8-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="940c8-457">DiscountDetails</span></span> |<span data-ttu-id="940c8-458">모든 관련 할인에 대한 상세 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="940c8-459">송장과 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="940c8-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="940c8-460">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="940c8-461">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="940c8-462">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="940c8-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="940c8-463">송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="940c8-464">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="940c8-465">송장 요금 설명</span><span class="sxs-lookup"><span data-stu-id="940c8-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="940c8-466">조정 파일 요금 설명(ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="940c8-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="940c8-467">이 요금은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="940c8-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="940c8-468">ChargeTypes를 송장에 매핑하려면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="940c8-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="940c8-469">라이선스 기준 청구</span><span class="sxs-lookup"><span data-stu-id="940c8-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="940c8-470">승인 수수료</span><span class="sxs-lookup"><span data-stu-id="940c8-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-471">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="940c8-472">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-473">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="940c8-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-474">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-475">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="940c8-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-476">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-477">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="940c8-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-478">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-479">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-480">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="940c8-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-481">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-482">연간 청구를 사용 하는 경우 구독에 대 한 청구 유형</span><span class="sxs-lookup"><span data-stu-id="940c8-482">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-483">구매 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-484">월별 청구를 사용 하는 경우 구독에 대 한 청구 유형</span><span class="sxs-lookup"><span data-stu-id="940c8-484">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-485">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-486">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="940c8-487">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-488">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-489">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-490">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="940c8-491">사용 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="940c8-492">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="940c8-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-493">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="940c8-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="940c8-494">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-495">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="940c8-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-496">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="940c8-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="940c8-497">크레딧</span><span class="sxs-lookup"><span data-stu-id="940c8-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="940c8-498">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="940c8-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-499">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="940c8-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-500">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="940c8-501">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="940c8-502">사용량 기준 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="940c8-503">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-504">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="940c8-505">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-506">주기 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-507">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-508">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-509">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-510">취소 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-511">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="940c8-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="940c8-512">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="940c8-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="940c8-513">여러 종류의 요금에 적용될 수 있음</span><span class="sxs-lookup"><span data-stu-id="940c8-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="940c8-514">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="940c8-515"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="940c8-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="940c8-516">여러 종류의 요금에 적용될 수 있음</span><span class="sxs-lookup"><span data-stu-id="940c8-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="940c8-517">예외: "품목 오프셋"에는 이미 세금이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="940c8-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="940c8-518">위의 크레딧, 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="940c8-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="940c8-519">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="940c8-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="940c8-520">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="940c8-521">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="940c8-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
