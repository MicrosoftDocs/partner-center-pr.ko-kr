---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 보려면 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753855"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="07ce4-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="07ce4-103">Use the reconciliation files</span></span>

<span data-ttu-id="07ce4-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="07ce4-104">**Applies to**</span></span>

-  <span data-ttu-id="07ce4-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="07ce4-105">Partner Center</span></span>
-  <span data-ttu-id="07ce4-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="07ce4-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="07ce4-107">**적절 한 역할**</span><span class="sxs-lookup"><span data-stu-id="07ce4-107">**Appropriate roles**</span></span>

- <span data-ttu-id="07ce4-108">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="07ce4-108">Billing admin</span></span>
- <span data-ttu-id="07ce4-109">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="07ce4-109">Global admin</span></span>

<span data-ttu-id="07ce4-110">청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 보려면 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="07ce4-111">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="07ce4-112">서식 지정 문제</span><span class="sxs-lookup"><span data-stu-id="07ce4-112">Formatting issues</span></span>

<span data-ttu-id="07ce4-113">경우에 따라 정찰 파일에 서식 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="07ce4-114">이는 예를 들어 EN-US 로캘이 사용 되지 않는 경우에 발생할 수 있습니다. 이러한 문제를 해결 하려면 아래 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="07ce4-115">Excel에서 .csv 파일을 열고 첫 번째 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="07ce4-116">리본 메뉴에서 <strong>데이터</strong>를 선택 하 고 <strong>열 텍스트를</strong>선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="07ce4-117">텍스트를 열로 변환 마법사에서 구분 된 <strong>파일 형식</strong>을 선택 하 고 <strong>다음</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="07ce4-118">구분 기호 필드에서 <strong>쉼표</strong>를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="07ce4-119"><strong>탭</strong> 이 이미 선택 되어 있으면 그대로 둘 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="07ce4-120"><strong>다음</strong>을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="07ce4-121">열 데이터 형식 필드에서 <strong>Date: MDY</strong>를 선택 하 고 <strong>다음</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="07ce4-122">열 데이터 형식 필드에서 모든 금액 열에 대해 <strong>텍스트</strong> 를 선택한 다음 <strong>마침</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="07ce4-123">Large 정찰 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="07ce4-123">Downloading a large recon file</span></span>

