---
title: 파트너 테 넌 트에 대 한 재조정 MFA | 파트너 센터
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 테 넌 트에 대해 재조정 MFA를 사용 하 여 고객 리소스에 대 한 액세스를 보호 하는 방법을 알아봅니다. 샘플 시나리오를 포함 합니다.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급업체, CPV, 다단계 인증, MFA, 보안 애플리케이션 모델, 보안 앱 모델, 보안
ms.localizationpriority: medium
ms.openlocfilehash: f0beb695bee9a67f79373ea903158de3fbb66851
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943106"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>파트너 테 넌 트에 대 한 MFA (재조정 Multi-factor Authentication)

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 관리자

이러한 파트너는 다음 영역에 대 한 MFA 확인을 완료 해야 합니다.

- [파트너 센터 대시보드](#partner-center-dashboard) (대상 H1 CY2020)
- [파트너 센터 API](#partner-center-api) (대상 H1 CY2020)
- [파트너 위임 된 관리](#partner-delegated-administration) (2019 년 11 월 18 일부 터)

이 기능의 목적은 파트너가 자격 증명을 손상 시 키 지 못하도록 고객 리소스에 대 한 액세스를 보호 하는 데 도움을 주는 것입니다.

## <a name="partner-center-dashboard"></a>파트너 센터 대시보드
파트너 센터 대시보드의 특정 페이지는 다음을 포함 하 여 MFA로 보호 됩니다.

* **고객** 탭의 모든 페이지
* **지원 > 고객 요청** 탭의 모든 페이지

이러한 페이지에 액세스 하려고 시도 했지만 이전에 MFA 확인을 완료 하지 않은 경우에는이 작업을 수행 해야 합니다.

다음 사용자 유형에는 이러한 MFA로 보호 된 페이지에 액세스할 수 있는 권한이 부여 되므로 다음을 포함 하 여이 기능의 영향을 받습니다.

* 관리 에이전트
* 판매 에이전트
* 기술 지원팀 에이전트

이 작업을 수행 하는 방법을 설명 하기 위해 다음 두 가지 예제를 고려 합니다.

**예제 1: 파트너가 Azure AD MFA를 구현 했습니다.**
1.  Jane은 CSP Contoso에 대해 작동 합니다. Contoso는 Azure AD MFA를 사용 하 여 Contoso partner 테 넌 트의 모든 사용자에 대해 MFA를 구현 했습니다.
2.  자신의 워크스테이션에서 Jane은 새 브라우저 세션을 시작 하 고 파트너 센터 대시보드 개요 페이지 (MFA로 보호 되지 않음)로 이동 합니다. 파트너 센터는 Jane을 Azure AD로 리디렉션하여 로그인 합니다.
3.  Contoso에서 기존 Azure AD MFA를 설정 했기 때문에 MFA 확인을 완료 하려면 Jane이 필요 합니다. 로그인 및 MFA 확인에 성공 하면 Jane은 파트너 센터 대시보드 개요 페이지로 다시 리디렉션됩니다.
4.  Jane은 파트너 센터에서 MFA로 보호 된 페이지 중 하나에 액세스 하려고 시도 합니다. Jane은 이전에 로그인 하는 동안 MFA 확인을 이미 완료 했으므로 Jane은 mfa 인증을 다시 수행 하지 않고도 MFA로 보호 된 페이지에 액세스할 수 있습니다.

**예 2: 파트너가 id 페더레이션을 사용 하 여 타사 MFA를 구현 했습니다.**
1. Trent는 CSP에 대해 작동 합니다. 정문은 id 페더레이션을 통해 Azure AD와 통합 된 타사 MFA를 사용 하 여 정문 partner 테 넌 트의 모든 사용자에 대해 MFA를 구현 했습니다.
2. 자신의 워크스테이션에서 Trent는 새 브라우저 세션을 시작 하 고 파트너 센터 대시보드 개요 페이지 (MFA로 보호 되지 않음)로 이동 합니다. 파트너 센터는 Justin을 Azure AD로 리디렉션하여 로그인 합니다.
3. Azure AD는 id 페더레이션을 설정 했기 때문에 페더레이션 id 공급자로 Trent를 리디렉션하여 로그인 및 MFA 확인을 완료 합니다. 로그인 및 MFA 확인이 성공적으로 완료 되 면 Trent가 Azure AD로 다시 리디렉션되고 파트너 센터 대시보드 개요 페이지로 리디렉션됩니다.
4. Justin는 파트너 센터에서 MFA로 보호 된 페이지 중 하나에 액세스 하려고 시도 합니다. 이전에 로그인 하는 동안 Trent에서 MFA 확인을 이미 완료 했으므로 Trent는 mfa 인증을 다시 수행 하지 않고도 MFA 보호 페이지에 액세스할 수 있습니다.

**예 3: 파트너가 MFA를 구현 하지 않았습니다.**
1. John은 CSP Fabrikam에 대해 작동 합니다. Fabrikam은 Fabrikam 파트너 테 넌 트의 모든 사용자에 대해 MFA를 구현 하지 않았습니다.
2. 자신의 워크스테이션에서 새 브라우저 세션을 시작 하 고 파트너 센터 대시보드 개요 페이지 (MFA로 보호 되지 않음)로 이동 합니다. 파트너 센터는 John을 Azure AD로 리디렉션하여 로그인 합니다.
3. Fabrikam은 MFA를 구현 하지 않았으므로 MFA 확인을 완료할 필요가 없습니다. 성공적으로 로그인 되 면 John은 파트너 센터 대시보드 개요 페이지로 다시 리디렉션됩니다.
4. John은 파트너 센터에서 MFA로 보호 된 페이지 중 하나에 액세스 하려고 시도 합니다. John이 MFA 확인을 완료 하지 않았기 때문에 파트너 센터는 John을 Azure AD로 리디렉션하여 MFA 확인을 완료 합니다. John이 MFA를 완료 하는 데 처음으로 필요 하기 때문에 John은 Microsoft Authenticator 앱을 사용 하 여 MFA에 등록 하도록 요청 했습니다. MFA를 등록 하 고 MFA를 성공적으로 확인 한 후 John은 이제 MFA로 보호 된 페이지에 액세스할 수 있습니다.

## <a name="partner-center-api"></a>파트너 센터 API

파트너 센터 API는 앱 전용 인증과 앱 + 사용자 인증을 모두 지원 합니다. 앱 + 사용자 인증을 사용 하는 경우 파트너 센터에서 MFA 확인이 필요 합니다. 구체적으로 말해서 파트너 응용 프로그램은 파트너 센터에 API 요청을 보내려고 할 때 요청의 인증 헤더에 액세스 토큰을 포함 해야 합니다. 파트너 센터가 앱 + 사용자 인증을 사용 하 여 얻은 액세스 토큰을 사용 하 여 API 요청을 수신 하는 경우 파트너 센터 API는 *AMR (인증 방법 참조)* 클레임에 *MFA* 값이 있는지 확인 합니다. JWT 디코더를 사용 하 여 액세스 토큰에 필요한 AMR (인증 방법 참조) 값이 포함 되어 있는지 여부를 확인할 수 있습니다.

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
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

값이 있는 경우 파트너 센터는 MFA 확인이 완료 되었음을 확인 하 고 API 요청을 처리 합니다. 값이 없는 경우 파트너 센터 API는 다음 응답으로 요청을 거부 합니다.

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>파트너 위임 된 관리

### <a name="using-service-portals"></a>서비스 포털 사용

관리 에이전트 및 기술 지원팀 에이전트를 비롯 한 파트너 계정은 파트너 위임 된 관리자 권한을 사용 하 여 Microsoft Online Services 포털, CLI (명령줄 인터페이스) 및 Api (앱 + 사용자 인증 사용)를 통해 고객 리소스를 관리할 수 있습니다.

고객 리소스를 관리 하기 위해 파트너 위임 된 관리자 권한을 사용 하 여 Microsoft Online Services 포털에 액세스 하는 경우 이러한 포털의 대부분은 파트너 계정을 대화형으로 인증 하 고 고객 Azure Active Directory 테 넌 트를로 설정 해야 합니다. 인증 컨텍스트-고객 테 넌 트에 로그인 하려면 파트너 계정이 필요 합니다.

Azure Active Directory에서 그러한 인증 요청을 수신 하는 경우 MFA 확인을 완료 하려면 파트너 계정이 필요 합니다. 파트너 계정이 관리 되는 id 인지 페더레이션 id 인지에 따라 다음과 같은 두 가지 사용자 환경을 사용할 수 있습니다.

- 파트너 계정이 **관리 되** 는 id 인 경우 Azure Active Directory는 사용자에 게 MFA 확인을 완료 하 라는 메시지를 직접 표시 합니다. 파트너 계정이 이전에 Azure Active Directory MFA에 등록 되지 않은 경우 사용자에 게 먼저 [mfa 등록을 완료](#mfa-registration-experience) 하 라는 메시지가 표시 됩니다.

- 파트너 계정이 **페더레이션** id 인 경우 환경은 파트너 관리자가 Azure Active Directory에서 페더레이션을 구성 하는 방법에 따라 달라 집니다. Azure Active Directory에서 페더레이션을 설정할 때 파트너 관리자는 페더레이션 id 공급자가 MFA를 지원 하는지 여부를 Azure Active Directory를 나타낼 수 있습니다. 이 경우 Azure Active Directory은 사용자를 페더레이션된 id 공급자로 리디렉션하여 MFA 확인을 완료 합니다. 그렇지 않으면 사용자에 게 MFA 확인을 완료 하 라는 메시지를 직접 표시 하는 Azure Active Directory. 파트너 계정이 이전에 Azure Active Directory MFA에 등록 되지 않은 경우 사용자에 게 먼저 [mfa 등록을 완료](#mfa-registration-experience) 하 라는 메시지가 표시 됩니다.

전반적인 환경은 최종 고객 테 넌 트가 관리자를 위해 MFA를 구현한 시나리오와 매우 비슷합니다. 예를 들어, 고객 테 넌 트는 관리자 [에 게 AZURE AD 기준 정책-mfa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)를 사용 하도록 설정 했습니다 .이 경우 관리 권한이 있는 모든 계정에 관리 권한이 있는 모든 계정에서 관리자 에이전트 및 기술 지원팀 에이전트를 비롯 한 mfa 확인을 통해 고객 테 넌 트 테스트를 위해 파트너는 고객 테 넌 트의 [관리자 정책에 대해 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 를 사용 하도록 설정한 다음, 파트너 위임 된 관리 권한을 사용 하 여 고객 테 넌 트에 액세스할 수 있습니다.

> [!NOTE]
> 파트너 위임 된 관리자 권한을 사용 하 여 고객 리소스에 액세스할 때 모든 Microsoft Online Service 포털에는 파트너 계정이 고객 테 넌 트에 로그인 하는 데 필요 하지 않습니다. 대신 파트너 테 넌 트에 로그인 하는 데 파트너 계정만 필요 합니다. Exchange 관리 센터를 예로 들 수 있습니다. 시간이 지남에 따라 파트너 위임 된 관리자 권한을 사용 하는 경우 이러한 포털이 파트너 계정이 고객 테 넌 트에 로그인 하는 데 필요 합니다.

### <a name="using-service-apis"></a>서비스 Api 사용
일부 Microsoft Online Services Api (예: Azure Resource Manager, Azure AD Graph, Microsoft Graph 등)는 파트너 위임 된 관리자 권한을 사용 하 여 프로그래밍 방식으로 고객 리소스를 관리 하는 파트너를 지원 합니다. 이러한 Api를 사용 하 여 파트너 위임 된 관리자 권한을 활용 하려면 파트너 응용 프로그램에서 API 요청 인증 헤더에 액세스 토큰을 포함 해야 합니다. 여기서는 Azure AD를 사용 하 여 인증 하는 파트너 사용자 계정을 사용 하 여 액세스 토큰을 가져옵니다. 인증 컨텍스트로 설정 된 customer Azure AD입니다. 파트너 응용 프로그램은 파트너 사용자 계정이 고객 테 넌 트에 로그인 하는 데 필요 합니다.

Azure AD가 인증 요청 등을 수신 하는 경우 Azure AD에서 MFA 확인을 완료 하려면 파트너 사용자 계정이 필요 합니다. 이전에 파트너 사용자 계정이 MFA에 등록 되지 않은 경우 사용자 계정에 먼저 MFA 등록을 완료 하 라는 메시지가 표시 됩니다.

파트너 위임 된 관리자 권한을 사용 하 여 이러한 Api와 통합 된 모든 파트너 응용 프로그램은이 기능의 영향을 받습니다. 파트너 응용 프로그램이 중단 없이 이러한 Api를 계속 사용할 수 있도록 하려면 다음을 수행 합니다.

- 파트너는 액세스 토큰을 가져오기 위해 Azure AD에서 비 대화형 사용자 인증 방법을 사용 하지 않도록 해야 합니다. [암호 흐름과](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)같은 비 대화형 사용자 인증 방법을 사용 하는 경우 Azure AD는 사용자에 게 MFA 확인을 완료 하 라는 메시지를 표시할 수 없습니다. 파트너는 대신 [Openid connect Connect flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) 와 같은 대화형 사용자 인증 방법을 사용 하도록 전환 해야 합니다.
- 대화형 사용자 인증 방법 중에는 파트너가 이미 MFA에 대해 사용 하도록 설정 된 파트너 사용자 계정을 사용 해야 합니다. 또는 Azure AD에서 메시지가 표시 되 면 파트너는 로그인 중에 MFA 등록 및 MFA 확인을 완료할 수 있습니다.
- 최종 고객 테 넌 트가 관리자를 위해 MFA를 구현한 시나리오와 매우 비슷합니다. 예를 들어 고객 테 넌 트는 관리자 [에 게 AZURE AD 기준 정책-mfa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)를 사용 하도록 설정 했습니다 .이 경우 관리 권한이 있는 모든 사용자 계정에 관리 권한이 있는 사용자 계정으로 관리자 에이전트 및 기술 지원팀 에이전트를 포함 하 여 mfa 확인이 있는 고객 테 넌 트 테스트를 위해 파트너는 고객 테 넌 트의 [관리자 정책에 대해 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) 를 사용 하도록 설정한 다음, 파트너 위임 된 관리 권한을 사용 하 여 프로그래밍 방식으로 고객 테 넌 트에 액세스할 수 있습니다.

### <a name="mfa-registration-experience"></a>MFA 등록 환경
MFA 확인 중에 파트너 계정이 MFA에 등록 되지 않은 경우 Azure AD는 먼저 MFA 등록을 완료 하 라는 메시지를 표시 합니다.

![MFA 등록 1 단계](images/MfaRegistration1.png)

[ **다음**]을 클릭 하면 사용자에 게 확인 방법 목록 (전화, SMS 및 인증자 앱 포함)을 선택 하 라는 메시지가 표시 됩니다.

![MFA 등록 2 단계](images/MfaRegistration2.png)

등록이 성공적으로 완료 되 면 사용자가 선택한 확인에 따라 MFA 확인을 완료 해야 합니다.



## <a name="request-for-technical-exception"></a>기술 예외 요청

Microsoft Online Services에 대 한 기술적인 문제가 발생 하 고 적절 한 솔루션이 나 해결 방법이 없는 경우에는 ts 확인을 억제 하기 위해 파트너가 기술 예외를 적용할 수 있습니다. 이 작업을 수행 하기 전에 다음 섹션을 검토 하세요.

 - [파트너가 보고 하는 일반적인 문제 목록](#list-of-common-issues-reported-by-partners)
 - [기술 예외에 대 한 요청을 제출 하는 방법](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>파트너가 보고 하는 일반적인 문제 목록
기술 예외를 적용 하기 전에 다른 파트너가 보고 하는 일반적인 문제 목록을 검토 하 여 유효한 기술 예외 원인 인지 파악 하십시오.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>문제 1: 파트너가 파트너 에이전트에 대해 MFA를 구현 하는 데 더 많은 시간이 필요 합니다.
파트너가 시작 되지 않았거나, 고객 리소스를 관리 하기 위해 파트너 위임 된 관리 권한을 사용 하 여 Microsoft Online Services 포털에 액세스 해야 하는 파트너 에이전트에 대해 MFA를 구현 하는 과정을 진행 하 고 있습니다. 파트너는 MFA 구현을 완료 하는 데 더 많은 시간이 필요 합니다. 이는 올바른 기술 예외 원인 인가요?

**Válasz:** Nem. 파트너는 중단을 방지 하기 위해 사용자에 대 한 MFA를 구현 하도록 계획 해야 합니다.

> [!NOTE]
> 파트너가 파트너 에이전트에 대해 MFA를 구현 하지 않은 경우에도 파트너 에이전트는 MFA 등록 및 MFA 확인을 완료할 수 있는 경우 파트너 위임 된 관리 권한을 사용 하 여 Microsoft Online Services 포털에 계속 액세스할 수 있습니다. 고객 테 넌 트에 로그인 하는 동안 메시지가 표시 됩니다. MFA 등록을 완료 하면 MFA에 대해 사용자가 자동으로 사용 하도록 설정 되지 않습니다.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>문제 2: 파트너가 위임 된 관리자 권한을 사용 하지 않는 사용자 계정에 대해 MFA를 구현 하지 않았습니다.
파트너는 파트너 테 넌 트의 일부 사용자에 게 파트너 위임 된 관리 권한을 사용 하 여 고객 리소스를 관리 하기 위해 Microsoft Online Services 포털에 액세스할 필요가 없습니다. 파트너는 이러한 사용자에 대해 MFA를 구현 하는 중 이며 완료 하는 데 시간이 더 필요 합니다. 이는 올바른 기술 예외 원인 인가요?

**Válasz:** Nem. 이러한 사용자 계정은 파트너 위임 된 관리 권한을 사용 하 여 고객 리소스를 관리 하지 않으므로 고객 테 넌 트에 로그인 하는 데 필요 하지 않습니다. 고객 테 넌 트에 로그인 하는 동안 MFA 확인을 요구 하는 Azure AD의 영향을 받지 않습니다.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>문제 3: 파트너가 사용자 서비스 계정에 대해 MFA를 구현 하지 않았습니다.
파트너는 장치에서 서비스 계정으로 사용 중인 파트너 테 넌 트의 일부 사용자 계정을 가집니다. 일반적으로 파트너 위임 된 관리 권한을 사용 하 여 고객 리소스를 관리 하기 위해 액세스 파트너 센터 또는 Microsoft Online Services 포털이 필요 하지 않은 낮은 권한의 계정입니다. 이는 올바른 기술 예외 원인 인가요?

**Válasz:** Nem. 이러한 사용자 계정은 파트너 위임 된 관리 권한을 사용 하 여 고객 리소스를 관리 하지 않으므로 고객 테 넌 트에 로그인 하는 데 필요 하지 않습니다. 고객 테 넌 트에 로그인 하는 동안 MFA 확인을 요구 하는 Azure AD의 영향을 받지 않습니다.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>문제 4: 파트너가 MS Authenticator 앱을 사용 하 여 MFA를 구현할 수 없음
파트너는 직원에 게 개인 모바일 장치를 회사 영역으로 가져올 수 없도록 하는 "청소 데스크" 정책이 있습니다. 개인 모바일 장치에 액세스 하지 않으면 직원은 Azure AD 기준 정책에서 지원 되는 유일한 MFA 확인 인 MS Authenticator 앱을 설치할 수 없습니다. 이는 올바른 기술 예외 원인 인가요?

**답변**: 아니요, 올바른 기술 예외 이유가 아닙니다. 파트너는 파트너 센터에 액세스할 때 여전히 MFA 확인을 완료할 수 있도록 다음과 같은 대안을 고려해 야 합니다.
- MS Authenticator 앱 외에도, Azure AD 기준 정책은 Microsoft Windows를 실행 하는 지원 되는 Windows 컴퓨터 일 수 있는 타사의 호환 인증 앱과 함께 사용할 수 있습니다.
- 파트너는 추가 인증 방법을 제공할 수 있는 Azure AD Premium 또는 타사 MFA 솔루션 (Azure AD와 호환)에 등록할 수도 있습니다.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>문제 5: 파트너가 레거시 인증 프로토콜을 사용 하기 때문에 MFA를 구현할 수 없음
파트너에는 아직 MFA와 호환 되지 않는 레거시 인증 프로토콜을 사용 하는 일부 파트너 에이전트가 있습니다. 예를 들어 사용자는 여전히 레거시 인증 프로토콜을 기반으로 하는 Outlook 2010를 사용 하 고 있습니다. 이러한 파트너 에이전트에 대해 MFA를 사용 하도록 설정 하면 레거시 인증 프로토콜의 사용이 중단 됩니다.

**답변**: 아니요, 올바른 기술 예외 이유가 아닙니다. 파트너는 이러한 프로토콜을 MFA 인증으로 보호할 수 없고 자격 증명 손상에 훨씬 더 취약 하기 때문에 보안에 영향을 주므로 레거시 인증 프로토콜을 사용 하지 않는 것이 좋습니다. 레거시 인증 프로토콜을 사용 하지 않고 이동 하는 것이 옵션이 아닌 경우 파트너는 응용 프로그램 암호 사용을 지 원하는 Azure AD Premium에 등록 하는 것을 고려해 야 합니다. 응용 프로그램 암호는 대개 사람이 생성 한 암호 보다 강력한 일회용 시스템 생성 암호입니다. 파트너는 응용 프로그램 암호를 사용 하 여 사용자에 대해 MFA를 구현할 수 있으며, 레거시 인증 프로토콜만 응용 프로그램 암호로 대체 합니다.

> [!NOTE]
> 파트너가 파트너 에이전트에 대해 MFA를 구현 하지 않은 경우에도 파트너 에이전트는 MFA 등록 및 MFA 확인을 완료할 수 있는 경우 파트너 위임 된 관리 권한을 사용 하 여 Microsoft Online Services 포털에 계속 액세스할 수 있습니다. 고객 테 넌 트에 로그인 하는 동안 메시지가 표시 됩니다. MFA 등록을 완료 하면 MFA에 대해 사용자가 자동으로 사용 하도록 설정 되지 않습니다.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>문제 6: 파트너가 MFA를 지원 하지 않는 Exchange Online PowerShell을 사용 하 고 있습니다.
파트너는 고객을 대신 하 여 Exchange online 서비스를 관리 하기 위해 파트너 위임 된 관리 권한을 가진 Exchange Online PowerShell을 사용 합니다. Exchange Online PowerShell은 MFA를 지원 하지 않습니다. 파트너가 사용자를 위해 MFA를 구현 하는 경우 이러한 사용자는 더 이상 Exchange Online PowerShell에 액세스할 수 없게 됩니다. 이는 올바른 기술 예외 원인 인가요?

**답변**: 예, 올바른 기술 예외 원인으로 간주할 수 있습니다. [파트너 위임 된 관리를 지 원하는 기존 Exchange Online PowerShell 모듈](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) 에는 파트너 사용자가 고객 테 넌 트에 로그인 할 필요가 없으므로 MFA 확인이 필요한 Azure AD의 영향을 받지 않습니다. 그러나 MFA와 호환 되지 않습니다. Microsoft Exchange Online 팀은 파트너 위임 된 관리 권한 및 MFA를 모두 지 원하는 새로운 PowerShell 모듈을 개발 하 고 있습니다. 새 PowerShell 모듈을 사용할 수 있을 때까지 파트너는 기존 PowerShell 모듈을 사용 해야 하는 사용자에 대해 MFA를 구현할 수 없습니다. 이러한 사용자가 Azure AD로 인해 다른 Microsoft Online Services에 액세스 하는 데 문제가 발생 하는 경우 테 넌 트 간 로그인 중에 MFA 확인이 필요한 파트너는 MFA 확인을 표시 하지 않도록 기술 예외를 요청할 수 있습니다.

> [!NOTE]
> 파트너가 Exchange Online PowerShell 모듈에 액세스 해야 하는 사용자에 대해 MFA를 구현할 수 없더라도 이러한 사용자는 Microsoft Online Services에 액세스 하 여 제공 된 파트너 위임 된 관리 권한을 사용 하 여 고객 리소스를 관리할 수 있습니다. 고객 테 넌 트에 로그인 하는 동안 메시지가 표시 되 면 MFA 등록 및 MFA 확인을 완료할 수 있습니다. MFA 등록을 완료 하면 MFA에 대해 사용자가 자동으로 사용 하도록 설정 되지 않으므로 Exchange Online PowerShell 모듈에 대 한 액세스에는 영향을 주지 않습니다.

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>문제 7: 파트너가 Azure AD에서 인식 되지 않는 타사 MFA를 구현 했습니다.
파트너는 타사 MFA 솔루션을 사용 하 여 사용자에 대해 MFA를 구현 했습니다. 그러나 파트너가 사용자 인증 중에 MFA 확인이 완료 되었음을 Azure AD로 릴레이 하도록 타사 MFA 솔루션을 올바르게 구성할 수 없습니다. 이는 올바른 기술 예외 원인 인가요?

**답변**: 예, 올바른 기술 예외 원인으로 간주할 수 있습니다. 기술 예외에 대 한 요청을 제출 하기 전에 타사 MFA 솔루션 공급자에 게 문의 하 여 사용자 인증 중에 MFA 확인이 완료 되었음을 나타내는 *authenticationmethodsreferences* 클레임 (값 *Multipleauthn*)을 Azure AD로 전달 하도록 mfa 솔루션을 구성할 수 없는지 확인 하세요. 기술 예외에 대 한 요청을 제출 하는 동안 사용 된 타사 MFA 솔루션에 대 한 세부 정보를 제공 하 고 통합 방법 (예: id 페더레이션 또는 Azure AD 사용자 지정 컨트롤 사용)을 지정 하세요.

### <a name="how-to-submit-a-request-for-technical-exception"></a>기술 예외에 대 한 요청을 제출 하는 방법

기술 예외에 대 한 요청을 제출 하려면:

1. 전역 관리자 또는 관리 에이전트로 파트너 센터에 로그인 합니다.
2.  > **파트너 지원 요청** **지원** 으로 이동한 다음 **새 요청**을 클릭 하 여 새 파트너 서비스 요청을 만듭니다.
4. **MFA 및 보안 응용 프로그램 모델** 항목 아래에서 문제 유형으로 **기술 예외에 대 한 선택 (제출 요청을 제출** 합니다.
6. 기술 예외에 대 한 서비스 요청을 제출 하는 데 필요한 세부 정보를 제공 하 고 **제출**을 클릭 합니다.

Microsoft는 기술 예외에 대 한 요청에 대 한 응답을 제공 하는 데 최대 3 일까지 걸릴 수 있습니다.
