---
title: 파트너 보안 요구 사항
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: MFA(Multi-factor Authentication)를 활성화하고 보안 애플리케이션 모델 프레임워크를 도입하기 위한 파트너 보안 요구 사항을 소개합니다.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 201ea34d30814974936da032805f1ee7dfa590be
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145850"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>파트너 센터 또는 파트너 센터 API 사용 시 보안 요구 사항

**적절한 역할**: 모든 파트너 센터 사용자

이 문서에서는 관리자, 제어판 공급업체 및 클라우드 솔루션 공급자 프로그램에 참여하는 파트너에 대한 필수 보안 요구 사항과 인증 옵션 및 기타 보안 고려 사항에 대해 설명합니다. 개인 정보 보호 및 보안은 최우선 순위입니다. 최선의 방어는 예방이며, 가장 약한 링크를 강화해야 한다는 것을 알고 있습니다. 따라서 에코시스템의 모든 사람이 조치를 취하고, 적절한 보안 보호가 마련되어야 합니다.

## <a name="mandatory-security-requirements"></a>필수 보안 요구 사항

필수 보안 요구 사항을 구현하지 않는 파트너는 클라우드 솔루션 공급자 프로그램에서 거래하거나 위임된 관리자 권한을 사용하여 고객 테넌트를 관리할 수 없게 됩니다. 또한 보안 요구 사항을 구현하지 않는 파트너는 프로그램 참여가 어려울 수 있습니다. 파트너 보안 요구 사항과 관련된 사용 약관은 Microsoft 파트너 계약에 추가되었습니다. 관리자와 관련이 있으므로 동일한 계약 요구 사항이 적용됩니다.

사용자와 사용자의 고객을 보호하기 위해 파트너에게 즉시 다음과 같은 조치를 취하도록 하고 있습니다.  

1. **파트너 테넌트의 모든 사용자에 대해 MFA(다단계 인증)를 사용합니다**. 파트너 테넌트의 모든 사용자 계정에 MFA를 적용해야 합니다. 사용자는 Microsoft 상용 클라우드 서비스에 로그인하거나 파트너 센터 또는 API를 통해 클라우드 솔루션 공급자 프로그램에서 거래할 때 MFA를 거쳐야 합니다.

2. **보안 애플리케이션 모델 프레임워크를 채택** 합니다. 파트너 센터 API와 통합된 모든 파트너는 모든 앱 및 사용자 인증 모델 애플리케이션에 대해 [보안 애플리케이션 모델 프레임워크](/partner-center/develop/enable-secure-app-model)를 채택해야 합니다.

    > [!IMPORTANT]
    > 파트너는 MFA 사용 시 중단되지 않도록 Azure Resource Manager, Microsoft Graph와 같은 Microsoft API와 통합하거나 사용자 자격 증명을 사용하여 PowerShell과 같은 자동화를 활용하는 경우 보안 애플리케이션 모델을 구현하는 것이 좋습니다.

이러한 보안 요구 사항은 인프라를 보호하고 신원 도용 또는 기타 사기 사건과 같은 잠재적인 보안 위험으로부터 고객의 데이터를 보호하는 데 도움이 됩니다.  

## <a name="implementing-multi-factor-authentication"></a>다단계 인증 구현

파트너 보안 요구 사항을 준수하려면 파트너 테넌트의 각 사용자 계정에 대해 MFA를 구현 및 적용해야 합니다. 다음 방법 중 하나로 이 작업을 수행할 수 있습니다.

