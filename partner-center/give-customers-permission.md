---
title: 고객에게 자신의 서비스를 구매할 수 있는 권한 부여
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 프로그램 파트너가 고객에 게 구매한 구독에 대 한 Azure 예약과 같은 고유한 서비스를 구입할 수 있도록 하는 방법을 알아봅니다.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: 구독, 셀프 서비스 구매, 셀프 서비스 RI, RI 사용, ri 사용 안 함, 셀프 서비스, 고객 구매, 고객 권한, 고객 구매 예약 인스턴스, 고객 구입 Azure 예약, 셀프 서비스를 사용 하도록 설정
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255467"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a><span data-ttu-id="cf073-104">고객에 게 자신의 제품 또는 서비스를 구매할 수 있는 권한을 부여 하는 방법을 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-104">Learn how to give customers permission to buy their own products or services</span></span>

<span data-ttu-id="cf073-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="cf073-105">**Applies to**</span></span>

- <span data-ttu-id="cf073-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="cf073-106">Partner Center</span></span>
- <span data-ttu-id="cf073-107">CSP 프로그램의 파트너</span><span class="sxs-lookup"><span data-stu-id="cf073-107">Partners in the CSP program</span></span>

<span data-ttu-id="cf073-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="cf073-108">**Appropriate roles**</span></span>

- <span data-ttu-id="cf073-109">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="cf073-109">Admin agent</span></span>
- <span data-ttu-id="cf073-110">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="cf073-110">Sales agent</span></span>

<span data-ttu-id="cf073-111">이 문서에서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너가 고객에 게 자신의 서비스 또는 리소스 중 일부를 구매할 수 있는 권한을 부여 하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-111">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="cf073-112">CSP 프로그램의 파트너는 파트너 센터와 상용 마켓플레이스를 사용 하 여 고객을 위한 솔루션 및 서비스를 구입 하는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-112">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="cf073-113">파트너는 일부 고객이 Azure Portal에서 직접 이러한 서비스를 프로 비전 할 수 있도록 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-113">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="cf073-114">예를 들면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-114">Here's an example.</span></span> <span data-ttu-id="cf073-115">파트너 센터에서 고객에 대 한 Azure 계획 구독을 구매 한다고 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-115">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="cf073-116">그런 다음 고객을 대신 하 여 해당 구독에 다른 리소스 또는 서비스를 추가 하기로 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-116">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="cf073-117">이 경우 고객의 구독 (예: 예약 된 가상 머신 인스턴스 추가)에 Azure 예약을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-117">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="cf073-118">그런 다음 고객이 Azure Portal에서 Azure 예약 리소스를 추가로 프로 비전 하도록 허용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-118">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="cf073-119">이제 **고객 권한** 기능을 사용 하 여 고객에 게 Azure 리소스를 통해 더 많은 셀프 서비스 옵션을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-119">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="cf073-120">고객에 대 한 권한을 설정 하 여 고객은 자신의 리소스 (예: 자신의 Azure 예약 구입)를 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-120">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="cf073-121">파트너 센터의 고객 권한 개요</span><span class="sxs-lookup"><span data-stu-id="cf073-121">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="cf073-122">고객 **계정** 페이지를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-122">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="cf073-123">현재이 기능은 다음을 지원 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-123">Currently, this feature supports:</span></span>

- <span data-ttu-id="cf073-124">**Azure 예약:** 이 권한을 설정 하면 고객이 구매한 특정 Azure 구독에 대해 자신의 Azure 예약을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-124">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="cf073-125">고객 권한을 설정 하기 전에 다음과 같은 중요 한 사항에 유의 하십시오.</span><span class="sxs-lookup"><span data-stu-id="cf073-125">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="cf073-126">기본적으로 고객 권한은 파트너 센터에서 자동으로 사용 하지 않도록 설정 (해제) 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-126">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>
- <span data-ttu-id="cf073-127">고객에 대 한 권한을 설정 하거나 해제 하려면 먼저 파트너 센터에서 관리 에이전트의 역할을 할당 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-127">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>
  <span data-ttu-id="cf073-128">판매 에이전트 또는 지원 센터 에이전트의 역할이 할당 된 파트너는 읽기 전용 액세스 권한을 가지 며 고객 권한을 설정 하거나 해제할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-128">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>
