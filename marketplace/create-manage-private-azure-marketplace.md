---
title: Azure Portal에서 개인 Azure Marketplace 만들기 및 관리
description: Azure Portal에서 개인 Azure Marketplace (미리 보기)를 만들고 관리 하는 방법에 대해 알아봅니다. 관리자는 개인 Azure Marketplace (미리 보기)를 사용 하 여 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760829"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Azure Portal에서 개인 Azure Marketplace (미리 보기)를 만들고 관리 합니다.

관리자는 개인 Azure Marketplace (미리 보기)를 사용 하 여 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다. 이를 위해 승인 하 고 기업의 정책을 준수 하는 제공만 배포할 수 있습니다. 개인 Azure Marketplace를 사용 하 여 사용자는 온라인 스토어에서 구입 및 배포할 규격 제안을 검색할 수 있습니다. 

Marketplace 관리자 (할당 된 역할)로 서 승인 된 제안 및 계획을 추가할 수 있는 사용 안 함 및 빈 개인 저장소로 시작 합니다. 이 문서에서는 사용자에 대해 개인 Azure Marketplace를 만들고, 관리 하 고, 사용 하도록 설정 하는 방법을 설명 합니다.

참고:

- 개인 Azure Marketplace 테 넌 트 수준에 있으므로 테 넌 트의 모든 사용자에 게 동일한 큐 레이트 목록이 표시 됩니다.
- 모든 Microsoft 솔루션은 개인 Azure Marketplace에 자동으로 추가 됩니다.

## <a name="assign-the-marketplace-admin-role"></a>Marketplace 관리자 역할 할당

테 넌 트 전역 관리자는 개인 저장소를 관리 하는 개인 Azure Marketplace 관리자에 게 **Marketplace 관리자** 역할을 할당 해야 합니다.

>[!IMPORTANT]
> 개인 Azure Marketplace 관리에 대 한 액세스는 IT 관리자가 Marketplace 관리자 역할이 할당 된 경우에만 사용할 수 있습니다.

### <a name="prerequisites"></a>필수 조건

이러한 필수 구성 요소를 충족 해야 테 넌 트 범위에서 사용자에 게 Marketplace 관리자 역할을 할당할 수 있습니다.

- **전역 관리자** 사용자에 대 한 액세스 권한이 있습니다.
- 테 넌 트에 구독이 하나 이상 있습니다 (모든 형식일 수 있음).
- 전역 관리자 사용자에 게 선택한 구독에 대 한 **참가자** 역할 이상이 할당 됩니다.

### <a name="assign-the-marketplace-admin-role-with-iam"></a>IAM을 사용 하 여 Marketplace 관리자 역할 할당

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.
1. **모든 서비스** 를 선택한 다음 **Marketplace** 를 선택 합니다.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="주 창을 Azure Portal 합니다.":::

3. 왼쪽의 옵션에서 **비공개 Marketplace** 를 선택 합니다.
1. **액세스 제어 (IAM)** 를 선택 하 여 Marketplace 관리자 역할을 할당 합니다.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="IAM 액세스 제어 화면":::

1. **추가** > **역할 할당 추가** 를 선택합니다.
1. **역할** 아래에서 **Marketplace 관리자** 를 선택 합니다.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="역할 할당 메뉴.":::

1. 드롭다운 목록에서 원하는 사용자를 선택한 다음 **완료** 를 선택 합니다.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>PowerShell을 사용 하 여 Marketplace 관리자 역할 할당

다음 PowerShell 스크립트를 사용 하 여 Marketplace 관리자 역할을 할당 합니다. 다음 매개 변수가 필요 합니다.

- **TenantId:** 범위에 있는 테 넌 트의 ID입니다 (Marketplace 관리자 역할은 테 넌 트 범위에 할당 가능).
- **SubscriptionId:** 전역 관리자에 게 **참여자** 역할이 할당 된 구독입니다.
- **Globaladminusername:** 전역 관리자의 사용자 이름입니다.
- **UsernameToAssignRoleFor:** Marketplace 관리자 역할이 할당 될 사용자 이름입니다.

> [!NOTE]
> 테 넌 트에 초대 된 게스트 사용자의 경우 Marketplace 관리자 역할을 할당 하는 데 해당 계정을 사용할 수 있을 때까지 최대 48 시간이 걸릴 수 있습니다. 자세한 내용은 [AZURE ACTIVE DIRECTORY B2B 공동 작업 사용자의 속성](/azure/active-directory/b2b/user-properties)을 참조 하세요.

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

Az. Portal PowerShell 모듈에 포함 된 cmdlet에 대 한 자세한 내용은 [Microsoft Azure PowerShell: 포털 대시보드 cmdlet](/powershell/module/az.portal/)을 참조 하세요.

## <a name="create-private-azure-marketplace"></a>개인 Azure Marketplace 만들기

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.
2. **모든 서비스** 를 선택한 다음 **Marketplace** 를 선택 합니다.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="주 창을 Azure Portal 합니다.":::

3. 왼쪽의 옵션에서 **비공개 Marketplace** 를 선택 합니다.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Azure Portal 주 창에서 비공개 Marketplace를 선택 합니다.":::

