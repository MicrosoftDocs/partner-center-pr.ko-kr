---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 07/08/2019
description: 청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 보려면 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8fae84790aa84b3c5a006d65a632668a33ac24a7
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820559"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b89d2-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="b89d2-103">Use the reconciliation files</span></span>

<span data-ttu-id="b89d2-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="b89d2-104">**Applies to**</span></span>

-  <span data-ttu-id="b89d2-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b89d2-105">Partner Center</span></span>
-  <span data-ttu-id="b89d2-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b89d2-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="b89d2-107">청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 보려면 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="b89d2-108">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="b89d2-109">서식 지정 문제</span><span class="sxs-lookup"><span data-stu-id="b89d2-109">Formatting issues</span></span>

<span data-ttu-id="b89d2-110">경우에 따라 정찰 파일에 서식 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="b89d2-111">이는 예를 들어 EN-US 로캘이 사용 되지 않는 경우에 발생할 수 있습니다. 이러한 문제를 해결 하려면 아래 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="b89d2-112">Excel에서 .csv 파일을 열고 첫 번째 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="b89d2-113">리본 메뉴에서 <strong>데이터</strong>를 선택 하 고 <strong>열 텍스트를</strong>선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="b89d2-114">텍스트를 열로 변환 마법사에서 구분 된 <strong>파일 형식</strong>을 선택 하 고 <strong>다음</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b89d2-115">구분 기호 필드에서 <strong>쉼표</strong>를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="b89d2-116"><strong>탭</strong> 이 이미 선택 되어 있으면 그대로 둘 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="b89d2-117"><strong>다음</strong>을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="b89d2-118">열 데이터 형식 필드에서 날짜를 선택 <strong>합니다. MDY</strong>을 선택한 후 <strong>다음</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b89d2-119">열 데이터 형식 필드에서 모든 금액 열에 대해 <strong>텍스트</strong> 를 선택한 다음 <strong>마침</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="b89d2-120">Large 정찰 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="b89d2-120">Downloading a large recon file</span></span>

