---
title: Azure Portal에서 개인 Azure Marketplace 만들기 및 관리
description: Azure Portal에서 개인 Azure Marketplace (미리 보기)를 만들고 관리 하는 방법에 대해 알아봅니다. 관리자는 개인 Azure Marketplace (미리 보기)를 사용 하 여 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712769"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Azure Portal에서 개인 Azure Marketplace 만들기 및 관리

관리자는 개인 Azure Marketplace를 통해 사용자가 사용할 수 있는 타사 솔루션을 제어할 수 있습니다. 이를 위해 사용자는 관리자가 승인한 제품만 배포할 수 있으며 기업의 정책을 준수할 수 있습니다. 사용자는 개인 Azure Marketplace를 사용 하 여 온라인 스토어에서 구입 및 배포할 규격 제안을 검색할 수 있습니다.

Marketplace 관리자 (할당 된 역할)로 서 승인 된 제안 및 계획을 추가할 수 있는 사용 안 함 및 빈 개인 저장소로 시작 합니다. 이 문서에서는 필요한 역할을 할당 하 고, 개인 저장소를 만들고, 항목을 관리 하 고, 사용자 요청을 승인 하 고, 사용자에 게 개인 Azure Marketplace를 사용 하도록 설정 하는 방법을 설명

> [!NOTE]
> - 개인 Azure Marketplace 테 넌 트 수준에 있으므로 테 넌 트의 모든 사용자에 게 동일한 큐 레이트 목록이 표시 됩니다.
> - 모든 Microsoft 솔루션 ( [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)은 자동으로 개인 Azure Marketplace에 추가 됩니다.

## <a name="assign-the-marketplace-admin-role"></a>Marketplace 관리자 역할 할당

테 넌 트 전역 관리자는 개인 저장소를 관리 하는 개인 Azure Marketplace 관리자에 게 **Marketplace 관리자** 역할을 할당 해야 합니다.

>[!IMPORTANT]
> 개인 Azure Marketplace 관리에 대 한 액세스는 IT 관리자가 Marketplace 관리자 역할이 할당 된 경우에만 사용할 수 있습니다.

### <a name="prerequisites"></a>필수 조건

이러한 필수 구성 요소는 사용자에 게 Marketplace 관리자 역할을 할당 하 여 테 넌 트 범위에서 사용자에 게 할당 해야 합니다.

- **전역 관리자** 사용자에 대 한 액세스 권한이 있습니다.
- 테 넌 트에 구독이 하나 이상 있습니다 (모든 형식일 수 있음).
- 전역 관리자 사용자에 게 선택한 구독에 대 한 **참가자** 역할 이상이 할당 됩니다.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>액세스 제어 (IAM)를 사용 하 여 Marketplace 관리자 역할 할당

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.
1. **모든 서비스** 를 선택한 다음 **Marketplace** 를 선택 합니다.
1. 왼쪽의 메뉴에서 **비공개 Marketplace** 를 선택 합니다.

    [![Marketplace의 왼쪽에 있는 개인 marketplace 메뉴 옵션을 표시 합니다.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. **액세스 제어 (IAM)** 를 선택 하 여 Marketplace 관리자 역할을 할당 합니다.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="I A M 액세스 제어 화면을 표시 합니다.":::

1. **추가** > **역할 할당 추가** 를 선택합니다.
1. **역할** 아래에서 **Marketplace 관리자** 를 선택 합니다.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="역할 할당 메뉴를 표시 합니다.":::

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

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal 주 창을 표시 합니다.":::

3. 왼쪽의 메뉴에서 **비공개 Marketplace** 를 선택 합니다.

4. **시작** 을 선택 하 여 개인 Azure Marketplace 만들기를 선택 합니다 .이 작업은 한 번만 수행 하면 됩니다.

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="' Azure Portal의 주 창에서 시작 하기를 선택 하는 방법을 보여 줍니다.":::

    이 테 넌 트에 대해 개인 Azure Marketplace 이미 있는 경우 **Marketplace 관리가** 기본적으로 선택 됩니다.

5. 완료 되 면 비어 있고 사용 하지 않도록 설정 된 개인 Azure Marketplace를 갖게 됩니다.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="빈 개인 Azure Marketplace 화면을 표시 합니다.":::

## <a name="add-items-from-gallery"></a>갤러리에서 항목 추가

항목은 제품 및 계획의 조합입니다. Marketplace 관리 페이지에서 항목을 검색 하 여 추가할 수 있습니다.

1. **항목 추가** 를 선택 합니다.

2. **갤러리** 를 찾아보거나 검색 필드를 사용 하 여 원하는 항목을 찾습니다.

    [![갤러리를 찾아보거나 검색 필드를 사용 하는 방법을 보여 줍니다.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. 기본적으로 새 제품을 추가할 때 모든 현재 계획이 승인 된 목록에 추가 됩니다. 선택한 항목을 추가 하기 전에 계획 선택을 수정 하려면 제품의 타일에서 드롭다운 메뉴를 선택 하 고 필요한 계획을 업데이트 합니다.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="필요한 계획을 업데이트 하는 방법을 보여 줍니다.":::

4. 선택한 후 왼쪽 아래에서 **완료** 를 선택 합니다.

>[!Note]
> Marketplace에 **항목 추가** 는 타사 제품에 대해서만 사용할 수 있습니다. Microsoft 솔루션 ( [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)은 "기본적으로 승인 됨"으로 태그가 지정 되 고 개인 Marketplace에서 관리할 수 없습니다.

## <a name="edit-items-plans"></a>항목의 계획 편집

Marketplace 관리 페이지에서 항목의 계획을 편집할 수 있습니다.

1. **계획** 열의 해당 항목에 대 한 드롭다운 메뉴에서 사용 가능한 계획을 검토 합니다.
2. 확인란을 선택 하거나 선택을 취소 하 여 사용자가 사용할 수 있도록 설정할 계획을 선택 합니다.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="필요한 항목에 대 한 확인란을 선택 하거나 선택 취소 하는 방법을 보여 줍니다.":::

> [!NOTE]
> 각 제품에는 업데이트를 수행 하기 위해 하나 이상의 계획을 선택 해야 합니다. 제품 관련 요금제를 모두 제거 하려면 전체 제품을 삭제 합니다 (다음 섹션 참조).

## <a name="delete-offers"></a>제안 삭제

Marketplace 관리 페이지에서 제품 이름 옆의 확인란을 선택 하 고 (위 화면 참조) **항목 삭제** 를 선택 합니다.

## <a name="enabledisable-private-azure-marketplace"></a>개인 Azure Marketplace 사용/사용 안 함

Marketplace 관리 페이지에 다음 배너 중 하나가 표시 됩니다 .이 배너에는 개인 Azure Marketplace의 현재 상태가 표시 됩니다.

:::image type="content" source="media/private-azure/state-disable.png" alt-text="' 상태 비활성화 ' 배너를 표시 합니다.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="' 상태 사용 ' 배너를 표시 합니다.":::

필요에 따라 개인 Azure Marketplace를 사용 하거나 사용 하지 않도록 설정할 수 있습니다.

- 사용 하지 않도록 설정 된 경우 **개인 Marketplace** 사용을 선택 합니다.
- 사용 하도록 설정 된 경우 **개인 Marketplace** 사용 안 함을 선택 합니다.

## <a name="private-azure-marketplace-notification-center"></a>개인 Azure Marketplace 알림 센터

알림 센터는 세 가지 유형의 알림으로 구성 되며 Marketplace 관리자는 알림을 기반으로 작업을 수행할 수 있습니다.

- 승인 된 목록에 없는 항목에 대 한 사용자의 승인 요청 (아래에 [제안 또는 요금제 추가 요청](#request-to-add-offers-or-plans) )을 참조 하세요.
- 승인 된 목록에 하나 이상의 계획이 이미 있는 제안에 대 한 새 계획 알림
- 승인 된 목록에 있지만 전역 Azure Marketplace에서 제거 된 항목에 대 한 계획 알림이 제거 되었습니다.

알림 센터에 액세스 하려면:

1. 왼쪽 메뉴에서 **알림** 을 선택 합니다.

    [![알림 메뉴를 표시 합니다.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. 추가 작업에 대 한 줄임표 메뉴를 선택 합니다.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="추가 옵션 메뉴 결과를 표시 합니다.":::

1. 계획 요청에서 **요청 표시** 는 특정 제품에 대 한 모든 사용자 요청을 검토할 수 있는 승인 요청 양식을 엽니다.
1. **승인** 또는 **거부** 를 선택 합니다.

    [![승인 및 거부 옵션을 표시 합니다.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. 드롭다운 메뉴에서 승인할 계획을 선택 합니다.
1. 의견을 추가 하 고 **제출** 을 선택 합니다.

## <a name="browsing-private-azure-marketplace"></a>비공개 Azure Marketplace 찾아보기

개인 Azure Marketplace를 사용 하는 경우 Marketplace 관리자가 승인한 요금제를 사용자에 게 표시 합니다.

- 녹색 **승인** 된 알림은 승인 된 파트너 (타사) 제품을 나타냅니다.
- 파란색 **승인** 된 알림은 승인 된 Microsoft 제품 ( [보증 Linux 배포판](/azure/virtual-machines/linux/endorsed-distros)포함)을 나타냅니다.

사용자는 승인 되지 않은 제품을 필터링 할 수 있습니다.

[![필터링 옵션을 보여 줍니다.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>개인 Azure Marketplace에서 구입 또는 배포

제품 세부 정보 페이지 환경은 글로벌 Azure Marketplace와 유사 하지만 세 가지 전용 Azure Marketplace 특정 시나리오를 제공 합니다.

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