---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 07/08/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 보려면 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 7b27e99e5c0dc55fad3b06cc22316e8282dbe35c
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653981"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="45e3b-103">조정 파일 사용</span><span class="sxs-lookup"><span data-stu-id="45e3b-103">Use the reconciliation files</span></span>

<span data-ttu-id="45e3b-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="45e3b-104">**Applies to**</span></span>

-  <span data-ttu-id="45e3b-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="45e3b-105">Partner Center</span></span>
-  <span data-ttu-id="45e3b-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="45e3b-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="45e3b-107">청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 보려면 파트너 센터에서 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="45e3b-108">세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="45e3b-109">서식 지정 문제</span><span class="sxs-lookup"><span data-stu-id="45e3b-109">Formatting issues</span></span>

<span data-ttu-id="45e3b-110">경우에 따라 정찰 파일에 서식 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="45e3b-111">이는 예를 들어 EN-US 로캘이 사용 되지 않는 경우에 발생할 수 있습니다. 이러한 문제를 해결 하려면 아래 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="45e3b-112">Excel에서 .csv 파일을 열고 첫 번째 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="45e3b-113">리본 메뉴에서 <strong>데이터</strong>를 선택 하 고 <strong>열 텍스트를</strong>선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="45e3b-114">텍스트를 열로 변환 마법사에서 구분 된 <strong>파일 형식</strong>을 선택 하 고 <strong>다음</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="45e3b-115">구분 기호 필드에서 <strong>쉼표</strong>를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="45e3b-116"><strong>탭</strong> 이 이미 선택 되어 있으면 그대로 둘 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="45e3b-117"><strong>다음</strong>을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="45e3b-118">열 데이터 형식 필드에서 <strong>Date: MDY</strong>를 선택 하 고 <strong>다음</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="45e3b-119">열 데이터 형식 필드에서 모든 금액 열에 대해 <strong>텍스트</strong> 를 선택한 다음 <strong>마침</strong>을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="45e3b-120">Large 정찰 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="45e3b-120">Downloading a large recon file</span></span>