4. **시작** 을 선택 하 여 개인 Azure Marketplace 만들기를 선택 합니다 .이 작업은 한 번만 수행 하면 됩니다.

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure Portal 주 창에서 시작을 선택 합니다.":::

    이 테 넌 트에 대해 개인 Azure Marketplace 이미 있는 경우 **Marketplace 관리가** 기본적으로 선택 됩니다.

5. 완료 되 면 비어 있고 사용 하지 않도록 설정 된 개인 Azure Marketplace를 갖게 됩니다.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="빈 개인 Azure Marketplace 화면입니다.":::

## <a name="add-items-from-gallery"></a>갤러리에서 항목 추가

항목은 제품 및 계획의 조합입니다. Marketplace 관리 페이지에서 항목을 검색 하 여 추가할 수 있습니다.

1. **항목 추가** 를 선택 합니다.

2. **갤러리** 를 찾아보거나 검색 필드를 사용 하 여 원하는 항목을 찾습니다.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="갤러리를 찾아보거나 검색 필드를 사용 합니다.":::

3. 기본적으로 새 제품을 추가할 때 모든 현재 계획이 허용 목록에 추가 됩니다. 선택한 항목을 추가 하기 전에 계획 선택을 수정 하려면 제품의 타일에서 드롭다운 메뉴를 선택 하 고 필요한 계획을 업데이트 합니다.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="필수 계획을 업데이트 합니다.":::

4. 선택한 후 왼쪽 아래에서 **완료** 를 선택 합니다.

>[!Note]
> Marketplace에 **항목 추가** 는 타사 제품에 대해서만 사용할 수 있습니다. Microsoft 제품은 기본적으로 허용 됩니다.

## <a name="edit-item-plans"></a>항목 계획 편집

Marketplace 관리 페이지에서 항목의 계획을 편집할 수 있습니다.

1. **계획** 열의 해당 항목에 대 한 드롭다운 메뉴에서 사용 가능한 계획을 검토 합니다.
2. 확인란을 선택 하거나 선택을 취소 하 여 사용자가 사용할 수 있도록 설정할 계획을 선택 합니다.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="필요한 항목에 대 한 확인란을 선택 하거나 선택 취소 합니다.":::

> [!NOTE]
> 업데이트를 수행 하려면 각 제품에 하나 이상의 계획이 선택 되어 있어야 합니다. 제품 관련 요금제를 모두 제거 하려면 전체 제품을 삭제 합니다 (다음 섹션 참조).

## <a name="delete-offers"></a>제안 삭제

Marketplace 관리 페이지에서 제품 이름 옆의 확인란을 선택 하 고 (위 화면 참조) **항목 삭제** 를 선택 합니다.

## <a name="enabledisable-private-azure-marketplace"></a>개인 Azure Marketplace 사용/사용 안 함

Marketplace 관리 페이지에 다음 배너 중 하나가 표시 됩니다 .이 배너에는 개인 Azure Marketplace의 현재 상태가 표시 됩니다.

:::image type="content" source="media/private-azure/state-disable.png" alt-text="상태 배너 사용 안 함":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="상태 배너 사용":::

필요에 따라 개인 Azure Marketplace를 사용 하거나 사용 하지 않도록 설정할 수 있습니다.

- 사용 하지 않도록 설정 된 경우 **개인 Marketplace** 사용을 선택 합니다.
- 사용 하도록 설정 된 경우 **개인 Marketplace** 사용 안 함을 선택 합니다.

## <a name="browsing-private-azure-marketplace"></a>비공개 Azure Marketplace 찾아보기

개인 Azure Marketplace를 사용 하는 경우 Marketplace 관리자가 허용 하는 요금제를 사용자에 게 표시 합니다.

- 녹색 **허용** 통지는 허용 되는 파트너 (타사) 제품을 나타냅니다.
- 파란색 **허용** 된 알림은 허용 된 Microsoft 제품을 나타냅니다.

사용자는 허용 되지 않는 제품을 필터링 할 수 있습니다.

:::image type="content" source="media/private-azure/filter-option.png" alt-text="필터링 옵션입니다.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>개인 Azure Marketplace에서 구입 또는 배포

제품 세부 정보 페이지 환경은 공용 Azure Marketplace와 유사 하지만 세 가지 전용 Azure Marketplace 특정 시나리오를 제공 합니다.

- 사용자가 허용 된 계획을 선택 하면 **만들기** 단추가 활성화 됩니다.

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="계획을 만들 수 있는 제품 배너입니다.":::

- 사용자가 허용 되지 않는 계획을 선택 하는 경우 해당 계획은 허용 되지 않으며 **만들기** 단추를 사용할 수 없습니다.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="계획을 만들 수 없는 배너를 제공 합니다.":::

- 제품 계획 선택이 제품 정보 페이지에 표시 되지 않지만 관리자가 하나 이상의 계획을 승인한 경우 배너에는 허용 되는 계획과 **만들기** 단추가 활성화 됩니다.

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="계획을 만들고 사용 가능한 계획을 표시할 수 있음을 나타내는 배너를 제공 합니다.":::

## <a name="contact-support"></a>지원에 문의

Azure Marketplace 지원이 필요한 경우 [Microsoft Q&A](/answers/products/)를 참조 하세요. 
