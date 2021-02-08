---
title: Azure 플랜 청구 - 청구서 및 조정 파일
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure 요금제에 대한 청구와 관련된 청구서 및 조정 파일 구조에 액세스하고 이해하는 방법을 알아봅니다.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924995"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="e8cd8-103">CSP의 새로운 상거래 환경 - Azure 청구</span><span class="sxs-lookup"><span data-stu-id="e8cd8-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="e8cd8-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="e8cd8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e8cd8-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="e8cd8-105">Admin agent</span></span>
- <span data-ttu-id="e8cd8-106">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="e8cd8-106">Billing admin</span></span>
- <span data-ttu-id="e8cd8-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="e8cd8-107">Global admin</span></span>

<span data-ttu-id="e8cd8-108">이 문서에서는 Azure 플랜의 대금 청구와 관련된 청구서 및 조정 파일 구조에 액세스하고 이해하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="e8cd8-109">Azure 플랜에 따른 청구는 잘 조정된 단일 청구 날짜와 월별 청구 기간을 사용하는 간소화된 청구 환경입니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="e8cd8-110">청구 기본 정보 요약</span><span class="sxs-lookup"><span data-stu-id="e8cd8-110">Summary of billing essentials</span></span>

- <span data-ttu-id="e8cd8-111">**청구서 날짜**: 청구서 및 조정 파일은 8일(UTC 자정)에 파트너 센터 대시보드/API에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="e8cd8-112">**청구서 청구 기간**: 청구서 청구 기간은 달력의 월을 기준으로 조정됩니다(예: 10/1-10/31, 11/1-11/30).</span><span class="sxs-lookup"><span data-stu-id="e8cd8-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="e8cd8-113">**서비스 기간 요금 청구**: 요금은 달력의 월을 기준으로 조정됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="e8cd8-114">예를 들어 청구 파트너가 10/15에 Azure 플랜을 통해 Azure 서비스를 추가하고 고객이 10/15에 Azure 서비스 사용을 시작하는 경우 청구 파트너는 서비스 기간 10/15 - 10/31에 고객이 사용한 요금에 대한 청구서/조정 파일을 11/8에 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="e8cd8-115">12/8에 생성될 다음 달 청구서에는 서비스 기간 11/1 - 11/31의 모든 요금이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="e8cd8-116">**청구서 결제 기간**: 순 60일.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="e8cd8-117">**청구서 통화** : 2021년 1월 28일부터 EU/EFTA 및 영국 지역의 파트너 중에서 신규 고객 및 기존 CSP 고객이 2020년 5월 11일 전에 테넌트가 생성된 새 상거래 제품을 처음으로 구매한 파트너의 경우 해당 구매 대금은 파트너 위치 통화로 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="e8cd8-118">EU/EFTA 및 영국 외부 지역의 파트너는 파트너 위치 통화로 계속 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="e8cd8-119">**파트너 인센티브**: 청구 월이 끝나고 45일 후에 결제됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="e8cd8-120">청구서 및 조정 파일 액세스</span><span class="sxs-lookup"><span data-stu-id="e8cd8-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="e8cd8-121">청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="e8cd8-122">청구서 및 조정 파일에 액세스하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="e8cd8-123">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="e8cd8-124">파트너 센터 메뉴에서 **청구** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="e8cd8-125">**되풀이** 및 **일회성** 탭과 관심 있는 통화를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="청구":::

4. <span data-ttu-id="e8cd8-127">**청구서** 또는 **조정 파일** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="e8cd8-128">과거의 청구서 및 조정 파일을 보려면 아래쪽에서 청구 기록 행을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="e8cd8-129">사용량 데이터 이해</span><span class="sxs-lookup"><span data-stu-id="e8cd8-129">Understanding usage data</span></span> 