<span data-ttu-id="45e3b-121">정찰 파일은 매우 커질 수 있으며 다운로드 하기도 어렵습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="45e3b-122">대량 정찰 파일을 다운로드 하는 데 도움이 되는 PowerShell 스크립트는 [청구서 품목 가져오기 항목](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="45e3b-123">파트너 기준 항목별로</span><span class="sxs-lookup"><span data-stu-id="45e3b-123">Itemize by partner</span></span>


<span data-ttu-id="45e3b-124">간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="45e3b-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-125">MPN ID</span></span></th>
<th><span data-ttu-id="45e3b-126">설명</span><span class="sxs-lookup"><span data-stu-id="45e3b-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="45e3b-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="45e3b-128">CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</span><span class="sxs-lookup"><span data-stu-id="45e3b-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-129">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="45e3b-130">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="45e3b-131">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="45e3b-132">파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="45e3b-133">eTo를 보거나 업데이트 하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음, 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="45e3b-134">고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="45e3b-135"><strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="45e3b-136">CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="45e3b-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="45e3b-137">CSP 파트너에 MPN ID가 없는 재판매인이 있는 경우이 값은 파트너의 MPN ID로 대신 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="45e3b-138">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="45e3b-139">라이선스 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="45e3b-139">License-based file fields</span></span>


<span data-ttu-id="45e3b-140">고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="45e3b-141"><strong>열의</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="45e3b-142"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="45e3b-143"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="45e3b-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="45e3b-145">특정 청구 엔터티의 고유 식별자(GUID 형식).</span><span class="sxs-lookup"><span data-stu-id="45e3b-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="45e3b-146">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="45e3b-147">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="45e3b-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="45e3b-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="45e3b-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="45e3b-150">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="45e3b-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="45e3b-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="45e3b-152">OrderID</span></span></td>
<td><p><span data-ttu-id="45e3b-153">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="45e3b-154">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="45e3b-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="45e3b-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="45e3b-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="45e3b-157">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="45e3b-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="45e3b-158">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="45e3b-159">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="45e3b-160">Syndication_Partner_Subscription_Number를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="45e3b-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="45e3b-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="45e3b-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="45e3b-163">구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="45e3b-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="45e3b-164">고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="45e3b-165">이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="45e3b-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="45e3b-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="45e3b-167">OfferID</span></span></td>
<td><p><span data-ttu-id="45e3b-168">고유 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="45e3b-168">Unique offer ID.</span></span> <span data-ttu-id="45e3b-169">가격표에 따른 표준 제품 ID.</span><span class="sxs-lookup"><span data-stu-id="45e3b-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="45e3b-170"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="45e3b-171">아래의 DurableOfferID를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="45e3b-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="45e3b-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="45e3b-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="45e3b-174">고유 지속형 제품 ID(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="45e3b-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="45e3b-175"><b>참고</b>: 이 값은 가격 목록의 제품 ID와 일치합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="45e3b-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="45e3b-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="45e3b-177">OfferName</span></span></td>
<td><p><span data-ttu-id="45e3b-178">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="45e3b-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="45e3b-179">Microsoft Office 365(계획 E3)</span><span class="sxs-lookup"><span data-stu-id="45e3b-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="45e3b-181">구독 시작 날짜(주문이 제출된 다음 날로 설정됨).</span><span class="sxs-lookup"><span data-stu-id="45e3b-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="45e3b-182">구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="45e3b-183">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="45e3b-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="45e3b-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="45e3b-186">구독 종료 날짜: 12개월 + 시작 날짜 이후 x일(파트너 청구 날짜에 맞추기 위해) 또는 갱신 날짜로부터 12개월.</span><span class="sxs-lookup"><span data-stu-id="45e3b-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="45e3b-187">갱신 시 가격은 현재 가격표로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="45e3b-188">자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="45e3b-189">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="45e3b-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="45e3b-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="45e3b-192">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="45e3b-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="45e3b-193">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="45e3b-194">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="45e3b-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="45e3b-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="45e3b-197">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="45e3b-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="45e3b-198">고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="45e3b-199">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="45e3b-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="45e3b-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="45e3b-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="45e3b-202">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-202">The type of charge or adjustment.</span></span> <span data-ttu-id="45e3b-203"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="45e3b-204"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="45e3b-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="45e3b-206">실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음.</span><span class="sxs-lookup"><span data-stu-id="45e3b-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="45e3b-207">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="45e3b-208">6.82</span><span class="sxs-lookup"><span data-stu-id="45e3b-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-209">Quantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-209">Quantity</span></span></td>
<td><p><span data-ttu-id="45e3b-210">실제 사용자 수.</span><span class="sxs-lookup"><span data-stu-id="45e3b-210">Number of seats.</span></span> <span data-ttu-id="45e3b-211">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="45e3b-212">2</span><span class="sxs-lookup"><span data-stu-id="45e3b-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-213">합계</span><span class="sxs-lookup"><span data-stu-id="45e3b-213">Amount</span></span></td>
<td><p><span data-ttu-id="45e3b-214">수량의 가격 합계.</span><span class="sxs-lookup"><span data-stu-id="45e3b-214">Total of price for quantity.</span></span> <span data-ttu-id="45e3b-215">금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="45e3b-216">13.32</span><span class="sxs-lookup"><span data-stu-id="45e3b-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="45e3b-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="45e3b-218">이러한 요금에 적용된 할인 금액.</span><span class="sxs-lookup"><span data-stu-id="45e3b-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="45e3b-219">역량 또는 맵과 함께 제공 되는 제품 라이선스 또는 동기에 적합 한 새 구독은이 열에 할인 금액을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="45e3b-220">2.32</span><span class="sxs-lookup"><span data-stu-id="45e3b-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="45e3b-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="45e3b-222">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="45e3b-222">Total before tax.</span></span> <span data-ttu-id="45e3b-223">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="45e3b-224">11</span><span class="sxs-lookup"><span data-stu-id="45e3b-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-225">Tax</span><span class="sxs-lookup"><span data-stu-id="45e3b-225">Tax</span></span></td>
<td><p><span data-ttu-id="45e3b-226">시장의&#39;세금 규칙 및 특정 상황에 따라 세금 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="45e3b-227">0</span><span class="sxs-lookup"><span data-stu-id="45e3b-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="45e3b-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="45e3b-229">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="45e3b-229">Total after tax.</span></span> <span data-ttu-id="45e3b-230">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="45e3b-231">11</span><span class="sxs-lookup"><span data-stu-id="45e3b-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-232">Currency</span><span class="sxs-lookup"><span data-stu-id="45e3b-232">Currency</span></span></td>
<td><p><span data-ttu-id="45e3b-233">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="45e3b-233">Currency type.</span></span> <span data-ttu-id="45e3b-234">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="45e3b-235">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="45e3b-236">EUR</span><span class="sxs-lookup"><span data-stu-id="45e3b-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="45e3b-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="45e3b-238">파트너&#39;센터에 보고 된 고객의 조직 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="45e3b-239">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="45e3b-240">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="45e3b-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="45e3b-241">MPNID</span></span></td>
<td><p><span data-ttu-id="45e3b-242">CSP 파트너의 MPN ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="45e3b-243">4390934</span><span class="sxs-lookup"><span data-stu-id="45e3b-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="45e3b-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="45e3b-245">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="45e3b-246"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="45e3b-247">4390934</span><span class="sxs-lookup"><span data-stu-id="45e3b-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="45e3b-248">DomainName</span></span></td>
<td><p><span data-ttu-id="45e3b-249">고객&#39;을 식별 하는 데 사용 되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="45e3b-250">고객/파트너가 O365 포털을 통해 베 니 티/default 도메인을 업데이트할 수 있으므로 고객을 고유 하 게 식별 하는 데 사용 하면 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="45e3b-251">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="45e3b-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="45e3b-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="45e3b-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="45e3b-254">구독 애칭.</span><span class="sxs-lookup"><span data-stu-id="45e3b-254">Subscription nickname.</span></span> <span data-ttu-id="45e3b-255">애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="45e3b-256">프로젝트 온라인</span><span class="sxs-lookup"><span data-stu-id="45e3b-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="45e3b-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="45e3b-258">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="45e3b-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="45e3b-259">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="45e3b-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="45e3b-260">프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</span><span class="sxs-lookup"><span data-stu-id="45e3b-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="45e3b-261">사용 기반 파일 필드</span><span class="sxs-lookup"><span data-stu-id="45e3b-261">Usage-based file fields</span></span>


<span data-ttu-id="45e3b-262">고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="45e3b-263">다음 필드에서는 사용된 서비스와 요금을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="45e3b-264"><strong>열의</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="45e3b-265"><strong>설명</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="45e3b-266"><strong>샘플 값</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="45e3b-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="45e3b-268">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="45e3b-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="45e3b-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="45e3b-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="45e3b-271">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="45e3b-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="45e3b-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="45e3b-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="45e3b-274">파트너 계정 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="45e3b-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="45e3b-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="45e3b-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="45e3b-277">파트너&#39;센터에 보고 된 고객의 조직 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="45e3b-278">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="45e3b-279">테스트 고객 A</span><span class="sxs-lookup"><span data-stu-id="45e3b-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="45e3b-280">MPNID</span></span></td>
<td><p><span data-ttu-id="45e3b-281">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="45e3b-282">4390934</span><span class="sxs-lookup"><span data-stu-id="45e3b-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="45e3b-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="45e3b-284">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="45e3b-285"><a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="45e3b-286">4390934</span><span class="sxs-lookup"><span data-stu-id="45e3b-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="45e3b-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="45e3b-288">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="45e3b-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="45e3b-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="45e3b-291">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="45e3b-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="45e3b-292">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="45e3b-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="45e3b-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="45e3b-295">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="45e3b-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="45e3b-296">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="45e3b-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="45e3b-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="45e3b-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="45e3b-299">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="45e3b-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="45e3b-300">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="45e3b-301">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="45e3b-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="45e3b-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="45e3b-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="45e3b-304">서비스의 애칭.</span><span class="sxs-lookup"><span data-stu-id="45e3b-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="45e3b-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="45e3b-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="45e3b-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="45e3b-307">서비스 제품의 LOB(기간 업무)</span><span class="sxs-lookup"><span data-stu-id="45e3b-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="45e3b-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="45e3b-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="45e3b-309">OrderID</span></span></td>
<td><p><span data-ttu-id="45e3b-310">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="45e3b-311">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="45e3b-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="45e3b-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="45e3b-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="45e3b-314">해당 Azure 서비스의 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="45e3b-315">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="45e3b-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="45e3b-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="45e3b-317">Microsoft Azure 서비스의 특정 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="45e3b-318">Service Bus 개인 또는 팩</span><span class="sxs-lookup"><span data-stu-id="45e3b-318">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="45e3b-319">SQL Azure database-Business 또는 Web Edition</span><span class="sxs-lookup"><span data-stu-id="45e3b-319">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="45e3b-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="45e3b-321">모든 서비스 데이터 및 가격 책정 구조에 대한 특정 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="45e3b-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="45e3b-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="45e3b-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="45e3b-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="45e3b-324">Azure 리소스의 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="45e3b-325">데이터 수신(GB)</span><span class="sxs-lookup"><span data-stu-id="45e3b-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="45e3b-326">데이터 발신(GB)</span><span class="sxs-lookup"><span data-stu-id="45e3b-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-327">국가</span><span class="sxs-lookup"><span data-stu-id="45e3b-327">Region</span></span></td>
<td><p><span data-ttu-id="45e3b-328">사용이 적용되는 지역입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-328">The region the usage applies to.</span></span> <span data-ttu-id="45e3b-329">요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="45e3b-330">아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</span><span class="sxs-lookup"><span data-stu-id="45e3b-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-331">SKU</span><span class="sxs-lookup"><span data-stu-id="45e3b-331">SKU</span></span></td>
<td><p><span data-ttu-id="45e3b-332">제품에 대한 MSFT 고유 식별자</span><span class="sxs-lookup"><span data-stu-id="45e3b-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="45e3b-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="45e3b-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="45e3b-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="45e3b-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="45e3b-335">지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량.</span><span class="sxs-lookup"><span data-stu-id="45e3b-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="45e3b-336">Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="45e3b-337">1</span><span class="sxs-lookup"><span data-stu-id="45e3b-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="45e3b-339">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="45e3b-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="45e3b-340">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="45e3b-341">11</span><span class="sxs-lookup"><span data-stu-id="45e3b-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="45e3b-343">제품의 일부로 포함된 단위.</span><span class="sxs-lookup"><span data-stu-id="45e3b-343">Units included as part of the offer.</span></span> <span data-ttu-id="45e3b-344">일반적으로 CSP에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="45e3b-345">0</span><span class="sxs-lookup"><span data-stu-id="45e3b-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="45e3b-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="45e3b-347">제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</span><span class="sxs-lookup"><span data-stu-id="45e3b-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="45e3b-348">ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="45e3b-349">11</span><span class="sxs-lookup"><span data-stu-id="45e3b-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="45e3b-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="45e3b-351">구독 시작 날짜에 유효한 제품 가격</span><span class="sxs-lookup"><span data-stu-id="45e3b-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="45e3b-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="45e3b-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="45e3b-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="45e3b-354">ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="45e3b-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="45e3b-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="45e3b-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="45e3b-357">시장의&#39;세금 규칙 및 특정 상황에 따라 세금 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="45e3b-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="45e3b-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="45e3b-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="45e3b-360">세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</span><span class="sxs-lookup"><span data-stu-id="45e3b-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="45e3b-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="45e3b-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-362">Currency</span><span class="sxs-lookup"><span data-stu-id="45e3b-362">Currency</span></span></td>
<td><p><span data-ttu-id="45e3b-363">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="45e3b-363">Currency type.</span></span> <span data-ttu-id="45e3b-364">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="45e3b-365">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="45e3b-366">EUR</span><span class="sxs-lookup"><span data-stu-id="45e3b-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="45e3b-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="45e3b-368">세전 단가.</span><span class="sxs-lookup"><span data-stu-id="45e3b-368">Pretax price per unit.</span></span> <span data-ttu-id="45e3b-369">PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="45e3b-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="45e3b-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="45e3b-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="45e3b-372">세후 단가.</span><span class="sxs-lookup"><span data-stu-id="45e3b-372">Post tax price per unit.</span></span> <span data-ttu-id="45e3b-373">PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="45e3b-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="45e3b-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="45e3b-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="45e3b-376">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-376">The type of charge or adjustment.</span></span> <span data-ttu-id="45e3b-377"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="45e3b-378"><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="45e3b-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="45e3b-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="45e3b-380">MSFT 청구 플랫폼에서 고유한 계정 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="45e3b-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="45e3b-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="45e3b-383">서비스 배포 날짜</span><span class="sxs-lookup"><span data-stu-id="45e3b-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="45e3b-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="45e3b-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="45e3b-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="45e3b-386">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="45e3b-387">동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</span><span class="sxs-lookup"><span data-stu-id="45e3b-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="45e3b-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="45e3b-389">이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="45e3b-390">예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="45e3b-391">이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="45e3b-392">AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</span><span class="sxs-lookup"><span data-stu-id="45e3b-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="45e3b-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="45e3b-394">개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</span><span class="sxs-lookup"><span data-stu-id="45e3b-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="45e3b-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="45e3b-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-396">Project</span><span class="sxs-lookup"><span data-stu-id="45e3b-396">Project</span></span></td>
<td><p><span data-ttu-id="45e3b-397">해당 서비스 인스턴스에 대한 고객 정의 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="45e3b-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="45e3b-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="45e3b-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="45e3b-400">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="45e3b-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="45e3b-401">예를 들어 30 일 동안 개별적으로 프로 비전 된 연결이 있는 경우 서비스 정보 1은 "1.000000 연결/30 일"을 읽습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="45e3b-402">프로 비전 된 ServiceBus 연결의 25 개가 있고 해당 일 동안 1을 사용한 경우 해당 일에 대 한 일일 사용 문은 "25 개의 연결/30 일 사용: 1.000000"을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="45e3b-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="45e3b-404">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="45e3b-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="45e3b-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="45e3b-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="45e3b-406">DomainName</span></span></td>
<td><p><span data-ttu-id="45e3b-407">고객&#39;을 식별 하는 데 사용 되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="45e3b-408">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="45e3b-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="45e3b-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="45e3b-410">Unit</span><span class="sxs-lookup"><span data-stu-id="45e3b-410">Unit</span></span></td>
<td><p><span data-ttu-id="45e3b-411">리소스 이름의 단위</span><span class="sxs-lookup"><span data-stu-id="45e3b-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="45e3b-412">GB 또는 시간</span><span class="sxs-lookup"><span data-stu-id="45e3b-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="45e3b-413">일회성 및 되풀이 파일 필드</span><span class="sxs-lookup"><span data-stu-id="45e3b-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="45e3b-414">Column</span><span class="sxs-lookup"><span data-stu-id="45e3b-414">Column</span></span></th>
<th><span data-ttu-id="45e3b-415">설명</span><span class="sxs-lookup"><span data-stu-id="45e3b-415">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="45e3b-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="45e3b-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="45e3b-417">특정 청구 엔터티에 대 한 고유 Microsoft Azure Active Directory 테 넌 트 식별자 (GUID 형식)입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="45e3b-418">조정에는 필요하지 않지만 유용한 정보일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="45e3b-419">모든 행에서 같습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-420">고객 Id</span><span class="sxs-lookup"><span data-stu-id="45e3b-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="45e3b-421">사용자를 식별 하는 데 사용 되는 GUID 형식의 고유한 Microsoft Azure Active Directory 테 넌 트 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-422">고객 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="45e3b-423">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="45e3b-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="45e3b-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="45e3b-425">고객을 식별하는 데 사용되는 고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="45e3b-426">고객/파트너가 O365 포털을 통해 베 니 티/default 도메인을 업데이트할 수 있으므로 고객을 고유 하 게 식별 하는 데 사용 하면 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="45e3b-427">두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-428">고객 국가</span><span class="sxs-lookup"><span data-stu-id="45e3b-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="45e3b-429">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-430">송장 번호</span><span class="sxs-lookup"><span data-stu-id="45e3b-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="45e3b-431">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="45e3b-432">MpnId</span></span></td>
<td><p><span data-ttu-id="45e3b-433">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-434">대리점 MpnId</span><span class="sxs-lookup"><span data-stu-id="45e3b-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="45e3b-435">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-436">주문 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-436">Order ID</span></span></td>
<td><p><span data-ttu-id="45e3b-437">Microsoft commerce platform의 주문에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="45e3b-438">지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-439">주문 날짜</span><span class="sxs-lookup"><span data-stu-id="45e3b-439">Order date</span></span></td>
<td><p><span data-ttu-id="45e3b-440">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="45e3b-441">ProductId</span></span></td>
<td><p><span data-ttu-id="45e3b-442">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="45e3b-443">SkuId</span></span></td>
<td><p><span data-ttu-id="45e3b-444">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="45e3b-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="45e3b-446">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-446">The ID for a particular Availability.</span></span> <span data-ttu-id="45e3b-447">"가용성"은 특정 SKU를 특정 국가, 통화, 산업 부문 등에 구매할 수 있는지 여부를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-447">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-448">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="45e3b-449">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-450">제품 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-450">Product name</span></span></td>
<td><p><span data-ttu-id="45e3b-451">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="45e3b-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="45e3b-453">제품 게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-453">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="45e3b-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="45e3b-455">이 게시자에 대 한 고유 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-456">구독 설명</span><span class="sxs-lookup"><span data-stu-id="45e3b-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="45e3b-457">구독의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-458">구독 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="45e3b-459">Microsoft commerce platform의 구독에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="45e3b-460">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="45e3b-461">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="45e3b-463">요금 시작일.</span><span class="sxs-lookup"><span data-stu-id="45e3b-463">Start day of the charges.</span></span> <span data-ttu-id="45e3b-464">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="45e3b-466">요금 종료일.</span><span class="sxs-lookup"><span data-stu-id="45e3b-466">End day of the charges.</span></span> <span data-ttu-id="45e3b-467">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-468">용어 및 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="45e3b-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="45e3b-469">구매를 위한 용어 길이와 청구 주기입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="45e3b-470">예: "1 년, 월"</span><span class="sxs-lookup"><span data-stu-id="45e3b-470">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-471">청구 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="45e3b-472">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-473">단가</span><span class="sxs-lookup"><span data-stu-id="45e3b-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="45e3b-474">구매 시 가격표에 게시 된 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="45e3b-475">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-476">유효 단가</span><span class="sxs-lookup"><span data-stu-id="45e3b-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="45e3b-477">조정을 수행한 후 단가입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-478">Quantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-478">Quantity</span></span></td>
<td><p><span data-ttu-id="45e3b-479">단위 수입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-479">Number of units.</span></span> <span data-ttu-id="45e3b-480">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-481">단위 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-481">Unit type</span></span></td>
<td><p><span data-ttu-id="45e3b-482">구입할 단위의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="45e3b-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="45e3b-484">해당 할인에 대 한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-485">하위 합계</span><span class="sxs-lookup"><span data-stu-id="45e3b-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="45e3b-486">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="45e3b-486">Total before tax.</span></span> <span data-ttu-id="45e3b-487">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-488">세금 합계</span><span class="sxs-lookup"><span data-stu-id="45e3b-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="45e3b-489">해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</span><span class="sxs-lookup"><span data-stu-id="45e3b-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-490">총액</span><span class="sxs-lookup"><span data-stu-id="45e3b-490">Total</span></span></td>
<td><p><span data-ttu-id="45e3b-491">세금을 적용한 후의 총액.</span><span class="sxs-lookup"><span data-stu-id="45e3b-491">Total after tax.</span></span> <span data-ttu-id="45e3b-492">송장에 세금이 부과되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-493">Currency</span><span class="sxs-lookup"><span data-stu-id="45e3b-493">Currency</span></span></td>
<td><p><span data-ttu-id="45e3b-494">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="45e3b-494">Currency type.</span></span> <span data-ttu-id="45e3b-495">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="45e3b-496">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="45e3b-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="45e3b-498">주문 ID에 대 한 대체 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-499">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="45e3b-499">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="45e3b-500">월간 청구를 사용 하는 경우 매월 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-500">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="45e3b-501">그렇지 않으면 빈 값입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-501">Otherwise blank.</span></span> </p></td>
</tr>

</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="45e3b-502">매일 등급 사용 파일 필드</span><span class="sxs-lookup"><span data-stu-id="45e3b-502">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="45e3b-503">Column</span><span class="sxs-lookup"><span data-stu-id="45e3b-503">Column</span></span></th>
<th><span data-ttu-id="45e3b-504">설명</span><span class="sxs-lookup"><span data-stu-id="45e3b-504">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="45e3b-505">PartnerId</span><span class="sxs-lookup"><span data-stu-id="45e3b-505">PartnerId</span></span></td>
<td><p><span data-ttu-id="45e3b-506">GUID 형식의 파트너 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-506">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-507">PartnerName</span><span class="sxs-lookup"><span data-stu-id="45e3b-507">PartnerName</span></span></td>
<td><p><span data-ttu-id="45e3b-508">파트너 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-508">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-509">CustomerId</span><span class="sxs-lookup"><span data-stu-id="45e3b-509">CustomerId</span></span></td>
<td><p><span data-ttu-id="45e3b-510">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-510">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-511">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="45e3b-511">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="45e3b-512">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="45e3b-512">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="45e3b-513">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-513">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-514">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="45e3b-514">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="45e3b-515">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-515">The customer's domain name.</span></span> <span data-ttu-id="45e3b-516">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-516">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-517">고객 국가</span><span class="sxs-lookup"><span data-stu-id="45e3b-517">Customer country</span></span></td>
<td><p><span data-ttu-id="45e3b-518">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-518">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-519">MPNID</span><span class="sxs-lookup"><span data-stu-id="45e3b-519">MPNID</span></span></td>
<td><p><span data-ttu-id="45e3b-520">CSP 파트너의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-520">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-521">대리점 MPNID</span><span class="sxs-lookup"><span data-stu-id="45e3b-521">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="45e3b-522">구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-522">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="45e3b-523">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-524">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="45e3b-524">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="45e3b-525">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-525">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="45e3b-526">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-526">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-527">ProductId</span><span class="sxs-lookup"><span data-stu-id="45e3b-527">ProductId</span></span></td>
<td><p><span data-ttu-id="45e3b-528">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-528">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-529">SkuId</span><span class="sxs-lookup"><span data-stu-id="45e3b-529">SkuId</span></span></td>
<td><p><span data-ttu-id="45e3b-530">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-530">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-531">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="45e3b-531">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="45e3b-532">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-532">The ID for a particular Availability.</span></span> <span data-ttu-id="45e3b-533">"가용성"은 특정 SKU를 특정 국가, 통화, 산업 부문 등에 구매할 수 있는지 여부를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-533">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-534">SKU 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-534">SKU Name</span></span></td>
<td><p><span data-ttu-id="45e3b-535">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-535">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-536">PublisherName</span><span class="sxs-lookup"><span data-stu-id="45e3b-536">PublisherName</span></span></td>
<td><p><span data-ttu-id="45e3b-537">게시자의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-537">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-538">PublisherID</span><span class="sxs-lookup"><span data-stu-id="45e3b-538">PublisherID</span></span></td>
<td><p><span data-ttu-id="45e3b-539">GUID 형식의 게시자 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-539">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="45e3b-540">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-540">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-541">구독 설명</span><span class="sxs-lookup"><span data-stu-id="45e3b-541">Subscription Description</span></span></td>
<td><p><span data-ttu-id="45e3b-542">고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</span><span class="sxs-lookup"><span data-stu-id="45e3b-542">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="45e3b-543">(제품 이름과 동일한 필드).</span><span class="sxs-lookup"><span data-stu-id="45e3b-543">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-544">구독 ID</span><span class="sxs-lookup"><span data-stu-id="45e3b-544">Subscription ID</span></span></td>
<td><p><span data-ttu-id="45e3b-545">Microsoft 청구 플랫폼에서 구독의 고유 식별자.</span><span class="sxs-lookup"><span data-stu-id="45e3b-545">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="45e3b-546">지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-546">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="45e3b-547">이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-547">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-548">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-548">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="45e3b-549">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</span><span class="sxs-lookup"><span data-stu-id="45e3b-549">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="45e3b-550">시간은 항상 해당하는 날의 시작인 0:00입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-550">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-551">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="45e3b-551">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="45e3b-552">이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</span><span class="sxs-lookup"><span data-stu-id="45e3b-552">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="45e3b-553">시간은 항상 해당 일의 마지막인 23:59입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-553">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-554">사용 날짜</span><span class="sxs-lookup"><span data-stu-id="45e3b-554">Usage Date</span></span></td>
<td><p><span data-ttu-id="45e3b-555">서비스 사용 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-555">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-556">측정기 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-556">Meter Type</span></span></td>
<td><p><span data-ttu-id="45e3b-557">측정기의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-557">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-558">미터 범주</span><span class="sxs-lookup"><span data-stu-id="45e3b-558">Meter Category</span></span></td>
<td><p><span data-ttu-id="45e3b-559">사용에 대 한 최상위 수준 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-559">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-560">측정기 Id</span><span class="sxs-lookup"><span data-stu-id="45e3b-560">Meter Id</span></span></td>
<td><p><span data-ttu-id="45e3b-561">사용 되는 측정기의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-561">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-562">미터 하위 범주</span><span class="sxs-lookup"><span data-stu-id="45e3b-562">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="45e3b-563">요금에 영향을 줄 수 있는 Azure 서비스의 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-563">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-564">미터 이름</span><span class="sxs-lookup"><span data-stu-id="45e3b-564">Meter Name</span></span></td>
<td><p><span data-ttu-id="45e3b-565">사용 되는 측정기에 대 한 측정 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-565">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-566">측정기 지역</span><span class="sxs-lookup"><span data-stu-id="45e3b-566">Meter Region</span></span></td>
<td><p><span data-ttu-id="45e3b-567">이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-567">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-568">Unit</span><span class="sxs-lookup"><span data-stu-id="45e3b-568">Unit</span></span></td>
<td><p><span data-ttu-id="45e3b-569">리소스 이름의 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-569">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-570">소비 된 수량</span><span class="sxs-lookup"><span data-stu-id="45e3b-570">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="45e3b-571">보고 기간 중 소비된 서비스 양(시간, GB 등).</span><span class="sxs-lookup"><span data-stu-id="45e3b-571">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="45e3b-572">이전 보고 기간의 미청구 사용량도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-572">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-573">리소스 위치</span><span class="sxs-lookup"><span data-stu-id="45e3b-573">Resource Location</span></span></td>
<td><p><span data-ttu-id="45e3b-574">측정기가 실행 되 고 있는 데이터 센터입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-574">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-575">사용 된 서비스</span><span class="sxs-lookup"><span data-stu-id="45e3b-575">Consumed Service</span></span></td>
<td><p><span data-ttu-id="45e3b-576">사용한 Azure 플랫폼 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-576">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="45e3b-577">리소스 URI</span><span class="sxs-lookup"><span data-stu-id="45e3b-577">Resource URI</span></span></td>
<td><p><span data-ttu-id="45e3b-578">사용 되는 리소스의 URI입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-578">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-579">청구 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-579">Charge type</span></span></td>
<td><p><span data-ttu-id="45e3b-580">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-580">The type of charge or adjustment.</span></span> <span data-ttu-id="45e3b-581">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-581">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-582">단가</span><span class="sxs-lookup"><span data-stu-id="45e3b-582">Unit price</span></span></td>
<td><p><span data-ttu-id="45e3b-583">구매 시 가격표에 게시 된 라이선스 당 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-583">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="45e3b-584">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-585">Quantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-585">Quantity</span></span></td>
<td><p><span data-ttu-id="45e3b-586">라이선스의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-586">Number of licenses.</span></span> <span data-ttu-id="45e3b-587">조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-587">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-588">단위 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-588">Unit type</span></span></td>
<td><p><span data-ttu-id="45e3b-589">미터의 요금이 청구 되는 단위 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-589">The type of unit the meter is charged in.</span></span> <span data-ttu-id="45e3b-590">현재 활동에 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-590">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-591">청구 전 세금</span><span class="sxs-lookup"><span data-stu-id="45e3b-591">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="45e3b-592">세금 전 총 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-592">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-593">청구 통화</span><span class="sxs-lookup"><span data-stu-id="45e3b-593">Billing currency</span></span></td>
<td><p><span data-ttu-id="45e3b-594">고객 지역의 통화</span><span class="sxs-lookup"><span data-stu-id="45e3b-594">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-595">가격 책정 pretax 합계</span><span class="sxs-lookup"><span data-stu-id="45e3b-595">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="45e3b-596">세금이 추가 되기 전의 가격 책정입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-596">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-597">가격 책정 통화</span><span class="sxs-lookup"><span data-stu-id="45e3b-597">Pricing currency</span></span></td>
<td><p><span data-ttu-id="45e3b-598">가격표의 통화입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-598">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="45e3b-599">서비스 정보 1</span><span class="sxs-lookup"><span data-stu-id="45e3b-599">Service Info 1</span></span></td>
<td><p><span data-ttu-id="45e3b-600">지정일에 프로비전 및 사용된 ServiceBus 연결 수</span><span class="sxs-lookup"><span data-stu-id="45e3b-600">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-601">서비스 정보 2</span><span class="sxs-lookup"><span data-stu-id="45e3b-601">Service Info 2</span></span></td>
<td><p><span data-ttu-id="45e3b-602">선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-602">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="45e3b-603">추가 정보</span><span class="sxs-lookup"><span data-stu-id="45e3b-603">Additional Info</span></span></td>
<td><p><span data-ttu-id="45e3b-604">다른 열에서 다루지 않는 추가 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-604">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="45e3b-605">청구서와 조정 파일 간 요금 매핑</span><span class="sxs-lookup"><span data-stu-id="45e3b-605">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="45e3b-606">송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-606">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="45e3b-607">송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-607">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="45e3b-608">사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위).</span><span class="sxs-lookup"><span data-stu-id="45e3b-608">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="45e3b-609">청구서에 "조정"으로 표시 되는 일회용 크레딧, 할인율 또는 환불 조정 파일에 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-609">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="45e3b-610">아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-610">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="45e3b-611"><strong>송장 청구 설명</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-611"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-612"><strong>조정 파일 요금 설명 (Chargetcharcolumn)</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-612"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-613"><strong>이 요금은 어떻게 청구 되나요?</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-613"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-614"><strong>이러한 ChargeTypes을 청구서에 어떻게 할까요? 지도?</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-614"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="45e3b-615"><strong>라이선스 기반 요금</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-615"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-616">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-616">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-617">고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-617">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="45e3b-618">라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-618">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-619">취소 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-619">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-620">연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-620">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-621">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="45e3b-621">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-622">구독에 대한 정기 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-622">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-623">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="45e3b-623">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-624">연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-624">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-625">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-625">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-626">취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</span><span class="sxs-lookup"><span data-stu-id="45e3b-626">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-627">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-627">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-628">연간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-628">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-629">구매 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-629">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-630">월간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형</span><span class="sxs-lookup"><span data-stu-id="45e3b-630">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-631">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-631">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-632">구독 갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-632">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="45e3b-633">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-633">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-634">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-634">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-635">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-635">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-636">활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-636">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="45e3b-637"><strong>일회성 요금</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-637"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="45e3b-638">신규 항목</span><span class="sxs-lookup"><span data-stu-id="45e3b-638">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-639">새 구매가 생성 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-639">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-640">addQuantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-640">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-641">원래 구매 환불 및 증가 후 새로운 수량 모두에 사용 됨</span><span class="sxs-lookup"><span data-stu-id="45e3b-641">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-642">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="45e3b-642">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-643">원래 구매 환불 및 감소 후 새로운 수량 모두에 사용 됨</span><span class="sxs-lookup"><span data-stu-id="45e3b-643">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-644">취소</span><span class="sxs-lookup"><span data-stu-id="45e3b-644">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-645">구독이 취소 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-645">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-646">변환</span><span class="sxs-lookup"><span data-stu-id="45e3b-646">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-647">라이선스가 업그레이드 될 때 사용 되지만 사용자의 수는 변경 되지 않은 상태로 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45e3b-647">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="45e3b-648"><strong>사용 요금</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-648"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-649">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="45e3b-649">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-650">현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="45e3b-650">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="45e3b-651">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-651">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-652">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="45e3b-652">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-653">현재 청구 기간의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="45e3b-653">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="45e3b-654"><strong>크레딧</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-654"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-655">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="45e3b-655">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-656">세금을 포함하여 품목의 전액 또는 일부 금액 환불</span><span class="sxs-lookup"><span data-stu-id="45e3b-656">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-657">라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-657">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="45e3b-658">사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-658">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="45e3b-659"><strong>사용량 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-659"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-660">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-660">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-661">구독을 활성화할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-661">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="45e3b-662">사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-662">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-663">주기 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-663">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-664">정기 요금에 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-664">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-665">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-665">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-666">구독을 갱신할 때 적용되는 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-666">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-667">취소 할인</span><span class="sxs-lookup"><span data-stu-id="45e3b-667">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-668">할인이 취소될 때 적용되는 요금</span><span class="sxs-lookup"><span data-stu-id="45e3b-668">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="45e3b-669"><strong>라이선스 기반 할인</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-669"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-670"><em>여러 요금 유형에 적용 될 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="45e3b-670"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="45e3b-671">라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-671">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="45e3b-672"><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="45e3b-672"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-673"><em>여러 요금 유형에 적용 될 수 있습니다.</em></span><span class="sxs-lookup"><span data-stu-id="45e3b-673"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="45e3b-674"><em>예외: 줄 항목 &quot;에 세금이 이미 포함 되어 &quot;Offset. 위의 크레딧을 참조 하세요.</em></span><span class="sxs-lookup"><span data-stu-id="45e3b-674"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-675">세금 또는 VAT(부가가치세)</span><span class="sxs-lookup"><span data-stu-id="45e3b-675">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="45e3b-676">라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-676">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="45e3b-677">사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</span><span class="sxs-lookup"><span data-stu-id="45e3b-677">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
