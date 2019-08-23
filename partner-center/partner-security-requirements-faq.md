---
title: 파트너 보안 요구 사항 FAQ | 파트너 센터
ms.topic: article
ms.date: 07/18/2019
description: 파트너 보안 요구 사항에 대 한 질문과 대답
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급 업체, CPV, multi-factor authentication, MFA, 보안 응용 프로그램 모델, 보안 앱 모델, 보안
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820593"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>파트너 보안 요구 사항에 대 한 질문과 대답

이 문서에는 [파트너 보안 요구 사항](partner-security-requirements.md)에 대 한 몇 가지 질문과 대답이 포함 되어 있습니다.

## <a name="partner-security-requirements"></a>파트너 보안 요구 사항

### <a name="what-are-the-new-partner-security-requirements"></a>새로운 파트너 보안 요구 사항은 무엇 인가요?

파트너와 고객을 보호 하기 위해 파트너는 다음과 같은 작업을 즉시 수행 해야 합니다.  

1. **파트너 테 넌 트의 모든 사용자에 대해 MFA (Multi-factor Authentication)를 사용 하도록 설정**합니다. 파트너 테 넌 트의 모든 사용자는 파트너 센터 또는 Api를 통해 Microsoft 상용 클라우드 서비스 또는 공급자에 로그인 할 때 MFA (Multi-factor Authentication)를 사용 해야 합니다. 기본 보호 정책의 사용을 통해 MFA는 파트너 테 넌 트의 모든 사용자에 게 무료로 제공 됩니다.

2. **보안 응용 프로그램 모델 프레임 워크를 채택**합니다. Azure Resource Manager, Microsoft Graph 및 파트너 센터 API와 같은 Microsoft API와 통합 되는 모든 파트너는 보안 응용 프로그램 모델 프레임 워크를 채택 하 여 기준 정책을 사용 하는 경우 통합이 중단 되지 않도록 해야 합니다. 
 
MFA (Multi-factor Authentication)를 사용 하도록 설정 하 고 보안 응용 프로그램 모델 프레임 워크를 사용 하면 인프라를 보호 하 고 도난 또는 기타 사기 행위를 식별 하는 등의 잠재적인 보안 위험 으로부터 고객의 데이터를 보호할 수 있습니다.  

### <a name="which-partners-need-to-meet-the-requirements"></a>요구 사항을 충족 해야 하는 파트너는 무엇 인가요?

이러한 요구 사항은 다음과 같은 파트너 그룹에 대 한 것입니다.
- Microsoft 상용 클라우드 서비스를 사용 하 여 거래 하는 CSP (클라우드 솔루션 공급자) 프로그램에 참여 하는 모든 파트너 조직
  - 직접 청구 파트너
  - 간접 공급자
  - 간접 재판매인
- 모든 제어판 공급 업체
- 모든 Advisor 프로그램 파트너  

소 버린 클라우드 (21Vianet, 미국 정부 및 독일)를 통해 거래 하는 모든 파트너는 8 월 1 일부 터 새로운 보안 요구 사항을 충족 하는 데 필요 하지 않습니다. 그러나 소 버린 클라우드를 사용 하는 모든 파트너는 이러한 새 보안 요구 사항을 즉시 적용 하 고 채택 하는 것이 좋습니다. Microsoft는 나중에 소 버린 클라우드에 대해 이러한 보안 요구 사항을 적용 하는 것과 관련 된 추가 세부 정보를 제공 합니다.

### <a name="what-are-the-key-timelines-and-milestones"></a>핵심 타임 라인 및 마일스 톤은 무엇 인가요?

이러한 보안 요구 사항과 관련 된 용어는 클라우드 솔루션 공급자 프로그램 가이드에 즉시 추가 될 예정입니다. 2019 년 8 월 1 일부 터 적용 되는 CSP 프로그램 참여를 준수 하도록 이러한 보안 요구 사항을 구현 해야 합니다. 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>작업을 수행 하지 않으면 어떻게 되나요?

이러한 보안 방법 및 의무를 준수 하지 못하는 파트너는 이러한 파트너 보안 요구 사항이 적용 되 면 클라우드 솔루션 공급자 프로그램을 실행 하거나 위임 관리자 권한을 활용 하는 고객 테 넌 트를 관리할 수 없습니다. Microsoft는 요구 사항에 대 한 적용 날짜를 설정 하는 과정을 진행 중 이며, 파트너에 게 자세한 정보를 제공 합니다.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Microsoft에서 이러한 새 요구 사항을 적용 하는 이유는 무엇 인가요?
고객과 파트너의 보안 및 개인 정보는 Microsoft의 최우선 순위입니다. 주로 id 손상 인시던트에 관련 된 더 정교 하 고 보안 공격 수가 계속 해 서 표시 됩니다. 예방 제어는 보안 공격을 방지 하기 위해 전반적인 방어 전략에서 주요 역할을 수행 하므로 파트너와 고객을 보호 하기 위한 필수 보안 요구 사항 집합을 적용 하기 시작 합니다.

