---
title: 보안 요구 사항을 파트너 | 파트너 센터
ms.topic: article
ms.date: 06/25/2019
description: 회사의 고문 및 클라우드 솔루션 공급자 프로그램에 참여 하는 파트너에 대 한 보안 요구 사항에 알아봅니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램을 컨트롤 패널 공급 업체, CSP, CPV, multi-factor authentication에 MFA 보안 응용 프로그램 모델, 안전한 앱 모델, 보안
ms.localizationpriority: medium
ms.openlocfilehash: 8f513b96619819cd6ba892625e47731170d22130
ms.sourcegitcommit: de88bb4cd994f1a106a5d02242261042958d4300
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2019
ms.locfileid: "67549533"
---
# <a name="partner-security-requirements"></a>파트너 보안 요구 사항

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 컨트롤에 대 한 패널 공급 업체
- 모든 관리자

보안 및 개인 고객 및 파트너의 Microsoft에 대 한 최상위 우선 순위 이며 주로 손상 된 id와 관련 된 보다 복잡 한 보안 공격의 증가를 계속 합니다. 보안 공격을 막기 위해 전체 방어 전략에서 키 역할을 수행 하는 예방적 컨트롤에 따라 다양 한 파트너 및 고객을 보호 하기 위해 필수 보안 요구 사항 적용 시작 합니다.

> [!NOTE]
> 소 버린 클라우드 (21Vianet US Government 및 Germany)를 통해 구속력 있는 모든 파트너 역할을 즉시 이러한 새 보안 요구 사항을 채택 하는 것이 좋습니다. 그러나 이러한 파트너는 2019 년 8 월 1 일 적용 새 보안 요구 사항을 충족 필요가 없습니다. Microsoft는 향후 소 버린 클라우드에 대 한 이러한 보안 요구 사항 적용에 대 한 추가 세부 정보를 제공 합니다.

## <a name="overview-of-the-requirements"></a>요구 사항의 개요

클라우드 솔루션 공급자 프로그램, 컨트롤 패널 공급 업체 및 관리자 파트너에 참여 하는 모든 파트너는 파트너 테 넌 트의 서비스 계정을 포함 하 여 각 사용자에 대해 Multi-factor Authentication (MFA)을 적용 해야 합니다. 두 개를 사용 하 여 이렇게 [Azure Active Directory 기준 정책을](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)합니다. 기본 정책은 조직에서는 여러 일반적인 공격 으로부터 보호 하는 미리 정의 된 정책 집합. 이러한 일반적인 공격 암호 스프레이, 재생 및 피싱에 포함할 수 있습니다. 기본 정책은 Azure Active Directory의 모든 버전에서 사용할 수 있습니다. Microsoft 기본 보호 정책은 이러한에서 제공 하 추가에서 최고의 보안 사례를 구현 하는 고객 및 파트너를 사용 하도록 설정 하려면 모든 사용자에 게 합니다.

두 기준 정책은 활성화 해야 하는 아래 표에 설명 되어 있습니다.

|**정책**| |
|-----|-----|
|**관리자에 대해 MFA 요구**|관리자 정책에 대 한 필요한 MFA를 사용 하도록 설정한 관리자 역할의 사용자를 Authenticator 앱을 사용 하 여 MFA에 등록 해야 합니다. MFA 등록이 완료 되 면 관리자가 MFA를 수행할 때마다 로그인 해야 합니다.|
|**최종 사용자 보호**|최종 사용자 보호는 디렉터리의 모든 사용자를 보호 하는 위험 기반 MFA 기본 정책입니다. 이 정책을 사용 하면 Authenticator 앱을 사용 하 여 MFA에 등록 하는 모든 사용자가 필요 합니다. 사용자는 차단 됩니다 MFA에 등록 될 때까지 로그인에서 14 일간 MFA 등록 프롬프트를 무시할 수 있습니다. MFA에 등록 되 면 위험한 로그인 시도 하는 동안에 사용자 MFA에 대 한 메시지가 표시 됩니다. 손상 된 사용자 계정 암호 다시 설정 되 고 위험 이벤트 해제 된 될 때까지 차단 됩니다.|

이러한 정책을 사용할 경우 각 사용자를 추가 비용 없이 Azure MFA를 사용할 수 있게 됩니다. 타사 솔루션을 사용 하는 경우 Microsoft 상용 클라우드 서비스에 액세스 하는 경우 각 사용자에 대 한 MFA를 적용할 필요가 됩니다.

