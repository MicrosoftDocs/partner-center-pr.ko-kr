---
title: 파트너 보안 요구 사항 | 파트너 센터
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 클라우드 솔루션 공급자 프로그램에 참여하는 관리자 및 파트너에 대한 보안 요구 사항에 대해 알아봅니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급업체, CPV, 다단계 인증, MFA, 보안 애플리케이션 모델, 보안 앱 모델, 보안
ms.localizationpriority: high
ms.openlocfilehash: b481bd3e8729c63425c45e1f9767722130dc0833
ms.sourcegitcommit: bf10a7123490ab08c6c3a58cec7045c5d38d16cc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/12/2019
ms.locfileid: "73964209"
---
# <a name="partner-security-requirements"></a>파트너 보안 요구 사항

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 제어판 공급업체
- 모든 관리자

개인 정보 보호 및 보안 강화는 최우선 순위입니다. 최선의 방어는 예방이며, 가장 약한 링크를 강화해야 한다는 것을 알고 있습니다. 따라서 에코시스템의 모든 사람이 조치를 취하고, 적절한 보안 보호가 마련되어야 합니다. Microsoft에서는 파트너와 고객을 보호하기 위해 클라우드 솔루션 공급자 프로그램에 참여하는 관리자, 제어판 공급업체 및 파트너에 대한 일련의 필수 보안 요구 사항을 도입하고 있습니다.

## <a name="overview"></a>개요

파트너는 파트너 테넌트의 모든 사용자에게 다단계 인증을 적용해야 합니다. 파트너 보안 요구 사항과 관련된 사용 약관은 Microsoft 파트너 계약에 추가되었습니다. 관리자와 관련이 있으므로 동일한 계약 요구 사항이 적용됩니다.

이러한 요구 사항이 적용되면 필수 보안 요구 사항을 구현하지 않는 파트너는 클라우드 솔루션 공급자 프로그램에서 거래하거나 위임된 관리자 권한을 이용하여 고객 테넌트를 관리할 수 없게 됩니다. 또한 보안 요구 사항을 구현하지 않는 파트너는 프로그램 참여가 어려울 수 있습니다.  

사용자와 사용자의 고객을 보호하기 위해 파트너에게 즉시 다음과 같은 조치를 취하도록 하고 있습니다.  

1. **파트너 테넌트의 모든 사용자에 대해 MFA(Multi-Factor Authentication)를 사용**합니다. 파트너 테넌트의 모든 사용자 계정은 Microsoft 상용 클라우드 서비스에 로그인하거나 파트너 센터 또는 API를 통해 클라우드 솔루션 공급자에서 거래할 때 MFA(다단계 인증)를 거쳐야 합니다. 

2. **보안 애플리케이션 모델 프레임워크를 채택**합니다. 보안 애플리케이션 모델 프레임워크를 채택합니다. 파트너 센터 API와 통합된 모든 파트너는 모든 앱 + 사용자 인증 모델 애플리케이션에 대해 보안 애플리케이션 모델 프레임워크를 채택해야 합니다.

    > [!IMPORTANT]
    > 파트너는 MFA 사용 시 중단되지 않도록 Azure Resource Manager, Microsoft Graph와 같은 Microsoft API와 통합하거나 사용자 자격 증명을 사용하여 PowerShell과 같은 자동화를 활용하기 위해 보안 애플리케이션 모델을 구현하는 것이 좋습니다.

MFA(Multi-Factor Authentication)를 사용하고 보안 애플리케이션 모델 프레임워크를 채택하면 도난 또는 기타 사기 사건 확인 등 잠재적인 보안 위험으로부터 고객의 데이터를 보호하고 인프라를 보호할 수 있습니다.  

## <a name="actions-that-you-need-to-take"></a>수행해야 하는 작업

파트너 보안 요구 사항을 준수하려면 파트너 테넌트의 각 사용자 계정에 다단계 인증을 적용해야 합니다. 이 작업은 다음 방법 중 하나를 통해 수행할 수 있습니다.

