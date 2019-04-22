---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 7022f1e3d26751e66f90db96bf6d881cb2a694d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/18/2019
ms.locfileid: "59430202"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="2ac9f-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="2ac9f-103">Use the reconciliation files</span></span>

<span data-ttu-id="2ac9f-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="2ac9f-104">**Applies to**</span></span>

-  <span data-ttu-id="2ac9f-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="2ac9f-105">Partner Center</span></span>
-  <span data-ttu-id="2ac9f-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="2ac9f-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="2ac9f-107">각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="2ac9f-108">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="2ac9f-109">서식 지정 문제</span><span class="sxs-lookup"><span data-stu-id="2ac9f-109">Formatting issues</span></span>

<span data-ttu-id="2ac9f-110">경우에 따라 여러 파일에 서식 지정 문제 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="2ac9f-111">(이 경우 발생할 수 있습니다, 예를 들어 EN-US 로캘을 사용 되지 않습니다.) 이러한 문제를 해결 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="2ac9f-112">Excel에서.csv 파일을 열고 첫 번째 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="2ac9f-113">리본에서 선택 <strong>데이터</strong>를 선택한 후 <strong>열에 텍스트</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="2ac9f-114">텍스트 변환 마법사에서에서 선택 <strong>파일 형식을 구분</strong>를 선택한 후 <strong>다음</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="2ac9f-115">구분 기호 필드에서 선택 <strong>쉼표로</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="2ac9f-116">하는 경우 <strong>탭</strong> 은 이미 선택 상태로 남겨둘 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="2ac9f-117"><strong>다음</strong>을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="2ac9f-118">열 데이터 형식 필드에서 선택 <strong>날짜: MDY</strong>를 선택한 후 <strong>다음</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="2ac9f-119">열 데이터 형식 필드에서 선택 <strong>텍스트</strong> 열을 선택한 후 모든 금액에 대 한 <strong>마침</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="2ac9f-120">파트너가 항목별로 정리</span><span class="sxs-lookup"><span data-stu-id="2ac9f-120">Itemize by partner</span></span>


<span data-ttu-id="2ac9f-121">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 모두 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2ac9f-122">MPN ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-122">MPN ID</span></span></th>
<th><span data-ttu-id="2ac9f-123">설명</span><span class="sxs-lookup"><span data-stu-id="2ac9f-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2ac9f-124">MPN ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="2ac9f-125">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-126">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="2ac9f-127">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="2ac9f-128">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2ac9f-129">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="2ac9f-130">eTo 확인 하거나 업데이트 대리점에서 파트너 센터 메뉴에서 선택 <strong>고객</strong>, 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="2ac9f-131">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="2ac9f-132"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="2ac9f-133">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="2ac9f-134">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="2ac9f-135">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="2ac9f-136">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="2ac9f-136">License-based file fields</span></span>


