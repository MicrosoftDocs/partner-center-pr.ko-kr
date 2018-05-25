---
title: 조정 파일 사용 | 파트너 센터
description: 청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892138374f5730bdc10bdf07f75d0a8e3ef56bea
ms.sourcegitcommit: 2d3203dd5e2653af031a8009aa3b999a454acef5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/10/2018
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="1e2a2-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="1e2a2-103">Use the reconciliation files</span></span>

**<span data-ttu-id="1e2a2-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="1e2a2-104">Applies to</span></span>**

-  <span data-ttu-id="1e2a2-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="1e2a2-105">Partner Center</span></span>
-  <span data-ttu-id="1e2a2-106">Microsoft Cloud for US Government용 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="1e2a2-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="1e2a2-107">Microsoft 클라우드 독일 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="1e2a2-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="1e2a2-108">청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="1e2a2-109">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="1e2a2-110">파트너를 기준으로 항목별로 구분</span><span class="sxs-lookup"><span data-stu-id="1e2a2-110">Itemize by partner</span></span>


<span data-ttu-id="1e2a2-111">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1e2a2-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-112">MPN ID</span></span></th>
<th><span data-ttu-id="1e2a2-113">설명</span><span class="sxs-lookup"><span data-stu-id="1e2a2-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1e2a2-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="1e2a2-115">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-116">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="1e2a2-117">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="1e2a2-118">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1e2a2-119">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="1e2a2-120">재판매인을 보거나 업데이트하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="1e2a2-121">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="1e2a2-122"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="1e2a2-123">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="1e2a2-124">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="1e2a2-125">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="1e2a2-126">라이선스 기준 파일 필드</span><span class="sxs-lookup"><span data-stu-id="1e2a2-126">License-based file fields</span></span>


