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
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848950"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>계정 설정 또는 MPN 갱신 문제 해결

### <a name="applies-to"></a>적용 대상

- 파트너 센터
 
### <a name="appropriate-roles"></a>적절한 역할

- 글로벌 관리자
- MPN 파트너 관리자 
 

파트너 센터 계정을 설정할 때 발생 하는 일반적인 문제를 해결 하기 위한 몇 가지 제안 사항은 다음과 같습니다.

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>파트너 구성원 센터에서 마이그레이션하는 경우에는 어떻게 되나요? 회사 정보 필드는 편집할 수 없습니다.

이는 파트너가 파트너 센터에 이미 있는 경우 (예를 들어, CSP 계정), 회사에 대 한 모든 정보가 파트너 센터에 존재 하는 것으로 표시 되는 읽기 전용 화면을 표시 하는 경우에 발생 합니다.

이 화면에서는 세부 정보를 변경할 수 없습니다. 이것은 의도적 이며 오류가 아닙니다.

**수락** 을 선택 하 고 **계속** 진행 합니다.

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>등록 하려고 하거나 파트너 구성원 센터에서 마이그레이션해야 하는 경우, IT 부서가 **파트너 센터에 등록**해제 되었다는 오류 메시지가 표시 됩니다. 

바 이럴 사용자가 사용 하지 않도록 설정 되어 있거나, Azure AD 테 넌 트에서 바 이럴 등록을 사용할 수 없기 때문에이 메시지가 표시 됩니다. Azure AD 계정에 대 한 전역 관리자는 다음 PowerShell 명령을 실행 하 여 필요한 기능을 사용 하도록 설정할 수 있습니다.

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

자세한 내용은 [셀프 서비스 등록](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) 을 참조 하세요.

### <a name="you-forgot-your-password"></a>암호를 잊은 경우

암호를 잊은 경우 로그인 페이지에서 계정에 **액세스할 수 없습니까?** 링크를 선택 하 여 암호를 재설정 하거나 전역 관리자에 게 새 자격 증명을 할당 하도록 요청할 수 있습니다.

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>"회사에 대해 알려주세요." 화면에서 "오류가 발생 했습니다." 오류가 표시 됩니다.

이는 일반적으로 회사 전화 번호에서 특수 문자, 공백 또는 국가 코드를 실수로 사용 하는 경우에 발생 합니다. 전화 번호 필드에 입력 한 값은 최대 10 자만 포함할 수 있습니다.

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>신용 카드를 통해 구매를 완료 하려고 했지만 "주문이 거부 되었습니다." 라는 오류 메시지가 표시 됩니다. 정보를 확인 하세요. "

항상 신용 카드에 해당 하는 주소를 삽입 해야 하며 법적 엔터티에 해당 하는 것은 아닙니다. 또한 우편 번호가 올바르고 사용 하는 주소에 해당 하는지 확인 합니다.

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>오프 라인 결제에서 온라인 지불 방법으로 전환 하려고 합니다. 

원래 주문을 취소 하 고 기본 결제 방법을 사용 하 여 다시 구매 해야 합니다.

주문을 취소 하려면:

1. 대시보드에서 **멤버 자격 제안** 탭을 선택 합니다.

2. **취소 순서** 선택

3. 확인 창이 표시 되 고 초기 주문을 취소 하기 위해 확인 해야 합니다.
