---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 9997b01c76dacb736baa33f458def0b820753f1d
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682511"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="cd6f3-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="cd6f3-103">Use the reconciliation files</span></span>

<span data-ttu-id="cd6f3-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="cd6f3-104">**Applies to**</span></span>

-  <span data-ttu-id="cd6f3-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="cd6f3-105">Partner Center</span></span>
-  <span data-ttu-id="cd6f3-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="cd6f3-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="cd6f3-107">각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="cd6f3-108">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="cd6f3-109">파트너가 항목별로 정리</span><span class="sxs-lookup"><span data-stu-id="cd6f3-109">Itemize by partner</span></span>


<span data-ttu-id="cd6f3-110">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 모두 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cd6f3-111">MPN ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-111">MPN ID</span></span></th>
<th><span data-ttu-id="cd6f3-112">설명</span><span class="sxs-lookup"><span data-stu-id="cd6f3-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cd6f3-113">MPN ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="cd6f3-114">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-115">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="cd6f3-116">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="cd6f3-117">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cd6f3-118">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="cd6f3-119">eTo 확인 하거나 업데이트 대리점에서 파트너 센터 메뉴에서 선택 <strong>고객</strong>, 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="cd6f3-120">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="cd6f3-121"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="cd6f3-122">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="cd6f3-123">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="cd6f3-124">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="cd6f3-125">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="cd6f3-125">License-based file fields</span></span>


<span data-ttu-id="cd6f3-126">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cd6f3-127"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="cd6f3-128"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="cd6f3-129"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="cd6f3-131">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="cd6f3-132">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="cd6f3-133">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="cd6f3-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="cd6f3-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="cd6f3-136">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="cd6f3-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="cd6f3-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-138">OrderID</span></span></td>
<td><p><span data-ttu-id="cd6f3-139">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="cd6f3-140">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="cd6f3-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="cd6f3-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="cd6f3-143">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cd6f3-144">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="cd6f3-145">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="cd6f3-146">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="cd6f3-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="cd6f3-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="cd6f3-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="cd6f3-149">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="cd6f3-150">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="cd6f3-151">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="cd6f3-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="cd6f3-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-153">OfferID</span></span></td>
<td><p><span data-ttu-id="cd6f3-154">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-154">Unique offer ID.</span></span> <span data-ttu-id="cd6f3-155">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="cd6f3-156"><b>참고</b>: 이 값은 가격 목록에서 제품 ID를 일치 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="cd6f3-157">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="cd6f3-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="cd6f3-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="cd6f3-160">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="cd6f3-161"><b>참고</b>: 이 값에는 가격 목록에서 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="cd6f3-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="cd6f3-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-163">OfferName</span></span></td>
<td><p><span data-ttu-id="cd6f3-164">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="cd6f3-165">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="cd6f3-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-167">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="cd6f3-168">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="cd6f3-169">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cd6f3-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cd6f3-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-172">구독 종료 날짜: 12 개월 + x 일 후 시작 날짜 (종료 날짜를 청구 하는 파트너와 맞춤) 또는 갱신 날짜 로부터 12 개월입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="cd6f3-173">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="cd6f3-174">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="cd6f3-175">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cd6f3-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cd6f3-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-178">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="cd6f3-179">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="cd6f3-180">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cd6f3-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="cd6f3-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-183">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="cd6f3-184">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="cd6f3-185">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="cd6f3-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="cd6f3-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="cd6f3-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="cd6f3-188">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-188">The type of charge or adjustment.</span></span> <span data-ttu-id="cd6f3-189"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="cd6f3-190"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="cd6f3-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="cd6f3-192">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cd6f3-193">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="cd6f3-194">6.82</span><span class="sxs-lookup"><span data-stu-id="cd6f3-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-195">수량</span><span class="sxs-lookup"><span data-stu-id="cd6f3-195">Quantity</span></span></td>
<td><p><span data-ttu-id="cd6f3-196">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-196">Number of seats.</span></span> <span data-ttu-id="cd6f3-197">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="cd6f3-198">2</span><span class="sxs-lookup"><span data-stu-id="cd6f3-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-199">Amount</span><span class="sxs-lookup"><span data-stu-id="cd6f3-199">Amount</span></span></td>
<td><p><span data-ttu-id="cd6f3-200">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-200">Total of price for quantity.</span></span> <span data-ttu-id="cd6f3-201">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="cd6f3-202">13.32</span><span class="sxs-lookup"><span data-stu-id="cd6f3-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="cd6f3-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="cd6f3-204">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="cd6f3-205">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="cd6f3-206">2.32</span><span class="sxs-lookup"><span data-stu-id="cd6f3-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="cd6f3-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="cd6f3-208">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-208">Total before tax.</span></span> <span data-ttu-id="cd6f3-209">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="cd6f3-210">11</span><span class="sxs-lookup"><span data-stu-id="cd6f3-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-211">Tax</span><span class="sxs-lookup"><span data-stu-id="cd6f3-211">Tax</span></span></td>
<td><p><span data-ttu-id="cd6f3-212">세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="cd6f3-213">0</span><span class="sxs-lookup"><span data-stu-id="cd6f3-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="cd6f3-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="cd6f3-215">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-215">Total after tax.</span></span> <span data-ttu-id="cd6f3-216">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="cd6f3-217">11</span><span class="sxs-lookup"><span data-stu-id="cd6f3-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-218">Currency</span><span class="sxs-lookup"><span data-stu-id="cd6f3-218">Currency</span></span></td>
<td><p><span data-ttu-id="cd6f3-219">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-219">Currency type.</span></span> <span data-ttu-id="cd6f3-220">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="cd6f3-221">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="cd6f3-222">EUR</span><span class="sxs-lookup"><span data-stu-id="cd6f3-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="cd6f3-224">고객&#39;파트너 센터에 보고 된 s 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="cd6f3-225">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="cd6f3-226">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="cd6f3-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-227">MPNID</span></span></td>
<td><p><span data-ttu-id="cd6f3-228">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="cd6f3-229">4390934</span><span class="sxs-lookup"><span data-stu-id="cd6f3-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="cd6f3-231">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cd6f3-232"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="cd6f3-233">4390934</span><span class="sxs-lookup"><span data-stu-id="cd6f3-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-234">DomainName</span></span></td>
<td><p><span data-ttu-id="cd6f3-235">고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="cd6f3-236">이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="cd6f3-237">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="cd6f3-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cd6f3-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="cd6f3-240">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-240">Subscription nickname.</span></span> <span data-ttu-id="cd6f3-241">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="cd6f3-242">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="cd6f3-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="cd6f3-244">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="cd6f3-245">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="cd6f3-246">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="cd6f3-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="cd6f3-247">사용량 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="cd6f3-247">Usage-based file fields</span></span>


