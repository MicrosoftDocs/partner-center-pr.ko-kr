---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 03/15/2019
description: 각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fca9897720412a77ac39c86ba31db411c58c2cb0
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343465"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="40882-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="40882-103">Use the reconciliation files</span></span>

<span data-ttu-id="40882-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="40882-104">**Applies to**</span></span>

-  <span data-ttu-id="40882-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="40882-105">Partner Center</span></span>
-  <span data-ttu-id="40882-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="40882-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="40882-107">각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="40882-108">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="40882-109">서식 지정 문제</span><span class="sxs-lookup"><span data-stu-id="40882-109">Formatting issues</span></span>

<span data-ttu-id="40882-110">경우에 따라 여러 파일에 서식 지정 문제 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="40882-111">(이 경우 발생할 수 있습니다, 예를 들어 EN-US 로캘을 사용 되지 않습니다.) 이러한 문제를 해결 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="40882-112">Excel에서.csv 파일을 열고 첫 번째 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="40882-113">리본에서 선택 <strong>데이터</strong>를 선택한 후 <strong>열에 텍스트</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="40882-114">텍스트 변환 마법사에서에서 선택 <strong>파일 형식을 구분</strong>를 선택한 후 <strong>다음</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="40882-115">구분 기호 필드에서 선택 <strong>쉼표로</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="40882-116">하는 경우 <strong>탭</strong> 은 이미 선택 상태로 남겨둘 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="40882-117"><strong>다음</strong>을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="40882-118">열 데이터 형식 필드에서 선택 <strong>날짜: MDY</strong>를 선택한 후 <strong>다음</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="40882-119">열 데이터 형식 필드에서 선택 <strong>텍스트</strong> 열을 선택한 후 모든 금액에 대 한 <strong>마침</strong>합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="40882-120">여러 큰 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="40882-120">Downloading a large recon file</span></span>

<span data-ttu-id="40882-121">모두 정찰 파일 크기가 매우 커질 수 및 다운로드 하기 어려운 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="40882-122">여러 큰 파일을 다운로드 하는 데 PowerShell 스크립트를 참조 하세요 [청구서 줄 항목 가져오기](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items)합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="40882-123">파트너가 항목별로 정리</span><span class="sxs-lookup"><span data-stu-id="40882-123">Itemize by partner</span></span>


<span data-ttu-id="40882-124">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 모두 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="40882-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="40882-125">MPN ID</span></span></th>
<th><span data-ttu-id="40882-126">설명</span><span class="sxs-lookup"><span data-stu-id="40882-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="40882-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="40882-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="40882-128">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="40882-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-129">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="40882-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="40882-130">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="40882-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="40882-131">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40882-132">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="40882-133">eTo 확인 하거나 업데이트 대리점에서 파트너 센터 메뉴에서 선택 <strong>고객</strong>, 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="40882-134">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="40882-135"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="40882-136">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="40882-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="40882-137">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="40882-138">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="40882-139">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="40882-139">License-based file fields</span></span>