- [Azure AD 보안 기본값](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 구현하는지 확인

- 각 사용자 계정에 대해 Azure Active Directory Premium을 구입합니다. 자세한 내용은 [클라우드 기반 Azure Multi-Factor Authentication 배포 계획](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)을 참조하세요.

- 타사 솔루션을 사용하여 파트너 테넌트의 각 사용자 계정에 다단계 인증 적용 솔루션이 예상 정보를 제공하도록 보장하려면 [보안 요구 사항이 적용되는 방식](#how-the-requirements-will-be-enforced)을 참조하세요.

> [!NOTE]
> 소버린 클라우드(21Vianet, 미국 정부 및 독일)에 대해 계약 상 다단계 인증이 필요하지 않더라도 이러한 보안 요구 사항을 채택하는 것이 좋습니다.

## <a name="security-defaults"></a>보안 기본값

- 보안 기본값은 기준 정책을 대체합니다. 

- 기준 정책은 향후 몇 달 동안 유지될 것이며 2020년 2월말 중단될 예정입니다.

- 기준 정책을 이미 채택한 파트너는 보안 기본값으로 전환하기 위한 조치를 취해야 합니다.

- 보안 기본값을 사용하면 모든 정책이 한 번에 활성화됩니다. 

- 자세한 내용은 [조직에 Multi-Factor Authentication 사용](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-get-started) 및 [Azure Active Directory 보안 기본값](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 참조하세요.

> [!NOTE]
> Azure AD 보안 기본값은 기본 보호 정책의 진화를 단순화한 것입니다. 기준 보호 정책을 이미 사용한 경우 보안 기본값을 사용하는 것이 좋습니다.

기준 정책에서 보안 기본값으로 전환하려는 경우 [보안 기본값이란 무엇인가요?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)를 참조하세요.

### <a name="consideration"></a>고려 사항

이러한 요구 사항은 파트너 테넌트의 모든 사용자 계정에 적용되므로, Azure Active Directory에서 다단계 인증을 수행할 수 없는 사용자 계정의 확인뿐만 아니라 조직이 최신 인증을 지원하지 않는 애플리케이션 및 디바이스를 사용하는 경우 등 원활한 배포를 위해 몇 가지 사항을 고려해야 합니다.

작업을 수행하기 전에 다음을 확인하는 것이 좋습니다. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>최신 인증 사용을 지원하지 않는 애플리케이션 또는 디바이스가 있나요?

다단계 인증 레거시 인증을 적용할 때 IMAP, POP3, SMTP 등의 프로토콜을 사용하면 차단됩니다. 이러한 프로토콜은 다단계 인증을 지원하지 않기 때문입니다. 이러한 제한 사항을 해결하려면 [앱 암호](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)라고 하는 기능을 사용하여 애플리케이션 또는 디바이스에서 계속 인증합니다. 앱 암호를 해당 환경에서 사용할 수 있는지 확인하려면 [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)에 설명된 앱 암호 사용에 대한 고려 사항을 검토해야 합니다.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>파트너 테넌트와 연결된 라이선스에서 제공하는 Office 365를 사용하는 사용자가 있나요?

솔루션을 구현하기 전에 파트너 테넌트의 사용자가 어떤 Microsoft Office 버전을 사용하는지 확인하는 것이 좋습니다. 작업을 수행하기 전에 [Office 365 배포의 다단계 인증 계획](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)을 살펴보세요. 사용자가 Outlook과 같은 애플리케이션의 연결 문제를 경험하게 될 가능성이 있습니다. 다단계 인증을 적용하기 전에 Outlook 2013 SP1 이상을 사용 중이고, 조직에서 최신 인증을 사용하는지 확인해야 합니다. 자세한 내용은 [Exchange Online에서 최신 인증 사용](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)을 참조하세요.

Microsoft Office 2013이 설치된 Windows를 실행하는 모든 디바이스에서 최신 인증을 사용하도록 설정하려면 레지스트리 키를 두 개 만들어야 합니다. [Windows 디바이스에서 Office 2013에 최신 인증 사용](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)을 참조하세요.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>사용자가 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 정책이 있나요?

직원이 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 회사 정책은 구현하는 다단계 인증 솔루션에 영향을 주므로 이러한 정책을 식별하는 것이 중요합니다. 확인에 인증 앱만 사용할 수 있는 [Azure AD 보안 기본값](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 구현하여 제공되는 솔루션 등의 여러 솔루션이 있습니다. 조직에 모바일 디바이스 사용을 금지하는 정책이 있는 경우 다음 옵션 중 하나를 고려해야 합니다.

- 보안 시스템에서 실행할 수 있는 시간 기반 TOTP(시간 제약이 있는 일회성 암호) 애플리케이션 배포

- 파트너 테넌트의 각 사용자 계정에 다단계 인증을 적용하는 가장 적절한 확인 옵션을 제공하는 타사 솔루션 구현

- 관련 사용자를 위해 [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) 라이선스 구매

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>인증에 사용자 자격 증명을 활용하는 자동화 또는 통합이 있나요?

서비스 계정을 비롯한 각 사용자에게 MFA를 적용하는 것이 요구 사항이므로 파트너 디렉터리에서 인증에 사용자 자격 증명을 활용하는 모든 자동화 또는 통합이 영향을 받습니다. 따라서 이러한 상황에서 사용되는 계정을 식별하는 것이 중요합니다. 다음은 고려해야 할 애플리케이션 또는 서비스 예의 목록입니다.

- 고객을 대신하여 리소스를 프로비저닝하는 데 사용되는 제어판 

- 청구 및 고객 지원에 사용되는 모든 플랫폼(CSP 프로그램 관련)과의 통합

- Az, AzureRM, Azure AD, MS Online 등의 모듈을 활용하는 PowerShell 스크립트

위의 목록은 포괄적이지 않습니다. 따라서 사용 중인 환경에서 인증에 사용자 자격 증명을 활용하는 애플리케이션 또는 서비스에 대한 완전한 평가를 수행하는 것이 중요합니다. 다단계 인증에 대한 요구 사항에 대처하려면 [보안 애플리케이션 모델 프레임워크](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)의 지침을 구현해야 합니다(가능한 경우).

## <a name="accessing-your-environment"></a>환경 액세스

다단계 인증을 수행하지 않고 인증하는 대상과 주체를 더 잘 이해하려면 로그인 활동을 검토하는 것이 좋습니다. Azure Active Directory Premium을 통해 로그인 보고서를 활용할 수 있습니다. 자세한 내용은 [Azure Active Directory 포털의 로그인 활동 보고서](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)를 참조하세요. Azure Active Directory Premium이 없거나 PowerShell을 통해 이 보고서를 가져오는 방법을 찾고 있으면 [파트너 센터 PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) 모듈에서 [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet을 활용해야 합니다.

## <a name="how-the-requirements-will-be-enforced"></a>요구 사항이 적용되는 방식

파트너 보안 요구 사항은 Azure Active Directory를 통해 적용된 후 파트너 센터에서 적용되며, MFA 클레임이 있는지 확인하여 다단계 인증 확인이 발생했는지 파악하는 방식으로 적용됩니다. 2019년 11월 18일부터 Microsoft는 파트너 테넌트에 대한 추가 보안 보호 기능(이전의 "기술 적용")을 활성화합니다. 

활성화하면, 파트너 테넌트의 사용자에게 AOBO(관리자 위임) 작업을 수행할 때 MFA(다단계 인증) 확인을 완료하라는 메시지가 표시됩니다. Microsoft는 추가 시나리오 및 사용자 역할에 대한 보안 보호 범위를 계속 확장하여 파트너에게 사전에 통지합니다. 자세한 내용은 자주 업데이트 되는 이 문서를 참조하세요. 요구 사항을 충족하지 못한 파트너는 비즈니스가 중단되지 않도록 가능한 한 빨리 이러한 조치를 구현해야 합니다. 

Azure Multi-Factor Authentication 또는 Azure AD 보안 기본값을 사용하는 경우 수행해야 하는 추가 작업이 없습니다.

타사 다단계 인증 솔루션을 사용하는 경우 MFA 클레임이 발급되지 않을 가능성이 있습니다. 이 클레임이 없는 경우 Azure Active Directory는 다단계 인증에서 인증 요청을 요구했는지 확인할 수 없습니다. 솔루션에서 예상 클레임을 발급하는지 확인하는 방법에 대한 자세한 내용은 [파트너 보안 요구 사항 테스트](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)를 참조하세요. 

> [!IMPORTANT]
> 타사 솔루션이 예상 클레임을 발급하지 않을 경우 솔루션을 개발한 공급업체와 협력하여 어떤 조치가 필요한지 확인해야 합니다.

## <a name="resources-and-support"></a>리소스 및 지원

다음은 지원 및 샘플 코드를 찾을 수 있는 리소스입니다.

- [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - 예정된 이벤트에 대해 알아보고 궁금한 점을 물어볼 수 있는 온라인 커뮤니티입니다.
- [파트너 센터 .NET 샘플](https://github.com/microsoft/partner-center-dotnet-samples) - 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, .NET을 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 Java 샘플](https://github.com/microsoft/partner-center-java-samples) - 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, Java를 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 PowerShell - Multi-Factor Authentication](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) - PowerShell을 사용하여 보안 애플리케이션 모델 프레임워크를 구현하는 방법에 대해 자세히 설명하는 문서입니다.
