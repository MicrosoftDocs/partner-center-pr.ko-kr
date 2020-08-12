---
title: Azure CSP에 대한 관리자 권한 복구
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너가 고객의 Azure CSP 구독을 관리할 수 있도록 고객이 파트너의 관리자 권한을 복구하도록 돕는 방법에 대해 알아봅니다.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811333"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>고객의 Azure CSP 구독에 대한 관리자 권한 복구  

**적용 가능한 역할**

- 글로벌 관리자
- 관리 에이전트

CSP 파트너로서 고객은 Azure 사용량과 해당 시스템을 관리할 것으로 기대하는 경우가 많습니다. 이렇게 하려면 관리자 권한이 있어야 합니다. 고객과의 재판매인 관계가 설정되면 일부 권한이 부여됩니다. 다른 권한은 고객이 사용자에게 부여합니다.

## <a name="admin-privileges-for-azure-in-csp"></a>CSP의 Azure에 대한 관리자 권한

CSP에는 Azure에 대한 다음 두 가지 수준의 관리자 권한이 있습니다.

**테넌트 수준 관리자 권한**(**위임된 관리자 권한**) – CSP 파트너는 고객과의 CSP 재판매인 관계를 설정하면서 이러한 권한을 얻습니다. 이를 통해 CSP 파트너는 고객의 테넌트에 액세스할 수 있으므로 사용자 추가/관리, 암호 재설정 및 사용자 라이선스 관리와 같은 관리 기능을 수행할 수 있습니다.

**구독 수준 관리자 권한** – CSP 파트너는 고객에 대한 Azure CSP 구독을 만들면서 이러한 권한을 얻습니다. 이러한 권한이 있으면 CSP 파트너는 이러한 구독에 완전하게 액세스할 수 있으므로 Azure 리소스를 프로비저닝하고 관리할 수 있습니다.

## <a name="reinstate-csp-partners-admin-privileges"></a>CSP 파트너의 관리자 권한 복구

위임된 관리자 권한을 다시 얻으려면 고객과 협력해야 합니다.

1. 파트너 센터 대시보드에 로그인하고, 파트너 센터 메뉴에서 **고객**을 선택합니다.

2. 협력하는 고객을 선택하고, **재판매인 관계를 요청**합니다. 그러면 테넌트 관리자 권한이 있는 고객에 대한 링크가 생성됩니다.

3. 해당 사용자는 링크를 선택하고, 재판매인 관계 요청을 승인해야 합니다.

   :::image type="content" source="images/azure/revoke4.png" alt-text="재판매인 관계":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>관리 에이전트 그룹을 Azure CSP 구독 소유자로 추가

고객은 관리 에이전트 그룹을 Azure CSP 구독 소유자로 추가해야 합니다.

1. PowerShell 콘솔 또는 PowerShell ISE(통합 스크립팅 환경)를 사용합니다. AzureAD 모듈이 설치되어 있는지 확인합니다.

2. Azure AD 테넌트에 연결합니다.

   ```powershell
   Connect-AzureAD
   ```

3. 관리 에이전트 그룹의 ObjectId를 가져옵니다.

   ```powershell
   Get-AzureADGroup
   ```
   다음 단계는 Azure CSP 구독에 대한 소유자 액세스 권한이 있는 고객 회사의 사용자가 수행합니다.

4. Azure CSP 구독에 대한 소유자 액세스 권한이 있는 사용자는 자신의 자격 증명을 사용하여 Azure에 로그인합니다.

   ```powershell
   Connect-AzAccount
   ```

5. 그런 다음, 관리 에이전트 그룹을 소유자로 CSP Azure 구독에 추가할 수 있습니다.

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>다음 단계

[Azure 플랜 하에서 구독 및 리소스 관리](azure-plan-manage.md)