<span data-ttu-id="40882-140">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="40882-141"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="40882-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="40882-142"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="40882-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="40882-143"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="40882-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="40882-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="40882-145">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="40882-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="40882-146">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="40882-147">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="40882-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="40882-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="40882-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="40882-150">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="40882-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="40882-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="40882-152">OrderID</span></span></td>
<td><p><span data-ttu-id="40882-153">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="40882-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="40882-154">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="40882-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="40882-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="40882-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="40882-157">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="40882-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="40882-158">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="40882-159">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="40882-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="40882-160">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="40882-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="40882-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="40882-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="40882-163">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="40882-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="40882-164">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="40882-165">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="40882-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="40882-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="40882-167">OfferID</span></span></td>
<td><p><span data-ttu-id="40882-168">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="40882-168">Unique offer ID.</span></span> <span data-ttu-id="40882-169">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="40882-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="40882-170"><b>참고</b>: 이 값은 가격 목록에서 제품 ID를 일치 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="40882-171">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="40882-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="40882-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="40882-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="40882-174">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="40882-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="40882-175"><b>참고</b>: 이 값에는 가격 목록에서 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="40882-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="40882-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="40882-177">OfferName</span></span></td>
<td><p><span data-ttu-id="40882-178">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="40882-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="40882-179">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="40882-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="40882-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="40882-181">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="40882-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="40882-182">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="40882-183">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40882-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="40882-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="40882-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="40882-186">구독 종료 날짜: 12 개월 + x 일 후 시작 날짜 (종료 날짜를 청구 하는 파트너와 맞춤) 또는 갱신 날짜 로부터 12 개월입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="40882-187">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="40882-188">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="40882-189">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40882-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="40882-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40882-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40882-192">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="40882-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="40882-193">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="40882-194">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40882-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="40882-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40882-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40882-197">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="40882-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="40882-198">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="40882-199">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="40882-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="40882-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="40882-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="40882-202">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="40882-202">The type of charge or adjustment.</span></span> <span data-ttu-id="40882-203"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="40882-204"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="40882-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="40882-206">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="40882-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="40882-207">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="40882-208">6.82</span><span class="sxs-lookup"><span data-stu-id="40882-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-209">수량</span><span class="sxs-lookup"><span data-stu-id="40882-209">Quantity</span></span></td>
<td><p><span data-ttu-id="40882-210">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="40882-210">Number of seats.</span></span> <span data-ttu-id="40882-211">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="40882-212">2</span><span class="sxs-lookup"><span data-stu-id="40882-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-213">Amount</span><span class="sxs-lookup"><span data-stu-id="40882-213">Amount</span></span></td>
<td><p><span data-ttu-id="40882-214">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="40882-214">Total of price for quantity.</span></span> <span data-ttu-id="40882-215">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="40882-216">13.32</span><span class="sxs-lookup"><span data-stu-id="40882-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="40882-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="40882-218">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="40882-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="40882-219">인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="40882-220">2.32</span><span class="sxs-lookup"><span data-stu-id="40882-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="40882-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="40882-222">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="40882-222">Total before tax.</span></span> <span data-ttu-id="40882-223">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="40882-224">11</span><span class="sxs-lookup"><span data-stu-id="40882-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-225">Tax</span><span class="sxs-lookup"><span data-stu-id="40882-225">Tax</span></span></td>
<td><p><span data-ttu-id="40882-226">세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="40882-227">0</span><span class="sxs-lookup"><span data-stu-id="40882-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="40882-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="40882-229">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="40882-229">Total after tax.</span></span> <span data-ttu-id="40882-230">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="40882-231">11</span><span class="sxs-lookup"><span data-stu-id="40882-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-232">Currency</span><span class="sxs-lookup"><span data-stu-id="40882-232">Currency</span></span></td>
<td><p><span data-ttu-id="40882-233">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="40882-233">Currency type.</span></span> <span data-ttu-id="40882-234">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="40882-235">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="40882-236">EUR</span><span class="sxs-lookup"><span data-stu-id="40882-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="40882-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="40882-238">고객&#39;파트너 센터에 보고 된 s 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="40882-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="40882-239">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="40882-240">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="40882-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="40882-241">MPNID</span></span></td>
<td><p><span data-ttu-id="40882-242">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="40882-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="40882-243">4390934</span><span class="sxs-lookup"><span data-stu-id="40882-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="40882-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="40882-245">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40882-246"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="40882-247">4390934</span><span class="sxs-lookup"><span data-stu-id="40882-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="40882-248">DomainName</span></span></td>
<td><p><span data-ttu-id="40882-249">고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="40882-250">이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="40882-251">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="40882-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="40882-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="40882-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="40882-254">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="40882-254">Subscription nickname.</span></span> <span data-ttu-id="40882-255">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="40882-256">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="40882-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="40882-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="40882-258">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="40882-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="40882-259">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="40882-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="40882-260">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="40882-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="40882-261">사용량 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="40882-261">Usage-based file fields</span></span>


