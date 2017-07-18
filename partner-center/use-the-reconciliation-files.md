---
title: "조정 파일 사용 | 파트너 센터"
description: "청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 61e71d4207d9e8ac68ee4fcfc1f0d04282474032
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/19/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="09ff0-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="09ff0-103">Use the reconciliation files</span></span>

**<span data-ttu-id="09ff0-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="09ff0-104">Applies to</span></span>**

-  <span data-ttu-id="09ff0-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="09ff0-105">Partner Center</span></span>
-  <span data-ttu-id="09ff0-106">미국 정부용 Microsoft 클라우드 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="09ff0-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="09ff0-107">Microsoft 클라우드 독일 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="09ff0-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="09ff0-108">청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="09ff0-109">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <span data-ttu-id="09ff0-110"><a href="" id="itemizebypartner"></a>파트너를 기준으로 항목별로 구분</span><span class="sxs-lookup"><span data-stu-id="09ff0-110"><a href="" id="itemizebypartner"></a>Itemize by partner</span></span>


<span data-ttu-id="09ff0-111">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="09ff0-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-112">MPN ID</span></span></th>
<th><span data-ttu-id="09ff0-113">설명</span><span class="sxs-lookup"><span data-stu-id="09ff0-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="09ff0-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="09ff0-115">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="09ff0-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-116">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="09ff0-117">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="09ff0-118">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="09ff0-119">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="09ff0-120">재판매인을 보거나 업데이트하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="09ff0-121">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="09ff0-122"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="09ff0-123">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="09ff0-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="09ff0-124">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="09ff0-125">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <span data-ttu-id="09ff0-126"><a href="" id="licencebasedfiles"></a> 라이선스 기준 파일 필드</span><span class="sxs-lookup"><span data-stu-id="09ff0-126"><a href="" id="licencebasedfiles"></a> License-based file fields</span></span>


