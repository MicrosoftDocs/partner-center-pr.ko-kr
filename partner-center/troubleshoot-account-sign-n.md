---
title: 파트너 센터 계정 설정 또는 MPN 갱신 문제 해결
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 파트너 센터에서 등록 문제 해결
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 58acef4599333929446a283ecde1cca9f3ef9ce8
ms.sourcegitcommit: 983457c8e8fcfbfe48b80b1c86fe894c1e106eb3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/03/2020
ms.locfileid: "89443589"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>계정 설정 또는 MPN 갱신 문제 해결

**적용 대상**

- 파트너 센터
 
**적절한 역할**

- 글로벌 관리자
- MPN 파트너 관리자 
 
파트너 센터 계정을 설정할 때 발생 하는 일반적인 문제를 해결 하기 위한 몇 가지 제안 사항은 다음과 같습니다.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>파트너 구성원 센터에서 마이그레이션하는 경우에는 어떻게 되나요? 회사 정보 필드는 편집할 수 없습니다.

파트너가 파트너 센터에 이미 있는 경우 (예를 들어, CSP 계정) 회사에 대 한 모든 정보가 파트너 센터에 있는 것 처럼 표시 되는 읽기 전용 화면이 표시 됩니다.

이 화면에서는 세부 정보를 변경할 수 없습니다. 이것은 의도적 이며 오류가 아닙니다.

**수락** 을 선택 하 고 **계속** 진행 합니다.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT 부서가 **파트너 센터 등록을 해제 한**경우


바 이럴 사용자가 사용 하지 않도록 설정 되어 있거나, Azure AD 테 넌 트에서 바 이럴 등록을 사용할 수 없기 때문에이 메시지가 표시 됩니다. Azure AD 계정에 대 한 전역 관리자는 다음 PowerShell 명령을 실행 하 여 필요한 기능을 사용 하도록 설정할 수 있습니다.

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

자세한 내용은 [셀프 서비스 등록](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) 을 참조 하세요.

## <a name="you-forgot-your-password"></a>암호를 잊은 경우

암호를 잊은 경우 로그인 페이지에서 계정에 **액세스할 수 없습니까?** 링크를 선택 하 여 암호를 재설정 하거나 전역 관리자에 게 새 자격 증명을 할당 하도록 요청할 수 있습니다.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>"회사에 대해 알려주세요." 화면에서 "오류가 발생 했습니다." 오류가 표시 됩니다.

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