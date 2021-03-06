---
title: 고객의 관리자 권한 얻기
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객의 서비스 또는 구독을 대신 관리하는 데 필요한 권한을 얻습니다. 권한 부여, 해지 및 관리 방법에 대해 알아봅니다.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 779e76d6bb3e8df679a5ca6fa8ce441e42529161
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147295"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>고객의 서비스 또는 구독을 관리하는 권한 얻기

**적절한 역할**: 관리 에이전트 | 영업 에이전트

고객을 대신하여 고객 서비스 또는 구독을 관리하려면 고객이 해당 서비스에 대한 관리자 권한을 부여해야 합니다. 고객으로부터 관리자 권한을 얻으려면 고객에게 이메일로 재판매인 관계 요청을 보내야 합니다. 고객이 요청을 승인하면 해당 서비스의 관리 포털에 로그인하여 고객 대신 서비스를 관리할 수 있습니다. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>귀사와 재판매인 관계를 맺도록 고객 초대

1.  **고객** 을 선택한 다음, **재판매인 관계 요청** 을 선택합니다.

2.  다음 페이지에서 임시 이메일 메시지를 검토합니다. 기본 이메일 애플리케이션에서 초안 메시지를 열거나 메시지를 클립보드에 복사하여 이메일에 붙여넣을 수 있습니다. 

    >[!IMPORTANT]
    >이메일에서 텍스트를 편집할 수 있지만, 이메일에 링크를 포함하는 것을 잊지 마세요. 이 링크는 고객을 귀사의 계정에 직접 연결하는 맞춤형 링크입니다. 
    
3.  이 단계를 마쳤으면 **완료** 를 선택합니다.

4.  고객에게 이메일을 보냅니다.

5.  고객이 초대를 수락하면 **고객** 페이지에 고객이 표시되고, 여기서 고객의 서비스를 프로비저닝하고 관리할 수 있습니다.

6.  고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장한 다음, 관리하려는 서비스의 관리 포털을 선택합니다.

>[!IMPORTANT]  
>고객이 서비스의 관리 포털에서 관리자 권한을 다시 할당하거나 제거할 수 있습니다. 그러나 관리자 권한을 제거하면 더 이상 고객을 대신하여 Microsoft에 서비스 요청을 제출할 수 없다는 것을 고객에게 알려야 합니다. 고객과 계약을 다시 협상하기 전에는 고객을 대신하여 이러한 유형의 서비스 요청을 열 수 없습니다.

고객은 Office 365 관리 포털에서 테넌트에 대한 관리자 권한을 가진 파트너를 찾을 수 있습니다. 이렇게 하려면 다음을 수행합니다.

1. 고객은 Office 365 관리 포털에 글로벌 관리자로 로그인해야 합니다.

2. **설정** > **파트너 관계** 를 선택합니다.

3. **파트너 관계** 페이지에 고객과 협력 관계에 있는 파트너 및 테넌트에 대한 관리 권한이 위임된 파트너 목록이 표시됩니다.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>고객이 파트너의 위임된 관리자 권한을 관리할 수 있음 

고객은 테넌트에서 파트너에게 위임된 관리자 권한을 제거할 수 있으며, 이 경우에도 구독 및 라이선스 갱신 목적으로 파트너와의 관계를 계속 유지할 수 있습니다. 고객은 Office 365 관리 센터의 **파트너 관계** 페이지에서 Office 365 계정에 대한 권한 및 사용 권한을 관리합니다. 이 페이지에서 고객은 다음을 수행할 수 있습니다.

- 관계를 맺고 있는 파트너 및 관리자 권한이 위임된 파트너 확인

- 파트너에게 위임된 테넌트 관리 권한 제거

파트너에게 위임된 관리 권한을 제거하려면 다음을 수행합니다.

1. **파트너 관계** 페이지에서 원하는 파트너를 선택합니다.
2. 세부 정보 창에서 **위임된 관리자 제거** 를 선택합니다.
3. 확인 창에서 **제거** 를 선택합니다.

>[!IMPORTANT]  
>파트너에 대한 Azure AD 역할 할당은 암시적입니다. Azure AD Portal/PowerShell/Graph를 사용하여 Azure AD 역할의 구성원을 나열하려고 시도하면 파트너가 반환되지 않습니다. 파트너가 Azure AD 역할에 할당되었는지 확인하려면 Office 365 관리자 포털의 파트너 관계 페이지를 참조하여 위임된 관리 권한이 파트너에게 부여되었는지 여부를 확인해야 합니다.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD의 위임된 관리자 권한 

