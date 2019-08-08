---
title: 파트너 보안 요구 사항 | 파트너 센터
ms.topic: article
ms.date: 08/05/2019
description: 클라우드 솔루션 공급자 프로그램에 참여 하는 관리자 및 파트너에 대 한 보안 요구 사항에 대해 알아봅니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급 업체, CPV, multi-factor authentication, MFA, 보안 응용 프로그램 모델, 보안 앱 모델, 보안
ms.localizationpriority: medium
ms.openlocfilehash: 39081f42c326665bdc30bf25df302d9ae00d9723
ms.sourcegitcommit: fe21430f96e203d279714623888224662d2782a2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2019
ms.locfileid: "68787252"
---
# <a name="partner-security-requirements"></a>파트너 보안 요구 사항

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 제어판 공급 업체
- 모든 관리자

개인 정보 보호 및 보안은 가장 높은 우선 순위에 있습니다. 가장 좋은 방어는 방지 하 고 가장 약한 링크 만큼만 강력 하다는 것을 알고 있습니다. 즉, 에코 시스템의 모든 사용자가 적절 한 보안 보호 기능을 제공 해야 합니다. 파트너와 고객을 보호 하기 위해 클라우드 솔루션 공급자 프로그램에 참여 하는 관리자, 제어판 공급 업체 및 파트너에 대 한 필수 보안 요구 사항 집합을 소개 합니다.

2019 년 8 월 1 일부 터 모든 파트너는 서비스 계정을 비롯 한 모든 사용자에 게 multi-factor authentication을 적용 하는 데 필요 합니다.

> [!NOTE]
> 소 버린 클라우드 (21Vianet, 미국 정부 및 독일)를 통해 거래 하는 모든 파트너는 이러한 새 보안 요구 사항을 즉시 적용 하 고 채택 하는 것이 좋습니다. 그러나 이러한 파트너는 2019 년 8 월 1 일부 터 적용 되는 새로운 보안 요구 사항을 충족 하는 데 필요 하지 않습니다. Microsoft는 나중에 소 버린 클라우드에 대해 이러한 보안 요구 사항을 적용 하는 것과 관련 된 추가 세부 정보를 제공 합니다.

