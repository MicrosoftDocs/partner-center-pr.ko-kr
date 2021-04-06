---
title: 고객이 CSP에서 자신의 서비스를 구입할 수 있도록 허용
description: CSP 프로그램 파트너가 파트너 센터에서 구매한 구독에 대해 Azure 예약과 같은 고유한 서비스를 구입할 수 있도록 하는 방법을 알아봅니다.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4feaa8cba8ba17f553b5e936dcf892ffbf7ccc82
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441305"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="75b77-103">파트너 센터에서 고객에 게 자신의 제품 또는 서비스를 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="75b77-103">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="75b77-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="75b77-104">**Appropriate roles**</span></span>

- <span data-ttu-id="75b77-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="75b77-105">Admin agent</span></span>
- <span data-ttu-id="75b77-106">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="75b77-106">Sales agent</span></span>

<span data-ttu-id="75b77-107">이 문서에서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너가 고객에 게 자신의 서비스 또는 리소스 중 일부를 구매할 수 있는 권한을 부여 하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-107">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="75b77-108">CSP 프로그램의 파트너는 파트너 센터와 상용 마켓플레이스를 사용 하 여 고객을 위한 솔루션 및 서비스를 구입 하는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-108">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="75b77-109">파트너는 일부 고객이 Azure Portal에서 직접 이러한 서비스를 프로 비전 할 수 있도록 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-109">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="75b77-110">예제는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-110">Here's an example.</span></span> <span data-ttu-id="75b77-111">파트너 센터에서 고객에 대 한 Azure 계획 구독을 구매 한다고 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-111">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="75b77-112">그런 다음 고객을 대신 하 여 해당 구독에 다른 리소스 또는 서비스를 추가 하기로 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-112">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="75b77-113">이 경우 고객의 구독 (예: 예약 된 가상 머신 인스턴스 추가)에 Azure 예약을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-113">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="75b77-114">그런 다음 고객이 Azure Portal에서 Azure 예약 리소스를 추가로 프로 비전 하도록 허용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-114">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="75b77-115">이제 **고객 권한** 기능을 사용 하 여 고객에 게 Azure 리소스를 통해 더 많은 셀프 서비스 옵션을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-115">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="75b77-116">고객에 대 한 권한을 설정 하 여 고객은 자신의 리소스 (예: 자신의 Azure 예약 구입)를 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-116">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="75b77-117">파트너 센터의 고객 권한 개요</span><span class="sxs-lookup"><span data-stu-id="75b77-117">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="75b77-118">고객 **계정** 페이지를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-118">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="75b77-119">현재이 기능은 다음을 지원 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-119">Currently, this feature supports:</span></span>