### <a name="does-this-apply-to-all-geographies"></a>이는 모든 지역에 적용 되나요?

예, 모든 지역에 적용 됩니다. 소 버린 클라우드 (21Vianet, 미국 정부 및 독일)를 통해 거래 하는 모든 파트너는 이러한 새 보안 요구 사항을 즉시 적용 하 고 채택 하는 것이 좋습니다. 그러나 이러한 파트너는 8 월 1 일부 터 적용 되는 새로운 보안 요구 사항을 충족 하는 데 필요 하지 않습니다. Microsoft는 나중에 소 버린 클라우드에 대해 이러한 보안 요구 사항을 적용 하는 것과 관련 된 추가 세부 정보를 제공 합니다.

## <a name="required-actions"></a>필요한 작업

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>요구 사항을 충족 하기 위해 수행 해야 하는 주요 작업은 무엇 인가요?  
CSP 프로그램의 모든 파트너 (직접 청구, 간접 공급자 및 간접 재판매인), 관리자 및 제어판 공급 업체는 요구 사항을 충족 해야 합니다.

1. **모든 사용자에 대해 MFA 적용**

    파트너 테 넌 트의 모든 사용자에 대해 MFA를 적용 하려면 CSP 프로그램, 관리자 및 제어판 공급 업체의 모든 파트너가 필요 합니다. 이렇게 하려면 [관리자에 대해 MFA 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), [최종 사용자 보호 기준](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)및 향후 기준 정책을 사용 하도록 설정 하면 됩니다. 기준 정책에서 제공 하는 기능은 파트너와 고객이 지속적으로 변화 하는 보안 위협 으로부터 보호 될 수 있도록 지속적으로 발전 하 고 있습니다. 따라서 자세히 알아보려면 [기준 정책 설명서](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) 를 검토 하는 것이 중요 합니다.

    - 기준 [정책을 참조 하세요. 관리자 용 mfa 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 기준 정책을 사용 하도록 설정 하는 방법에 대 한 자세한 내용은 관리자 용 mfa를 사용 해야 합니다.
    - 기준 [정책을 참조 하세요. 최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책을 사용 하도록 설정 하는 방법에 대 한 자세한 내용은 최종 사용자 보호를 참조 하세요.
    - [기준 보호 정책의](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)개념을 이해 합니다.

    추가 고려 사항:

    - 간접 공급자는 간접적 재판매인과 협력 하 여 파트너 센터에 등록 하 고 (아직 수행 하지 않은 경우) 대리점에서 요구 사항을 충족 하도록 권장 해야 합니다.
    - Azure MFA는 [Microsoft Authenticator 앱](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)을 사용 하는 유일한 확인 방법으로 기준 정책에 따라 무료로 파트너 테 넌 트의 모든 사용자가 사용할 수 있게 됩니다.
    - SMS 또는 전자 메일과 같은 다른 방법이 필요한 경우에는 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) sku를 통해 추가 인증 방법을 사용할 수 있습니다.
    - 파트너는 Microsoft 상용 클라우드 서비스에 액세스할 때 각 사용자 마다 타사 MFA 솔루션을 활용할 수도 있습니다.

2. **보안 응용 프로그램 모델 프레임 워크 도입**

    Api (예: Azure Resource Manager, Microsoft Graph, 파트너 센터 API 등)를 사용 하 여 사용자 지정 통합을 개발한 모든 파트너 또는 PowerShell과 같은 도구를 사용 하 여 사용자 지정 자동화를 구현한 모든 파트너는 [보안 응용 프로그램 모델을 채택 해야 합니다. ](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)Microsoft 클라우드 서비스와 통합 하기 위한 프레임 워크입니다. 이렇게 하지 않으면 MFA 배포로 인해 중단이 발생할 수 있습니다. 다음 리소스는 모델을 채택 하는 방법에 대 한 개요 및 지침을 제공 합니다.

    - [보안 응용 프로그램 모델 개요](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [파트너 센터: 보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP 프로그램의 파트너: 보안 응용 프로그램 모델을 사용 하도록 설정 하기 위한 .NET 샘플 코드](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [CSP 프로그램의 파트너: 보안 응용 프로그램 모델을 사용 하도록 설정 하기 위한 Java 샘플 코드](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [파트너 센터 인증 문서](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [파트너 센터 PowerShell MFA (Multi-factor Authentication) 문서](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    제어판을 사용 하는 경우 보안 응용 프로그램 모델 프레임 워크의 채택을 관련 하 여 공급 업체에 문의 해야 합니다.

    제어판 공급 업체는 파트너 센터에 제어판 공급 업체에 [등록](https://docs.microsoft.com/partner-center/enroll-as-cpv)하고이 요구 사항을 즉시 구현 하기 시작 해야 합니다. [파트너 센터를 참조 하세요. 보안 응용 프로그램 모델](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)프레임 워크. 제어판 공급 업체는 자격 증명 대신 CSP 파트너의 동의를 수락 하 고 관리 하 고 기존의 모든 CSP 파트너 자격 증명을 제거 해야 합니다.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-mfa"></a>MFA 란?

MFA (multi-factor Authentication)는 둘 이상의 필수 보안 및 유효성 검사 절차를 통해 개인이 인증 되는 보안 메커니즘입니다. 다음 인증 방법을 두 가지 이상 요구 하는 방식으로 작동 합니다.

- 사용자가 알고 있는 사항(일반적으로 암호)
- 사용자의 소유물(전화기처럼 쉽게 복제되지 않는 신뢰할 수 있는 장치)
- 사용자의 신체 관련 항목(생체 공학)

### <a name="what-are-baseline-protection-policies"></a>기준선 보호 정책 이란? 

[Microsoft 기본 보호 정책](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (현재 미리 보기)는 여러 일반적인 공격 으로부터 조직을 보호 하는 데 도움이 되는 미리 정의 된 정책 집합입니다. 이러한 일반적인 공격은 암호 스프레이, 재생 및 피싱을 포함할 수 있습니다. 기본 정책은 모든 버전의 Azure Active Directory에서 사용할 수 있습니다. Microsoft는 id 기반 공격이 지난 몇 년 동안 증가 하 여 모든 사용자에 게 이러한 기본 보호 정책을 사용할 수 있도록 합니다. 이러한 정책의 목표는 모든 조직에서 추가 비용 없이 기본 보안 수준을 사용 하도록 설정 하는 것입니다.

> [!NOTE]
> Microsoft 기본 정책 및 관련 기능은 지속적으로 변화 하는 보안 위협 으로부터 파트너와 고객의 보호를 강화 하기 위해 지속적으로 발전 하 고 있습니다. 기본 정책에 따라 몇 가지 이름 지정 및 분류 변경이 곧 있을 수 있습니다. 기본 정책 페이지를 직접 방문 하 여 최신 정보를 확인 하는 것이 좋습니다.

### <a name="what-baseline-policies-must-i-enable"></a>어떤 기준 정책을 사용 하도록 설정 해야 하나요?

파트너 테 넌 트의 각 사용자에 게 MFA를 제공 하기 위해 현재 기준 보호 정책을 활용 하려는 경우 관리자 및 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책 [에 대해 mfa 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 를 사용 하도록 설정 해야 합니다. 이러한 기준 보호 정책은 모바일 장치를 통해 Microsoft Authenticator 앱을 사용 하는 파트너에 대해서만 무료로 파트너 테 넌 트의 각 사용자에 대 한 MFA 요구 사항을 충족 합니다.

[관리자에 대 한 MFA 필요 기준 정책은](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 파트너 디렉터리의 관리자에 게 활용 되며 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책은 파트너 테 넌 트의 관리자가 아닌 사용자를 보호 하기 위해 활용 됩니다. 이러한 정책을 사용 하도록 설정 하면 사용자가 MFA에 등록 해야 합니다. 사용자가 성공적으로 등록 되 면 정책 조건을 기반으로 로그인을 시도 하는 동안 MFA를 묻는 메시지가 표시 됩니다. 기준 정책에서 제공 하는 기능은 파트너와 고객이 지속적으로 변화 하는 보안 위협 으로부터 보호 될 수 있도록 지속적으로 발전 하 고 있습니다. 따라서 자세히 알아보려면 [기준 정책 설명서](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) 를 검토 하는 것이 중요 합니다.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>관리자 정책에 대해 MFA 필요를 사용 하도록 설정 어떻게 할까요?? 

Azure 관리 포털을 통해 관리자 기준 정책을 위한 MFA 필요를 사용할 수 있습니다. 기준 [정책을 참조 하세요. 이 기준 정책을 사용](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 하도록 설정 하는 방법에 대 한 자세한 내용은 관리자 용 MFA를 사용 해야 합니다.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>최종 사용자 보호 정책을 사용 하도록 설정 어떻게 할까요? 시겠습니까?

Azure 관리 포털을 통해 최종 사용자 보호 기준 정책을 사용 하도록 설정할 수 있습니다. 기준 [정책을 참조 하세요. 이 기준 정책을](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 사용 하도록 설정 하는 방법에 대 한 자세한 내용은 최종 사용자 보호를 참조 하세요.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>기준 정책을 자동으로 사용 하도록 설정 하 시겠습니까? 

아니요,이 정책을 사용 하도록 설정 하려면 전역 관리자, 보안 관리자 또는 조건부 액세스 관리자 역할의 구성원 인 사용자는 정책을 즉시 사용 하도록 정책을 구성 해야 합니다.

### <a name="what-is-the-cost-of-enabling-mfa"></a>MFA를 사용 하도록 설정 하는 비용은 얼마 인가요?

Microsoft는 관리자 및 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 보호 정책 [에 대해 mfa 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 를 구현 하 여 무료로 mfa를 제공 합니다. 이 버전의 MFA를 통해 사용할 수 있는 유일한 확인 옵션은 [Microsoft Authenticator 앱](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)입니다. 전화 통화 또는 SMS 메시지가 필요한 경우 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 라이선스를 구입 해야 합니다. 또는 타사 솔루션을 활용 하 여 파트너 테 넌 트의 각 사용자에 대해 MFA를 제공할 수 있습니다 .이 경우에는 MFA 솔루션이 적용 되 고 있으며 사용자가 준수 하는지 확인 해야 합니다.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>MFA 솔루션이 이미 있는 경우 수행 해야 하는 작업은 무엇 인가요?

이러한 보안 요구 사항에 따라 파트너 테 넌 트의 사용자는 Microsoft 상용 클라우드 서비스에 액세스할 때 MFA를 사용 하 여 인증 해야 합니다. 타사 솔루션을 사용 하 여 이러한 요구 사항을 충족할 수 있습니다. Microsoft는 Azure Active Directory와의 호환성을 위해 독립적인 id 공급자에 대 한 유효성 검사 테스트를 더 이상 제공 하지 않습니다. 상호 운용성을 위해 제품을 테스트 하려는 경우에는 다음 [지침](https://www.microsoft.com/download/details.aspx?id=56843)을 참조 하세요.

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>MFA를 인증 하는 데 사용할 수 있는 확인 방법

Microsoft는 관리자 및 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 보호 정책 [에 대해 mfa 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 를 구현 하 여 무료로 mfa를 제공 합니다. 이 버전의 MFA를 통해 사용할 수 있는 유일한 확인 옵션은 [Microsoft Authenticator 앱](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)입니다. 전화 통화 또는 SMS 메시지가 필요한 경우 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 라이선스를 구입 해야 합니다. 또는 타사 솔루션을 활용 하 여 파트너 테 넌 트의 각 사용자에 대해 MFA를 제공할 수 있습니다 .이 경우에는 MFA 솔루션이 적용 되 고 있으며 사용자가 준수 하는지 확인 해야 합니다.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>여러 파트너 테 넌 트를 사용 하 여 transact-sql 합니다. MFA를 모두 구현 해야 하나요?

예, CSP 프로그램 또는 Advisor 프로그램과 연결 된 각 Azure Active Directory 테 넌 트에 대해 MFA를 적용 해야 합니다. Azure Active Directory Premium 라이선스를 구매 하려는 경우 각 Azure Active Directory 테 넌 트에서 사용자에 대 한 라이선스를 구매 해야 합니다.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>파트너 테 넌 트의 각 사용자에 게 MFA를 적용 해야 하나요? 

관리자 및 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) [를 위한 mfa 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 기본 보호 정책은 파트너 테 넌 트의 각 사용자에 대해 mfa를 적용 합니다. 이러한 정책을 활용 하 여 MFA를 제공 하 고 [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) 응용 프로그램을 사용 하는 경우 추가 라이선스를 구매할 필요가 없습니다. 그렇지 않으면 파트너 테 넌 트의 각 사용자에 게 MFA를 제공 하는 적절 한 솔루션을 구매 해야 합니다.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Microsoft와 직접 요금을 청구 하는 파트너입니다. 무엇을 해야 하나요?

직접 청구 클라우드 솔루션 공급자 파트너는 파트너 테 넌 트의 각 사용자에 대해 MFA를 적용 해야 합니다.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>저는 간접 재판매인 이며 배포자 인 경우에만 발생 합니다. 그래도이 작업을 수행 해야 하나요?

모든 간접 대리점은 파트너 테 넌 트의 각 사용자에 대해 MFA를 적용 해야 합니다. 간접 재판매인이 수행 해야 하는 작업입니다.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>파트너 센터 API를 사용 하지 않습니다. 그래도 MFA를 구현 해야 하나요?

예, 파트너 테 넌 트의 파트너 관리자 사용자 및 최종 사용자를 포함 한 모든 사용자에 게이 보안 요구 사항이 적용 됩니다.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Azure Active Directory와 호환 되는 MFA 솔루션을 제공 하는 타사 공급 업체는 무엇 인가요?

[Gartner](https://www.gartner.com/en/webinars/3881781)와 같이 온라인으로 MFA 솔루션에 대 한 많은 독립적인 검토가 있습니다. MFA 공급 업체 및 솔루션을 검토할 때 파트너는 선택한 솔루션이 Azure Active Directory와 호환 되는지 확인 해야 합니다.

Microsoft는 Azure Active Directory와의 호환성을 위해 독립적인 id 공급자에 대 한 유효성 검사 테스트를 더 이상 제공 하지 않습니다. 상호 운용성을 위해 제품을 테스트 하려는 경우에는 다음 [지침](https://www.microsoft.com/download/details.aspx?id=56843)을 참조 하세요.

자세한 내용은 [AZURE AD 페더레이션 호환성 목록](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)을 참조 하세요.

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Integration 샌드박스에서 MFA를 테스트 하려면 어떻게 해야 하나요?

Integration 샌드박스 테 넌 트에 대해 [관리자](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 및 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책을 사용 하도록 설정 해야 합니다. 이 정책을 통해 테 넌 트의 각 사용자는 MFA를 사용 하 여 인증 해야 합니다.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>MFA를 사용 하 여 고객의 테 넌 트와 상호 작용 하는 방법 

아니요. 이러한 보안 요구 사항을 충족 하는 것은 고객을 관리 하는 방법에 영향을 주지 않습니다. 위임 된 관리 작업을 수행 하는 기능은 중단 되지 않습니다.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>고객은 파트너 보안 요구 사항을 적용 하나요?

아니요, 고객의 Azure AD 테 넌 트의 각 사용자에 대해 MFA를 적용 해야 하는 것은 아닙니다. 그러나 각 고객을 사용 하 여 사용자를 보호 하는 최선의 방법을 결정 하는 것이 좋습니다.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>앱 암호를 기준 보호 정책과 함께 사용할 수 있나요?

예, [앱 암호](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) 를 사용할 수 있습니다. [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) 에 설명 된 앱 암호 사용에 대 한 고려 사항을 검토 하 여 필요에 따라 지원 되는지 확인 해야 합니다.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>이 요구 사항에서 사용자를 제외할 수 있나요? 

아니요. 파트너 테 넌 트에서 서비스 계정을 포함 한 각 사용자는 MFA를 사용 하 여 인증 해야 합니다.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>파트너 보안 요구 사항이 통합 샌드박스에 적용 되나요?

예, 파트너 보안 요구 사항은 통합 샌드박스에 적용 됩니다. 즉, integration sandbox 테 넌 트에서 사용자를 위한 적절 한 MFA 솔루션을 구현 해야 합니다. MFA를 제공 하는 기본 보호 정책을 구현 하는 것이 좋습니다.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>응급 액세스 (브레이크 유리) 계정을 구성 어떻게 할까요??

Azure AD 테 넌 트에서 실수로 잠기는 것을 방지 하기 위해 하나 또는 두 개의 응급 액세스 계정을 만드는 것이 모범 사례로 간주 됩니다. 파트너 보안 요구 사항과 관련 하 여 각 사용자가 MFA를 사용 하 여 인증 해야 합니다. 따라서이는 응급 액세스 계정의 정의를 수정 해야 함을 의미 합니다. MFA에 타사 솔루션을 활용 하는 계정일 수 있습니다.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>게스트 사용자는 파트너 보안 요구 사항의 영향을 받는 방법

게스트 사용자는 파트너 테 넌 트의 리소스에 액세스할 때 MFA를 사용 하 여 인증 해야 합니다. 파트너 보안 요구 사항은 자체 테 넌 트의 리소스에 액세스 하는 게스트 사용자에 게 영향을 주지 않습니다.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>타사 솔루션을 사용 하는 경우 ADFS (Active Directory 페더레이션 서비스)가 필요 한가요? 

아니요, 타사 솔루션을 사용 하는 경우에는 ADFS (Active Directory 페더레이션 서비스)를 사용할 필요가 없습니다. 솔루션 공급 업체와 협력 하 여 솔루션에 대 한 요구 사항을 결정 하는 것이 좋습니다.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>기본 보호 정책을 사용 하도록 설정 해야 하나요?

아니요, 기본 보호 정책을 사용 하도록 설정할 필요는 없습니다. 유일한 요구 사항은 파트너 테 넌 트에서 서비스 계정을 포함 하 여 각 사용자에 대해 MFA를 적용 하는 것입니다.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>조건부 액세스를 사용 하 여 MFA 요구 사항을 충족할 수 있나요?

예, 조건부 액세스를 사용 하 여 파트너 테 넌 트에서 서비스 계정을 비롯 한 각 사용자에 대해 MFA를 적용할 수 있습니다. 그러나 파트너의 매우 높은 권한이 있는 경우 각 사용자에 게 모든 단일 인증에 대 한 MFA 챌린지를 제공 해야 합니다. 즉, MFA에 대 한 요구 사항을 회피 하는 조건부 액세스 기능을 활용할 수 없습니다.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>기준 보호 정책을 구현 하 여 제공 되는 확인 옵션은 무엇 인가요? 

기본 보호 정책을 구현 하 여 사용할 수 있는 MFA 버전을 고려 하 여, 인증자 앱만 사용할 수 있습니다. 전화 통화 및 문자 메시지 메시지의 사용은 안전 하지 않은 것으로 간주 됩니다. 따라서 이러한 옵션은이 버전의 MFA를 통해 사용할 수 없습니다.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>에서 사용 하는 서비스 계정이 파트너 보안 요구 사항의 영향을 받을 Azure AD Connect 있나요?

아니요, Azure AD Connect에서 사용 하는 서비스 계정은 파트너 보안 요구 사항의 영향을 받지 않습니다. MFA를 적용 한 결과로 Azure AD Connect에 문제가 발생 하는 경우 Microsoft 지원에 문의 하 여 기술 지원 요청을 여세요.

## <a name="secure-application-model"></a>보안 응용 프로그램 모델

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>요구 사항에 맞게 보안 응용 프로그램 모델을 채택 해야 하는 사람은 누구 인가요?

Microsoft는 Multi-factor Authentication을 활용 하는 CSP (클라우드 솔루션 공급자) 파트너 및 CPV (제어판 공급 업체)를 인증 하기 위한 안전 하 고 확장 가능한 프레임 워크를 도입 하 고 있습니다. 자세한 내용은 [보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 를 참조 하세요. Api (예: Azure Resource Manager, Microsoft Graph, 파트너 센터 API 등)를 사용 하 여 사용자 지정 통합을 개발한 모든 파트너 또는 PowerShell과 같은 도구를 사용 하 여 사용자 지정 자동화를 구현한 모든 파트너는 [보안 응용 프로그램 모델을 채택 해야 합니다. ](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)Microsoft 클라우드 서비스와 통합 하기 위한 프레임 워크입니다.

### <a name="what-is-the-secure-application-model"></a>보안 응용 프로그램 모델 이란?

Microsoft는 Multi-factor Authentication을 활용 하는 CSP (클라우드 솔루션 공급자) 파트너 및 CPV (제어판 공급 업체)를 인증 하기 위한 안전 하 고 확장 가능한 프레임 워크를 도입 하 고 있습니다. 자세한 내용은 [보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 를 참조 하세요.  

### <a name="how-do-i-implement-the-secure-application-model"></a>보안 응용 프로그램 모델을 구현할 어떻게 할까요? 있나요?

Api (예: Azure Resource Manager, Microsoft Graph, 파트너 센터 API 등)를 사용 하 여 사용자 지정 통합을 개발한 모든 파트너 또는 PowerShell과 같은 도구를 사용 하 여 사용자 지정 자동화를 구현한 모든 파트너는 [보안 응용 프로그램 모델을 채택 해야 합니다. ](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)Microsoft 클라우드 서비스와 통합 하기 위한 프레임 워크입니다. 이렇게 하지 않으면 MFA 배포로 인해 중단이 발생할 수 있습니다. 다음 리소스는 모델을 채택 하는 방법에 대 한 개요 및 지침을 제공 합니다.

- [보안 응용 프로그램 모델 개요](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [파트너 센터: 보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP 프로그램의 파트너: 보안 응용 프로그램 모델을 사용 하도록 설정 하기 위한 .NET 샘플 코드](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [CSP 프로그램의 파트너: 보안 응용 프로그램 모델을 사용 하도록 설정 하기 위한 Java 샘플 코드](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [파트너 센터 인증 문서](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [파트너 센터 PowerShell MFA (Multi-factor Authentication) 문서](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

제어판을 사용 하는 경우 보안 응용 프로그램 모델 프레임 워크의 채택을 관련 하 여 공급 업체에 문의 해야 합니다.

제어판 공급 업체는 파트너 센터에 제어판 공급 업체에 [등록](https://docs.microsoft.com/partner-center/enroll-as-cpv)하고이 요구 사항을 즉시 구현 하기 시작 해야 합니다. [파트너 센터를 참조 하세요. 보안 응용 프로그램 모델](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)프레임 워크. 제어판 공급 업체는 자격 증명 대신 CSP 파트너의 동의를 수락 하 고 관리 하 고 기존의 모든 CSP 파트너 자격 증명을 제거 해야 합니다.

### <a name="who-is-a-control-panel-vendor-cpv"></a>CPV (제어판 공급 업체)는 누구 인가요? 
제어판 공급 업체는 CSP 파트너가 파트너 센터 Api와 통합 하는 데 사용할 앱을 개발 하는 독립 소프트웨어 공급 업체입니다. 제어판 공급 업체는 파트너 센터 대시보드 또는 Api에 직접 액세스할 수 있는 CSP 파트너가 아닙니다. 자세한 설명은 [파트너 센터 내에서 사용할 수 있습니다. 보안 응용 프로그램 모델](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)가이드를 참조 하세요.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>보안 응용 프로그램 모델은 파트너 센터 API/SDK 전용으로 구현 해야 하나요? 

*관리자 용 MFA* 및 *최종 사용자 보호* 기준 정책을 모두 사용 하도록 설정 하면 각 사용자가 다단계 인증을 사용 하 여 인증 해야 합니다. 즉, 비 대화형으로 실행 되며 인증에 사용자 자격 증명을 사용 하는 데 사용 되는 각 API, CLI 및 PowerShell 모듈 (예: Azure, Azure AD, MS Online, 파트너 센터 등)에 대해 보안 응용 프로그램 모델을 구현 해야 합니다.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>PowerShell과 같은 자동화 도구를 사용 하 고 있습니다. 보안 응용 프로그램 모델을 구현할 어떻게 할까요? 있나요?  

자동화가 비 대화형으로 실행 되 고 인증을 위해 사용자 자격 증명을 사용 하는 경우 보안 응용 프로그램 모델을 구현 해야 합니다. [보안 응용 프로그램 모델 보기 | 파트너 센터 PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) 을 구현 하는 방법에 대 한 지침을 제공 합니다.  모든 자동화 도구가 액세스 토큰을 사용 하 여 인증 하는 기능을 제공 하는 것은 아닙니다. 변경 해야 하는 사항을 이해 하는 데 도움이 필요한 경우 [파트너 센터 보안 지침](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 그룹에 메시지를 게시 하세요.

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>동의 프로세스를 수행할 때 응용 프로그램 관리자가 제공 해야 하는 사용자 자격 증명은 무엇입니까? 

최소 권한 사용 권한이 할당 된 서비스 계정을 사용 하는 것이 좋습니다. 파트너 센터 API와 관련 하 여, 영업 에이전트 또는 관리 에이전트 역할이 할당 된 계정을 사용 해야 합니다.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>응용 프로그램 관리자가 승인 프로세스를 수행할 때 전역 관리자 자격 증명을 제공 하지 않는 이유는 무엇 인가요?

위험을 완화 하는 것과 같은 방법으로 최소한의 권한을 사용 하는 것이 좋습니다. 전역 관리자 권한이 있는 계정은 필요한 것 보다 많은 권한을 제공 하므로 사용 하지 않는 것이 좋습니다.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>CSP 파트너입니다. 이 솔루션을 구현 하는 동안 CPV (제어판 공급 업체)가 작동 하 고 있는지 확인 어떻게 할까요?? 

CPV (제어판 공급 업체) 솔루션을 사용 하 여 CSP (클라우드 솔루션 공급자) 프로그램에서 transact-sql을 사용 하는 파트너의 경우 CPV에 게 문의 해야 합니다. 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>CPV입니다. 등록 어떻게 할까요?? 

CPV (제어판 공급 업체)로 등록 하려면 [여기](https://docs.microsoft.com/partner-center/enroll-as-cpv)에 제공 된 지침을 따르세요.

등록 링크를 받으려면 cpvs는에 연락 [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) 하 여 cpvs와 비즈니스 관계에 있는 Microsoft 직원 스폰서를 제공 하거나 비즈니스를 알고 있어야 합니다. 예를 들어 PDM (파트너 개발 관리자)이 있습니다.

파트너 센터에 등록 하 고 응용 프로그램을 등록 하면 파트너 센터 Api에 액세스할 수 있습니다. 새 CPV를 사용할 경우 파트너 센터 알림을 통해 샌드박스 정보를 받게 됩니다. Microsoft CPV로 등록을 완료 하 고 CPV 규약을 수락한 후 다음을 수행할 수 있습니다.

1. 다중 테 넌 트 응용 프로그램 관리 (파트너 센터에서 응용 프로그램을 Azure Portal에 추가 하 고 등록 및 등록 취소). 참고: CPVs는 파트너 센터 Api에 대 한 권한을 부여 받으려면 파트너 센터에서 해당 응용 프로그램을 등록 해야 합니다. Azure Portal 단독으로 응용 프로그램을 추가 해도 파트너 센터 Api에 대 한 CPV 응용 프로그램에는 권한이 부여 되지 않습니다.
2. CPV 프로필을 보고 관리 합니다.
3. CPV 기능에 액세스 해야 하는 사용자를 보고 관리 합니다. CPV가 가질 수 있는 유일한 역할은 전역 관리자입니다.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>파트너 센터 SDK를 사용 하 고 있습니다. SDK가 보안 응용 프로그램 모델을 자동으로 채택 하나요? 

아니요, [보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)에 제공 된 지침을 따라야 합니다.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>MFA를 사용 하도록 설정 하지 않은 계정을 사용 하 여 보안 응용 프로그램 모델에 대 한 새로 고침 토큰을 생성할 수 있나요?

예, MFA를 적용 하지 않은 계정을 사용 하 여 새로 고침 토큰을 생성할 수 있습니다. 그러나 MFA를 사용 하도록 설정 하지 않은 계정을 사용 하 여 생성 된 토큰은 MFA 요구 사항으로 인해 리소스에 액세스할 수 없기 때문에이 작업을 수행 하면 안 됩니다.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA를 사용 하도록 설정 하는 경우 응용 프로그램에서 액세스 토큰을 가져오는 방법

새 보안 요구 사항을 준수 하는 동안이 작업을 수행 하는 방법에 대 한 세부 정보를 제공 하는 [보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 를 따라야 합니다. [여기](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)에서 .NET 샘플 코드를, [여기](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)에서 Java 샘플 코드를 찾을 수 있습니다.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV 테 넌 트 또는 CSP 파트너의 테 넌 트에 Azure AD 응용 프로그램을 만들어야 하나요?

CPV는 CPV로 등록 된 테 넌 트에 Azure Active Directory 응용 프로그램을 만들어야 합니다.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>앱 전용 인증을 사용 하는 CSP입니다. 변경 해야 하나요?

사용자 자격 증명을 사용 하 여 액세스 토큰을 요청 하지 않으므로 앱 전용 인증만 영향을 받지 않습니다. 사용자 자격 증명을 공유 하는 경우 CPVs (제어판 공급 업체)는 [보안 응용 프로그램 모델 프레임 워크](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 를 채택 하 고 기존 파트너 자격 증명을 모두 제거 해야 합니다.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV는 앱 전용 인증 스타일을 활용 하 여 액세스 토큰을 가져올 수 있나요?

아니요, 제어판 공급 업체 파트너가 앱 전용 인증 스타일을 사용 하 여 파트너를 대신해 액세스 토큰을 요청할 수 없습니다. 앱 + 사용자 인증 스타일을 활용 하는 보안 응용 프로그램 모델을 구현 해야 합니다.

## <a name="key-resources"></a>주요 리소스

### <a name="how-to-get-started"></a>시작하는 방법

- [파트너 보안 요구 사항: 단계별 가이드](https://docs.microsoft.com/partner-center/partner-security-requirements)
- 이 [파트너 센터 보안 지침 그룹](https://aka.ms/MPCSecurityGuidance)에 질문 및 피드백을 보냅니다.
- 예정 된 파트너 사무실 시간 및 웹 세미나에 참석 합니다. [여기에서 자세한 일정과 리소스](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)를 확인 하세요.

### <a name="resources-for-enabling-mfa"></a>MFA 사용을 위한 리소스

- [기준 보호 정책의](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)개념을 이해 합니다.
- 기준 [정책을 참조 하세요. 관리자 용 mfa 필요](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 기준 정책을 사용 하도록 설정 하는 방법에 대 한 자세한 내용은 관리자 용 mfa를 사용 해야 합니다.
- 기준 [정책을 참조 하세요. 최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책을 사용 하도록 설정 하는 방법에 대 한 자세한 내용은 최종 사용자 보호를 참조 하세요.

### <a name="resources-for-adopting-secure-application-model"></a>보안 응용 프로그램 모델 채택을 위한 리소스

- [보안 응용 프로그램 모델 개요](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [파트너 센터: 보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP 프로그램의 파트너: 보안 응용 프로그램 모델을 사용 하도록 설정 하기 위한 .NET 샘플 코드](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [CSP 프로그램의 파트너: 보안 응용 프로그램 모델을 사용 하도록 설정 하기 위한 Java 샘플 코드](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [파트너 센터 인증 문서](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [파트너 센터 PowerShell MFA (Multi-factor Authentication) 문서](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>지원

### <a name="where-can-i-ask-get-support"></a>지원을 받을 수 있는 곳은 어디 인가요?

또한 리소스를 활용 하 여 보안 요구 사항을 충족 하는 지원을 위해 ASfP (파트너에 대 한 고급 지원)가 서비스 계정 관리자에 문의 하는 경우 PSfP (파트너 계약)에 대 한 프리미어 지원 서비스 계정 관리자 및 기술 계정 관리자에 게 문의 하세요.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>기준 정책 사용에 대 한 도움을 받으려면 어떻게 해야 하나요?

- 파트너는 MPN 혜택에서 자문 시간을 활용 하 여 보안 요구 사항을 구현 하는 방법에 대 한 자세한 지침을 얻을 수 있습니다.
- Azure Active Directory에 대 한 기술 제품 지원 옵션은 MPN 혜택을 통해 제공 됩니다. 활성 ASfP 또는 PSfP 계약에 대 한 액세스 권한이 있는 파트너는 연결 된 계정 관리자 (SAM/TAM)와 함께 사용할 수 있는 옵션을 가장 잘 이해할 수 있습니다.
- 파트너 센터에서 기준선 정책 구현에 대 한 지원은 [파트너 센터 서비스 요청](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)을 통해 액세스할 수 있습니다. 항목으로 *MFA & 보안 응용 프로그램 모델* 을 선택 합니다.

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>보안 응용 프로그램 모델 프레임 워크를 채택 하는 기술 정보를 얻을 어떻게 할까요? 있나요? 

Azure Active Directory에 대 한 기술 제품 지원 옵션은 MPN 혜택을 통해 제공 됩니다. 활성 ASfP 또는 PSfP 구독에 대 한 액세스 권한이 있는 파트너는 연결 된 계정 관리자 (SAM/TAM)와 함께 사용할 수 있는 옵션을 가장 잘 이해할 수 있습니다.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>기술적인 일반적인 문제에 대 한 자세한 정보는 어디서 찾을 수 있나요? 

기술적 일반적인 문제에 대 한 정보는 [여기](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)를 참조 하세요.