- [Azure AD(Azure Active Directory) 보안 기본값](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 구현합니다. [다음 섹션](#security-defaults)에서 자세히 살펴봅니다.

- 각 사용자 계정에 대해 Azure Active Directory Premium을 구매합니다. 자세한 내용은 [Azure AD Multi-Factor Authentication 배포 계획](/azure/active-directory/authentication/howto-mfa-getstarted)을 참조하세요.

- 타사 솔루션을 사용하여 파트너 테넌트의 각 사용자 계정에 MFA를 적용합니다. 솔루션이 예상 정보를 제공하도록 보장하려면 [보안 요구 사항이 적용되는 방식](#how-the-requirements-are-enforced)을 참조하세요.

> [!NOTE]
> 소버린 클라우드(미국 정부 및 독일)에 대해 계약 상 다단계 인증이 필요하지 않더라도 이러한 보안 요구 사항을 채택하는 것이 좋습니다.

### <a name="security-defaults"></a>보안 기본값

파트너가 MFA 요구 사항을 구현하기 위해 선택할 수 있는 옵션 중 하나는 Azure AD에서 보안 기본값을 사용하는 것입니다. 보안 기본값은 추가 비용 없이 기본 보안 수준을 제공합니다. 보안 기본값을 사용하도록 설정하기 전에 Azure AD를 사용하여 조직에 MFA를 사용하도록 설정하는 방법과 아래의 주요 고려 사항을 검토하세요.

- 기준 정책을 이미 채택한 파트너는 보안 기본값으로 전환하기 위한 조치를 취해야 합니다.

- 보안 기본값은 미리 보기 기준 정책의 일반 공급 대체 기능입니다. 파트너가 보안 기본값을 사용하도록 설정한 후에는 더 이상 기준 정책을 사용하도록 설정할 수 없습니다.

- 보안 기본값을 사용하면 모든 정책이 한 번에 활성화됩니다.

- [조건부 액세스](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)를 사용 중인 파트너는 [보안 기본값을 사용할 수 없습니다](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- 지금은 레거시 인증을 차단하지 않습니다. 그러나 신원 도용과 관련된 대부분의 이벤트가 레거시 인증을 사용하는 로그인 시도에서 발생하므로 파트너는 이러한 이전 프로토콜에서 이전하는 것이 좋습니다.

- Azure AD Connect 동기화 계정은 보안 기본값에서 제외됩니다.

자세한 내용은 [조직에 대한 AD Azure Multi-Factor Authentication 개요](/azure/active-directory/authentication/concept-mfa-get-started) 및 [보안 기본값이란?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 참조하세요.

> [!NOTE]
> Azure AD 보안 기본값은 기본 보호 정책의 진화를 단순화한 것입니다. 기본 보호 정책을 이미 사용한 경우 [보안 기본값](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 사용하는 것이 좋습니다.

## <a name="implementation-considerations"></a>구현 고려 사항

이러한 요구 사항은 파트너 테넌트의 모든 사용자 계정에 적용되므로 원활한 배포를 위한 몇 가지 사항을 고려해야 합니다. 예를 들어 MFA를 수행할 수 없는 Azure AD의 사용자 계정과 최신 인증을 지원하지 않는 조직의 애플리케이션 및 디바이스를 확인합니다.

작업을 수행하기 전에 다음과 같은 유효성 검사를 완료하는 것이 좋습니다. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>최신 인증 사용을 지원하지 않는 애플리케이션 또는 디바이스가 있나요?

MFA를 적용하면 IMAP, POP3, SMTP 등의 기존 인증 사용 프로토콜이 MFA를 지원하지 않기 때문에 차단됩니다. 이러한 제한 사항을 해결하려면 애플리케이션 또는 디바이스에서 계속 인증하도록 [앱 암호](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) 기능을 사용합니다. 앱 암호를 사용자의 환경에서 사용할 수 있는지 확인하려면 [앱 암호 사용에 대한 고려 사항](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)을 검토합니다.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>파트너 테넌트와 연결된 라이선스가 있는 Office 365 사용자가 있나요?

솔루션을 구현하기 전에 파트너 테넌트의 사용자가 어떤 Microsoft Office 버전을 사용하는지 확인하는 것이 좋습니다. 사용자가 Outlook과 같은 애플리케이션의 연결 문제를 경험하게 될 가능성이 있습니다. MFA를 적용하기 전에 Outlook 2013 SP1 이상을 사용하고 있고, 조직에서 최신 인증을 사용하는지 확인해야 합니다. 자세한 내용은 [Exchange Online에서 최신 인증 사용](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)을 참조하세요. 

Microsoft Office 2013이 설치된 Windows를 실행하는 모든 디바이스에서 최신 인증을 사용하도록 설정하려면 레지스트리 키를 두 개 만들어야 합니다. [Windows 디바이스에서 Office 2013에 최신 인증 사용](/office365/admin/security-and-compliance/enable-modern-authentication)을 참조하세요.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>사용자가 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 정책이 있나요?

직원이 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 회사 정책은 구현하는 MFA 솔루션에 영향을 주므로 이러한 정책을 식별하는 것이 중요합니다. 확인에 인증 앱만 사용할 수 있는 [Azure AD 보안 기본값](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 구현하여 제공되는 솔루션 등의 여러 솔루션이 있습니다. 조직에 모바일 디바이스 사용을 금지하는 정책이 있는 경우 다음 옵션 중 하나를 고려합니다.

- 보안 시스템에서 실행할 수 있는 시간 기반 TOTP(시간 제약이 있는 일회성 암호) 애플리케이션을 배포합니다.

- 가장 적절한 인증 옵션을 제공하는 파트너 테넌트의 각 사용자 계정에 MFA를 적용하는 타사 솔루션을 구현합니다.

- 관련 사용자를 위해 [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) 라이선스를 구매합니다.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>인증에 사용자 자격 증명을 활용하는 자동화 또는 통합이 있나요?

파트너 디렉터리에서 서비스 계정을 비롯한 각 사용자에 대해 MFA를 적용하기 때문에, 인증을 위해 사용자 자격 증명을 사용하는 모든 자동화 또는 통합에 영향을 미칩니다. 따라서 이러한 상황에서 어떤 계정이 사용되는지 식별하는 것이 중요합니다. 고려할 다음 샘플 애플리케이션 또는 서비스 목록을 참조하세요.

- 고객을 대신하여 리소스를 프로비저닝하는 데 사용되는 제어판

- 청구 및 고객 지원에 사용되는 모든 플랫폼(CSP 프로그램 관련)과의 통합

- Az, AzureRM, Azure AD, MS Online 등의 모듈을 사용하는 PowerShell 스크립트

위의 목록은 포괄적이지 않습니다. 따라서 사용 중인 환경에서 인증에 사용자 자격 증명을 사용하는 애플리케이션 또는 서비스에 대한 완전한 평가를 수행하는 것이 중요합니다. MFA에 대한 요구 사항에 대처하려면 [보안 애플리케이션 모델 프레임워크](/partner-center/develop/enable-secure-app-model)의 지침을 구현해야 합니다(가능한 경우).

## <a name="accessing-your-environment"></a>환경 액세스

MFA를 거치지 않고 인증하는 대상과 주체를 더 잘 이해하려면 로그인 활동을 검토하는 것이 좋습니다. Azure Active Directory Premium을 통해 로그인 보고서를 사용할 수 있습니다. 이 주제에 대한 자세한 내용은 [Azure Active Directory 포털의 로그인 활동 보고서](/azure/active-directory/reports-monitoring/concept-sign-ins)를 참조하세요. Azure Active Directory Premium이 없거나 PowerShell을 통해 이 로그인 활동을 가져오는 방법을 찾고 있다면 [파트너 센터 PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) 모듈에서 [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) cmdlet을 사용해야 합니다.

## <a name="how-the-requirements-are-enforced"></a>요구 사항이 적용되는 방식

파트너 보안 요구 사항은 Azure AD를 통해 적용된 후 파트너 센터에서 적용되며, MFA 클레임이 있는지 확인하여 MFA 확인이 발생했는지 파악하는 방식으로 적용됩니다. 2019년 11월 18일부터 Microsoft는 파트너 테넌트에 대한 추가 보안 보호 기능(이전의 "기술 적용")을 활성화했습니다.

이 기능을 활성화하면, 파트너 테넌트의 사용자에게 AOBO(관리자 위임) 작업을 수행하거나, 파트너 센터 포털에 액세스하거나, 파트너 센터 API를 호출할 때 MFA 확인을 완료하라는 메시지가 표시됩니다. 자세한 내용은 [파트너 테넌트에 대한 MFA(Multi-Factor Authentication) 위임](partner-security-requirements-mandating-mfa.md)을 참조하세요. 

요구 사항을 충족하지 못한 파트너는 비즈니스가 중단되지 않도록 가능한 한 빨리 이러한 조치를 구현해야 합니다. Azure Active Directory Multi-Factor Authentication 또는 Azure AD 보안 기본값을 사용하는 경우 수행해야 하는 추가 작업이 없습니다.

타사 MFA 솔루션을 사용하는 경우 MFA 클레임이 발급되지 않을 가능성이 있습니다. 이 클레임이 없는 경우 Azure AD는 MFA에서 인증 요청을 요구했는지 확인할 수 없습니다. 솔루션에서 예상 클레임을 발급하는지 확인하는 방법에 대한 자세한 내용은 [파트너 보안 요구 사항 테스트](/powershell/partnercenter/test-partner-security-requirements)를 참조하세요. 

> [!IMPORTANT]
> 타사 솔루션이 예상 클레임을 발급하지 않을 경우 솔루션을 개발한 공급업체와 협력하여 어떤 조치가 필요한지 확인해야 합니다.

## <a name="resources-and-samples"></a>리소스 및 샘플

지원 및 샘플 코드에 대해 다음 리소스를 참조하세요.

- [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): 파트너 센터 보안 지침 그룹 커뮤니티는 예정된 이벤트에 대해 알아보고 궁금한 점을 물어볼 수 있는 온라인 커뮤니티입니다.
- [파트너 센터 .NET 샘플](https://github.com/microsoft/partner-center-dotnet-samples): 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, .NET을 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 Java 샘플](https://github.com/microsoft/partner-center-java-samples): 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, Java를 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 PowerShell - Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): 이 Multi-Factor Authentication 문서는 PowerShell을 사용하여 보안 애플리케이션 모델 프레임워크를 구현하는 방법에 대해 자세히 설명합니다.

## <a name="next-steps"></a>다음 단계

- [파트너 테넌트에 대한 MFA(Multi-Factor Authentication) 위임](partner-security-requirements-mandating-mfa.md)