<span data-ttu-id="1e2a2-127">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="1e2a2-128">열</span><span class="sxs-lookup"><span data-stu-id="1e2a2-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="1e2a2-129">설명</span><span class="sxs-lookup"><span data-stu-id="1e2a2-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="1e2a2-130">샘플 값</span><span class="sxs-lookup"><span data-stu-id="1e2a2-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-131">PartnerID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="1e2a2-132">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1e2a2-133">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1e2a2-134">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="1e2a2-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="1e2a2-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="1e2a2-137">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1e2a2-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="1e2a2-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-139">OrderID</span></span></td>
<td><p><span data-ttu-id="1e2a2-140">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1e2a2-141">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1e2a2-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1e2a2-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1e2a2-144">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1e2a2-145">지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1e2a2-146">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="1e2a2-147">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="1e2a2-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1e2a2-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="1e2a2-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="1e2a2-150">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="1e2a2-151">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="1e2a2-152">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1e2a2-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="1e2a2-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-154">OfferID</span></span></td>
<td><p><span data-ttu-id="1e2a2-155">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-155">Unique offer ID.</span></span> <span data-ttu-id="1e2a2-156">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="1e2a2-157"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="1e2a2-158">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="1e2a2-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="1e2a2-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="1e2a2-161">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="1e2a2-162"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="1e2a2-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="1e2a2-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-164">OfferName</span></span></td>
<td><p><span data-ttu-id="1e2a2-165">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="1e2a2-166">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-168">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="1e2a2-169">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="1e2a2-170">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1e2a2-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1e2a2-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-173">구독 종료 날짜: 12개월 + 시작 날짜 이후 x일(파트너 청구 날짜에 맞추기 위해) 또는 갱신 날짜로부터 12개월.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="1e2a2-174">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="1e2a2-175">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="1e2a2-176">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1e2a2-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1e2a2-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-179">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="1e2a2-180">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1e2a2-181">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1e2a2-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1e2a2-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-184">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="1e2a2-185">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1e2a2-186">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1e2a2-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="1e2a2-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1e2a2-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="1e2a2-189">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-189">The type of charge or adjustment.</span></span> <span data-ttu-id="1e2a2-190"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1e2a2-191"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="1e2a2-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="1e2a2-193">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1e2a2-194">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1e2a2-195">6.82</span><span class="sxs-lookup"><span data-stu-id="1e2a2-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="1e2a2-196">Quantity</span></span></td>
<td><p><span data-ttu-id="1e2a2-197">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-197">Number of seats.</span></span> <span data-ttu-id="1e2a2-198">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1e2a2-199">2</span><span class="sxs-lookup"><span data-stu-id="1e2a2-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-200">Amount</span><span class="sxs-lookup"><span data-stu-id="1e2a2-200">Amount</span></span></td>
<td><p><span data-ttu-id="1e2a2-201">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-201">Total of price for quantity.</span></span> <span data-ttu-id="1e2a2-202">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="1e2a2-203">13.32</span><span class="sxs-lookup"><span data-stu-id="1e2a2-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="1e2a2-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="1e2a2-205">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="1e2a2-206">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="1e2a2-207">2.32</span><span class="sxs-lookup"><span data-stu-id="1e2a2-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="1e2a2-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="1e2a2-209">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-209">Total before tax.</span></span> <span data-ttu-id="1e2a2-210">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="1e2a2-211">11</span><span class="sxs-lookup"><span data-stu-id="1e2a2-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-212">Tax</span><span class="sxs-lookup"><span data-stu-id="1e2a2-212">Tax</span></span></td>
<td><p><span data-ttu-id="1e2a2-213">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1e2a2-214">0</span><span class="sxs-lookup"><span data-stu-id="1e2a2-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="1e2a2-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="1e2a2-216">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-216">Total after tax.</span></span> <span data-ttu-id="1e2a2-217">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="1e2a2-218">11</span><span class="sxs-lookup"><span data-stu-id="1e2a2-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-219">Currency</span><span class="sxs-lookup"><span data-stu-id="1e2a2-219">Currency</span></span></td>
<td><p><span data-ttu-id="1e2a2-220">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-220">Currency type.</span></span> <span data-ttu-id="1e2a2-221">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="1e2a2-222">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1e2a2-223">EUR</span><span class="sxs-lookup"><span data-stu-id="1e2a2-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="1e2a2-225">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="1e2a2-226">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1e2a2-227">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="1e2a2-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-228">MPNID</span></span></td>
<td><p><span data-ttu-id="1e2a2-229">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="1e2a2-230">4390934</span><span class="sxs-lookup"><span data-stu-id="1e2a2-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1e2a2-232">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1e2a2-233">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="1e2a2-234">4390934</span><span class="sxs-lookup"><span data-stu-id="1e2a2-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-235">DomainName</span></span></td>
<td><p><span data-ttu-id="1e2a2-236">고객을 식별하는 데 사용되는 고객의 도메인 이름.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="1e2a2-237">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1e2a2-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1e2a2-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1e2a2-240">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-240">Subscription nickname.</span></span> <span data-ttu-id="1e2a2-241">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="1e2a2-242">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1e2a2-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1e2a2-244">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1e2a2-245">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="1e2a2-246">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="1e2a2-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="1e2a2-247">사용량 기준 파일 필드</span><span class="sxs-lookup"><span data-stu-id="1e2a2-247">Usage-based file fields</span></span>


