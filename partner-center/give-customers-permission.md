---
title: 고객이 CSP에서 자신의 서비스를 구매할 수 있도록 허용
description: CSP 프로그램 파트너가 고객이 파트너 센터 구매한 구독에 대해 Azure 예약과 같은 자체 서비스를 구매할 수 있도록 하는 방법을 알아봅니다.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150763"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="b1818-103">고객에게 파트너 센터 자신의 제품 또는 서비스를 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="b1818-103">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="b1818-104">**적절한 역할:** 관리 에이전트 | 판매 에이전트</span><span class="sxs-lookup"><span data-stu-id="b1818-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="b1818-105">이 문서에서는 CSP(클라우드 솔루션 공급자) 프로그램의 파트너가 자신의 서비스 또는 리소스 중 일부를 구매할 수 있는 권한을 고객에게 부여하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-105">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="b1818-106">CSP 프로그램의 파트너는 종종 파트너 센터 및 상업용 Marketplace를 사용하여 고객을 위한 솔루션과 서비스를 구입합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-106">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="b1818-107">그런 다음 파트너는 일부 고객이 Azure Portal 직접 이러한 서비스를 프로비전할 수 있도록 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-107">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="b1818-108">예를 들면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-108">Here's an example.</span></span> <span data-ttu-id="b1818-109">파트너 센터 고객에 대한 Azure 플랜 구독을 구입한다고 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-109">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="b1818-110">그런 다음, 고객을 대신하여 해당 구독에 다른 리소스 또는 서비스를 추가하기로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-110">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="b1818-111">이 경우 고객의 구독에 Azure 예약을 추가할 수 있습니다(예: 예약된 가상 머신 인스턴스 추가).</span><span class="sxs-lookup"><span data-stu-id="b1818-111">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="b1818-112">그런 다음 고객이 Azure Portal Azure 예약 리소스를 추가로 프로비저닝하도록 허용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-112">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="b1818-113">이제 고객 **권한** 기능을 통해 고객에게 Azure 리소스를 통해 더 많은 셀프 서비스 옵션을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-113">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="b1818-114">고객에 대한 권한을 설정하여 고객이 자신의 리소스(예: 자신의 Azure 예약 구매)를 구매할 수 있도록 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-114">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="b1818-115">파트너 센터 고객 권한 개요</span><span class="sxs-lookup"><span data-stu-id="b1818-115">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="b1818-116">고객 **계정** 페이지를 사용하여 고객 권한을 설정(또는 해제)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-116">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="b1818-117">현재 이 기능은 다음을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-117">Currently, this feature supports:</span></span>

