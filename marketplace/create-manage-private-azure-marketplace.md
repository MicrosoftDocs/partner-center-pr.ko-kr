---
title: Azure Portal에서 개인 Azure Marketplace 만들기 및 관리
description: Azure Portal에서 개인 Azure Marketplace (미리 보기)를 만들고 관리 하는 방법에 대해 알아봅니다.
ms.prod: marketplace-customer
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: 31179d9fd4068348e689d8b426b7a0307112501a
ms.sourcegitcommit: af4726de429d2b9b7c3656d5cac7d542b0d4af74
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2020
ms.locfileid: "93414861"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="d4481-103">Azure Portal에서 개인 Azure Marketplace (미리 보기)를 만들고 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="d4481-104">관리자는 개인 Azure Marketplace (미리 보기)를 사용 하 여 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="d4481-105">이를 위해 승인 하 고 기업의 정책을 준수 하는 제공만 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="d4481-106">개인 Azure Marketplace를 사용 하 여 사용자는 온라인 스토어에서 구입 및 배포할 규격 제안을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="d4481-107">Marketplace 관리자 (할당 된 역할)로 서 승인 된 제안 및 계획을 추가할 수 있는 사용 안 함 및 빈 개인 저장소로 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="d4481-108">이 문서에서는 사용자에 대해 개인 Azure Marketplace를 만들고, 관리 하 고, 사용 하도록 설정 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="d4481-109">참고:</span><span class="sxs-lookup"><span data-stu-id="d4481-109">Notes:</span></span>

- <span data-ttu-id="d4481-110">개인 Azure Marketplace 테 넌 트 수준에 있으므로 테 넌 트의 모든 사용자에 게 동일한 큐 레이트 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="d4481-111">모든 Microsoft 솔루션은 개인 Azure Marketplace에 자동으로 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="d4481-112">Marketplace 관리자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="d4481-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="d4481-113">테 넌 트 전역 관리자는 개인 저장소를 관리 하는 개인 Azure Marketplace 관리자에 게 **Marketplace 관리자** 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d4481-114">개인 Azure Marketplace 관리에 대 한 액세스는 IT 관리자가 Marketplace 관리자 역할이 할당 된 경우에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="d4481-115">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="d4481-115">Prerequisites</span></span>

<span data-ttu-id="d4481-116">이러한 필수 구성 요소를 충족 해야 테 넌 트 범위에서 사용자에 게 Marketplace 관리자 역할을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="d4481-117">**전역 관리자** 사용자에 대 한 액세스 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="d4481-118">테 넌 트에 구독이 하나 이상 있습니다 (모든 형식일 수 있음).</span><span class="sxs-lookup"><span data-stu-id="d4481-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="d4481-119">전역 관리자 사용자에 게 2 단계에서 선택한 구독에 대 한 **참가자** 역할 이상이 할당 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="d4481-120">전역 관리자의 액세스 권한이 **예** ( [상승-액세스-전역-관리자](/azure/role-based-access-control/elevate-access-global-admin))로 설정 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="d4481-121">PowerShell을 사용 하 여 Marketplace 관리자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="d4481-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="d4481-122">다음 PowerShell 스크립트를 사용 하 여 Marketplace 관리자 역할을 할당 합니다. 다음 매개 변수가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="d4481-123">**TenantId:** 범위에 있는 테 넌 트의 ID입니다 (Marketplace 관리자 역할은 테 넌 트 범위에 할당 가능).</span><span class="sxs-lookup"><span data-stu-id="d4481-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="d4481-124">**SubscriptionId:** 전역 관리자에 게 **참여자** 역할이 할당 된 구독입니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="d4481-125">**Globaladminusername:** 전역 관리자의 사용자 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="d4481-126">**UsernameToAssignRoleFor:** Marketplace 관리자 역할이 할당 될 사용자 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="d4481-127">테 넌 트에 초대 된 게스트 사용자의 경우 Marketplace 관리자 역할을 할당 하는 데 해당 계정을 사용할 수 있을 때까지 최대 48 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="d4481-128">자세한 내용은 [AZURE ACTIVE DIRECTORY B2B 공동 작업 사용자의 속성](/azure/active-directory/b2b/user-properties)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="d4481-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole {
[CmdletBinding()]
param(
[Parameter(Mandatory)]
[string]$TenantId,

[Parameter(Mandatory)]
[string]$SubscriptionId,

[Parameter(Mandatory)]
[string]$GlobalAdminUsername,

[Parameter(Mandatory)]
[string]$UsernameToAssignRoleFor
)

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin"

Write-Output "TenantId = $TenantId"
Write-Output "SubscriptionId = $SubscriptionId"
Write-Output "GlobalAdminUsername = $GlobalAdminUsername"
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor"

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)"

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

if($profile -eq $null)
{
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop
}
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername)
{
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)"
}
else
{
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)"
}

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="d4481-129">Az. Portal PowerShell 모듈에 포함 된 cmdlet에 대 한 자세한 내용은 [Microsoft Azure PowerShell: 포털 대시보드 cmdlet](/powershell/module/az.portal/)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="d4481-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="d4481-130">개인 Azure Marketplace 만들기</span><span class="sxs-lookup"><span data-stu-id="d4481-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="d4481-131">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="d4481-132">**모든 서비스** 를 선택한 다음 **Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="주 창을 Azure Portal 합니다.":::

3. <span data-ttu-id="d4481-134">왼쪽의 옵션에서 **비공개 Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Azure Portal 주 창에서 비공개 Marketplace를 선택 합니다.":::