<span data-ttu-id="07ce4-124">정찰 파일은 매우 커질 수 있으며 다운로드 하기도 어렵습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="07ce4-125">대량 정찰 파일을 다운로드 하는 데 도움이 되는 PowerShell 스크립트는 [청구서 품목 가져오기 항목](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="07ce4-126">파트너 기준 항목별로</span><span class="sxs-lookup"><span data-stu-id="07ce4-126">Itemize by partner</span></span>


<span data-ttu-id="07ce4-127">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="07ce4-128">MPN ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-128">MPN ID</span></span></th>
<th><span data-ttu-id="07ce4-129">설명</span><span class="sxs-lookup"><span data-stu-id="07ce4-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="07ce4-130">MPN ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="07ce4-131">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="07ce4-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-132">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="07ce4-133">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="07ce4-134">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="07ce4-135">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="07ce4-136">eTo를 보거나 업데이트 하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음, 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="07ce4-137">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="07ce4-138"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="07ce4-139">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="07ce4-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="07ce4-140">CSP 파트너에 MPN ID가 없는 재판매인이 있는 경우이 값은 파트너의 MPN ID로 대신 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="07ce4-141">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="07ce4-142">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="07ce4-142">License-based file fields</span></span>


<span data-ttu-id="07ce4-143">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="07ce4-144"><strong>열의</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="07ce4-145"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="07ce4-146"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="07ce4-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="07ce4-148">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="07ce4-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="07ce4-149">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="07ce4-150">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="07ce4-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="07ce4-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="07ce4-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="07ce4-153">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="07ce4-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="07ce4-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="07ce4-155">OrderID</span></span></td>
<td><p><span data-ttu-id="07ce4-156">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="07ce4-157">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="07ce4-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="07ce4-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="07ce4-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="07ce4-160">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="07ce4-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="07ce4-161">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="07ce4-162">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="07ce4-163">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="07ce4-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="07ce4-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="07ce4-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="07ce4-166">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="07ce4-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="07ce4-167">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="07ce4-168">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="07ce4-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="07ce4-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="07ce4-170">OfferID</span></span></td>
<td><p><span data-ttu-id="07ce4-171">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="07ce4-171">Unique offer ID.</span></span> <span data-ttu-id="07ce4-172">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="07ce4-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="07ce4-173"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="07ce4-174">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="07ce4-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="07ce4-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="07ce4-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="07ce4-177">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="07ce4-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="07ce4-178"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="07ce4-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="07ce4-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="07ce4-180">OfferName</span></span></td>
<td><p><span data-ttu-id="07ce4-181">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="07ce4-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="07ce4-182">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="07ce4-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="07ce4-184">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="07ce4-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="07ce4-185">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="07ce4-186">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="07ce4-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="07ce4-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="07ce4-189">구독 종료 날짜: 12개월 + 시작 날짜 이후 x일(파트너 청구 날짜에 맞추기 위해) 또는 갱신 날짜로부터 12개월.</span><span class="sxs-lookup"><span data-stu-id="07ce4-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="07ce4-190">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="07ce4-191">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="07ce4-192">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="07ce4-193">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="07ce4-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="07ce4-195">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="07ce4-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="07ce4-196">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="07ce4-197">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="07ce4-198">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="07ce4-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="07ce4-200">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="07ce4-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="07ce4-201">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="07ce4-202">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="07ce4-203">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="07ce4-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="07ce4-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="07ce4-205">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-205">The type of charge or adjustment.</span></span> <span data-ttu-id="07ce4-206"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="07ce4-207"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="07ce4-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="07ce4-209">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="07ce4-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="07ce4-210">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="07ce4-211">6.82</span><span class="sxs-lookup"><span data-stu-id="07ce4-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-212">Quantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-212">Quantity</span></span></td>
<td><p><span data-ttu-id="07ce4-213">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="07ce4-213">Number of seats.</span></span> <span data-ttu-id="07ce4-214">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="07ce4-215">2</span><span class="sxs-lookup"><span data-stu-id="07ce4-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-216">합계</span><span class="sxs-lookup"><span data-stu-id="07ce4-216">Amount</span></span></td>
<td><p><span data-ttu-id="07ce4-217">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="07ce4-217">Total of price for quantity.</span></span> <span data-ttu-id="07ce4-218">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="07ce4-219">13.32</span><span class="sxs-lookup"><span data-stu-id="07ce4-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="07ce4-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="07ce4-221">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="07ce4-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="07ce4-222">역량 또는 맵과 함께 제공 되는 제품 라이선스 또는 동기에 적합 한 새 구독은이 열에 할인 금액을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="07ce4-223">2.32</span><span class="sxs-lookup"><span data-stu-id="07ce4-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-224">Subtotal</span><span class="sxs-lookup"><span data-stu-id="07ce4-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="07ce4-225">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="07ce4-225">Total before tax.</span></span> <span data-ttu-id="07ce4-226">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="07ce4-227">11</span><span class="sxs-lookup"><span data-stu-id="07ce4-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-228">Tax</span><span class="sxs-lookup"><span data-stu-id="07ce4-228">Tax</span></span></td>
<td><p><span data-ttu-id="07ce4-229">시장의&#39;세금 규칙 및 특정 상황에 따라 세금 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="07ce4-230">0</span><span class="sxs-lookup"><span data-stu-id="07ce4-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="07ce4-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="07ce4-232">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="07ce4-232">Total after tax.</span></span> <span data-ttu-id="07ce4-233">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="07ce4-234">11</span><span class="sxs-lookup"><span data-stu-id="07ce4-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-235">Currency</span><span class="sxs-lookup"><span data-stu-id="07ce4-235">Currency</span></span></td>
<td><p><span data-ttu-id="07ce4-236">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="07ce4-236">Currency type.</span></span> <span data-ttu-id="07ce4-237">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="07ce4-238">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="07ce4-239">EUR</span><span class="sxs-lookup"><span data-stu-id="07ce4-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="07ce4-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="07ce4-241">파트너&#39;센터에 보고 된 고객의 조직 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="07ce4-242">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="07ce4-243">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="07ce4-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="07ce4-244">MPNID</span></span></td>
<td><p><span data-ttu-id="07ce4-245">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="07ce4-246">4390934</span><span class="sxs-lookup"><span data-stu-id="07ce4-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="07ce4-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="07ce4-248">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="07ce4-249"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="07ce4-250">4390934</span><span class="sxs-lookup"><span data-stu-id="07ce4-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="07ce4-251">DomainName</span></span></td>
<td><p><span data-ttu-id="07ce4-252">고객&#39;을 식별 하는 데 사용 되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="07ce4-253">고객/파트너가 O365 포털을 통해 베 니 티/default 도메인을 업데이트할 수 있으므로 고객을 고유 하 게 식별 하는 데 사용 하면 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="07ce4-254">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="07ce4-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="07ce4-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="07ce4-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="07ce4-257">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="07ce4-257">Subscription nickname.</span></span> <span data-ttu-id="07ce4-258">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="07ce4-259">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="07ce4-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="07ce4-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="07ce4-261">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="07ce4-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="07ce4-262">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="07ce4-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="07ce4-263">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="07ce4-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="07ce4-264">사용 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="07ce4-264">Usage-based file fields</span></span>


<span data-ttu-id="07ce4-265">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="07ce4-266">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="07ce4-267"><strong>열의</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="07ce4-268"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="07ce4-269"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="07ce4-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="07ce4-271">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="07ce4-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="07ce4-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="07ce4-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="07ce4-274">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="07ce4-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="07ce4-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="07ce4-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="07ce4-277">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="07ce4-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="07ce4-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="07ce4-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="07ce4-280">파트너&#39;센터에 보고 된 고객의 조직 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="07ce4-281">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="07ce4-282">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="07ce4-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="07ce4-283">MPNID</span></span></td>
<td><p><span data-ttu-id="07ce4-284">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="07ce4-285">4390934</span><span class="sxs-lookup"><span data-stu-id="07ce4-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="07ce4-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="07ce4-287">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="07ce4-288"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="07ce4-289">4390934</span><span class="sxs-lookup"><span data-stu-id="07ce4-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="07ce4-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="07ce4-291">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="07ce4-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="07ce4-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="07ce4-294">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="07ce4-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="07ce4-295">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="07ce4-296">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="07ce4-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="07ce4-298">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="07ce4-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="07ce4-299">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="07ce4-300">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="07ce4-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="07ce4-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="07ce4-302">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="07ce4-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="07ce4-303">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="07ce4-304">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="07ce4-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="07ce4-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="07ce4-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="07ce4-307">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="07ce4-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="07ce4-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="07ce4-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="07ce4-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="07ce4-310">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="07ce4-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="07ce4-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="07ce4-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="07ce4-312">OrderID</span></span></td>
<td><p><span data-ttu-id="07ce4-313">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="07ce4-314">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="07ce4-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="07ce4-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="07ce4-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="07ce4-317">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="07ce4-318">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="07ce4-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="07ce4-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="07ce4-320">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="07ce4-321">Service Bus 개인 또는 팩</span><span class="sxs-lookup"><span data-stu-id="07ce4-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="07ce4-322">SQL Azure database-Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="07ce4-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="07ce4-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="07ce4-324">모든 서비스 데이터 및 가격 책정 구조에 대한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="07ce4-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="07ce4-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="07ce4-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-326">Resource Name</span><span class="sxs-lookup"><span data-stu-id="07ce4-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="07ce4-327">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="07ce4-328">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="07ce4-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="07ce4-329">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="07ce4-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-330">국가</span><span class="sxs-lookup"><span data-stu-id="07ce4-330">Region</span></span></td>
<td><p><span data-ttu-id="07ce4-331">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-331">The region the usage applies to.</span></span> <span data-ttu-id="07ce4-332">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="07ce4-333">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="07ce4-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-334">SKU</span><span class="sxs-lookup"><span data-stu-id="07ce4-334">SKU</span></span></td>
<td><p><span data-ttu-id="07ce4-335">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="07ce4-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="07ce4-336">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="07ce4-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="07ce4-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="07ce4-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="07ce4-338">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="07ce4-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="07ce4-339">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="07ce4-340">1</span><span class="sxs-lookup"><span data-stu-id="07ce4-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="07ce4-342">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="07ce4-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="07ce4-343">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="07ce4-344">11</span><span class="sxs-lookup"><span data-stu-id="07ce4-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="07ce4-346">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="07ce4-346">Units included as part of the offer.</span></span> <span data-ttu-id="07ce4-347">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="07ce4-348">0</span><span class="sxs-lookup"><span data-stu-id="07ce4-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="07ce4-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="07ce4-350">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="07ce4-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="07ce4-351">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="07ce4-352">11</span><span class="sxs-lookup"><span data-stu-id="07ce4-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="07ce4-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="07ce4-354">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="07ce4-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="07ce4-355">$0.0808</span><span class="sxs-lookup"><span data-stu-id="07ce4-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="07ce4-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="07ce4-357">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="07ce4-358">$0.085</span><span class="sxs-lookup"><span data-stu-id="07ce4-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="07ce4-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="07ce4-360">시장의&#39;세금 규칙 및 특정 상황에 따라 세금 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="07ce4-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="07ce4-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="07ce4-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="07ce4-363">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="07ce4-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="07ce4-364">$0.93</span><span class="sxs-lookup"><span data-stu-id="07ce4-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-365">Currency</span><span class="sxs-lookup"><span data-stu-id="07ce4-365">Currency</span></span></td>
<td><p><span data-ttu-id="07ce4-366">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="07ce4-366">Currency type.</span></span> <span data-ttu-id="07ce4-367">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="07ce4-368">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="07ce4-369">EUR</span><span class="sxs-lookup"><span data-stu-id="07ce4-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="07ce4-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="07ce4-371">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="07ce4-371">Pretax price per unit.</span></span> <span data-ttu-id="07ce4-372">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="07ce4-373">$0.08</span><span class="sxs-lookup"><span data-stu-id="07ce4-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="07ce4-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="07ce4-375">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="07ce4-375">Post tax price per unit.</span></span> <span data-ttu-id="07ce4-376">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="07ce4-377">$0.08</span><span class="sxs-lookup"><span data-stu-id="07ce4-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="07ce4-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="07ce4-379">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-379">The type of charge or adjustment.</span></span> <span data-ttu-id="07ce4-380"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="07ce4-381"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="07ce4-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="07ce4-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="07ce4-383">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="07ce4-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="07ce4-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="07ce4-386">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="07ce4-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="07ce4-387">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="07ce4-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="07ce4-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="07ce4-389">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="07ce4-390">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="07ce4-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="07ce4-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="07ce4-392">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="07ce4-393">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="07ce4-394">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="07ce4-395">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="07ce4-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="07ce4-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="07ce4-397">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="07ce4-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="07ce4-398">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="07ce4-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-399">Project</span><span class="sxs-lookup"><span data-stu-id="07ce4-399">Project</span></span></td>
<td><p><span data-ttu-id="07ce4-400">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="07ce4-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="07ce4-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="07ce4-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="07ce4-403">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="07ce4-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="07ce4-404">예를 들어 30 일 동안 개별적으로 프로 비전 된 연결이 있는 경우 서비스 정보 1은 "1.000000 연결/30 일"을 읽습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="07ce4-405">프로 비전 된 ServiceBus 연결의 25 개가 있고 해당 일 동안 1을 사용한 경우 해당 일에 대 한 일일 사용 문은 "25 개의 연결/30 일 사용: 1.000000"을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="07ce4-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="07ce4-407">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="07ce4-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="07ce4-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="07ce4-409">DomainName</span></span></td>
<td><p><span data-ttu-id="07ce4-410">고객&#39;을 식별 하는 데 사용 되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="07ce4-411">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="07ce4-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="07ce4-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-413">Unit</span><span class="sxs-lookup"><span data-stu-id="07ce4-413">Unit</span></span></td>
<td><p><span data-ttu-id="07ce4-414">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="07ce4-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="07ce4-415">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="07ce4-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="07ce4-416">일회성 및 되풀이 파일 필드</span><span class="sxs-lookup"><span data-stu-id="07ce4-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="07ce4-417">Column</span><span class="sxs-lookup"><span data-stu-id="07ce4-417">Column</span></span></th>
<th><span data-ttu-id="07ce4-418">설명</span><span class="sxs-lookup"><span data-stu-id="07ce4-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="07ce4-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="07ce4-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="07ce4-420">특정 청구 엔터티에 대 한 고유 Microsoft Azure Active Directory 테 넌 트 식별자 (GUID 형식)입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="07ce4-421">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="07ce4-422">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-423">고객 Id</span><span class="sxs-lookup"><span data-stu-id="07ce4-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="07ce4-424">사용자를 식별 하는 데 사용 되는 GUID 형식의 고유한 Microsoft Azure Active Directory 테 넌 트 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-425">고객 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="07ce4-426">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="07ce4-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="07ce4-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="07ce4-428">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="07ce4-429">고객/파트너가 O365 포털을 통해 베 니 티/default 도메인을 업데이트할 수 있으므로 고객을 고유 하 게 식별 하는 데 사용 하면 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="07ce4-430">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-431">고객 국가</span><span class="sxs-lookup"><span data-stu-id="07ce4-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="07ce4-432">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-433">송장 번호</span><span class="sxs-lookup"><span data-stu-id="07ce4-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="07ce4-434">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="07ce4-435">MpnId</span></span></td>
<td><p><span data-ttu-id="07ce4-436">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-437">대리점 MpnId</span><span class="sxs-lookup"><span data-stu-id="07ce4-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="07ce4-438">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-439">주문 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-439">Order ID</span></span></td>
<td><p><span data-ttu-id="07ce4-440">Microsoft commerce platform의 주문에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="07ce4-441">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-442">주문 날짜</span><span class="sxs-lookup"><span data-stu-id="07ce4-442">Order date</span></span></td>
<td><p><span data-ttu-id="07ce4-443">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="07ce4-444">ProductId</span></span></td>
<td><p><span data-ttu-id="07ce4-445">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="07ce4-446">SkuId</span></span></td>
<td><p><span data-ttu-id="07ce4-447">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="07ce4-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="07ce4-449">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-449">The ID for a particular Availability.</span></span> <span data-ttu-id="07ce4-450">"가용성"은 특정 SKU를 특정 국가, 통화, 산업 부문 등에 구매할 수 있는지 여부를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-451">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="07ce4-452">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-453">제품 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-453">Product name</span></span></td>
<td><p><span data-ttu-id="07ce4-454">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="07ce4-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="07ce4-456">제품 게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="07ce4-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="07ce4-458">이 게시자에 대 한 고유 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-459">구독 설명</span><span class="sxs-lookup"><span data-stu-id="07ce4-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="07ce4-460">구독의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-461">구독 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="07ce4-462">Microsoft commerce platform의 구독에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="07ce4-463">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="07ce4-464">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="07ce4-466">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="07ce4-466">Start day of the charges.</span></span> <span data-ttu-id="07ce4-467">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="07ce4-469">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="07ce4-469">End day of the charges.</span></span> <span data-ttu-id="07ce4-470">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-471">용어 및 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="07ce4-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="07ce4-472">구매를 위한 용어 길이와 청구 주기입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="07ce4-473">예: "1 년, 월"</span><span class="sxs-lookup"><span data-stu-id="07ce4-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-474">청구 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="07ce4-475">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-476">단가</span><span class="sxs-lookup"><span data-stu-id="07ce4-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="07ce4-477">구매 시 가격표에 게시 된 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="07ce4-478">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-479">유효 단가</span><span class="sxs-lookup"><span data-stu-id="07ce4-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="07ce4-480">조정을 수행한 후 단가입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-481">Quantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-481">Quantity</span></span></td>
<td><p><span data-ttu-id="07ce4-482">단위 수입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-482">Number of units.</span></span> <span data-ttu-id="07ce4-483">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-484">단위 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-484">Unit type</span></span></td>
<td><p><span data-ttu-id="07ce4-485">구입할 단위의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="07ce4-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="07ce4-487">해당 할인에 대 한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-488">하위 합계</span><span class="sxs-lookup"><span data-stu-id="07ce4-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="07ce4-489">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="07ce4-489">Total before tax.</span></span> <span data-ttu-id="07ce4-490">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-491">세금 합계</span><span class="sxs-lookup"><span data-stu-id="07ce4-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="07ce4-492">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="07ce4-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-493">총액</span><span class="sxs-lookup"><span data-stu-id="07ce4-493">Total</span></span></td>
<td><p><span data-ttu-id="07ce4-494">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="07ce4-494">Total after tax.</span></span> <span data-ttu-id="07ce4-495">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-496">Currency</span><span class="sxs-lookup"><span data-stu-id="07ce4-496">Currency</span></span></td>
<td><p><span data-ttu-id="07ce4-497">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="07ce4-497">Currency type.</span></span> <span data-ttu-id="07ce4-498">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="07ce4-499">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="07ce4-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="07ce4-501">주문 ID에 대 한 대체 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="07ce4-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="07ce4-503">월간 청구를 사용 하는 경우 매월 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="07ce4-504">그렇지 않으면 빈 값입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="07ce4-506">구입 하거나 사용한 총 단위를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-507">pricingCurrency</span><span class="sxs-lookup"><span data-stu-id="07ce4-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="07ce4-508">리소스 또는 제품 가격을 나열 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="07ce4-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="07ce4-510">가격 책정 통화에 적용 된 환율 통화 (고객) 청구 통화</span><span class="sxs-lookup"><span data-stu-id="07ce4-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="07ce4-512">요금 청구 통화 환율이 결정 되는 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="07ce4-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="07ce4-514">소비 라인 항목에 대 한 측정기 설명</span><span class="sxs-lookup"><span data-stu-id="07ce4-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="07ce4-515">매일 등급 사용 파일 필드</span><span class="sxs-lookup"><span data-stu-id="07ce4-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="07ce4-516">Column</span><span class="sxs-lookup"><span data-stu-id="07ce4-516">Column</span></span></th>
<th><span data-ttu-id="07ce4-517">설명</span><span class="sxs-lookup"><span data-stu-id="07ce4-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="07ce4-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="07ce4-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="07ce4-519">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="07ce4-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="07ce4-521">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="07ce4-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="07ce4-523">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="07ce4-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="07ce4-525">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="07ce4-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="07ce4-526">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="07ce4-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="07ce4-528">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-528">The customer's domain name.</span></span> <span data-ttu-id="07ce4-529">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-530">고객 국가</span><span class="sxs-lookup"><span data-stu-id="07ce4-530">Customer country</span></span></td>
<td><p><span data-ttu-id="07ce4-531">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="07ce4-532">MPNID</span></span></td>
<td><p><span data-ttu-id="07ce4-533">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-534">대리점 MPNID</span><span class="sxs-lookup"><span data-stu-id="07ce4-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="07ce4-535">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="07ce4-536">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="07ce4-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="07ce4-538">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="07ce4-539">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="07ce4-540">ProductId</span></span></td>
<td><p><span data-ttu-id="07ce4-541">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="07ce4-542">SkuId</span></span></td>
<td><p><span data-ttu-id="07ce4-543">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="07ce4-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="07ce4-545">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-545">The ID for a particular Availability.</span></span> <span data-ttu-id="07ce4-546">"가용성"은 특정 SKU를 특정 국가, 통화, 산업 부문 등에 구매할 수 있는지 여부를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-547">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="07ce4-548">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="07ce4-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="07ce4-550">게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="07ce4-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="07ce4-552">GUID 형식의 게시자 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="07ce4-553">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-554">구독 설명</span><span class="sxs-lookup"><span data-stu-id="07ce4-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="07ce4-555">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="07ce4-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="07ce4-556">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="07ce4-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-557">구독 ID</span><span class="sxs-lookup"><span data-stu-id="07ce4-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="07ce4-558">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="07ce4-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="07ce4-559">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="07ce4-560">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="07ce4-562">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="07ce4-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="07ce4-563">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="07ce4-565">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="07ce4-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="07ce4-566">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-567">사용 날짜</span><span class="sxs-lookup"><span data-stu-id="07ce4-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="07ce4-568">서비스 사용 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-569">측정기 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="07ce4-570">측정기의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-571">미터 범주</span><span class="sxs-lookup"><span data-stu-id="07ce4-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="07ce4-572">사용에 대 한 최상위 수준 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-573">측정기 Id</span><span class="sxs-lookup"><span data-stu-id="07ce4-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="07ce4-574">사용 되는 측정기의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-575">미터 하위 범주</span><span class="sxs-lookup"><span data-stu-id="07ce4-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="07ce4-576">요금에 영향을 줄 수 있는 Azure 서비스의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-577">미터 이름</span><span class="sxs-lookup"><span data-stu-id="07ce4-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="07ce4-578">사용 되는 측정기에 대 한 측정 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-579">측정기 지역</span><span class="sxs-lookup"><span data-stu-id="07ce4-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="07ce4-580">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-581">Unit</span><span class="sxs-lookup"><span data-stu-id="07ce4-581">Unit</span></span></td>
<td><p><span data-ttu-id="07ce4-582">리소스 이름의 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-583">소비 된 수량</span><span class="sxs-lookup"><span data-stu-id="07ce4-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="07ce4-584">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="07ce4-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="07ce4-585">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-586">리소스 위치</span><span class="sxs-lookup"><span data-stu-id="07ce4-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="07ce4-587">측정기가 실행 되 고 있는 데이터 센터입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-588">사용 된 서비스</span><span class="sxs-lookup"><span data-stu-id="07ce4-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="07ce4-589">사용한 Azure 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="07ce4-590">리소스 URI</span><span class="sxs-lookup"><span data-stu-id="07ce4-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="07ce4-591">사용 되는 리소스의 URI입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-592">청구 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-592">Charge type</span></span></td>
<td><p><span data-ttu-id="07ce4-593">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-593">The type of charge or adjustment.</span></span> <span data-ttu-id="07ce4-594">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-595">단가</span><span class="sxs-lookup"><span data-stu-id="07ce4-595">Unit price</span></span></td>
<td><p><span data-ttu-id="07ce4-596">구매 시 가격표에 게시 된 라이선스 당 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="07ce4-597">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-598">Quantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-598">Quantity</span></span></td>
<td><p><span data-ttu-id="07ce4-599">라이선스의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-599">Number of licenses.</span></span> <span data-ttu-id="07ce4-600">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-601">단위 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-601">Unit type</span></span></td>
<td><p><span data-ttu-id="07ce4-602">미터의 요금이 청구 되는 단위 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="07ce4-603">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-604">청구 전 세금</span><span class="sxs-lookup"><span data-stu-id="07ce4-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="07ce4-605">세금 전 총 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-606">청구 통화</span><span class="sxs-lookup"><span data-stu-id="07ce4-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="07ce4-607">고객 지역의 통화</span><span class="sxs-lookup"><span data-stu-id="07ce4-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-608">가격 책정 pretax 합계</span><span class="sxs-lookup"><span data-stu-id="07ce4-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="07ce4-609">세금이 추가 되기 전의 가격 책정입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-610">가격 책정 통화</span><span class="sxs-lookup"><span data-stu-id="07ce4-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="07ce4-611">가격표의 통화입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-612">서비스 정보 1</span><span class="sxs-lookup"><span data-stu-id="07ce4-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="07ce4-613">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="07ce4-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="07ce4-614">서비스 정보 2</span><span class="sxs-lookup"><span data-stu-id="07ce4-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="07ce4-615">선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="07ce4-616">추가 정보</span><span class="sxs-lookup"><span data-stu-id="07ce4-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="07ce4-617">다른 열에서 다루지 않는 추가 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="07ce4-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="07ce4-619">단위당 청구 되는 실제 값 (할인, 획득 크레딧 등 포함)입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="07ce4-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="07ce4-621">가격 책정 통화에 대해 (고객) 청구 통화로 적용 되는 환율입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="07ce4-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="07ce4-623">청구 통화 환율에 대 한 가격 책정 통화를 결정 하는 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="07ce4-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="07ce4-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="07ce4-625">Azure subscriptionID를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="07ce4-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="07ce4-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="07ce4-627">Azure 구독의 이름을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="07ce4-628">청구서와 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="07ce4-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="07ce4-629">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="07ce4-630">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="07ce4-631">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="07ce4-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="07ce4-632">청구서에 "조정"으로 표시 되는 일회용 크레딧, 할인율 또는 환불 조정 파일에 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="07ce4-633">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="07ce4-634"><strong>송장 청구 설명</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-635"><strong>조정 파일 요금 설명 (Chargetcharcolumn)</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-636"><strong>이 요금은 어떻게 청구 되나요?</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-637"><strong>이러한 ChargeTypes을 청구서에 어떻게 할까요? 지도?</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="07ce4-638"><strong>라이선스 기반 요금</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-639">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-640">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="07ce4-641">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-642">취소 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-643">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-644">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="07ce4-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-645">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-646">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="07ce4-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-647">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-648">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-649">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="07ce4-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-650">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-651">연간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-652">구매 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-653">월간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형</span><span class="sxs-lookup"><span data-stu-id="07ce4-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-654">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-655">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="07ce4-656">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-657">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-658">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-659">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="07ce4-660"><strong>일회성 요금</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="07ce4-661">신규 항목</span><span class="sxs-lookup"><span data-stu-id="07ce4-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-662">새 구매가 생성 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-664">원래 구매 환불 및 증가 후 새로운 수량 모두에 사용 됨</span><span class="sxs-lookup"><span data-stu-id="07ce4-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="07ce4-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-666">원래 구매 환불 및 감소 후 새로운 수량 모두에 사용 됨</span><span class="sxs-lookup"><span data-stu-id="07ce4-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-667">취소</span><span class="sxs-lookup"><span data-stu-id="07ce4-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-668">구독이 취소 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-669">변환</span><span class="sxs-lookup"><span data-stu-id="07ce4-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-670">라이선스가 업그레이드 될 때 사용 되지만 사용자의 수는 변경 되지 않은 상태로 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ce4-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="07ce4-671"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-672">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="07ce4-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-673">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="07ce4-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="07ce4-674">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-675">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="07ce4-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-676">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="07ce4-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="07ce4-677"><strong>크레딧</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-678">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="07ce4-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-679">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="07ce4-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-680">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="07ce4-681">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="07ce4-682"><strong>사용량 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-683">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-684">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="07ce4-685">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-686">주기 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-687">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-688">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-689">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-690">취소 할인</span><span class="sxs-lookup"><span data-stu-id="07ce4-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-691">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="07ce4-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="07ce4-692"><strong>라이선스 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-693"><em>여러 요금 유형에 적용 될 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="07ce4-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="07ce4-694">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="07ce4-695"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="07ce4-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-696"><em>여러 요금 유형에 적용 될 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="07ce4-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="07ce4-697"><em>예외: 줄 항목 &quot;에 세금이 이미 포함 되어 &quot;Offset. 위의 크레딧을 참조 하세요.</em></span><span class="sxs-lookup"><span data-stu-id="07ce4-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-698">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="07ce4-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="07ce4-699">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="07ce4-700">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="07ce4-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
