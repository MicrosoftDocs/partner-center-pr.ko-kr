---
title: 파트너 테넌트에 대한 MFA 위임
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 테넌트에 대한 MFA를 위임하여 고객 리소스에 안전하게 액세스하는 방법을 알아봅니다. 샘플 시나리오가 포함되어 있습니다.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 01122e81254a8e63f9bbf8d6bc3d3271accac74a
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680396"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>파트너 테넌트에 대한 MFA(Multi-Factor Authentication) 위임

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 관리자

**영향을 받는 역할**

- 관리 에이전트
- 영업 상담원
- 기술 지원팀 상담원
- 대금 청구 관리자
- 전역 관리자

이 기능은 파트너가 자격 증명을 손상시키지 않도록 고객 리소스에 대한 액세스를 보호하기 위한 것입니다.
파트너는 게스트 사용자를 포함하여 파트너 테넌트의 모든 사용자 계정에 MFA(Multi-Factor Authentication)를 적용해야 하며, 이 기능을 사용하는 경우 이러한 파트너 역할은 다음 영역에 대한 MFA 확인을 완료하도록 위임됩니다.

- [파트너 센터 대시보드](#partner-center-dashboard)
- [파트너 센터 API](#partner-center-api)
- [파트너에게 위임된 관리](#partner-delegated-administration)

더 강력하고 지속적인 보안 및 개인 정보 보호가 최우선 순위이며, 파트너가 고객과 테넌트를 보호할 수 있도록 지속적으로 지원하고 있습니다. CSP(클라우드 솔루션 공급자) 프로그램, CPV(제어판 공급업체) 및 관리자에 참여하는 모든 파트너는 규정을 준수하기 위한 [파트너 보안 요구 사항](partner-security-requirements.md)을 구현해야 합니다.

Microsoft는 파트너가 ID 도용 관련 사고로부터 기업과 고객을 보호할 수 있도록 파트너 테넌트에 대한 추가 보안 보호 기능을 활성화했습니다. 이로써 파트너는 MFA(다단계 인증) 확인을 위임하여 파트너의 테넌트와 고객이 무단 액세스를 방지하도록 할 수 있습니다. 

이 설명서에서는 파트너에게 보안 보호 기능의 활성화와 관련된 자세한 환경과 지침을 제공합니다.

## <a name="partner-center-dashboard"></a>파트너 센터 대시보드

파트너 센터 대시보드의 특정 페이지는 다음을 포함하여 MFA로 보호됩니다.

- **고객** 탭의 모든 페이지(예: https://partner.microsoft.com/commerce/* URL을 통해 액세스할 수 있는 모든 페이지)
- **지원 > 고객 요청** 탭의 모든 페이지(예: https://partner.microsoft.com/dashboard/support/csp/customers/* 에서 액세스한 페이지)
- 청구 페이지

이러한 페이지에 액세스하려고 하지만 이전에 MFA 확인을 완료하지 않은 경우 이 작업을 수행해야 합니다.

> [!NOTE]
> 개요 페이지, 서비스 상태 확인 페이지와 같은 파트너 센터의 다른 페이지는 MFA로 보호되지 않습니다.

다음 사용자 유형은 이러한 MFA로 보호된 페이지에 액세스할 수 있는 권한이 있으므로 이 기능의 영향을 받습니다.


| MFA로 보호되는 페이지       | 관리 담당자      |  영업 담당자     |   기술 지원팀 담당자     | 전역 관리자      |  대금 청구 관리자     | 
|---    |---    |---    |---    |---    |---    |
| 고객 탭의 모든 페이지      |   x    |    x   |  x     |       |       |
| 지원 > 고객 요청 탭의 모든 페이지     | x      |       |    x   |       |       |
| 청구 페이지     |   x    |       |       |    x   |   x    |

## <a name="examples-showing-how-verification-works"></a>확인이 작동하는 방법을 보여주는 예제

확인이 작동하는 방법을 설명하기 위해 다음 두 가지 예제를 고려합니다.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>예제 1: 파트너가 Azure AD MFA를 구현함

1. Jane은 CSP Contoso에서 근무합니다. Contoso에서 Azure AD(Azure Active Directory) MFA를 사용하여 Contoso 파트너 테넌트의 모든 사용자에 대해 MFA를 구현했습니다.

2. Jane이 새 브라우저 세션을 시작하여 파트너 센터 대시보드 개요 페이지(MFA로 보호되지 않음)로 이동합니다. 파트너 센터에서 Jane을 Azure AD로 리디렉션하여 로그인합니다.

3. Contoso의 기존 Azure AD MFA 설정으로 인해 Jane이 MFA 확인을 완료해야 합니다. 로그인 및 MFA 확인이 성공하면 Jane이 파트너 센터 대시보드 개요 페이지로 다시 리디렉션됩니다.

4. Jane이 파트너 센터에서 MFA로 보호되는 페이지 중 하나에 액세스하려고 합니다. Jane이 이전에 로그인하는 동안 이미 MFA 확인을 완료했으므로 Jane은 MFA 확인을 다시 수행하지 않고도 MFA로 보호되는 페이지에 액세스할 수 있습니다.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>예제 2: 파트너가 ID 페더레이션을 사용하여 타사 MFA를 구현함

1. Trent는 CSP Wingtip에서 근무합니다. Wingtip에서 ID 페더레이션을 통해 Azure AD와 통합된 타사 MFA를 사용하여 Wingtip 파트너 테넌트의 모든 사용자에 대해 MFA를 구현했습니다.

2. Trent가 새 브라우저 세션을 시작하여 파트너 센터 대시보드 개요 페이지(MFA로 보호되지 않음)로 이동합니다. 파트너 센터에서 Trent를 Azure AD로 리디렉션하여 로그인합니다.

3. Wingtip에서 ID 페더레이션을 설정했으므로 Azure AD에서 Trent가 페더레이션 ID 공급자로 리디렉션되어 로그인 및 MFA 확인을 완료합니다. 로그인 및 MFA 확인이 완료되면 Trent가 Azure AD로 다시 리디렉션된 다음, 파트너 센터 대시보드 개요 페이지로 리디렉션됩니다.

4. Trent가 파트너 센터에서 MFA로 보호되는 페이지 중 하나에 액세스하려고 합니다. Trent가 이전에 로그인하는 동안 이미 MFA 확인을 완료했으므로 Trent는 MFA 확인을 다시 수행하지 않고도 MFA로 보호되는 페이지에 액세스할 수 있습니다.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>예제 3: 파트너가 MFA를 구현하지 않음

1. John은 CSP Fabrikam에서 근무합니다. Fabrikam에서 Fabrikam 파트너 테넌트의 모든 사용자에 대해 MFA를 구현하지 않았습니다.

2. John이 새 브라우저 세션을 시작하여 파트너 센터 대시보드 개요 페이지(MFA로 보호되지 않음)로 이동합니다. 파트너 센터에서 John을 Azure AD로 리디렉션하여 로그인합니다.

3. Fabrikam에서 MFA를 구현하지 않았으므로 John이 MFA 확인을 완료할 필요가 없습니다. 로그인이 성공하면 John이 파트너 센터 대시보드 개요 페이지로 다시 리디렉션됩니다.

4. John이 파트너 센터에서 MFA로 보호되는 페이지 중 하나에 액세스하려고 합니다. John이 MFA 확인을 완료하지 않았으므로 파트너 센터에서 John이 Azure AD로 리디렉션되어 MFA 확인을 완료합니다. John은 이번에 처음으로 MFA를 완료해야 하므로 John에게 [MFA에 등록](#mfa-registration-experience)하라는 메시지가 표시됩니다. MFA 등록 및 MFA 확인이 성공하면 이제 John이 MFA로 보호되는 페이지에 액세스할 수 있습니다.

5. Fabrikam에서 사용자에 대해 MFA를 구현하기 하루 전에 John이 새 브라우저 세션을 시작하여 파트너 센터 대시보드 개요 페이지(MFA로 보호되지 않음)로 이동합니다. 파트너 센터에서 John을 Azure AD로 리디렉션하여 MFA 프롬프트 없이 로그인합니다. 

6. John이 파트너 센터에서 MFA로 보호되는 페이지 중 하나에 액세스하려고 합니다. John이 MFA 확인을 완료하지 않았으므로 파트너 센터에서 John이 Azure AD로 리디렉션되어 MFA 확인을 완료합니다. John이 MFA를 등록했으므로 이번에는 MFA 확인을 완료하라는 메시지만 표시됩니다.

> [!NOTE]
>작업: 회사 관리자는 지금 파트너 센터에서 제안하는 [옵션](partner-security-requirements.md#actions-that-you-need-to-take)을 통해 MFA를 구현해야 합니다.

## <a name="partner-center-api"></a>파트너 센터 API

파트너 센터 API는 앱 전용 인증 및 앱 + 사용자 인증을 모두 지원합니다. 

앱 + 사용자 인증을 사용하는 경우 파트너 센터에서 MFA 확인이 필요합니다. 더 구체적으로, 파트너 애플리케이션에서 API 요청을 파트너 센터에 보내려면 액세스 토큰을 요청의 권한 부여 헤더에 포함해야 합니다. 

> [!NOTE]
>[보안 애플리케이션 모델](/partner-center/develop/enable-secure-app-model)은 파트너 센터 API를 호출할 때 Microsoft Azure MFA 아키텍처를 통해 CSP 파트너 및 CPV를 인증하기 위한 안전하고 확장 가능한 프레임워크이며, 테넌트에서 MFA를 사용하도록 설정하기 전에 이를 구현해야 합니다. 

파트너 센터에서 앱 + 사용자 인증을 사용하여 얻은 액세스 토큰이 포함된 API 요청을 받으면 파트너 센터 API에서 *MFA* 값이 *AMR(인증 방법 참조)* 클레임에 있는지 확인합니다. JWT 디코더를 사용하여 예상 AMR(인증 방법 참조) 값이 액세스 토큰에 포함되어 있는지 여부를 확인할 수 있습니다.

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

값이 있는 경우 파트너 센터에서 MFA 확인이 완료된 것으로 결정하여 API 요청을 처리합니다. 값이 없는 경우 파트너 센터 API에서 다음과 같은 응답으로 요청을 거부합니다.

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

앱 전용 인증을 사용하는 경우 앱 전용 인증을 지원하는 API가 MFA를 요구하지 않고 지속적으로 작동합니다.

## <a name="partner-delegated-administration"></a>파트너에게 위임된 관리

### <a name="using-service-portals"></a>서비스 포털 사용

관리 담당자 및 기술 지원팀 담당자를 포함한 파트너 계정은 파트너에게 위임된 관리 권한을 사용하여 Microsoft Online Services 포털, CLI(명령줄 인터페이스) 및 API(앱 + 사용자 인증 사용)를 통해 고객 리소스를 관리할 수 있습니다.

파트너에게 위임된 관리 권한(관리자 위임)을 사용하여 고객 리소스를 관리하는 Microsoft Online Services 포털에 액세스하는 경우, 이러한 포털에서는 대부분 인증 컨텍스트로 설정된 고객 Azure Active Directory 테넌트를 통해 파트너 계정에서 대화형으로 인증하도록 요구합니다. 이 경우 파트너 계정이 고객 테넌트에 로그인하는 데 필요합니다.

Azure Active Directory에서 이러한 인증 요청을 받으면 파트너 계정에서 MFA 확인을 완료해야 합니다. 파트너 계정이 관리 ID인지, 아니면 페더레이션 ID인지에 따라 다음과 같은 두 가지 사용자 환경을 사용할 수 있습니다.

- 파트너 계정이 **관리** ID인 경우 Azure Active Directory에서 사용자에게 MFA 확인을 완료하라는 메시지를 직접 표시합니다. 파트너 계정이 이전에 MFA를 위해 Azure Active Directory에 등록되지 않은 경우 먼저 [MFA 등록을 완료](#mfa-registration-experience)하도록 사용자에게 요청합니다.

- 파트너 계정이 **페더레이션** ID인 경우 파트너 관리자가 Azure Active Directory에서 페더레이션을 구성한 방법에 따라 이 환경이 달라집니다. Azure Active Directory에서 페더레이션을 설정하는 경우 파트너 관리자는 페더레이션 ID 공급자에서 MFA를 지원하는지 여부를 Azure Active Directory에 나타낼 수 있습니다. 이 경우 Azure Active Directory에서 사용자가 페더레이션 ID 공급자로 리디렉션되어 MFA 확인을 완료합니다. 그렇지 않으면 Azure Active Directory에서 사용자에게 MFA 확인을 완료하라는 메시지를 직접 표시합니다. 파트너 계정이 이전에 MFA를 위해 Azure Active Directory에 등록되지 않은 경우 먼저 [MFA 등록을 완료](#mfa-registration-experience)하도록 사용자에게 요청합니다.

전반적인 환경은 최종 고객 테넌트가 관리자를 대신하여 MFA를 구현한 시나리오와 비슷합니다. 예를 들어 고객 테넌트에서 [Azure AD 보안 기본값](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 사용하도록 설정했습니다. 이 경우 관리 권한이 있는 모든 계정에서 관리 담당자 및 기술 지원팀 담당자를 포함하여 MFA 확인을 통해 고객 테넌트에 로그인해야 합니다. 테스트를 위해 파트너는 고객 테넌트에서 [Azure AD 보안 기본값](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 사용하도록 설정한 다음, 파트너에게 위임된 관리 권한을 사용하여 고객 테넌트에 액세스하려고 시도할 수 있습니다.

> [!NOTE]
> 일부 Microsoft Online Services 포털에서는 파트너에게 위임된 관리 권한을 사용하여 고객 리소스에 액세스할 때 파트너 계정에서 고객 테넌트에 로그인해야 합니다. 이를 대신하여 파트너 계정만 파트너 테넌트에 로그인하도록 요구합니다. 예를 들어 Exchange 관리 센터가 있습니다. 시간이 지남에 따라 이러한 포털에서는 파트너에게 위임된 관리 권한을 사용할 때 파트너 계정에서 고객 테넌트에 로그인해야 합니다.

### <a name="using-service-apis"></a>서비스 API 사용

일부 Microsoft Online Services API(예: Azure Resource Manager, Azure AD Graph, Microsoft Graph 등)는 파트너에게 위임된 관리 권한을 사용하여 고객 리소스를 프로그래밍 방식으로 관리할 수 있도록 지원합니다. 이러한 API에서 파트너에게 위임된 관리 권한을 활용하려면 파트너 애플리케이션에서 액세스 토큰을 API 요청 권한 부여 헤더에 포함해야 합니다. 여기서는 인증 컨텍스트로 설정된 고객 Azure AD를 통해 Azure AD에서 사용자 계정을 인증하여 액세스 토큰을 가져옵니다. 파트너 애플리케이션은 파트너 사용자 계정에서 고객 테넌트에 로그인하는 데 필요합니다.

Azure AD에서 이러한 인증 요청을 받으면 Azure AD에서 파트너 사용자 계정이 MFA 확인을 완료하도록 요구합니다. 파트너 사용자 계정이 이전에 MFA에 등록되지 않은 경우 먼저 MFA 등록을 완료하라는 메시지가 사용자 계정에 표시됩니다.

파트너에게 위임된 관리 권한을 사용하여 이러한 API와 통합된 모든 파트너 애플리케이션은 이 기능의 영향을 받습니다. 파트너 애플리케이션에서 이러한 API를 중단 없이 계속 사용할 수 있도록 하려면 다음을 수행합니다.

- 파트너는 Azure AD에서 비대화형 사용자 인증 방법을 사용하여 액세스 토큰을 가져오지 않아야 합니다. [암호 흐름](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)과 같은 비대화형 사용자 인증 방법을 사용하는 경우 Azure AD에서 사용자에게 MFA 확인을 완료하라는 메시지를 표시할 수 없습니다. 파트너는 대신 [OpenID Connect 흐름](/azure/active-directory/develop/v1-protocols-openid-connect-code)과 같은 대화형 사용자 인증 방법을 사용하도록 전환해야 합니다.

- 대화형 사용자 인증 방법 중에는 파트너가 MFA에 대해 이미 사용하도록 설정된 파트너 사용자 계정을 사용해야 합니다. 또는 Azure AD에서 메시지가 표시되면 파트너가 로그인 중에 MFA 등록 및 MFA 확인을 완료할 수 있습니다.

- 이는 최종 고객 테넌트가 관리자를 대신하여 MFA를 구현한 시나리오와 비슷합니다. 예를 들어 고객 테넌트에서 [Azure AD 보안 기본값](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 사용하도록 설정했습니다. 이 경우 관리 권한이 있는 모든 사용자 계정에서 관리 담당자 및 기술 지원팀 담당자를 포함하여 MFA 확인을 통해 고객 테넌트에 로그인해야 합니다. 테스트를 위해 파트너는 고객 테넌트에서 [Azure AD 보안 기본값](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 사용하도록 설정한 다음, 파트너에게 위임된 관리 권한을 사용하여 프로그래밍 방식으로 고객 테넌트에 액세스하려고 시도할 수 있습니다.

### <a name="mfa-registration-experience"></a>MFA 등록 환경

MFA 확인 중에 파트너 계정이 이전에 MFA에 등록되지 않은 경우 Azure AD에서 사용자에게 먼저 MFA 등록을 완료하라는 메시지를 표시합니다.

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA 등록 1단계":::

**다음** 을 클릭하면 사용자에게 확인 방법 목록에서 선택하라는 메시지가 표시됩니다.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA 등록 1단계":::

등록이 성공하면 사용자가 선택한 확인에 따라 MFA 확인을 완료해야 합니다.

## <a name="request-for-technical-exception"></a>기술 예외 요청

Microsoft Online Services와 관련된 기술적 문제가 발생하고 실행 가능한 솔루션 또는 해결 방법이 없는 경우 MFA 확인을 억제하기 위해 파트너가 기술 예외를 적용할 수 있습니다. 이렇게 하려면 먼저 다음 섹션을 검토하세요.

- [파트너가 보고하는 일반적인 문제 목록](#list-of-common-issues-reported-by-partners)
- [기술 예외 요청을 제출하는 방법](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>파트너가 보고하는 일반적인 문제 목록
기술 예외를 적용하기 전에 다른 파트너가 보고한 일반적인 문제 목록을 검토하여 기술 예외에 대한 타당한 이유인지를 파악합니다.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>문제 1: 파트너가 파트너 에이전트에 대해 MFA를 구현하는 데 더 많은 시간이 필요함
파트너가 파트너에게 위임된 관리 권한을 사용하여 고객 리소스를 관리하기 위해 Microsoft Online Services 포털에 액세스해야 하는 파트너 에이전트에 대해 MFA 구현을 시작하지 않았거나 아직 진행 중입니다. 파트너가 MFA 구현을 완료하는 데 더 많은 시간이 필요합니다. 이 문제는 기술 예외에 대한 타당한 이유인가요?

**대답** : 아니요. 파트너는 중단을 방지하기 위해 사용자에 대해 MFA를 구현하도록 계획해야 합니다.

> [!NOTE]
> 파트너가 파트너 에이전트에 대해 MFA를 구현하지 않은 경우에도, 파트너 에이전트가 고객 테넌트에 로그인하는 중에 메시지가 표시될 때 MFA 등록 및 MFA 확인을 완료할 수 있으면, 파트너에게 위임된 관리 권한을 사용하여 Microsoft Online Services 포털에 계속 액세스할 수 있습니다. MFA 등록을 완료하더라도 사용자가 MFA를 사용하도록 자동으로 설정되지 않습니다.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>문제 2: 파트너가 위임된 관리 권한을 사용하지 않는 사용자 계정에 대해 MFA를 구현하지 않음
파트너에는 파트너에게 위임된 관리 권한을 사용하여 고객 리소스를 관리하기 위해 Microsoft Online Services 포털에 액세스할 필요가 없는 파트너 테넌트의 일부 사용자가 있습니다. 파트너는 이러한 사용자에 대해 MFA를 구현하고 있으며, 완료하는 데 더 많은 시간이 필요합니다. 이 문제는 기술 예외에 대한 타당한 이유인가요?

**대답** : 아니요. 이러한 사용자 계정은 파트너에게 위임된 관리 권한을 사용하여 고객 리소스를 관리하지 않으므로 고객 테넌트에 로그인할 필요가 없습니다. 고객 테넌트에 로그인하는 중에 MFA 확인을 요구하는 Azure AD의 영향을 받지 않습니다.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>문제 3: 파트너가 사용자 서비스 계정에 대해 MFA를 구현하지 않음
파트너에는 파트너 테넌트의 일부 사용자 계정이 있으며, 이러한 계정은 디바이스에서 서비스 계정으로 사용됩니다. 이러한 계정은 파트너에게 위임된 관리 권한을 사용하여 고객 리소스를 관리하기 위해 파트너 센터 또는 Microsoft Online Services 포털에 액세스할 필요가 없는 낮은 권한의 계정입니다. 이 문제는 기술 예외에 대한 타당한 이유인가요?

**대답** : 아니요. 이러한 사용자 계정은 파트너에게 위임된 관리 권한을 사용하여 고객 리소스를 관리하지 않으므로 고객 테넌트에 로그인할 필요가 없습니다. 고객 테넌트에 로그인하는 중에 MFA 확인을 요구하는 Azure AD의 영향을 받지 않습니다.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>문제 4: 파트너가 MS Authenticator 앱을 사용하여 MFA를 구현할 수 없음
파트너에는 직원이 개인 모바일 디바이스를 작업 영역으로 가져올 수 없도록 하는 "클린 데스크" 정책이 있습니다. 개인 모바일 디바이스에 액세스하지 않으면 직원이 Azure AD 보안 기본값에서 지원하는 유일한 MFA 확인인 MS Authenticator 앱을 설치할 수 없습니다. 이 문제는 기술 예외에 대한 타당한 이유인가요?

**대답** : 아니요, 이는 기술적 예외에 대한 타당한 이유가 아닙니다. 파트너는 파트너 센터에 액세스할 때 직원이 여전히 MFA 확인을 완료할 수 있도록 다음과 같은 대안을 고려해야 합니다.
- 파트너는 추가 확인 방법을 제공할 수 있는 Azure AD Premium 또는 타사 MFA 솔루션(Azure AD와 호환)에 가입할 수도 있습니다.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>문제 5: 레거시 인증 프로토콜을 사용하므로 파트너가 MFA를 구현할 수 없음
파트너에는 아직도 MFA와 호환되지 않는 레거시 인증 프로토콜을 사용하는 일부 파트너 에이전트가 있습니다. 예를 들어 사용자는 레거시 인증 프로토콜을 기반으로 하는 Outlook 2010을 여전히 사용하고 있습니다. 이러한 파트너 에이전트에 대해 MFA를 사용하도록 설정하면 레거시 인증 프로토콜의 사용이 중단됩니다.

**대답** : 아니요, 이는 기술적 예외에 대한 타당한 이유가 아닙니다. 레거시 인증 프로토콜은 MFA 확인을 통해 보호할 수 없고 자격 증명 손상에 훨씬 취약하여 잠재적으로 보안에 영향을 주므로 파트너는 이러한 인증 프로토콜을 사용하지 않는 것이 좋습니다. 레거시 인증 프로토콜을 사용하지 않도록 전환할 수 없는 경우 파트너는 애플리케이션 암호의 사용을 지원하는 Azure AD Premium에 가입하는 것을 고려해야 합니다. 애플리케이션 암호는 일회성 시스템 생성 암호이며, 일반적으로 사용자 생성 암호보다 더 강력합니다. 애플리케이션 암호를 사용하면 파트너는 사용자에 대해 MFA를 구현할 수 있으며, 레거시 인증 프로토콜에 대해서만 애플리케이션 암호로 대체할 수 있습니다.

[기본 인증 및 Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282)에 대한 게시물을 참조하고, 레거시 Outlook 인증 지원에 대한 최신 계획을 이해하고. [Exchange 팀 블로그](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange)에 따라 예정된 뉴스를 받으세요. 

> [!NOTE]
> 파트너가 파트너 에이전트에 대해 MFA를 구현하지 않은 경우에도, 파트너 에이전트가 고객 테넌트에 로그인하는 중에 메시지가 표시될 때 MFA 등록 및 MFA 확인을 완료할 수 있으면, 파트너에게 위임된 관리 권한을 사용하여 Microsoft Online Services 포털에 계속 액세스할 수 있습니다. MFA 등록을 완료하더라도 사용자가 MFA를 사용하도록 자동으로 설정되지 않습니다.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>문제 6: 파트너가 Azure AD에서 인식되지 않는 타사 MFA를 구현함
파트너가 타사 MFA 솔루션을 사용하여 사용자에 대해 MFA를 구현했습니다. 그러나 파트너는 사용자 인증 중에 MFA 확인이 완료되었음을 Azure AD에 릴레이하도록 타사 MFA 솔루션을 올바르게 구성할 수 없습니다. 이 문제는 기술 예외에 대한 타당한 이유인가요?

**대답** : 예, 이 문제는 기술 예외에 대한 타당한 이유로 간주될 수 있습니다. 기술 예외 요청을 제출하기 전에 타사 MFA 솔루션 공급자에게 *authenticationmethodsreferences* 클레임( *multipleauthn* 값 포함)을 Azure AD로 전달하여 사용자 인증 중에 MFA 확인이 완료되었음을 나타내도록 MFA 솔루션을 구성할 수 없는지 확인합니다. 기술 예외 요청을 제출하는 동안 사용된 타사 MFA 솔루션의 세부 정보를 제공하고, 통합 방법(예: ID 페더레이션 또는 Azure AD 사용자 지정 제어 사용)을 표시하고, 기술 예외 요청에서 다음 정보를 지원 문서로 제공해야 합니다.

- 타사 MFA 구성

- 타사 MFA 사용 계정에서 실행되는 [파트너 보안 요구 사항 테스트](/powershell/partnercenter/test-partner-security-requirements)의 결과

- 사용하고 있거나 사용하려는 타사 MFA 솔루션에 대한 구매 주문

### <a name="how-to-submit-a-request-for-technical-exception"></a>기술 예외 요청을 제출하는 방법

기술 예외 요청을 제출하려면 다음을 수행합니다.

1. 글로벌 관리자 또는 관리 담당자 권한으로 파트너 센터에 로그인합니다.

2. **지원** > **파트너 지원 요청** 으로 차례로 이동하고 **새 요청** 을 클릭하여 새 파트너 서비스 요청을 만듭니다.

3. 검색 상자에서 **MFA - 예외 요청** 을 검색합니다. 또는 [범주]에서 **CSP** 를 선택하고, [항목]에서 **계정, 온보딩, 액세스** 를 선택하고, 하위 항목에서 **MFA - 예외 요청** 을 선택하고, **다음 단계** 를 선택합니다.

4. 기술 예외에 대한 서비스 요청을 제출하는 데 필요한 세부 정보를 제공하고, **제출** 을 클릭합니다.

Microsoft에서 기술 예외 요청에 대한 응답을 제공하는 데 최대 3일 정도 걸릴 수 있습니다.