- <span data-ttu-id="b1818-118">**Azure 예약:** 이 권한을 설정하면 고객이 구매한 특정 Azure 구독에 대해 자신의 Azure 예약을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-118">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="b1818-119">고객 권한을 설정하기 전에 다음 중요한 사항에 유의하세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-119">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="b1818-120">기본적으로 고객 권한은 파트너 센터 자동으로 비활성화(해제)됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-120">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="b1818-121">고객에 대한 사용 권한을 설정(또는 해제)하려면 먼저 파트너 센터 관리 에이전트의 역할이 할당되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-121">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="b1818-122">영업 담당자 또는 지원 센터 에이전트 역할이 할당된 파트너는 읽기 전용 액세스 권한을 가지며 고객 권한을 설정하거나 해제할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-122">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="b1818-123">선택한 모든 고객에 대해 사용 권한을 설정(사용)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-123">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="b1818-124">파트너 센터 대시보드 또는 파트너 센터 API를 사용하여 고객 권한을 설정(또는 해제)할 수 [있습니다.](/partner-center/develop/manage-customers)</span><span class="sxs-lookup"><span data-stu-id="b1818-124">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="b1818-125">특정 고객에 대한 사용 권한을 설정(사용)한 후에는 해당 고객이 구매한 후속 구매에 대해 요금을 지불할 책임이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-125">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="b1818-126">고객이 구매한 구매를 교환, 취소 또는 갱신하려는 경우(또는 예약의 초기 범위를 변경하려는 경우) 고객이 직접 교환하거나 취소하거나 갱신할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-126">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="b1818-127">파트너는 구매를 교환, 취소 및 갱신하거나 나중에 예약 범위를 변경할 수 있도록 파트너에게 요청해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-127">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="b1818-128">특정 고객에 대한 사용 권한을 설정하면 고객이 나중에 구매한 내용에 대한 알림이 **없습니다.**</span><span class="sxs-lookup"><span data-stu-id="b1818-128">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="b1818-129">고객이 나중에 구매한 내용은 고객이 구매한 내용과 함께 파트너 센터 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-129">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="b1818-130">이러한 구매는 고객의 **주문 기록** 페이지, **예약** 페이지 또는 [**활동 로그**](activity-logs.md)에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-130">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="b1818-131">고객이 지불할 가격 및 고객이 구매를 관리하는 방법에 대한 자세한 내용은 고객이 [구매한 예약을 관리하는 데 도움을](give-customers-permission.md#help-customers-manage-reservations-they-purchase)참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-131">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="b1818-132">고객에게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="b1818-132">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="b1818-133">Azure 예약은 할인된 요금으로 Azure 서비스를 구입할 수 있는 좋은 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-133">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="b1818-134">Azure 예약의 이점에 대한 자세한 내용은 [Azure Reservations란?을 참조하세요.](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="b1818-134">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="b1818-135">이제 이미 수행 중일 수 있는 것처럼 고객을 대신하여 Azure 예약을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-135">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="b1818-136">또는 고객에게 자신의 Azure 예약을 구매할 수 있는 권한을 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-136">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="b1818-137">고객에게 자신의 Azure 예약을 구매할 수 있는 권한을 부여한 후 구매한 모든 예약을 관리하는 데 도움을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-137">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="b1818-138">자세한 내용은 [고객이 구매한 예약 관리 지원](give-customers-permission.md#help-customers-manage-reservations-they-purchase)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-138">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="b1818-139">고객이 자신의 Azure 예약을 구매할 수 있도록 하려면</span><span class="sxs-lookup"><span data-stu-id="b1818-139">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="b1818-140">고객이 대신 구매한 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-140">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="b1818-141">이 구독에 대 한 **소유자** 역할이 사용자에 게 할당 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-141">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="b1818-142">고객 권한 (이 기능 **을** 설정)을 사용 하 여 자신의 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-142">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="b1818-143">각 단계가 아래에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-143">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="b1818-144">고객이 기존 Azure 구독을 보유 하 고 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="b1818-144">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="b1818-145">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하기 전에 고객이 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-145">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="b1818-146">고객이 파트너 센터에 현재 Azure 구독을 표시 하지 않는 경우 고객 권한을 설정 하기 전에 구독을 구입 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-146">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="b1818-147">고객이 이미 Azure 구독을 보유 하 고 있는지 확인 하려면 파트너 센터 대시보드에 로그인 한 다음 **CSP** 와 **고객** 을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-147">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="b1818-148">목록에서 특정 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-148">Select the specific customer from the list.</span></span> <span data-ttu-id="b1818-149">그런 다음 **구독** 을 선택 하 고 azure 요금제 또는 azure Global에 대 한 사용 빈도 기반 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-149">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="b1818-150">고객이 기존 Azure 구독을 보유 하 고 있지 않은 경우 해당 구독을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-150">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="b1818-151">[Azure 계획 구매를](purchase-azure-plan.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-151">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="b1818-152">Azure에서 고객이 올바른 역할을 할당 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-152">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="b1818-153">고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후에는 고객과 연결 된 키 사용자에 게 해당 Azure 구독에 대 한 올바른 **소유자** 역할이 할당 되었는지도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-153">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="b1818-154">사용자가 구매한 Azure 구독에 대해 Azure 예약을 구입 해야 하는 RBAC (역할 기반 액세스)입니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-154">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="b1818-155">일부 파트너는 자신의 Azure 리소스를 적극적으로 관리 하 고 프로 비전 하려는 고객에 게 **소유자** 역할을 이미 할당 했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-155">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="b1818-156">구매한 이전 구독을 관리 하기 위해 고객에 게 **소유자** 상태를 이미 할당 한 경우이 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-156">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="b1818-157">담당자에 게 **소유자** 역할이 할당 되지 않은 경우 Azure 예약을 구매 하지 못하도록 하는 Azure Portal 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-157">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="b1818-158">고객에 게 Azure 구독에 대 한 **소유자** 역할이 할당 되었는지 확인 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-158">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="b1818-159">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-159">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b1818-160">**CSP**, **고객** 을 차례로 선택 하 고 특정 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-160">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="b1818-161">해당 고객에 대 한 **구독** 을 선택 하 고 특정 Azure 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-161">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="b1818-162">해당 고객의 구독 옆에 있는 **관리** 단추를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-162">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="b1818-163">이렇게 하면 [Azure Portal](https://portal.azure.com/)열립니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-163">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="b1818-164">특정 사용자에 게 **소유자** 역할을 할당 하려면 다음 단계에 따라 [사용자를 관리자로 할당](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-164">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="b1818-165">고객 권한을 설정 하거나 해제 하 여 자신의 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-165">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="b1818-166">고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후 사용자에 게 해당 구독에 대 한 **소유자** 역할이 할당 되 면 고객 권한을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-166">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="b1818-167">이러한 단계를 사용 하 여 고객 권한을 해제 (해제) 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-167">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="b1818-168">파트너 센터 대시보드 또는 [파트너 센터 api](/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-168">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="b1818-169">파트너 센터에서 고객 권한을 설정 하거나 해제 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-169">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="b1818-170">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-170">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b1818-171">왼쪽 탐색 메뉴에서 **CSP**, **고객** 을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-171">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="b1818-172">고객 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-172">A customer list appears.</span></span>

3. <span data-ttu-id="b1818-173">특정 고객 이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-173">Select a specific customer name.</span></span>

4. <span data-ttu-id="b1818-174">고객 메뉴에서 **계정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-174">Select **Account** from the customer menu.</span></span> <span data-ttu-id="b1818-175">고객 **계정** 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-175">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="b1818-176">페이지 맨 아래에 있는 **고객 권한** 영역을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-176">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="계정 페이지에 대 한 고객 권한입니다." border="true":::

6. <span data-ttu-id="b1818-178">**Azure 예약** 에서 **고객이 구매할 수 있음** 옵션을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-178">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="b1818-179">고객 권한을 켜려면 이 옵션 옆에 있는 스위치를 **켜기** 위치로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-179">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="b1818-180">고객 권한을 해제하려면 스위치를 **끄기** 위치로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-180">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="b1818-181">고객의 사용 권한을 설정하여 자신의 Azure 예약을 구매할 때 발생하는 다른 일을 알아보려면 [파트너 센터 고객 권한 개요를](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-181">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="b1818-182">고객 권한을 설정(또는 해제)하면 활동 로그는 각 작업을 기록합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-182">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="b1818-183">(이 로그는 파트너 센터 대시보드의 위쪽에서 기어 아이콘을 선택하면 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-183">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="b1818-184">고객 권한을 설정하거나 해제하면 활동 로그에서 **고객 구매 권한 만들기** 또는 고객 구매 **권한 삭제로** 작업이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-184">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="b1818-185">고객이 구매한 예약을 관리하는 데 도움을 주세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-185">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="b1818-186">고객에게 자신의 Azure 예약을 구매할 수 있는 권한을 부여하면 구매한 리소스를 더 잘 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-186">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="b1818-187">고객은 [Azure Portal](https://portal.azure.com/)직접 Azure 예약의 여러 측면을 직접 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-187">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="b1818-188">CSP 구독 내에서 구매하는 Azure 예약의 몇 가지 다른 측면을 관리하는 데 도움이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-188">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="b1818-189">고객이 Azure 예약의 이러한 측면을 관리하는 데 대한 자세한 내용을 이해하게 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-189">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="b1818-190">고객이 Azure 예약에 대해 지불하는 가격</span><span class="sxs-lookup"><span data-stu-id="b1818-190">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="b1818-191">고객이 Azure 예약 사용을 최적화하는 방법</span><span class="sxs-lookup"><span data-stu-id="b1818-191">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="b1818-192">고객이 공유 범위의 예약을 구매하면 어떻게 되나요?</span><span class="sxs-lookup"><span data-stu-id="b1818-192">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="b1818-193">고객이 예약을 변경, 취소 및 갱신하거나 범위를 변경하려는 경우 어떻게 되나요?</span><span class="sxs-lookup"><span data-stu-id="b1818-193">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="b1818-194">**가격 고객은 예약 비용을 지불합니다.**</span><span class="sxs-lookup"><span data-stu-id="b1818-194">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="b1818-195">고객은 CSP 파트너 청구 계정에서 이전에 구매한 구독에 따라 Azure 예약을 구매하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-195">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="b1818-196">이 구독을 기반으로 구매한 Azure 예약에 대한 고객의 가격도 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-196">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="b1818-197">이 가격은 Azure Portal 고객이 보는 웹 직접 가격과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-197">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="b1818-198">**고객이 예약 사용을 최적화할 수 있는 방법입니다.**</span><span class="sxs-lookup"><span data-stu-id="b1818-198">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="b1818-199">일부 고객은 예약 사용을 최적화 하는 방법 또는 구매 중에 예약의 초기 범위를 할당 하는 방법에 대해 자세히 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-199">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="b1818-200">자세한 내용은 고객이 [Azure 리소스에 대 한 예약 관리](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)를 읽도록 요청 하세요.</span><span class="sxs-lookup"><span data-stu-id="b1818-200">For more information, ask customers to read [Manage reservations for Azure resources](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="b1818-201">**고객이 공유 범위를 사용 하 여 예약을 구매 하면 어떻게 되나요?**</span><span class="sxs-lookup"><span data-stu-id="b1818-201">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="b1818-202">고객이 이전 CSP 구독을 기반으로 하는 예약을 구매 하 고 해당 예약에 공유 범위를 할당 하는 경우 해당 고객에 게 제공 된 모든 구독에 대해 CSP가 제공 하는 모든 할인의 일치 사용에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-202">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="b1818-203">**고객이 수행한 구매를 교환, 취소 또는 갱신 하거나 예약의 초기 범위를 변경 하려는 경우에는 어떻게 해야 하나요?**</span><span class="sxs-lookup"><span data-stu-id="b1818-203">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="b1818-204">고객은 파트너에 게 예약의 초기 범위를 변경 하는 데 도움을 요청 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-204">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="b1818-205">또한 예약을 교환, 취소 또는 갱신 하기 위한 파트너의 도움이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-205">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="b1818-206">CSP 파트너가 구매한 구독에 기반 하 여 예약으로 이러한 작업을 수행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1818-206">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b1818-207">다음 단계</span><span class="sxs-lookup"><span data-stu-id="b1818-207">Next steps</span></span>

- [<span data-ttu-id="b1818-208">고객을 대신 하 여 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="b1818-208">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="b1818-209">파트너 센터-Microsoft 예약 판매</span><span class="sxs-lookup"><span data-stu-id="b1818-209">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="b1818-210">고객을 대신 하 여 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="b1818-210">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)