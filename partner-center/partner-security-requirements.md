---
title: 보안 요구 사항을 파트너 | 파트너 센터
ms.topic: article
ms.date: 06/25/2019
description: 회사의 고문 및 클라우드 솔루션 공급자 프로그램에 참여 하는 파트너에 대 한 보안 요구 사항에 알아봅니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램을 컨트롤 패널 공급 업체, CSP, CPV, multi-factor authentication에 MFA 보안 응용 프로그램 모델, 안전한 앱 모델, 보안
ms.localizationpriority: medium
ms.openlocfilehash: de1452ce14c8343e2e05dcc65a7a6c05259576c5
ms.sourcegitcommit: ca7f000a58575fa9a089693256c095120dde3c5d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/24/2019
ms.locfileid: "67347002"
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
> 소 버린 클라우드 (21Vianet US Government 및 Germany)를 통해 구속력 있는 모든 파트너 역할을 즉시 이러한 새 보안 요구 사항을 채택 하는 것이 좋습니다. 그러나 이러한 파트너 년 7 월 1 일부 터 유효 새 보안 요구 사항에 맞게 않아도 됩니다. Microsoft는 향후 소 버린 클라우드에 대 한 이러한 보안 요구 사항 적용에 대 한 추가 세부 정보를 제공 합니다.

## <a name="overview-of-the-requirements"></a>요구 사항의 개요

클라우드 솔루션 공급자 프로그램, 컨트롤 패널 공급 업체 및 관리자 파트너에 있는 모든 파트너가 참여 하는 각 사용자가 파트너 테 넌 트에 대 한 Multi-factor Authentication (MFA)을 적용 해야 합니다. 두 개를 사용 하 여 이렇게 [Azure Active Directory 기준 정책을](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)합니다. 기본 정책은 조직에서는 여러 일반적인 공격 으로부터 보호 하는 미리 정의 된 정책 집합. 이러한 일반적인 공격 암호 스프레이, 재생 및 피싱에 포함할 수 있습니다. 기본 정책은 Azure Active Directory의 모든 버전에서 사용할 수 있습니다. Microsoft 기본 보호 정책은 이러한에서 제공 하 모든 사용자에 게 id를 기반으로 공격 지난 몇 년간 점점 증가 하 고 되었기 때문입니다.

두 기준 정책은 활성화 해야 하는 아래 표에 설명 되어 있습니다.

|**정책**| |
|-----|-----|
|**관리자에 대해 MFA 요구**|관리자 정책에 대 한 필요한 MFA를 사용 하도록 설정한 관리자 역할의 사용자를 Authenticator 앱을 사용 하 여 MFA에 등록 해야 합니다. MFA 등록이 완료 되 면 관리자가 MFA를 수행할 때마다 로그인 해야 합니다.|
|**최종 사용자 보호**|최종 사용자 보호는 디렉터리의 모든 사용자를 보호 하는 위험 기반 MFA 기본 정책입니다. 이 정책을 사용 하면 Authenticator 앱을 사용 하 여 MFA에 등록 하는 모든 사용자가 필요 합니다. 사용자는 차단 됩니다 MFA에 등록 될 때까지 로그인에서 14 일간 MFA 등록 프롬프트를 무시할 수 있습니다. MFA에 등록 되 면 위험한 로그인 시도 하는 동안에 사용자 MFA에 대 한 메시지가 표시 됩니다. 손상 된 사용자 계정 암호 다시 설정 되 고 위험 이벤트 해제 된 될 때까지 차단 됩니다.|

이러한 정책을 사용할 경우 각 사용자를 추가 비용 없이 Azure MFA를 사용할 수 있게 됩니다. 타사 솔루션을 사용 하는 경우 Microsoft 상용 클라우드 서비스에 액세스 하는 경우 각 사용자에 대 한 MFA를 적용할 필요가 됩니다.