<span data-ttu-id="09ff0-127">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="09ff0-128">열</span><span class="sxs-lookup"><span data-stu-id="09ff0-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="09ff0-129">설명</span><span class="sxs-lookup"><span data-stu-id="09ff0-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="09ff0-130">샘플 값</span><span class="sxs-lookup"><span data-stu-id="09ff0-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-131">OperatingUnit</span><span class="sxs-lookup"><span data-stu-id="09ff0-131">OperatingUnit</span></span></td>
<td><p><span data-ttu-id="09ff0-132">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="09ff0-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="09ff0-133">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="09ff0-134">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="09ff0-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="09ff0-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="09ff0-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="09ff0-137">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID.</span><span class="sxs-lookup"><span data-stu-id="09ff0-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="09ff0-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="09ff0-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="09ff0-139">OrderID</span></span></td>
<td><p><span data-ttu-id="09ff0-140">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="09ff0-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="09ff0-141">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="09ff0-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="09ff0-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="09ff0-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="09ff0-144">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="09ff0-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="09ff0-145">지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="09ff0-146">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="09ff0-147">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="09ff0-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="09ff0-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="09ff0-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="09ff0-150">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="09ff0-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="09ff0-151">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="09ff0-152">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="09ff0-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="09ff0-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="09ff0-154">OfferID</span></span></td>
<td><p><span data-ttu-id="09ff0-155">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="09ff0-155">Unique offer ID.</span></span> <span data-ttu-id="09ff0-156">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="09ff0-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="09ff0-157"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="09ff0-158">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="09ff0-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="09ff0-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="09ff0-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="09ff0-161">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="09ff0-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="09ff0-162"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="09ff0-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="09ff0-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="09ff0-164">OfferName</span></span></td>
<td><p><span data-ttu-id="09ff0-165">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="09ff0-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="09ff0-166">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="09ff0-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="09ff0-168">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="09ff0-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="09ff0-169">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="09ff0-170">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="09ff0-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="09ff0-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="09ff0-173">구독 종료 날짜: 12개월 + 시작 날짜 이후 x일(파트너 청구 날짜에 맞추기 위해) 또는 갱신 날짜로부터 12개월.</span><span class="sxs-lookup"><span data-stu-id="09ff0-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="09ff0-174">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="09ff0-175">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="09ff0-176">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="09ff0-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="09ff0-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="09ff0-179">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="09ff0-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="09ff0-180">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="09ff0-181">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="09ff0-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="09ff0-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="09ff0-184">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="09ff0-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="09ff0-185">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="09ff0-186">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="09ff0-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="09ff0-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="09ff0-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="09ff0-189">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="09ff0-189">The type of charge or adjustment.</span></span> <span data-ttu-id="09ff0-190"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="09ff0-191"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="09ff0-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="09ff0-193">실제 사용자 수당 가격.</span><span class="sxs-lookup"><span data-stu-id="09ff0-193">Price per seat.</span></span> <span data-ttu-id="09ff0-194">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="09ff0-195">6.82</span><span class="sxs-lookup"><span data-stu-id="09ff0-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="09ff0-196">Quantity</span></span></td>
<td><p><span data-ttu-id="09ff0-197">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="09ff0-197">Number of seats.</span></span> <span data-ttu-id="09ff0-198">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="09ff0-199">2</span><span class="sxs-lookup"><span data-stu-id="09ff0-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-200">Amount</span><span class="sxs-lookup"><span data-stu-id="09ff0-200">Amount</span></span></td>
<td><p><span data-ttu-id="09ff0-201">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="09ff0-201">Total of price for quantity.</span></span> <span data-ttu-id="09ff0-202">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="09ff0-203">13.32</span><span class="sxs-lookup"><span data-stu-id="09ff0-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="09ff0-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="09ff0-205">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="09ff0-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="09ff0-206">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="09ff0-207">2.32</span><span class="sxs-lookup"><span data-stu-id="09ff0-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="09ff0-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="09ff0-209">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="09ff0-209">Total before tax.</span></span> <span data-ttu-id="09ff0-210">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="09ff0-211">11</span><span class="sxs-lookup"><span data-stu-id="09ff0-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-212">Tax</span><span class="sxs-lookup"><span data-stu-id="09ff0-212">Tax</span></span></td>
<td><p><span data-ttu-id="09ff0-213">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="09ff0-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="09ff0-214">0</span><span class="sxs-lookup"><span data-stu-id="09ff0-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="09ff0-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="09ff0-216">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="09ff0-216">Total after tax.</span></span> <span data-ttu-id="09ff0-217">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="09ff0-218">11</span><span class="sxs-lookup"><span data-stu-id="09ff0-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-219">Currency</span><span class="sxs-lookup"><span data-stu-id="09ff0-219">Currency</span></span></td>
<td><p><span data-ttu-id="09ff0-220">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="09ff0-220">Currency type.</span></span> <span data-ttu-id="09ff0-221">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="09ff0-222">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="09ff0-223">EUR</span><span class="sxs-lookup"><span data-stu-id="09ff0-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="09ff0-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="09ff0-225">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="09ff0-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="09ff0-226">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="09ff0-227">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="09ff0-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="09ff0-228">MPNID</span></span></td>
<td><p><span data-ttu-id="09ff0-229">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="09ff0-230">4390934</span><span class="sxs-lookup"><span data-stu-id="09ff0-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="09ff0-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="09ff0-232">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="09ff0-233">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="09ff0-234">4390934</span><span class="sxs-lookup"><span data-stu-id="09ff0-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="09ff0-235">DomainName</span></span></td>
<td><p><span data-ttu-id="09ff0-236">고객을 식별하는 데 사용되는 고객의 도메인 이름.</span><span class="sxs-lookup"><span data-stu-id="09ff0-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="09ff0-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="09ff0-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="09ff0-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="09ff0-239">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="09ff0-239">Subscription nickname.</span></span> <span data-ttu-id="09ff0-240">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="09ff0-241">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="09ff0-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="09ff0-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="09ff0-243">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="09ff0-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="09ff0-244">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="09ff0-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="09ff0-245">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="09ff0-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <span data-ttu-id="09ff0-246"><a href="" id="usagebasedfiles"></a>사용량 기준 파일 필드</span><span class="sxs-lookup"><span data-stu-id="09ff0-246"><a href="" id="usagebasedfiles"></a>Usage-based file fields</span></span>


