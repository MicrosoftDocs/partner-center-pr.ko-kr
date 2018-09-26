---
title: Azure 예약에 대한 청구 | 파트너 센터
Description: Information about billing for Azure reservations.
author: v-petand
keywords: Azure RI, azure reserved instances, 예약, vm, 관리, 청구, 구입
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: 1f29c884d155a64ba4d592466a87682313ce9610
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877413"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a><span data-ttu-id="2f97c-103">Microsoft Azure Reserved VM Instances 청구</span><span class="sxs-lookup"><span data-stu-id="2f97c-103">Microsoft Azure Reserved VM Instances billing</span></span>

**<span data-ttu-id="2f97c-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="2f97c-104">Applies to</span></span>**

-  <span data-ttu-id="2f97c-105">파트너 대시보드</span><span class="sxs-lookup"><span data-stu-id="2f97c-105">Partner Dashboard</span></span>
-  <span data-ttu-id="2f97c-106">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2f97c-106">Microsoft Azure portal</span></span>
-  <span data-ttu-id="2f97c-107">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="2f97c-107">Partners in CSP</span></span>

<span data-ttu-id="2f97c-108">클라우드 솔루션 공급자(CSP) 프로그램의 파트너는 이제 Microsoft Azure 가상 컴퓨터에서 고객에게 예약한 인스턴스를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-108">Partners in the Cloud Solution Provider program (CSP) can offer their customers reserved instances on Microsoft Azure virtual machines.</span></span> <span data-ttu-id="2f97c-109">고객은 1년 또는 3년의 기간 동안 미리 가상 컴퓨터를 예약하여 Azure 사용량을 상당 부분 절약할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-109">Customers can reserve virtual machines in advance – for one-year or three-year terms – and experience significant savings on Azure usage.</span></span>   

<span data-ttu-id="2f97c-110">고객은 Azure Reserved VM Instances에 대한 비용을 미리 지불합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-110">Your customers pay in advance for Azure Reserved VM Instances.</span></span> <span data-ttu-id="2f97c-111">고객을 대신하여 Azure Reserved VM Instances를 구입하면 이러한 일회성 요금에 대한 송장 및 조정 파일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-111">When you buy Azure Reserved VM Instances on behalf of a customer, you’ll receive invoices and reconciliation files for these one-time charges.</span></span> 

>[!IMPORTANT]
><span data-ttu-id="2f97c-112">다른 통화를 사용하는 시장의 고객을 위해 Azure Reserved VM Instances를 구입한 경우에는 여러분의 위치가 아니라 고객의 시장을 기준으로 기본 청구 통화가 결정됩니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-112">If you purchase Azure Reserved VM Instances for a customer in a market with a currency different from yours, the default billing currency is based on the customer’s market, not your location.</span></span> <span data-ttu-id="2f97c-113">여러 시장의 고객을 확보하고 있는 경우에는 해당 통화로 고객에게 청구를 할 수 있도록 비용이 청구되는 각 통화에 대해 별도의 송장과 조정 파일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-113">If you have customers in multiple markets, you’ll receive separate invoices and reconciliation files for each currency customers need to be billed in, allowing you to invoice your customers in the appropriate currency.</span></span> 

<span data-ttu-id="2f97c-114">일회성 요금 송장 및 조정 파일에 액세스하려면 파트너 대시보드에서 **청구**를 선택한 다음 **일회성**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-114">To access one-time charge invoices and reconciliation files, select **Billing** from your Partner Dashboard and then select **One time**.</span></span> 

