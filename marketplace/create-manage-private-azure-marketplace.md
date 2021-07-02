---
title: Azure Portal에서 개인 Azure Marketplace 만들기 및 관리
description: Azure Portal에서 개인 Azure Marketplace (미리 보기)를 만들고 관리 하는 방법에 대해 알아봅니다. 관리자는 개인 Azure Marketplace (미리 보기)를 사용 하 여 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173690"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="b0c58-104">Azure Portal에서 개인 Azure Marketplace 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="b0c58-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="b0c58-105">관리자는 개인 Azure Marketplace를 통해 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="b0c58-106">이를 위해 사용자는 관리자가 승인한 제품만 배포할 수 있으며 기업의 정책을 준수할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="b0c58-107">사용자는 개인 Azure Marketplace를 사용 하 여 온라인 스토어에서 구입 및 배포할 규격 제안을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="b0c58-108">Marketplace 관리자 (할당 된 역할)로 서 승인 된 제안 및 계획을 추가할 수 있는 사용 안 함 및 빈 개인 저장소로 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="b0c58-109">이 문서에서는 필요한 역할을 할당 하 고, 개인 저장소를 만들고, 항목을 관리 하 고, 사용자 요청을 승인 하 고, 사용자에 게 개인 Azure Marketplace를 사용 하도록 설정 하는 방법을 설명</span><span class="sxs-lookup"><span data-stu-id="b0c58-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="b0c58-110">개인 Azure Marketplace 테 넌 트 수준에 있으므로 테 넌 트의 모든 사용자에 게 동일한 큐 레이트 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="b0c58-111">모든 Microsoft 솔루션 ( [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)은 자동으로 개인 Azure Marketplace에 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="b0c58-112">Marketplace 관리자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="b0c58-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="b0c58-113">테 넌 트 전역 관리자는 개인 저장소를 관리 하는 개인 Azure Marketplace 관리자에 게 **Marketplace 관리자** 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="b0c58-114">개인 Azure Marketplace 관리에 대 한 액세스는 IT 관리자가 Marketplace 관리자 역할이 할당 된 경우에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="b0c58-115">필수 조건</span><span class="sxs-lookup"><span data-stu-id="b0c58-115">Prerequisites</span></span>

<span data-ttu-id="b0c58-116">이러한 필수 구성 요소는 사용자에 게 Marketplace 관리자 역할을 할당 하 여 테 넌 트 범위에서 사용자에 게 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="b0c58-117">**전역 관리자** 사용자에 대 한 액세스 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="b0c58-118">테 넌 트에 구독이 하나 이상 있습니다 (모든 형식일 수 있음).</span><span class="sxs-lookup"><span data-stu-id="b0c58-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="b0c58-119">전역 관리자 사용자에 게 선택한 구독에 대 한 **참가자** 역할 이상이 할당 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="b0c58-120">액세스 제어 (IAM)를 사용 하 여 Marketplace 관리자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="b0c58-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="b0c58-121">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="b0c58-122">**모든 서비스** 를 선택한 다음 **Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="b0c58-123">왼쪽의 메뉴에서 **비공개 Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Marketplace의 왼쪽에 있는 개인 marketplace 메뉴 옵션을 표시 합니다.":::

1. <span data-ttu-id="b0c58-125">**액세스 제어 (IAM)** 를 선택 하 여 Marketplace 관리자 역할을 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="I A M 액세스 제어 화면을 표시 합니다.":::

1. <span data-ttu-id="b0c58-127">**추가** > **역할 할당 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="b0c58-128">**역할** 아래에서 **Marketplace 관리자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="역할 할당 메뉴를 표시 합니다.":::

