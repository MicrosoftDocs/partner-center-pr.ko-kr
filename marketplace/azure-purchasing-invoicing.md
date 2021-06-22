---
title: Azure Marketplace 소프트웨어 및 솔루션 구매
description: Azure Marketplace 소프트웨어 구매 및 관리를 간소화하고 간소화하는 도구에 대해 알아봅니다.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431555"
---
# <a name="azure-marketplace-purchasing"></a><span data-ttu-id="7bee0-103">구매 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7bee0-103">Azure Marketplace purchasing</span></span>

<span data-ttu-id="7bee0-104">Azure Marketplace 구매, 계산 및 구매 정책 관리 프로세스를 간소화하고 간소화하는 다양한 도구와 기능이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-104">Azure Marketplace has numerous tools and features that simplify and streamline the process of purchasing, invoicing, and managing purchasing policy.</span></span>

## <a name="simplified-procurement"></a><span data-ttu-id="7bee0-105">간소화된 조달</span><span class="sxs-lookup"><span data-stu-id="7bee0-105">Simplified procurement</span></span>

<span data-ttu-id="7bee0-106">Azure Marketplace의 다양한 구매 옵션을 사용하면 조달 프로세스를 간소화하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-106">Azure Marketplace helps you simplify the procurement process through different purchasing options.</span></span> <span data-ttu-id="7bee0-107">Azure 계정과 연결된 신용 카드를 사용하여 제품을 구매하는 경우 모든 구매는 단일 청구서에 통합되고 선택한 신용 카드로 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-107">If you purchase products using a credit card associated with your Azure account, all purchases will be consolidated on a single invoice and billed to the credit card of choice.</span></span> <span data-ttu-id="7bee0-108">대규모 고객인 경우 기업계약 사용하여 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-108">If you are a large customer, you can purchase using an Enterprise Agreement.</span></span> <span data-ttu-id="7bee0-109">EA를 사용하면 모든 소프트웨어 구매가 Azure 청구서에 자동으로 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-109">With an EA, any software purchases are automatically included in your Azure invoice.</span></span> <span data-ttu-id="7bee0-110">청구서에는 먼저 Azure 사용 요금이 포함되고 그 다음에 Azure Marketplace 요금이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-110">Your invoice will contain Azure usage charges first, followed by Azure Marketplace charges.</span></span>

<span data-ttu-id="7bee0-111">Azure Marketplace 통해 구매하는 경우 개별 공급업체 관계 및 청구서를 관리하는 복잡성을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-111">When you purchase through Azure Marketplace, you eliminate the complexity of managing individual vendor relationships and invoices.</span></span> <span data-ttu-id="7bee0-112">Microsoft에서 Azure Marketplace 구매와 Azure 요금을 모두 포함하는 단일 통합 월별 청구서를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-112">You get a single, consolidated monthly bill from Microsoft that includes both your Azure Marketplace purchases and your Azure charges.</span></span>

## <a name="permission-to-purchase"></a><span data-ttu-id="7bee0-113">구매할 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="7bee0-113">Permission to purchase</span></span>

<span data-ttu-id="7bee0-114">올바른 소프트웨어 애플리케이션을 찾은 후에는 구매를 완료하는 것이 간단합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-114">After you've found the right software application, completing the purchase is simple.</span></span> <span data-ttu-id="7bee0-115">그러나 Azure 구독 내에서 적절한 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-115">You will, however, need suitable permissions within the Azure subscription.</span></span> <span data-ttu-id="7bee0-116">Azure는 RBAC(역할 [기반 Access Control)](/azure/role-based-access-control/overview) 모델에서 작동하기 때문에 계정을 구매하려면 **구독 소유자** 또는 **기여자** 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-116">Since Azure operates on a [Role Based Access Control](/azure/role-based-access-control/overview) (RBAC) model, your account needs **subscription owner** or **contributor** permissions to make a purchase.</span></span>

<span data-ttu-id="7bee0-117">구매를 완료하기 전에 사용자가 Azure 테넌트에서 올바른 구성을 가지고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-117">Before completing a purchase, make sure the user has the correct configuration in the Azure tenant.</span></span> <span data-ttu-id="7bee0-118">이렇게 하면 구매하는 동안 오류를 방지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-118">This will help prevent errors during purchase.</span></span>

