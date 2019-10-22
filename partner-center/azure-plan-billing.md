---
title: Azure 플랜 - 청구 | 파트너 센터
ms.topic: article
ms.date: 10/04/2019
description: 청구서 및 조정 파일 구조에 대해 설명
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171296"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="dfdf8-103">CSP의 새로운 상거래 환경 - Azure 청구</span><span class="sxs-lookup"><span data-stu-id="dfdf8-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="dfdf8-104">Azure 플랜 하에서는 잘 조정된 단일 청구 날짜와 월 기반 청구 기간을 사용하여 간편하게 청구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="dfdf8-105">청구 플랫폼에 대한 자세한 내용은 [파트너 센터 최신 상거래 운영 가이드](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="dfdf8-106">청구 기본 정보 요약</span><span class="sxs-lookup"><span data-stu-id="dfdf8-106">Summary of billing essentials</span></span>

- <span data-ttu-id="dfdf8-107">**청구서 날짜**: 청구서 및 조정 파일은 8일(UTC 자정)에 파트너 센터 대시보드/API에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="dfdf8-108">**청구서 청구 기간**: 청구서 청구 기간은 달력의 월을 기준으로 조정됩니다(예: 10/1-10/31, 11/1-11/30).</span><span class="sxs-lookup"><span data-stu-id="dfdf8-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="dfdf8-109">**서비스 기간 요금 청구**: 요금은 달력의 월을 기준으로 조정됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="dfdf8-110">예를 들어 청구 파트너가 10/15에 Azure 플랜을 통해 Azure 서비스를 추가하고 고객이 10/15에 Azure 서비스 사용을 시작하는 경우 청구 파트너는 서비스 기간 10/15 - 10/31에 고객이 사용한 요금에 대한 청구서/조정 파일을 11/8에 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="dfdf8-111">12/8에 생성될 다음 달 청구서에는 서비스 기간 11/1 - 11/31의 모든 요금이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="dfdf8-112">**청구서 결제 기간**: 순 60일.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="dfdf8-113">**청구서 통화** : 파트너는 고객의 국가에 할당된 통화로 계속 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="dfdf8-114">예를 들어 청구 파트너가 아일랜드에 있고 고객은 영국, 노르웨이 및 독일에 있는 경우 청구 파트너는 GBP, NOK 및 EUR 청구서/조정 파일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="dfdf8-115">**파트너 인센티브**: 청구 월이 끝나고 45일 후에 결제됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="dfdf8-116">청구서 및 조정 파일 액세스</span><span class="sxs-lookup"><span data-stu-id="dfdf8-116">Access your invoices and recon files</span></span>

<span data-ttu-id="dfdf8-117">청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="dfdf8-118">**청구서 및 조정 파일에 액세스하려면**</span><span class="sxs-lookup"><span data-stu-id="dfdf8-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="dfdf8-119">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dfdf8-120">파트너 센터 메뉴에서 **청구**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="dfdf8-121">원하는 **달력 기반**  및 통화에 대한 탭을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![청구](images/azure/billing1.png)

4. <span data-ttu-id="dfdf8-123">**청구서 및 조정 파일**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="dfdf8-124">과거의 청구서 및 조정 파일을 보려면 아래쪽에서 청구 기록 행을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="dfdf8-125">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="dfdf8-125">Read the invoice</span></span>

1. <span data-ttu-id="dfdf8-126">청구서는 매월 8일 이후에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="dfdf8-127">파트너는 60일 내에 결제 금액을 송금해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="dfdf8-128">청구 기간에는 지정된 달력 월(예: 10/1-10/31)이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="dfdf8-129">요금은 순 조정액입니다(금액은 "관리형 서비스에 대해 파트너가 획득한 순 크레딧").</span><span class="sxs-lookup"><span data-stu-id="dfdf8-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="dfdf8-130">자세한 청구 정보는 청구서 조정 파일 및 일일 평가 사용량 파일을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![청구서](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="dfdf8-132">조정 파일 읽기</span><span class="sxs-lookup"><span data-stu-id="dfdf8-132">Read the recon file</span></span>

1. <span data-ttu-id="dfdf8-133">각 Azure 구독 미터의 조정 파일에 최대 2개의 청구 항목이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="dfdf8-134">미터가 월 전체에 걸쳐 할인 또는 크레딧 자격을 획득한 경우(예: 계층 1 할인 또는 관리형 서비스에 대한 파트너 획득 크레딧) 조정 파일에는 청구 항목이 하나만 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="dfdf8-135">**PriceAdjusmentDescription** 열은 할인 또는 획득한 크레딧을 참조합니다. 유효 단가는 소매 가격에서 파트너가 획득한 크레딧 또는 기타 할인을 뺀 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="dfdf8-136">미터가 월 전체에 걸쳐 관리형 서비스에 대한 파트너 획득 크레딧 자격을 얻지 못하면 조정 파일에는 청구 항목이 하나만 포함되고 유효 단가는 소매 가격(단가)이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="dfdf8-137">미터가 월의 일부 기간에 대해 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득한 경우에는 조정 파일에 두 개의 청구 항목이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="dfdf8-138">하나는 미터가 자격을 획득한 날을 표시하고 다른 하나는 미터가 자격을 획득하지 못한 날을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="dfdf8-139">일일 사용량 파일 읽기</span><span class="sxs-lookup"><span data-stu-id="dfdf8-139">Read the daily usage file</span></span>

- <span data-ttu-id="dfdf8-140">Azure 플랜 하의 구독 미터는 날마다 평가하여 누적됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="dfdf8-141">**관리형 서비스에 대한 파트너 획득 크레딧**은 매일 확인 및 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="dfdf8-142">모든 구독 미터에는 서비스가 사용된 월의 모든 날에 대한 행이 하나 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="dfdf8-143">아래 예제를 살펴보세요.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-143">In the example below:</span></span>

  - <span data-ttu-id="dfdf8-144">미터가 7/1 – 7/3에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).</span><span class="sxs-lookup"><span data-stu-id="dfdf8-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="dfdf8-145">미터가 7/4 – 7/7에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득하지 못했습니다(유효 단가는 소매 가격).</span><span class="sxs-lookup"><span data-stu-id="dfdf8-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="dfdf8-146">미터가 7/8 – 7/31에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).</span><span class="sxs-lookup"><span data-stu-id="dfdf8-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="dfdf8-148">고객 통화로 작성된 청구서</span><span class="sxs-lookup"><span data-stu-id="dfdf8-148">Invoice in customer currency</span></span> 