<span data-ttu-id="1e2a2-248">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="1e2a2-249">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="1e2a2-250">열</span><span class="sxs-lookup"><span data-stu-id="1e2a2-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="1e2a2-251">설명</span><span class="sxs-lookup"><span data-stu-id="1e2a2-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="1e2a2-252">샘플 값</span><span class="sxs-lookup"><span data-stu-id="1e2a2-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="1e2a2-254">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="1e2a2-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1e2a2-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="1e2a2-257">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="1e2a2-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="1e2a2-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="1e2a2-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="1e2a2-260">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="1e2a2-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="1e2a2-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="1e2a2-263">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="1e2a2-264">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1e2a2-265">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="1e2a2-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-266">MPNID</span></span></td>
<td><p><span data-ttu-id="1e2a2-267">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="1e2a2-268">4390934</span><span class="sxs-lookup"><span data-stu-id="1e2a2-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1e2a2-270">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1e2a2-271">[파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="1e2a2-272">4390934</span><span class="sxs-lookup"><span data-stu-id="1e2a2-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1e2a2-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1e2a2-274">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="1e2a2-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="1e2a2-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="1e2a2-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-277">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1e2a2-278">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1e2a2-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1e2a2-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-281">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1e2a2-282">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1e2a2-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="1e2a2-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1e2a2-285">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1e2a2-286">지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1e2a2-287">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1e2a2-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1e2a2-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1e2a2-290">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="1e2a2-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1e2a2-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1e2a2-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1e2a2-293">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="1e2a2-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1e2a2-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-295">OrderID</span></span></td>
<td><p><span data-ttu-id="1e2a2-296">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1e2a2-297">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1e2a2-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1e2a2-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="1e2a2-300">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="1e2a2-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="1e2a2-301">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="1e2a2-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="1e2a2-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="1e2a2-303">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="1e2a2-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1e2a2-304">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="1e2a2-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="1e2a2-305">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="1e2a2-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="1e2a2-307">모든 서비스 데이터 및 가격 책정 구조에 대한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="1e2a2-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="1e2a2-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1e2a2-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="1e2a2-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="1e2a2-310">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="1e2a2-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1e2a2-311">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="1e2a2-312">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-313">Region</span><span class="sxs-lookup"><span data-stu-id="1e2a2-313">Region</span></span></td>
<td><p><span data-ttu-id="1e2a2-314">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-314">The region the usage applies to.</span></span> <span data-ttu-id="1e2a2-315">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="1e2a2-316">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="1e2a2-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-317">SKU</span><span class="sxs-lookup"><span data-stu-id="1e2a2-317">SKU</span></span></td>
<td><p><span data-ttu-id="1e2a2-318">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="1e2a2-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="1e2a2-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="1e2a2-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1e2a2-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="1e2a2-321">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="1e2a2-322">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="1e2a2-323">1</span><span class="sxs-lookup"><span data-stu-id="1e2a2-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="1e2a2-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="1e2a2-325">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="1e2a2-326">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="1e2a2-327">11</span><span class="sxs-lookup"><span data-stu-id="1e2a2-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="1e2a2-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="1e2a2-329">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-329">Units included as part of the offer.</span></span> <span data-ttu-id="1e2a2-330">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="1e2a2-331">0</span><span class="sxs-lookup"><span data-stu-id="1e2a2-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1e2a2-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="1e2a2-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="1e2a2-333">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="1e2a2-334">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="1e2a2-335">11</span><span class="sxs-lookup"><span data-stu-id="1e2a2-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="1e2a2-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="1e2a2-337">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="1e2a2-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="1e2a2-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="1e2a2-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="1e2a2-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="1e2a2-340">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1e2a2-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="1e2a2-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="1e2a2-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="1e2a2-343">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1e2a2-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="1e2a2-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="1e2a2-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="1e2a2-346">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="1e2a2-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="1e2a2-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="1e2a2-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-348">Currency</span><span class="sxs-lookup"><span data-stu-id="1e2a2-348">Currency</span></span></td>
<td><p><span data-ttu-id="1e2a2-349">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-349">Currency type.</span></span> <span data-ttu-id="1e2a2-350">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="1e2a2-351">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1e2a2-352">EUR</span><span class="sxs-lookup"><span data-stu-id="1e2a2-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1e2a2-354">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-354">Pretax price per unit.</span></span> <span data-ttu-id="1e2a2-355">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1e2a2-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="1e2a2-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1e2a2-358">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-358">Post tax price per unit.</span></span> <span data-ttu-id="1e2a2-359">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1e2a2-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="1e2a2-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1e2a2-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="1e2a2-362">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-362">The type of charge or adjustment.</span></span> <span data-ttu-id="1e2a2-363"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1e2a2-364"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="1e2a2-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="1e2a2-366">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="1e2a2-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="1e2a2-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="1e2a2-369">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="1e2a2-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="1e2a2-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1e2a2-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="1e2a2-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="1e2a2-372">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="1e2a2-373">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="1e2a2-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="1e2a2-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="1e2a2-375">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="1e2a2-376">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="1e2a2-377">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="1e2a2-378">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="1e2a2-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="1e2a2-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="1e2a2-380">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="1e2a2-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="1e2a2-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="1e2a2-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-382">Project</span><span class="sxs-lookup"><span data-stu-id="1e2a2-382">Project</span></span></td>
<td><p><span data-ttu-id="1e2a2-383">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="1e2a2-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="1e2a2-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1e2a2-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="1e2a2-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="1e2a2-386">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="1e2a2-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="1e2a2-387">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="1e2a2-388">25팩 ServiceBus 연결 하나를 프로비전하고 해당 날짜에 연결 1개를 사용한 경우 해당 날짜의 일일 사용 내역서는 "25개 연결/30일 - 사용됨: 1.000000"으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="1e2a2-390">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1e2a2-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1e2a2-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1e2a2-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-392">DomainName</span></span></td>
<td><p><span data-ttu-id="1e2a2-393">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="1e2a2-394">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1e2a2-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1e2a2-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="1e2a2-396">단위</span><span class="sxs-lookup"><span data-stu-id="1e2a2-396">Unit</span></span></td>
<td><p><span data-ttu-id="1e2a2-397">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="1e2a2-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="1e2a2-398">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="1e2a2-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="1e2a2-399">일회성구입 파일 필드</span><span class="sxs-lookup"><span data-stu-id="1e2a2-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="1e2a2-400">필드</span><span class="sxs-lookup"><span data-stu-id="1e2a2-400">Field</span></span>** |**<span data-ttu-id="1e2a2-401">정의</span><span class="sxs-lookup"><span data-stu-id="1e2a2-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="1e2a2-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-402">PartnerId</span></span> |<span data-ttu-id="1e2a2-403">GUID 형식의 파트너 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="1e2a2-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-404">CustomerId</span></span> |<span data-ttu-id="1e2a2-405">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="1e2a2-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-406">CustomerName</span></span> |<span data-ttu-id="1e2a2-407">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="1e2a2-408">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="1e2a2-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-409">CustomerDomainName</span></span> |<span data-ttu-id="1e2a2-410">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="1e2a2-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="1e2a2-411">CustomerCountry</span></span> |<span data-ttu-id="1e2a2-412">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="1e2a2-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1e2a2-413">InvoiceNumber</span></span> |<span data-ttu-id="1e2a2-414">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="1e2a2-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-415">MpnId</span></span> |<span data-ttu-id="1e2a2-416">CSP 파트너(직접 또는 간접)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="1e2a2-417">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="1e2a2-417">Reseller MPN ID</span></span> |<span data-ttu-id="1e2a2-418">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="1e2a2-419">예약에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="1e2a2-420">파트너 센터에서 특정 예약에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="1e2a2-421">CSP 파트너가 고객에게 직접 예약을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="1e2a2-422">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="1e2a2-423">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="1e2a2-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-424">OrderId</span></span> |<span data-ttu-id="1e2a2-425">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1e2a2-426">지원 팀에 문의할 때는 Azure 예약을 식별하는 것이 유용할 수 있지만, 조정에서는 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="1e2a2-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="1e2a2-427">OrderDate</span></span> |<span data-ttu-id="1e2a2-428">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-428">The date the order was placed.</span></span> |
|<span data-ttu-id="1e2a2-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-429">ProductId</span></span> |<span data-ttu-id="1e2a2-430">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-430">The ID for the product.</span></span> |
|<span data-ttu-id="1e2a2-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-431">SkuId</span></span>  |<span data-ttu-id="1e2a2-432">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="1e2a2-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1e2a2-433">AvailabilityId</span></span> |<span data-ttu-id="1e2a2-434">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-434">The ID for a particular Availability.</span></span> <span data-ttu-id="1e2a2-435">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="1e2a2-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-436">SkuName</span></span>  |<span data-ttu-id="1e2a2-437">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="1e2a2-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="1e2a2-438">ProductName</span></span> |<span data-ttu-id="1e2a2-439">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-439">The name of the product.</span></span> |
|<span data-ttu-id="1e2a2-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1e2a2-440">ChargeType</span></span> |<span data-ttu-id="1e2a2-441">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="1e2a2-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="1e2a2-442">UnitPrice</span></span> |<span data-ttu-id="1e2a2-443">주문한 각 제품의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-443">Price per product ordered.</span></span> |
|<span data-ttu-id="1e2a2-444">수량</span><span class="sxs-lookup"><span data-stu-id="1e2a2-444">Quantity</span></span> |<span data-ttu-id="1e2a2-445">주문한 제품의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-445">Number of products ordered.</span></span> |
|<span data-ttu-id="1e2a2-446">소계</span><span class="sxs-lookup"><span data-stu-id="1e2a2-446">Subtotal</span></span> |<span data-ttu-id="1e2a2-447">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-447">Total before tax.</span></span> <span data-ttu-id="1e2a2-448">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="1e2a2-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="1e2a2-449">TaxTotal</span></span> |<span data-ttu-id="1e2a2-450">적용 가능한 모든 세금의 총액입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="1e2a2-451">총액</span><span class="sxs-lookup"><span data-stu-id="1e2a2-451">Total</span></span> |<span data-ttu-id="1e2a2-452">총 구입 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="1e2a2-453">통화</span><span class="sxs-lookup"><span data-stu-id="1e2a2-453">Currency</span></span> |<span data-ttu-id="1e2a2-454">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-454">Currency type.</span></span> <span data-ttu-id="1e2a2-455">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="1e2a2-456">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="1e2a2-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="1e2a2-457">DiscountDetails</span></span> |<span data-ttu-id="1e2a2-458">모든 관련 할인에 대한 상세 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="1e2a2-459">송장과 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="1e2a2-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="1e2a2-460">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="1e2a2-461">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="1e2a2-462">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="1e2a2-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="1e2a2-463">송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="1e2a2-464">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="1e2a2-465">송장 요금 설명</span><span class="sxs-lookup"><span data-stu-id="1e2a2-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="1e2a2-466">조정 파일 요금 설명(ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="1e2a2-467">이 요금은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="1e2a2-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="1e2a2-468">ChargeTypes를 송장에 매핑하려면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="1e2a2-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="1e2a2-469">반복 청구 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-469">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-470">승인 수수료</span><span class="sxs-lookup"><span data-stu-id="1e2a2-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-471">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="1e2a2-472">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-473">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="1e2a2-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-474">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-475">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="1e2a2-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-476">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-477">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="1e2a2-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-478">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-479">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-480">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="1e2a2-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-481">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-482">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-482">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-483">구매 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-484">구독의 초기 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-484">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-485">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-486">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-487">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-488">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="1e2a2-489">기타 제품 및 서비스</span><span class="sxs-lookup"><span data-stu-id="1e2a2-489">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-490">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-491">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-492">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-492">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="1e2a2-493">사용 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-493">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-494">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-494">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-495">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-495">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="1e2a2-496">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-496">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-497">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-497">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-498">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-498">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="1e2a2-499">크레딧 및 조정</span><span class="sxs-lookup"><span data-stu-id="1e2a2-499">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-500">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="1e2a2-500">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-501">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="1e2a2-501">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-502">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-502">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="1e2a2-503">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-503">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="1e2a2-504">기타 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-504">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="1e2a2-505">(사용량 기반)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-505">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-506">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-506">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-507">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-507">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="1e2a2-508">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-508">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-509">주기 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-509">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-510">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-510">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="1e2a2-511">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-511">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-512">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-512">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="1e2a2-513">취소 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-513">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-514">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="1e2a2-514">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="1e2a2-515">기타 할인</span><span class="sxs-lookup"><span data-stu-id="1e2a2-515">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="1e2a2-516">(라이선스 기반)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-516">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="1e2a2-517">여러 종류의 요금에 적용될 수 있음</span><span class="sxs-lookup"><span data-stu-id="1e2a2-517">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="1e2a2-518">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-518">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1e2a2-519"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="1e2a2-519"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="1e2a2-520">여러 종류의 요금에 적용될 수 있음</span><span class="sxs-lookup"><span data-stu-id="1e2a2-520">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="1e2a2-521">예외: "품목 오프셋"에는 이미 세금이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-521">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="1e2a2-522">위의 크레딧 및 조정을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e2a2-522">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-523">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="1e2a2-523">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="1e2a2-524">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-524">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="1e2a2-525">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="1e2a2-525">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
