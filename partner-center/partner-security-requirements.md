---
title: 파트너 보안 요구 사항 | 파트너 센터
ms.topic: article
ms.date: 10/11/2019
description: 클라우드 솔루션 공급자 프로그램에 참여하는 관리자 및 파트너에 대한 보안 요구 사항에 대해 알아봅니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급업체, CPV, 다단계 인증, MFA, 보안 애플리케이션 모델, 보안 앱 모델, 보안
ms.localizationpriority: high
ms.openlocfilehash: b09588387d3b4f0f3f726a700245999c89755199
ms.sourcegitcommit: 9dd6f1ee0ebc132442126340c9df8cf7e3e1d3ad
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/16/2019
ms.locfileid: "72425207"
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

## <a name="overview"></a>개요

2019년 8월 1일부터 모든 파트너는 파트너 테넌트의 모든 사용자에게 다단계 인증을 적용해야 합니다. 파트너 보안 요구 사항과 관련된 용어가 [클라우드 솔루션 공급자 프로그램 가이드](https://go.microsoft.com/fwlink/p/?LinkId=617100)에 추가되었습니다. 관리자와 관련이 있으므로 동일한 계약 요구 사항이 적용됩니다.

> [!NOTE]
> 소버린 클라우드(21Vianet, 미국 정부 및 독일)를 통해 거래하는 모든 파트너는 이러한 보안 요구 사항을 즉시 적용하고 채택할 것을 적극 권장합니다. 그러나 이러한 파트너는 2019년 8월 1일부터 적용되는 보안 요구 사항을 충족할 필요가 없습니다. Microsoft에서는 나중에 소버린 클라우드에 대한 이러한 보안 요구 사항의 적용과 관련된 추가 세부 정보를 제공할 예정입니다.

이러한 요구 사항이 적용되면 필수 보안 요구 사항을 구현하지 않는 파트너가 클라우드 솔루션 공급자 프로그램에서 거래하거나 위임 관리자 권한을 활용하는 고객 테넌트를 관리할 수 없게 됩니다.

## <a name="actions-that-you-need-to-take"></a>수행해야 하는 작업

파트너 보안 요구 사항을 준수하려면 파트너 테넌트의 각 사용자 계정에 다단계 인증을 적용해야 합니다. 이 작업은 다음 방법 중 하나를 통해 수행할 수 있습니다.

- Azure Active Directory에서 추가 비용 없이 [관리자용 MFA 필요](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 및 [최종 사용자 보호](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) 기준 보호 정책 기능을 구현합니다.
- 각 사용자 계정에 대해 Azure Active Directory Premium을 구입합니다. 자세한 내용은 [클라우드 기반 Azure Multi-Factor Authentication 배포 계획](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)을 참조하세요.
- 타사 솔루션을 사용하여 파트너 테넌트의 각 사용자 계정에 다단계 인증 적용 솔루션이 예상 정보를 제공하도록 보장하려면 [보안 요구 사항이 적용되는 방식](#how-the-requirements-will-be-enforced)을 참조하세요.

### <a name="consideration"></a>고려 사항

이러한 요구 사항은 파트너 테넌트의 모든 사용자 계정에 적용되므로 원활한 배포를 위해 고려해야 할 몇 가지 사항이 있습니다. 이러한 고려 사항에는 다단계 인증을 수행할 수 없는 Azure Active Directory의 사용자 계정, 그리고 조직에서 사용하는 최신 인증을 지원하지 않는 애플리케이션 및 디바이스를 식별하는 작업이 포함됩니다.

작업을 수행하기 전에 다음을 확인하는 것이 좋습니다.

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>최신 인증 사용을 지원하지 않는 애플리케이션 또는 디바이스가 있나요?

다단계 인증 레거시 인증을 적용할 때 IMAP, POP3, SMTP 등의 프로토콜을 사용하면 차단됩니다. 이러한 프로토콜은 다단계 인증을 지원하지 않기 때문입니다. 이러한 제한 사항을 해결하려면 [앱 암호](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)라고 하는 기능을 사용하여 애플리케이션 또는 디바이스에서 계속 인증하도록 할 수 있습니다. 앱 암호를 해당 환경에서 사용할 수 있는지 확인하려면 [여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)에 설명된 앱 암호 사용에 대한 고려 사항을 검토해야 합니다.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>파트너 테넌트와 연결된 라이선스에서 제공하는 Office 365를 사용하는 사용자가 있나요?

솔루션을 구현하기 전에 파트너 테넌트의 사용자가 어떤 Microsoft Office 버전을 사용하는지 확인하는 것이 좋습니다. 작업을 수행하기 전에 [Office 365 배포의 다단계 인증 계획](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)을 살펴보세요. 사용자가 Outlook과 같은 애플리케이션의 연결 문제를 경험하게 될 가능성이 있습니다. 다단계 인증을 적용하기 전에 Outlook 2013 SP1 이상을 사용 중이고, 조직에서 최신 인증을 사용하는지 확인해야 합니다. 자세한 내용은 [Exchange Online에서 최신 인증 사용](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)을 참조하세요.

Microsoft Office 2013이 설치된 Windows를 실행하는 모든 디바이스에서 최신 인증을 사용하도록 설정하려면 레지스트리 키를 두 개 만들어야 합니다. [Windows 디바이스에서 Office 2013에 최신 인증 사용](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)을 참조하세요.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>사용자가 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 정책이 있나요?

직원이 업무 시간에 모바일 디바이스를 사용하지 못하게 하는 회사 정책은 구현하는 다단계 인증 솔루션에 영향을 주므로 이러한 정책을 식별하는 것이 중요합니다. 확인 작업에 인증 앱만 사용할 수 있는 [기준 보호 정책](/azure/active-directory/conditional-access/concept-baseline-protection)을 구현하여 제공되는 솔루션을 포함하여 여러 솔루션이 있습니다. 조직에 모바일 디바이스 사용을 금지하는 정책이 있는 경우 다음 옵션 중 하나를 고려해야 합니다.

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

다단계 인증을 요구받지 않고 인증하는 주체를 정확하게 파악하려면 Azure Active Directory 감사 로그를 쿼리하는 것이 좋습니다. 이러한 작업은 [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) 모듈과 아래의 스크립트를 사용하여 수행할 수 있습니다. 전날에 다단계 인증을 요구받지 않고 발생한 인증 시도에 대한 인사이트를 제공하는 보고서가 생성됩니다.

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

$report | Where-Object {$_.mfaRequired -eq $false -and $_.loginSucceeded -eq $true} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

위의 스크립트를 실행한 후에는 report.csv 파일에서 세부 정보를 볼 수 있습니다. 여기에는 사용자에게 MFA 챌린지에 대한 메시지가 표시되지 않았던 전날에 발생한 인증 시도 목록이 포함됩니다. 각 항목을 검토하여 올바른 동작인지 확인하고 필요한 경우 작동하는지 확인해야 합니다.

![평가 도구](images/security/assessment-report.png)

## <a name="how-the-requirements-will-be-enforced"></a>요구 사항이 적용되는 방식

파트너 보안 요구 사항은 Azure Active Directory를 통해 적용된 후 파트너 센터에서 적용되며, MFA 클레임이 있는지 확인하여 다단계 인증 확인이 발생했는지 파악하는 방식으로 적용됩니다. Azure Multi-Factor Authentication 또는 기준 보호 정책을 사용하는 경우 수행해야 하는 추가 작업이 없습니다.

타사 다단계 인증 솔루션을 사용하는 경우 MFA 클레임이 발급되지 않을 가능성이 있습니다. 이 클레임이 없는 경우 Azure Active Directory는 다단계 인증에서 인증 요청을 요구했는지 확인할 수 없습니다. 솔루션에서 예상 클레임을 발급하는지 확인하는 방법에 대한 자세한 내용은 [파트너 보안 요구 사항 테스트](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)를 참조하세요.

> [!IMPORTANT]
> 타사 솔루션이 예상 클레임을 발급하지 않을 경우 솔루션을 개발한 공급업체와 협력하여 어떤 조치가 필요한지 확인해야 합니다.

## <a name="resources-and-support"></a>리소스 및 지원

다음은 지원 및 샘플 코드를 찾을 수 있는 리소스입니다.

- [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - 예정된 이벤트에 대해 알아보고 궁금한 점을 물어볼 수 있는 온라인 커뮤니티입니다.
- [파트너 센터 .NET 샘플](https://github.com/microsoft/partner-center-dotnet-samples) - 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, .NET을 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 Java 샘플](https://github.com/microsoft/partner-center-java-samples) - 이 GitHub 리포지토리에는 보안 애플리케이션 모델 프레임워크를 구현하는 방법을 보여주며, Java를 사용하여 개발된 샘플이 포함되어 있습니다.
- [파트너 센터 PowerShell - Multi-Factor Authentication](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) - PowerShell을 사용하여 보안 애플리케이션 모델 프레임워크를 구현하는 방법에 대해 자세히 설명하는 문서입니다.
