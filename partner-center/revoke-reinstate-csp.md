---
title: Azure CSP에 대한 관리자 권한 복구
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너가 고객의 Azure CSP 구독을 관리할 수 있도록 고객이 파트너의 관리자 권한을 복구하도록 돕는 방법에 대해 알아봅니다.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315850"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>고객의 Azure CSP 구독에 대한 관리자 권한 복구  

**적용 가능한 역할**

- 글로벌 관리자
- 관리 에이전트

CSP 파트너로서 고객은 Azure 사용량과 해당 시스템을 관리할 것으로 기대하는 경우가 많습니다. 이렇게 하려면 관리자 권한이 있어야 합니다. 고객과의 재판매인 관계가 설정되면 일부 권한이 부여됩니다. 다른 권한은 고객이 사용자에게 부여합니다.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP의 Azure에 대한 관리자 권한

CSP에는 Azure에 대한 다음 두 가지 수준의 관리자 권한이 있습니다.

**테넌트 수준 관리자 권한**(**위임된 관리자 권한**) – CSP 파트너는 고객과의 CSP 재판매인 관계를 설정하면서 이러한 권한을 얻습니다. 위임된 관리자 권한을 통해 CSP 파트너는 고객의 테넌트에 액세스할 수 있으므로 사용자 추가/관리, 암호 재설정 및 사용자 라이선스 관리와 같은 관리 기능을 수행할 수 있습니다.

**구독 수준 관리자 권한** – CSP 파트너는 고객에 대한 Azure CSP 구독을 만들면서 이러한 권한을 얻습니다. 이러한 권한이 있으면 CSP 파트너는 이러한 구독에 완전하게 액세스할 수 있으므로 Azure 리소스를 프로비저닝하고 관리할 수 있습니다.

## <a name="reinstate-csp-partners-admin-privileges"></a>CSP 파트너의 관리자 권한 복구

고객에게 AdminAgents 그룹의 개체 ID를 제공하는 한 고객은 CSP 역할 할당을 다시 만들 수 있습니다. 위임된 관리자 권한을 다시 얻으려면 고객과 협력해야 합니다.

1. 파트너 센터 대시보드에 로그인하고, 파트너 센터 메뉴에서 **고객** 을 선택합니다.

2. 협력하는 고객을 선택하고, **재판매인 관계를 요청** 합니다. 그러면 테넌트 관리자 권한이 있는 고객에 대한 링크가 생성됩니다.

3. 해당 고객은 링크를 선택하고, 재판매인 관계 요청을 승인해야 합니다.

   :::image type="content" source="images/azure/revoke4.png" alt-text="재판매인 관계 만들기의 이메일 예제":::

4. 파트너는 AdminAgents 그룹의 개체 ID를 가져오기 위해 파트너 테넌트에 연결해야 합니다.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. **소유자 또는 사용자 액세스 관리자** 역할을 하며 구독 수준에서 역할 할당을 만들 수 있는 권한이 있는 고객은 다음을 수행합니다.


    1. CSP 구독이 있는 테넌트에 연결합니다.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. 구독에 연결합니다(사용자에게 테넌트의 여러 구독에 대한 역할 할당 권한이 있는 경우에만 적용 가능).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"`


    3. 역할 할당 만들기
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


구독 범위 대신 리소스 그룹 수준 또는 리소스 수준에서 소유자 역할 권한을 부여하려는 경우 다음 명령을 사용할 수 있습니다.


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>다음 단계

- [Azure 플랜 하에서 구독 및 리소스 관리](azure-plan-manage.md)