4. <span data-ttu-id="d4481-136">**시작** 을 선택 하 여 개인 Azure Marketplace 만들기를 선택 합니다 .이 작업은 한 번만 수행 하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure Portal 주 창에서 시작을 선택 합니다.":::

    <span data-ttu-id="d4481-138">이 테 넌 트에 대해 개인 Azure Marketplace 이미 있는 경우 **Marketplace 관리가** 기본적으로 선택 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="d4481-139">완료 되 면 비어 있고 사용 하지 않도록 설정 된 개인 Azure Marketplace를 갖게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="빈 개인 Azure Marketplace 화면입니다.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="d4481-141">갤러리에서 항목 추가</span><span class="sxs-lookup"><span data-stu-id="d4481-141">Add items from gallery</span></span>

<span data-ttu-id="d4481-142">항목은 제품 및 계획의 조합입니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="d4481-143">Marketplace 관리 페이지에서 항목을 검색 하 여 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="d4481-144">**항목 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-144">Select **Add items**.</span></span>

2. <span data-ttu-id="d4481-145">**갤러리** 를 찾아보거나 검색 필드를 사용 하 여 원하는 항목을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="갤러리를 찾아보거나 검색 필드를 사용 합니다.":::

3. <span data-ttu-id="d4481-147">기본적으로 새 제품을 추가할 때 모든 현재 계획이 허용 목록에 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="d4481-148">선택한 항목을 추가 하기 전에 계획 선택을 수정 하려면 제품의 타일에서 드롭다운 메뉴를 선택 하 고 필요한 계획을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="필수 계획을 업데이트 합니다.":::

4. <span data-ttu-id="d4481-150">선택한 후 왼쪽 아래에서 **완료** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="d4481-151">Marketplace에 **항목 추가** 는 타사 제품에 대해서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="d4481-152">Microsoft 제품은 기본적으로 허용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="d4481-153">항목 계획 편집</span><span class="sxs-lookup"><span data-stu-id="d4481-153">Edit item plans</span></span>

<span data-ttu-id="d4481-154">Marketplace 관리 페이지에서 항목의 계획을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="d4481-155">**계획** 열의 해당 항목에 대 한 드롭다운 메뉴에서 사용 가능한 계획을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="d4481-156">확인란을 선택 하거나 선택을 취소 하 여 사용자가 사용할 수 있도록 설정할 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="필요한 항목에 대 한 확인란을 선택 하거나 선택 취소 합니다.":::

> [!NOTE]
> <span data-ttu-id="d4481-158">업데이트를 수행 하려면 각 제품에 하나 이상의 계획이 선택 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="d4481-159">제품 관련 요금제를 모두 제거 하려면 전체 제품을 삭제 합니다 (다음 섹션 참조).</span><span class="sxs-lookup"><span data-stu-id="d4481-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="d4481-160">제안 삭제</span><span class="sxs-lookup"><span data-stu-id="d4481-160">Delete offers</span></span>

<span data-ttu-id="d4481-161">Marketplace 관리 페이지에서 제품 이름 옆의 확인란을 선택 하 고 (위 화면 참조) **항목 삭제** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="d4481-162">개인 Azure Marketplace 사용/사용 안 함</span><span class="sxs-lookup"><span data-stu-id="d4481-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="d4481-163">Marketplace 관리 페이지에 다음 배너 중 하나가 표시 됩니다 .이 배너에는 개인 Azure Marketplace의 현재 상태가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="상태 배너 사용 안 함":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="상태 배너 사용":::

<span data-ttu-id="d4481-166">필요에 따라 개인 Azure Marketplace를 사용 하거나 사용 하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="d4481-167">사용 하지 않도록 설정 된 경우 **개인 Marketplace** 사용을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="d4481-168">사용 하도록 설정 된 경우 **개인 Marketplace** 사용 안 함을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="d4481-169">비공개 Azure Marketplace 찾아보기</span><span class="sxs-lookup"><span data-stu-id="d4481-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="d4481-170">개인 Azure Marketplace를 사용 하는 경우 Marketplace 관리자가 허용 하는 요금제를 사용자에 게 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="d4481-171">녹색 **허용** 통지는 허용 되는 파트너 (타사) 제품을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="d4481-172">파란색 **허용** 된 알림은 허용 된 Microsoft 제품을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="d4481-173">사용자는 허용 되지 않는 제품을 필터링 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="필터링 옵션입니다.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="d4481-175">개인 Azure Marketplace에서 구입 또는 배포</span><span class="sxs-lookup"><span data-stu-id="d4481-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="d4481-176">제품 세부 정보 페이지 환경은 공용 Azure Marketplace와 유사 하지만 세 가지 전용 Azure Marketplace 특정 시나리오를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="d4481-177">사용자가 허용 된 계획을 선택 하면 **만들기** 단추가 활성화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="계획을 만들 수 있는 제품 배너입니다.":::

- <span data-ttu-id="d4481-179">사용자가 허용 되지 않는 계획을 선택 하는 경우 해당 계획은 허용 되지 않으며 **만들기** 단추를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="계획을 만들 수 없는 배너를 제공 합니다.":::

- <span data-ttu-id="d4481-181">제품 계획 선택이 제품 정보 페이지에 표시 되지 않지만 관리자가 하나 이상의 계획을 승인한 경우 배너에는 허용 되는 계획과 **만들기** 단추가 활성화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4481-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="계획을 만들고 사용 가능한 계획을 표시할 수 있는 제품 배너입니다.":::

## <a name="contact-support"></a><span data-ttu-id="d4481-183">기술 지원 서비스에 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="d4481-183">Contact support</span></span>

<span data-ttu-id="d4481-184">Azure Marketplace 지원이 필요한 경우 [Microsoft Q&A](/answers/products/)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="d4481-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
