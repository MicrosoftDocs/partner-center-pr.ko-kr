---
title: Azure CSP에 대한 관리자 권한 복구
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너가 고객의 Azure CSP(클라우드 솔루션 공급자) 구독을 관리할 수 있도록 고객이 파트너의 관리자 권한을 복구하도록 돕는 방법에 대해 알아봅니다.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d784aef33cce2a722583a77e73c35d5fc8136b1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551591"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="10f4f-103">고객의 Azure CSP 구독에 대한 관리자 권한 복구</span><span class="sxs-lookup"><span data-stu-id="10f4f-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="10f4f-104">**적절한 역할**: 전역 관리자 | 관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="10f4f-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="10f4f-105">CSP(클라우드 솔루션 공급자) 파트너로서 고객은 Azure 사용량과 해당 시스템을 관리할 것으로 기대하는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="10f4f-106">이렇게 하려면 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="10f4f-107">고객과의 재판매인 관계가 설정되면 일부 권한이 부여됩니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="10f4f-108">다른 권한은 고객이 사용자에게 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="10f4f-109">CSP의 Azure에 대한 관리자 권한</span><span class="sxs-lookup"><span data-stu-id="10f4f-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="10f4f-110">CSP에는 Azure에 대한 다음 두 가지 수준의 관리자 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="10f4f-111">**테넌트 수준 관리자 권한(위임된 관리자 권한)** : CSP 파트너는 고객과의 CSP 재판매인 관계를 설정하면서 이러한 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="10f4f-112">위임된 관리자 권한은 CSP 파트너에게 고객의 테넌트에 대한 액세스 권한을 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="10f4f-113">이 액세스를 통해 사용자 추가/관리, 암호 초기화 및 사용자 라이선스 관리와 같은 관리 기능을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="10f4f-114">**구독 수준 관리자 권한**: CSP 파트너는 고객에 대한 Azure CSP 구독을 만들면서 이러한 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="10f4f-115">이러한 권한이 있으면 CSP 파트너는 이러한 구독에 완전하게 액세스할 수 있으므로 Azure 리소스를 프로비저닝하고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="10f4f-116">CSP 파트너의 관리자 권한 복구</span><span class="sxs-lookup"><span data-stu-id="10f4f-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="10f4f-117">고객에게 AdminAgents 그룹의 `object ID`를 제공하는 경우 고객은 CSP 역할 할당을 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="10f4f-118">위임된 관리자 권한을 다시 얻으려면 다음 단계를 통해 고객과 협력해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="10f4f-119">파트너 센터 대시보드에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="10f4f-120">파트너 센터 메뉴에서 **고객** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="10f4f-121">협력하는 고객을 선택하고 **재판매인 관계를 요청** 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="10f4f-122">이 작업은 테넌트 관리자 권한이 있는 고객에 대한 링크를 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="10f4f-123">고객은 링크를 선택하고 재판매인 관계 요청을 승인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="재판매인 관계 만들기의 이메일 예제":::

5. <span data-ttu-id="10f4f-125">파트너는 AdminAgents 그룹의 개체 ID를 가져오기 위해 파트너 테넌트에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="10f4f-126">고객은 PowerShell 또는 Azure CLI를 사용하여 다음 단계를 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="10f4f-127">고객에게는 다음이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-127">Your customer must have:</span></span>

- <span data-ttu-id="10f4f-128">**소유자** 또는 **사용자 액세스 관리자** 의 역할</span><span class="sxs-lookup"><span data-stu-id="10f4f-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="10f4f-129">구독 수준에서 역할 할당을 만들 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="10f4f-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="10f4f-130">a.</span><span class="sxs-lookup"><span data-stu-id="10f4f-130">a.</span></span> <span data-ttu-id="10f4f-131">PowerShell의 경우에만 고객이 `Az.Resources` 모듈을 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="10f4f-132">b.</span><span class="sxs-lookup"><span data-stu-id="10f4f-132">b.</span></span> <span data-ttu-id="10f4f-133">고객은 CSP 구독이 있는 테넌트에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="10f4f-134">c.</span><span class="sxs-lookup"><span data-stu-id="10f4f-134">c.</span></span> <span data-ttu-id="10f4f-135">고객은 구독에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-135">The customer connects to the subscription.</span></span> <span data-ttu-id="10f4f-136">사용자에게 테넌트의 여러 구독에 대한 역할 할당 권한이 있는 *경우에만* 적용 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="10f4f-137">d.</span><span class="sxs-lookup"><span data-stu-id="10f4f-137">d.</span></span> <span data-ttu-id="10f4f-138">그러면 고객이 역할 할당을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="10f4f-139">구독 범위에서 소유자 권한을 부여하는 대신 리소스 그룹 또는 리소스 수준에서 권한을 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="10f4f-140">리소스 그룹 수준에서</span><span class="sxs-lookup"><span data-stu-id="10f4f-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="10f4f-141">리소스 수준에서</span><span class="sxs-lookup"><span data-stu-id="10f4f-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="10f4f-142">위의 단계가 작동하지 않거나 시도할 때 오류가 발생하면 다음 "catch-all" 프로시저를 시도하여 고객의 관리자 권한을 복구합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="10f4f-143">문제 해결</span><span class="sxs-lookup"><span data-stu-id="10f4f-143">Troubleshooting</span></span>

<span data-ttu-id="10f4f-144">고객이 위의 6단계를 완료할 수 없는 경우 고객이 다음 명령을 시도하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="10f4f-145">추가 분석을 위해 결과 `newRoleAssignment.log` 파일을 Microsoft에 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="10f4f-146">`Import-Module` 중 "catch-all" 프로시저가 실패하는 경우 다음 단계를 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="10f4f-147">모듈이 사용 중이어서 가져오기가 실패하면 모든 창을 닫았다가 다시 열어 PowerShell 세션을 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="10f4f-148">`Get-Module Az.Resources -ListAvailable`을 사용하여 `Az.Resources`의 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="10f4f-149">버전 4.1.1이 사용 가능한 목록에 없는 경우 `Update-Module Az.Resources -Force`를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="10f4f-150">오류가 `Az.Accounts`가 특정 버전이어야 한다고 표시하면 해당 모듈도 업데이트하여 `Az.Resources`를 `Az.Accounts`로 바꿉니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="10f4f-151">그런 다음, PowerShell 세션을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="10f4f-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="10f4f-152">다음 단계</span><span class="sxs-lookup"><span data-stu-id="10f4f-152">Next steps</span></span>

- [<span data-ttu-id="10f4f-153">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="10f4f-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