<span data-ttu-id="7bee0-119">Azure Portal Azure Marketplace 경험에서 구매할 애플리케이션을 찾고 **만들기** 또는 **설정 + 구독을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-119">In the Azure Marketplace experience in the Azure portal, find the application you want to buy and select **Create** or **Set up + subscribe**.</span></span> <span data-ttu-id="7bee0-120">새 솔루션을 사용하기 전에 일부 정보를 완료하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-120">You'll be prompted to complete some information before being able to use your new solution.</span></span>

> [!CAUTION]
> <span data-ttu-id="7bee0-121">프라이빗 마켓플레이스에 대한 승인은 솔루션 조달을 나타내지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-121">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="제안 만들기 단추입니다.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="설정 + 구독 단추입니다.":::

<span data-ttu-id="7bee0-124">Azure Marketplace 온라인 스토어에서 솔루션을 배포하려면 제품 설명 페이지에서 **지금 받기를** 선택한 다음, Azure 계정 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-124">If you want to deploy a solution from the Azure Marketplace online store, select **Get it now** on the product description page and then sign in with your Azure account credentials.</span></span>

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketplace 로그인 대화 상자입니다.":::

<span data-ttu-id="7bee0-126">로그인하면 구매를 완료하기 위해 Azure Portal 제품으로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-126">Once you sign in, you will be redirected to the product in the Azure portal to complete your purchase.</span></span>

## <a name="purchase-policy-management"></a><span data-ttu-id="7bee0-127">구매 정책 관리</span><span class="sxs-lookup"><span data-stu-id="7bee0-127">Purchase policy management</span></span>

<span data-ttu-id="7bee0-128">Microsoft를 사용하면 Azure 구독 관리자로서 청구 프로필을 통해 사용자 구매를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-128">Microsoft lets you manage user purchases through your billing profile as the Azure subscription administrator.</span></span> <span data-ttu-id="7bee0-129">다음 세 가지 옵션 중에서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-129">Choose from three options:</span></span>

- <span data-ttu-id="7bee0-130">**무료 + 유료** – 사용자가 Azure Marketplace 소프트웨어 애플리케이션을 획득할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-130">**Free + Paid** – Allows users to acquire any Azure Marketplace software application.</span></span>
- <span data-ttu-id="7bee0-131">**무료** – 사용자가 Azure Marketplace 무료 소프트웨어만 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-131">**Free** – Allows users to deploy only free software from Azure Marketplace.</span></span>
- <span data-ttu-id="7bee0-132">**아니요** – 사용자가 Azure Marketplace 소프트웨어를 배포할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-132">**No** – Prevents users from deploying any software from Azure Marketplace.</span></span>

<span data-ttu-id="7bee0-133">이러한 설정은 Azure 구독에 액세스할 수 있는 모든 사용자에게 적용되며, 이를 통해 Azure Portal 통해 IT 조달을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-133">These settings apply to all users with access to your Azure subscription, which gives you the capability to control IT procurement through the Azure portal.</span></span>

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure Portal 통해 IT 조달을 제어합니다.":::

## <a name="cost-management"></a><span data-ttu-id="7bee0-135">비용 관리</span><span class="sxs-lookup"><span data-stu-id="7bee0-135">Cost management</span></span>

<span data-ttu-id="7bee0-136">Azure Marketplace 제품을 구매할 때 비용을 관리하는 데 도움이 되는 인사이트를 얻고자 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-136">As you purchase products from Azure Marketplace, you want to get insights that help you manage costs.</span></span> <span data-ttu-id="7bee0-137">Azure Cost Management 구매한 제품에 대한 정보를 볼 수 있는 무료 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-137">Azure Cost Management is a free tool for viewing information on the products you've purchased.</span></span> <span data-ttu-id="7bee0-138">Cost Management 사용하여 시간에 따라 비용을 지출하는 서비스와 해당 비용이 설정한 예산에 대해 어떻게 추적되는지에 대한 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-138">You can use Cost Management to see details of what services you're spending money on over time and how those costs track against the budgets you've set.</span></span> <span data-ttu-id="7bee0-139">예산을 설정하는 것 외에도 보고서를 예약하고 구독 비용을 분석할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-139">In addition to setting budgets, you can schedule reports and analyze subscription costs.</span></span> <span data-ttu-id="7bee0-140">비용 분석 및 Azure Cost Management 예산 [만들기에서](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)Microsoft Learn 모듈을 완료하여 Azure Cost Management 대해 자세히 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-140">Learn more about Azure Cost Management by completing the Microsoft Learn module on [Analyze costs and create budgets with Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).</span></span>