<span data-ttu-id="dfdf8-149">Azure 플랜을 통한 Azure 서비스는 USD로 가격이 책정되며 고객의 국가에 할당된 통화 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="dfdf8-150">청구 통화가 USD가 아니면 사용되는 환율이 청구서의 마지막 페이지에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="dfdf8-151">환율은 매월 결정되며 다음 청구서부터 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="dfdf8-152">국가 통화의 전체 목록은 [최신 상거래 제품 사용 가능 국가 및 고객 통화표](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="dfdf8-153">Microsoft는 [톰슨 로이터](https://developers.thomsonreuters.com/content/wm-company)의 환율을 사용하여 청구서 통화 전환에 사용할 가격 책정 통화를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="dfdf8-154">환율은 매월 1일의 전날에 갱신되어 1일부터 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="dfdf8-155">**예**:  서비스 기간 8월 1일 – 8월 31일의 사용 요금은 8월 1일에 게시된 환율로 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="dfdf8-156">이 요금은 9월 청구서에 표시되며, 청구서의 마지막 페이지에 환율이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="dfdf8-157">파트너 테넌트 사용자는 청구 통화에 관계없이 모든 고객과 모든 주문에 대한 역할 관련 정보를 계속 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="dfdf8-158">또한 사용자는 모든 청구서를 모든 통화로 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="dfdf8-159">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="dfdf8-159">Azure reservations</span></span> 

<span data-ttu-id="dfdf8-160">Azure 플랜을 통해 [Azure 예약](https://docs.microsoft.com/partner-center/azure-reservations)을 구매하는 경우 파트너 센터에서 일회성 청구를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="dfdf8-161">월별 청구는 Azure Portal에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="dfdf8-162">파트너 센터에서도 향후 월별 청구를 제공할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="dfdf8-163">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="dfdf8-163">Azure cost management</span></span> 

<span data-ttu-id="dfdf8-164">조직에서는 Azure Cost Management 도구를 사용하여 Microsoft Azure의 비용을 시각화하고 관리하고 최적화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="dfdf8-165">이 기능은 Azure Portal에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="dfdf8-166">파트너는 다음과 같은 기능을 제공하는 상시 사용 가능하고 대기 시간이 짧은 솔루션을 사용할 수 있게 될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="dfdf8-167">풍부한 분석 및 예산 경고</span><span class="sxs-lookup"><span data-stu-id="dfdf8-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="dfdf8-168">API 및 Power BI 커넥터</span><span class="sxs-lookup"><span data-stu-id="dfdf8-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="dfdf8-169">다중 고객 보기</span><span class="sxs-lookup"><span data-stu-id="dfdf8-169">Multi-customer view</span></span> 
- <span data-ttu-id="dfdf8-170">무료로 Azure 비용 관리</span><span class="sxs-lookup"><span data-stu-id="dfdf8-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="dfdf8-171">역할/사용자 확장</span><span class="sxs-lookup"><span data-stu-id="dfdf8-171">Expansion of roles/users</span></span> 

<span data-ttu-id="dfdf8-172">이 기능에 대한 자세한 내용은 2019년 2월부터 기업 계약에 사용할 수 있게 된 [Azure Cost Management](https://azure.microsoft.com/services/cost-management)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="dfdf8-173">이 도구는 CSP에서 새 Azure 상거래 환경의 일부로 구매한 Azure 서비스에만 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="dfdf8-174">Azure 지출</span><span class="sxs-lookup"><span data-stu-id="dfdf8-174">Azure spending</span></span> 

<span data-ttu-id="dfdf8-175">조만간 CSP의 새로운 상거래 환경을 위한 파트너 센터에서 Azure 지출 도구를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="dfdf8-176">이 기능이 적용되면 파트너는 다음 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="dfdf8-177">고객의 총 예산</span><span class="sxs-lookup"><span data-stu-id="dfdf8-177">Total budget on a customer</span></span> 
- <span data-ttu-id="dfdf8-178">기존 Azure 플랜의 총 예상 지출</span><span class="sxs-lookup"><span data-stu-id="dfdf8-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="dfdf8-179">각 청구 기간의 고객 사용 백분율</span><span class="sxs-lookup"><span data-stu-id="dfdf8-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="dfdf8-180">Azure 플랜을 통한 Azure 서비스의 청구 모델은 종량제이므로, 청구 금액이 예상을 초과하지 않도록 파트너는 월별 예산을 적용하고 사용량 비율을 추적할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="dfdf8-181">예산을 한 고객에게 또는 동시에 여러 고객에게 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure 지출](images/azure/azurespend.png)

<span data-ttu-id="dfdf8-183">**자세한 내용**</span><span class="sxs-lookup"><span data-stu-id="dfdf8-183">**For more information**</span></span>

-  <span data-ttu-id="dfdf8-184">PEC(파트너 획득 크레딧) 계산 방식은 파트너 센터 대시보드를 통해 사용할 수 있는 가격표에서 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfdf8-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="dfdf8-185">Azure 플랜 구매</span><span class="sxs-lookup"><span data-stu-id="dfdf8-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="dfdf8-186">CSP의 새로운 상거래 환경에 대한 가격표</span><span class="sxs-lookup"><span data-stu-id="dfdf8-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
