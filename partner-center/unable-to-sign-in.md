---
title: 파트너 센터에 로그인 할 수 없습니다.
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 가능한 원인 문제를 해결 하 고 파트너 센터에 로그인 할 수 없는 경우에 대 한 해결 방법-암호 재설정, 역할 확인 및 자격 증명 확인에 대해 자세히 알아보세요.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266574"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>파트너 센터의 로그인 문제 해결

**적절한 역할**

- 파트너 센터에 관심이 있는 모든 파트너

이 문서에는 파트너 센터에 대 한 일반적인 로그인 문제에 대 한 솔루션이 포함 되어 있습니다.

## <a name="youve-forgotten-your-password-for-partner-center"></a>파트너 센터에 대 한 암호를 잊어버린 경우

암호를 잊은 경우 파트너 센터에 로그인 할 수 없는 경우 지원 담당자에 게 문의 하세요. [비즈니스 제품 지원](/microsoft-365/admin/contact-support-for-business-products)에서 적절 한 연락처를 찾습니다.

MPN 파트너 라면 전역 관리자에 게 새 암호를 만들도록 요청 하세요. CSP 간접 재판매인 인 경우 간접 공급자에 게 문의 하 여 Azure AD 테 넌 트에 대 한 새 전역 관리자를 만들거나 위임 된 관리자 권한을 사용 하 여 새 암호를 만듭니다.

암호를 재설정 하 고 회사 계정에 대 한 액세스 권한을 다시 얻는 방법에 대해 자세히 알아보려면 [보안 정보를 사용 하 여 회사 또는 학교 암호 재설정](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)을 참조 하세요.

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>파트너 센터에서 예상 페이지 또는 기능을 보거나 관리할 수 없습니다.

파트너 센터의 페이지에 대 한 액세스는 할당 된 역할에 의해 제어 됩니다. 할당 된 역할을 확인 하려면 파트너 센터에서 설정 아이콘을 선택 하 고 **계정 설정** 을 선택한 다음 계정 설정에서 **사용자 관리** 를 선택 합니다. 검색에서 이름을 입력 한 다음 결과를 확인 합니다.

원하는 역량, 고객, 성과급 또는 사용자를 보거나 관리할 수 없는 경우 다음 해결 방법을 시도해 보세요.

- MPN, CSP 및 조회의 기능에 액세스 하려면 전역 관리자 또는 계정 관리자에 게 문의 하세요. 파트너 센터에서 사용할 수 있는 역할 및 작업에 대 한 자세한 내용은 [사용자에 게 역할 할당 & 권한](permissions-overview.md)을 참조 하세요.
- 상용 Marketplace 및 Windows & Xbox, Office 스토어, Microsoft Edge 및 하드웨어 개발자 프로그램의 기능에 액세스 하려면 조직의 소유자 또는 관리자 역할을 담당 하는 사용자에 게 문의 하세요. 역할 및 권한에 대 한 자세한 내용은 [Microsoft 파트너 센터에서 상업적 marketplace 계정을 관리 하는 방법](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)을 참조 하세요.

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>파트너 센터에서 제안 또는 혜택을 볼 수 없습니다.

올바른 자격 증명을 사용 하 여 로그인 했는지 확인 합니다. 예를 들어, 회사 계정과 개인 계정은 같은 것 처럼 보일 수 있지만 하나는 사용자가 abc@contoso.com 만든 개인 계정일 수 있으며 다른 계정은 사용자를 대신 하 여 설정 된 비즈니스 계정일 수 있습니다. 이 경우 로그인 했지만 MPN, CSP, 상용 Marketplace와 관련 된 예상 기능을 볼 수 없는 경우 회사 계정을 선택 해 보세요.

## <a name="next-steps"></a>다음 단계

- [계정 정보 확인](verification-responses.md)
- [암호 다시 설정하기](reset-my-pasword.md)
- [사용자 암호 다시 설정](reset-a-user-password.md)