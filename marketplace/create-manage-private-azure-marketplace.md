---
title: Azure Portal 프라이빗 Azure Marketplace 만들기 및 관리
description: Azure Portal 프라이빗 Azure Marketplace(미리 보기)를 만들고 관리하는 방법을 알아봅니다. 프라이빗 Azure Marketplace(미리 보기)를 통해 관리자는 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431666"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Azure Portal 프라이빗 Azure Marketplace 만들기 및 관리

프라이빗 Azure Marketplace 통해 관리자는 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다. 이렇게 하려면 사용자가 관리자가 승인한 제안만 배포하고 기업의 정책을 준수할 수 있습니다. Private Azure Marketplace 통해 사용자는 온라인 스토어에서 구매 및 배포할 규격 제안을 검색할 수 있습니다.

Marketplace 관리자(할당된 역할)는 승인된 제안 및 플랜을 추가할 수 있는 비활성 및 빈 프라이빗 저장소로 시작합니다. 이 문서에서는 필요한 역할을 할당하고, 프라이빗 저장소를 만들고, 항목을 관리하고, 사용자 요청을 승인하고, 사용자에 대한 프라이빗 Azure Marketplace 사용하도록 설정하는 방법을 설명합니다.

> [!NOTE]
> - 프라이빗 Azure Marketplace 테넌트 수준에 있으므로 테넌트 아래의 모든 사용자에게 동일한 큐레이팅된 목록이 표시됩니다.
> - 모든 Microsoft [솔루션(보증된 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)은 Private Azure Marketplace 자동으로 추가됩니다.

## <a name="assign-the-marketplace-admin-role"></a>Marketplace 관리자 역할 할당

테넌트 전역 관리자 프라이빗 스토어를 관리할 Private Azure Marketplace 관리자에게 **Marketplace** 관리자 역할을 할당해야 합니다.

>[!IMPORTANT]
> 프라이빗 Azure Marketplace 관리에 대한 액세스는 Marketplace 관리자 역할이 할당된 IT 관리자만 사용할 수 있습니다.

### <a name="prerequisites"></a>필수 조건

테넌트 범위의 사용자에게 Marketplace 관리자 역할을 할당하려면 다음 필수 조건이 필요합니다.

- **전역 관리자** 사용자에 액세스할 수 있습니다.
- 테넌트는 하나 이상의 구독을 가지고 있습니다(모든 형식일 수 있습니다).
- 전역 관리자 사용자에게는 선택한 구독에 대한 **기여자** 역할 이상에 할당됩니다.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>액세스 제어를 사용하여 Marketplace 관리자 역할 할당(IAM)

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.
1. **모든 서비스를** 선택한 **다음, Marketplace를** 선택합니다.
1. 왼쪽 메뉴에서 **프라이빗 마켓플레이스를** 선택합니다.

    [![Marketplace 왼쪽에 프라이빗 마켓플레이스 메뉴 옵션을 표시합니다.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. **액세스 제어(IAM)를** 선택하여 Marketplace 관리자 역할을 할당합니다.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="IM 액세스 제어 화면을 표시합니다.":::

1. **추가** > **역할 할당 추가** 를 선택합니다.
1. **역할** 아래에서 **Marketplace 관리자를** 선택합니다.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="역할 할당 메뉴를 표시합니다.":::

1. 드롭다운 목록에서 원하는 사용자를 선택한 다음, **완료를** 선택합니다.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>PowerShell을 사용하여 Marketplace 관리자 역할 할당

다음 PowerShell 스크립트를 사용하여 Marketplace 관리자 역할을 할당합니다. 다음 매개 변수가 필요합니다.

- **TenantId:** 범위에 있는 테넌트 ID입니다(Marketplace 관리자 역할은 테넌트 범위에서 할당 가능).
- **SubscriptionId:** 전역 관리자에게 **기여자** 역할 이상 할당이 할당된 구독입니다.
- **GlobalAdminUsername:** 전역 관리자의 사용자 이름입니다.
- **UsernameToAssignRoleFor:** Marketplace 관리자 역할이 할당될 사용자 이름입니다.

> [!NOTE]
> 테넌트로 초대된 게스트 사용자의 경우 해당 계정이 Marketplace 관리자 역할을 할당할 수 있을 때까지 최대 48시간이 걸릴 수 있습니다. 자세한 내용은 [Azure Active Directory B2B 협업 사용자의 속성을 참조하세요.](/azure/active-directory/b2b/user-properties)

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

Az.Portal PowerShell 모듈에 포함된 cmdlet에 대한 자세한 내용은 [Microsoft Azure PowerShell: 포털 대시보드 cmdlet을 참조하세요.](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>Private Azure Marketplace 만들기

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.
2. **모든 서비스를** 선택한 **다음, Marketplace를** 선택합니다.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal 주 창을 표시합니다.":::

3. 왼쪽 메뉴에서 **프라이빗 마켓플레이스를** 선택합니다.

4. **시작을** 선택하여 프라이빗 Azure Marketplace 만듭니다(이 작업을 한 번만 수행).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="'Azure Portal 시작' 주 창을 선택하는 방법을 보여줍니다.":::

    이 테넌트용 프라이빗 Azure Marketplace 이미 있는 경우 Marketplace **관리가** 기본적으로 선택됩니다.

5. 완료되면 비어 있고 비활성화된 Private Azure Marketplace 갖게 됩니다.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="빈 프라이빗 Azure Marketplace 화면을 표시합니다.":::

## <a name="add-items-from-gallery"></a>갤러리에서 항목 추가

항목은 제품과 플랜의 조합입니다. Marketplace 관리 페이지에서 항목을 검색하고 추가할 수 있습니다.

1. **항목 추가를** 선택합니다.

2. **갤러리를** 찾아보거나 검색 필드를 사용하여 원하는 항목을 찾습니다.

    [![갤러리를 찾아보거나 검색 필드를 사용하는 방법을 보여줍니다.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. 기본적으로 새 제안을 추가할 때 모든 현재 계획이 승인된 목록에 추가됩니다. 선택한 항목을 추가하기 전에 계획 선택을 수정하려면 제품 타일에서 드롭다운 메뉴를 선택하고 필요한 계획을 업데이트합니다.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="필요한 계획을 업데이트하는 방법을 보여줍니다.":::

4. 선택한 후 왼쪽 아래에서 **완료를** 선택합니다.

>[!Note]
> Marketplace에 **항목 추가는** Microsoft 이외의 제품에서만 사용할 수 있습니다. Microsoft [솔루션(보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)은 "기본적으로 승인"으로 태그가 지정되며 Private Marketplace에서 관리될 수 없습니다.

## <a name="edit-items-plans"></a>항목의 계획 편집

Marketplace 관리 페이지에서 항목의 계획을 편집할 수 있습니다.

1. **계획** 열의 드롭다운 메뉴에서 해당 항목의 사용 가능한 계획을 검토합니다.
2. 확인란을 선택하거나 선택을 취소하여 사용자가 사용할 계획을 선택합니다.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="필수 항목에 대한 확인란을 선택하거나 선택 취소하는 방법을 보여 있습니다.":::

> [!NOTE]
> 각 제안에는 업데이트가 발생하도록 하나 이상의 플랜이 선택되어 있어야 합니다. 제안과 관련된 모든 플랜을 제거하려면 전체 제안을 삭제합니다(다음 섹션 참조).

## <a name="delete-offers"></a>제안 삭제

Marketplace 관리 페이지에서 제품 이름 옆에 있는 확인란(위의 화면 참조)을 선택하고 **항목 삭제를** 선택합니다.

## <a name="enabledisable-private-azure-marketplace"></a>Private Azure Marketplace 사용/사용 안 함

Marketplace 관리 페이지에 프라이빗 Azure Marketplace 현재 상태를 보여 주는 배너 중 하나가 표시됩니다.

:::image type="content" source="media/private-azure/state-disable.png" alt-text="'상태 사용 안 함' 배너를 표시합니다.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="'상태 사용' 배너를 표시합니다.":::

필요에 따라 프라이빗 Azure Marketplace 사용하거나 사용하지 않도록 설정할 수 있습니다.

- 사용하지 않도록 설정한 경우 **프라이빗 마켓플레이스 사용을** 선택하여 사용하도록 설정합니다.
- 사용하도록 설정된 경우 **프라이빗 마켓플레이스 사용 안 함을** 선택하여 사용하지 않도록 설정합니다.

## <a name="private-azure-marketplace-notification-center"></a>프라이빗 Azure Marketplace 알림 센터

알림 센터는 세 가지 유형의 알림으로 구성되며 Marketplace 관리자가 알림에 따라 작업을 수행할 수 있습니다.

- 승인된 목록에 없는 항목에 대한 사용자의 승인 요청(아래 [제품 또는 플랜 추가 요청](#request-to-add-offers-or-plans) 참조).
- 승인된 목록에 하나 이상의 계획이 이미 있는 제안에 대한 새 계획 알림입니다.
- 승인된 목록에 있지만 전역 Azure Marketplace 제거된 항목에 대한 계획 알림이 제거되었습니다.

알림 센터에 액세스하려면 다음을 수행합니다.

1. 왼쪽 메뉴에서 **알림을** 선택합니다.

    [![알림 메뉴를 표시합니다.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. 더 많은 작업을 수행하려면 말임표 메뉴를 선택합니다.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="추가 옵션 메뉴 결과를 표시합니다.":::

1. 계획 요청의 경우 **요청 표시는** 특정 제안에 대한 모든 사용자 요청을 검토할 수 있는 승인 요청 양식을 엽니다.
1. **승인** 또는 **거부를** 선택합니다.

    [![승인 및 거부 옵션을 표시합니다.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. 드롭다운 메뉴에서 승인할 계획을 선택합니다.
1. 주석을 추가하고 **제출을** 선택합니다.

## <a name="browsing-private-azure-marketplace"></a>프라이빗 Azure Marketplace 찾아보기

프라이빗 Azure Marketplace 사용하도록 설정하면 Marketplace 관리자가 승인한 플랜이 표시됩니다.

- 녹색 **승인 알림은 승인된** 파트너(비 Microsoft) 제안을 나타냅니다.
- 파란색 **승인 알림은 승인된** Microsoft [제안(보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)을 나타냅니다.

사용자는 승인된 제품과 승인되지 않은 제품 간에 필터링할 수 있습니다.

[![필터링 옵션을 표시합니다.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>프라이빗 Azure Marketplace 구입 또는 배포

제품 세부 정보 페이지 환경은 글로벌 Azure Marketplace 비슷하지만 세 가지 프라이빗 Azure Marketplace 특정 시나리오가 있습니다.

- 사용자가 승인 된 계획을 선택 하는 경우 **만들기** 단추를 사용할 수 있습니다.

    [![계획을 만들 수 있는 제품 배너를 표시 합니다.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- 제품 계획 선택이 제품 정보 페이지에 표시 되지 않지만 관리자가 하나 이상의 계획을 승인한 경우, 배너에 승인 된 계획과 **만들기** 단추가 활성화 됩니다.

    [![계획을 만들 수 있고 사용 가능한 요금제를 표시 하는 제품 배너를 표시 합니다.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- 사용자가 승인 되지 않은 요금제를 선택 하면 배너는 계획을 승인 되지 않은 것으로 메모 하 고 **만들기** 단추를 사용할 수 없습니다. 사용자는 여전히 계획을 승인 된 목록에 추가 하도록 요청할 수 있습니다 (다음 섹션 참조).

## <a name="request-to-add-offers-or-plans"></a>제안 또는 계획 추가 요청

현재 개인 Azure Marketplace에서 승인 되지 않은 공개 제품 또는 계획을 추가 하도록 요청할 수 있습니다.

1. 배너에서 **추가할 요청** 을 선택 하 여 **액세스 요청 양식을** 엽니다.

    [![' 추가 요청 ' 링크가 포함 된 배너를 표시 합니다.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![제안 또는 계획에 대 한 액세스 요청 양식을 표시 합니다.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. 요청에 추가할 계획을 선택 합니다.**모든 계획** 은 Marketplace 관리자에 게 제품 내 계획에 대 한 기본 설정이 없음을 알립니다.

1. **사유** 를 추가 하 고 요청을 제출 하는 **요청** 을 선택 합니다.
  
    [![샘플 항목이 포함 된 제안 또는 계획에 대 한 액세스 요청 폼을 표시 합니다.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. 보류 중인 요청에 대 한 표시가 **요청을 철회** 하는 옵션과 함께 액세스 요청 폼에 표시 됩니다.

    [![요청 취소 링크를 사용 하 여 승인 되거나 보류 중인 계획의 목록을 표시 합니다.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> 제출한 후에는 마켓플레이스 관리자가 요청을 검토 하 고 조치를 취하는 [알림 센터로](#private-azure-marketplace-notification-center) 승인 요청 양식이 전송 됩니다.

> [!CAUTION]
> 비공개 Marketplace에 대 한 승인은 솔루션 조달을 나타내지는 않습니다.

## <a name="frequently-asked-questions-faqs"></a>FAQ(질문과 대답)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Azure Policy를 통해 Marketplace 타사 응용 프로그램을 이미 차단 하 고 있습니다. 이 방법은 어떻게 다른 가요?

현재 Marketplace에서 타사 서비스를 제한 하는 두 가지 방법이 있습니다.

1. EA 포털 또는 Azure Portal을 통해 타사 서비스를 사용 하지 않도록 설정 하거나 "무료 또는 BYOL Sku만 해당"으로 제한 합니다.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Azure Portal에서 서비스를 제한 하는 방법을 보여 줍니다.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E A 포털에서 서비스를 제한 하는 방법을 보여 줍니다.":::

2. 특정 Vm만 허용 하는 Azure policy를 만듭니다. Windows Vm에 정책을 적용 하는 방법에 대 한 자세한 내용은 [Azure Resource Manager를 사용 하 여 Windows vm에 정책 적용](/azure/virtual-machines/windows/policy)을 참조 하세요.

개인 Azure Marketplace 특정 제공 및 계획을 제한 하 고 허용 하는 유연성을 향상 시킬 수 있습니다. 최종 사용자에 게 타사 서비스를 배포 하기 전까지 marketplace 갤러리의 배포에 대 한 가용성을 알립니다. 타사 서비스의 배포를 허용 하려면 Azure Marketplace를 EA 포털에서 설정/사용으로 설정 하 고 Azure Portal 합니다.

- 개인 Azure Marketplace는 가상 머신으로 제한 되지 않는 파트너 솔루션을 만들 수 있습니다.
- 비공개 Azure Marketplace는 계획 수준에서 ' 현재 및 미래 요금제 '를 설정할 수도 있습니다.
- 개인 Azure Marketplace는 최종 사용자에 게 배포할 수 있으며 배포할 수 없는 항목에 대해 맨 앞에 알려줄 수 있습니다.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>개인 제품 및 개인 Azure Marketplace 간의 차이점은 무엇 인가요?

**개인 제안을** 통해 게시자는 대상 고객 에게만 표시 되는 계획을 만들 수 있습니다. 이렇게 하면 사용자 지정 된 솔루션을 협상 된 가격 책정, 개인 사용 조건 및 특수 한 구성과 개인적으로 공유할 수 있습니다. 자세한 내용은 [상업적 marketplace의 개인 제품](/azure/marketplace/private-offers)을 참조 하세요.

관리자는 Azure Portal의 **개인 Azure Marketplace** 를 사용 하 여 사용자가 배포할 수 있는 타사 솔루션을 미리 승인할 수 있습니다. 사용자는 개인 Azure Marketplace를 사용 하 여 규정 준수 제안을 찾고 구매 하 고 배포 하 여 Azure Marketplace 이점을 누릴 수 있습니다. 개인 Marketplace에서 구독 기반 개인 제안을 관리 하려면 Marketplace 관리자에 게 특정 구독에 대 한 "읽기" 이상의 역할이 있어야 합니다.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>개인 제품을 개인 Azure Marketplace에 추가 했습니다. Marketplace 관리 탭에 표시 되지 않는 이유는 무엇 인가요?

구독 기반 개인 제품은 비공개 제품 설정에서 나열 된 구독에 대해서만 표시 됩니다. 비공개 제품을 보려면 전역 구독 필터가 모든 구독을 표시 하는지 확인 합니다.

[![개인 marketplace 필터를 표시 합니다.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>개인 Azure Marketplace에 사용자 지정 이미지를 포함할 수 있나요?

아니요. 개인 Azure Marketplace를 사용 하면 IT 관리자가 글로벌 Azure Marketplace에서 타사 솔루션을 관리 하 고 curate 할 수 있습니다. 사용자 지정 이미지는 글로벌 Azure Marketplace에 있지 않으므로 IT 관리자는 사용자 지정 이미지를 선택 하 여 선택할 수 없습니다. 사용자 지정 이미지를 공유 하려면 [공유 이미지 갤러리](/azure/virtual-machines/shared-image-galleries)를 사용 합니다.

1. 단계별 가이드 SIG (공유 이미지 갤러리) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell))를 만듭니다.
2. SIG 내에서 이미지 정의를 만듭니다. 고객은 OS 상태 필드에 대해 **일반화** 된을 선택 해야 합니다. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. 관리 되는 이미지를 공유 이미지 갤러리 ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell))로 가져옵니다.
4. SIG VM 이미지는 하나의 구독에 상주 합니다. 다른 구독에서 사용할 수 있도록 하려면 앱 등록 ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants))을 사용 합니다.

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>게시자가 Microsoft가 아닌 경우에도 **기본적으로** 몇 가지 제안이 승인 되는 이유는 무엇 인가요?

Microsoft는 Azure에서 Linux 및 오픈 소스 기술을 지원 합니다. [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros) 은 Azure에서 지원 되 고 가격은 virtual machines에 통합 됩니다. Azure Linux 에이전트는 이미 Azure Marketplace에 미리 설치 되어 있기 때문에 Microsoft 제품 처럼 취급 됩니다. Microsoft 제공은 기본적으로 승인 되므로 보증 Linux 배포판은 개인 Azure Marketplace에서 관리할 수 없으며 기본적으로 승인 됩니다.

## <a name="contact-support"></a>지원에 문의

- Azure Marketplace 지원이 필요한 경우 [Microsoft Q&A](/answers/products/)를 참조 하세요.