---
title: 조정 파일 (21Vianet에서 운영 하는 파트너 센터)를 사용 합니다.
ms.topic: article
ms.date: 10/29/2018
description: 청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584986"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="7650b-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="7650b-103">Use the reconciliation files</span></span>

<span data-ttu-id="7650b-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="7650b-104">**Applies to**</span></span>

-   <span data-ttu-id="7650b-105">21Vianet에서 운영하는 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="7650b-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="7650b-106">청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="7650b-107">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="7650b-108">파트너가 항목별로 정리</span><span class="sxs-lookup"><span data-stu-id="7650b-108">Itemize by partner</span></span>


<span data-ttu-id="7650b-109">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 모두 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="7650b-110">MPN ID</span><span class="sxs-lookup"><span data-stu-id="7650b-110">MPN ID</span></span></th>
<th><span data-ttu-id="7650b-111">설명</span><span class="sxs-lookup"><span data-stu-id="7650b-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="7650b-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="7650b-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="7650b-113">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="7650b-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-114">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="7650b-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="7650b-115">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="7650b-116">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7650b-117">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="7650b-118">재판매인을 보거나 업데이트하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="7650b-119">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="7650b-120"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="7650b-121">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="7650b-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="7650b-122">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="7650b-123">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="7650b-124">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="7650b-124">License-based file fields</span></span>


<span data-ttu-id="7650b-125">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="7650b-126"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="7650b-127"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="7650b-128"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="7650b-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="7650b-130">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="7650b-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="7650b-131">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="7650b-132">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="7650b-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="7650b-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="7650b-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="7650b-135">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="7650b-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="7650b-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="7650b-137">OrderID</span></span></td>
<td><p><span data-ttu-id="7650b-138">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="7650b-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="7650b-139">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="7650b-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="7650b-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="7650b-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="7650b-142">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="7650b-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="7650b-143">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="7650b-144">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="7650b-145">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="7650b-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="7650b-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="7650b-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="7650b-148">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="7650b-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="7650b-149">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="7650b-150">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="7650b-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="7650b-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="7650b-152">OfferID</span></span></td>
<td><p><span data-ttu-id="7650b-153">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="7650b-153">Unique offer ID.</span></span> <span data-ttu-id="7650b-154">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="7650b-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="7650b-155"><b>참고</b>: 이 값은 가격 목록에서 제품 ID를 일치 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="7650b-156">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="7650b-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="7650b-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="7650b-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="7650b-159">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="7650b-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="7650b-160"><b>참고</b>: 이 값에는 가격 목록에서 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="7650b-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="7650b-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="7650b-162">OfferName</span></span></td>
<td><p><span data-ttu-id="7650b-163">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="7650b-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="7650b-164">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="7650b-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="7650b-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="7650b-166">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="7650b-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="7650b-167">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="7650b-168">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7650b-169">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="7650b-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="7650b-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="7650b-171">구독 종료 날짜: 12 개월 + x 일 후 시작 날짜 (종료 날짜를 청구 하는 파트너와 맞춤) 또는 갱신 날짜 로부터 12 개월입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="7650b-172">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="7650b-173">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="7650b-174">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7650b-175">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="7650b-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="7650b-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="7650b-177">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="7650b-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="7650b-178">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="7650b-179">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7650b-180">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="7650b-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="7650b-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="7650b-182">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="7650b-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="7650b-183">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="7650b-184">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="7650b-185">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="7650b-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="7650b-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="7650b-187">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="7650b-187">The type of charge or adjustment.</span></span> <span data-ttu-id="7650b-188"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="7650b-189"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="7650b-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="7650b-191">실제 사용자 수당 가격.</span><span class="sxs-lookup"><span data-stu-id="7650b-191">Price per seat.</span></span> <span data-ttu-id="7650b-192">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="7650b-193">6.82</span><span class="sxs-lookup"><span data-stu-id="7650b-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-194">수량</span><span class="sxs-lookup"><span data-stu-id="7650b-194">Quantity</span></span></td>
<td><p><span data-ttu-id="7650b-195">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="7650b-195">Number of seats.</span></span> <span data-ttu-id="7650b-196">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="7650b-197">2</span><span class="sxs-lookup"><span data-stu-id="7650b-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-198">합계</span><span class="sxs-lookup"><span data-stu-id="7650b-198">Amount</span></span></td>
<td><p><span data-ttu-id="7650b-199">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="7650b-199">Total of price for quantity.</span></span> <span data-ttu-id="7650b-200">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="7650b-201">13.32</span><span class="sxs-lookup"><span data-stu-id="7650b-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="7650b-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="7650b-203">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="7650b-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="7650b-204">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="7650b-205">2.32</span><span class="sxs-lookup"><span data-stu-id="7650b-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-206">Subtotal</span><span class="sxs-lookup"><span data-stu-id="7650b-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="7650b-207">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="7650b-207">Total before tax.</span></span> <span data-ttu-id="7650b-208">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="7650b-209">11</span><span class="sxs-lookup"><span data-stu-id="7650b-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-210">Tax</span><span class="sxs-lookup"><span data-stu-id="7650b-210">Tax</span></span></td>
<td><p><span data-ttu-id="7650b-211">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="7650b-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="7650b-212">0</span><span class="sxs-lookup"><span data-stu-id="7650b-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="7650b-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="7650b-214">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="7650b-214">Total after tax.</span></span> <span data-ttu-id="7650b-215">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="7650b-216">11</span><span class="sxs-lookup"><span data-stu-id="7650b-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-217">Currency</span><span class="sxs-lookup"><span data-stu-id="7650b-217">Currency</span></span></td>
<td><p><span data-ttu-id="7650b-218">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="7650b-218">Currency type.</span></span> <span data-ttu-id="7650b-219">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="7650b-220">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="7650b-221">CNY</span><span class="sxs-lookup"><span data-stu-id="7650b-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="7650b-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="7650b-223">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="7650b-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="7650b-224">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="7650b-225">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="7650b-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="7650b-226">MPNID</span></span></td>
<td><p><span data-ttu-id="7650b-227">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="7650b-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="7650b-228">4390934</span><span class="sxs-lookup"><span data-stu-id="7650b-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="7650b-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="7650b-230">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7650b-231">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="7650b-232">4390934</span><span class="sxs-lookup"><span data-stu-id="7650b-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="7650b-233">DomainName</span></span></td>
<td><p><span data-ttu-id="7650b-234">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="7650b-235">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7650b-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="7650b-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="7650b-237">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="7650b-237">Subscription nickname.</span></span> <span data-ttu-id="7650b-238">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="7650b-239">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="7650b-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="7650b-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="7650b-241">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="7650b-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="7650b-242">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="7650b-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="7650b-243">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="7650b-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="7650b-244">사용량 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="7650b-244">Usage-based file fields</span></span>


