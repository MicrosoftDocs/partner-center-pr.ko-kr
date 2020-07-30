---
title: 파트너 센터 계정에 테 넌 트 추가
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 계정을 통해 여러 테 넌 트 관리
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389518"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>파트너 센터 계정에서 여러 테 넌 트 추가 및 관리

**적용 대상**

- 파트너 센터

**적절한 역할**

- 글로벌 관리자

파트너 센터 계정에서 여러 Azure AD 테 넌 트를 관리 해야 하는 이유는 여러 가지가 있습니다. 예를 들어 회사에서 다른 회사를 구매 하 고 새 회사의 직원이 파트너 센터를 사용할 수 있도록 하려고 합니다. 그러나 두 회사를 분리 하는 것이 좋습니다. 이 경우 새 회사의 Azure AD 테 넌 트를 파트너의 PNG (global account)와 연결 합니다. 이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.

## <a name="add-another-azure-ad-tenant-to-your-account"></a>계정에 다른 Azure AD 테 넌 트 추가

1. 전역 관리자 권한으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인 합니다.
1. **설정** 아이콘에서 **계정 설정** 을 선택 하 고 **테 넌 트**를 선택 합니다.
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="테 넌 트 연결"::: 

3. **다른 AD 테 넌 트 연결** 을 선택 하 고 연결 하려는 테 넌 트를 지정 합니다.

1. 전역 관리자 권한으로 연결 하려는 테 넌 트에 로그인 하 고 연결을 확인 합니다. 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="테 넌 트 연결 확인"::: 

5. 확인 한 후에는 **모든 설정** 된 알림이 표시 됩니다.  **테 넌 트 관리로 돌아가기** 를 선택 하면 새로 추가 된 테 넌 트가 나열 됩니다.
 
## <a name="next-steps"></a>다음 단계

- [사용자 추가](create-user-accounts-and-set-permissions.md)
