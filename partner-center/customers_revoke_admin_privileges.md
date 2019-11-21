---
title: 고객이 파트너에게 관리 권한을 위임하는 경우 | 파트너 센터
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to ask customers to delegate administrator permissions to a reseller or remove the same permissions and how to use the permissions.
author: LauraBrenner
ms.author: labrenne
keywords: delegated admin privileges, admin on behalf of, remove privileges, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 8f49fa5c4b320d05c6c6a9049b41170457bb394f
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253479"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>고객이 파트너에게 관리 권한을 위임하는 경우

**적용 대상**

-  파트너 센터

고객을 대신하여 고객 서비스 또는 구독을 관리하려면 고객이 해당 서비스에 대한 관리자 권한을 부여해야 합니다. 고객으로부터 관리자 권한을 얻으려면 고객에게 전자 메일로 재판매인 관계 요청을 보내야 합니다. 고객이 요청을 승인하면 해당 서비스의 관리 포털에 로그인하여 고객 대신 서비스를 관리할 수 있습니다. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>귀사와 재판매인 관계를 맺도록 고객 초대

1.  Select **Customers** and then select **Request a reseller relationship**.

2.  다음 페이지에서 임시 이메일 메시지를 검토합니다. 기본 전자 메일 응용 프로그램에서 임시 메시지를 열거나 클립보드에 메시지를 복사한 후 전자 메일에 붙여 넣을 수 있습니다. 

    >[!IMPORTANT]
    >이메일에서 텍스트를 편집할 수 있지만, 이메일에 링크를 포함하는 것을 잊지 마세요. 이 링크는 고객을 귀사의 계정에 직접 연결하는 맞춤형 링크입니다. 
    
3.  Select **Done** when you've completed this step.

4.  고객에게 이메일을 보냅니다.

5.  고객이 초대를 수락하면 **고객** 페이지에 고객이 표시되고, 귀사는 여기서 해당 고객의 서비스를 프로비전하고 관리할 수 있습니다.

6.  To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name and then select the admin portal for the service you want to manage.

>[!IMPORTANT]  
>Customers can reassign or remove administrator permissions in a service's admin portal. 그러나 고객이 관리자 권한을 다시 할당하거나 제거하더라도 고객과 계약을 다시 협상할 때까지는 계속해서 고객 지원을 제공하고 클라우드 재판매인 계약의 약관을 준수할 책임이 있습니다. In this situation, if the customer requires help, contact Microsoft support to open a service request on behalf of the customer.

Your customers can find out which of their partners have admin privileges to their tenant from within the Office 365 admin portal. 이렇게 하려면 다음을 수행합니다.

1. The customer needs to sign in to the Office 365 admin portal as a Global admin.

2. Select **Settings** > **Partner relationships**.

3. On the **Partner relationships** page, the customer will see a list of the partners with whom they work and those that have been granted delegated administration privileges to their tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Customers can manage a partner's delegated admin privileges 

Your customer may decide to remove your delegated admin privileges from their tenant but retain the relationship with you for subscription and license renewal purposes. 고객은 Office 365 관리 센터의 **파트너 관계** 페이지에서 Office 365 계정에 대한 권한 및 사용 권한을 관리합니다. 이 페이지에서 고객은 다음을 수행할 수 있습니다.

- 관계를 맺고 있는 파트너 및 관리자 권한이 위임된 파트너 확인

- Remove a partner's delegated administration privileges from the tenant

파트너에게 위임된 관리 권한을 제거하려면 다음을 수행합니다.

1. **파트너 관계** 페이지에서 관심 파트너를 선택합니다.
2. 세부 정보 창에서 **위임된 관리자 제거**를 선택합니다.
3. 확인 창에서 **제거**를 선택합니다.

>[!IMPORTANT]  
>Azure AD 역할 할당은 암시적입니다. Azure AD Portal/PowerShell/Graph를 사용하여 Azure AD 역할의 구성원을 나열하려고 시도하는 경우 파트너가 반환되지 않습니다. 파트너가 Azure AD 역할에 할당되었는지 확인하려면 Office 365 관리자 포털의 파트너 관계 페이지를 참조하여 위임된 관리 권한이 파트너에게 부여되었는지 여부를 확인해야 합니다.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD의 위임된 관리자 권한 

There are two security groups, Admin Agents and Helpdesk Agents, in the partner's Azure AD tenant that are used for delegated administration. 고객이 파트너에게 위임된 관리 권한을 부여한 경우:

- The Admin Agent group is assigned to the Global Administrator role in the customer's Azure AD tenant.

- The Helpdesk Agent group is assigned to the Helpdesk Administrator role in the customer's Azure AD tenant.

Based on the directory roles assigned, members of both groups can sign in to the customer's Azure AD tenant and O365 services using their partner credentials and administrator on behalf of the customer.

If your customer removes delegated admin privileges, the Azure AD role assignments are removed, and you will no longer be able to manage the customer's Azure AD tenant.

### <a name="azure-subscriptions-and-resource-management"></a>Azure 구독 및 리소스 관리

각 Azure 구독에는 고유한 리소스 관리 역할 세트가 있습니다. Before a CSP partner can manage a customer's Azure subscription, the partner must be assigned to one or more roles under the Azure subscription. 특히 다음 사항에 주의하세요.

- 고객이 재판매인 초대를 수락하고 파트너에게 위임된 관리 권한을 부여하면 파트너는 고객 테넌트의 기존 Azure 구독에 자동으로 액세스하지 않습니다.

- CSP 파트너가 고객에게 새로운 Azure 구독을 제공하면 CSP 파트너 테넌트의 관리자 에이전트 그룹에 구독에 대한 소유자 역할이 자동으로 할당됩니다. 이 역할 할당을 기반으로 그룹 구성원은 구독에 따라 리소스에 액세스하고 이를 관리할 수 있습니다.

- When a customer removes delegated administration privileges from a partner using Office 365 Portal, the partner can still manage the customer's Azure subscription as long as the partner is still assigned to one or more roles under the subscription. 파트너의 Azure 구독 관리를 중지하려면 고객이 해당 역할 할당을 제거해야 합니다.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

From Partner Center, CSP partners can manage Autopilot profiles for their customers without delegated admin privileges under these circumstances: 

- If a customer removes delegated administration privileges but retains a reseller relationship with you, you can continue to manage Autopilot profiles for them.

- You can manage customer devices that you or another partner have added. 

- You can't manage devices your customer has added through the Microsoft Store for Business, Microsoft Store for Education, or Microsoft Intune Portal.

For more information about Autopilot, see [Simplify device setup with Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>The current Autopilot management experience in Partner Center might continue to change. At the time this article was published, the following changes are being considered:

- 파트너가 프로필을 추가/업데이트/제거하고 고객 테넌트의 모든 장치에서 프로필을 적용/제거하려면 파트너가 위임된 관리 권한을 고객에게 부여 받아야 합니다.

- Partner must be granted delegated administration privilege by the customer before the partner can remove devices added by other partners or by the customer in the customer tenant. Otherwise, the partner can remove only devices added previously by the same partner.