<span data-ttu-id="40882-262">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="40882-263">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="40882-264"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="40882-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="40882-265"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="40882-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="40882-266"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="40882-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="40882-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="40882-268">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="40882-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="40882-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="40882-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="40882-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="40882-271">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="40882-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="40882-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="40882-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="40882-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="40882-274">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="40882-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="40882-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="40882-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="40882-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="40882-277">고객&#39;파트너 센터에 보고 된 s 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="40882-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="40882-278">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="40882-279">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="40882-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="40882-280">MPNID</span></span></td>
<td><p><span data-ttu-id="40882-281">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="40882-282">4390934</span><span class="sxs-lookup"><span data-stu-id="40882-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="40882-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="40882-284">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40882-285"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="40882-286">4390934</span><span class="sxs-lookup"><span data-stu-id="40882-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="40882-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="40882-288">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="40882-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="40882-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="40882-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40882-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40882-291">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="40882-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="40882-292">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="40882-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="40882-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40882-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40882-295">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="40882-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="40882-296">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="40882-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="40882-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="40882-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="40882-299">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="40882-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="40882-300">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="40882-301">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="40882-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="40882-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="40882-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="40882-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="40882-304">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="40882-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="40882-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="40882-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="40882-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="40882-307">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="40882-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="40882-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="40882-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="40882-309">OrderID</span></span></td>
<td><p><span data-ttu-id="40882-310">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="40882-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="40882-311">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="40882-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="40882-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="40882-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="40882-314">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="40882-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="40882-315">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="40882-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="40882-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="40882-317">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="40882-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="40882-318">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="40882-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="40882-319">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="40882-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="40882-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="40882-321">모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="40882-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="40882-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="40882-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="40882-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="40882-324">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="40882-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="40882-325">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="40882-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="40882-326">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="40882-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-327">Region</span><span class="sxs-lookup"><span data-stu-id="40882-327">Region</span></span></td>
<td><p><span data-ttu-id="40882-328">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-328">The region the usage applies to.</span></span> <span data-ttu-id="40882-329">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="40882-330">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="40882-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-331">SKU</span><span class="sxs-lookup"><span data-stu-id="40882-331">SKU</span></span></td>
<td><p><span data-ttu-id="40882-332">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="40882-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="40882-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="40882-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="40882-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="40882-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="40882-335">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="40882-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="40882-336">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="40882-337">1</span><span class="sxs-lookup"><span data-stu-id="40882-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="40882-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="40882-339">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="40882-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="40882-340">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="40882-341">11</span><span class="sxs-lookup"><span data-stu-id="40882-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="40882-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="40882-343">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="40882-343">Units included as part of the offer.</span></span> <span data-ttu-id="40882-344">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="40882-345">0</span><span class="sxs-lookup"><span data-stu-id="40882-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="40882-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="40882-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="40882-347">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="40882-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="40882-348">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="40882-349">11</span><span class="sxs-lookup"><span data-stu-id="40882-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="40882-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="40882-351">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="40882-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="40882-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="40882-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="40882-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="40882-354">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="40882-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="40882-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="40882-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="40882-357">세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="40882-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="40882-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="40882-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="40882-360">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="40882-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="40882-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="40882-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-362">Currency</span><span class="sxs-lookup"><span data-stu-id="40882-362">Currency</span></span></td>
<td><p><span data-ttu-id="40882-363">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="40882-363">Currency type.</span></span> <span data-ttu-id="40882-364">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="40882-365">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="40882-366">EUR</span><span class="sxs-lookup"><span data-stu-id="40882-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="40882-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="40882-368">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="40882-368">Pretax price per unit.</span></span> <span data-ttu-id="40882-369">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="40882-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="40882-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="40882-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="40882-372">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="40882-372">Post tax price per unit.</span></span> <span data-ttu-id="40882-373">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="40882-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="40882-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="40882-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="40882-376">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="40882-376">The type of charge or adjustment.</span></span> <span data-ttu-id="40882-377"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="40882-378"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="40882-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="40882-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="40882-380">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="40882-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="40882-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="40882-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="40882-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="40882-383">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="40882-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="40882-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="40882-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="40882-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="40882-386">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="40882-387">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="40882-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="40882-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="40882-389">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="40882-390">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="40882-391">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="40882-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="40882-392">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="40882-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="40882-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="40882-394">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="40882-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="40882-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="40882-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-396">Project</span><span class="sxs-lookup"><span data-stu-id="40882-396">Project</span></span></td>
<td><p><span data-ttu-id="40882-397">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="40882-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="40882-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="40882-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="40882-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="40882-400">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="40882-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="40882-401">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="40882-402">해당 날짜에 대 한 일일 사용량 명세서 477860 경우 프로 비전 하는 service Bus 연결 25 팩 있고 해당 일 동안 1을 사용 하면, "25 개 연결 / 30 일 – 사용: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="40882-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="40882-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="40882-404">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="40882-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="40882-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="40882-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="40882-406">DomainName</span></span></td>
<td><p><span data-ttu-id="40882-407">고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="40882-408">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="40882-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="40882-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="40882-410">단위</span><span class="sxs-lookup"><span data-stu-id="40882-410">Unit</span></span></td>
<td><p><span data-ttu-id="40882-411">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="40882-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="40882-412">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="40882-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="40882-413">일회성 및 되풀이 파일 필드</span><span class="sxs-lookup"><span data-stu-id="40882-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="40882-414">Column</span><span class="sxs-lookup"><span data-stu-id="40882-414">Column</span></span></th>
<th><span data-ttu-id="40882-415">설명</span><span class="sxs-lookup"><span data-stu-id="40882-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="40882-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="40882-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="40882-417">특정 청구 엔터티 GUID 형식에서에 대 한 고유한 Microsoft Azure Active Directory 테 넌 트 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="40882-418">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="40882-419">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-420">Customer Id</span><span class="sxs-lookup"><span data-stu-id="40882-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="40882-421">고유한 Microsoft Azure Active Directory 테 넌 트 ID를 GUID 형식으로 고객을 식별 하는 데 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-422">고객 이름</span><span class="sxs-lookup"><span data-stu-id="40882-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="40882-423">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="40882-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="40882-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="40882-425">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="40882-426">이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="40882-427">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-428">고객 국가</span><span class="sxs-lookup"><span data-stu-id="40882-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="40882-429">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-430">송장 번호</span><span class="sxs-lookup"><span data-stu-id="40882-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="40882-431">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="40882-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="40882-432">MpnId</span></span></td>
<td><p><span data-ttu-id="40882-433">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="40882-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="40882-435">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-436">주문 ID</span><span class="sxs-lookup"><span data-stu-id="40882-436">Order ID</span></span></td>
<td><p><span data-ttu-id="40882-437">Microsoft commerce platform은 주문에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="40882-438">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-439">주문 날짜</span><span class="sxs-lookup"><span data-stu-id="40882-439">Order date</span></span></td>
<td><p><span data-ttu-id="40882-440">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="40882-441">ProductId</span></span></td>
<td><p><span data-ttu-id="40882-442">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="40882-443">SkuId</span></span></td>
<td><p><span data-ttu-id="40882-444">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="40882-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="40882-446">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-446">The ID for a particular Availability.</span></span> <span data-ttu-id="40882-447">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-448">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="40882-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="40882-449">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-450">제품 이름</span><span class="sxs-lookup"><span data-stu-id="40882-450">Product name</span></span></td>
<td><p><span data-ttu-id="40882-451">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="40882-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="40882-453">제품의 게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="40882-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="40882-455">이 게시자에 대 한 고유 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-456">구독 설명</span><span class="sxs-lookup"><span data-stu-id="40882-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="40882-457">구독의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-458">구독 ID</span><span class="sxs-lookup"><span data-stu-id="40882-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="40882-459">Microsoft commerce platform은 구독에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="40882-460">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="40882-461">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="40882-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40882-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40882-463">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="40882-463">Start day of the charges.</span></span> <span data-ttu-id="40882-464">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40882-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40882-466">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="40882-466">End day of the charges.</span></span> <span data-ttu-id="40882-467">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-468">용어 및 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="40882-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="40882-469">기간 및 구매에 대 한 청구 주기입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="40882-470">예를 들어, "1 년, 월."</span><span class="sxs-lookup"><span data-stu-id="40882-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-471">청구 유형</span><span class="sxs-lookup"><span data-stu-id="40882-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="40882-472">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="40882-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-473">Unit Price</span><span class="sxs-lookup"><span data-stu-id="40882-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="40882-474">구매 시 게시 된 가격표의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="40882-475">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-476">효과적인 단가</span><span class="sxs-lookup"><span data-stu-id="40882-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="40882-477">단위 가격 조정을 만든 후입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-478">수량</span><span class="sxs-lookup"><span data-stu-id="40882-478">Quantity</span></span></td>
<td><p><span data-ttu-id="40882-479">단위 수입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-479">Number of units.</span></span> <span data-ttu-id="40882-480">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-481">단위 형식</span><span class="sxs-lookup"><span data-stu-id="40882-481">Unit type</span></span></td>
<td><p><span data-ttu-id="40882-482">구매 되는 단위의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="40882-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="40882-484">적용 가능한 할인을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-485">Sub Total</span><span class="sxs-lookup"><span data-stu-id="40882-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="40882-486">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="40882-486">Total before tax.</span></span> <span data-ttu-id="40882-487">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-488">세금 합계</span><span class="sxs-lookup"><span data-stu-id="40882-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="40882-489">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="40882-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-490">Total</span><span class="sxs-lookup"><span data-stu-id="40882-490">Total</span></span></td>
<td><p><span data-ttu-id="40882-491">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="40882-491">Total after tax.</span></span> <span data-ttu-id="40882-492">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-493">Currency</span><span class="sxs-lookup"><span data-stu-id="40882-493">Currency</span></span></td>
<td><p><span data-ttu-id="40882-494">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="40882-494">Currency type.</span></span> <span data-ttu-id="40882-495">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="40882-496">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="40882-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="40882-498">대체 식별자에는 주문 id입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="40882-499">매일 배분 사용 현황 파일 필드</span><span class="sxs-lookup"><span data-stu-id="40882-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="40882-500">Column</span><span class="sxs-lookup"><span data-stu-id="40882-500">Column</span></span></th>
<th><span data-ttu-id="40882-501">설명</span><span class="sxs-lookup"><span data-stu-id="40882-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="40882-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="40882-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="40882-503">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="40882-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="40882-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="40882-505">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="40882-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="40882-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="40882-507">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="40882-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="40882-509">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="40882-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="40882-510">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="40882-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="40882-512">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-512">The customer’s domain name.</span></span> <span data-ttu-id="40882-513">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-514">고객 국가</span><span class="sxs-lookup"><span data-stu-id="40882-514">Customer country</span></span></td>
<td><p><span data-ttu-id="40882-515">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="40882-516">MPNID</span></span></td>
<td><p><span data-ttu-id="40882-517">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-518">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="40882-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="40882-519">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="40882-520">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="40882-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="40882-522">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="40882-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="40882-523">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="40882-524">ProductId</span></span></td>
<td><p><span data-ttu-id="40882-525">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="40882-526">SkuId</span></span></td>
<td><p><span data-ttu-id="40882-527">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="40882-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="40882-529">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-529">The ID for a particular Availability.</span></span> <span data-ttu-id="40882-530">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-531">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="40882-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="40882-532">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="40882-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="40882-534">게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="40882-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="40882-536">GUID 형식으로 게시자의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="40882-537">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="40882-538">구독 설명</span><span class="sxs-lookup"><span data-stu-id="40882-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="40882-539">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="40882-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="40882-540">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="40882-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-541">구독 ID</span><span class="sxs-lookup"><span data-stu-id="40882-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="40882-542">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="40882-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="40882-543">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="40882-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="40882-544">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="40882-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="40882-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="40882-546">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="40882-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="40882-547">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="40882-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="40882-549">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="40882-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="40882-550">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-551">사용 날짜</span><span class="sxs-lookup"><span data-stu-id="40882-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="40882-552">서비스 사용의 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-553">미터 종류</span><span class="sxs-lookup"><span data-stu-id="40882-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="40882-554">측정기의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-555">미터 범주</span><span class="sxs-lookup"><span data-stu-id="40882-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="40882-556">사용에 대 한 최상위 수준 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-557">미터 Id</span><span class="sxs-lookup"><span data-stu-id="40882-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="40882-558">사용 중인 미터에 대 한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-559">미터 하위 범주</span><span class="sxs-lookup"><span data-stu-id="40882-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="40882-560">속도 영향을 줄 수 있는 Azure 서비스의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-561">미터 이름</span><span class="sxs-lookup"><span data-stu-id="40882-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="40882-562">사용 중인 미터에 대 한 측정 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-563">요금제 지역</span><span class="sxs-lookup"><span data-stu-id="40882-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="40882-564">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-565">단위</span><span class="sxs-lookup"><span data-stu-id="40882-565">Unit</span></span></td>
<td><p><span data-ttu-id="40882-566">단위 리소스 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-567">사용한 수량</span><span class="sxs-lookup"><span data-stu-id="40882-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="40882-568">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="40882-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="40882-569">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-570">리소스 위치</span><span class="sxs-lookup"><span data-stu-id="40882-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="40882-571">측정기 실행 되 고 있는 데이터 센터입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-572">사용 되는 서비스</span><span class="sxs-lookup"><span data-stu-id="40882-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="40882-573">사용한 Azure 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-574">리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="40882-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="40882-575">배포 된 측정기 실행 되는 리소스 그룹입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-576">리소스 URI</span><span class="sxs-lookup"><span data-stu-id="40882-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="40882-577">사용 중인 리소스의 URI입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-578">청구 유형</span><span class="sxs-lookup"><span data-stu-id="40882-578">Charge type</span></span></td>
<td><p><span data-ttu-id="40882-579">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="40882-579">The type of charge or adjustment.</span></span> <span data-ttu-id="40882-580">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-581">단가</span><span class="sxs-lookup"><span data-stu-id="40882-581">Unit price</span></span></td>
<td><p><span data-ttu-id="40882-582">라이선스를 구매 시 가격표를 게시 하는 대로 당 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="40882-583">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-584">수량</span><span class="sxs-lookup"><span data-stu-id="40882-584">Quantity</span></span></td>
<td><p><span data-ttu-id="40882-585">라이선스의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-585">Number of licenses.</span></span> <span data-ttu-id="40882-586">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-587">단위 형식</span><span class="sxs-lookup"><span data-stu-id="40882-587">Unit type</span></span></td>
<td><p><span data-ttu-id="40882-588">측정기 요금이 청구 되는 단위의 형식입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="40882-589">현재 작업에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-590">청구 전 세금</span><span class="sxs-lookup"><span data-stu-id="40882-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="40882-591">세금 전에 총 공간입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-592">청구 통화</span><span class="sxs-lookup"><span data-stu-id="40882-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="40882-593">고객의 지리적 지역에 통화</span><span class="sxs-lookup"><span data-stu-id="40882-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-594">세금 공제 전 가격 책정 요약</span><span class="sxs-lookup"><span data-stu-id="40882-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="40882-595">가격 책정 세금 추가 되기 전에 합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-596">통화 가격 책정</span><span class="sxs-lookup"><span data-stu-id="40882-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="40882-597">가격표에서 통화입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-598">서비스 정보 1</span><span class="sxs-lookup"><span data-stu-id="40882-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="40882-599">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="40882-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-600">서비스 정보 2</span><span class="sxs-lookup"><span data-stu-id="40882-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="40882-601">선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="40882-602">Tags</span><span class="sxs-lookup"><span data-stu-id="40882-602">Tags</span></span></td>
<td><p><span data-ttu-id="40882-603">청구 레코드를 그룹화 하려면 측정기에 할당 하는 태그입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="40882-604">예를 들어를 측정기를 사용 하는 부서에서 비용을 배분 하는데 태그를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="40882-605">추가 정보</span><span class="sxs-lookup"><span data-stu-id="40882-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="40882-606">다른 열에서 다루지 않는 추가 정보.</span><span class="sxs-lookup"><span data-stu-id="40882-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="40882-607">청구서 및 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="40882-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="40882-608">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="40882-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="40882-609">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="40882-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="40882-610">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="40882-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="40882-611">송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="40882-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="40882-612">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="40882-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="40882-613"><strong>청구서 금액 충전 설명</strong></span><span class="sxs-lookup"><span data-stu-id="40882-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-614"><strong>조정 파일 금액 설명 (ChargeType 열)</strong></span><span class="sxs-lookup"><span data-stu-id="40882-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-615"><strong>이 요금 이란 무엇 인가요?</strong></span><span class="sxs-lookup"><span data-stu-id="40882-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-616"><strong>이러한 ChargeTypes를 청구서에 매핑하려면 어떻게 하나요?</strong></span><span class="sxs-lookup"><span data-stu-id="40882-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="40882-617"><strong>라이선스 기반 요금</strong></span><span class="sxs-lookup"><span data-stu-id="40882-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-618">활성화 수수료</span><span class="sxs-lookup"><span data-stu-id="40882-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-619">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="40882-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="40882-620">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-621">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="40882-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-622">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-623">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="40882-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-624">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="40882-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-625">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="40882-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-626">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-627">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-628">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="40882-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-629">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-630">연간 청구를 사용 하는 경우 구독에 대 한 요금 유형</span><span class="sxs-lookup"><span data-stu-id="40882-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-631">구매 요금</span><span class="sxs-lookup"><span data-stu-id="40882-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-632">월 청구 비용은 사용 하는 경우 구독에 대 한 요금 유형</span><span class="sxs-lookup"><span data-stu-id="40882-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-633">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-634">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="40882-635">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="40882-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-636">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="40882-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-637">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-638">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="40882-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="40882-639"><strong>일회성 요금</strong></span><span class="sxs-lookup"><span data-stu-id="40882-639"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="40882-640">단추를 사용하여 새</span><span class="sxs-lookup"><span data-stu-id="40882-640">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-641">새 구매를 만들 때 사용</span><span class="sxs-lookup"><span data-stu-id="40882-641">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-642">addQuantity</span><span class="sxs-lookup"><span data-stu-id="40882-642">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-643">증가 한 후 원래 구매 및 새 수량은 환불이 적용 모두 사용</span><span class="sxs-lookup"><span data-stu-id="40882-643">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="40882-644">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="40882-644">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-645">감소 후 원래 구매 및 새 수량은 환불이 적용 모두 사용</span><span class="sxs-lookup"><span data-stu-id="40882-645">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="40882-646">Cancel</span><span class="sxs-lookup"><span data-stu-id="40882-646">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-647">구독 취소 되 면 사용</span><span class="sxs-lookup"><span data-stu-id="40882-647">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="40882-648">변환</span><span class="sxs-lookup"><span data-stu-id="40882-648">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-649">라이선스를 업그레이드 하지만 좌석 수 그대로 유지 하는 경우에 사용</span><span class="sxs-lookup"><span data-stu-id="40882-649">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="40882-650"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="40882-650"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-651">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="40882-651">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-652">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="40882-652">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="40882-653">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-654">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="40882-654">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-655">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="40882-655">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="40882-656"><strong>크레딧</strong></span><span class="sxs-lookup"><span data-stu-id="40882-656"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-657">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="40882-657">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-658">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="40882-658">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-659">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-659">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="40882-660">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-660">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="40882-661"><strong>사용량 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="40882-661"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-662">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="40882-662">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-663">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="40882-663">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="40882-664">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-664">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-665">주기 할인</span><span class="sxs-lookup"><span data-stu-id="40882-665">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-666">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="40882-666">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-667">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="40882-667">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-668">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="40882-668">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-669">취소 할인</span><span class="sxs-lookup"><span data-stu-id="40882-669">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-670">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="40882-670">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="40882-671"><strong>라이선스 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="40882-671"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-672"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="40882-672"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="40882-673">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-673">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="40882-674"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="40882-674"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-675"><em>여러 요금 유형에 적용할 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="40882-675"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="40882-676"><em>예외: &quot;품목 요금 차감&quot; 이미 세금이 포함 되어 있습니다. 위의 크레딧을 참조 하세요.</em></span><span class="sxs-lookup"><span data-stu-id="40882-676"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-677">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="40882-677">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="40882-678">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-678">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="40882-679">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="40882-679">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