<span data-ttu-id="cd6f3-248">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="cd6f3-249">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cd6f3-250"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="cd6f3-251"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="cd6f3-252"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="cd6f3-254">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="cd6f3-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="cd6f3-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="cd6f3-257">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="cd6f3-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="cd6f3-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="cd6f3-260">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="cd6f3-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="cd6f3-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="cd6f3-263">고객&#39;파트너 센터에 보고 된 s 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="cd6f3-264">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="cd6f3-265">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="cd6f3-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-266">MPNID</span></span></td>
<td><p><span data-ttu-id="cd6f3-267">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="cd6f3-268">4390934</span><span class="sxs-lookup"><span data-stu-id="cd6f3-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="cd6f3-270">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cd6f3-271"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="cd6f3-272">4390934</span><span class="sxs-lookup"><span data-stu-id="cd6f3-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="cd6f3-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="cd6f3-274">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="cd6f3-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="cd6f3-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="cd6f3-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-277">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="cd6f3-278">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="cd6f3-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="cd6f3-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-281">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="cd6f3-282">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="cd6f3-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="cd6f3-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="cd6f3-285">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cd6f3-286">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="cd6f3-287">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="cd6f3-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="cd6f3-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="cd6f3-290">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="cd6f3-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cd6f3-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="cd6f3-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="cd6f3-293">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="cd6f3-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="cd6f3-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cd6f3-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-295">OrderID</span></span></td>
<td><p><span data-ttu-id="cd6f3-296">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="cd6f3-297">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="cd6f3-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="cd6f3-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="cd6f3-300">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="cd6f3-301">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="cd6f3-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="cd6f3-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="cd6f3-303">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="cd6f3-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="cd6f3-304">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="cd6f3-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="cd6f3-305">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="cd6f3-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="cd6f3-307">모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="cd6f3-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="cd6f3-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="cd6f3-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="cd6f3-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="cd6f3-310">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="cd6f3-311">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="cd6f3-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="cd6f3-312">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="cd6f3-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-313">Region</span><span class="sxs-lookup"><span data-stu-id="cd6f3-313">Region</span></span></td>
<td><p><span data-ttu-id="cd6f3-314">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-314">The region the usage applies to.</span></span> <span data-ttu-id="cd6f3-315">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="cd6f3-316">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="cd6f3-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-317">SKU</span><span class="sxs-lookup"><span data-stu-id="cd6f3-317">SKU</span></span></td>
<td><p><span data-ttu-id="cd6f3-318">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="cd6f3-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="cd6f3-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="cd6f3-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="cd6f3-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="cd6f3-321">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="cd6f3-322">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="cd6f3-323">1</span><span class="sxs-lookup"><span data-stu-id="cd6f3-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="cd6f3-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="cd6f3-325">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="cd6f3-326">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="cd6f3-327">11</span><span class="sxs-lookup"><span data-stu-id="cd6f3-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="cd6f3-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="cd6f3-329">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-329">Units included as part of the offer.</span></span> <span data-ttu-id="cd6f3-330">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="cd6f3-331">0</span><span class="sxs-lookup"><span data-stu-id="cd6f3-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="cd6f3-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="cd6f3-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="cd6f3-333">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="cd6f3-334">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="cd6f3-335">11</span><span class="sxs-lookup"><span data-stu-id="cd6f3-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="cd6f3-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="cd6f3-337">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="cd6f3-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="cd6f3-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="cd6f3-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="cd6f3-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="cd6f3-340">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cd6f3-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="cd6f3-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="cd6f3-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="cd6f3-343">세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="cd6f3-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="cd6f3-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="cd6f3-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="cd6f3-346">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="cd6f3-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="cd6f3-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="cd6f3-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-348">Currency</span><span class="sxs-lookup"><span data-stu-id="cd6f3-348">Currency</span></span></td>
<td><p><span data-ttu-id="cd6f3-349">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-349">Currency type.</span></span> <span data-ttu-id="cd6f3-350">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="cd6f3-351">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="cd6f3-352">EUR</span><span class="sxs-lookup"><span data-stu-id="cd6f3-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="cd6f3-354">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-354">Pretax price per unit.</span></span> <span data-ttu-id="cd6f3-355">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cd6f3-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="cd6f3-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="cd6f3-358">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-358">Post tax price per unit.</span></span> <span data-ttu-id="cd6f3-359">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="cd6f3-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="cd6f3-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="cd6f3-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="cd6f3-362">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-362">The type of charge or adjustment.</span></span> <span data-ttu-id="cd6f3-363"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="cd6f3-364"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="cd6f3-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="cd6f3-366">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="cd6f3-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="cd6f3-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-369">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="cd6f3-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="cd6f3-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="cd6f3-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="cd6f3-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="cd6f3-372">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="cd6f3-373">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="cd6f3-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="cd6f3-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="cd6f3-375">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="cd6f3-376">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="cd6f3-377">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="cd6f3-378">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="cd6f3-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="cd6f3-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="cd6f3-380">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="cd6f3-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="cd6f3-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="cd6f3-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-382">프로젝트</span><span class="sxs-lookup"><span data-stu-id="cd6f3-382">Project</span></span></td>
<td><p><span data-ttu-id="cd6f3-383">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="cd6f3-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="cd6f3-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="cd6f3-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="cd6f3-386">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="cd6f3-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="cd6f3-387">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="cd6f3-388">해당 날짜에 대 한 일일 사용량 명세서 477860 경우 프로 비전 하는 service Bus 연결 25 팩 있고 해당 일 동안 1을 사용 하면, "25 개 연결 / 30 일 – 사용: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="cd6f3-390">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="cd6f3-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="cd6f3-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cd6f3-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-392">DomainName</span></span></td>
<td><p><span data-ttu-id="cd6f3-393">고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="cd6f3-394">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="cd6f3-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cd6f3-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="cd6f3-396">단위</span><span class="sxs-lookup"><span data-stu-id="cd6f3-396">Unit</span></span></td>
<td><p><span data-ttu-id="cd6f3-397">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="cd6f3-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="cd6f3-398">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="cd6f3-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="cd6f3-399">일회성 및 되풀이 파일 필드</span><span class="sxs-lookup"><span data-stu-id="cd6f3-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cd6f3-400">Column</span><span class="sxs-lookup"><span data-stu-id="cd6f3-400">Column</span></span></th>
<th><span data-ttu-id="cd6f3-401">설명</span><span class="sxs-lookup"><span data-stu-id="cd6f3-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="cd6f3-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="cd6f3-403">특정 청구 엔터티 GUID 형식에서에 대 한 고유한 Microsoft Azure Active Directory 테 넌 트 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="cd6f3-404">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="cd6f3-405">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-406">Customer Id</span><span class="sxs-lookup"><span data-stu-id="cd6f3-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="cd6f3-407">고유한 Microsoft Azure Active Directory 테 넌 트 ID를 GUID 형식으로 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-408">고객 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="cd6f3-409">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="cd6f3-411">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="cd6f3-412">이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="cd6f3-413">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-414">고객 국가</span><span class="sxs-lookup"><span data-stu-id="cd6f3-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="cd6f3-415">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-416">송장 번호</span><span class="sxs-lookup"><span data-stu-id="cd6f3-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="cd6f3-417">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="cd6f3-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-418">MpnId</span></span></td>
<td><p><span data-ttu-id="cd6f3-419">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-420">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="cd6f3-421">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-422">주문 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-422">Order ID</span></span></td>
<td><p><span data-ttu-id="cd6f3-423">Microsoft commerce platform은 주문에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="cd6f3-424">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-425">주문 날짜</span><span class="sxs-lookup"><span data-stu-id="cd6f3-425">Order date</span></span></td>
<td><p><span data-ttu-id="cd6f3-426">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-427">ProductId</span></span></td>
<td><p><span data-ttu-id="cd6f3-428">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-429">SkuId</span></span></td>
<td><p><span data-ttu-id="cd6f3-430">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="cd6f3-432">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-432">The ID for a particular Availability.</span></span> <span data-ttu-id="cd6f3-433">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-434">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="cd6f3-435">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-436">제품 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-436">Product name</span></span></td>
<td><p><span data-ttu-id="cd6f3-437">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="cd6f3-439">제품의 게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="cd6f3-441">이 게시자에 대 한 고유 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-442">구독 설명</span><span class="sxs-lookup"><span data-stu-id="cd6f3-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="cd6f3-443">구독의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-444">구독 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="cd6f3-445">Microsoft commerce platform은 구독에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="cd6f3-446">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="cd6f3-447">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-449">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-449">Start day of the charges.</span></span> <span data-ttu-id="cd6f3-450">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-452">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-452">End day of the charges.</span></span> <span data-ttu-id="cd6f3-453">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-454">용어 및 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="cd6f3-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="cd6f3-455">기간 및 구매에 대 한 청구 주기입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="cd6f3-456">예를 들어, "1 년, 월."</span><span class="sxs-lookup"><span data-stu-id="cd6f3-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-457">청구 유형</span><span class="sxs-lookup"><span data-stu-id="cd6f3-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="cd6f3-458">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-459">Unit Price</span><span class="sxs-lookup"><span data-stu-id="cd6f3-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="cd6f3-460">구매 시 게시 된 가격표의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cd6f3-461">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-462">효과적인 단가</span><span class="sxs-lookup"><span data-stu-id="cd6f3-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="cd6f3-463">단위 가격 조정을 만든 후입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-464">수량</span><span class="sxs-lookup"><span data-stu-id="cd6f3-464">Quantity</span></span></td>
<td><p><span data-ttu-id="cd6f3-465">단위 수입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-465">Number of units.</span></span> <span data-ttu-id="cd6f3-466">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-467">단위 형식</span><span class="sxs-lookup"><span data-stu-id="cd6f3-467">Unit type</span></span></td>
<td><p><span data-ttu-id="cd6f3-468">구매 되는 단위의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="cd6f3-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="cd6f3-470">적용 가능한 할인을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-471">Sub Total</span><span class="sxs-lookup"><span data-stu-id="cd6f3-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="cd6f3-472">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-472">Total before tax.</span></span> <span data-ttu-id="cd6f3-473">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-474">세금 합계</span><span class="sxs-lookup"><span data-stu-id="cd6f3-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="cd6f3-475">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-476">Total</span><span class="sxs-lookup"><span data-stu-id="cd6f3-476">Total</span></span></td>
<td><p><span data-ttu-id="cd6f3-477">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-477">Total after tax.</span></span> <span data-ttu-id="cd6f3-478">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-479">Currency</span><span class="sxs-lookup"><span data-stu-id="cd6f3-479">Currency</span></span></td>
<td><p><span data-ttu-id="cd6f3-480">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-480">Currency type.</span></span> <span data-ttu-id="cd6f3-481">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="cd6f3-482">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="cd6f3-484">대체 식별자에는 주문 id입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-484">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="cd6f3-485">매일 배분 사용 현황 파일 필드</span><span class="sxs-lookup"><span data-stu-id="cd6f3-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="cd6f3-486">Column</span><span class="sxs-lookup"><span data-stu-id="cd6f3-486">Column</span></span></th>
<th><span data-ttu-id="cd6f3-487">설명</span><span class="sxs-lookup"><span data-stu-id="cd6f3-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="cd6f3-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="cd6f3-489">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="cd6f3-491">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="cd6f3-493">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="cd6f3-495">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="cd6f3-496">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="cd6f3-498">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-498">The customer’s domain name.</span></span> <span data-ttu-id="cd6f3-499">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-500">고객 국가</span><span class="sxs-lookup"><span data-stu-id="cd6f3-500">Customer country</span></span></td>
<td><p><span data-ttu-id="cd6f3-501">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-502">MPNID</span></span></td>
<td><p><span data-ttu-id="cd6f3-503">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-504">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="cd6f3-505">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="cd6f3-506">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="cd6f3-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="cd6f3-508">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="cd6f3-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="cd6f3-509">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-510">ProductId</span></span></td>
<td><p><span data-ttu-id="cd6f3-511">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-512">SkuId</span></span></td>
<td><p><span data-ttu-id="cd6f3-513">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="cd6f3-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="cd6f3-515">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-515">The ID for a particular Availability.</span></span> <span data-ttu-id="cd6f3-516">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-517">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="cd6f3-518">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="cd6f3-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="cd6f3-520">게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="cd6f3-522">GUID 형식으로 게시자의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="cd6f3-523">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="cd6f3-524">구독 설명</span><span class="sxs-lookup"><span data-stu-id="cd6f3-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="cd6f3-525">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="cd6f3-526">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-527">구독 ID</span><span class="sxs-lookup"><span data-stu-id="cd6f3-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="cd6f3-528">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="cd6f3-529">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="cd6f3-530">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-532">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="cd6f3-533">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="cd6f3-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="cd6f3-535">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="cd6f3-536">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-537">사용 날짜</span><span class="sxs-lookup"><span data-stu-id="cd6f3-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="cd6f3-538">서비스 사용의 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-539">미터 종류</span><span class="sxs-lookup"><span data-stu-id="cd6f3-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="cd6f3-540">측정기의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-541">미터 범주</span><span class="sxs-lookup"><span data-stu-id="cd6f3-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="cd6f3-542">사용에 대 한 최상위 수준 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-543">미터 Id</span><span class="sxs-lookup"><span data-stu-id="cd6f3-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="cd6f3-544">사용 중인 미터에 대 한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-545">미터 하위 범주</span><span class="sxs-lookup"><span data-stu-id="cd6f3-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="cd6f3-546">속도 영향을 줄 수 있는 Azure 서비스의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-547">미터 이름</span><span class="sxs-lookup"><span data-stu-id="cd6f3-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="cd6f3-548">사용 중인 미터에 대 한 측정 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-549">요금제 지역</span><span class="sxs-lookup"><span data-stu-id="cd6f3-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="cd6f3-550">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-551">단위</span><span class="sxs-lookup"><span data-stu-id="cd6f3-551">Unit</span></span></td>
<td><p><span data-ttu-id="cd6f3-552">단위 리소스 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-553">사용한 수량</span><span class="sxs-lookup"><span data-stu-id="cd6f3-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="cd6f3-554">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="cd6f3-555">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-556">리소스 위치</span><span class="sxs-lookup"><span data-stu-id="cd6f3-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="cd6f3-557">측정기 실행 되 고 있는 데이터 센터입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-558">사용 되는 서비스</span><span class="sxs-lookup"><span data-stu-id="cd6f3-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="cd6f3-559">사용한 Azure 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-560">리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="cd6f3-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="cd6f3-561">배포 된 측정기 실행 되는 리소스 그룹입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-562">리소스 URI</span><span class="sxs-lookup"><span data-stu-id="cd6f3-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="cd6f3-563">사용 중인 리소스의 URI입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-564">청구 유형</span><span class="sxs-lookup"><span data-stu-id="cd6f3-564">Charge type</span></span></td>
<td><p><span data-ttu-id="cd6f3-565">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-565">The type of charge or adjustment.</span></span> <span data-ttu-id="cd6f3-566">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-567">단가</span><span class="sxs-lookup"><span data-stu-id="cd6f3-567">Unit price</span></span></td>
<td><p><span data-ttu-id="cd6f3-568">라이선스를 구매 시 가격표를 게시 하는 대로 당 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="cd6f3-569">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-570">수량</span><span class="sxs-lookup"><span data-stu-id="cd6f3-570">Quantity</span></span></td>
<td><p><span data-ttu-id="cd6f3-571">라이선스의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-571">Number of licenses.</span></span> <span data-ttu-id="cd6f3-572">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-573">단위 형식</span><span class="sxs-lookup"><span data-stu-id="cd6f3-573">Unit type</span></span></td>
<td><p><span data-ttu-id="cd6f3-574">측정기 요금이 청구 되는 단위의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="cd6f3-575">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-576">청구 전 세금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="cd6f3-577">세금 전에 총 공간입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-578">청구 통화</span><span class="sxs-lookup"><span data-stu-id="cd6f3-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="cd6f3-579">고객의 지리적 지역에 통화</span><span class="sxs-lookup"><span data-stu-id="cd6f3-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-580">세금 공제 전 가격 책정 요약</span><span class="sxs-lookup"><span data-stu-id="cd6f3-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="cd6f3-581">가격 책정 세금 추가 되기 전에 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-582">통화 가격 책정</span><span class="sxs-lookup"><span data-stu-id="cd6f3-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="cd6f3-583">가격표에서 통화입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-584">서비스 정보 1</span><span class="sxs-lookup"><span data-stu-id="cd6f3-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="cd6f3-585">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="cd6f3-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-586">서비스 정보 2</span><span class="sxs-lookup"><span data-stu-id="cd6f3-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="cd6f3-587">선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="cd6f3-588">Tags</span><span class="sxs-lookup"><span data-stu-id="cd6f3-588">Tags</span></span></td>
<td><p><span data-ttu-id="cd6f3-589">청구 레코드를 그룹화 하려면 측정기에 할당 하는 태그입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="cd6f3-590">예를 들어를 측정기를 사용 하는 부서에서 비용을 배분 하는데 태그를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="cd6f3-591">추가 정보</span><span class="sxs-lookup"><span data-stu-id="cd6f3-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="cd6f3-592">다른 열에서 다루지 않는 추가 정보.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="cd6f3-593">청구서 및 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="cd6f3-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="cd6f3-594">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="cd6f3-595">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="cd6f3-596">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="cd6f3-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="cd6f3-597">송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="cd6f3-598">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="cd6f3-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="cd6f3-599"><strong>청구서 금액 충전 설명</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-600"><strong>조정 파일 금액 설명 (ChargeType 열)</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-601"><strong>이 요금 이란 무엇 인가요?</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-602"><strong>이러한 ChargeTypes를 청구서에 매핑하려면 어떻게 하나요?</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="cd6f3-603"><strong>라이선스 기반 요금</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-604">활성화 수수료</span><span class="sxs-lookup"><span data-stu-id="cd6f3-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-605">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="cd6f3-606">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-607">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="cd6f3-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-608">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-609">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="cd6f3-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-610">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-611">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="cd6f3-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-612">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-613">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-614">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="cd6f3-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-615">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-616">연간 청구를 사용 하는 경우 구독에 대 한 요금 유형</span><span class="sxs-lookup"><span data-stu-id="cd6f3-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-617">구매 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-618">월 청구 비용은 사용 하는 경우 구독에 대 한 요금 유형</span><span class="sxs-lookup"><span data-stu-id="cd6f3-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-619">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-620">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="cd6f3-621">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-622">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-623">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-624">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="cd6f3-625"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-626">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-627">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="cd6f3-628">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-629">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-630">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-631"><strong>크레딧</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-632">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="cd6f3-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-633">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="cd6f3-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-634">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="cd6f3-635">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="cd6f3-636"><strong>사용량 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-637">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-638">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="cd6f3-639">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-640">주기 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-641">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-642">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-643">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-644">취소 할인</span><span class="sxs-lookup"><span data-stu-id="cd6f3-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-645">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="cd6f3-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="cd6f3-646"><strong>라이선스 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-647"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="cd6f3-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-648">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="cd6f3-649"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="cd6f3-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-650"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="cd6f3-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="cd6f3-651"><em>예외: &quot;품목 요금 차감&quot; 이미 세금이 포함 되어 있습니다. 위의 크레딧을 참조 하세요.</em></span><span class="sxs-lookup"><span data-stu-id="cd6f3-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-652">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="cd6f3-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="cd6f3-653">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="cd6f3-654">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="cd6f3-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
