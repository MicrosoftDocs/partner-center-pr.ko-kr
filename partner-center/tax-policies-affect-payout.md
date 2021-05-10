---
title: 세금 정책이 Azure Marketplace 지급에 미치는 영향
description: 세금 정책이 Azure Marketplace 지급에 미치는 영향을 알아봅니다.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686316"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="9746f-103">세금 정책이 Azure Marketplace 지급에 미치는 영향</span><span class="sxs-lookup"><span data-stu-id="9746f-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="9746f-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="9746f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9746f-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="9746f-105">Global admin</span></span>
- <span data-ttu-id="9746f-106">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="9746f-106">User management admin</span></span>
- <span data-ttu-id="9746f-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="9746f-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="9746f-108">소개</span><span class="sxs-lookup"><span data-stu-id="9746f-108">Introduction</span></span>

<span data-ttu-id="9746f-109">Microsoft 상업용 Marketplace는 전 세계에 도달합니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="9746f-110">트랜잭션은 경계를 넘어 ISV와 고객의 위치에 따라 세금에 미치는 영향이 달라질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="9746f-111">Microsoft AppSource 및 Azure Marketplace 파트너 센터 세금 프로필 정보를 사용하여 ISV의 국가를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="9746f-112">고객의 국가를 확인하려면 고객의 청구 정보를 사용하거나 고객이 EU에 있는 경우 두 가지 정보를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="9746f-113">다음 시나리오를 더 잘 이해하려면 Microsoft가 게시자를 대신하여 세금을 징수하고 지불하는지 또는 해당 책임이 게시자에 속하는지 여부를 보여 주는 [세금 세부 정보](tax-details-marketplace.md) 표를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9746f-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="9746f-114">이 항목의 모든 예제 판매 값 및 세금 비율은 정확한 수치가 아니라 설명 목적으로만 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="9746f-115">Microsoft 관리 세금 국가의 게시자 거래</span><span class="sxs-lookup"><span data-stu-id="9746f-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="9746f-116">**시나리오 A** – [Microsoft 관리 세금 국가에서](tax-details-marketplace.md#microsoft-managed-countries)게시자와 고객 간에 이루어지는 트랜잭션입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="9746f-117">이러한 트랜잭션은 판매 시 해당 세금이 추가되며 Microsoft는 해당 국가에 해당 세금을 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="9746f-118">지급에서 세금이 징수되지 않으며 지급 계산은 세금 배타적입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="9746f-119">미국 이외의 게시자와 미국 고객 간의 트랜잭션에 대한 [시나리오 D를](#foreign-publisher-transacts-with-us-customer) 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9746f-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="지급 프로세스 시나리오 A에 대한 워크플로를 표시합니다.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="9746f-121">Marketplace 요금이 세금이 부과되는 Microsoft 관리 세금 국가의 게시자 거래</span><span class="sxs-lookup"><span data-stu-id="9746f-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="9746f-122">**시나리오 B** – 미국 기반 게시자(파트너 센터 세금 프로필 정보로 정의됨)에서 해당 국가에서 Marketplace 요금(세금 서비스)에 대해 세금을 부과한 Microsoft 관리형 세금 국가의 고객 간에 이루어지는 트랜잭션입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="9746f-123">이 시나리오에서는 상점 서비스 요금에 대한 세금이 게시자의 지급액에서 차감됩니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="지급 프로세스 시나리오 B에 대한 워크플로를 표시합니다.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="9746f-125">게시자 엔터티입니다의 게시자 관리 세금 국가</span><span class="sxs-lookup"><span data-stu-id="9746f-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="9746f-126">**시나리오 C** – 고객에 게 원천 세금을 적용 하지 않는 게시자 관리 세금 국가의 게시자와 고객 간에 발생 하는 트랜잭션입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="9746f-127">고객은 판매 시점에서 세금을 지불 하지 않으며 해당 세금을 지불 하기 위한 게시자의 의무입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="9746f-128">국가별 가격 책정 (예: 예정 된 세금 오프셋)에 대 한 자세한 내용은 [상용 marketplace 제품에 대 한 계획 및 가격 책정](/azure/marketplace/plans-pricing#custom-prices)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="9746f-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="지급 process 시나리오 C에 대 한 워크플로를 표시 합니다.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="9746f-130">미국 고객과의 외부 게시자 엔터티입니다</span><span class="sxs-lookup"><span data-stu-id="9746f-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="9746f-131">**시나리오 D** – 미국 조약이 없는 국가에서 모든 외부 게시자 (파트너 센터 세금 프로필 정보로 정의 [됨)는](#foreign-publisher-with-a-treaty-transacts-with-us-customer)미국 조약 (고객 계정 주소로 정의 됨)에 따라 미국 기반 고객에 대 한 판매를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="9746f-132">미국 정부에서는 게시자를 대신 하 여 Microsoft 보유 세금을 요구 합니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="9746f-133">지급에서 publisher로 세금 보안상 이유로은 제공 가격을 기준으로 계산 됩니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="지급 process 시나리오 D에 대 한 워크플로를 표시 합니다.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="9746f-135">미국 고객과 협약 엔터티입니다 있는 외부 게시자</span><span class="sxs-lookup"><span data-stu-id="9746f-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="9746f-136">**시나리오 E** – 미국 협약에 의해 정의 된 모든 외부 게시자 (고객 계정 주소에 정의 된 대로 미국 협약 프로필 정보로 정의 됨)</span><span class="sxs-lookup"><span data-stu-id="9746f-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="9746f-137">미국 정부에서는 게시자를 대신 하 여 Microsoft에서 세금을 보유 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="지급 process 시나리오 E에 대 한 워크플로를 표시 합니다.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="9746f-139">외부 게시자는 Microsoft에서 관리 하는 국가 (아일랜드 외부)에서 EU VAT로 등록 된 고객에 게 판매 됩니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="9746f-140">**시나리오 F** -Microsoft-Managed 국가에서 외부 게시자와 EU (아일랜드 외부)에 등록 된 고객 간의 모든 트랜잭션입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="9746f-141">고객은 판매에 대 한 세금을 지불 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="지급 process 시나리오 F에 대 한 워크플로를 보여 줍니다.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="9746f-143">외부 게시자는 Microsoft에서 관리 하는 국가 (아일랜드)에서 EU VAT로 등록 된 고객에 게 판매 됩니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="9746f-144">**시나리오 G** – Microsoft-Managed 국가에서 외신 게시자와 EU VAT 등록 고객(아일랜드 내) 간의 모든 거래입니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="9746f-145">고객은 Vat VAT를 지급하고 Microsoft는 이 세금을 지방 정부에게 지급합니다.</span><span class="sxs-lookup"><span data-stu-id="9746f-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="지급 프로세스 시나리오 G에 대한 워크플로를 표시합니다.":::

## <a name="next-steps"></a><span data-ttu-id="9746f-147">다음 단계</span><span class="sxs-lookup"><span data-stu-id="9746f-147">Next steps</span></span>

- [<span data-ttu-id="9746f-148">게시자 FAQ</span><span class="sxs-lookup"><span data-stu-id="9746f-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="9746f-149">지불 및 세금 프로필을 만드는 지침</span><span class="sxs-lookup"><span data-stu-id="9746f-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)