---
title: 파트너 센터 계정에 테 넌 트 추가
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 계정에서 여러 Azure AD 테 넌 트를 추가, 통합 또는 관리 하는 방법을 알아봅니다. 또한이 작업을 수행 하는 몇 가지 이유에 대해 알아보세요.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175165"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>파트너 센터 계정에서 여러 테 넌 트 추가 및 관리

**적용 대상**

- 파트너 센터

**적절한 역할**

- 글로벌 관리자

이 기능을 사용하여 회사의 여러 테넌트를 관리하고 파트너 센터 계정에 통합할 수 있습니다. 파트너 센터 계정에서 여러 Azure AD 테 넌 트를 관리 해야 하는 이유는 여러 가지가 있습니다. 예를 들면 다음과 같습니다.

- 회사에서 다른 회사를 구입할 수 있으며, 새 회사 직원 들이 파트너 센터를 사용할 수 있도록 하려고 합니다. 그러나 두 회사를 분리 하는 것이 좋습니다. 이 경우 새 회사의 Azure AD 테 넌 트를 파트너의 글로벌 계정 (표준)과 연결 합니다. 이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.

- 비즈니스를 실행 하는 데 둘 이상의 테 넌 트가 있는 경우 (예: contoso.com, contoso.uk, contoso.in) 다중 테 넌 트를 사용 하 여 동일한 PC 계정에 연결할 수 있습니다.

- 인수를 합병 하려면 둘 이상의 테 넌 트를 사용 해야 합니다 (예: Contoso가 Fabrikam을 획득 하는 경우 Constoso.com 및 Fabrikam.com 각 테 넌 트를 모두 사용할 수 있어야 함).

- 테 넌 트의 사용자는 다음을 수행할 수 있어야 합니다.
    1.  교육, 디지털 다운로드, MCP 연결을 위한 파트너 센터 액세스
    2.  MPN Admin, 성과급 관리자 등과 같은 파트너 센터 역할을 할당 받아야 합니다.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>계정에 다른 Azure AD 테 넌 트 추가

1. 전역 관리자 권한으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인 합니다.
1. **설정** 아이콘에서 **계정 설정** 을 선택 하 고 **테 넌 트**를 선택 합니다.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="테 넌 트 연결"::: 

3. **다른 AD 테 넌 트 연결** 을 선택 하 고 연결 하려는 테 넌 트를 지정 합니다.

1. 전역 관리자 권한으로 연결 하려는 테 넌 트에 로그인 하 고 연결을 확인 합니다. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="테 넌 트 연결"::: 

5. 확인 한 후에는 **모든 설정** 된 알림이 표시 됩니다.  **테 넌 트 관리로 돌아가기** 를 선택 하면 새로 추가 된 테 넌 트가 나열 됩니다. 
 

>[!NOTE]
>다른 파트너 센터 계정에 이미 연결 되어 있는 경우에는 테 넌 트를 계정에 연결할 수 없습니다.

 
## <a name="next-steps"></a>다음 단계

- [사용자 추가](create-user-accounts-and-set-permissions.md)