<span data-ttu-id="7650b-245">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="7650b-246">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="7650b-247"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="7650b-248"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="7650b-249"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="7650b-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="7650b-251">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="7650b-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="7650b-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="7650b-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="7650b-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="7650b-254">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="7650b-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="7650b-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="7650b-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="7650b-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="7650b-257">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="7650b-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="7650b-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="7650b-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="7650b-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="7650b-260">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="7650b-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="7650b-261">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="7650b-262">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="7650b-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="7650b-263">MPNID</span></span></td>
<td><p><span data-ttu-id="7650b-264">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="7650b-265">4390934</span><span class="sxs-lookup"><span data-stu-id="7650b-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="7650b-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="7650b-267">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="7650b-268">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="7650b-269">4390934</span><span class="sxs-lookup"><span data-stu-id="7650b-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="7650b-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="7650b-271">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="7650b-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="7650b-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="7650b-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="7650b-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="7650b-274">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="7650b-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="7650b-275">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="7650b-276">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="7650b-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="7650b-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="7650b-278">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="7650b-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="7650b-279">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="7650b-280">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="7650b-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="7650b-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="7650b-282">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="7650b-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="7650b-283">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="7650b-284">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="7650b-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="7650b-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="7650b-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="7650b-287">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="7650b-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="7650b-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="7650b-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="7650b-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="7650b-290">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="7650b-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="7650b-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="7650b-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="7650b-292">OrderID</span></span></td>
<td><p><span data-ttu-id="7650b-293">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="7650b-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="7650b-294">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="7650b-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="7650b-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="7650b-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="7650b-297">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="7650b-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="7650b-298">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="7650b-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="7650b-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="7650b-300">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="7650b-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="7650b-301">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="7650b-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="7650b-302">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="7650b-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="7650b-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="7650b-304">모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="7650b-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="7650b-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="7650b-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-306">Resource Name</span><span class="sxs-lookup"><span data-stu-id="7650b-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="7650b-307">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="7650b-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="7650b-308">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="7650b-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="7650b-309">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="7650b-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-310">Region</span><span class="sxs-lookup"><span data-stu-id="7650b-310">Region</span></span></td>
<td><p><span data-ttu-id="7650b-311">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-311">The region the usage applies to.</span></span> <span data-ttu-id="7650b-312">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="7650b-313">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="7650b-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-314">SKU</span><span class="sxs-lookup"><span data-stu-id="7650b-314">SKU</span></span></td>
<td><p><span data-ttu-id="7650b-315">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="7650b-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="7650b-316">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="7650b-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="7650b-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="7650b-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="7650b-318">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="7650b-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="7650b-319">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="7650b-320">1</span><span class="sxs-lookup"><span data-stu-id="7650b-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="7650b-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="7650b-322">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="7650b-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="7650b-323">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="7650b-324">11</span><span class="sxs-lookup"><span data-stu-id="7650b-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="7650b-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="7650b-326">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="7650b-326">Units included as part of the offer.</span></span> <span data-ttu-id="7650b-327">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="7650b-328">0</span><span class="sxs-lookup"><span data-stu-id="7650b-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="7650b-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="7650b-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="7650b-330">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="7650b-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="7650b-331">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="7650b-332">11</span><span class="sxs-lookup"><span data-stu-id="7650b-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="7650b-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="7650b-334">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="7650b-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="7650b-335">$0.0808</span><span class="sxs-lookup"><span data-stu-id="7650b-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="7650b-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="7650b-337">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="7650b-338">$0.085</span><span class="sxs-lookup"><span data-stu-id="7650b-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="7650b-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="7650b-340">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="7650b-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="7650b-341">$0.08</span><span class="sxs-lookup"><span data-stu-id="7650b-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="7650b-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="7650b-343">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="7650b-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="7650b-344">$0.93</span><span class="sxs-lookup"><span data-stu-id="7650b-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-345">Currency</span><span class="sxs-lookup"><span data-stu-id="7650b-345">Currency</span></span></td>
<td><p><span data-ttu-id="7650b-346">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="7650b-346">Currency type.</span></span> <span data-ttu-id="7650b-347">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="7650b-348">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="7650b-349">CNY</span><span class="sxs-lookup"><span data-stu-id="7650b-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="7650b-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="7650b-351">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="7650b-351">Pretax price per unit.</span></span> <span data-ttu-id="7650b-352">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="7650b-353">$0.08</span><span class="sxs-lookup"><span data-stu-id="7650b-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="7650b-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="7650b-355">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="7650b-355">Post tax price per unit.</span></span> <span data-ttu-id="7650b-356">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="7650b-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="7650b-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="7650b-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="7650b-359">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="7650b-359">The type of charge or adjustment.</span></span> <span data-ttu-id="7650b-360"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="7650b-361"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7650b-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="7650b-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="7650b-363">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="7650b-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="7650b-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="7650b-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="7650b-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="7650b-366">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="7650b-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="7650b-367">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="7650b-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="7650b-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="7650b-369">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="7650b-370">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="7650b-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="7650b-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="7650b-372">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="7650b-373">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="7650b-374">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="7650b-375">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="7650b-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="7650b-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="7650b-377">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="7650b-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="7650b-378">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="7650b-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-379">Project</span><span class="sxs-lookup"><span data-stu-id="7650b-379">Project</span></span></td>
<td><p><span data-ttu-id="7650b-380">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="7650b-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="7650b-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="7650b-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="7650b-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="7650b-383">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="7650b-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="7650b-384">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="7650b-385">해당 날짜에 대 한 일일 사용량 명세서 477860 경우 프로 비전 하는 service Bus 연결 25 팩 있고 해당 일 동안 1을 사용 하면, "25 개 연결 / 30 일 – 사용: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="7650b-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="7650b-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="7650b-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="7650b-387">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="7650b-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="7650b-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="7650b-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="7650b-389">DomainName</span></span></td>
<td><p><span data-ttu-id="7650b-390">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="7650b-391">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7650b-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="7650b-392">청구서 및 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="7650b-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="7650b-393">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="7650b-394">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="7650b-395">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="7650b-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="7650b-396"><strong>청구서 금액 충전 설명</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-397"><strong>조정 파일 금액 설명 (ChargeType 열)</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-398"><strong>이 요금 이란 무엇 인가요?</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-399"><strong>이러한 ChargeTypes를 청구서에 매핑하려면 어떻게 하나요?</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="7650b-400"><strong>반복 청구 요금</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-401">취소 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="7650b-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-402">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="7650b-403">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-404">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="7650b-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-405">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-406">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="7650b-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-407">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-408">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-409">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="7650b-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-410">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-411">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-412">구매 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-413">구독의 초기 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-414">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-415">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-416">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-417">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-418"><strong>다른 제품 및 서비스</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-419">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-420">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-421">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="7650b-422"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-423">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="7650b-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-424">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="7650b-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="7650b-425">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-426">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="7650b-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-427">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="7650b-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-428"><strong>크레딧 &amp; 조정</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-429">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="7650b-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-430">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="7650b-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-431">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="7650b-432">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="7650b-433"><strong>기타 할인</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="7650b-434">
<em>(usage-based)</em></span><span class="sxs-lookup"><span data-stu-id="7650b-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-435">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-436">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="7650b-437">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-438">주기 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-439">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="7650b-440">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-441">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="7650b-442">취소 할인</span><span class="sxs-lookup"><span data-stu-id="7650b-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-443">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="7650b-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-444"><strong>기타 할인</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="7650b-445">
<em>(라이선스 기반)</em></span><span class="sxs-lookup"><span data-stu-id="7650b-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-446"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="7650b-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="7650b-447">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="7650b-448"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="7650b-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-449"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="7650b-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="7650b-450"><em>예외: "품목 요금 차감" 세금을 이미 포함 되어 있습니다. 크레딧 참조 &amp; 조정 위의 합니다.</em></span><span class="sxs-lookup"><span data-stu-id="7650b-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-451">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="7650b-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="7650b-452">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="7650b-453">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="7650b-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