<span data-ttu-id="7bee0-141">Azure Cost Management의 비용 분석 도구에서 Azure Marketplace 요금 및 청구서를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-141">You can view your Azure Marketplace charges and invoices on the cost analysis tool under Azure Cost Management.</span></span>

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Azure Cost Management 사용하여 구매한 제품에 대한 인사이트를 얻습니다.":::

## <a name="purchase-validation-checks"></a><span data-ttu-id="7bee0-143">구매 유효성 검사</span><span class="sxs-lookup"><span data-stu-id="7bee0-143">Purchase validation checks</span></span>

<span data-ttu-id="7bee0-144">Azure Marketplace 통해 제품을 구매하는 것은 여러 가지 이유로 실패할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-144">Purchasing an offer through Azure Marketplace can fail for different reasons.</span></span> <span data-ttu-id="7bee0-145">구매에 CLI(명령줄 인터페이스)를 사용하면 Azure Marketplace 사용할 수 없거나 표시되지 않는 제안을 구매하려고 할 수 있기 때문에 오류가 발생할 가능성이 높습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-145">Using the command-line interface (CLI) for a purchase is more likely to cause errors since you may be trying to purchase an offer that is not available or visible in Azure Marketplace.</span></span> <span data-ttu-id="7bee0-146">다음은 구매 실패를 일으킬 수 있는 검사입니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-146">Following are the checks that can cause a purchase to fail:</span></span>

1. <span data-ttu-id="7bee0-147">구독은 EA(기업계약)에 속하며 EA 관리자는 Azure Marketplace 구매를 사용하지 않도록 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-147">The subscription belongs to an Enterprise Agreement (EA) and the EA admin disabled Azure Marketplace purchases.</span></span>
1. <span data-ttu-id="7bee0-148">EA 관리자는 무료 제안에 대해서만 구매를 사용하도록 설정했으며, 이 제안은 유료 제안입니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-148">The EA admin has enabled purchases only for free offers and the offer is a paid offer.</span></span>
1. <span data-ttu-id="7bee0-149">마켓플레이스에서 제안을 찾을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-149">The offer is not found in the marketplace.</span></span>
1. <span data-ttu-id="7bee0-150">ISV(Independent Software Vendor)는 적어도 해당 지역에서 제안 판매를 중지했습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-150">The Independent Software Vendor (ISV) stopped selling the offer, at least in your region.</span></span>
1. <span data-ttu-id="7bee0-151">사용 중인 구독은 제안을 사용할 수 없는 지역의 청구 계정에 속합니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-151">The subscription you are using belongs to a billing account in a region where the offer is not available.</span></span>
1. <span data-ttu-id="7bee0-152">구독/청구 계정은 유효한 결제 방법(예: 유효한 신용 카드)과 연결되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-152">The subscription/billing account is not associated with a valid payment instrument (such as a valid credit card).</span></span>
1. <span data-ttu-id="7bee0-153">구독이 CSP(클라우드 솔루션 공급자)에 속하고 ISV가 CSP를 통한 판매를 거부했습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-153">The subscription belongs to a Cloud Solution Provider (CSP) and the ISV declined to sell through a CSP.</span></span>
1. <span data-ttu-id="7bee0-154">프라이빗 마켓플레이스는 구독에 대해 사용하도록 설정되며 허용된 제품 목록에는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-154">Private Marketplace is enabled for the subscription and the offer is not in the list of allowed offers.</span></span>
1. <span data-ttu-id="7bee0-155">이 제안은 특정 고객에 대한 프라이빗/미리 보기이며 구독은 허용된 고객 목록에 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7bee0-155">The offer is Private/Preview for specific customers and the subscription is not in the list of allowed customers.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7bee0-156">다음 단계</span><span class="sxs-lookup"><span data-stu-id="7bee0-156">Next steps</span></span>

- [<span data-ttu-id="7bee0-157">청구 및 송장 작성</span><span class="sxs-lookup"><span data-stu-id="7bee0-157">Billing and invoicing</span></span>](billing-invoicing.md)