1. <span data-ttu-id="e8cd8-130">Azure 플랜은 사용량에 대한 루트 또는 최상위 컨테이너입니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="e8cd8-131">모든 사용량은 단일 Azure 플랜에 다시 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="e8cd8-132">플랜 내에는 하나 이상의 Azure 구독이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="e8cd8-133">이러한 구독은 리소스 관리 및 배포에 사용되는 컨테이너입니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="e8cd8-134">구독 내에서 리소스 그룹은 그룹 리소스에 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="e8cd8-135">모든 리소스는 하나의 리소스 그룹에 배포됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="e8cd8-136">리소스의 예로 가상 머신 및 스토리지 계정이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="e8cd8-137">리소스 내보내기 측정기: 측정기는 리소스의 사용량을 측정하며, 하나의 리소스에서 여러 측정기의 사용량을 내보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="e8cd8-138">측정기는 ProductId, SKUId 및 AvailabilityId로 식별됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="e8cd8-139">구독 리소스 그룹 및 계량의 계층 구조</span><span class="sxs-lookup"><span data-stu-id="e8cd8-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="e8cd8-140">**Azure 계정(테넌트)**</span><span class="sxs-lookup"><span data-stu-id="e8cd8-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="e8cd8-141">구독 A</span><span class="sxs-lookup"><span data-stu-id="e8cd8-141">Subscription A</span></span>
    - <span data-ttu-id="e8cd8-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="e8cd8-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="e8cd8-143">가상 머신(리소스)</span><span class="sxs-lookup"><span data-stu-id="e8cd8-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="e8cd8-144">컴퓨팅 측정기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-144">Compute meter</span></span>
        - <span data-ttu-id="e8cd8-145">가상 네트워크(리소스)</span><span class="sxs-lookup"><span data-stu-id="e8cd8-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="e8cd8-146">청구 측정기 없음</span><span class="sxs-lookup"><span data-stu-id="e8cd8-146">No billing meter</span></span>

    - <span data-ttu-id="e8cd8-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="e8cd8-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="e8cd8-148">가상 머신(리소스)</span><span class="sxs-lookup"><span data-stu-id="e8cd8-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="e8cd8-149">컴퓨터 측정기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-149">Computer meter</span></span>
        - <span data-ttu-id="e8cd8-150">프리미엄 SSD 관리 디스크(리소스)</span><span class="sxs-lookup"><span data-stu-id="e8cd8-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="e8cd8-151">스토리지 용량 측정기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-151">Storage capacity meter</span></span>
            - <span data-ttu-id="e8cd8-152">스토리지 작업 수 측정기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-152">Storage operations meter</span></span>

- <span data-ttu-id="e8cd8-153">구독 B   -ResourceGroup 1       - Azure SQL(리소스)           - DTU 측정기       - VPN Gateway(리소스)           - VPN Gateway 측정기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="e8cd8-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="e8cd8-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="e8cd8-155">Virtual Network 인터페이스(리소스)</span><span class="sxs-lookup"><span data-stu-id="e8cd8-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="e8cd8-156">청구 측정기 없음</span><span class="sxs-lookup"><span data-stu-id="e8cd8-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="e8cd8-157">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-157">Read the invoice</span></span>

1. <span data-ttu-id="e8cd8-158">청구서는 매월 8일 이후에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="e8cd8-159">파트너는 60일 내에 결제 금액을 송금해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="e8cd8-160">청구 기간에는 지정된 달력 월(예: 10/1-10/31)이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="e8cd8-161">요금은 순 조정액입니다(금액은 "관리형 서비스에 대해 파트너가 획득한 순 크레딧").</span><span class="sxs-lookup"><span data-stu-id="e8cd8-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="e8cd8-162">자세한 청구 정보는 청구서 조정 파일 및 일일 평가 사용량 파일을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="청구서":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="e8cd8-164">청구서 조정 파일 읽기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="e8cd8-165">각 Azure 플랜과 측정기의 조합은 조정 파일에 최대 두 개의 청구 줄을 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="e8cd8-166">측정기가 한 달 전체에 걸쳐 모든 유형의 할인 또는 크레딧(예: 계층화된 할인 또는 관리형 서비스에 대한 파트너 획득 크레딧)에 적합한 경우 조정 파일에는 하나의 청구 줄만 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="e8cd8-167">**PriceAdjusmentDescription** 열은 할인 또는 획득 크레딧을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="e8cd8-168">할인 또는 파트너 획득 크레딧에 적합한 특정 측정기에 대한 리소스가 없으면, 조정 파일에 하나의 청구 줄만 포함되며 유효 단가는 소매 가격(단가)이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="e8cd8-169">측정기 또는 해당 측정기를 내보내는 리소스가 월의 일부 동안 **관리형 서비스에 대한 파트너 획득 크레딧** 에 적합한 경우 조정 파일에는 두 줄의 청구가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="e8cd8-170">하나는 미터가 자격을 획득한 날을 표시하고 다른 하나는 미터가 자격을 획득하지 못한 날을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="e8cd8-171">일일 사용량 파일 읽기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-171">Read the daily usage file</span></span>

