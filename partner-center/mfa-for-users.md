---
title: 다단계 인증을 사용하여 사용자 설정
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: MFA를 사용하여 직원을 설정하는 방법 알아보기
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450810"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>다단계 인증을 사용하여 사용자 설정

**적절한 역할**: 전역 관리자

개인 정보 보호 및 보안 강화는 최우선 순위입니다. 최선의 방어는 예방이며, 가장 약한 링크를 강화해야 한다는 것을 알고 있습니다. 따라서 에코시스템의 모든 사람이 조치를 취하고, 적절한 보안 보호가 마련되어야 합니다. 모든 파트너가 파트너 테넌트의 사용자에 대해 MFA(다단계 인증)를 사용하도록 설정하는 것이 좋습니다. 

## <a name="add-multi-factor-authentication-for-your-users"></a>사용자에 대한 다단계 인증 추가

이 작업을 완료하려면 회사의 전역 관리자여야 합니다.

Azure AD 테넌트에 사용자를 추가할 때 사용자에 대한 MFA를 사용하는 것이 가장 쉽습니다.

1. [Azure Portal](https://portal.azure.com)에 로그인한 후 **사용자 관리** 로 이동합니다.
1. **다단계 인증** 을 선택합니다.
1. 사용하도록 설정하려는 사용자를 선택한 후 **사용** 을 선택합니다.

그러면 이 사용자에 대한 MFA가 설정됩니다. 사용하도록 설정되면 사용자가 처음으로 로그인할 때 MFA 확인을 설정하라는 메시지가 표시됩니다. 이후에는 로그인 시 이메일 또는 문자 메시지(설정에 따라 다름)를 통해 전송된 코드를 입력하라는 메시지가 표시됩니다.  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="확인 방법 지정.":::

>[!NOTE]
>위와 동일한 단계를 사용하고 **적용** 을 선택하여 사용자가 MFA를 사용하도록 **강제** 할 수 있습니다. 자세한 내용은 [사용자별 Azure Multi-Factor Authentication을 사용하여 로그인 이벤트 보호](/azure/active-directory/authentication/howto-mfa-userstates)를 참조하세요. 

모든 사용자는 처음에  **사용 안 함** 으로 설정되어 있습니다. 사용자별 Azure Active Directory Multi-Factor Authentication에 사용자를 등록하면 해당 사용자의 상태가  **사용** 으로 변경됩니다. 사용하도록 설정된 사용자가 로그인하고 등록 프로세스를 완료하면 해당 사용자의 상태가  **적용됨** 으로 변경됩니다. 

## <a name="next-steps"></a>다음 단계

- [사용자에게 역할 및 사용 권한 할당](permissions-overview.md)