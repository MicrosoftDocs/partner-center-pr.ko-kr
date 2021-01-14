---
title: '빠른 시작: PowerShell을 사용 하 여 개인 Azure Marketplace 관리'
description: 이 빠른 시작에서는 Azure PowerShell를 사용 하 여 개인 Azure Marketplace에서 제품을 관리 하는 방법을 보여 줍니다.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182344"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="12075-103">빠른 시작: PowerShell을 사용 하 여 개인 Azure Marketplace 관리</span><span class="sxs-lookup"><span data-stu-id="12075-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="12075-104">이 문서에서는 [Az. Marketplace](/powershell/module/az.marketplace) PowerShell 모듈을 사용 하 여 개인 Azure Marketplace에서 제품을 관리 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="12075-105">개인 Azure Marketplace 현재 공개 미리 보기 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="12075-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="12075-106">이 미리 보기 버전은 서비스 수준 계약 없이 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="12075-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="12075-107">프로덕션 워크로드에는 권장되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="12075-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="12075-108">일부 기능은 지원 되지 않거나 제한 된 기능을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="12075-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="12075-109">자세한 내용은 [Microsoft Azure Preview에 대한 추가 사용 약관](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="12075-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="12075-110">요구 사항</span><span class="sxs-lookup"><span data-stu-id="12075-110">Requirements</span></span>

* <span data-ttu-id="12075-111">Azure 구독이 아직 없는 경우 시작하기 전에 [체험](https://azure.microsoft.com/free/) 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="12075-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="12075-112">Azure PowerShell을 로컬로 사용하도록 선택하는 경우:</span><span class="sxs-lookup"><span data-stu-id="12075-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="12075-113">[Az PowerShell 모듈을 설치합니다](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="12075-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="12075-114">[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet을 사용하여 Azure 계정에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="12075-115">Azure Cloud Shell을 사용하도록 선택하는 경우:</span><span class="sxs-lookup"><span data-stu-id="12075-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="12075-116">자세한 내용은 [Azure Cloud Shell 개요](/azure/cloud-shell/overview)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="12075-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="12075-117">**Az** PowerShell module은 preview에 있지만 cmdlet을 사용 하 여 별도로 설치 해야 합니다. `Install-Module`</span><span class="sxs-lookup"><span data-stu-id="12075-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="12075-118">이 PowerShell 모듈이 일반 공급되면 이후 Az PowerShell 모듈 릴리스의 일부가 되며 기본적으로 Azure Cloud Shell 내에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="12075-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="12075-119">여러 Azure 구독이 있는 경우 리소스에 대한 요금이 청구되는 적절한 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="12075-120">[Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet을 사용하여 특정 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="12075-121">개인 저장소 나열</span><span class="sxs-lookup"><span data-stu-id="12075-121">List private stores</span></span>

<span data-ttu-id="12075-122">개인 저장소 목록을 검색 하려면 [AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="12075-123">다음 예제에서는 테 넌 트 범위에서 만들어진 개인 저장소를 나열 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="12075-124">개인 marketplace에 제품 추가</span><span class="sxs-lookup"><span data-stu-id="12075-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="12075-125">개인 저장소에 제품을 추가 하려면 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="12075-126">다음 예에서는 테 넌 트 범위 아래에 생성 된 개인 저장소의 개인 marketplace에 지정 된 제품을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="12075-127">개인 저장소 제안 가져오기</span><span class="sxs-lookup"><span data-stu-id="12075-127">Get private store offers</span></span>

<span data-ttu-id="12075-128">하나 이상의 개인 저장소 제안을 가져오려면 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="12075-129">다음 예제에서는 테 넌 트 범위 아래에 추가 된 지정 된 개인 저장소와 연결 된 제안을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="12075-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="12075-130">제안 제거</span><span class="sxs-lookup"><span data-stu-id="12075-130">Remove an offer</span></span>

<span data-ttu-id="12075-131">개인 저장소에서 제품을 제거 하려면 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="12075-132">다음 예제에서는 테 넌 트 범위에서 만들어진 개인 저장소에서 제품을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="12075-133">다음 단계</span><span class="sxs-lookup"><span data-stu-id="12075-133">Next steps</span></span>

<span data-ttu-id="12075-134">[개인 Azure Marketplace를 만들고 관리](create-manage-private-azure-marketplace.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="12075-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>