<span data-ttu-id="2ac9f-137">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2ac9f-138"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-138"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="2ac9f-139"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-139"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="2ac9f-140"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-140"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="2ac9f-142">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="2ac9f-143">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="2ac9f-144">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="2ac9f-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="2ac9f-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="2ac9f-147">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="2ac9f-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="2ac9f-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-149">OrderID</span></span></td>
<td><p><span data-ttu-id="2ac9f-150">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2ac9f-151">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="2ac9f-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="2ac9f-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="2ac9f-154">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2ac9f-155">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="2ac9f-156">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="2ac9f-157">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="2ac9f-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="2ac9f-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="2ac9f-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="2ac9f-160">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="2ac9f-161">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="2ac9f-162">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="2ac9f-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="2ac9f-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-164">OfferID</span></span></td>
<td><p><span data-ttu-id="2ac9f-165">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-165">Unique offer ID.</span></span> <span data-ttu-id="2ac9f-166">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="2ac9f-167"><b>참고</b>: 이 값은 가격 목록에서 제품 ID를 일치 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="2ac9f-168">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="2ac9f-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="2ac9f-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="2ac9f-171">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="2ac9f-172"><b>참고</b>: 이 값에는 가격 목록에서 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="2ac9f-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="2ac9f-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-174">OfferName</span></span></td>
<td><p><span data-ttu-id="2ac9f-175">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="2ac9f-176">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="2ac9f-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-178">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="2ac9f-179">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="2ac9f-180">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2ac9f-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2ac9f-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-183">구독 종료 날짜: 12 개월 + x 일 후 시작 날짜 (종료 날짜를 청구 하는 파트너와 맞춤) 또는 갱신 날짜 로부터 12 개월입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="2ac9f-184">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="2ac9f-185">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="2ac9f-186">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2ac9f-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2ac9f-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-189">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="2ac9f-190">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="2ac9f-191">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2ac9f-192">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2ac9f-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-194">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="2ac9f-195">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="2ac9f-196">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="2ac9f-197">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="2ac9f-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2ac9f-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="2ac9f-199">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-199">The type of charge or adjustment.</span></span> <span data-ttu-id="2ac9f-200"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="2ac9f-201"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="2ac9f-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="2ac9f-203">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2ac9f-204">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="2ac9f-205">6.82</span><span class="sxs-lookup"><span data-stu-id="2ac9f-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-206">수량</span><span class="sxs-lookup"><span data-stu-id="2ac9f-206">Quantity</span></span></td>
<td><p><span data-ttu-id="2ac9f-207">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-207">Number of seats.</span></span> <span data-ttu-id="2ac9f-208">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="2ac9f-209">2</span><span class="sxs-lookup"><span data-stu-id="2ac9f-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-210">Amount</span><span class="sxs-lookup"><span data-stu-id="2ac9f-210">Amount</span></span></td>
<td><p><span data-ttu-id="2ac9f-211">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-211">Total of price for quantity.</span></span> <span data-ttu-id="2ac9f-212">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="2ac9f-213">13.32</span><span class="sxs-lookup"><span data-stu-id="2ac9f-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="2ac9f-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="2ac9f-215">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="2ac9f-216">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="2ac9f-217">2.32</span><span class="sxs-lookup"><span data-stu-id="2ac9f-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-218">Subtotal</span><span class="sxs-lookup"><span data-stu-id="2ac9f-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="2ac9f-219">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-219">Total before tax.</span></span> <span data-ttu-id="2ac9f-220">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="2ac9f-221">11</span><span class="sxs-lookup"><span data-stu-id="2ac9f-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-222">Tax</span><span class="sxs-lookup"><span data-stu-id="2ac9f-222">Tax</span></span></td>
<td><p><span data-ttu-id="2ac9f-223">세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="2ac9f-224">0</span><span class="sxs-lookup"><span data-stu-id="2ac9f-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="2ac9f-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="2ac9f-226">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-226">Total after tax.</span></span> <span data-ttu-id="2ac9f-227">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="2ac9f-228">11</span><span class="sxs-lookup"><span data-stu-id="2ac9f-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-229">Currency</span><span class="sxs-lookup"><span data-stu-id="2ac9f-229">Currency</span></span></td>
<td><p><span data-ttu-id="2ac9f-230">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-230">Currency type.</span></span> <span data-ttu-id="2ac9f-231">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="2ac9f-232">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="2ac9f-233">EUR</span><span class="sxs-lookup"><span data-stu-id="2ac9f-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="2ac9f-235">고객&#39;파트너 센터에 보고 된 s 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="2ac9f-236">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="2ac9f-237">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="2ac9f-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-238">MPNID</span></span></td>
<td><p><span data-ttu-id="2ac9f-239">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="2ac9f-240">4390934</span><span class="sxs-lookup"><span data-stu-id="2ac9f-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="2ac9f-242">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2ac9f-243"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="2ac9f-244">4390934</span><span class="sxs-lookup"><span data-stu-id="2ac9f-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-245">DomainName</span></span></td>
<td><p><span data-ttu-id="2ac9f-246">고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="2ac9f-247">이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="2ac9f-248">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="2ac9f-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2ac9f-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="2ac9f-251">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-251">Subscription nickname.</span></span> <span data-ttu-id="2ac9f-252">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="2ac9f-253">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="2ac9f-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="2ac9f-255">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="2ac9f-256">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="2ac9f-257">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="2ac9f-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="2ac9f-258">사용량 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="2ac9f-258">Usage-based file fields</span></span>