1. <span data-ttu-id="b0c58-130">드롭다운 목록에서 원하는 사용자를 선택한 다음 **완료** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="b0c58-131">PowerShell을 사용 하 여 Marketplace 관리자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="b0c58-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="b0c58-132">다음 PowerShell 스크립트를 사용 하 여 Marketplace 관리자 역할을 할당 합니다. 다음 매개 변수가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="b0c58-133">**TenantId:** 범위에 있는 테 넌 트의 ID입니다 (Marketplace 관리자 역할은 테 넌 트 범위에 할당 가능).</span><span class="sxs-lookup"><span data-stu-id="b0c58-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="b0c58-134">**SubscriptionId:** 전역 관리자에 게 **참여자** 역할이 할당 된 구독입니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="b0c58-135">**Globaladminusername:** 전역 관리자의 사용자 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="b0c58-136">**UsernameToAssignRoleFor:** Marketplace 관리자 역할이 할당 될 사용자 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="b0c58-137">테 넌 트에 초대 된 게스트 사용자의 경우 Marketplace 관리자 역할을 할당 하는 데 해당 계정을 사용할 수 있을 때까지 최대 48 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="b0c58-138">자세한 내용은 [Azure Active Directory B2B 공동 작업 사용자의 속성](/azure/active-directory/b2b/user-properties)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b0c58-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="b0c58-139">Az. portal PowerShell 모듈에 포함 된 cmdlet에 대 한 자세한 내용은 [Microsoft Azure PowerShell: 포털 대시보드 cmdlet](/powershell/module/az.portal/)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b0c58-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="b0c58-140">개인 Azure Marketplace 만들기</span><span class="sxs-lookup"><span data-stu-id="b0c58-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="b0c58-141">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="b0c58-142">**모든 서비스** 를 선택한 다음 **Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal 주 창을 표시 합니다.":::

3. <span data-ttu-id="b0c58-144">왼쪽의 메뉴에서 **비공개 Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="b0c58-145">**시작** 를 선택 하 여 개인 Azure Marketplace을 만듭니다 (한 번만 수행 하면 됩니다).</span><span class="sxs-lookup"><span data-stu-id="b0c58-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure Portal ' 주 창에서 ' 시작를 선택 하는 방법을 보여 줍니다.":::

    <span data-ttu-id="b0c58-147">이 테 넌 트에 대해 개인 Azure Marketplace 이미 있는 경우 **Marketplace 관리가** 기본적으로 선택 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="b0c58-148">완료 되 면 비어 있고 사용 하지 않도록 설정 된 개인 Azure Marketplace를 갖게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="빈 개인 Azure Marketplace 화면을 표시 합니다.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="b0c58-150">갤러리에서 항목 추가</span><span class="sxs-lookup"><span data-stu-id="b0c58-150">Add items from gallery</span></span>

<span data-ttu-id="b0c58-151">항목은 제품 및 계획의 조합입니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="b0c58-152">Marketplace 관리 페이지에서 항목을 검색 하 여 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="b0c58-153">**항목 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-153">Select **Add items**.</span></span>

2. <span data-ttu-id="b0c58-154">**갤러리** 를 찾아보거나 검색 필드를 사용 하 여 원하는 항목을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="갤러리를 찾아보거나 검색 필드를 사용 하는 방법을 보여 줍니다.":::

3. <span data-ttu-id="b0c58-156">기본적으로 새 제품을 추가할 때 모든 현재 계획이 승인 된 목록에 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="b0c58-157">선택한 항목을 추가 하기 전에 계획 선택을 수정 하려면 제품의 타일에서 드롭다운 메뉴를 선택 하 고 필요한 계획을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="필요한 계획을 업데이트 하는 방법을 보여 줍니다.":::