- <span data-ttu-id="cf073-129">선택한 모든 고객에 대 한 사용 권한을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-129">You can turn on (enable) permissions for any customer you choose.</span></span>
- <span data-ttu-id="cf073-130">파트너 센터 대시보드 또는 [파트너 센터 api](https://docs.microsoft.com/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-130">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>
- <span data-ttu-id="cf073-131">특정 고객에 대 한 사용 권한을 설정한 후에는 해당 고객의 이후 구매에 대 한 요금을 지불 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-131">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="cf073-132">고객이 구매한 구매를 교환 하거나 취소 하거나 갱신 하려는 경우에는 자체적으로 수행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-132">If customers want to exchange, cancel or renew a purchase they have made, they will not be able to do so themselves.</span></span> <span data-ttu-id="cf073-133">파트너는 이러한 구매를 교환, 취소 또는 갱신할 수 있도록 파트너에 게 요청 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-133">They need to ask you, as the partner, to help them exchange, cancel, or renew these purchases.</span></span>
- <span data-ttu-id="cf073-134">특정 고객에 대 한 사용 권한을 설정한 후에는 고객의 이후 구매에 대 한 알림이 표시 **되지** 않습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-134">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>
- <span data-ttu-id="cf073-135">고객의 나중에 구매한 제품은 사용자가 구입한 모든 구매와 함께 파트너 센터에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-135">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="cf073-136">고객의 **주문 기록** 페이지, 해당 **예약** 페이지 또는 [**활동 로그**](activity-logs.md)에서 이러한 구매를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-136">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="cf073-137">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="cf073-137">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="cf073-138">Azure 예약은 할인 된 요금으로 Azure 서비스를 구매할 수 있는 좋은 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-138">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="cf073-139">Azure 예약의 이점에 대 한 자세한 내용은 [Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="cf073-139">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="cf073-140">이제 이미 수행 했을 수 있으므로 고객을 대신 하 여 Azure 예약을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-140">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="cf073-141">또는 고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-141">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="cf073-142">사용자가 자신의 Azure 예약을 구매할 수 있는 권한을 부여한 후에는 구매한 예약을 관리 하는 방법을 이해 하는 데 도움을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-142">After you give customers permission to buy their own Azure reservations, you can help them understand how to manage any reservations they purchase.</span></span> <span data-ttu-id="cf073-143">예를 들어 고객은 예약 사용을 최적화 하는 방법 또는 예약의 범위를 변경 하는 방법을 알고 싶을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-143">For instance, customers might want to know how to optimize their use of a reservation or how to change a reservation’s scope.</span></span> <span data-ttu-id="cf073-144">이러한 항목에 대 한 자세한 내용은 [Azure 리소스에 대 한 예약 관리]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance)를 고객에 게 요청 하세요.</span><span class="sxs-lookup"><span data-stu-id="cf073-144">For more information about these topics, ask customers to read [Manage reservations for Azure resources]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="cf073-145">고객이 자신의 Azure 예약을 구매할 수 있도록 하려면</span><span class="sxs-lookup"><span data-stu-id="cf073-145">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="cf073-146">고객이 대신 구매한 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-146">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="cf073-147">이 구독에 대 한 **소유자** 역할이 사용자에 게 할당 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-147">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="cf073-148">고객 권한 (이 기능 **을**설정)을 사용 하 여 자신의 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-148">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="cf073-149">각 단계가 아래에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-149">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="cf073-150">고객이 기존 Azure 구독을 보유 하 고 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="cf073-150">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="cf073-151">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하기 전에 고객이 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-151">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="cf073-152">고객이 파트너 센터에 현재 Azure 구독을 표시 하지 않는 경우 고객 권한을 설정 하기 전에 구독을 구입 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-152">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="cf073-153">고객이 이미 Azure 구독을 보유 하 고 있는지 확인 하려면 파트너 센터 대시보드에 로그인 한 다음 **CSP** 와 **고객**을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-153">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="cf073-154">목록에서 특정 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-154">Select the specific customer from the list.</span></span> <span data-ttu-id="cf073-155">그런 다음 **구독** 을 선택 하 고 azure 요금제 또는 azure Global에 대 한 사용 빈도 기반 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-155">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="cf073-156">고객이 기존 Azure 구독을 보유 하 고 있지 않은 경우 해당 구독을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-156">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="cf073-157">[Azure 계획 구매를](purchase-azure-plan.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="cf073-157">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="cf073-158">Azure에서 고객이 올바른 역할을 할당 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-158">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="cf073-159">고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후에는 고객과 연결 된 키 사용자에 게 해당 Azure 구독에 대 한 올바른 **소유자** 역할이 할당 되었는지도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-159">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="cf073-160">사용자가 구매한 Azure 구독에 대해 Azure 예약을 구입 해야 하는 RBAC (역할 기반 액세스)입니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-160">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="cf073-161">일부 파트너는 자신의 Azure 리소스를 적극적으로 관리 하 고 프로 비전 하려는 고객에 게 **소유자** 역할을 이미 할당 했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-161">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="cf073-162">구매한 이전 구독을 관리 하기 위해 고객에 게 **소유자** 상태를 이미 할당 한 경우이 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-162">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="cf073-163">담당자에 게 **소유자** 역할이 할당 되지 않은 경우 Azure 예약을 구매 하지 못하도록 하는 Azure Portal 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-163">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="cf073-164">고객에 게 Azure 구독에 대 한 **소유자** 역할이 할당 되었는지 확인 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-164">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="cf073-165">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cf073-166">**CSP**, **고객** 을 차례로 선택 하 고 특정 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-166">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="cf073-167">해당 고객에 대 한 **구독** 을 선택 하 고 특정 Azure 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-167">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="cf073-168">해당 고객의 구독 옆에 있는 **관리** 단추를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-168">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="cf073-169">이렇게 하면 [Azure Portal](https://portal.azure.com/)열립니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-169">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="cf073-170">특정 사용자에 게 **소유자** 역할을 할당 하려면 다음 단계에 따라 [사용자를 관리자로 할당](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-170">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="cf073-171">고객 권한을 설정 하거나 해제 하 여 자신의 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-171">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="cf073-172">고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후 사용자에 게 해당 구독에 대 한 **소유자** 역할이 할당 되 면 고객 권한을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-172">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="cf073-173">이러한 단계를 사용 하 여 고객 권한을 해제 (해제) 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-173">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="cf073-174">파트너 센터 대시보드 또는 [파트너 센터 api](https://docs.microsoft.com/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-174">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="cf073-175">파트너 센터에서 고객 권한을 설정 하거나 해제 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-175">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="cf073-176">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-176">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cf073-177">왼쪽 탐색 메뉴에서 **CSP**, **고객**을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-177">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="cf073-178">고객 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-178">A customer list appears.</span></span>

3. <span data-ttu-id="cf073-179">특정 고객 이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-179">Select a specific customer name.</span></span>

4. <span data-ttu-id="cf073-180">고객 메뉴에서 **계정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-180">Select **Account** from the customer menu.</span></span> <span data-ttu-id="cf073-181">고객 **계정** 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-181">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="cf073-182">페이지 맨 아래에 있는 **고객 권한** 영역을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-182">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   ![계정 페이지에 대 한 고객 권한](images/give-customers-permission-reservations.png)

6. <span data-ttu-id="cf073-184">**Azure 예약**에서 **고객이 구매할 수 있음** 옵션을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-184">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="cf073-185">고객 권한을 설정 하려면이 옵션 옆의 스위치를 **on** 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-185">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="cf073-186">고객 권한을 해제 하려면 스위치를 **off** 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-186">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="cf073-187">자신의 Azure 예약을 구매 하기 위해 고객의 권한을 설정할 때 발생 하는 다른 작업에 대해 알아보려면 [파트너 센터에서 고객 권한 개요](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="cf073-187">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span> <span data-ttu-id="cf073-188">고객 권한을 설정 하거나 해제 하면 활동 로그에서 각 작업을 기록 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-188">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="cf073-189">파트너 센터 대시보드 위쪽에서 기어 아이콘을 선택 하면이 로그에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-189">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="cf073-190">고객 권한을 설정 하거나 해제 하는 경우 작업은 **고객 구매 권한 만들기** 또는 **고객 구매 권한 삭제** 를 활동 로그에 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf073-190">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="see-also"></a><span data-ttu-id="cf073-191">참고 항목</span><span class="sxs-lookup"><span data-stu-id="cf073-191">See also</span></span>

- [<span data-ttu-id="cf073-192">고객을 대신 하 여 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="cf073-192">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="cf073-193">파트너 센터-Microsoft 예약 판매</span><span class="sxs-lookup"><span data-stu-id="cf073-193">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)
- [<span data-ttu-id="cf073-194">고객을 대신 하 여 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="cf073-194">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md) 