> [!IMPORTANT]
> 파트너 디렉터리에 모든 사용자에 대 한 MFA를 적용 하므로 모든 자동화 및 사용자 자격 증명을 활용 하는 통합에 영향을 미칠이 됩니다 수 있습니다. 이 영향을 해결 하기 위해 프로그램 automation 또는 통합 Microsoft 상용 클라우드 서비스에 연결 하는 방법을 수정 해야 합니다. 구현 하는 것이 좋습니다. 경우에 연결 하는 서비스는 토큰 기반된 인증을 지원 합니다 [응용 프로그램 모델 보안 프레임 워크](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)합니다.

## <a name="what-actions-do-i-need-to-take"></a>작업을 수행 하나요? 

파트너 테 넌 트의 사용자는 보호 되도록 각 사용자 (서비스 계정 포함)에 대 한 MFA를 적용 해야 합니다. 사용 하 여이 작업을 수행할 수 있습니다 합니다 [관리자에 대 한 MFA를 요구](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 하 고 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책을 합니다. 가 이러한 정책은 사용 하도록 설정 하기 전에 수행할 작업 및 어떤 영향을 미치는지 모든 자동화 및 통합 사용자에 게 이해 해야 합니다.

> [!NOTE]
> [기본 정책은](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) 초과 개선 될 것입니다. 정책의 발전에 대 한 자세한 설명서를 주기적으로 검토 하는 것이 좋습니다.

### <a name="considerations"></a>고려 사항

파트너 디렉터리에 모든 사용자에 게 보안 요구 사항을 적용 하기 때문에 원활한 배포에 대 한 몇 가지 고려 사항이 필요 합니다. 이 고려할 사항 없거나 응용 프로그램 및 최신 인증을 지원 하지 않는 조직에서 사용 하는 클라이언트와 함께 MFA를 수행 하지 않아야 하는 Azure Active Directory에서 사용자를 식별 합니다.

#### <a name="self-service-password-reset"></a>셀프 서비스 암호 재설정

셀프 서비스 암호 재설정 (SSPR)에 IT 직원에 게 문의 하지 않고도 암호를 재설정할 수 있는 Azure Active Directory 기능입니다. 직원에 대 한 등록 해야 합니다 또는 셀프 서비스 암호 재설정 서비스를 사용 하 여 등록 합니다. 등록 하는 동안 직원이 조직에서 사용 하도록 설정 하는 하나 이상의 인증 방법을 선택 합니다.

SSPR에는 직원 들을 빠르게 차단을 위치 또는 하루 중 시간에 관계 없이 작업을 계속할 수 있습니다. 를 허용 자체를 차단 해제 하 여 조직의 생산성 아닌 시간 및 가장 일반적인 암호 관련 문제에 대 한 높은 지원 비용을 줄일 수 있습니다.

경우는 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책을 사용 하는 손상 된 사용자 계정 암호 다시 설정 되 고 위험 이벤트 해제 된까지 차단 됩니다. 이러한 점을 고려 것이 좋습니다 SSPR에 등록 하려면 다음을 수행 하는 각 사용자에 게 전역 관리자 인

1. 이동 된 [SSPR 설치 페이지](https://aka.ms/ssprsetup)
2. 사용자 이름 및 암호를 입력 합니다.
3. 암호를 재설정할 때 사용자를 확인 하는 데 사용할 확인 옵션 중 하나 이상을 구성 합니다.  

계정이 손상 된 경우 관리자가 영향을 받는 사용자에 대 한 액세스를 복원 하는 작업을 수행 해야 합니다. 참조를 [차단을 해제 하는 단계](#recovering-compromised-accounts) 사용자 차단을 해제 하는 프로세스에 대 한 자세한 내용은 합니다.

#### <a name="legacy-protocols"></a>레거시 프로토콜

레거시 인증 프로토콜 (예: IMAP, SMTP, POP3, 등)는 인증 요청을 메일 클라이언트에서 사용 됩니다. 이러한 프로토콜에서 MFA를 지원 하지 않습니다. 계정 손상 대부분이 MFA를 바이패스 하는 동안 레거시 프로토콜에 대 한 공격을 수행 하는 잘못 된 행위자가 발생 합니다. 파트너 디렉터리의 계정에 로그인 할 때 MFA가 필요한 및 믿지 못할 자에 MFA를 바이패스 하 수 없는 되도록 이러한 보안 요구 사항에는 레거시 프로토콜의 모든 인증 요청을 차단 합니다.

### <a name="enabling-the-baseline-policies"></a>기준 정책을 사용 하도록 설정

참조를 [파트너 보안 요구 사항 자습서 구현](tutorials/partner-security-requirements.yml) 기준 정책 구현에 대 한 단계별된 환경에 대 한 합니다.  

#### <a name="require-mfa-for-admins"></a>관리자에 대해 MFA 요구

합니다 *관리자에 대 한 MFA를 요구* 기준 정책을 가장 권한이 있는 Azure Active Directory 역할을 할 것으로 간주 하는 다음 디렉터리 역할에 대 한 MFA를 요구 합니다.

- 전역 관리자
- SharePoint 관리자
- Exchange 관리자
- 조건부 액세스 관리자
- 보안 관리자
- 기술 지원팀 관리자 / 암호 관리자
- 대금 청구 관리자
- 사용자 관리자

관리자 정책에 대 한 필요한 MFA를 사용 하도록 설정 하면, 위의 9 관리자 역할에 Authenticator 앱을 사용 하 여 MFA에 등록 해야 합니다. MFA 등록 완료 되 면 관리자에 로그인 할 때마다 MFA를 수행 해야 합니다.

조직에 이러한 계정은 스크립트 또는 코드에서 사용 중인 경우 대체 하 여 고려해 야 [identities 관리](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)합니다.

이 정책을 사용 하도록 설정 및 관리자에 게 보호 합니다.

1. 에 로그인 합니다 **Azure portal** 전역 관리자, 보안 관리자 또는 조건부 액세스 관리자입니다.
2. 이동할 **Azure Active Directory** > **조건부 액세스**합니다.
3. 정책 목록에서 선택 **기준 정책: 관리자에 대 한 MFA를 요구할**합니다.
4. 설정할 **정책을 사용 하도록 설정** 하 **즉시 정책을 사용 하 여**입니다.
5. 클릭 **저장할**합니다.

    ![관리자에 대해 MFA 요구](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> 이 정책은 사용 하기 전에 사용자가 레거시 인증 프로토콜을 사용 하지 않는 있는지 확인 합니다. 문서를 참조 [방법: Azure Active directory 조건부 액세스를 사용 하 여 레거시 인증 블록](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) 자세한 내용은 합니다.

> [!IMPORTANT]
> 위임 된 관리자 권한을 사용 하 여 Exchange Online PowerShell에 연결 하는 능력에 영향을 주는 알려진된 문제는 있습니다. 참조를 [Exchange Online PowerShell](#exchange-online-powershell) 알려진 경우에이 정책을 사용 하도록 설정 하기 전에 문제를이 PowerShell 모듈을 사용 하 여 합니다.

#### <a name="end-user-protection"></a>최종 사용자 보호

최종 사용자 보호 기준 정책을 디렉터리의 모든 사용자를 보호합니다. 이 정책을 사용 하면 모든 사용자가 14 일 이내에 Azure MFA에 등록 해야 합니다. 등록 되 면 위험한 로그인 시도 하는 동안에 사용자 MFA에 대 한 메시지가 표시 됩니다. 손상 된 사용자 계정 암호 다시 설정 하 고 사건의 위험이 될 때까지 차단 됩니다.

정책 **기준 정책: 최종 사용자 보호** 미리 구성 되어 및 Azure portal에서 조건부 액세스 블레이드로 이동 하면 위쪽에 표시 됩니다.

이 정책을 사용 하도록 설정 및 사용자를 보호 합니다.

1. 에 로그인 합니다 **Azure portal** 전역 관리자, 보안 관리자 또는 조건부 액세스 관리자입니다.
2. 이동할 **Azure Active Directory** > **조건부 액세스**합니다.
3. 정책 목록에서 선택 **기준 정책: 최종 사용자 보호 (미리 보기)** 합니다.
4. 설정할 **정책을 사용 하도록 설정** 하 **즉시 정책을 사용 하 여**입니다.
5. 클릭 **저장할**합니다.

    ![최종 사용자 보호](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> 이 정책은 사용 하기 전에 사용자가 레거시 인증 프로토콜을 사용 하지 않는 있는지 확인 합니다. 문서를 참조 [방법: Azure Active directory 조건부 액세스를 사용 하 여 레거시 인증 블록](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) 자세한 내용은 합니다.

> [!IMPORTANT]
> 위임 된 관리자 권한을 사용 하 여 Exchange Online PowerShell에 연결 하는 능력에 영향을 주는 알려진된 문제에 있습니다. 참조를 [Exchange Online PowerShell](#exchange-online-powershell) 알려진 경우에이 정책을 사용 하도록 설정 하기 전에 문제를이 PowerShell 모듈을 사용 하 여 합니다.

## <a name="common-issues"></a>일반적인 문제

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

기본 정책은 사용 하도록 설정한 후 볼 수 있습니다 자동화 및 통합에는 발생 하는 다음과 같은 예외

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

이 예외에 대 한 이유는 사용자 자격 증명을 사용 하 여 인증 하 고 MFA가 이제 필요 합니다. 이 예외를 해결 하기 위해 인증에 대 한 액세스 토큰을 사용 해야 합니다. 참조 된 [응용 프로그램 모델 보안 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 자세한 내용은 합니다.

>[!IMPORTANT]
>최신 Api 및 PowerShell 모듈에는 인증에 대 한 액세스 토큰을 사용할 수 있도록을 지원 합니다. 그러나 몇 가지는 현재이 기능을 지원 하지 않습니다. 활용 하려는 API 또는 PowerShell 모듈 경우 인증에 대 한 액세스 토큰 사용을 지원 결정을 할 경우 다음에 메시지 게시 합니다 [파트너 센터 보안 지침 그룹](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 커뮤니티입니다.

#### <a name="aadsts700082"></a>AADSTS700082

다음과 같은 예외가 초기 새로 고침 토큰을 생성 한 후 90 일 동안 받게 가능성이 매우 응용 프로그램 모델 보안 프레임 워크를 구현한 경우

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Azure Active Directory와 관련 하 여 새로 고침에 대 한 최대 수명 토큰 90 일입니다. 이 오류를 해결 하기 위해 생성 하 고 안전 하 게 새로운 새로 고침 토큰을 저장 해야 합니다. Azure Active Directory에 액세스 토큰에 대 한 각 요청을 사용 하 여 새로운 새로 고침 토큰이 반환 되기 때문에 새로 고침 토큰을 프로그래밍 방식으로 업데이트할 수 있습니다 note 합니다. 만료 되기 전까지 안전 하 게 저장 된 새로 고침 토큰을 업데이트 하려면 적절 한 논리를 구현할 수 있습니다.

참조 [Azure Active Directory에서 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 자세한 내용은 합니다.

### <a name="recovering-compromised-accounts"></a>손상 된 계정 복구

고객을 보호 하기 위해, Microsoft의 유출 된 자격 증명 서비스는 공개적으로 사용할 수 있는 사용자 이름/암호 쌍을 찾습니다. 일치 하는 경우 사용자에 해당 계정을 즉시 보호 있도록 도와 드립니다. 유출 된 자격 증명을 가진 것으로 식별 된 사용자는 손상 확인 됩니다. 이러한 사용자가 암호 재설정 될 때까지 로그인에서 차단 됩니다.

Azure AD Premium 라이선스가 할당 된 사용자가 디렉터리에서 기능을 사용 하는 경우 셀프 서비스 암호 재설정 (SSPR)을 통한 액세스를 복원할 수 있습니다. 차단 되는 premium 라이선스가 없는 사용자가 암호 직접 재설정을 수행 하 고 플래그가 지정 된 사용자 위험 이벤트를 해제 하려면 관리자에 문의 해야 합니다.

#### <a name="steps-to-unblock-a-user"></a>사용자 차단 해제 하는 단계

사용자의 로그인 로그를 검사 하 여 사용자 정책에 의해 차단 되었다는 것을 확인 합니다.

1. 관리자로 로그인 해야 합니다 **Azure portal** 이동할 **Azure Active Directory** > **사용자** > 사용자의 이름을 클릭 하 고 이동 로그인 합니다.
2. 차단 된 사용자에 암호 재설정을 시작 하려면 관리자로 이동 해야 **Azure Active Directory** > **위험 플래그가 지정 된 사용자**
3. 사용자의 최근 로그인 활동에 대 한 정보를 보려는 계정이 차단 되는 사용자를 클릭 합니다.
4. 다음 로그인 시 변경 해야 하는 임시 암호를 할당 하는 데 암호 재설정을 클릭 합니다.
5. 사용자의 위험 점수를 다시 설정 하려면 모든 이벤트를 해제 하는 클릭 합니다.

사용자 수 이제 암호를 재설정 하 고 응용 프로그램에 액세스 합니다.

## <a name="known-issues"></a>알려진 문제

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

MFA가 설정 된 경우 파트너가 고객에 대 한 작업을 수행 하려면 Exchange Online PowerShell을 사용 하 여 해당 위임 된 관리자 권한을 사용할 수 없습니다. 참조 [multi-factor authentication 인증을 사용 하 여 Exchange Online PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) 이 제한에 대 한 자세한 내용은 합니다.

## <a name="resources-and-support"></a>리소스 및 지원

통해 합니다 [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 는 추가 리소스를 확인할를 기술 근무 시간 같은 예정 된 이벤트에 알아봅니다. 참조 된 [질문과 대답](http://assetsprod.microsoft.com/security-requirements-faq.pdf) 요구 사항에 대 한 자세한 문서.

### <a name="developers"></a>개발자

- [보안 응용 프로그램 모델을 사용 하도록 설정](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [파트너 센터.NET 샘플](https://github.com/microsoft/partner-center-dotnet-samples)
- [파트너 센터 Java 샘플](https://github.com/microsoft/partner-center-java-samples)
- [응용 프로그램 보안 모델을 구현 하는 파트너 센터 PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