<span data-ttu-id="09ff0-247">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="09ff0-248">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="09ff0-249">열</span><span class="sxs-lookup"><span data-stu-id="09ff0-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="09ff0-250">설명</span><span class="sxs-lookup"><span data-stu-id="09ff0-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="09ff0-251">샘플 값</span><span class="sxs-lookup"><span data-stu-id="09ff0-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="09ff0-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="09ff0-253">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="09ff0-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="09ff0-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="09ff0-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="09ff0-256">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="09ff0-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="09ff0-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="09ff0-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="09ff0-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="09ff0-259">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="09ff0-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="09ff0-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="09ff0-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="09ff0-262">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="09ff0-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="09ff0-263">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="09ff0-264">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="09ff0-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="09ff0-265">MPNID</span></span></td>
<td><p><span data-ttu-id="09ff0-266">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="09ff0-267">4390934</span><span class="sxs-lookup"><span data-stu-id="09ff0-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="09ff0-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="09ff0-269">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="09ff0-270">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="09ff0-271">4390934</span><span class="sxs-lookup"><span data-stu-id="09ff0-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="09ff0-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="09ff0-273">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="09ff0-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="09ff0-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="09ff0-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="09ff0-276">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="09ff0-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="09ff0-277">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="09ff0-278">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="09ff0-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="09ff0-280">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="09ff0-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="09ff0-281">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="09ff0-282">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="09ff0-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="09ff0-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="09ff0-284">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="09ff0-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="09ff0-285">지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="09ff0-286">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="09ff0-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="09ff0-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="09ff0-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="09ff0-289">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="09ff0-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="09ff0-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="09ff0-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="09ff0-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="09ff0-292">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="09ff0-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="09ff0-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="09ff0-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="09ff0-294">OrderID</span></span></td>
<td><p><span data-ttu-id="09ff0-295">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="09ff0-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="09ff0-296">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="09ff0-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="09ff0-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="09ff0-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="09ff0-299">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="09ff0-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="09ff0-300">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="09ff0-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="09ff0-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="09ff0-302">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="09ff0-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="09ff0-303">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="09ff0-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="09ff0-304">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="09ff0-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="09ff0-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="09ff0-306">모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="09ff0-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="09ff0-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="09ff0-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-308">Resource Name</span><span class="sxs-lookup"><span data-stu-id="09ff0-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="09ff0-309">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="09ff0-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="09ff0-310">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="09ff0-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="09ff0-311">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="09ff0-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-312">Region</span><span class="sxs-lookup"><span data-stu-id="09ff0-312">Region</span></span></td>
<td><p><span data-ttu-id="09ff0-313">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-313">The region the usage applies to.</span></span> <span data-ttu-id="09ff0-314">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="09ff0-315">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="09ff0-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-316">SKU</span><span class="sxs-lookup"><span data-stu-id="09ff0-316">SKU</span></span></td>
<td><p><span data-ttu-id="09ff0-317">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="09ff0-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="09ff0-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="09ff0-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="09ff0-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="09ff0-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="09ff0-320">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="09ff0-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="09ff0-321">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="09ff0-322">1</span><span class="sxs-lookup"><span data-stu-id="09ff0-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="09ff0-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="09ff0-324">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="09ff0-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="09ff0-325">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="09ff0-326">11</span><span class="sxs-lookup"><span data-stu-id="09ff0-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="09ff0-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="09ff0-328">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="09ff0-328">Units included as part of the offer.</span></span> <span data-ttu-id="09ff0-329">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="09ff0-330">0</span><span class="sxs-lookup"><span data-stu-id="09ff0-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="09ff0-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="09ff0-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="09ff0-332">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="09ff0-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="09ff0-333">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="09ff0-334">11</span><span class="sxs-lookup"><span data-stu-id="09ff0-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="09ff0-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="09ff0-336">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="09ff0-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="09ff0-337">$0.0808</span><span class="sxs-lookup"><span data-stu-id="09ff0-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="09ff0-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="09ff0-339">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="09ff0-340">$0.085</span><span class="sxs-lookup"><span data-stu-id="09ff0-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="09ff0-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="09ff0-342">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="09ff0-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="09ff0-343">$0.08</span><span class="sxs-lookup"><span data-stu-id="09ff0-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="09ff0-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="09ff0-345">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="09ff0-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="09ff0-346">$0.93</span><span class="sxs-lookup"><span data-stu-id="09ff0-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-347">Currency</span><span class="sxs-lookup"><span data-stu-id="09ff0-347">Currency</span></span></td>
<td><p><span data-ttu-id="09ff0-348">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="09ff0-348">Currency type.</span></span> <span data-ttu-id="09ff0-349">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="09ff0-350">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="09ff0-351">EUR</span><span class="sxs-lookup"><span data-stu-id="09ff0-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="09ff0-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="09ff0-353">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="09ff0-353">Pretax price per unit.</span></span> <span data-ttu-id="09ff0-354">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="09ff0-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="09ff0-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="09ff0-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="09ff0-357">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="09ff0-357">Post tax price per unit.</span></span> <span data-ttu-id="09ff0-358">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="09ff0-359">$0.08</span><span class="sxs-lookup"><span data-stu-id="09ff0-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="09ff0-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="09ff0-361">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="09ff0-361">The type of charge or adjustment.</span></span> <span data-ttu-id="09ff0-362"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="09ff0-363"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="09ff0-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="09ff0-365">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="09ff0-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="09ff0-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="09ff0-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="09ff0-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="09ff0-368">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="09ff0-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="09ff0-369">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="09ff0-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="09ff0-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="09ff0-371">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="09ff0-372">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="09ff0-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="09ff0-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="09ff0-374">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="09ff0-375">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="09ff0-376">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="09ff0-377">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="09ff0-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="09ff0-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="09ff0-379">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="09ff0-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="09ff0-380">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="09ff0-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-381">Project</span><span class="sxs-lookup"><span data-stu-id="09ff0-381">Project</span></span></td>
<td><p><span data-ttu-id="09ff0-382">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="09ff0-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="09ff0-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="09ff0-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="09ff0-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="09ff0-385">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="09ff0-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="09ff0-386">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="09ff0-387">25팩 ServiceBus 연결 하나를 프로비전하고 해당 날짜에 연결 1개를 사용한 경우 해당 날짜의 일일 사용 내역서는 "25개 연결/30일 - 사용됨: 1.000000"으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="09ff0-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="09ff0-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="09ff0-389">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID.</span><span class="sxs-lookup"><span data-stu-id="09ff0-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="09ff0-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="09ff0-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="09ff0-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="09ff0-391">DomainName</span></span></td>
<td><p><span data-ttu-id="09ff0-392">고객을 식별하는 데 사용되는 고객의 도메인 이름.</span><span class="sxs-lookup"><span data-stu-id="09ff0-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="09ff0-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="09ff0-393">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <span data-ttu-id="09ff0-394"><a href="" id="charge_types">송장과 조정 파일 간 요금 매핑</a></span><span class="sxs-lookup"><span data-stu-id="09ff0-394"><a href="" id="charge_types"></a>Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="09ff0-395">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-395">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="09ff0-396">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-396">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="09ff0-397">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-397">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="09ff0-398">송장 요금 설명</span><span class="sxs-lookup"><span data-stu-id="09ff0-398">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="09ff0-399">조정 파일 요금 설명(ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="09ff0-399">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="09ff0-400">이 요금은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="09ff0-400">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="09ff0-401">ChargeTypes를 송장에 매핑하려면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="09ff0-401">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="09ff0-402">반복 청구 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-402">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="09ff0-403">취소 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="09ff0-403">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-404">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-404">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="09ff0-405">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-405">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-406">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="09ff0-406">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-407">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-407">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-408">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="09ff0-408">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-409">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-409">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-410">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-410">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-411">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="09ff0-411">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-412">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-412">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-413">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-413">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-414">구매 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-414">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-415">구독의 초기 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-415">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-416">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-416">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-417">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-417">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-418">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-418">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-419">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-419">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="09ff0-420">기타 제품 및 서비스</span><span class="sxs-lookup"><span data-stu-id="09ff0-420">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="09ff0-421">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-421">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-422">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-422">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-423">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-423">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="09ff0-424">사용 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-424">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="09ff0-425">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="09ff0-425">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-426">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="09ff0-426">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="09ff0-427">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-427">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-428">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="09ff0-428">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-429">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="09ff0-429">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="09ff0-430">크레딧 및 조정</span><span class="sxs-lookup"><span data-stu-id="09ff0-430">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="09ff0-431">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="09ff0-431">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-432">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="09ff0-432">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-433">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-433">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="09ff0-434">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-434">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="09ff0-435">기타 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-435">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="09ff0-436">(사용량 기반)</span><span class="sxs-lookup"><span data-stu-id="09ff0-436">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="09ff0-437">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-437">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-438">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-438">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="09ff0-439">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-439">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-440">주기 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-440">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-441">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-441">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="09ff0-442">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-442">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-443">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-443">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="09ff0-444">취소 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-444">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-445">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="09ff0-445">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="09ff0-446">기타 할인</span><span class="sxs-lookup"><span data-stu-id="09ff0-446">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="09ff0-447">(라이선스 기반)</span><span class="sxs-lookup"><span data-stu-id="09ff0-447">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="09ff0-448">여러 종류의 요금에 적용될 수 있음</span><span class="sxs-lookup"><span data-stu-id="09ff0-448">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="09ff0-449">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-449">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="09ff0-450"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="09ff0-450"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="09ff0-451">여러 종류의 요금에 적용될 수 있음</span><span class="sxs-lookup"><span data-stu-id="09ff0-451">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="09ff0-452">예외: "품목 오프셋"에는 이미 세금이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09ff0-452">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="09ff0-453">위의 크레딧 및 조정을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09ff0-453">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="09ff0-454">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="09ff0-454">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="09ff0-455">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-455">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="09ff0-456">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="09ff0-456">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