위임된 관리에 사용되는 파트너의 Azure AD 테넌트에는 관리자 에이전트 및 기술 지원팀 에이전트의 두 가지 보안 그룹이 있습니다. 고객이 파트너에게 위임된 관리 권한을 부여한 경우:

- 관리자 에이전트 그룹은 고객의 Azure AD 테넌트에서 글로벌 관리자 역할로 할당됩니다.

- 기술 지원팀 에이전트 그룹은 고객의 Azure AD 테넌트에서 기술 지원팀 관리자 역할로 할당됩니다.

할당된 디렉토리 역할에 따라 두 그룹의 구성원은 고객을 대신하여 파트너 자격 증명 및 관리자를 사용해서 고객의 Azure AD 테넌트 및 O365 서비스에 로그인할 수 있습니다.

고객이 위임된 관리자 권한을 제거하면 Azure AD 역할 할당이 제거되고 파트너는 더 이상 고객의 Azure AD 테넌트를 관리할 수 없습니다.

### <a name="azure-subscriptions-and-resource-management"></a>Azure 구독 및 리소스 관리

각 Azure 구독에는 고유한 리소스 관리 역할 세트가 있습니다. CSP 파트너가 고객의 Azure 구독을 관리하려면 해당 파트너는 Azure 구독에 속한 하나 이상의 역할에 할당되어야 합니다. 특히 다음 사항에 주의하세요.

- 고객이 재판매인 초대를 수락하고 파트너에게 위임된 관리 권한을 부여해도 고객 테넌트의 기존 Azure 구독에 대한 액세스 권한이 파트너에게 자동으로 부여되지 않습니다.

- CSP 파트너가 고객에게 새로운 Azure 구독을 제공하면 CSP 파트너 테넌트의 관리자 에이전트 그룹에 구독에 대한 소유자 역할이 자동으로 할당됩니다. 이 역할 할당을 기반으로 그룹 구성원은 구독의 리소스에 액세스하고 관리할 수 있습니다.

- 고객이 Office 365 Portal을 사용하여 파트너의 위임된 관리 권한을 제거해도 파트너는 구독에 속한 하나 이상의 역할에 할당되어 있는 한 고객의 Azure 구독을 관리할 수 있습니다. 파트너의 Azure 구독 관리를 중지하려면 고객이 해당 역할 할당을 제거해야 합니다.

## <a name="windows-autopilot"></a>Windows Autopilot

다음과 같은 상황에서 CSP 파트너는 위임된 관리자 권한 없이 파트너 센터에서 고객의 Autopilot 프로필을 관리할 수 있습니다. 

- 고객이 위임된 관리 권한을 제거하지만 재판매인 관계를 유지하는 경우 파트너는 고객의 Autopilot 프로필을 계속 관리할 수 있습니다.

- 파트너는 자신 또는 다른 파트너가 추가한 고객 디바이스를 관리할 수 있습니다. 

- 파트너는 고객이 비즈니스용 Microsoft Store, 교육용 Microsoft Store 또는 Microsoft Intune 포털을 통해 추가한 디바이스를 관리할 수 없습니다.

Autopilot에 대한 자세한 내용은 [Windows Autopilot으로 디바이스 설치 간소화](autopilot.md)를 참조하세요.

>[!IMPORTANT]  
>파트너 센터의 현재 Autopilot 관리 환경은 지속적으로 변경될 것입니다. 이 문서가 게시된 시점을 기준으로 다음과 같은 변경 사항을 고려 중입니다.

- 파트너가 프로필을 추가/업데이트/제거하고 고객 테넌트의 모든 디바이스에서 프로필을 적용/제거하려면 고객이 파트너에게 위임된 관리 권한을 부여해야 합니다.

- 파트너가 고객 테넌트에서 다른 파트너 또는 고객이 업로드한 디바이스를 제거하려면 고객이 파트너에게 위임된 관리 권한을 부여해야 합니다. 그렇지 않으면 파트너는 이전에 동일한 파트너가 추가한 디바이스만 제거할 수 있습니다.