<span data-ttu-id="b89d2-121">정찰 파일은 매우 커질 수 있으며 다운로드 하기도 어렵습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="b89d2-122">대량 정찰 파일을 다운로드 하는 데 도움이 되는 PowerShell 스크립트는 [청구서 품목 가져오기 항목](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b89d2-123">파트너 기준 항목별로</span><span class="sxs-lookup"><span data-stu-id="b89d2-123">Itemize by partner</span></span>


<span data-ttu-id="b89d2-124">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 모두 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b89d2-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-125">MPN ID</span></span></th>
<th><span data-ttu-id="b89d2-126">설명</span><span class="sxs-lookup"><span data-stu-id="b89d2-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b89d2-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="b89d2-128">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="b89d2-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-129">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b89d2-130">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b89d2-131">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b89d2-132">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b89d2-133">eTo를 보거나 업데이트 하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음, 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b89d2-134">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b89d2-135"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b89d2-136">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="b89d2-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b89d2-137">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="b89d2-138">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="b89d2-139">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="b89d2-139">License-based file fields</span></span>


<span data-ttu-id="b89d2-140">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b89d2-141"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="b89d2-142"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="b89d2-143"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b89d2-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="b89d2-145">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="b89d2-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b89d2-146">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b89d2-147">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b89d2-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b89d2-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b89d2-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="b89d2-150">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b89d2-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b89d2-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="b89d2-152">OrderID</span></span></td>
<td><p><span data-ttu-id="b89d2-153">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="b89d2-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b89d2-154">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b89d2-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b89d2-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b89d2-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b89d2-157">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="b89d2-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b89d2-158">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b89d2-159">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b89d2-160">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b89d2-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b89d2-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b89d2-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b89d2-163">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="b89d2-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b89d2-164">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b89d2-165">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b89d2-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b89d2-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="b89d2-167">OfferID</span></span></td>
<td><p><span data-ttu-id="b89d2-168">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="b89d2-168">Unique offer ID.</span></span> <span data-ttu-id="b89d2-169">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="b89d2-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b89d2-170"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b89d2-171">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b89d2-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b89d2-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b89d2-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b89d2-174">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="b89d2-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b89d2-175"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b89d2-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b89d2-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="b89d2-177">OfferName</span></span></td>
<td><p><span data-ttu-id="b89d2-178">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="b89d2-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b89d2-179">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="b89d2-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b89d2-181">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="b89d2-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b89d2-182">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b89d2-183">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b89d2-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b89d2-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b89d2-186">구독 종료 날짜: 시작 날짜 이후 12 개월 + x 일 (파트너 청구 날짜에 맞추기) 또는 갱신 날짜 로부터 12 개월</span><span class="sxs-lookup"><span data-stu-id="b89d2-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b89d2-187">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b89d2-188">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b89d2-189">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b89d2-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b89d2-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b89d2-192">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="b89d2-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b89d2-193">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b89d2-194">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b89d2-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b89d2-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b89d2-197">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="b89d2-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="b89d2-198">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b89d2-199">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b89d2-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b89d2-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b89d2-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="b89d2-202">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="b89d2-202">The type of charge or adjustment.</span></span> <span data-ttu-id="b89d2-203"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b89d2-204"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b89d2-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b89d2-206">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="b89d2-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b89d2-207">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b89d2-208">6.82</span><span class="sxs-lookup"><span data-stu-id="b89d2-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-209">수량</span><span class="sxs-lookup"><span data-stu-id="b89d2-209">Quantity</span></span></td>
<td><p><span data-ttu-id="b89d2-210">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="b89d2-210">Number of seats.</span></span> <span data-ttu-id="b89d2-211">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b89d2-212">2</span><span class="sxs-lookup"><span data-stu-id="b89d2-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-213">Amount</span><span class="sxs-lookup"><span data-stu-id="b89d2-213">Amount</span></span></td>
<td><p><span data-ttu-id="b89d2-214">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="b89d2-214">Total of price for quantity.</span></span> <span data-ttu-id="b89d2-215">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b89d2-216">13.32</span><span class="sxs-lookup"><span data-stu-id="b89d2-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b89d2-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b89d2-218">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="b89d2-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b89d2-219">역량 또는 맵과 함께 제공 되는 제품 라이선스 또는 동기에 적합 한 새 구독은이 열에 할인 금액을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b89d2-220">2.32</span><span class="sxs-lookup"><span data-stu-id="b89d2-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b89d2-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="b89d2-222">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="b89d2-222">Total before tax.</span></span> <span data-ttu-id="b89d2-223">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b89d2-224">11</span><span class="sxs-lookup"><span data-stu-id="b89d2-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-225">Tax</span><span class="sxs-lookup"><span data-stu-id="b89d2-225">Tax</span></span></td>
<td><p><span data-ttu-id="b89d2-226">시장의&#39;세금 규칙 및 특정 상황에 따라 세금 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b89d2-227">0</span><span class="sxs-lookup"><span data-stu-id="b89d2-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b89d2-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b89d2-229">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="b89d2-229">Total after tax.</span></span> <span data-ttu-id="b89d2-230">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b89d2-231">11</span><span class="sxs-lookup"><span data-stu-id="b89d2-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-232">Currency</span><span class="sxs-lookup"><span data-stu-id="b89d2-232">Currency</span></span></td>
<td><p><span data-ttu-id="b89d2-233">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="b89d2-233">Currency type.</span></span> <span data-ttu-id="b89d2-234">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="b89d2-235">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b89d2-236">EUR</span><span class="sxs-lookup"><span data-stu-id="b89d2-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b89d2-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="b89d2-238">파트너&#39;센터에 보고 된 고객의 조직 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b89d2-239">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b89d2-240">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="b89d2-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="b89d2-241">MPNID</span></span></td>
<td><p><span data-ttu-id="b89d2-242">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b89d2-243">4390934</span><span class="sxs-lookup"><span data-stu-id="b89d2-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b89d2-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b89d2-245">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b89d2-246"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b89d2-247">4390934</span><span class="sxs-lookup"><span data-stu-id="b89d2-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="b89d2-248">DomainName</span></span></td>
<td><p><span data-ttu-id="b89d2-249">고객&#39;을 식별 하는 데 사용 되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b89d2-250">고객/파트너가 O365 포털을 통해 베 니 티/default 도메인을 업데이트할 수 있으므로 고객을 고유 하 게 식별 하는 데 사용 하면 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b89d2-251">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b89d2-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b89d2-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b89d2-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b89d2-254">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="b89d2-254">Subscription nickname.</span></span> <span data-ttu-id="b89d2-255">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b89d2-256">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="b89d2-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b89d2-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b89d2-258">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="b89d2-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b89d2-259">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="b89d2-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b89d2-260">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="b89d2-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b89d2-261">사용 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="b89d2-261">Usage-based file fields</span></span>


<span data-ttu-id="b89d2-262">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b89d2-263">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b89d2-264"><strong>열</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="b89d2-265"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="b89d2-266"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b89d2-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="b89d2-268">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b89d2-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b89d2-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b89d2-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="b89d2-271">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b89d2-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="b89d2-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b89d2-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b89d2-274">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b89d2-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="b89d2-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b89d2-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="b89d2-277">파트너&#39;센터에 보고 된 고객의 조직 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b89d2-278">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b89d2-279">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="b89d2-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="b89d2-280">MPNID</span></span></td>
<td><p><span data-ttu-id="b89d2-281">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b89d2-282">4390934</span><span class="sxs-lookup"><span data-stu-id="b89d2-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b89d2-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b89d2-284">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b89d2-285"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b89d2-286">4390934</span><span class="sxs-lookup"><span data-stu-id="b89d2-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b89d2-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b89d2-288">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="b89d2-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b89d2-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b89d2-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b89d2-291">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="b89d2-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b89d2-292">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b89d2-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b89d2-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b89d2-295">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="b89d2-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b89d2-296">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b89d2-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b89d2-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b89d2-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b89d2-299">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="b89d2-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b89d2-300">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b89d2-301">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b89d2-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b89d2-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b89d2-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b89d2-304">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="b89d2-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b89d2-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b89d2-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b89d2-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b89d2-307">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="b89d2-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b89d2-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b89d2-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="b89d2-309">OrderID</span></span></td>
<td><p><span data-ttu-id="b89d2-310">Microsoft 청구 플랫폼에서 주문의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="b89d2-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b89d2-311">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b89d2-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b89d2-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b89d2-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="b89d2-314">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b89d2-315">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="b89d2-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b89d2-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="b89d2-317">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="b89d2-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b89d2-318">서비스 버스 - 개별 또는 팩</span><span class="sxs-lookup"><span data-stu-id="b89d2-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="b89d2-319">SQL Azure 데이터베이스 - Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="b89d2-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b89d2-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b89d2-321">모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="b89d2-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b89d2-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b89d2-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="b89d2-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="b89d2-324">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b89d2-325">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="b89d2-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b89d2-326">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="b89d2-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-327">Region</span><span class="sxs-lookup"><span data-stu-id="b89d2-327">Region</span></span></td>
<td><p><span data-ttu-id="b89d2-328">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-328">The region the usage applies to.</span></span> <span data-ttu-id="b89d2-329">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b89d2-330">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="b89d2-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-331">SKU</span><span class="sxs-lookup"><span data-stu-id="b89d2-331">SKU</span></span></td>
<td><p><span data-ttu-id="b89d2-332">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="b89d2-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b89d2-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="b89d2-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b89d2-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b89d2-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b89d2-335">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="b89d2-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b89d2-336">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b89d2-337">1</span><span class="sxs-lookup"><span data-stu-id="b89d2-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b89d2-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b89d2-339">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="b89d2-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b89d2-340">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b89d2-341">11</span><span class="sxs-lookup"><span data-stu-id="b89d2-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b89d2-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b89d2-343">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="b89d2-343">Units included as part of the offer.</span></span> <span data-ttu-id="b89d2-344">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b89d2-345">0</span><span class="sxs-lookup"><span data-stu-id="b89d2-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b89d2-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b89d2-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b89d2-347">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="b89d2-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b89d2-348">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b89d2-349">11</span><span class="sxs-lookup"><span data-stu-id="b89d2-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b89d2-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="b89d2-351">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="b89d2-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b89d2-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="b89d2-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b89d2-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b89d2-354">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b89d2-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="b89d2-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b89d2-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b89d2-357">시장의&#39;세금 규칙 및 특정 상황에 따라 세금 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b89d2-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="b89d2-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b89d2-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b89d2-360">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="b89d2-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b89d2-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="b89d2-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-362">Currency</span><span class="sxs-lookup"><span data-stu-id="b89d2-362">Currency</span></span></td>
<td><p><span data-ttu-id="b89d2-363">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="b89d2-363">Currency type.</span></span> <span data-ttu-id="b89d2-364">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="b89d2-365">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b89d2-366">EUR</span><span class="sxs-lookup"><span data-stu-id="b89d2-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b89d2-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b89d2-368">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="b89d2-368">Pretax price per unit.</span></span> <span data-ttu-id="b89d2-369">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b89d2-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="b89d2-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b89d2-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b89d2-372">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="b89d2-372">Post tax price per unit.</span></span> <span data-ttu-id="b89d2-373">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b89d2-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="b89d2-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b89d2-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="b89d2-376">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="b89d2-376">The type of charge or adjustment.</span></span> <span data-ttu-id="b89d2-377"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b89d2-378"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b89d2-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b89d2-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b89d2-380">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b89d2-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="b89d2-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="b89d2-383">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="b89d2-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b89d2-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b89d2-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b89d2-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b89d2-386">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b89d2-387">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="b89d2-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b89d2-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="b89d2-389">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b89d2-390">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b89d2-391">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b89d2-392">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="b89d2-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b89d2-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b89d2-394">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="b89d2-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b89d2-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="b89d2-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-396">프로젝트</span><span class="sxs-lookup"><span data-stu-id="b89d2-396">Project</span></span></td>
<td><p><span data-ttu-id="b89d2-397">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b89d2-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b89d2-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b89d2-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b89d2-400">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="b89d2-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b89d2-401">예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="b89d2-402">25 개의 ServiceBus 연결이 프로 비전 되 고 해당 일 중에 1을 사용한 경우 해당 일에 대 한 일일 사용 명세서는 "25 개의 연결/30 일 – 사용 됨"을 표시 합니다. 1.000000 ".</span><span class="sxs-lookup"><span data-stu-id="b89d2-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b89d2-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="b89d2-404">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b89d2-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b89d2-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b89d2-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="b89d2-406">DomainName</span></span></td>
<td><p><span data-ttu-id="b89d2-407">고객&#39;을 식별 하는 데 사용 되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b89d2-408">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b89d2-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b89d2-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b89d2-410">단위</span><span class="sxs-lookup"><span data-stu-id="b89d2-410">Unit</span></span></td>
<td><p><span data-ttu-id="b89d2-411">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="b89d2-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b89d2-412">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="b89d2-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="b89d2-413">일회성 및 되풀이 파일 필드</span><span class="sxs-lookup"><span data-stu-id="b89d2-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b89d2-414">Column</span><span class="sxs-lookup"><span data-stu-id="b89d2-414">Column</span></span></th>
<th><span data-ttu-id="b89d2-415">설명</span><span class="sxs-lookup"><span data-stu-id="b89d2-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="b89d2-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b89d2-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="b89d2-417">특정 청구 엔터티에 대 한 고유 Microsoft Azure Active Directory 테 넌 트 식별자 (GUID 형식)입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b89d2-418">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b89d2-419">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-420">Customer Id</span><span class="sxs-lookup"><span data-stu-id="b89d2-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="b89d2-421">사용자를 식별 하는 데 사용 되는 GUID 형식의 고유한 Microsoft Azure Active Directory 테 넌 트 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-422">고객 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="b89d2-423">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="b89d2-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b89d2-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b89d2-425">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b89d2-426">고객/파트너가 O365 포털을 통해 베 니 티/default 도메인을 업데이트할 수 있으므로 고객을 고유 하 게 식별 하는 데 사용 하면 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b89d2-427">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-428">고객 국가</span><span class="sxs-lookup"><span data-stu-id="b89d2-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="b89d2-429">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-430">송장 번호</span><span class="sxs-lookup"><span data-stu-id="b89d2-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="b89d2-431">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="b89d2-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="b89d2-432">MpnId</span></span></td>
<td><p><span data-ttu-id="b89d2-433">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-434">대리점 MpnId</span><span class="sxs-lookup"><span data-stu-id="b89d2-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="b89d2-435">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-436">주문 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-436">Order ID</span></span></td>
<td><p><span data-ttu-id="b89d2-437">Microsoft commerce platform의 주문에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="b89d2-438">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-439">주문 날짜</span><span class="sxs-lookup"><span data-stu-id="b89d2-439">Order date</span></span></td>
<td><p><span data-ttu-id="b89d2-440">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="b89d2-441">ProductId</span></span></td>
<td><p><span data-ttu-id="b89d2-442">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="b89d2-443">SkuId</span></span></td>
<td><p><span data-ttu-id="b89d2-444">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b89d2-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b89d2-446">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-446">The ID for a particular Availability.</span></span> <span data-ttu-id="b89d2-447">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-448">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="b89d2-449">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-450">제품 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-450">Product name</span></span></td>
<td><p><span data-ttu-id="b89d2-451">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b89d2-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="b89d2-453">제품 게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b89d2-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="b89d2-455">이 게시자에 대 한 고유 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-456">구독 설명</span><span class="sxs-lookup"><span data-stu-id="b89d2-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b89d2-457">구독의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-458">구독 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b89d2-459">Microsoft commerce platform의 구독에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="b89d2-460">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b89d2-461">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b89d2-463">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="b89d2-463">Start day of the charges.</span></span> <span data-ttu-id="b89d2-464">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b89d2-466">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="b89d2-466">End day of the charges.</span></span> <span data-ttu-id="b89d2-467">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-468">용어 및 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="b89d2-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="b89d2-469">구매를 위한 용어 길이와 청구 주기입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="b89d2-470">예: "1 년, 월"</span><span class="sxs-lookup"><span data-stu-id="b89d2-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-471">청구 유형</span><span class="sxs-lookup"><span data-stu-id="b89d2-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="b89d2-472">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="b89d2-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-473">Unit Price</span><span class="sxs-lookup"><span data-stu-id="b89d2-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="b89d2-474">구매 시 가격표에 게시 된 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b89d2-475">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-476">유효 단가</span><span class="sxs-lookup"><span data-stu-id="b89d2-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="b89d2-477">조정을 수행한 후 단가입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-478">수량</span><span class="sxs-lookup"><span data-stu-id="b89d2-478">Quantity</span></span></td>
<td><p><span data-ttu-id="b89d2-479">단위 수입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-479">Number of units.</span></span> <span data-ttu-id="b89d2-480">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-481">단위 형식</span><span class="sxs-lookup"><span data-stu-id="b89d2-481">Unit type</span></span></td>
<td><p><span data-ttu-id="b89d2-482">구입할 단위의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="b89d2-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="b89d2-484">해당 할인에 대 한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-485">하위 합계</span><span class="sxs-lookup"><span data-stu-id="b89d2-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="b89d2-486">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="b89d2-486">Total before tax.</span></span> <span data-ttu-id="b89d2-487">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-488">세금 합계</span><span class="sxs-lookup"><span data-stu-id="b89d2-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="b89d2-489">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="b89d2-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-490">Total</span><span class="sxs-lookup"><span data-stu-id="b89d2-490">Total</span></span></td>
<td><p><span data-ttu-id="b89d2-491">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="b89d2-491">Total after tax.</span></span> <span data-ttu-id="b89d2-492">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-493">Currency</span><span class="sxs-lookup"><span data-stu-id="b89d2-493">Currency</span></span></td>
<td><p><span data-ttu-id="b89d2-494">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="b89d2-494">Currency type.</span></span> <span data-ttu-id="b89d2-495">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="b89d2-496">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="b89d2-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="b89d2-498">주문 ID에 대 한 대체 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="b89d2-499">매일 등급 사용 파일 필드</span><span class="sxs-lookup"><span data-stu-id="b89d2-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b89d2-500">Column</span><span class="sxs-lookup"><span data-stu-id="b89d2-500">Column</span></span></th>
<th><span data-ttu-id="b89d2-501">설명</span><span class="sxs-lookup"><span data-stu-id="b89d2-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="b89d2-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b89d2-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="b89d2-503">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b89d2-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="b89d2-505">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="b89d2-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="b89d2-507">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="b89d2-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="b89d2-509">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="b89d2-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b89d2-510">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b89d2-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b89d2-512">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-512">The customer’s domain name.</span></span> <span data-ttu-id="b89d2-513">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-514">고객 국가</span><span class="sxs-lookup"><span data-stu-id="b89d2-514">Customer country</span></span></td>
<td><p><span data-ttu-id="b89d2-515">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="b89d2-516">MPNID</span></span></td>
<td><p><span data-ttu-id="b89d2-517">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-518">대리점 MPNID</span><span class="sxs-lookup"><span data-stu-id="b89d2-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="b89d2-519">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b89d2-520">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b89d2-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b89d2-522">지정한 트랜잭션이 표시되는 송장 번호</span><span class="sxs-lookup"><span data-stu-id="b89d2-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="b89d2-523">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="b89d2-524">ProductId</span></span></td>
<td><p><span data-ttu-id="b89d2-525">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="b89d2-526">SkuId</span></span></td>
<td><p><span data-ttu-id="b89d2-527">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b89d2-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b89d2-529">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-529">The ID for a particular Availability.</span></span> <span data-ttu-id="b89d2-530">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-531">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="b89d2-532">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b89d2-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="b89d2-534">게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b89d2-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="b89d2-536">GUID 형식의 게시자 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="b89d2-537">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="b89d2-538">구독 설명</span><span class="sxs-lookup"><span data-stu-id="b89d2-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b89d2-539">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="b89d2-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b89d2-540">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="b89d2-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-541">구독 ID</span><span class="sxs-lookup"><span data-stu-id="b89d2-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b89d2-542">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="b89d2-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b89d2-543">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b89d2-544">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b89d2-546">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="b89d2-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b89d2-547">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b89d2-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b89d2-549">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="b89d2-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b89d2-550">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-551">사용 날짜</span><span class="sxs-lookup"><span data-stu-id="b89d2-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="b89d2-552">서비스 사용 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-553">측정기 유형</span><span class="sxs-lookup"><span data-stu-id="b89d2-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="b89d2-554">측정기의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-555">미터 범주</span><span class="sxs-lookup"><span data-stu-id="b89d2-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="b89d2-556">사용에 대 한 최상위 수준 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-557">측정기 Id</span><span class="sxs-lookup"><span data-stu-id="b89d2-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="b89d2-558">사용 되는 측정기의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-559">미터 하위 범주</span><span class="sxs-lookup"><span data-stu-id="b89d2-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="b89d2-560">요금에 영향을 줄 수 있는 Azure 서비스의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-561">미터 이름</span><span class="sxs-lookup"><span data-stu-id="b89d2-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="b89d2-562">사용 되는 측정기에 대 한 측정 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-563">측정기 지역</span><span class="sxs-lookup"><span data-stu-id="b89d2-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="b89d2-564">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-565">단위</span><span class="sxs-lookup"><span data-stu-id="b89d2-565">Unit</span></span></td>
<td><p><span data-ttu-id="b89d2-566">리소스 이름의 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-567">소비 된 수량</span><span class="sxs-lookup"><span data-stu-id="b89d2-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="b89d2-568">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="b89d2-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="b89d2-569">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-570">리소스 위치</span><span class="sxs-lookup"><span data-stu-id="b89d2-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="b89d2-571">측정기가 실행 되 고 있는 데이터 센터입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-572">사용 된 서비스</span><span class="sxs-lookup"><span data-stu-id="b89d2-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="b89d2-573">사용한 Azure 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="b89d2-574">리소스 URI</span><span class="sxs-lookup"><span data-stu-id="b89d2-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="b89d2-575">사용 되는 리소스의 URI입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-576">청구 유형</span><span class="sxs-lookup"><span data-stu-id="b89d2-576">Charge type</span></span></td>
<td><p><span data-ttu-id="b89d2-577">요금 또는 조정 유형.</span><span class="sxs-lookup"><span data-stu-id="b89d2-577">The type of charge or adjustment.</span></span> <span data-ttu-id="b89d2-578">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-579">단가</span><span class="sxs-lookup"><span data-stu-id="b89d2-579">Unit price</span></span></td>
<td><p><span data-ttu-id="b89d2-580">구매 시 가격표에 게시 된 라이선스 당 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b89d2-581">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-582">수량</span><span class="sxs-lookup"><span data-stu-id="b89d2-582">Quantity</span></span></td>
<td><p><span data-ttu-id="b89d2-583">라이선스의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-583">Number of licenses.</span></span> <span data-ttu-id="b89d2-584">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-585">단위 형식</span><span class="sxs-lookup"><span data-stu-id="b89d2-585">Unit type</span></span></td>
<td><p><span data-ttu-id="b89d2-586">미터의 요금이 청구 되는 단위 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="b89d2-587">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-588">청구 전 세금</span><span class="sxs-lookup"><span data-stu-id="b89d2-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="b89d2-589">세금 전 총 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-590">청구 통화</span><span class="sxs-lookup"><span data-stu-id="b89d2-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="b89d2-591">고객 지역의 통화</span><span class="sxs-lookup"><span data-stu-id="b89d2-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-592">가격 책정 pretax 합계</span><span class="sxs-lookup"><span data-stu-id="b89d2-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="b89d2-593">세금이 추가 되기 전의 가격 책정입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-594">가격 책정 통화</span><span class="sxs-lookup"><span data-stu-id="b89d2-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="b89d2-595">가격표의 통화입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b89d2-596">서비스 정보 1</span><span class="sxs-lookup"><span data-stu-id="b89d2-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="b89d2-597">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="b89d2-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-598">서비스 정보 2</span><span class="sxs-lookup"><span data-stu-id="b89d2-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="b89d2-599">선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b89d2-600">추가 정보</span><span class="sxs-lookup"><span data-stu-id="b89d2-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="b89d2-601">다른 열에서 다루지 않는 추가 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="b89d2-602">청구서와 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="b89d2-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b89d2-603">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b89d2-604">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b89d2-605">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="b89d2-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b89d2-606">송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b89d2-607">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="b89d2-608"><strong>송장 청구 설명</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-609"><strong>조정 파일 요금 설명 (Chargetcharcolumn)</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-610"><strong>이 요금은 어떻게 청구 되나요?</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-611"><strong>이러한 ChargeTypes을 청구서에 어떻게 할까요? 지도?</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="b89d2-612"><strong>라이선스 기반 요금</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-613">활성화 수수료</span><span class="sxs-lookup"><span data-stu-id="b89d2-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-614">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="b89d2-615">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-616">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="b89d2-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-617">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-618">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="b89d2-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-619">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-620">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="b89d2-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-621">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-622">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-623">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="b89d2-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-624">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-625">연간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형</span><span class="sxs-lookup"><span data-stu-id="b89d2-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-626">구매 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-627">월간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형</span><span class="sxs-lookup"><span data-stu-id="b89d2-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-628">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-629">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="b89d2-630">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-631">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-632">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-633">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="b89d2-634"><strong>일회성 요금</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="b89d2-635">단추를 사용하여 새</span><span class="sxs-lookup"><span data-stu-id="b89d2-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-636">새 구매가 생성 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b89d2-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-638">원래 구매 환불 및 증가 후 새로운 수량 모두에 사용 됨</span><span class="sxs-lookup"><span data-stu-id="b89d2-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-639">remov</span><span class="sxs-lookup"><span data-stu-id="b89d2-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-640">원래 구매 환불 및 감소 후 새로운 수량 모두에 사용 됨</span><span class="sxs-lookup"><span data-stu-id="b89d2-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-641">취소</span><span class="sxs-lookup"><span data-stu-id="b89d2-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-642">구독이 취소 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-643">변환</span><span class="sxs-lookup"><span data-stu-id="b89d2-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-644">라이선스가 업그레이드 될 때 사용 되지만 사용자의 수는 변경 되지 않은 상태로 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b89d2-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="b89d2-645"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-646">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="b89d2-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-647">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="b89d2-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b89d2-648">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-649">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="b89d2-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-650">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="b89d2-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="b89d2-651"><strong>크레딧</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-652">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="b89d2-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-653">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="b89d2-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-654">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b89d2-655">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="b89d2-656"><strong>사용량 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-657">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-658">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="b89d2-659">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-660">주기 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-661">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-662">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-663">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-664">취소 할인</span><span class="sxs-lookup"><span data-stu-id="b89d2-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-665">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="b89d2-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="b89d2-666"><strong>라이선스 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-667"><em>여러 요금 유형에 적용 될 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="b89d2-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="b89d2-668">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b89d2-669"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="b89d2-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-670"><em>여러 요금 유형에 적용 될 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="b89d2-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="b89d2-671"><em>예외: &quot;Offset 품목&quot; 에 이미 세금이 포함 되어 있습니다. 위의 크레딧을 참조 하세요.</em></span><span class="sxs-lookup"><span data-stu-id="b89d2-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-672">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="b89d2-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b89d2-673">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b89d2-674">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="b89d2-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
