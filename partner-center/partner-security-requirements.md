---
title: 파트너 보안 요구 사항 | 파트너 센터
ms.topic: article
ms.date: 09/25/2019
description: 클라우드 솔루션 공급자 프로그램에 참여하는 관리자 및 파트너에 대한 보안 요구 사항에 대해 알아봅니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급업체, CPV, 다단계 인증, MFA, 보안 애플리케이션 모델, 보안 앱 모델, 보안
ms.localizationpriority: high
ms.openlocfilehash: ea155cf760850def85146d8c4e7e847fab5d7213
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318484"
---
# <a name="partner-security-requirements"></a>파트너 보안 요구 사항

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 제어판 공급업체
- 모든 관리자

개인 정보 보호 및 보안 강화는 최우선 순위입니다. 최선의 방어는 예방이며, 가장 약한 링크를 강화해야 한다는 것을 알고 있습니다. 따라서 에코시스템의 모든 사람이 조치를 취하고, 적절한 보안 기능을 마련해야 합니다. Microsoft에서는 파트너와 고객을 보호하기 위해 클라우드 솔루션 공급자 프로그램에 참여하는 관리자, 제어판 공급업체 및 파트너에 대한 일련의 필수 보안 요구 사항을 도입하고 있습니다.

2019년 8월 1일부터 모든 파트너는 서비스 계정을 비롯한 모든 사용자의 파트너 테넌트에 다단계 인증을 적용해야 합니다.

> [!NOTE]
> 소버린 클라우드(21Vianet, 미국 정부 및 독일)를 통해 거래하는 모든 파트너는 이러한 새 보안 요구 사항을 즉시 적용하고 채택할 것을 적극 권장합니다. 그러나 이러한 파트너는 2019년 8월 1일부터 적용되는 새로운 보안 요구 사항을 충족할 필요가 없습니다. Microsoft에서는 나중에 소버린 클라우드에 대한 이러한 보안 요구 사항의 적용과 관련된 추가 세부 정보를 제공할 예정입니다.

