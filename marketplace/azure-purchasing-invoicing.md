---
title: Azure Marketplace에서 소프트웨어 및 솔루션 구매
description: Azure Marketplace에서 소프트웨어 구매 및 관리를 간소화 하 고 간소화 하는 도구에 대해 알아봅니다.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: de58fad7af7dd2cd6b8c98e5763557d54cc776a2
ms.sourcegitcommit: c46658f4d70004596e758fe4cd8671b6e9dadeab
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/20/2021
ms.locfileid: "98584203"
---
# <a name="azure-marketplace-purchasing"></a><span data-ttu-id="3f4b3-103">Azure Marketplace 구매</span><span class="sxs-lookup"><span data-stu-id="3f4b3-103">Azure Marketplace purchasing</span></span>

<span data-ttu-id="3f4b3-104">Azure Marketplace는 구매 정책 구매, 청구 및 관리 프로세스를 간소화 하 고 간소화 하는 다양 한 도구와 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-104">Azure Marketplace has numerous tools and features that simplify and streamline the process of purchasing, invoicing, and managing purchasing policy.</span></span>

## <a name="simplified-procurement"></a><span data-ttu-id="3f4b3-105">조달 조달</span><span class="sxs-lookup"><span data-stu-id="3f4b3-105">Simplified procurement</span></span>

<span data-ttu-id="3f4b3-106">Azure Marketplace의 다양한 구매 옵션을 사용하면 조달 프로세스를 간소화하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-106">Azure Marketplace helps you simplify the procurement process through different purchasing options.</span></span> <span data-ttu-id="3f4b3-107">Azure 계정과 연결 된 신용 카드를 사용 하 여 제품을 구매 하는 경우 모든 구매는 단일 송장에 통합 되며 선택한 신용 카드로 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-107">If you purchase products using a credit card associated with your Azure account, all purchases will be consolidated on a single invoice and billed to the credit card of choice.</span></span> <span data-ttu-id="3f4b3-108">규모가 많은 고객의 경우 기업계약를 사용 하 여 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-108">If you are a large customer, you can purchase using an Enterprise Agreement.</span></span> <span data-ttu-id="3f4b3-109">EA를 사용 하면 모든 소프트웨어 구매가 Azure 청구서에 자동으로 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-109">With an EA, any software purchases are automatically included in your Azure invoice.</span></span> <span data-ttu-id="3f4b3-110">청구서에는 먼저 Azure 사용 요금이 포함되고 그 다음에 Azure Marketplace 요금이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-110">Your invoice will contain Azure usage charges first, followed by Azure Marketplace charges.</span></span>

<span data-ttu-id="3f4b3-111">Azure Marketplace를 통해 구매 하는 경우 개별 공급 업체 관계와 송장을 관리 하는 복잡성을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-111">When you purchase through Azure Marketplace, you eliminate the complexity of managing individual vendor relationships and invoices.</span></span> <span data-ttu-id="3f4b3-112">Microsoft에서 Azure Marketplace 구매 및 Azure 요금을 모두 포함 하는 통합 된 단일 월별 요금 청구를 받습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-112">You get a single, consolidated monthly bill from Microsoft that includes both your Azure Marketplace purchases and your Azure charges.</span></span>

## <a name="permission-to-purchase"></a><span data-ttu-id="3f4b3-113">구입할 권한</span><span class="sxs-lookup"><span data-stu-id="3f4b3-113">Permission to purchase</span></span>

<span data-ttu-id="3f4b3-114">올바른 소프트웨어 응용 프로그램을 찾았으면 구매를 완료 하는 것이 간단 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-114">After you've found the right software application, completing the purchase is simple.</span></span> <span data-ttu-id="3f4b3-115">그러나 Azure 구독 내에서 적절 한 사용 권한이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-115">You will, however, need suitable permissions within the Azure subscription.</span></span> <span data-ttu-id="3f4b3-116">Azure는 RBAC ( [역할 기반 Access Control](/azure/role-based-access-control/overview) ) 모델에서 작동 하므로 구매 하려면 계정에 **구독 소유자** 또는 **참가자** 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-116">Since Azure operates on a [Role Based Access Control](/azure/role-based-access-control/overview) (RBAC) model, your account needs **subscription owner** or **contributor** permissions to make a purchase.</span></span>

