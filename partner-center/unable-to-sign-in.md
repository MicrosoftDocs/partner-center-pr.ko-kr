---
title: 파트너 센터 로그인할 수 없음
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 가능한 원인을 해결하고 파트너 센터 로그인할 수 없는 경우에 대한 해결 방법을 알아봅니다. 암호 재설정, 역할 확인 및 자격 증명 확인에 대해 자세히 알아보세요.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2b67201355e748f9280d28413a8737a9b07db5c6
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431492"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>파트너 센터 로그인 문제 해결

**적절한 역할:** 파트너 센터 관심이 있는 모든 파트너

이 문서에는 파트너 센터 일반적인 로그인 문제에 대한 솔루션이 포함되어 있습니다.

## <a name="youve-forgotten-your-password-for-partner-center"></a>파트너 센터 암호를 잊어버렸습니다.

암호를 잊어서 파트너 센터 로그인할 수 없는 경우 지원에 문의하세요. 비즈니스 제품 지원 에서 적절한 [연락처를 찾습니다.](/microsoft-365/admin/contact-support-for-business-products)

MPN(Microsoft 파트너 네트워크) 파트너인 경우 전역 관리자에게 새 암호를 만들도록 요청합니다. CSP(클라우드 솔루션 공급자) 간접 대리점인 경우 간접 공급자에게 AD(Azure Active Directory) 테넌트에서 새 전역 관리자를 만들거나 위임된 관리자 권한을 사용하여 새 암호를 만들도록 요청합니다.

암호를 재설정하고 작업 계정에 대한 액세스 권한을 다시 받을 수 있는 방법에 대한 자세한 내용은 [보안 정보를 사용하여 직장 또는 학교 암호 재설정을 참조하세요.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>파트너 센터 예상 페이지 또는 기능을 보거나 관리할 수 없습니다.

파트너 센터 페이지에 대한 액세스는 할당된 역할에 의해 제어됩니다. 할당된 역할을 확인하려면 파트너 센터 설정 아이콘을 선택하고 **계정 설정** 을 선택한 다음 계정 설정에서 **사용자 관리를** 선택합니다. 검색에서 이름을 입력한 다음 결과를 확인합니다.

원하는 역량, 고객, 인센티브 또는 사용자를 보거나 관리할 수 없는 경우 다음 솔루션을 사용해 보세요.

- MPN, CSP 및 조회 기능에 액세스하려면 전역 관리자 또는 계정 관리자에게 문의하세요. 역할 및 파트너 센터 사용하도록 설정하는 작업에 대한 자세한 내용은 [사용자에게 역할 & 권한 할당을 참조하세요.](permissions-overview.md)
- 상업용 Marketplace 및 Windows & Xbox, Office Store, Microsoft Edge 및 하드웨어 개발자 프로그램의 기능에 액세스하려면 조직의 소유자 또는 관리자 역할에 있는 사람에게 문의하세요. 역할 및 권한에 대한 자세한 내용은 [Microsoft 파트너 센터 상업용 Marketplace 계정을 관리하는 방법을](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)참조하세요.

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>파트너 센터 제안 또는 혜택을 볼 수 없습니다.

올바른 자격 증명을 사용하여 로그인하고 있는지 확인합니다. 예를 들어 작업 및 개인 계정은 동일하게 보일 수 있지만(예: abc@contoso.com ) 하나는 직접 만든 개인 계정일 수 있고 다른 하나는 사용자 대신 설정된 비즈니스 계정일 수 있습니다. 이 경우 로그인했지만 MPN, CSP, 상업용 Marketplace와 관련된 예상 기능을 볼 수 없는 경우 작업 계정을 선택해 보세요.

## <a name="next-steps"></a>다음 단계

- [계정 정보 확인](verification-responses.md)
- [암호 다시 설정하기](reset-my-pasword.md)
- [사용자 암호 다시 설정](reset-a-user-password.md)