파트너 보안 요구 사항과 관련 된 용어는 [클라우드 솔루션 공급자 프로그램 가이드](https://go.microsoft.com/fwlink/p/?LinkId=617100)에 추가 되었습니다. 2019 년 8 월 1 일부 터 클라우드 솔루션 공급자 프로그램에 참여 하는 모든 파트너가 약관을 준수 해야 합니다. 관리자와 관련이 있으므로 동일한 계약 요구 사항이 적용 됩니다.

필수 보안 요구 사항을 구현 하지 않는 파트너는 이러한 요구 사항이 적용 되 면 클라우드 솔루션 공급자 프로그램을 실행 하거나 위임 관리자 권한을 활용 하는 고객 테 넌 트를 관리할 수 없습니다. Microsoft는 요구 사항에 대 한 기술 적용 날짜를 설정 하는 과정을 진행 중 이며, 파트너에 게 자세한 정보를 제공 합니다.

## <a name="what-actions-do-i-need-to-take"></a>수행 해야 하는 작업은 무엇 인가요?

파트너의 매우 높은 권한이 있는 경우 각 사용자에 게 모든 단일 인증에 대 한 MFA 챌린지를 제공 해야 합니다. 다음 방법 중 하나를 통해 수행할 수 있습니다.

- Azure AD Premium를 구현 하 고 MFA가 각 사용자에 게 적용 되는지 확인
- [기준 보호 정책](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) 구현
- 타사 솔루션을 구현 하 고 각 사용자에 대해 MFA를 적용 하는지 확인

> [!IMPORTANT]
> 이러한 요구 사항을 기술적으로 적용 한 후에는 모든 단일 인증에 MFA 챌린지가 있어야 합니다. Microsoft 상용 클라우드 서비스에 액세스할 때 MFA를 사용 하 여 인증을 방지 하기 위해 조건부 액세스의 모든 기능을 사용할 수는 없습니다.

### <a name="considerations"></a>고려 사항

이러한 요구 사항은 파트너 테 넌 트에서 서비스 계정을 비롯 한 모든 사용자에 게 적용 되므로 원활한 배포를 위해 수행 해야 할 몇 가지 고려 사항이 있습니다. 이러한 고려 사항에는 MFA를 수행할 수 없는 Azure AD의 사용자 및 최신 인증을 지원 하지 않는 조직에서 사용 하는 응용 프로그램 및 장치를 식별 하는 작업이 포함 됩니다.

작업을 수행 하기 전에 다음을 확인 하는 것이 좋습니다.

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>인증할 때 MFA 사용을 지원 하지 않는 응용 프로그램 또는 장치가 있나요?

MFA 레거시 인증을 적용 하는 경우 이러한 프로토콜이 MFA를 지원 하지 않으므로 IMAP, POP3, SMTP 등의 프로토콜을 사용 하는 것이 차단 됩니다. 이러한 제한을 해결 하기 위해 [앱 암호](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) 라고 하는 기능을 사용 하 여 응용 프로그램 또는 장치에서 인증을 받을 수 있는지 확인할 수 있습니다. 환경에서 사용할 수 있는지 확인 하려면 [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) 에 설명 된 앱 암호 사용에 대 한 고려 사항을 검토 해야 합니다.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>파트너 테 넌 트와 연결 된 라이선스에서 제공 하는 Office 365를 사용 하는 사용자가 있나요?

솔루션을 구현 하기 전에 파트너 테 넌 트의 사용자가 Microsoft Office 버전을 사용 하는 이유를 확인 하는 것이 좋습니다. 작업을 수행 하기 전에 [Office 365 배포에 대 한 multi-factor authentication 계획을](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) 검토 합니다. 사용자가 Outlook과 같은 응용 프로그램의 연결 문제를 경험 하 게 될 가능성이 있습니다. MFA를 적용 하기 전에 Outlook 2013 SP1 이상을 사용 하 고 조직에서 최신 인증을 사용 하도록 설정 했는지 확인 해야 합니다. 자세한 내용은 [Exchange Online에서 최신 인증 사용](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) 을 참조 하세요.

Microsoft Office 2013가 설치 된 Windows를 실행 하는 모든 장치에 대 한 최신 인증을 사용 하도록 설정 하려면 두 개의 레지스트리 키를 만들어야 합니다. [Windows 장치에서 Office 2013에 대 한 최신 인증 사용](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)을 참조 하세요.

> [!IMPORTANT]
> 사용자에 게 Azure AD MFA를 사용 하도록 설정 하 고 최신 인증을 사용 하도록 설정 되지 않은 Office 2013를 실행 하는 장치가 있는 경우 해당 장치에서 앱 암호를 사용 해야 합니다. 앱 암호에 대 한 자세한 내용 및 사용 해야 하는 경우/위치 및 사용 방법에 대 한 자세한 내용은 다음을 참조 하세요. [Azure Multi-factor Authentication을 사용 하는 앱 암호](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>작업 하는 동안 사용자가 모바일 장치를 사용할 수 없도록 하는 정책이 있나요?

직원이 모바일 장치를 사용 하지 못하도록 하는 회사 정책을 식별 하는 것은 구현 하는 MFA 솔루션에 영향을 주므로 회사 정책을 식별 하는 것이 중요 합니다. 인증을 위해 인증 앱을 사용 하도록 허용 하는 [기본 보호 정책의](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)구현을 통해 제공 되는 것과 같은 MFA 솔루션이 있습니다. 조직의 모바일 장치 사용을 방해 하는 정책이 있는 경우 다음 옵션 중 하나를 고려해 야 합니다.

- Authenticator 앱을 설치할 수 있는 가상화 된 Android 장치 배포
- 가장 적절 한 인증 옵션을 제공 하는 파트너 테 넌 트의 각 사용자에 대해 MFA를 적용 하는 타사 솔루션을 구현 합니다.
- 영향을 받는 사용자에 대 한 [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) 라이선스 구매

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>인증을 위해 사용자 자격 증명을 활용 하는 자동화 또는 통합은 무엇 인가요?

서비스 계정을 비롯 하 여 각 사용자에 대해 MFA를 적용 하는 것이 요구 사항 이므로 인증을 위해 사용자 자격 증명을 활용 하는 모든 automation 또는 통합은 영향을 받습니다. 따라서 이러한 상황에서 사용 되는 계정을 식별 하는 것이 중요 합니다. 다음은 고려해 야 할 응용 프로그램 또는 서비스의 예제 목록입니다.

- 고객을 대신 하 여 리소스를 프로 비전 하는 데 사용 되는 제어판
- 청구에 사용 되는 모든 플랫폼과의 통합 (CSP 프로그램과 관련) 및 고객 지원
- Az, AzureRM, Azure AD, MS Online 등을 활용 하는 PowerShell 스크립트

위의 목록은 포괄적이 지 않습니다. 따라서 사용자 환경에서 인증에 대 한 사용자 자격 증명을 활용 하는 응용 프로그램 또는 서비스에 대 한 완전 한 평가를 수행 하는 것이 중요 합니다. MFA 요구 사항에 경합 하려면 가능한 경우 [보안 응용 프로그램 모델 프레임 워크](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) 에서 지침을 구현 해야 합니다. 보안 응용 프로그램 모델 프레임 워크를 구현할 수 있는 방법을 이해 하는 데 도움이 되는 추가 리소스는 다음과 같습니다.

- [파트너 센터 .Net 샘플](https://github.com/microsoft/partner-center-dotnet-samples) -이 GitHub 리포지토리에는 .net을 사용 하 여 개발 된 샘플이 포함 되어 보안 응용 프로그램 모델 프레임 워크를 구현할 수 있는 방법을 보여 줍니다.
- [파트너 센터 Java 샘플](https://github.com/microsoft/partner-center-java-samples) -이 GitHub 리포지토리에는 java를 사용 하 여 개발 된 샘플이 포함 되어 있으며,이를 통해 보안 응용 프로그램 모델 프레임 워크를 구현할 수 있는 방법을 보여 줍니다.
- [파트너 센터 powershell-보안 응용 프로그램 모델](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) -powershell을 사용 하 여 보안 응용 프로그램 모델 프레임 워크를 구현 하는 방법에 대 한 세부 정보를 제공 하는 문서입니다.
- [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) -예정 된 이벤트를 학습 하 고 있을 수 있는 질문을 할 수 있는 온라인 커뮤니티입니다.

### <a name="enforcing-mfa-for-all-users"></a>모든 사용자에 대해 MFA 적용

이 섹션에서는 [기준 보호 정책을](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) 사용 하 여 파트너 테 넌 트에서 서비스 계정을 비롯 한 각 사용자에 대해 MFA를 적용 하는 방법을 설명 합니다. Azure AD Premium를 사용 하려는 경우 [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)에 설명 된 단계를 따르세요.

> [!NOTE]
> Azure AD와 호환 되는 타사 솔루션을 사용 하 여 서비스 계정을 비롯 한 모든 사용자에 대해 MFA를 적용할 수 있습니다. 솔루션을 구현 하는 방법에 대 한 자세한 내용은 공급 업체의 설명서를 참조 하세요.

기준 보호 정책은 여러 일반적인 공격 으로부터 조직을 보호 하는 데 도움이 되는 미리 정의 된 정책 집합입니다. 이러한 일반적인 공격은 암호 스프레이, 재생 및 피싱을 포함할 수 있습니다. 기본 보호 정책은 모든 버전의 Azure Active Directory에서 사용할 수 있습니다. Microsoft는 고객과 파트너가 최고의 보안 사례를 구현할 수 있도록 모든 사용자가 이러한 기본 보호 정책을 사용할 수 있도록 합니다.

사용 하도록 설정 해야 하는 두 가지 기준 보호 정책은 아래 표에 설명 되어 있습니다.

|**정책**| |
|-----|-----|
|**관리자 용 MFA 필요**|관리자에 대해 MFA 필요 정책을 사용 하도록 설정 하면 관리자 역할의 사용자가 Authenticator 앱을 사용 하 여 MFA에 등록 해야 합니다. MFA 등록이 완료 되 면 관리자가 로그인 할 때마다 MFA를 수행 해야 합니다.|
|**최종 사용자 보호**|최종 사용자 보호는 디렉터리의 모든 사용자를 보호 하는 위험 기반 MFA 기준 보호 정책입니다. 이 정책을 사용 하도록 설정 하려면 모든 사용자가 Authenticator 앱을 사용 하 여 MFA에 등록 해야 합니다. 사용자는 mfa 등록 프롬프트를 14 일 동안 무시할 수 있으며 그 후에는 MFA에 등록 하기 전까지 로그인이 차단 됩니다. MFA에 등록 되 면 사용자에 게 위험한 로그인 시도 중에만 MFA를 묻는 메시지가 표시 됩니다. 손상 된 사용자 계정은 해당 암호를 다시 설정 하 고 위험 이벤트를 해제할 때까지 차단 됩니다.|

이러한 정책을 사용 하는 경우 각 사용자는 추가 비용 없이 인증을 위해 Authenticator 앱을 사용 하 여 Azure MFA를 활용할 수 있습니다.

#### <a name="configure-self-service-password-reset"></a>셀프 서비스 암호 재설정 구성

SSPR (셀프 서비스 암호 재설정)는 사용자가 지원 팀에 문의할 필요 없이 암호를 재설정할 수 있도록 하는 Azure Active Directory 기능입니다. 사용자는 서비스를 사용 하기 전에 셀프 서비스 암호 재설정을 위해 등록 하거나 등록 해야 합니다. 등록 하는 동안 사용자는 조직에서 사용 하도록 설정 된 하나 이상의 인증 방법을 선택 합니다.

[최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 보호 정책을 사용 하도록 설정 하면 암호를 다시 설정 하 고 위험 이벤트를 해제할 때까지 손상 된 모든 사용자 계정이 차단 됩니다. 이를 고려 하는 경우 전역 관리자 인 각 사용자는 다음을 수행 하 여 SSPR에 등록 하 여 잠기지 않도록 하는 것이 좋습니다.

1. [SSPR 설정 페이지로](https://aka.ms/ssprsetup) 이동 합니다.
2. 사용자 이름 및 암호 입력
3. 암호를 재설정할 때 사용자를 확인 하는 데 사용할 확인 옵션 중 하나 이상을 구성 합니다.  

계정이 손상 되 면 관리자는 영향을 받는 사용자에 대 한 액세스를 복원 하는 조치를 취해야 합니다. 사용자를 차단 해제 하는 프로세스에 대 한 세부 정보는 [사용자의 차단을 해제 하는 단계를](#recovering-compromised-accounts) 참조 하세요.

#### <a name="require-mfa-for-admins"></a>관리자 용 MFA 필요

*관리 기준에 Mfa 필요* 정책에는 다음 디렉터리 역할에 대 한 mfa가 필요 하며, 가장 권한 있는 Azure Active Directory 역할로 간주 됩니다.

- 전역 관리자
- SharePoint 관리자
- Exchange 관리자
- 조건부 액세스 관리자
- 보안 관리자
- 기술 지원팀 관리자/암호 관리자
- 대금 청구 관리자
- 사용자 관리자

관리자에 대해 MFA 필요 정책을 사용 하도록 설정 하면 위의 9 개 관리자 역할이 인증 앱을 사용 하 여 MFA에 등록 해야 합니다. MFA 등록이 완료 되 면 관리자는 로그인 할 때마다 MFA를 수행 해야 합니다.

조직에서 스크립트나 코드에 이러한 계정을 사용 하는 경우 [관리 되는 id](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)로 대체 하는 것이 좋습니다.

이 정책을 사용 하도록 설정 하 고 관리자를 보호 하려면 다음을 수행 합니다.

1. 전역 관리자, 보안 관리자 또는 조건부 액세스 관리자 권한으로 **Azure Portal** 에 로그인 합니다.
2. **Azure Active Directory** > **조건부 액세스**로 이동 합니다.
3. 정책 목록에서 기준 정책을 선택 **합니다. 관리자**용 MFA를 요구 합니다.
4. 정책 **사용을 즉시 정책**사용으로 설정 합니다.
5.  **저장**을 클릭 합니다.

> [!WARNING]
> 이 정책을 사용 하도록 설정 하기 전에 사용자가 레거시 인증 프로토콜을 사용 하 고 있지 않은지 확인 합니다. 이 정책의 구현을 통해 레거시 인증이 차단 됩니다.

> [!IMPORTANT]
> 위임 된 관리 권한을 사용 하 여 Exchange Online PowerShell에 연결 하는 기능에 영향을 주는 알려진 문제가 있습니다. 이 PowerShell 모듈을 사용 하는 경우이 정책을 사용 하도록 설정 하기 전에 [Exchange Online PowerShell](#exchange-online-powershell) 의 알려진 문제를 참조 하세요.

#### <a name="end-user-protection"></a>최종 사용자 보호

최종 사용자 보호 기준 정책은 디렉터리의 모든 사용자를 보호 합니다. 이 정책을 사용 하도록 설정 하려면 모든 사용자가 14 일 내에 Azure MFA에 등록 해야 합니다. 등록 한 후에는 사용자에 게 위험한 로그인 시도 중에만 MFA를 입력 하 라는 메시지가 표시 됩니다. 손상 된 사용자 계정은 암호 재설정 및 위험 해제 될 때까지 차단 됩니다.

정책 **기준 정책: 최종 사용자 보호** 는 미리 구성 되어 있으며 Azure Portal의 조건부 액세스 블레이드로 이동 하면 위쪽에 표시 됩니다.

이 정책을 사용 하도록 설정 하 고 사용자를 보호 하려면:

1. 전역 관리자, 보안 관리자 또는 조건부 액세스 관리자 권한으로 **Azure Portal** 에 로그인 합니다.
2. **Azure Active Directory** > **조건부 액세스**로 이동 합니다.
3. 정책 목록에서 기준 정책을 선택 **합니다. 최종 사용자 보호 (미리 보기**).
4. 정책 **사용을 즉시 정책**사용으로 설정 합니다.
5.  **저장**을 클릭 합니다.

> [!WARNING]
> 이 정책을 사용 하도록 설정 하기 전에 사용자가 레거시 인증 프로토콜을 사용 하 고 있지 않은지 확인 합니다. 이 정책의 구현을 통해 레거시 인증이 차단 됩니다.

> [!IMPORTANT]
> 위임 된 관리 권한을 사용 하 여 Exchange Online PowerShell에 연결 하는 기능에 영향을 주는 알려진 문제가 있습니다. 이 PowerShell 모듈을 사용 하는 경우이 정책을 사용 하도록 설정 하기 전에 [Exchange Online PowerShell](#exchange-online-powershell) 의 알려진 문제를 참조 하세요.

## <a name="common-issues"></a>일반적인 문제

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

기준 정책을 사용 하도록 설정 하면 다음과 같은 예외가 발생 하는 것을 알 수 있습니다.

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

이 예외가 발생 하는 이유는 사용자 자격 증명을 사용 하 여 인증 하 고 MFA가 필요 하기 때문입니다. 이 예외를 해결 하려면 인증을 위해 액세스 토큰을 활용 해야 합니다. 자세한 내용은 [보안 응용 프로그램 모델 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 를 참조 하세요.

>[!IMPORTANT]
>최신 Api 및 PowerShell 모듈은 인증을 위해 액세스 토큰을 활용 하는 기능을 지원 합니다. 그러나 현재이 기능을 지원 하지 않는 몇 가지 방법이 있습니다. 활용 하려는 API 또는 PowerShell 모듈이 인증에 대 한 액세스 토큰 사용을 지원 하는지 확인 하는 데 도움이 필요한 경우 [파트너 센터 보안 지침 그룹](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 커뮤니티에 메시지를 게시 합니다.

#### <a name="aadsts700082"></a>AADSTS700082

보안 응용 프로그램 모델 프레임 워크를 구현한 후에는 초기 새로 고침 토큰을 생성 한 후 90 일 후에 다음 예외가 발생할 가능성이 있습니다.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Azure Active Directory를 기준으로 새로 고침 토큰의 최대 수명은 90 일입니다. 이 오류를 해결 하려면 새 새로 고침 토큰을 생성 하 고 안전 하 게 저장 해야 합니다. 액세스 토큰에 대 한 Azure Active Directory 요청이 있을 때마다 새 새로 고침 토큰이 반환 되기 때문에 새로 고침 토큰을 프로그래밍 방식으로 업데이트할 수 있습니다. 만료 되기 전에 안전 하 게 저장 된 새로 고침 토큰을 업데이트 하는 적절 한 논리를 구현할 수 있습니다.

자세한 내용은 [Azure Active Directory 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 을 참조 하세요.

### <a name="recovering-compromised-accounts"></a>손상 된 계정 복구

Microsoft의 누출 자격 증명 서비스는 고객을 보호 하기 위해 공개적으로 사용할 수 있는 사용자 이름/암호 쌍을 찾습니다. 사용자 중 하 나와 일치 하는 경우 해당 계정을 즉시 보호 하는 데 도움이 됩니다. 누출 된 자격 증명이 있는 것으로 확인 된 사용자가 손상 된 것으로 확인 됩니다. 이러한 사용자는 암호를 다시 설정할 때까지 로그인이 차단 됩니다.

해당 디렉터리에서 기능을 사용 하도록 설정한 경우 Azure AD Premium 라이선스를 할당 받은 사용자는 셀프 서비스 암호 재설정 (SSPR)을 통해 액세스를 복원할 수 있습니다. 차단 될 프리미엄 라이선스가 없는 사용자는 관리자에 게 문의 하 여 수동 암호 재설정을 수행 하 고 플래그가 지정 된 사용자 위험 이벤트를 해제 해야 합니다.

#### <a name="steps-to-unblock-a-user"></a>사용자를 차단 해제 하는 단계

사용자의 로그인 로그를 검사 하 여 사용자가 정책에 의해 차단 되었는지 확인 합니다.

1. 관리자는 **Azure Portal** 에 로그인 하 고 **Azure Active Directory** > >**사용자** 로 이동 하 여 사용자의 이름을 클릭 하 고 로그인으로 이동 해야 합니다.
2. 차단 된 사용자에 대해 암호 재설정을 시작 하려면 관리자가**위험 플래그가 지정** 된 **Azure Active Directory** > 사용자로 이동 해야 합니다.
3. 계정이 차단 된 사용자를 클릭 하 여 사용자의 최근 로그인 활동에 대 한 정보를 볼 수 있습니다.
4. 다음 로그인 시 변경 해야 할 임시 암호를 할당 하려면 암호 다시 설정을 클릭 합니다.
5. 모든 이벤트 해제를 클릭 하 여 사용자의 위험 점수를 다시 설정 합니다.

이제 사용자는 로그인 하 여 암호를 재설정 하 고 응용 프로그램에 액세스할 수 있습니다.

## <a name="known-issues"></a>알려진 문제

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

MFA가 적용 되 면 파트너는 Exchange Online PowerShell을 통해 위임 된 관리 권한을 활용 하 여 고객에 대 한 작업을 수행할 수 없습니다. 이러한 제한 사항에 대 한 자세한 내용은 [다단계 인증을 사용 하 여 Exchange Online PowerShell에 연결을](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) 참조 하세요.

새 계정을 만들고 대화형 인증을 수행 하는 데이 계정을 사용 하지 않으면이 제한을 해결할 수 있습니다. [AZURE AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) 을 활용 하 여 새 계정을 만들고 초기 구성을 수행 하는 것이 좋습니다. 다음 PowerShell을 사용 하 여 계정을 만들고 구성할 수 있습니다.

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

다음에 PowerShell을 통해 Exchange Online에 연결 하는 경우이 계정을 사용 하 여 예상 대로 작동 합니다.

> [!IMPORTANT]
> 사용자가 MFA를 적용할 때 Exchange Online PowerShell에서 위임 된 관리 권한을 활용 하 여 고객에 대 한 작업을 수행할 수 있는 기능은 나중에 제공 될 예정입니다. 그때까지이 문제를 해결 해야 합니다.

## <a name="resources-and-support"></a>리소스 및 지원

[파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 를 통해 추가 리소스를 찾고 기술 사무실 시간 등의 예정 된 이벤트에 대해 알아볼 수 있습니다. 요구 사항에 대해 자세히 알아보려면 질문과 [대답](partner-security-requirements-faq.md) 문서를 참조 하세요.