4. <span data-ttu-id="b0c58-159">선택한 후 왼쪽 아래에서 **완료** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="b0c58-160">Marketplace에 **항목 추가** 는 타사 제품에 대해서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="b0c58-161">Microsoft 솔루션 ( [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)은 "기본적으로 승인 됨"으로 태그가 지정 되 고 개인 Marketplace에서 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="b0c58-162">항목의 계획 편집</span><span class="sxs-lookup"><span data-stu-id="b0c58-162">Edit item's plans</span></span>

<span data-ttu-id="b0c58-163">Marketplace 관리 페이지에서 항목의 계획을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="b0c58-164">**계획** 열의 해당 항목에 대 한 드롭다운 메뉴에서 사용 가능한 계획을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="b0c58-165">확인란을 선택 하거나 선택을 취소 하 여 사용자가 사용할 수 있도록 설정할 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="필요한 항목에 대 한 확인란을 선택 하거나 선택 취소 하는 방법을 보여 줍니다.":::

   > [!NOTE]
   > <span data-ttu-id="b0c58-167">각 제품에는 업데이트를 수행 하기 위해 하나 이상의 계획을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="b0c58-168">제품 관련 요금제를 모두 제거 하려면 전체 제품을 삭제 합니다 (다음 섹션 참조).</span><span class="sxs-lookup"><span data-stu-id="b0c58-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="b0c58-169">제안 삭제</span><span class="sxs-lookup"><span data-stu-id="b0c58-169">Delete offers</span></span>

<span data-ttu-id="b0c58-170">Marketplace 관리 페이지에서 제품 이름 옆의 확인란을 선택 하 고 (위 화면 참조) **항목 삭제** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="b0c58-171">개인 Azure Marketplace 사용/사용 안 함</span><span class="sxs-lookup"><span data-stu-id="b0c58-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="b0c58-172">Marketplace 관리 페이지에 다음 배너 중 하나가 표시 됩니다 .이 배너에는 개인 Azure Marketplace의 현재 상태가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="' 상태 비활성화 ' 배너를 표시 합니다.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="' 상태 사용 ' 배너를 표시 합니다.":::

<span data-ttu-id="b0c58-175">필요에 따라 개인 Azure Marketplace를 사용 하거나 사용 하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="b0c58-176">사용 하지 않도록 설정 된 경우 **개인 Marketplace** 사용을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="b0c58-177">사용 하도록 설정 된 경우 **개인 Marketplace** 사용 안 함을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="b0c58-178">개인 Azure Marketplace 알림 센터</span><span class="sxs-lookup"><span data-stu-id="b0c58-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="b0c58-179">알림 센터는 세 가지 유형의 알림으로 구성 되며 Marketplace 관리자는 알림을 기반으로 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="b0c58-180">승인 된 목록에 없는 항목에 대 한 사용자의 승인 요청 (아래에 [제안 또는 요금제 추가 요청](#request-to-add-offers-or-plans) )을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="b0c58-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="b0c58-181">승인 된 목록에 하나 이상의 계획이 이미 있는 제안에 대 한 새 계획 알림</span><span class="sxs-lookup"><span data-stu-id="b0c58-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="b0c58-182">승인 된 목록에 있지만 전역 Azure Marketplace에서 제거 된 항목에 대 한 계획 알림이 제거 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="b0c58-183">알림 센터에 액세스 하려면:</span><span class="sxs-lookup"><span data-stu-id="b0c58-183">To access the notification center:</span></span>

1. <span data-ttu-id="b0c58-184">왼쪽 메뉴에서 **알림** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="알림 메뉴를 표시 합니다.":::

1. <span data-ttu-id="b0c58-186">추가 작업에 대 한 줄임표 메뉴를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="추가 옵션 메뉴 결과를 표시 합니다.":::

1. <span data-ttu-id="b0c58-188">계획 요청에서 **요청 표시** 는 특정 제품에 대 한 모든 사용자 요청을 검토할 수 있는 승인 요청 양식을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="b0c58-189">**승인** 또는 **거부** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="승인 및 거부 옵션을 표시 합니다.":::

1. <span data-ttu-id="b0c58-191">드롭다운 메뉴에서 승인할 계획을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="b0c58-192">의견을 추가 하 고 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="b0c58-193">비공개 Azure Marketplace 찾아보기</span><span class="sxs-lookup"><span data-stu-id="b0c58-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="b0c58-194">개인 Azure Marketplace를 사용 하는 경우 Marketplace 관리자가 승인한 요금제를 사용자에 게 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="b0c58-195">녹색 **승인** 된 알림은 승인 된 파트너 (타사) 제품을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="b0c58-196">파란색 **승인** 된 알림은 승인 된 Microsoft 제품 ( [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="b0c58-197">사용자는 승인 되지 않은 제품을 필터링 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="필터링 옵션을 보여 줍니다.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="b0c58-199">개인 Azure Marketplace에서 구입 또는 배포</span><span class="sxs-lookup"><span data-stu-id="b0c58-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="b0c58-200">제품 세부 정보 페이지 환경은 글로벌 Azure Marketplace와 유사 하지만 세 가지 전용 Azure Marketplace 특정 시나리오를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="b0c58-201">사용자가 승인된 계획을 선택하면 **만들기** 단추가 사용하도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="계획을 만들 수 있다는 것을 표시하는 제안 배너를 표시합니다.":::

- <span data-ttu-id="b0c58-203">제품 계획 선택 항목이 제품 세부 정보 페이지에 표시되지 않지만 관리자가 하나 이상의 계획을 승인한 경우 승인된 계획이 표시되고 **만들기** 단추가 사용하도록 설정되는 배너가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="계획을 만들 수 있음을 나타내고 사용 가능한 계획을 표시하는 제안 배너를 표시합니다.":::

- <span data-ttu-id="b0c58-205">사용자가 승인되지 않은 계획을 선택하면 계획이 승인되지 않은 것으로 배너가 표시되고 **만들기** 단추가 비활성화됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="b0c58-206">사용자는 승인된 목록에 계획을 추가하도록 요청할 수 있습니다(다음 섹션 참조).</span><span class="sxs-lookup"><span data-stu-id="b0c58-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="b0c58-207">제안 또는 플랜 추가 요청</span><span class="sxs-lookup"><span data-stu-id="b0c58-207">Request to add offers or plans</span></span>

<span data-ttu-id="b0c58-208">프라이빗 Azure Marketplace 현재 승인되지 않은 공개 제안 또는 플랜을 추가하도록 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="b0c58-209">**배너에 추가할 요청을** 선택하여 **액세스 요청 양식을** 엽니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="'추가 요청' 링크가 있는 배너를 표시합니다.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="제안 또는 플랜에 대한 액세스 요청 양식을 표시합니다.":::

1. <span data-ttu-id="b0c58-212">요청에 추가할 플랜을 **선택합니다(모든 플랜은** Marketplace 관리자에게 제안 내 플랜에 대한 기본 설정이 없다는 것을 알려 줍니다).</span><span class="sxs-lookup"><span data-stu-id="b0c58-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="b0c58-213">**Justification을** 추가하고 **요청을** 선택하여 요청을 제출합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="샘플 항목이 있는 제안 또는 플랜에 대한 액세스 요청 양식을 표시합니다.":::

1. <span data-ttu-id="b0c58-215">보류 중인 요청에 대한 표시는 요청 철회 옵션이 있는 액세스 **요청** 양식에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="승인 요청 링크가 있는 승인되거나 보류 중인 계획 목록을 표시합니다.":::

> [!NOTE]
> <span data-ttu-id="b0c58-217">제출되면 Marketplace 관리자가 요청을 검토하고 조치를 취할 수 있도록 승인 요청 양식이 [알림 센터로](#private-azure-marketplace-notification-center) 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="b0c58-218">프라이빗 마켓플레이스에 대한 승인은 솔루션 조달을 나타내지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="b0c58-219">FAQ(질문과 대답)</span><span class="sxs-lookup"><span data-stu-id="b0c58-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="b0c58-220">Azure Policy 통해 Marketplace 타사 애플리케이션을 이미 차단하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="b0c58-221">어떻게 다른가요?</span><span class="sxs-lookup"><span data-stu-id="b0c58-221">How is this different?</span></span>

<span data-ttu-id="b0c58-222">현재 Marketplace에서 타사 서비스를 제한하는 방법에는 두 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="b0c58-223">EA 포털 또는 Azure Portal 통해 타사 서비스를 사용하지 않도록 설정하거나 "무료 또는 BYOL S SKU만"으로 제한합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Azure Portal 서비스를 제한하는 방법을 보여줍니다.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E A 포털에서 서비스를 제한하는 방법을 보여줍니다.":::

2. <span data-ttu-id="b0c58-226">특정 VM만 허용하는 Azure 정책을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="b0c58-227">Windows VM에 정책을 적용하는 방법에 대한 자세한 내용은 Azure Resource Manager 사용하여 [Windows VM에 정책 적용을](/azure/virtual-machines/windows/policy)참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b0c58-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="b0c58-228">프라이빗 Azure Marketplace 사용하면 특정 제안 및 플랜을 제한하고 허용하는 데 더 많은 유연성을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="b0c58-229">타사 서비스 배포를 시도하기 전에도 마켓플레이스 갤러리에서 배포할 수 있는 가용성을 최종 사용자에게 알릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="b0c58-230">타사 서비스의 배포를 허용하려면 EA Portal Azure Marketplace 설정/사용으로 설정하고 Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b0c58-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="b0c58-231">프라이빗 Azure Marketplace 가상 머신으로 제한되지 않는 파트너 솔루션을 큐레이팅할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="b0c58-232">프라이빗 Azure Marketplace 계획 수준에서 큐레이팅할 수 있으며 "현재 및 향후 계획"을 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="b0c58-233">프라이빗 Azure Marketplace 최종 사용자에게 배포할 수 있는 항목과 배포할 수 없는 항목에 대해 미리 알릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="b0c58-234">프라이빗 제안과 프라이빗 Azure Marketplace 차이점은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="b0c58-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="b0c58-235">**프라이빗 제안을** 통해 게시자는 대상 고객에게만 표시되는 플랜을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="b0c58-236">이를 통해 협상된 가격 책정, 프라이빗 사용 약관 및 특수 구성과 사용자 지정된 솔루션을 비공개로 공유할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="b0c58-237">자세한 내용은 [상업용 마켓플레이스의 프라이빗 제안을 참조하세요.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="b0c58-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="b0c58-238">**Azure Portal 프라이빗 Azure Marketplace** 통해 관리자는 사용자가 배포할 수 있는 타사 솔루션을 미리 승인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="b0c58-239">프라이빗 Azure Marketplace 통해 사용자는 규격 제품을 찾고, 구매하고, 배포하여 Azure Marketplace 이점을 누릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="b0c58-240">Private Marketplace에서 구독 기반 프라이빗 제안을 관리하려면 Marketplace 관리자에게 특정 구독에 대한 최소 "읽기" 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="b0c58-241">프라이빗 Azure Marketplace 프라이빗 제안을 추가했습니다. 마켓플레이스 관리 탭에 표시되지 않는 이유는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="b0c58-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="b0c58-242">구독 기반 프라이빗 제안은 프라이빗 제품 설정에 나열된 구독에 대해서만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="b0c58-243">프라이빗 제안을 보려면 전역 구독 필터에 모든 구독이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="프라이빗 마켓플레이스 필터를 표시합니다.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="b0c58-245">프라이빗 Azure Marketplace 사용자 지정 이미지를 포함할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="b0c58-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="b0c58-246">아니요.</span><span class="sxs-lookup"><span data-stu-id="b0c58-246">No.</span></span> <span data-ttu-id="b0c58-247">프라이빗 Azure Marketplace 사용하면 IT 관리자가 글로벌 Azure Marketplace 타사 솔루션을 관리하고 큐레이팅할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="b0c58-248">사용자 지정 이미지는 글로벌 Azure Marketplace 없으므로 IT 관리자는 사용자 지정 이미지를 선택하고 선택할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="b0c58-249">사용자 지정 이미지를 공유하려면 [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries)사용합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="b0c58-250">단계별 가이드 SIG(Shared Image Gallery 만들기) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="b0c58-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="b0c58-251">SIG 내에 이미지 정의를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="b0c58-252">고객은 OS 상태 필드에 대해 **일반화를** 선택해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="b0c58-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="b0c58-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="b0c58-254">관리되는 이미지를 Shared Image Gallery[가져옵니다(CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="b0c58-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="b0c58-255">SIG VM 이미지는 하나의 구독에 상주합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="b0c58-256">다른 구독에서 사용할 수 있도록 하려면 앱[등록(CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell)을](/azure/virtual-machines/windows/share-images-across-tenants)사용합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="b0c58-257">게시자가 Microsoft가 아니더라도 **기본적으로 승인된** 일부 제안이 표시되는 이유는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="b0c58-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="b0c58-258">Microsoft는 Azure에서 Linux 및 오픈 소스 기술을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="b0c58-259">[보증 Linux 배포판은](/azure/virtual-machines/linux/endorsed-distros) Azure에서 지원되며 가격은 가상 머신에 통합됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="b0c58-260">Azure Linux 에이전트는 이미 Azure Marketplace 사전 설치되어 있으므로 Microsoft 제안처럼 처리됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="b0c58-261">Microsoft 제안은 기본적으로 승인되므로 프라이빗 Azure Marketplace 보증 Linux 배포판은 관리될 수 없으며 기본적으로 승인됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="b0c58-262">지원에 문의</span><span class="sxs-lookup"><span data-stu-id="b0c58-262">Contact support</span></span>

- <span data-ttu-id="b0c58-263">Azure Marketplace 지원은 [Microsoft Q&A를](/answers/products/)방문합니다.</span><span class="sxs-lookup"><span data-stu-id="b0c58-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>