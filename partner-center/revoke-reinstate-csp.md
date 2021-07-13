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
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510179"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>고객의 Azure CSP 구독에 대한 관리자 권한 복구  

**적절한 역할**: 전역 관리자 | 관리자 에이전트

CSP(클라우드 솔루션 공급자) 파트너로서 고객은 Azure 사용량과 해당 시스템을 관리할 것으로 기대하는 경우가 많습니다. 이렇게 하려면 관리자 권한이 있어야 합니다. 고객과의 재판매인 관계가 설정되면 일부 권한이 부여됩니다. 다른 권한은 고객이 사용자에게 부여합니다.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP의 Azure에 대한 관리자 권한

CSP에는 Azure에 대한 다음 두 가지 수준의 관리자 권한이 있습니다.

- **테넌트 수준 관리자 권한(위임된 관리자 권한)** : CSP 파트너는 고객과의 CSP 재판매인 관계를 설정하면서 이러한 권한을 얻습니다. 위임된 관리자 권한은 CSP 파트너에게 고객의 테넌트에 대한 액세스 권한을 부여합니다. 이 액세스를 통해 사용자 추가/관리, 암호 초기화 및 사용자 라이선스 관리와 같은 관리 기능을 수행할 수 있습니다.
- **구독 수준 관리자 권한**: CSP 파트너는 고객에 대한 Azure CSP 구독을 만들면서 이러한 권한을 얻습니다. 이러한 권한이 있으면 CSP 파트너는 이러한 구독에 완전하게 액세스할 수 있으므로 Azure 리소스를 프로비저닝하고 관리할 수 있습니다.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>CSP 파트너의 관리자 권한 복구

고객에게 AdminAgents 그룹의 `object ID`를 제공하는 경우 고객은 CSP 역할 할당을 다시 만들 수 있습니다. 위임된 관리자 권한을 다시 얻으려면 다음 단계를 통해 고객과 협력해야 합니다.

1. 파트너 센터 대시보드에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객** 을 선택합니다.

3. 협력하는 고객을 선택하고 **재판매인 관계를 요청** 합니다. 이 작업은 테넌트 관리자 권한이 있는 고객에 대한 링크를 생성합니다.

4. 고객은 링크를 선택하고 재판매인 관계 요청을 승인해야 합니다.

   :::image type="content" source="images/azure/revoke4.png" alt-text="재판매인 관계 만들기의 이메일 예제":::

5. 파트너는 AdminAgents 그룹의 개체 ID를 가져오기 위해 파트너 테넌트에 연결해야 합니다.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. 고객은 PowerShell 또는 Azure CLI를 사용하여 다음 단계를 수행해야 합니다. 고객에게는 다음이 있어야 합니다.

- **소유자** 또는 **사용자 액세스 관리자** 의 역할 
- 구독 수준에서 역할 할당을 만들 수 있는 권한

   a. PowerShell의 경우에만 고객이 `Az.Resources` 모듈을 업데이트해야 합니다.
   ```powershell
   Update-Module Az.Resources
   ```

   b. 고객은 CSP 구독이 있는 테넌트에 연결합니다.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. 고객은 구독에 연결합니다. 사용자에게 테넌트의 여러 구독에 대한 역할 할당 권한이 있는 *경우에만* 적용 가능합니다.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. 그러면 고객이 역할 할당을 만듭니다.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

구독 범위에서 소유자 권한을 부여하는 대신 리소스 그룹 또는 리소스 수준에서 권한을 부여할 수 있습니다. 

- 리소스 그룹 수준에서

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- 리소스 수준에서

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

위의 단계가 작동하지 않거나 시도할 때 오류가 발생하면 다음 "catch-all" 프로시저를 시도하여 고객의 관리자 권한을 복구합니다.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>문제 해결

고객이 위의 6단계를 완료할 수 없는 경우 고객이 다음 명령을 시도하도록 합니다.

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

추가 분석을 위해 결과 `newRoleAssignment.log` 파일을 Microsoft에 제공합니다.

`Import-Module` 중 "catch-all" 프로시저가 실패하는 경우 다음 단계를 시도합니다.
- 모듈이 사용 중이어서 가져오기가 실패하면 모든 창을 닫았다가 다시 열어 PowerShell 세션을 다시 시작합니다.
- `Get-Module Az.Resources -ListAvailable`을 사용하여 `Az.Resources`의 버전을 확인합니다.
- 버전 4.1.1이 사용 가능한 목록에 없는 경우 `Update-Module Az.Resources -Force`를 사용해야 합니다.
- 오류가 `Az.Accounts`가 특정 버전이어야 한다고 표시하면 해당 모듈도 업데이트하여 `Az.Resources`를 `Az.Accounts`로 바꿉니다. 그런 다음, PowerShell 세션을 다시 시작해야 합니다.


## <a name="next-steps"></a>다음 단계

- [Azure 플랜 하에서 구독 및 리소스 관리](azure-plan-manage.md)