<span data-ttu-id="3f4b3-117">구매를 완료 하기 전에 사용자에 게 Azure 테 넌 트의 올바른 구성이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-117">Before completing a purchase, make sure the user has the correct configuration in the Azure tenant.</span></span> <span data-ttu-id="3f4b3-118">이렇게 하면 구매 중에 오류를 방지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-118">This will help prevent errors during purchase.</span></span>

<span data-ttu-id="3f4b3-119">Azure Portal의 Azure Marketplace 환경에서 구매할 응용 프로그램을 찾고 **만들기** 또는 **설정 + 구독** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-119">In the Azure Marketplace experience in the Azure portal, find the application you want to buy and select **Create** or **Set up + subscribe**.</span></span> <span data-ttu-id="3f4b3-120">새 솔루션을 사용할 수 있기 전에 몇 가지 정보를 입력 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-120">You'll be prompted to complete some information before being able to use your new solution.</span></span>

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="제안 만들기 단추입니다.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="설정 + 구독 단추입니다.":::

<span data-ttu-id="3f4b3-123">Azure Marketplace online 스토어에서 솔루션을 배포 하려면 제품 설명 페이지에서 **지금 가져오기** 를 선택 하 고 Azure 계정 자격 증명을 사용 하 여 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-123">If you want to deploy a solution from the Azure Marketplace online store, select **Get it now** on the product description page and then sign in with your Azure account credentials.</span></span>

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketplace 로그인 대화 상자입니다.":::

<span data-ttu-id="3f4b3-125">로그인 하면 Azure Portal의 제품으로 리디렉션되고 구매를 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-125">Once you sign in, you will be redirected to the product in the Azure portal to complete your purchase.</span></span>

## <a name="purchase-policy-management"></a><span data-ttu-id="3f4b3-126">구매 정책 관리</span><span class="sxs-lookup"><span data-stu-id="3f4b3-126">Purchase policy management</span></span>

<span data-ttu-id="3f4b3-127">Microsoft에서는 청구 프로필을 통해 Azure 구독 관리자로 사용자 구매를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-127">Microsoft lets you manage user purchases through your billing profile as the Azure subscription administrator.</span></span> <span data-ttu-id="3f4b3-128">다음 세 가지 옵션 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-128">Choose from three options:</span></span>

- <span data-ttu-id="3f4b3-129">**무료 + 유료** – 사용자가 모든 Azure Marketplace 소프트웨어 응용 프로그램을 확보할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-129">**Free + Paid** – Allows users to acquire any Azure Marketplace software application.</span></span>
- <span data-ttu-id="3f4b3-130">**무료** – 사용자가 Azure Marketplace에서 무료 소프트웨어만 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-130">**Free** – Allows users to deploy only free software from Azure Marketplace.</span></span>
- <span data-ttu-id="3f4b3-131">**아니요** – 사용자가 Azure Marketplace에서 소프트웨어를 배포 하지 못하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-131">**No** – Prevents users from deploying any software from Azure Marketplace.</span></span>

<span data-ttu-id="3f4b3-132">이러한 설정은 Azure 구독에 대 한 액세스 권한이 있는 모든 사용자에 게 적용 되어 Azure Portal를 통해 IT 조달을 제어 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-132">These settings apply to all users with access to your Azure subscription, which gives you the capability to control IT procurement through the Azure portal.</span></span>

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure Portal를 통해 IT 조달 제어":::

## <a name="cost-management"></a><span data-ttu-id="3f4b3-134">비용 관리</span><span class="sxs-lookup"><span data-stu-id="3f4b3-134">Cost management</span></span>

<span data-ttu-id="3f4b3-135">Azure Marketplace에서 제품을 구매할 때 비용을 관리 하는 데 도움이 되는 정보를 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-135">As you purchase products from Azure Marketplace, you want to get insights that help you manage costs.</span></span> <span data-ttu-id="3f4b3-136">Azure Cost Management은 구매한 제품에 대 한 정보를 볼 수 있는 무료 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-136">Azure Cost Management is a free tool for viewing information on the products you've purchased.</span></span> <span data-ttu-id="3f4b3-137">Cost Management를 사용 하 여 시간에 따라 비용을 지불 하는 서비스 및 설정 된 예산에 대해 해당 비용을 추적 하는 방법에 대 한 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-137">You can use Cost Management to see details of what services you're spending money on over time and how those costs track against the budgets you've set.</span></span> <span data-ttu-id="3f4b3-138">예산을 설정 하는 것 외에도 보고서를 예약 하 고 구독 비용을 분석할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-138">In addition to setting budgets, you can schedule reports and analyze subscription costs.</span></span> <span data-ttu-id="3f4b3-139">[비용 분석 및 Azure Cost Management를 사용 하 여 예산 만들기](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)에서 Microsoft Learn 모듈을 완료 하 여 Azure Cost Management에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-139">Learn more about Azure Cost Management by completing the Microsoft Learn module on [Analyze costs and create budgets with Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).</span></span>