<span data-ttu-id="2f97c-115">클라우드 솔루션 공급자 프로그램의 청구에 대한 자세한 내용은 [청구의 기본 사항](billing-basics.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2f97c-115">For more general information about billing in the Cloud Solution Provider program, see [Billing basics](billing-basics.md).</span></span>

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a><span data-ttu-id="2f97c-116">Azure Reserved VM Instance 송장 파일 정의</span><span class="sxs-lookup"><span data-stu-id="2f97c-116">Azure Reserved VM Instance invoice file definitions</span></span>

**<span data-ttu-id="2f97c-117">일반 청구 정보</span><span class="sxs-lookup"><span data-stu-id="2f97c-117">General billing information</span></span>**

|**<span data-ttu-id="2f97c-118">필드</span><span class="sxs-lookup"><span data-stu-id="2f97c-118">Field</span></span>** |**<span data-ttu-id="2f97c-119">정의</span><span class="sxs-lookup"><span data-stu-id="2f97c-119">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="2f97c-120">US FEIN</span><span class="sxs-lookup"><span data-stu-id="2f97c-120">US FEIN</span></span> |<span data-ttu-id="2f97c-121">연방 세금 ID 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-121">Your Federal Tax ID Number.</span></span> |
|<span data-ttu-id="2f97c-122">청구지</span><span class="sxs-lookup"><span data-stu-id="2f97c-122">Bill to</span></span> |<span data-ttu-id="2f97c-123">세금 목적으로 사용되는 법적 비즈니스 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-123">The legal business address used for tax purposes.</span></span> <span data-ttu-id="2f97c-124">이 주소를 변경하려면 계정 설정 > 파트너 청구 프로필로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-124">To change this address, go to Account settings > Partner billing profile.</span></span> |
|<span data-ttu-id="2f97c-125">요금</span><span class="sxs-lookup"><span data-stu-id="2f97c-125">Charges</span></span> |<span data-ttu-id="2f97c-126">현재 총 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-126">All current charges.</span></span> |
|<span data-ttu-id="2f97c-127">크레딧</span><span class="sxs-lookup"><span data-stu-id="2f97c-127">Credits</span></span> |<span data-ttu-id="2f97c-128">초기 구매 이후 환불 활동에 대한 크레딧입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-128">Credits for refund activity since initial purchase.</span></span> |
|<span data-ttu-id="2f97c-129">할인:</span><span class="sxs-lookup"><span data-stu-id="2f97c-129">Discounts</span></span> |<span data-ttu-id="2f97c-130">Azure 예약이나 고객 주문서의 기타 항목에 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-130">Discounts that may apply to Azure reservations or other items in the customer’s order.</span></span> |
|<span data-ttu-id="2f97c-131">세금</span><span class="sxs-lookup"><span data-stu-id="2f97c-131">Taxes</span></span> |<span data-ttu-id="2f97c-132">송장 2페이지의 시작 부분에 있는 세부 정보 섹션에 합산되어 있는 현재 요금의 총 세금입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-132">The total tax for the current charges as totaled in the details section beginning on page 2 of the invoice.</span></span> |
|<span data-ttu-id="2f97c-133">현재 총 요금</span><span class="sxs-lookup"><span data-stu-id="2f97c-133">Total current charges</span></span> |<span data-ttu-id="2f97c-134">기한이 결제 기한까지인 청구 기간의 결제액(청구 통화로 된 금액)입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-134">The amount due in your billing currency for the billing period, due by the payment due date.</span></span> |
|<span data-ttu-id="2f97c-135">결제 관련 지침</span><span class="sxs-lookup"><span data-stu-id="2f97c-135">Payment instructions</span></span> |<span data-ttu-id="2f97c-136">지역을 기준으로 송장 요금을 지불하는 시기와 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-136">Describes when and how to pay your invoice, based on your region.</span></span> <span data-ttu-id="2f97c-137">결제 시 항상 송장 번호를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-137">Always include your invoice number when making a payment.</span></span> |
|<span data-ttu-id="2f97c-138">송장 번호</span><span class="sxs-lookup"><span data-stu-id="2f97c-138">Invoice #</span></span> |<span data-ttu-id="2f97c-139">송장의 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-139">The number of your invoice.</span></span> |
|<span data-ttu-id="2f97c-140">송장 날짜</span><span class="sxs-lookup"><span data-stu-id="2f97c-140">Invoice date</span></span> |<span data-ttu-id="2f97c-141">송장이 생성된 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-141">The date your invoice was generated.</span></span> |
|<span data-ttu-id="2f97c-142">지급 조건</span><span class="sxs-lookup"><span data-stu-id="2f97c-142">Payment terms</span></span> |<span data-ttu-id="2f97c-143">일회성 구매에 대해서는 항상 60일 이내입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-143">For one-time purchases this will always be 60 days.</span></span> |
|<span data-ttu-id="2f97c-144">결제 기한</span><span class="sxs-lookup"><span data-stu-id="2f97c-144">Payment due date</span></span> |<span data-ttu-id="2f97c-145">이 날짜에 결제 금액이 들어와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-145">Your payment must be received by this date.</span></span> |


**<span data-ttu-id="2f97c-146">일회성 요금의 항목별 목록</span><span class="sxs-lookup"><span data-stu-id="2f97c-146">Itemized list of one-time charges</span></span>**

|**<span data-ttu-id="2f97c-147">필드</span><span class="sxs-lookup"><span data-stu-id="2f97c-147">Field</span></span>** |**<span data-ttu-id="2f97c-148">정의</span><span class="sxs-lookup"><span data-stu-id="2f97c-148">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="2f97c-149">날짜</span><span class="sxs-lookup"><span data-stu-id="2f97c-149">Date</span></span> |<span data-ttu-id="2f97c-150">구매 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-150">Date of purchase.</span></span> |
|<span data-ttu-id="2f97c-151">설명</span><span class="sxs-lookup"><span data-stu-id="2f97c-151">Description</span></span> |<span data-ttu-id="2f97c-152">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-152">Product name.</span></span> |
|<span data-ttu-id="2f97c-153">수량</span><span class="sxs-lookup"><span data-stu-id="2f97c-153">Quantity</span></span> |<span data-ttu-id="2f97c-154">구입한 제품(예: 예약)의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-154">The number of products (reservations, e.g.) purchased.</span></span> |
|<span data-ttu-id="2f97c-155">단가</span><span class="sxs-lookup"><span data-stu-id="2f97c-155">Unit price</span></span> |<span data-ttu-id="2f97c-156">각 제품(예: 예약)의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-156">Price per product (reservation, e.g.).</span></span> |
|<span data-ttu-id="2f97c-157">할인</span><span class="sxs-lookup"><span data-stu-id="2f97c-157">Discounts</span></span> |<span data-ttu-id="2f97c-158">적용 가능한 모든 할인 혜택입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-158">Any applicable discounts.</span></span> |
|<span data-ttu-id="2f97c-159">세전 금액</span><span class="sxs-lookup"><span data-stu-id="2f97c-159">Pre-tax amount</span></span> |<span data-ttu-id="2f97c-160">세금 부과 전 구입액의 소계입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-160">Sub-total of the purchases before taxes.</span></span> |
|<span data-ttu-id="2f97c-161">판매세</span><span class="sxs-lookup"><span data-stu-id="2f97c-161">Sales tax</span></span> |<span data-ttu-id="2f97c-162">세금 액수입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-162">Tax amount.</span></span> |
|<span data-ttu-id="2f97c-163">총액</span><span class="sxs-lookup"><span data-stu-id="2f97c-163">Total</span></span> |<span data-ttu-id="2f97c-164">지불해야 할 총액입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-164">Total to be paid.</span></span> |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a><span data-ttu-id="2f97c-165">Azure Reserved VM Instance 조정 파일 설명</span><span class="sxs-lookup"><span data-stu-id="2f97c-165">Azure Reserved VM Instance reconciliation file descriptions</span></span>

|**<span data-ttu-id="2f97c-166">필드</span><span class="sxs-lookup"><span data-stu-id="2f97c-166">Field</span></span>** |**<span data-ttu-id="2f97c-167">정의</span><span class="sxs-lookup"><span data-stu-id="2f97c-167">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="2f97c-168">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2f97c-168">PartnerId</span></span> |<span data-ttu-id="2f97c-169">GUID 형식의 파트너 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-169">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="2f97c-170">CustomerId</span><span class="sxs-lookup"><span data-stu-id="2f97c-170">CustomerId</span></span> |<span data-ttu-id="2f97c-171">고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-171">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="2f97c-172">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2f97c-172">CustomerName</span></span> |<span data-ttu-id="2f97c-173">파트너 센터에 보고된 고객의 조직 이름.</span><span class="sxs-lookup"><span data-stu-id="2f97c-173">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="2f97c-174">시스템 정보로 송장을 조정할 때 매우 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-174">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="2f97c-175">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="2f97c-175">CustomerDomainName</span></span> |<span data-ttu-id="2f97c-176">고객의 도메인 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-176">The customer’s domain name.</span></span> |
|<span data-ttu-id="2f97c-177">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="2f97c-177">CustomerCountry</span></span> |<span data-ttu-id="2f97c-178">고객이 위치한 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-178">The country in which the customer is located.</span></span> |
|<span data-ttu-id="2f97c-179">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="2f97c-179">InvoiceNumber</span></span> |<span data-ttu-id="2f97c-180">지정한 트랜잭션이 표시되는 송장 번호입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-180">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="2f97c-181">MpnId</span><span class="sxs-lookup"><span data-stu-id="2f97c-181">MpnId</span></span> |<span data-ttu-id="2f97c-182">CSP 파트너(직접 또는 간접)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-182">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="2f97c-183">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="2f97c-183">Reseller MPN ID</span></span> |<span data-ttu-id="2f97c-184">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-184">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="2f97c-185">예약에 대한 ROR(Reseller of Record)의 MPN ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-185">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="2f97c-186">파트너 센터에서 특정 예약에 대해 나열된 재판매인 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-186">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="2f97c-187">CSP 파트너가 고객에게 직접 예약을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</span><span class="sxs-lookup"><span data-stu-id="2f97c-187">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="2f97c-188">CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-188">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="2f97c-189">CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-189">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="2f97c-190">OrderId</span><span class="sxs-lookup"><span data-stu-id="2f97c-190">OrderId</span></span> |<span data-ttu-id="2f97c-191">Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-191">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2f97c-192">지원 팀에 문의할 때는 Azure 예약을 식별하는 것이 유용할 수 있지만, 조정에서는 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-192">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="2f97c-193">OrderDate</span><span class="sxs-lookup"><span data-stu-id="2f97c-193">OrderDate</span></span> |<span data-ttu-id="2f97c-194">주문이 이루어진 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-194">The date the order was placed.</span></span> |
|<span data-ttu-id="2f97c-195">ProductId</span><span class="sxs-lookup"><span data-stu-id="2f97c-195">ProductId</span></span> |<span data-ttu-id="2f97c-196">제품의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-196">The ID for the product.</span></span> |
|<span data-ttu-id="2f97c-197">SkuId</span><span class="sxs-lookup"><span data-stu-id="2f97c-197">SkuId</span></span>  |<span data-ttu-id="2f97c-198">특정 SKU의 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-198">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="2f97c-199">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="2f97c-199">AvailabilityId</span></span> |<span data-ttu-id="2f97c-200">특정 가용성에 대한 ID입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-200">The ID for a particular Availability.</span></span> <span data-ttu-id="2f97c-201">"가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-201">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="2f97c-202">SkuName</span><span class="sxs-lookup"><span data-stu-id="2f97c-202">SkuName</span></span>  |<span data-ttu-id="2f97c-203">특정 SKU의 제목입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-203">The title for a particular SKU.</span></span> |
|<span data-ttu-id="2f97c-204">ProductName</span><span class="sxs-lookup"><span data-stu-id="2f97c-204">ProductName</span></span> |<span data-ttu-id="2f97c-205">제품 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-205">The name of the product.</span></span> |
|<span data-ttu-id="2f97c-206">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2f97c-206">ChargeType</span></span> |<span data-ttu-id="2f97c-207">요금 또는 조정 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-207">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="2f97c-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="2f97c-208">UnitPrice</span></span> |<span data-ttu-id="2f97c-209">주문한 각 제품의 가격입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-209">Price per product ordered.</span></span> |
|<span data-ttu-id="2f97c-210">수량</span><span class="sxs-lookup"><span data-stu-id="2f97c-210">Quantity</span></span> |<span data-ttu-id="2f97c-211">주문한 제품의 수입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-211">Number of products ordered.</span></span> |
|<span data-ttu-id="2f97c-212">소계</span><span class="sxs-lookup"><span data-stu-id="2f97c-212">Subtotal</span></span> |<span data-ttu-id="2f97c-213">세금을 적용하기 전의 총액.</span><span class="sxs-lookup"><span data-stu-id="2f97c-213">Total before tax.</span></span> <span data-ttu-id="2f97c-214">할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-214">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="2f97c-215">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="2f97c-215">TaxTotal</span></span> |<span data-ttu-id="2f97c-216">적용 가능한 모든 세금의 총액입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-216">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="2f97c-217">총액</span><span class="sxs-lookup"><span data-stu-id="2f97c-217">Total</span></span> |<span data-ttu-id="2f97c-218">총 구입 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-218">The total amount of this purchase.</span></span> |
|<span data-ttu-id="2f97c-219">통화</span><span class="sxs-lookup"><span data-stu-id="2f97c-219">Currency</span></span> |<span data-ttu-id="2f97c-220">통화 형식.</span><span class="sxs-lookup"><span data-stu-id="2f97c-220">Currency type.</span></span> <span data-ttu-id="2f97c-221">각 청구 엔터티의 통화는 한 가지만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="2f97c-222">통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-222">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="2f97c-223">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="2f97c-223">DiscountDetails</span></span> |<span data-ttu-id="2f97c-224">모든 관련 할인에 대한 상세 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-224">Detailed listing of any relevant discounts.</span></span> |


## <a name="manage-your-billing"></a><span data-ttu-id="2f97c-225">청구 관리</span><span class="sxs-lookup"><span data-stu-id="2f97c-225">Manage your billing</span></span>

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a><span data-ttu-id="2f97c-226">현재 청구 상태, 송장 및 조정 파일 보기</span><span class="sxs-lookup"><span data-stu-id="2f97c-226">View your current billing status, invoices, and recon files</span></span>

1.  <span data-ttu-id="2f97c-227">파트너 대시보드에서 **청구**와 **일회성**을 차례로 선택하여 청구 상태를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-227">In your Partner Dashboard, select **Billing** and then **One time** to view your billing status.</span></span> 
2.  <span data-ttu-id="2f97c-228">자세한 정보를 보려면 송장 또는 조정 파일을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-228">Select an invoice or recon file to view more detailed information.</span></span> 

### <a name="view-a-customers-order-history"></a><span data-ttu-id="2f97c-229">고객의 주문 내역 보기</span><span class="sxs-lookup"><span data-stu-id="2f97c-229">View a customer’s order history</span></span>

1.  <span data-ttu-id="2f97c-230">대시보드 메뉴에서 **고객**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-230">Select **Customers** from your dashboard menu.</span></span>
2.  <span data-ttu-id="2f97c-231">**고객** 페이지에서 주문 내역을 확인하려는 고객을 찾고 아래쪽 화살표를 선택하여 고객의 기록을 펼쳐봅니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-231">On your **Customers** page, find the customer whose order history you want to view and then select the down arrow to expand the customer’s record.</span></span> 
3.  <span data-ttu-id="2f97c-232">**주문 보기**를 선택하여 주문 내역을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-232">Select **View orders** to display the order history.</span></span>

### <a name="create-a-credit-or-void-note"></a><span data-ttu-id="2f97c-233">크레딧 또는 빈 어음 만들기</span><span class="sxs-lookup"><span data-stu-id="2f97c-233">Create a credit or void note</span></span>

<span data-ttu-id="2f97c-234">송장을 취소한 다음 새 송장을 발행해야 하는 상황이 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-234">At some point you might need to void an invoice and then issue a new one.</span></span> <span data-ttu-id="2f97c-235">예를 들어, 고객이 기업 이름을 변경했는데 기존 이름으로 송장을 수신하는 경우입니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-235">For example, a customer may change the name of its business, and then receive an invoice with the old name.</span></span> 

<span data-ttu-id="2f97c-236">송장을 취소하고 새 송장을 발급 받으려면 조정 아래 청구 페이지에서 양식을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="2f97c-236">To void an invoice and have a new one issued, download the form from the billing page under adjustments.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="2f97c-237">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="2f97c-237">Azure reservations resources</span></span>
|**<span data-ttu-id="2f97c-238">자세한 내용</span><span class="sxs-lookup"><span data-stu-id="2f97c-238">For information about</span></span>**   |**<span data-ttu-id="2f97c-239">이 글 읽기</span><span class="sxs-lookup"><span data-stu-id="2f97c-239">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="2f97c-240">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="2f97c-240">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="2f97c-241">Microsoft Azure Reserved VM Instances 판매</span><span class="sxs-lookup"><span data-stu-id="2f97c-241">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="2f97c-242">파트너 대시보드에서 고객을 위한 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="2f97c-242">Purchasing Azure reservations for your customers in your Partner Dashboard</span></span>   |[<span data-ttu-id="2f97c-243">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="2f97c-243">Buy Azure reservations</span></span>](azure-reservations-buying.md)
| <span data-ttu-id="2f97c-244">파트너 대시보드에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="2f97c-244">Managing Azure reservations in your Partner Dashboard</span></span> | [<span data-ttu-id="2f97c-245">파트너 대시보드에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="2f97c-245">Managing Azure reservations in your Partner Dashboard</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="2f97c-246">Azure Portal에서 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="2f97c-246">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="2f97c-247">Azure 도움말의 [Azure Reserved VM Instances에서 가상 컴퓨터에 대한 사전 지불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2f97c-247">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="2f97c-248">Azure Portal에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="2f97c-248">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="2f97c-249">Azure 도움말의 [예약된 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2f97c-249">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="2f97c-250">파트너 센터 API를 사용하여 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="2f97c-250">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="2f97c-251">파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2f97c-251">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>

 