- <span data-ttu-id="75b77-120">**Azure 예약:** 이 권한을 설정 하면 고객이 구매한 특정 Azure 구독에 대해 자신의 Azure 예약을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-120">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="75b77-121">고객 권한을 설정 하기 전에 다음과 같은 중요 한 사항에 유의 하십시오.</span><span class="sxs-lookup"><span data-stu-id="75b77-121">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="75b77-122">기본적으로 고객 권한은 파트너 센터에서 자동으로 사용 하지 않도록 설정 (해제) 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-122">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="75b77-123">고객에 대 한 권한을 설정 하거나 해제 하려면 먼저 파트너 센터에서 관리 에이전트의 역할을 할당 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-123">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="75b77-124">판매 에이전트 또는 지원 센터 에이전트의 역할이 할당 된 파트너는 읽기 전용 액세스 권한을 가지 며 고객 권한을 설정 하거나 해제할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-124">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="75b77-125">선택한 모든 고객에 대 한 사용 권한을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-125">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="75b77-126">파트너 센터 대시보드 또는 [파트너 센터 api](/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-126">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="75b77-127">특정 고객에 대 한 사용 권한을 설정한 후에는 해당 고객의 이후 구매에 대 한 요금을 지불 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-127">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="75b77-128">고객이 만든 구매를 교환, 취소 또는 갱신 하려는 경우 (또는 예약의 초기 범위를 변경 하려는 경우) 스스로 스스로 작업을 수행할 수는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-128">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="75b77-129">파트너는 구매를 교환 하거나, 취소 하 고, 갱신 하거나, 예약의 범위를 나중에 변경 하는 데 도움을 요청 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-129">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="75b77-130">특정 고객에 대 한 사용 권한을 설정한 후에는 고객의 이후 구매에 대 한 알림이 표시 **되지** 않습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-130">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="75b77-131">고객의 나중에 구매한 제품은 사용자가 구입한 모든 구매와 함께 파트너 센터에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-131">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="75b77-132">고객의 **주문 기록** 페이지, 해당 **예약** 페이지 또는 [**활동 로그**](activity-logs.md)에서 이러한 구매를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-132">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="75b77-133">고객이 지불 하는 가격과 고객이 구매를 관리 하는 데 도움을 주는 방법에 대 한 자세한 내용은 [고객이 구매한 예약을 관리](give-customers-permission.md#help-customers-manage-reservations-they-purchase)하는 방법을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="75b77-133">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="75b77-134">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="75b77-134">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="75b77-135">Azure 예약은 할인된 요금으로 Azure 서비스를 구입할 수 있는 좋은 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-135">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="75b77-136">Azure 예약의 이점에 대 한 자세한 내용은 [Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="75b77-136">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="75b77-137">이제 이미 수행 했을 수 있으므로 고객을 대신 하 여 Azure 예약을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-137">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="75b77-138">또는 고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-138">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="75b77-139">사용자가 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하면 구매한 예약을 관리 하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-139">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="75b77-140">자세한 내용은 [고객이 구매한 예약 관리 지원](give-customers-permission.md#help-customers-manage-reservations-they-purchase)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="75b77-140">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="75b77-141">고객이 자신의 Azure 예약을 구매할 수 있도록 하려면</span><span class="sxs-lookup"><span data-stu-id="75b77-141">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="75b77-142">고객이 대신 구매한 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-142">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="75b77-143">이 구독에 대 한 **소유자** 역할이 사용자에 게 할당 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-143">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="75b77-144">고객 권한 (이 기능 **을** 설정)을 사용 하 여 자신의 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-144">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="75b77-145">각 단계가 아래에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-145">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="75b77-146">고객이 기존 Azure 구독을 보유 하 고 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="75b77-146">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="75b77-147">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하기 전에 고객이 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-147">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="75b77-148">고객이 파트너 센터에 현재 Azure 구독을 표시 하지 않는 경우 고객 권한을 설정 하기 전에 구독을 구입 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-148">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="75b77-149">고객이 이미 Azure 구독을 보유 하 고 있는지 확인 하려면 파트너 센터 대시보드에 로그인 한 다음 **CSP** 와 **고객** 을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-149">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="75b77-150">목록에서 특정 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-150">Select the specific customer from the list.</span></span> <span data-ttu-id="75b77-151">그런 다음 **구독** 을 선택 하 고 azure 요금제 또는 azure Global에 대 한 사용 빈도 기반 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-151">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="75b77-152">고객이 기존 Azure 구독을 보유 하 고 있지 않은 경우 해당 구독을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-152">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="75b77-153">[Azure 계획 구매를](purchase-azure-plan.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="75b77-153">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="75b77-154">Azure에서 고객이 올바른 역할을 할당 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-154">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="75b77-155">고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후에는 고객과 연결 된 키 사용자에 게 해당 Azure 구독에 대 한 올바른 **소유자** 역할이 할당 되었는지도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-155">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="75b77-156">사용자가 구매한 Azure 구독에 대해 Azure 예약을 구입 해야 하는 RBAC (역할 기반 액세스)입니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-156">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="75b77-157">일부 파트너는 자신의 Azure 리소스를 적극적으로 관리 하 고 프로 비전 하려는 고객에 게 **소유자** 역할을 이미 할당 했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-157">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="75b77-158">구매한 이전 구독을 관리 하기 위해 고객에 게 **소유자** 상태를 이미 할당 한 경우이 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-158">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="75b77-159">담당자에 게 **소유자** 역할이 할당 되지 않은 경우 Azure 예약을 구매 하지 못하도록 하는 Azure Portal 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-159">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="75b77-160">고객에 게 Azure 구독에 대 한 **소유자** 역할이 할당 되었는지 확인 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-160">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="75b77-161">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-161">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="75b77-162">**CSP**, **고객** 을 차례로 선택 하 고 특정 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-162">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="75b77-163">해당 고객에 대 한 **구독** 을 선택 하 고 특정 Azure 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-163">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="75b77-164">해당 고객의 구독 옆에 있는 **관리** 단추를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-164">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="75b77-165">이렇게 하면 [Azure Portal](https://portal.azure.com/)열립니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-165">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="75b77-166">특정 사용자에 게 **소유자** 역할을 할당 하려면 다음 단계에 따라 [사용자를 관리자로 할당](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-166">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="75b77-167">고객 권한을 설정 하거나 해제 하 여 자신의 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-167">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="75b77-168">고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후 사용자에 게 해당 구독에 대 한 **소유자** 역할이 할당 되 면 고객 권한을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-168">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="75b77-169">이러한 단계를 사용 하 여 고객 권한을 해제 (해제) 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-169">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="75b77-170">파트너 센터 대시보드 또는 [파트너 센터 api](/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-170">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="75b77-171">파트너 센터에서 고객 권한을 설정 하거나 해제 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-171">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="75b77-172">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-172">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="75b77-173">왼쪽 탐색 메뉴에서 **CSP**, **고객** 을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-173">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="75b77-174">고객 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-174">A customer list appears.</span></span>

3. <span data-ttu-id="75b77-175">특정 고객 이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-175">Select a specific customer name.</span></span>

4. <span data-ttu-id="75b77-176">고객 메뉴에서 **계정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-176">Select **Account** from the customer menu.</span></span> <span data-ttu-id="75b77-177">고객 **계정** 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-177">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="75b77-178">페이지 맨 아래에 있는 **고객 권한** 영역을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-178">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="계정 페이지에 대 한 고객 권한입니다." border="true":::

6. <span data-ttu-id="75b77-180">**Azure 예약** 에서 **고객이 구매할 수 있음** 옵션을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-180">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="75b77-181">고객 권한을 설정 하려면이 옵션 옆의 스위치를 **on** 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-181">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="75b77-182">고객 권한을 해제 하려면 스위치를 **off** 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-182">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="75b77-183">자신의 Azure 예약을 구매 하기 위해 고객의 권한을 설정할 때 발생 하는 다른 작업에 대해 알아보려면 [파트너 센터에서 고객 권한 개요](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="75b77-183">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="75b77-184">고객 권한을 설정 하거나 해제 하면 활동 로그에서 각 작업을 기록 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-184">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="75b77-185">파트너 센터 대시보드 위쪽에서 기어 아이콘을 선택 하면이 로그에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-185">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="75b77-186">고객 권한을 설정 하거나 해제 하는 경우 작업은 **고객 구매 권한 만들기** 또는 **고객 구매 권한 삭제** 를 활동 로그에 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-186">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="75b77-187">고객이 구매한 예약을 관리 하는 데 도움을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-187">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="75b77-188">사용자가 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하면 구매한 리소스를 보다 효율적으로 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-188">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="75b77-189">고객은 [Azure Portal](https://portal.azure.com/)에서 직접 Azure 예약의 여러 측면을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-189">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="75b77-190">CSP 구독 내에서 구매 하는 Azure 예약의 다른 몇 가지 측면을 관리 하는 데 도움이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-190">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="75b77-191">고객이 Azure 예약의 이러한 측면을 관리 하는 방법을 이해 하는 데 도움을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-191">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="75b77-192">고객이 Azure 예약에 대해 지불 하는 가격</span><span class="sxs-lookup"><span data-stu-id="75b77-192">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="75b77-193">고객이 Azure 예약 사용을 최적화 하는 방법</span><span class="sxs-lookup"><span data-stu-id="75b77-193">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="75b77-194">고객이 공유 범위를 사용 하 여 예약을 구매 하면 어떻게 되나요?</span><span class="sxs-lookup"><span data-stu-id="75b77-194">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="75b77-195">고객이 예약을 변경, 취소 및 갱신 하거나 범위를 변경 하려는 경우 어떻게 되나요?</span><span class="sxs-lookup"><span data-stu-id="75b77-195">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="75b77-196">**가격 고객은 예약에 대 한 비용을 지불 합니다.**</span><span class="sxs-lookup"><span data-stu-id="75b77-196">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="75b77-197">고객은 이전에 CSP 파트너 청구 계정에서 구매한 구독을 기준으로 Azure 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-197">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="75b77-198">이 구독을 기준으로 구매 하는 모든 Azure 예약에 대 한 고객의 가격은 사용자에 의해 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-198">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="75b77-199">이 가격은 Azure Portal 고객에 게 표시 되는 웹 직접 가격과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-199">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="75b77-200">**고객이 예약 사용을 최적화 하는 방법**</span><span class="sxs-lookup"><span data-stu-id="75b77-200">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="75b77-201">일부 고객은 예약 사용을 최적화 하는 방법 또는 구매 중에 예약의 초기 범위를 할당 하는 방법에 대해 자세히 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-201">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="75b77-202">자세한 내용은 고객이 [Azure 리소스에 대 한 예약 관리](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)를 읽도록 요청 하세요.</span><span class="sxs-lookup"><span data-stu-id="75b77-202">For more information, ask customers to read [Manage reservations for Azure resources](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="75b77-203">**고객이 공유 범위를 사용 하 여 예약을 구매 하면 어떻게 되나요?**</span><span class="sxs-lookup"><span data-stu-id="75b77-203">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="75b77-204">고객이 이전 CSP 구독을 기반으로 하는 예약을 구매 하 고 해당 예약에 공유 범위를 할당 하는 경우 해당 고객에 게 제공 된 모든 구독에 대해 CSP가 제공 하는 모든 할인의 일치 사용에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-204">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="75b77-205">**고객이 수행한 구매를 교환, 취소 또는 갱신 하거나 예약의 초기 범위를 변경 하려는 경우에는 어떻게 해야 하나요?**</span><span class="sxs-lookup"><span data-stu-id="75b77-205">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="75b77-206">고객은 파트너에 게 예약의 초기 범위를 변경 하는 데 도움을 요청 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-206">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="75b77-207">또한 예약을 교환, 취소 또는 갱신 하기 위한 파트너의 도움이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-207">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="75b77-208">CSP 파트너가 구매한 구독에 기반 하 여 예약으로 이러한 작업을 수행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="75b77-208">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="75b77-209">다음 단계</span><span class="sxs-lookup"><span data-stu-id="75b77-209">Next steps</span></span>

- [<span data-ttu-id="75b77-210">고객을 대신 하 여 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="75b77-210">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="75b77-211">파트너 센터-Microsoft 예약 판매</span><span class="sxs-lookup"><span data-stu-id="75b77-211">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="75b77-212">고객을 대신 하 여 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="75b77-212">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)