파트너 보안 요구 사항과 관련된 용어가 [클라우드 솔루션 공급자 프로그램 가이드](https://go.microsoft.com/fwlink/p/?LinkId=617100)에 추가되었습니다. 2019년 8월 1일부터 클라우드 솔루션 공급자 프로그램에 참여하는 모든 파트너는 사용 약관을 준수해야 합니다. 관리자와 관련이 있으므로 동일한 계약 요구 사항이 적용됩니다.

이러한 요구 사항이 적용되면 필수 보안 요구 사항을 구현하지 않는 파트너가 클라우드 솔루션 공급자 프로그램에서 거래하거나 위임 관리자 권한을 활용하는 고객 테넌트를 관리할 수 없게 됩니다. Microsoft는 요구 사항의 기술 적용 날짜를 정하는 중이며, 파트너에 게 이 날짜와 자세한 정보를 제공할 예정입니다.

## <a name="what-actions-do-i-need-to-take"></a>어떤 조치를 취해야 하나요?

파트너는 매우 높은 권한이 있으므로 각 사용자가 인증할 때마다 MFA 챌린지를 수행하도록 해야 합니다. 이 작업은 다음 방법 중 하나를 통해 수행할 수 있습니다.

- Azure AD Premium을 구현하고 MFA가 각 사용자에게 적용되는지 확인
- [기준 보호 정책](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) 구현
- 타사 솔루션을 구현하고 MFA가 각 사용자에게 적용되는지 확인

> [!IMPORTANT]
> 이러한 요구 사항을 기술적으로 적용한 후에는 인증할 때마다 MFA 챌린지가 표시되어야 합니다. Microsoft 상용 클라우드 서비스에 액세스할 때 MFA를 사용한 인증을 방지하기 위해 조건부 액세스의 모든 기능을 사용할 수 없습니다.

### <a name="considerations"></a>고려 사항

이러한 요구 사항은 파트너 테넌트에서 서비스 계정을 비롯한 모든 사용자에게 적용되므로 원활한 배포를 위해 고려해야 할 몇 가지 사항이 있습니다. 이러한 고려 사항에는 MFA를 수행할 수 없는 Azure AD의 사용자 및 최신 인증을 지원하지 않는 조직에서 사용하는 애플리케이션 및 디바이스를 식별하는 작업이 포함됩니다.

작업을 수행하기 전에 다음을 확인하는 것이 좋습니다.

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>인증할 때 MFA 사용을 지원하지 않는 애플리케이션 또는 디바이스가 있나요?

MFA 레거시 인증을 적용하는 경우 IMAP, POP3, SMTP 등의 프로토콜을 사용하면 차단됩니다. 이러한 프로토콜은 MFA를 지원하지 않기 때문입니다. 이러한 제한 사항을 해결하려면 [앱 암호](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)라고 하는 기능을 사용하여 애플리케이션 또는 디바이스에서 계속 인증하도록 할 수 있습니다. 앱 암호를 해당 환경에서 사용할 수 있는지 확인하려면 [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)에 설명된 앱 암호 사용에 대한 고려 사항을 검토해야 합니다.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>파트너 테넌트와 연결된 라이선스에서 제공하는 Office 365를 사용하는 사용자가 있나요?

솔루션을 구현하기 전에 파트너 테넌트의 사용자가 Microsoft Office 버전을 사용하는 이유를 확인하는 것이 좋습니다. 작업을 수행하기 전에 [Office 365 배포의 다단계 인증 계획](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)을 살펴보세요. 사용자가 Outlook과 같은 애플리케이션의 연결 문제를 경험하게 될 가능성이 있습니다. MFA를 적용하기 전에 Outlook 2013 SP1 이상을 사용 중이고, 조직에서 최신 인증을 사용하는지 확인해야 합니다. 자세한 내용은 [Exchange Online에서 최신 인증 사용](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)을 참조하세요.

Microsoft Office 2013이 설치된 Windows를 실행하는 모든 디바이스에서 최신 인증을 사용하도록 설정하려면 레지스트리 키를 두 개 만들어야 합니다. [Windows 디바이스에서 Office 2013에 최신 인증 사용](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)을 참조하세요.

> [!IMPORTANT]
> 사용자가 Azure AD MFA를 사용하도록 설정되어 있고, 최신 인증을 사용하도록 설정되지 않은 Office 2013을 실행 중인 디바이스가 있는 경우 해당 디바이스에서 앱 암호를 사용해야 합니다. 앱 암호와 앱 암호를 사용하는 경우/위치/방법에 대한 자세한 내용은 [Azure Multi-Factor Authentication과 앱 암호](https://go.microsoft.com/fwlink/p/?LinkId=528178)에서 확인할 수 있습니다.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>사용자가 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 정책이 있나요?

직원이 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 회사 정책은 구현하는 MFA 솔루션에 영향을 주므로 이러한 정책을 식별하는 것이 중요합니다. 인증에 인증 앱만 사용하도록 하는 [기준 보호 정책](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)의 구현을 통해 제공되는 솔루션과 같은 MFA 솔루션이 있습니다. 조직에 모바일 디바이스 사용을 금지하는 정책이 있는 경우 다음 옵션 중 하나를 고려해야 합니다.

- 보안 시스템에서 실행할 수 있는 시간 기반 TOTP(시간 제약이 있는 일회성 암호) 애플리케이션 배포
- 가장 적절한 인증 옵션을 제공하는 파트너 테넌트의 각 사용자에게 MFA를 적용하는 타사 솔루션 구현
- 관련 사용자를 위한 [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) 라이선스 구매

FIDO 보안 키 사용에 대한 지원은 기준 보호 정책에 대한 로드맵에 있습니다. 지원이 추가되면 두 번째 인증 단계에서 FIDO 보안 키를 활용할 수 있습니다. 그 전에는 인증자 앱만 사용할 수 있습니다.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>인증에 사용자 자격 증명을 활용하는 자동화 또는 통합이 있나요?

서비스 계정을 비롯한 각 사용자에게 MFA를 적용하는 것이 요구 사항이므로 파트너 디렉터리에서 인증에 사용자 자격 증명을 활용하는 모든 자동화 또는 통합이 영향을 받습니다. 따라서 이러한 상황에서 사용되는 계정을 식별하는 것이 중요합니다. 다음은 고려해야 할 애플리케이션 또는 서비스 예의 목록입니다.

- 고객을 대신하여 리소스를 프로비저닝하는 데 사용되는 제어판
- 청구 및 고객 지원에 사용되는 모든 플랫폼(CSP 프로그램 관련)과의 통합
- Az, AzureRM, Azure AD, MS Online 등의 모듈을 활용하는 PowerShell 스크립트

위의 목록은 포괄적이지 않습니다. 따라서 사용 중인 환경에서 인증에 사용자 자격 증명을 활용하는 애플리케이션 또는 서비스에 대한 완전한 평가를 수행하는 것이 중요합니다. MFA에 대한 요구 사항에 대처하려면 [보안 애플리케이션 모델 프레임워크](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)의 지침을 구현해야 합니다(가능한 경우). 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 이해하는 데 도움이 되는 추가 리소스는 다음과 같습니다.

- [파트너 센터 .NET 샘플](https://github.com/microsoft/partner-center-dotnet-samples) - 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, .NET을 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 Java 샘플](https://github.com/microsoft/partner-center-java-samples) - 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, Java를 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 PowerShell - 보안 애플리케이션 모델](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) - PowerShell을 사용하여 보안 애플리케이션 모델 프레임워크를 구현하는 방법에 대한 자세한 내용을 제공하는 문서입니다.
- [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - 예정된 이벤트에 대해 알아보고 궁금한 점을 물어볼 수 있는 온라인 커뮤니티입니다.

### <a name="enforcing-mfa-for-all-users"></a>모든 사용자에게 MFA 적용

이 섹션에서는 [기준 보호 정책](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)을 사용하여 파트너 테넌트의 서비스 계정을 비롯한 각 사용자에게 MFA를 적용하는 방법을 설명합니다. Azure AD Premium을 사용하려는 경우 [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)에 설명된 단계를 따르세요.

> [!NOTE]
> Azure AD와 호환되는 타사 솔루션을 사용하여 서비스 계정을 비롯한 모든 사용자에게 MFA를 적용할 수 있습니다. 솔루션을 구현하는 방법에 대한 자세한 내용은 공급업체의 설명서를 참조하세요.

기준 보호 정책은 여러 일반적인 공격으로부터 조직을 보호하는 데 도움이 되는 미리 정의된 정책 세트입니다. 이러한 일반적인 공격은 암호 스프레이, 재생 및 피싱을 포함할 수 있습니다. 기준 보호 정책은 모든 버전의 Azure Active Directory에서 사용할 수 있습니다. Microsoft는 고객과 파트너가 나중에 최고의 보안 사례를 구현할 수 있도록 모든 사용자가 이러한 기준 보호 정책을 사용할 수 있도록 합니다.

사용하도록 설정해야 하는 두 가지 기준 보호 정책은 아래 표에 설명되어 있습니다.

|**정책**| |
|-----|-----|
|**관리자용 MFA 필요**|관리자용 MFA 필요 정책이 사용하도록 설정되면 관리자 역할의 사용자가 인증자 앱을 사용하여 MFA에 등록해야 합니다. MFA 등록이 완료되면 관리자가 로그인할 때마다 MFA를 수행해야 합니다.|
|**최종 사용자 보호**|최종 사용자 보호는 디렉터리의 모든 사용자를 보호하는 위험 기반 MFA 기준 보호 정책입니다. 이 정책이 사용하도록 설정되면 모든 사용자가 인증자 앱을 사용하여 MFA에 등록해야 합니다. 사용자는 MFA 등록 프롬프트를 14일 동안 무시할 수 있으며 그 후에는 MFA에 등록하기 전까지 로그인이 차단됩니다. MFA에 등록된 사용자에게는 위험한 로그인 시도 중에만 MFA를 묻는 메시지가 표시됩니다. 손상된 사용자 계정은 해당 암호를 다시 설정하고 위험 이벤트를 해제할 때까지 차단됩니다.|

이러한 정책이 사용 설정되어 있으면 각 사용자는 추가 비용 없이 인증용 인증자 앱을 사용하여 Azure MFA를 활용할 수 있습니다.

#### <a name="configure-self-service-password-reset"></a>셀프 서비스 암호 재설정 구성

SSPR(셀프 서비스 암호 재설정)은 사용자가 지원 팀에 문의할 필요 없이 암호를 다시 설정할 수 있게 해주는 Azure Active Directory 기능입니다. 사용자는 서비스를 사용하기 전에 셀프 서비스 암호 재설정에 등록하거나 등록되어 있어야 합니다. 등록하는 동안 사용자는 조직에서 사용하도록 설정한 하나 이상의 인증 방법을 선택합니다.

[최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 보호 정책을 사용하도록 설정하면 암호를 다시 설정하고 위험 이벤트를 해제할 때까지 손상된 모든 사용자 계정이 차단됩니다. 이를 고려하여 전역 관리자인 각 사용자는 계정이 잠기지 않도록 다음을 수행하여 SSPR에 등록하는 것이 좋습니다.

1. [SSPR 설정 페이지](https://aka.ms/ssprsetup)로 이동합니다.
2. 사용자 이름과 암호 입력
3. 암호를 다시 설정할 때 사용자를 확인하는 데 사용되는 인증 옵션 중 하나 이상을 구성합니다.  

계정이 손상되면 관리자는 영향을 받는 사용자에 대한 액세스를 복원하는 조치를 취해야 합니다. 사용자를 차단 해제하는 프로세스에 대한 자세한 내용은 [사용자 차단 해제 단계](#recovering-compromised-accounts)를 참조하세요.

#### <a name="require-mfa-for-admins"></a>관리자용 MFA 필요

*관리자용 MFA 필요* 기준 정책은 가장 높은 권한을 가진 Azure Active Directory 역할로 간주되는 다음과 같은 디렉터리 역할에 MFA를 요구합니다.

- 전역 관리자
- SharePoint 관리자
- Exchange 관리자
- 조건부 액세스 관리자
- 보안 관리자
- 기술 지원팀 관리자/암호 관리자
- 대금 청구 관리자
- 사용자 관리자

관리자용 MFA 필요 정책이 사용하도록 설정되면 위의 관리자 역할 9개가 인증자 앱을 사용하여 MFA에 등록해야 합니다. MFA 등록이 완료되면 관리자가 로그인할 때마다 MFA를 수행해야 합니다.

조직에서 스크립트 또는 코드에 이러한 계정을 사용 중인 경우 이를 [관리 ID](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)로 바꾸는 것이 좋습니다.

이 정책을 사용하도록 설정하고 관리자를 보호하려면 다음을 수행합니다.

1. 글로벌 관리자, 보안 관리자 또는 조건부 액세스 관리자로 **Azure Portal**에 로그인합니다.
2. **Azure Active Directory** > **조건부 액세스**로 이동합니다.
3. 정책 목록에서 **기준 정책: 관리자용 MFA 필요**를 선택합니다.
4. **정책 사용**을 **즉시 정책 사용**으로 설정합니다.
5. **Save**을 클릭합니다.

> [!WARNING]
> 이 정책을 사용하도록 설정하기 전에 사용자가 레거시 인증 프로토콜을 사용하고 있지 않은지 확인합니다. 이 정책이 구현되면 레거시 인증이 차단됩니다.

> [!IMPORTANT]
> 위임된 관리 권한을 사용하여 Exchange Online PowerShell에 연결하는 기능에 영향을 주는 알려진 문제가 있습니다. 이러한 PowerShell 모듈을 사용 중인 경우 이러한 정책을 사용하도록 설정하기 전에 [Exchange Online PowerShell](#exchange-online-powershell)의 알려진 문제를 참조하세요.

#### <a name="end-user-protection"></a>최종 사용자 보호

최종 사용자 보호 기준 정책은 디렉터리의 모든 사용자를 보호합니다. 이 정책이 사용하도록 설정되면 모든 사용자가 14일 내에 Azure MFA에 등록해야 합니다. 등록된 사용자에게는 위험한 로그인 시도 중에만 MFA를 묻는 메시지가 표시됩니다. 손상된 사용자 계정은 암호를 다시 설정하고 위험을 해제할 때까지 차단됩니다.

**기준 정책: 최종 사용자 보호** 정책은 미리 구성된 상태로 제공되며 Azure Portal의 조건부 액세스 블레이드로 이동하면 위쪽에 표시됩니다.

이 정책을 사용하도록 설정하고 사용자를 보호하려면 다음을 수행합니다.

1. 글로벌 관리자, 보안 관리자 또는 조건부 액세스 관리자로 **Azure Portal**에 로그인합니다.
2. **Azure Active Directory** > **조건부 액세스**로 이동합니다.
3. 정책 목록에서 **기준 정책: 최종 사용자 보호(미리 보기)** 를 선택합니다.
4. **정책 사용**을 **즉시 정책 사용**으로 설정합니다.
5. **Save**을 클릭합니다.

> [!WARNING]
> 이 정책을 사용하도록 설정하기 전에 사용자가 레거시 인증 프로토콜을 사용하고 있지 않은지 확인합니다. 이 정책이 구현되면 레거시 인증이 차단됩니다.

> [!IMPORTANT]
> 위임된 관리 권한을 사용하여 Exchange Online PowerShell에 연결하는 기능에 영향을 주는 알려진 문제가 있습니다. 이러한 PowerShell 모듈을 사용 중인 경우 이러한 정책을 사용하도록 설정하기 전에 [Exchange Online PowerShell](#exchange-online-powershell)의 알려진 문제를 참조하세요.

## <a name="assessing-your-environment"></a>환경 평가

현재 파트너 보안 요구 사항 중 하나를 통해 파트너 테넌트의 각 사용자에게 MFA를 적용해야 합니다. 이 요구 사항은 다양한 방법으로 충족될 수 있으므로 추가 작업이 필요한지 여부를 평가하기 어려울 수 있습니다. Azure Active Directory 감사 로그 및 [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)와 같은 도구를 활용하여 MFA로 테넌트를 보호하는 데 추가 작업이 필요한지 평가할 수 있습니다. Microsoft는 파트너 센터의 환경을 사용하여 MFA와 보안 애플리케이션 모델 요구 사항에 대한 빠른 규정 준수 검사를 제공합니다.

Microsoft Secure Score는 강력한 시각화, 다른 Microsoft 제품과의 통합, 다른 회사와의 점수 비교, 범주별로 필터링 등의 기능을 제공합니다. 이 도구를 사용하여 조직 내에서 보안 강화 작업을 완료하고 점수 기록을 추적할 수 있습니다. 또한 타사 솔루션이 권장 개선 작업을 해결한 경우 점수가 반영될 수 있습니다.

![Microsoft Secure Score](images/security/secure-score.png)

> [!NOTE]
> Microsoft Secure Score를 개선하기 위해 수행할 수 있는 작업이 적용되려면 최대 24시간이 걸릴 수 있습니다.

Microsoft Secure Score는 보안 상태에 대한 숫자 표현만 제공합니다. MFA 챌린지에 대한 메시지를 표시하지 않고 인증 대상 또는 주체를 더 잘 이해하려면 Azure Active Directory 감사 로그를 쿼리하는 것이 좋습니다. 이러한 작업은 [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) 모듈과 아래의 스크립트를 사용하여 수행할 수 있습니다. MFA 챌린지에 대한 메시지가 표시되지 않았던 전날에 발생한 인증 시도에 대한 인사이트를 제공하는 보고서가 생성됩니다.

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

위의 스크립트를 실행한 후에는 report.csv 파일에서 세부 정보를 볼 수 있습니다. 여기에는 사용자에게 MFA 챌린지에 대한 메시지가 표시되지 않았던 전날에 발생한 인증 시도 목록이 포함됩니다. 각 항목을 검토하여 올바른 동작인지 확인하고 필요한 경우 작동하는지 확인해야 합니다.

![평가 도구](images/security/assessment-report.png)

## <a name="common-issues"></a>일반적인 문제

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

기준 정책을 사용하도록 설정하면 자동화 또는 통합 시 다음과 같은 예외가 발생하는 것을 알 수 있습니다.

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

이 예외가 발생하는 이유는 이제 MFA가 필요한데 사용자 자격 증명을 사용하여 인증하고 있기 때문입니다. 이 예외를 해결하려면 인증용 액세스 토큰을 활용해야 합니다. 자세한 내용은 [보안 애플리케이션 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)를 참조하세요.

>[!IMPORTANT]
>최신 API 및 PowerShell 모듈은 인증용 액세스 토큰을 활용하는 기능을 지원합니다. 그러나 현재 이 기능을 지원하지 않는 API 및 PowerShell 모듈도 있습니다. 활용하려는 API 또는 PowerShell 모듈이 인증용 액세스 토큰 사용을 지원하는지 확인하는 데 도움이 필요한 경우 [파트너 센터 보안 지침 그룹](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 커뮤니티에 메시지를 게시하세요.

#### <a name="aadsts700082"></a>AADSTS700082

보안 애플리케이션 모델 프레임워크를 구현하고 초기 새로 고침 토큰을 생성한 후 90일이 지나면 다음 예외가 발생할 가능성이 있습니다.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Azure Active Directory를 기준으로 새로 고침 토큰의 최대 수명은 90일입니다. 이 오류를 해결하려면 새 새로 고침 토큰을 생성하고 안전하게 저장해야 합니다. Azure Active Directory에 액세스 토큰에 대한 요청이 있을 때마다 새 새로 고침 토큰이 반환되기 때문에 새로 고침 토큰을 프로그래밍 방식으로 업데이트할 수 있습니다. 만료되기 전에 안전하게 저장된 새로 고침 토큰을 업데이트하는 적절한 논리를 구현할 수 있습니다.

자세한 내용은 [Azure Active Directory의 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)을 참조하세요.

### <a name="recovering-compromised-accounts"></a>손상된 계정 복구

Microsoft의 유출된 자격 증명 서비스는 고객을 보호하기 위해 공개적으로 사용할 수 있는 사용자 이름/암호 쌍을 찾습니다. 사용자 중 하나와 일치하는 계정을 즉시 보호하는 데 도움이 됩니다. 유출된 자격 증명이 있는 것으로 식별된 사용자는 손상된 것으로 확인됩니다. 이러한 사용자는 암호를 다시 설정할 때까지 로그인이 차단됩니다.

Azure AD Premium 라이선스를 할당받은 사용자는 셀프 서비스 암호 재설정(SSPR)을 통해 액세스를 복원할 수 있습니다(해당 디렉터리에 이 기능이 사용하도록 설정된 경우). 차단된 프리미엄 라이선스가 없는 사용자는 관리자에게 문의하여 수동 암호 재설정을 수행하고 플래그가 지정된 사용자 위험 이벤트를 해제해야 합니다.

#### <a name="steps-to-unblock-a-user"></a>사용자 차단 해제 단계

사용자의 로그인 로그를 검사하여 사용자가 정책에 의해 차단되었는지 확인합니다.

1. 관리자는 **Azure Portal**에 로그인하고 **Azure Active Directory** > **사용자**로 이동하여 사용자 이름을 클릭하고 로그인으로 이동합니다.
2. 차단된 사용자에 대한 암호 재설정을 시작하려면 관리자가 **Azure Active Directory** > **위험 플래그가 지정된 사용자**로 이동해야 합니다.
3. 계정이 차단된 사용자를 클릭하여 사용자의 최근 로그인 활동에 대한 정보를 볼 수 있습니다.
4. 다음 로그인 시 변경해야 할 임시 암호를 할당하려면 암호 재설정을 클릭합니다.
5. 모든 이벤트 해제를 클릭하여 사용자의 위험 점수를 다시 설정합니다.

이제 사용자가 로그인하여 암호를 재설정하고 애플리케이션에 액세스할 수 있습니다.

## <a name="known-issues"></a>알려진 문제

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

MFA가 적용되면 파트너는 Exchange Online PowerShell을 통해 위임된 관리 권한을 활용하여 고객에 대한 작업을 수행할 수 없습니다. 이러한 제한 사항에 대한 자세한 내용은 [다단계 인증을 사용하여 Exchange Online PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)을 참조하세요.

새 계정을 만든 후 해당 계정을 사용하여 대화형 인증을 수행하지 않으면 이 제한 사항을 해결할 수 있습니다. [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/)을 활용하여 새 계정을 만들고 초기 구성을 수행하는 것이 좋습니다. 다음 PowerShell을 사용하여 계정을 만들고 구성할 수 있습니다.

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

다음에 PowerShell을 통해 Exchange Online에 연결할 때 이 계정을 사용하면 계정이 올바르게 작동합니다.

> [!IMPORTANT]
> MFA가 적용되면 파트너가 Exchange Online PowerShell을 통해 위임된 관리 권한을 활용하여 고객에 대한 작업을 수행하는 기능을 나중에 사용할 수 있게 됩니다. 그때까지 이 문제를 해결해야 합니다.

## <a name="resources-and-support"></a>리소스 및 지원

[파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)를 통해 추가 리소스를 찾고 기술 업무 시간 등의 예정된 이벤트에 대해 알아볼 수 있습니다. 요구 사항에 대해 자세히 알아보려면 [질문과 대답](partner-security-requirements-faq.md) 문서를 참조하세요.