> [!IMPORTANT]
> 파트너 디렉터리에 모든 사용자에 대 한 MFA를 적용 하므로 모든 자동화 및 사용자 자격 증명을 활용 하는 통합에 영향을 미칠이 됩니다 수 있습니다. 하는 방법을 수정 해야 합니다.이 영향을 해결 하 여 자동화 및 통합 Microsoft 상용 클라우드 서비스에 연결 합니다. 구현 하는 것이 좋습니다. 경우에 연결 하는 서비스는 토큰 기반된 인증을 지원 합니다 [응용 프로그램 모델 보안 프레임 워크](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)합니다.

## <a name="what-actions-do-i-need-to-take"></a>작업을 수행 하나요? 

파트너의 각 사용자가 보호 되도록 해야 하는 사용 하도록 설정 합니다 [관리자에 대 한 MFA를 요구](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 및 [최종 사용자 보호](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 정책을 합니다. 가 이러한 정책은 사용 하도록 설정 하기 전에 수행할 작업 및 어떤 영향을 미치는지 모든 자동화 및 통합 사용자에 게 이해 해야 합니다.

### <a name="considerations"></a>고려 사항

파트너 디렉터리에 모든 사용자에 게 보안 요구 사항을 적용 하기 때문에 원활한 배포에 대 한 몇 가지 고려 사항이 필요 합니다. 이 고려할 사항 없거나 응용 프로그램 및 최신 인증을 지원 하지 않는 조직에서 사용 하는 클라이언트와 함께 MFA를 수행 하지 않아야 하는 Azure Active Directory에서 사용자를 식별 합니다.

#### <a name="legacy-protocols"></a>레거시 프로토콜

레거시 인증 프로토콜 (예: IMAP, SMTP, POP3, 등)는 인증 요청을 메일 클라이언트에서 사용 됩니다. 이러한 프로토콜에서 MFA를 지원 하지 않습니다. 대부분의 Microsoft에서 표시 되는 계정 손상은 MFA를 바이패스 하는 동안 레거시 프로토콜에 대 한 공격을 수행 하는 잘못 된 행위자가 발생 합니다. 파트너 디렉터리의 계정에 로그인 할 때 MFA가 필요한 및 믿지 못할 자에 MFA를 바이패스 하 수 없는 되도록 이러한 보안 요구 사항에는 레거시 프로토콜의 모든 인증 요청을 차단 합니다.

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

기본 정책은 사용 하도록 설정한 후 볼 수 있습니다 자동화 및 통합에는 발생 하는 다음과 유사한 예외가

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

이 예외에 대 한 이유는 사용자 자격 증명을 사용 하 여 인증 하 고 MFA가 이제 필요 합니다. 이 예외를 해결 하기 위해 인증에 대 한 액세스 토큰을 사용 해야 합니다. 참조 된 [응용 프로그램 모델 보안 가이드](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) 자세한 내용은 합니다.

>[!IMPORTANT]
>최신 Api 및 PowerShell 모듈에는 인증에 대 한 액세스 토큰을 사용할 수 있도록을 지원 합니다. 그러나 몇 가지는 현재이 기능을 지원 하지 않습니다. 활용 하려는 API 또는 PowerShell 모듈 경우 인증에 대 한 액세스 토큰 사용을 지원 결정을 할 경우 다음에 메시지 게시 합니다 [파트너 센터 보안 지침 그룹](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 커뮤니티입니다.

#### <a name="aadsts700082"></a>AADSTS700082

다음과 같은 예외가 초기 새로 고침 토큰을 생성 한 후 90 일 동안 받게 가능성이 매우 응용 프로그램 모델 보안 프레임 워크를 구현한 경우

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Azure Active Directory와 관련 하 여 새로 고침에 대 한 최대 수명 토큰 90 일입니다. 이 오류를 해결 하기 위해 생성 하 고 안전 하 게 새로운 새로 고침 토큰을 저장 해야 합니다. Azure Active Directory에 액세스 토큰에 대 한 각 요청을 사용 하 여 새로운 새로 고침 토큰이 반환 되기 때문에 새로 고침 토큰을 프로그래밍 방식으로 업데이트할 수 있습니다 note 합니다. 만료 되기 전까지 안전 하 게 저장 된 새로 고침 토큰을 업데이트 하려면 적절 한 논리를 구현할 수 있습니다.

참조 [Azure Active Directory에서 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 자세한 내용은 합니다.

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