<span data-ttu-id="3f4b3-140">Azure Cost Management의 비용 분석 도구에서 Azure Marketplace 요금 및 청구서를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-140">You can view your Azure Marketplace charges and invoices on the cost analysis tool under Azure Cost Management.</span></span>

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Azure Cost Management를 사용 하 여 구매한 제품에 대 한 정보를 얻을 수 있습니다.":::

## <a name="purchase-validation-checks"></a><span data-ttu-id="3f4b3-142">유효성 검사 구매</span><span class="sxs-lookup"><span data-stu-id="3f4b3-142">Purchase validation checks</span></span>

<span data-ttu-id="3f4b3-143">Azure Marketplace를 통해 제품을 구매 하는 것은 다양 한 이유로 실패할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-143">Purchasing an offer through Azure Marketplace can fail for different reasons.</span></span> <span data-ttu-id="3f4b3-144">Azure Marketplace에서 제공 되지 않거나 표시 되지 않는 제품을 구매 하려고 할 수 있으므로 구매에 CLI (명령줄 인터페이스)를 사용 하면 오류가 발생할 가능성이 높습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-144">Using the command-line interface (CLI) for a purchase is more likely to cause errors since you may be trying to purchase an offer that is not available or visible in Azure Marketplace.</span></span> <span data-ttu-id="3f4b3-145">다음은 구매가 실패할 수 있는 검사입니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-145">Following are the checks that can cause a purchase to fail:</span></span>

1. <span data-ttu-id="3f4b3-146">구독은 EA (기업계약)에 속하며 EA 관리자는 구매 Azure Marketplace 사용 하지 않도록 설정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-146">The subscription belongs to an Enterprise Agreement (EA) and the EA admin disabled Azure Marketplace purchases.</span></span>
1. <span data-ttu-id="3f4b3-147">EA 관리자는 무료 제품에 대해서만 구매를 사용 하도록 설정 했으며 제품은 유료 제품입니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-147">The EA admin has enabled purchases only for free offers and the offer is a paid offer.</span></span>
1. <span data-ttu-id="3f4b3-148">Marketplace에서 제품을 찾을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-148">The offer is not found in the marketplace.</span></span>
1. <span data-ttu-id="3f4b3-149">ISV (독립 소프트웨어 공급 업체)가 최소한의 지역에서 제품 판매를 중지 했습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-149">The Independent Software Vendor (ISV) stopped selling the offer, at least in your region.</span></span>
1. <span data-ttu-id="3f4b3-150">사용 중인 구독은 제품을 사용할 수 없는 지역의 청구 계정에 속합니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-150">The subscription you are using belongs to a billing account in a region where the offer is not available.</span></span>
1. <span data-ttu-id="3f4b3-151">구독/청구 계정이 유효한 결제 방법 (예: 유효한 신용 카드)과 연결 되어 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-151">The subscription/billing account is not associated with a valid payment instrument (such as a valid credit card).</span></span>
1. <span data-ttu-id="3f4b3-152">구독이 CSP (클라우드 솔루션 공급자)에 속하며 ISV가 CSP를 통해 판매 하지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-152">The subscription belongs to a Cloud Solution Provider (CSP) and the ISV declined to sell through a CSP.</span></span>
1. <span data-ttu-id="3f4b3-153">구독에 대해 개인 Marketplace가 사용 하도록 설정 되어 있으며 제품이 허용 된 제안 목록에 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-153">Private Marketplace is enabled for the subscription and the offer is not in the list of allowed offers.</span></span>
1. <span data-ttu-id="3f4b3-154">제품이 특정 고객에 대 한 비공개/미리 보기 이며, 구독이 허용 된 고객 목록에 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3f4b3-154">The offer is Private/Preview for specific customers and the subscription is not in the list of allowed customers.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3f4b3-155">다음 단계</span><span class="sxs-lookup"><span data-stu-id="3f4b3-155">Next steps</span></span>

- [<span data-ttu-id="3f4b3-156">청구 및 송장 작성</span><span class="sxs-lookup"><span data-stu-id="3f4b3-156">Billing and invoicing</span></span>](billing-invoicing.md)