<span data-ttu-id="2ac9f-259">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="2ac9f-260">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2ac9f-261"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-261"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="2ac9f-262"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-262"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="2ac9f-263"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-263"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="2ac9f-265">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="2ac9f-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="2ac9f-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="2ac9f-268">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="2ac9f-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="2ac9f-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="2ac9f-271">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="2ac9f-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="2ac9f-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="2ac9f-274">고객&#39;파트너 센터에 보고 된 s 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="2ac9f-275">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="2ac9f-276">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="2ac9f-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-277">MPNID</span></span></td>
<td><p><span data-ttu-id="2ac9f-278">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="2ac9f-279">4390934</span><span class="sxs-lookup"><span data-stu-id="2ac9f-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="2ac9f-281">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2ac9f-282"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="2ac9f-283">4390934</span><span class="sxs-lookup"><span data-stu-id="2ac9f-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="2ac9f-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="2ac9f-285">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="2ac9f-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="2ac9f-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="2ac9f-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-288">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="2ac9f-289">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2ac9f-290">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="2ac9f-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-292">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="2ac9f-293">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="2ac9f-294">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="2ac9f-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="2ac9f-296">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2ac9f-297">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="2ac9f-298">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="2ac9f-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="2ac9f-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="2ac9f-301">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="2ac9f-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2ac9f-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="2ac9f-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="2ac9f-304">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="2ac9f-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="2ac9f-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2ac9f-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-306">OrderID</span></span></td>
<td><p><span data-ttu-id="2ac9f-307">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2ac9f-308">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="2ac9f-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="2ac9f-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="2ac9f-311">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="2ac9f-312">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="2ac9f-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="2ac9f-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="2ac9f-314">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="2ac9f-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="2ac9f-315">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="2ac9f-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="2ac9f-316">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="2ac9f-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="2ac9f-318">모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="2ac9f-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="2ac9f-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="2ac9f-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-320">Resource Name</span><span class="sxs-lookup"><span data-stu-id="2ac9f-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="2ac9f-321">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="2ac9f-322">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="2ac9f-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="2ac9f-323">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="2ac9f-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-324">Region</span><span class="sxs-lookup"><span data-stu-id="2ac9f-324">Region</span></span></td>
<td><p><span data-ttu-id="2ac9f-325">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-325">The region the usage applies to.</span></span> <span data-ttu-id="2ac9f-326">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="2ac9f-327">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="2ac9f-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-328">SKU</span><span class="sxs-lookup"><span data-stu-id="2ac9f-328">SKU</span></span></td>
<td><p><span data-ttu-id="2ac9f-329">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="2ac9f-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="2ac9f-330">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="2ac9f-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="2ac9f-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="2ac9f-332">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="2ac9f-333">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="2ac9f-334">1</span><span class="sxs-lookup"><span data-stu-id="2ac9f-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="2ac9f-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="2ac9f-336">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="2ac9f-337">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="2ac9f-338">11</span><span class="sxs-lookup"><span data-stu-id="2ac9f-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="2ac9f-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="2ac9f-340">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-340">Units included as part of the offer.</span></span> <span data-ttu-id="2ac9f-341">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="2ac9f-342">0</span><span class="sxs-lookup"><span data-stu-id="2ac9f-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="2ac9f-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="2ac9f-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="2ac9f-344">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="2ac9f-345">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="2ac9f-346">11</span><span class="sxs-lookup"><span data-stu-id="2ac9f-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="2ac9f-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="2ac9f-348">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="2ac9f-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="2ac9f-349">$0.0808</span><span class="sxs-lookup"><span data-stu-id="2ac9f-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="2ac9f-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="2ac9f-351">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2ac9f-352">$0.085</span><span class="sxs-lookup"><span data-stu-id="2ac9f-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="2ac9f-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="2ac9f-354">세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="2ac9f-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="2ac9f-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="2ac9f-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="2ac9f-357">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="2ac9f-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="2ac9f-358">$0.93</span><span class="sxs-lookup"><span data-stu-id="2ac9f-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-359">Currency</span><span class="sxs-lookup"><span data-stu-id="2ac9f-359">Currency</span></span></td>
<td><p><span data-ttu-id="2ac9f-360">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-360">Currency type.</span></span> <span data-ttu-id="2ac9f-361">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="2ac9f-362">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="2ac9f-363">EUR</span><span class="sxs-lookup"><span data-stu-id="2ac9f-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="2ac9f-365">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-365">Pretax price per unit.</span></span> <span data-ttu-id="2ac9f-366">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2ac9f-367">$0.08</span><span class="sxs-lookup"><span data-stu-id="2ac9f-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="2ac9f-369">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-369">Post tax price per unit.</span></span> <span data-ttu-id="2ac9f-370">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2ac9f-371">$0.08</span><span class="sxs-lookup"><span data-stu-id="2ac9f-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2ac9f-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="2ac9f-373">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-373">The type of charge or adjustment.</span></span> <span data-ttu-id="2ac9f-374"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="2ac9f-375"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="2ac9f-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="2ac9f-377">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="2ac9f-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="2ac9f-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-380">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="2ac9f-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="2ac9f-381">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="2ac9f-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="2ac9f-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="2ac9f-383">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="2ac9f-384">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="2ac9f-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="2ac9f-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="2ac9f-386">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="2ac9f-387">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="2ac9f-388">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="2ac9f-389">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="2ac9f-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="2ac9f-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="2ac9f-391">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="2ac9f-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="2ac9f-392">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="2ac9f-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-393">프로젝트</span><span class="sxs-lookup"><span data-stu-id="2ac9f-393">Project</span></span></td>
<td><p><span data-ttu-id="2ac9f-394">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="2ac9f-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="2ac9f-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="2ac9f-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="2ac9f-397">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="2ac9f-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="2ac9f-398">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="2ac9f-399">해당 날짜에 대 한 일일 사용량 명세서 477860 경우 프로 비전 하는 service Bus 연결 25 팩 있고 해당 일 동안 1을 사용 하면, "25 개 연결 / 30 일 – 사용: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="2ac9f-401">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="2ac9f-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="2ac9f-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2ac9f-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-403">DomainName</span></span></td>
<td><p><span data-ttu-id="2ac9f-404">고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="2ac9f-405">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="2ac9f-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2ac9f-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="2ac9f-407">단위</span><span class="sxs-lookup"><span data-stu-id="2ac9f-407">Unit</span></span></td>
<td><p><span data-ttu-id="2ac9f-408">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="2ac9f-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="2ac9f-409">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="2ac9f-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="2ac9f-410">일회성 및 되풀이 파일 필드</span><span class="sxs-lookup"><span data-stu-id="2ac9f-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2ac9f-411">Column</span><span class="sxs-lookup"><span data-stu-id="2ac9f-411">Column</span></span></th>
<th><span data-ttu-id="2ac9f-412">설명</span><span class="sxs-lookup"><span data-stu-id="2ac9f-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="2ac9f-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="2ac9f-414">특정 청구 엔터티 GUID 형식에서에 대 한 고유한 Microsoft Azure Active Directory 테 넌 트 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="2ac9f-415">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="2ac9f-416">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-417">Customer Id</span><span class="sxs-lookup"><span data-stu-id="2ac9f-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="2ac9f-418">고유한 Microsoft Azure Active Directory 테 넌 트 ID를 GUID 형식으로 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-419">고객 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="2ac9f-420">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="2ac9f-422">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="2ac9f-423">이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="2ac9f-424">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-425">고객 국가</span><span class="sxs-lookup"><span data-stu-id="2ac9f-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="2ac9f-426">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-427">송장 번호</span><span class="sxs-lookup"><span data-stu-id="2ac9f-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="2ac9f-428">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="2ac9f-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-429">MpnId</span></span></td>
<td><p><span data-ttu-id="2ac9f-430">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="2ac9f-432">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-433">주문 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-433">Order ID</span></span></td>
<td><p><span data-ttu-id="2ac9f-434">Microsoft commerce platform은 주문에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="2ac9f-435">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-436">주문 날짜</span><span class="sxs-lookup"><span data-stu-id="2ac9f-436">Order date</span></span></td>
<td><p><span data-ttu-id="2ac9f-437">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-438">ProductId</span></span></td>
<td><p><span data-ttu-id="2ac9f-439">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-440">SkuId</span></span></td>
<td><p><span data-ttu-id="2ac9f-441">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="2ac9f-443">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-443">The ID for a particular Availability.</span></span> <span data-ttu-id="2ac9f-444">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-445">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="2ac9f-446">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-447">제품 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-447">Product name</span></span></td>
<td><p><span data-ttu-id="2ac9f-448">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="2ac9f-450">제품의 게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="2ac9f-452">이 게시자에 대 한 고유 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-453">구독 설명</span><span class="sxs-lookup"><span data-stu-id="2ac9f-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="2ac9f-454">구독의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-455">구독 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="2ac9f-456">Microsoft commerce platform은 구독에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="2ac9f-457">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="2ac9f-458">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-460">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-460">Start day of the charges.</span></span> <span data-ttu-id="2ac9f-461">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-463">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-463">End day of the charges.</span></span> <span data-ttu-id="2ac9f-464">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-465">용어 및 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="2ac9f-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="2ac9f-466">기간 및 구매에 대 한 청구 주기입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="2ac9f-467">예를 들어, "1 년, 월."</span><span class="sxs-lookup"><span data-stu-id="2ac9f-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-468">청구 유형</span><span class="sxs-lookup"><span data-stu-id="2ac9f-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="2ac9f-469">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-470">Unit Price</span><span class="sxs-lookup"><span data-stu-id="2ac9f-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="2ac9f-471">구매 시 게시 된 가격표의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2ac9f-472">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-473">효과적인 단가</span><span class="sxs-lookup"><span data-stu-id="2ac9f-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="2ac9f-474">단위 가격 조정을 만든 후입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-475">수량</span><span class="sxs-lookup"><span data-stu-id="2ac9f-475">Quantity</span></span></td>
<td><p><span data-ttu-id="2ac9f-476">단위 수입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-476">Number of units.</span></span> <span data-ttu-id="2ac9f-477">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-478">단위 형식</span><span class="sxs-lookup"><span data-stu-id="2ac9f-478">Unit type</span></span></td>
<td><p><span data-ttu-id="2ac9f-479">구매 되는 단위의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="2ac9f-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="2ac9f-481">적용 가능한 할인을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-482">Sub Total</span><span class="sxs-lookup"><span data-stu-id="2ac9f-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="2ac9f-483">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-483">Total before tax.</span></span> <span data-ttu-id="2ac9f-484">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-485">세금 합계</span><span class="sxs-lookup"><span data-stu-id="2ac9f-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="2ac9f-486">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-487">Total</span><span class="sxs-lookup"><span data-stu-id="2ac9f-487">Total</span></span></td>
<td><p><span data-ttu-id="2ac9f-488">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-488">Total after tax.</span></span> <span data-ttu-id="2ac9f-489">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-490">Currency</span><span class="sxs-lookup"><span data-stu-id="2ac9f-490">Currency</span></span></td>
<td><p><span data-ttu-id="2ac9f-491">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-491">Currency type.</span></span> <span data-ttu-id="2ac9f-492">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="2ac9f-493">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="2ac9f-495">대체 식별자에는 주문 id입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="2ac9f-496">매일 배분 사용 현황 파일 필드</span><span class="sxs-lookup"><span data-stu-id="2ac9f-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2ac9f-497">Column</span><span class="sxs-lookup"><span data-stu-id="2ac9f-497">Column</span></span></th>
<th><span data-ttu-id="2ac9f-498">설명</span><span class="sxs-lookup"><span data-stu-id="2ac9f-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="2ac9f-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="2ac9f-500">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="2ac9f-502">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="2ac9f-504">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="2ac9f-506">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="2ac9f-507">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="2ac9f-509">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-509">The customer’s domain name.</span></span> <span data-ttu-id="2ac9f-510">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-511">고객 국가</span><span class="sxs-lookup"><span data-stu-id="2ac9f-511">Customer country</span></span></td>
<td><p><span data-ttu-id="2ac9f-512">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-513">MPNID</span></span></td>
<td><p><span data-ttu-id="2ac9f-514">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-515">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="2ac9f-516">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2ac9f-517">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="2ac9f-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="2ac9f-519">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="2ac9f-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="2ac9f-520">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-521">ProductId</span></span></td>
<td><p><span data-ttu-id="2ac9f-522">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-523">SkuId</span></span></td>
<td><p><span data-ttu-id="2ac9f-524">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="2ac9f-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="2ac9f-526">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-526">The ID for a particular Availability.</span></span> <span data-ttu-id="2ac9f-527">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-528">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="2ac9f-529">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="2ac9f-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="2ac9f-531">게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="2ac9f-533">GUID 형식으로 게시자의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="2ac9f-534">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="2ac9f-535">구독 설명</span><span class="sxs-lookup"><span data-stu-id="2ac9f-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="2ac9f-536">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="2ac9f-537">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-538">구독 ID</span><span class="sxs-lookup"><span data-stu-id="2ac9f-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="2ac9f-539">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2ac9f-540">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="2ac9f-541">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-543">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="2ac9f-544">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2ac9f-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2ac9f-546">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="2ac9f-547">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-548">사용 날짜</span><span class="sxs-lookup"><span data-stu-id="2ac9f-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="2ac9f-549">서비스 사용의 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-550">미터 종류</span><span class="sxs-lookup"><span data-stu-id="2ac9f-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="2ac9f-551">측정기의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-552">미터 범주</span><span class="sxs-lookup"><span data-stu-id="2ac9f-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="2ac9f-553">사용에 대 한 최상위 수준 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-554">미터 Id</span><span class="sxs-lookup"><span data-stu-id="2ac9f-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="2ac9f-555">사용 중인 미터에 대 한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-556">미터 하위 범주</span><span class="sxs-lookup"><span data-stu-id="2ac9f-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="2ac9f-557">속도 영향을 줄 수 있는 Azure 서비스의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-558">미터 이름</span><span class="sxs-lookup"><span data-stu-id="2ac9f-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="2ac9f-559">사용 중인 미터에 대 한 측정 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-560">요금제 지역</span><span class="sxs-lookup"><span data-stu-id="2ac9f-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="2ac9f-561">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-562">단위</span><span class="sxs-lookup"><span data-stu-id="2ac9f-562">Unit</span></span></td>
<td><p><span data-ttu-id="2ac9f-563">단위 리소스 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-564">사용한 수량</span><span class="sxs-lookup"><span data-stu-id="2ac9f-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="2ac9f-565">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="2ac9f-566">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-567">리소스 위치</span><span class="sxs-lookup"><span data-stu-id="2ac9f-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="2ac9f-568">측정기 실행 되 고 있는 데이터 센터입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-569">사용 되는 서비스</span><span class="sxs-lookup"><span data-stu-id="2ac9f-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="2ac9f-570">사용한 Azure 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-571">리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="2ac9f-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="2ac9f-572">배포 된 측정기 실행 되는 리소스 그룹입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-573">리소스 URI</span><span class="sxs-lookup"><span data-stu-id="2ac9f-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="2ac9f-574">사용 중인 리소스의 URI입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-575">청구 유형</span><span class="sxs-lookup"><span data-stu-id="2ac9f-575">Charge type</span></span></td>
<td><p><span data-ttu-id="2ac9f-576">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-576">The type of charge or adjustment.</span></span> <span data-ttu-id="2ac9f-577">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-578">단가</span><span class="sxs-lookup"><span data-stu-id="2ac9f-578">Unit price</span></span></td>
<td><p><span data-ttu-id="2ac9f-579">라이선스를 구매 시 가격표를 게시 하는 대로 당 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2ac9f-580">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-581">수량</span><span class="sxs-lookup"><span data-stu-id="2ac9f-581">Quantity</span></span></td>
<td><p><span data-ttu-id="2ac9f-582">라이선스의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-582">Number of licenses.</span></span> <span data-ttu-id="2ac9f-583">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-584">단위 형식</span><span class="sxs-lookup"><span data-stu-id="2ac9f-584">Unit type</span></span></td>
<td><p><span data-ttu-id="2ac9f-585">측정기 요금이 청구 되는 단위의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="2ac9f-586">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-587">청구 전 세금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="2ac9f-588">세금 전에 총 공간입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-589">청구 통화</span><span class="sxs-lookup"><span data-stu-id="2ac9f-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="2ac9f-590">고객의 지리적 지역에 통화</span><span class="sxs-lookup"><span data-stu-id="2ac9f-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-591">세금 공제 전 가격 책정 요약</span><span class="sxs-lookup"><span data-stu-id="2ac9f-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="2ac9f-592">가격 책정 세금 추가 되기 전에 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-593">통화 가격 책정</span><span class="sxs-lookup"><span data-stu-id="2ac9f-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="2ac9f-594">가격표에서 통화입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-595">서비스 정보 1</span><span class="sxs-lookup"><span data-stu-id="2ac9f-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="2ac9f-596">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="2ac9f-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-597">서비스 정보 2</span><span class="sxs-lookup"><span data-stu-id="2ac9f-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="2ac9f-598">선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2ac9f-599">Tags</span><span class="sxs-lookup"><span data-stu-id="2ac9f-599">Tags</span></span></td>
<td><p><span data-ttu-id="2ac9f-600">청구 레코드를 그룹화 하려면 측정기에 할당 하는 태그입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="2ac9f-601">예를 들어를 측정기를 사용 하는 부서에서 비용을 배분 하는데 태그를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2ac9f-602">추가 정보</span><span class="sxs-lookup"><span data-stu-id="2ac9f-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="2ac9f-603">다른 열에서 다루지 않는 추가 정보.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="2ac9f-604">청구서 및 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="2ac9f-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="2ac9f-605">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="2ac9f-606">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="2ac9f-607">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="2ac9f-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="2ac9f-608">송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="2ac9f-609">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="2ac9f-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="2ac9f-610"><strong>청구서 금액 충전 설명</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-610"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-611"><strong>조정 파일 금액 설명 (ChargeType 열)</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-611"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-612"><strong>이 요금 이란 무엇 인가요?</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-612"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-613"><strong>이러한 ChargeTypes를 청구서에 매핑하려면 어떻게 하나요?</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-613"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="2ac9f-614"><strong>라이선스 기반 요금</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-614"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-615">활성화 수수료</span><span class="sxs-lookup"><span data-stu-id="2ac9f-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-616">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="2ac9f-617">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-618">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="2ac9f-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-619">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-620">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="2ac9f-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-621">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-622">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="2ac9f-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-623">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-624">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-625">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="2ac9f-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-626">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-627">연간 청구를 사용 하는 경우 구독에 대 한 요금 유형</span><span class="sxs-lookup"><span data-stu-id="2ac9f-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-628">구매 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-629">월 청구 비용은 사용 하는 경우 구독에 대 한 요금 유형</span><span class="sxs-lookup"><span data-stu-id="2ac9f-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-630">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-631">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="2ac9f-632">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-633">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-634">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-635">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="2ac9f-636"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-636"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-637">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-638">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="2ac9f-639">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-640">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-641">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-642"><strong>크레딧</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-642"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-643">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="2ac9f-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-644">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="2ac9f-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-645">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="2ac9f-646">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="2ac9f-647"><strong>사용량 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-647"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-648">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-649">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="2ac9f-650">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-651">주기 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-652">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-653">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-654">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-655">취소 할인</span><span class="sxs-lookup"><span data-stu-id="2ac9f-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-656">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="2ac9f-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="2ac9f-657"><strong>라이선스 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-657"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-658"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="2ac9f-658"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-659">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2ac9f-660"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="2ac9f-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-661"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="2ac9f-661"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="2ac9f-662"><em>예외: &quot;품목 요금 차감&quot; 이미 세금이 포함 되어 있습니다. 위의 크레딧을 참조 하세요.</em></span><span class="sxs-lookup"><span data-stu-id="2ac9f-662"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-663">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="2ac9f-663">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="2ac9f-664">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-664">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="2ac9f-665">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="2ac9f-665">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