- <span data-ttu-id="e8cd8-172">Azure 플랜 하의 구독 미터는 날마다 평가하여 누적됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="e8cd8-173">**관리형 서비스에 대한 파트너 획득 크레딧** 은 매일 확인 및 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="e8cd8-174">모든 구독 미터에는 서비스가 사용된 월의 모든 날에 대한 행이 하나 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="e8cd8-175">아래 예제를 살펴보세요.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-175">In the example below:</span></span>

  - <span data-ttu-id="e8cd8-176">미터가 7/1 – 7/3에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).</span><span class="sxs-lookup"><span data-stu-id="e8cd8-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="e8cd8-177">미터가 7/4 – 7/7에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득하지 못했습니다(유효 단가는 소매 가격).</span><span class="sxs-lookup"><span data-stu-id="e8cd8-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="e8cd8-178">미터가 7/8 – 7/31에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).</span><span class="sxs-lookup"><span data-stu-id="e8cd8-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="e8cd8-180">고객 통화로 작성된 청구서</span><span class="sxs-lookup"><span data-stu-id="e8cd8-180">Invoice in customer currency</span></span>

<span data-ttu-id="e8cd8-181">Azure 플랜을 통한 Azure 서비스는 USD로 가격이 책정되며 고객의 국가에 할당된 통화 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="e8cd8-182">청구 통화가 USD가 아닌 경우 사용되는 환율은 청구서의 마지막 페이지에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="e8cd8-183">환율은 매월 결정되며 다음 청구서부터 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="e8cd8-184">국가 통화의 전체 목록은 [최신 상거래 제품 사용 가능 국가 및 고객 통화표](https://go.microsoft.com/fwlink/?linkid=2112354)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="e8cd8-185">Microsoft는 변환을 위해 런던 증권 거래소를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="e8cd8-186">런던 증권 거래소에서 매월 마지막 영업일의 마지막 초의 환율과 동일한 환율을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="e8cd8-187">환율은 적용되는 월의 첫 번째 날짜 이전에 새로 고쳐지고 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="e8cd8-188">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="e8cd8-188">Azure reservations</span></span>


<span data-ttu-id="e8cd8-189">Azure 플랜을 통해 [Azure 예약](azure-reservations.md)을 구매하는 경우 일회성 또는 월간 청구를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="e8cd8-190">Azure 지출</span><span class="sxs-lookup"><span data-stu-id="e8cd8-190">Azure spending</span></span>

<span data-ttu-id="e8cd8-191">기존의 Azure 지출 환경이 파트너 센터에서 새 Azure 플랜 청구서를 지원하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="e8cd8-192">이를 통해 파트너는 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-192">This enables partners to:</span></span>

- <span data-ttu-id="e8cd8-193">고객 수준에서 설정된 예산에 대한 경고 보기, 관리 및 받기</span><span class="sxs-lookup"><span data-stu-id="e8cd8-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="e8cd8-194">Azure 플랜에 대한 총 예상 지출 보기(리소스 및 측정기 수준별로 세분화됨)</span><span class="sxs-lookup"><span data-stu-id="e8cd8-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="e8cd8-195">Azure 플랜을 통한 Azure 서비스의 청구 모델은 후불 사용량 요금제이므로 청구 금액이 예상 금액을 초과하지 않도록 파트너는 월별 예산을 적용하고 사용률을 추적할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="e8cd8-196">예산을 한 고객에게 또는 동시에 여러 고객에게 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure 지출":::

## <a name="next-steps"></a><span data-ttu-id="e8cd8-198">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e8cd8-198">Next steps</span></span>

- <span data-ttu-id="e8cd8-199">PEC(파트너 획득 크레딧)를 계산하는 방법을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="e8cd8-200">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/)에 로그인하고 사용 가능한 가격표를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="e8cd8-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="e8cd8-201">[Azure 플랜 구매](purchase-azure-plan.md)에 대한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="e8cd8-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="e8cd8-202">[CSP의 새로운 상거래 환경에 대한 가격표](azure-plan-price-list.md) 참조</span><span class="sxs-lookup"><span data-stu-id="e8cd8-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
