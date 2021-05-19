---
title: 인센티브 FAQ
ms.topic: how-to
ms.date: 02/05/2021
description: Microsoft 인센티브에 대한 질문과 대답입니다. 이 문서에는 사용자 역할, 등록 방법 또는 오류 메시지에 대해 수행할 수 있는 방법에 대한 질문이 포함되어 있습니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: a917f3648447ac273fae839d32a4b4d3ce80ae35
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152021"
---
# <a name="frequently-asked-questions-on-incentives"></a>인센티브에 대한 질문과 대답

**적절한 역할:** 인센티브 관리자 | 인센티브 사용자

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>인센티브에 등록하려면 전역 관리자가 되어야 합니까?

아니요. 전역 관리자와 계정 관리자는 모두 사용자를 인센티브 관리자로 할당할 수 있습니다. 인센티브 관리자는 파트너 센터 통해 회사의 인센티브 프로그램을 관리합니다. 자세한 내용은 [사용 권한 개요를 참조하세요.](permissions-overview.md)

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>회사가 이미 MPN(Microsoft 파트너 네트워크)의 멤버인 경우 어떻게 해야 합니까?

MPN에 가입하려고 하고 회사가 이미 구성원인 경우 MPN은 도메인을 인식하고 기존 계정에 연결합니다. 기존 계정은 동일한 이메일 도메인을 사용하는 동일한 회사 또는 관련 회사이거나 여러 도메인을 관리하는 데 동일한 Azure AD(Azure Activity Directory)일 수 있습니다.

법적 프로필 페이지에서 기본 연락처를 식별할 수 있습니다. 위치가 MPNHQ 위치인 경우 인센티브 관리에 필요한 권한으로 설정하기만 하면 됩니다. 역할 및 권한에 대한 자세한 내용은 [사용 권한 개요를 참조하세요.](permissions-overview.md)

MPNHQ 위치와 동일한 국가에 있지 않은 경우 이 시나리오에 대한 자세한 내용은 다중 국가 계정 지침을 [참조하세요.](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso)

## <a name="what-user-roles-are-available"></a>사용할 수 있는 사용자 역할은 무엇인가요?

파트너 센터 회사를 등록하는 사람은 기본적으로 기본 연락처 및 전역 관리자가 됩니다. 관리자는 포털에서 사용자를 초대하고 관리할 수 있습니다.

인센티브의 주요 역할은 인센티브 관리자 및 인센티브 사용자입니다. 성과급 관리자는 동기 프로그램에 등록 하 고 파트너에 대 한 은행 및 세금 세부 정보를 관리할 수 있습니다. 성과급 사용자는 도구에서 보고서를 보고 지불 된 항목 및 각 지불의 분석을 확인할 수 있지만, 은행 정보를 보거나 편집할 수는 없습니다. 파트너 전역 계정의 모든 위치에 두 역할을 모두 적용할 수 있습니다.

자세한 내용은 [사용 권한 개요](permissions-overview.md)를 참조 하세요.

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>회사에 대 한 전역 또는 계정 관리자 권한이 있는 사용자를 어떻게 확인할 수 있나요?

역할을 변경 하거나 새 사용자에 게 역할을 할당할 수 있는 전역 관리자 또는 계정 관리자를 찾으려면 다음을 수행 합니다.

1. 파트너 센터의 오른쪽 위에 있는 계정 설정 아이콘에서 **사용자 관리** 를 선택 합니다.
2. **전역 관리자** 또는 **계정 관리자** 를 기준으로 필터링 할 수도 있습니다.
3. **내 프로필** 로 이동 하 고, **역할 및 사용 권한을** 선택 하 고, 사용 권한을 상승 시키는 데 도움이 되는 다양 한 관리자 목록을 볼 수도 있습니다.
 
자세한 내용은 [역할 찾기](find-your-role.md)를 참조 하십시오.  

## <a name="i-cant-access-incentives-using-my-credentials"></a>내 자격 증명을 사용 하 여 성과급에 액세스할 수 없습니다.

성과급을 볼 수 없는 이유는 올바른 권한이 없는 것입니다. 다음 절차를 사용 하 여 문제를 해결할 수 있습니다.

1. Azure AD 테 넌 트 자격 증명 (작업 자격 증명)을 사용 하 여 [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/) 로그인 합니다. 로그인 할 수 없는 경우 회사의 전역 관리자에 게 문의 하세요.

2. 로그인 할 때 **회사 계정이** 나 **개인 계정을** 선택 하 라는 메시지가 표시 되 면 **회사 계정** 을 선택 합니다.

3. 파트너 센터 메뉴에서 **성과급** 을 선택 하 고 **개요** 를 선택 합니다. 성과급 관리자 또는 성과급 사용자 권한이 없는 경우 회사의 모든 전역 및 계정 관리자에 대 한 연락처 정보가 표시 됩니다. 이러한 관리자 중 한 명에 게 문의 하 여 필요한 MPN Id 및 동기 프로그램에 대 한 동기 역할을 얻으십시오.

4. 성과급 관리자 역할이 이미 있는 경우 액세스 권한이 있는 MPN Id 및 동기 프로그램에 대 한 회사의 등록이 표시 됩니다.

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>성과급 개요 페이지에 일부 등록 없습니다.

대시보드에 더 이상 표시 되지 않는 동기 프로그램이 있는 초대를 수신 했거나 등록 한 경우 적절 한 액세스 권한이 있는지 다시 확인 해야 합니다. 동기 사용자 또는 동기 관리자 역할을 가진 사용자만이 프로그램을 볼 수 있습니다. [역할 찾기](./find-your-role.md)를 참조 하세요.

역할 또는 권한을 변경 해야 하는 경우 회사의 전역 또는 계정 관리자에 게 문의 하세요. 이러한 사람에 대 한 자세한 내용은 [전역 관리자 찾기](./find-your-role.md#find-your-global-admin)를 참조 하세요.

개요 페이지에는 Azure AD 테 넌 트와 연결 된 파트너 전역 계정 (표준)과 연결 된 등록만 표시 됩니다. 회사에 둘 이상의 요소가 있는 경우 각각에 대해 서로 다른 자격 증명을 포함 해야 합니다.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>등록 프로세스 중에 오류 메시지가 표시 되거나 도움이 필요한 경우 누구에 게 연락 해야 하나요?

대시보드의 성과급 섹션 내에서 문제가 발생 하는 경우 온라인 지원 서비스가 있습니다. 지원 옵션을 참조 하세요 (? 아이콘)을 마우스 오른쪽 단추로 이동 합니다.

## <a name="next-steps"></a>다음 단계

- [인센티브 시작](incentives-get-started-intro.md)