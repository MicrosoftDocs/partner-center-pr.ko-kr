---
title: 파트너 센터 계정 설정 또는 MPN 갱신 문제 해결
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 파트너 센터 등록하려고 할 때의 문제를 해결합니다. 답변은 결제 방법, 암호 잊기 등의 문제를 해결합니다.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686265"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>계정 설정 또는 MPN 갱신 문제 해결


**적절한 역할**

- 글로벌 관리자
- MPN 파트너 관리자
 
다음은 파트너 센터 계정을 설정하는 경우 발생하는 일반적인 문제를 해결하기 위한 몇 가지 제안 사항입니다.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Partner Membership Center 마이그레이션하고 회사 정보 필드를 편집할 수 없는 경우 어떻게 되나요?

회사가 이미 파트너 센터 있는 경우(예: CSP 계정) 읽기 전용 화면이 표시됩니다. 이 화면에는 회사에 대한 모든 정보가 파트너 센터 표시됩니다.

이 화면에서는 세부 정보를 변경할 수 없습니다. 이는 오류가 아니라 의도적으로 한 것입니다.

**수락** 및 **계속을** 선택하여 계속합니다.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT 부서에서 **파트너 센터 등록을** 해제한 경우

바이럴 사용자가 비활성화되거나 Azure AD 테넌트에서 바이럴 등록이 비활성화되어 있으므로 이 메시지가 표시됩니다. Azure AD 계정의 전역 관리자는 다음 PowerShell 명령을 실행하여 필요한 기능을 사용하도록 설정할 수 있습니다.

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

자세한 내용은 [셀프 서비스 등록을 읽어보십시오.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>암호를 잊어버렸습니다.

암호를 잊어버린 경우 로그인 페이지에서 **계정에 액세스할 수 없나요?** 링크를 선택합니다. 이 옵션을 사용하면 암호를 재설정하거나 전역 관리자에게 새 자격 증명을 할당하도록 요청할 수 있습니다.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>"회사에 대해 알려주세요" 화면에서 "문제가 발생했습니다." 오류가 표시됩니다.

회사 전화 번호에서 특수 문자, 공백 또는 국가 코드를 실수로 사용 하는 경우이 오류 메시지는 일반적으로 표시 됩니다. 전화 번호 필드에 입력 한 값은 최대 10 자만 포함할 수 있습니다.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>신용 카드 구입 시 "주문이 거부 되었습니다." 라는 오류 메시지가 표시 됩니다. 정보를 확인 하세요. "


항상 법적 엔터티가 아닌 신용 카드에 해당 하는 주소를 사용 합니다. 또한 우편 번호가 올바르고 사용 하는 주소에 해당 하는지 확인 합니다.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>오프 라인 결제에서 온라인 지불 방법으로 전환 하려고 합니다. 

원래 주문을 취소 하 고 기본 결제 방법을 사용 하 여 다시 구매 해야 합니다.

주문을 취소 하려면:

1. 대시보드에서 **멤버 자격 제안** 탭을 선택 합니다.

2. **취소 순서** 선택

3. 확인 창이 표시 되 고 초기 주문을 취소 하기 위해 확인 해야 합니다.

## <a name="next-steps"></a>다음 단계

- [파트너 센터 계정 관리](partner-center-account-setup.md)
- [청구서 및 정찰 파일을 읽는 방법](read-your-bill.md)
