---
title: 파트너 보안 요구 사항 FAQ | 파트너 센터
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 보안 요구 사항에 대해 자주 묻는 질문
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급업체, CPV, 다단계 인증, MFA, 보안 애플리케이션 모델, 보안 앱 모델, 보안
ms.localizationpriority: high
ms.openlocfilehash: 72ad7bab25c295fa039e7b29f9d4369c0434814c
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2020
ms.locfileid: "80529772"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>파트너 보안 요구 사항에 대해 자주 묻는 질문

**적절한 사용자**

- 사용하도록 설정된 모든 사용자(게스트 사용자 포함)

이 문서에는 [파트너 보안 요구 사항](partner-security-requirements.md)에 대해 자주 묻는 질문이 몇 가지 포함되어 있습니다.

## <a name="partner-security-requirements"></a>파트너 보안 요구 사항

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>파트너 보안 요구 사항은 무엇이며 파트너가 구현해야 하는 이유는 무엇인가요?

더 강력하고 지속적인 보안 및 개인 정보 보호가 최우선 순위이며, 파트너가 고객과 테넌트를 보호할 수 있도록 지속적으로 지원하고 있습니다. 주로 ID 손상 사건과 관련된 보안 공격이 더욱 정교해 지고 있으며 그 수도 증가하고 있습니다. 예방 컨트롤이 보안 공격을 방지하기 위한 전반적인 방어 전략에서 주요 역할을 수행함에 따라 2019년에는 [필수 보안 요구 사항](partner-security-requirements.md)을 도입했습니다. CSP(클라우드 솔루션 공급자) 프로그램, 제어판 공급업체 및 관리자에 참여하는 모든 파트너는 규정을 준수하기 위한 요구 사항을 구현해야 합니다.

### <a name="what-are-the-key-timelines-and-milestones"></a>주요 타임라인 및 중요 시점은 무엇인가요?

이러한 보안 요구 사항과 관련된 사용 약관은 2019년 Microsoft 파트너 계약에 포함되어 있습니다. CSP 프로그램 참여를 계속 준수하려면 가능한 한 빨리 이러한 보안 요구 사항을 구현해야 합니다.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>이러한 파트너 보안 요구 사항을 구현하지 않으면 어떻게 되나요?

Microsoft 파트너 계약에서는 다단계 인증을 사용자 계정에 적용하고, 파트너 센터 API와 상호 작용할 수 있는 보안 애플리케이션 모델을 채택하도록 요구하고 있습니다. 

이러한 보안 관행을 준수하지 않는 파트너는 CSP 프로그램에서 거래하거나 대표 관리자 권한을 사용하여 고객 테넌트를 관리하는 기능을 손실할 수 있습니다.

### <a name="does-this-apply-to-all-geographies"></a>모든 지역에 적용되나요?

예, 모든 지역에 적용됩니다. 소버린 클라우드(21Vianet, 미국 정부 및 독일)를 통해 거래하는 모든 파트너는 이러한 새 보안 요구 사항을 즉시 적용하고 채택할 것을 적극 권장합니다. 그러나 이러한 파트너는 8월 1일에 적용되는 새로운 보안 요구 사항을 충족할 필요가 없습니다. Microsoft에서는 나중에 소버린 클라우드에 대한 이러한 보안 요구 사항의 적용과 관련된 추가 세부 정보를 제공할 예정입니다.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>계정에 대한 제외를 받을 수 있나요?

아니요, MFA를 적용해야 한다는 요구 사항에서는 어떠한 사용자 계정도 제외할 수 없습니다. 파트너에게 엄청난 권한이 부여되기 때문에 Microsoft 파트너 계약에서는 파트너 테넌트의 각 계정에 대해 다단계 인증을 적용하도록 요구하고 있습니다.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>파트너 보안 요구 사항을 충족했는지 확인하려면 어떻게 해야 하나요?

아래 단계를 완료해야 합니다.

- [파트너 보안 요구 사항](https://docs.microsoft.com/partner-center/partner-security-requirements)에서 설명하는 모든 요구 사항을 충족해야 합니다.
- 파트너 테넌트의 모든 사용자 계정에 다단계 인증이 적용되어 있는지 확인해야 합니다.

작업을 수행할 수 있는 주요 영역을 식별하는 데 도움이 되도록 파트너 센터를 통해 사용할 수 있는 [보안 요구 사항 상태](https://partner.microsoft.com/pcv/security/compliance) 보고서를 제공합니다.

상태 보고서에 대한 자세한 내용은 [파트너 보안 요구 사항 상태](https://docs.microsoft.com/partner-center/partner-security-compliance)를 참조하세요.

## <a name="required-actions"></a>필요한 작업

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>요구 사항을 충족하기 위해 수행해야 하는 주요 작업은 무엇인가요?

CSP 프로그램의 모든 파트너(직접 청구, 간접 공급자 및 간접 재판매인), 관리자 및 제어판 공급업체는 요구 사항을 충족해야 합니다.

1. **모든 사용자에 대해 MFA 적용**

    CSP 프로그램의 모든 파트너, Advisor 및 제어판 공급업체는 파트너 테넌트의 모든 사용자에 대해 MFA를 적용해야 합니다.

    추가 고려 사항:

    - 간접 공급자는 간접 재판매인과 협력하여 파트너 센터에 아직 온보딩하지 않은 경우 온보딩하고 재판매인이 요구 사항을 충족하도록 해야 합니다.
    - Azure MFA는 TOTP(시간 기반 일회용 암호)를 지원하는 인증자 애플리케이션의 유일한 확인 방법에서 Azure AD 보안 기본값을 통해 파트너 테넌트의 모든 사용자가 무료로 사용할 수 있습니다.
    - 전화 통화나 문자 메시지 같은 다른 방법이 필요한 경우 추가 검증 방법은 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU를 통해 사용할 수 있습니다.
    - 또한 파트너는 Microsoft 상용 클라우드 서비스에 액세스할 때 계정마다 타사 MFA 솔루션을 활용할 수 있습니다.

2. **보안 애플리케이션 모델 프레임워크 채택**

    모든 API(예: Azure Resource Manager, Microsoft Graph, 파트너 센터 API 등)를 사용하여 사용자 지정 통합을 개발하거나 PowerShell과 같은 도구를 사용하여 사용자 지정 자동화를 구현한 모든 파트너는 [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)(보안 애플리케이션 모델 프레임워크)를 채택하여 Microsoft 클라우드 서비스와 통합해야 합니다. 이렇게 하지 않으면 MFA 배포로 인해 중단될 수 있습니다. 다음은 이 모델을 채택하는 방법에 대한 개요 및 지침을 제공하는 리소스입니다.

    - [보안 애플리케이션 모델 개요](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [파트너 센터: 보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP 프로그램의 파트너: 보안 애플리케이션 모델을 활성화하는 .NET 샘플 코드](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [CSP 프로그램의 파트너: 보안 애플리케이션 모델을 활성화하는 Java 샘플 코드](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [파트너 센터 인증 문서](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [파트너 센터 PowerShell MFA(Multi-Factor Authentication) 문서](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    보안 애플리케이션 모델 프레임워크의 채택과 관련하여 제어판을 사용하는 경우 공급업체에 문의하세요.

    제어판 공급업체는 파트너 센터에 제어판 공급업체로 [온보딩](https://docs.microsoft.com/partner-center/enroll-as-cpv)하고 이 요구 사항 구현을 즉시 시작해야 합니다. [파트너 센터: 보안 애플리케이션 모델 프레임워크](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)를 참조하세요. 제어판 공급업체는 자격 증명 대신 CSP 파트너의 동의를 수락하고 관리해야 하며 기존 CSP 파트너의 자격 증명을 모두 제거해야 합니다.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>MFA(Multi-Factor Authentication)란 무엇인가요?

MFA는 개인이 둘 이상의 필수 보안 및 유효성 검사 절차를 통해 인증되는 보안 메커니즘입니다. 이는 다음 인증 방법을 둘 이상 요청하는 방식으로 작동합니다.

- 사용자가 알고 있는 사항(일반적으로 암호)
- 사용자의 소유물(전화기처럼 쉽게 복제되지 않는 신뢰할 수 있는 디바이스)
- 사용자의 신체 관련 항목(생체 인식)

### <a name="what-is-the-cost-of-enabling-mfa"></a>MFA 사용 비용은 무엇인가요?

Microsoft는 Azure AD 보안 기본값 구현을 통해 무료로 MFA를 제공합니다. 이 버전의 MFA를 통해 사용할 수 있는 유일한 확인 옵션은 인증 애플리케이션입니다. 전화 통화나 SMS 메시지가 필요한 경우 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 라이선스를 구매해야 합니다. 또는 타사 솔루션을 활용하여 파트너 테넌트의 각 사용자에게 MFA를 제공할 수 있습니다. 이 경우 사용자가 MFA 솔루션을 적용하고 이를 준수하는지 확인해야 합니다.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>MFA 솔루션이 이미 있는 경우 수행해야 하는 작업은 무엇인가요?

이러한 보안 요구 사항을 통해 파트너 테넌트의 사용자는 Microsoft 상용 클라우드 서비스에 액세스할 때 MFA를 사용하여 인증해야 합니다. 이러한 요구 사항은 타사 솔루션을 사용하여 충족할 수 있습니다. Microsoft는 Azure Active Directory와의 호환성을 위해 독립 ID 공급자에 대한 유효성 검사 테스트를 더 이상 제공하지 않습니다. 제품의 상호 운용성을 테스트하려면 이러한 [지침](https://www.microsoft.com/download/details.aspx?id=56843)을 참조하세요.

> [!IMPORTANT]
> 타사 솔루션을 사용하는 경우 해당 솔루션에서 MFA 값이 포함된 AMR(인증 방법 참조) 클레임을 발급하는지 확인해야 합니다. 타사 솔루션에서 예상 클레임을 발급하는지 확인하는 방법에 대한 자세한 내용은 [파트너 센터 요구 사항 테스트](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)를 참조하세요.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>여러 파트너 테넌트를 사용하여 거래합니다. 모든 파트너 테넌트에 MFA를 구현해야 하나요?

예, MFA는 CSP 프로그램 또는 관리자 프로그램과 연결된 각 Azure Active Directory 테넌트에 적용해야 합니다. Azure Active Directory Premium 라이선스를 구매하려면 각 Azure Active Directory 테넌트의 사용자에 대한 라이선스를 구매해야 합니다.

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>파트너 테넌트의 각 사용자 계정에 대해 MFA를 적용해야 하나요?

예, 각 사용자는 MFA를 적용해야 합니다. 그러나 Azure AD 보안 기본값을 사용하는 경우 해당 기능에서 MFA를 모든 사용자 계정에 적용하므로 추가 작업이 필요하지 않습니다. 보안 기본값을 사용하도록 설정하는 것은 사용자 계정에서 MFA를 준수하고, MFA를 적용할 때 영향을 받지 않는 손쉬운 방법이며 이는 무료입니다.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Microsoft의 직접 청구 파트너입니다. 무엇을 해야 하나요?

직접 청구 클라우드 솔루션 공급자 파트너는 파트너 테넌트의 각 사용자에 대해 MFA를 적용해야 합니다.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>간접 재판매인이며 배포자를 통해서만 거래합니다. 그래도 이 작업을 수행해야 하나요?

모든 간접 재판매인은 파트너 테넌트의 각 사용자에 대해 MFA를 적용해야 합니다. 이 작업은 간접 재판매인도 수행해야 합니다.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>파트너 센터 API를 사용하지 않습니다. 그래도 MFA를 구현해야 하나요?

예, 이 보안 요구 사항은 파트너 테넌트의 파트너 관리 사용자 및 최종 사용자를 포함한 모든 사용자에게 적용됩니다.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>어떤 타사 공급업체에서 Azure Active Directory와 호환되는 MFA 솔루션을 제공하나요?

MFA 공급업체 및 솔루션을 검토할 때 파트너는 선택한 솔루션이 Azure Active Directory와 호환되는지 확인해야 합니다.

Microsoft는 Azure Active Directory와의 호환성을 위해 독립 ID 공급자에 대한 유효성 검사 테스트를 더 이상 제공하지 않습니다. 제품의 상호 운용성을 테스트하려면 이러한 [지침](https://www.microsoft.com/download/details.aspx?id=56843)을 참조하세요.

자세한 내용은 [Azure AD 페더레이션 호환성 목록](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)을 참조하세요.

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>통합 샌드박스에서 MFA를 테스트하려면 어떻게 해야 하나요?

Azure AD 보안 기본값 기능을 사용하거나, 페더레이션을 활용하는 타사 솔루션을 활용할 수 있습니다.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>MFA를 사용하도록 설정하면 고객의 테넌트와 상호 작용하는 방법에 영향을 주나요?

아니요. 이러한 보안 요구 사항의 이행이 고객을 관리하는 방법에 영향을 주지는 않습니다. 위임된 관리 작업은 중단 없이 수행할 수 있습니다.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>제 고객은 파트너 보안 요구 사항의 영향을 받나요?

아니요, 고객의 Azure AD 테넌트에 있는 각 사용자에 대해 MFA를 적용할 필요는 없습니다. 그러나 각 고객과 협력하여 사용자를 보호할 최선의 방법을 확인하는 것이 좋습니다.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>이 요구 사항에서 사용자를 제외할 수 있나요?

아니요, 서비스 계정을 포함하여 파트너 테넌트의 각 사용자는 MFA를 사용하여 인증해야 합니다.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>파트너 보안 요구 사항은 통합 샌드박스에 적용되나요?

예, 파트너 보안 요구 사항은 통합 샌드박스에 적용됩니다. 즉, 통합 샌드박스 테넌트의 사용자에 대해 적절한 MFA 솔루션을 구현해야 합니다. MFA를 제공하려면 Azure AD 보안 기본값을 구현하는 것이 좋습니다.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>응급 액세스(비상) 계정을 구성하려면 어떻게 하나요?

Azure AD 테넌트에서 실수로 잠기지 않도록 하나 또는 두 개의 응급 액세스 계정을 만드는 것이 좋습니다. 파트너 보안 요구 사항과 관련하여 각 사용자는 MFA를 사용하여 인증해야 합니다. 즉, 응급 액세스 계정의 정의를 수정해야 합니다. 이는 MFA에 대해 타사 솔루션을 활용하는 계정일 수 있습니다.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>타사 솔루션을 사용하는 경우 ADFS(Active Directory Federation Service)가 필요한가요?

아니요, 타사 솔루션을 사용하는 경우 ADFS(Active Directory Federation Service)를 사용할 필요가 없습니다. 솔루션 공급업체와 협력하여 솔루션의 요구 사항이 무엇인지 확인하는 것이 좋습니다.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>반드시 Azure AD 보안 기본값을 사용해야 합니까?

아니요, Azure AD 보안 기본값을 사용할 필요는 없습니다.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>MFA 요구 사항을 충족하는 데 조건부 액세스를 사용할 수 있나요?

예, 조건부 액세스를 사용하여 서비스 계정을 포함한 파트너 테넌트의 각 사용자에 대해 MFA를 적용할 수 있습니다. 그러나 파트너가 되려면 매우 높은 권한이 필요하다는 가정하에 각 사용자가 인증할 때마다 MFA 챌린지를 수행하도록 해야 합니다. 즉, MFA 요구 사항을 우회하는 조건부 액세스의 기능을 활용할 수 없습니다.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect에서 사용하는 서비스 계정은 파트너 보안 요구 사항의 영향을 받나요?

아니요, Azure AD Connect에서 사용하는 서비스 계정은 파트너 보안 요구 사항의 영향을 받지 않습니다. MFA를 적용한 결과로 Azure AD Connect에서 문제가 발생하는 경우 Microsoft 지원에 문의하여 기술 지원 요청을 여세요.

## <a name="secure-application-model"></a>보안 애플리케이션 모델

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>요구 사항을 충족하려면 누가 보안 애플리케이션 모델을 채택해야 하나요?

Microsoft는 CSP(클라우드 솔루션 공급자) 파트너 및 CPV(제어판 공급업체)를 인증하기 위해 Multi-Factor Authentication을 활용하는 안전하고 확장 가능한 프레임워크를 도입하고 있습니다. 자세한 내용은 [보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)를 참조하세요. 모든 API(예: Azure Resource Manager, Microsoft Graph, 파트너 센터 API 등)를 사용하여 사용자 지정 통합을 개발하거나 PowerShell과 같은 도구를 사용하여 사용자 지정 자동화를 구현한 모든 파트너는 [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)(보안 애플리케이션 모델 프레임워크)를 채택하여 Microsoft 클라우드 서비스와 통합해야 합니다.

### <a name="what-is-the-secure-application-model"></a>보안 애플리케이션 모델이란 무엇인가요?

Microsoft는 CSP(클라우드 솔루션 공급자) 파트너 및 CPV(제어판 공급업체)를 인증하기 위해 Multi-Factor Authentication을 활용하는 안전하고 확장 가능한 프레임워크를 도입하고 있습니다. 자세한 내용은 [보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)를 참조하세요.  

### <a name="how-do-i-implement-the-secure-application-model"></a>보안 애플리케이션 모델을 구현하려면 어떻게 하나요?

모든 API(예: Azure Resource Manager, Microsoft Graph, 파트너 센터 API 등)를 사용하여 사용자 지정 통합을 개발하거나 PowerShell과 같은 도구를 사용하여 사용자 지정 자동화를 구현한 모든 파트너는 [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)(보안 애플리케이션 모델 프레임워크)를 채택하여 Microsoft 클라우드 서비스와 통합해야 합니다. 이렇게 하지 않으면 MFA 배포로 인해 중단될 수 있습니다. 다음은 이 모델을 채택하는 방법에 대한 개요 및 지침을 제공하는 리소스입니다.

- [보안 애플리케이션 모델 개요](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [파트너 센터: 보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP 프로그램의 파트너: 보안 애플리케이션 모델을 활성화하는 .NET 샘플 코드](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP 프로그램의 파트너: 보안 애플리케이션 모델을 활성화하는 Java 샘플 코드](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [파트너 센터 인증 문서](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [파트너 센터 PowerShell MFA(Multi-Factor Authentication) 문서](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

제어판을 사용하는 경우 보안 애플리케이션 모델 프레임워크 채택과 관련하여 공급업체에 문의해야 합니다.

제어판 공급업체는 파트너 센터에 제어판 공급업체로 [온보딩](https://docs.microsoft.com/partner-center/enroll-as-cpv)하고 이 요구 사항 구현을 즉시 시작해야 합니다. [파트너 센터: 보안 애플리케이션 모델 프레임워크](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)를 참조하세요. 제어판 공급업체는 자격 증명 대신 CSP 파트너의 동의를 수락하고 관리해야 하며 기존 CSP 파트너의 자격 증명을 모두 제거해야 합니다.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>파트너 센터 API/SDK에 대해서만 보안 애플리케이션 모델을 구현해야 하나요?

다단계 인증을 모든 사용자 계정에 적용하면 비대화형으로 실행되도록 설계된 자동화 또는 통합에 영향을 미칩니다. 파트너 보안 요구 사항에 따라 파트너 센터 API에 대한 보안 애플리케이션 모델을 사용해야 하지만 자동화 및 통합으로 두 번째 인증 요소를 해결하는 데 활용할 수 있습니다. 액세스되는 리소스는 액세스 토큰 기반 인증을 지원해야 합니다.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>PowerShell과 같은 자동화 도구를 사용하고 있습니다. 보안 애플리케이션 모델을 구현하려면 어떻게 하나요?

자동화가 비대화형으로 실행되도록 설계되고 사용자 자격 증명을 인증에 사용하는 경우 보안 애플리케이션 모델을 구현해야 합니다. 이 프레임워크 구현 방법에 대한 지침은 [Secure Application Model | Partner Center PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5)(보안 애플리케이션 모델 | 파트너 센터 PowerShell)을 참조하세요.  일부 자동화 도구는 액세스 토큰을 사용하여 인증하는 기능을 제공하지 않을 수 있습니다. 변경해야 하는 항목을 파악하는 데 도움이 필요한 경우 메시지를 [파트너 센터 보안 지침](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) 그룹에 게시하세요. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>동의 프로세스를 수행할 때 애플리케이션 관리자가 제공해야 하는 사용자 자격 증명은 무엇인가요?

최소 사용 권한이 할당된 서비스 계정을 사용하는 것이 좋습니다. 즉, 파트너 센터 API와 관련하여 영업 담당자 또는 관리 담당자 역할에 할당된 계정을 사용해야 합니다.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>애플리케이션 관리자가 동의 프로세스를 수행할 때 전역 관리 사용자 자격 증명을 제공하면 안 되는 이유는 무엇인가요?

위험을 줄이려면 최소 권한을 사용하는 것이 가장 좋습니다. 글로벌 관리자 권한이 있는 계정은 필요한 것보다 더 많은 권한을 제공하므로 사용하지 않는 것이 좋습니다.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>CSP 파트너입니다. 솔루션을 구현할 때 CPV(제어판 공급업체)가 작동하는지 여부를 어떻게 알 수 있나요?

CPV(제어판 공급업체) 솔루션을 사용하여 CSP(클라우드 솔루션 공급자) 프로그램에서 거래하는 파트너의 경우 CPV에 문의하는 것은 파트너의 책임입니다.

### <a name="who-is-a-control-panel-vendor-cpv"></a>CPV(제어판 공급업체)는 누구인가요?

제어판 공급업체는 CSP 파트너가 파트너 센터 API와 통합하는 데 사용할 앱을 개발하는 독립 소프트웨어 공급업체입니다. 제어판 공급업체는 파트너 센터 대시보드 또는 API에 직접 액세스할 수 있는 CSP 파트너가 아닙니다. 자세한 설명은 [파트너 센터: 보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) 내에서 제공됩니다.

### <a name="i-am-a-cpv-how-do-i-enroll"></a>CPV입니다. 등록하려면 어떻게 해야 하나요?

CPV(제어판 공급업체)로 등록하려면 [여기](https://docs.microsoft.com/partner-center/enroll-as-cpv)에 제공된 지침을 따르세요.

CPV는 [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com)에 연결하여 등록 링크를 받고, CPV와 비즈니스 관계가 있거나 해당 비즈니스에 대해 알고 있는 Microsoft 직원 스폰서를 제공해야 합니다. 예를 들어 PDM(파트너 개발 관리자)이 있습니다.

파트너 센터에 등록하고 애플리케이션을 등록하면 파트너 센터 API에 액세스할 수 있습니다. 새 CPV인 경우 파트너 센터 알림을 통해 샌드박스 정보를 받게 됩니다. Microsoft CPV로 등록을 완료하고 CPV 계약을 수락했으면 다음을 수행할 수 있습니다.

1. 다중 테넌트 애플리케이션을 관리(Azure Portal에 애플리케이션 추가, 파트너 센터에서 애플리케이션 등록 및 등록 취소)합니다. 참고: CPV는 파트너 센터 API에 대한 권한을 얻으려면 파트너 센터에 애플리케이션을 등록해야 합니다. Azure Portal에 애플리케이션을 추가하는 것만으로는 파트너 센터 API에 대한 권한이 CPV 애플리케이션에 부여되지 않습니다.
2. CPV 프로필을 보고 관리합니다.
3. CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다. CPV는 글로벌 관리자 역할만 보유할 수 있습니다.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>파트너 센터 SDK를 사용하고 있습니다. SDK에서 보안 애플리케이션 모델을 자동으로 채택하나요?

아니요, [보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)에서 제공하는 지침을 따라야 합니다.

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>MFA를 사용하도록 설정되지 않은 계정을 사용하여 보안 애플리케이션 모델에 대한 새로 고침 토큰을 생성할 수 있나요?

예, MFA가 적용되지 않은 계정을 사용하여 새로 고침 토큰을 생성할 수 있습니다. 그러나 MFA를 사용하지 않는 계정으로 생성된 토큰은 MFA에 대한 요구 사항으로 인해 리소스에 액세스할 수 없으므로 이렇게 해서는 안 됩니다.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA를 사용하는 경우 애플리케이션에서 액세스 토큰을 가져오려면 어떻게 해야 하나요?

새 보안 요구 사항을 준수하면서 이 작업을 수행하는 방법에 대한 정보를 제공하는 [Secure Application Model guide](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)(보안 애플리케이션 모델 가이드)를 따라야 합니다. .NET 샘플 코드는 [여기](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)에서 확인하고 Java 샘플 코드는 [여기](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)에서 확인할 수 있습니다.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV로서 CPV 테넌트 또는 CSP 파트너의 테넌트에 Azure AD 애플리케이션을 만들어야 하나요?

CPV는 CPV로서 등록과 연관된 테넌트에 Azure Active Directory 애플리케이션을 만들어야 합니다.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>앱 전용 인증을 사용하고 있는 CSP입니다. 변경해야 하나요?

사용자 자격 증명을 사용하여 액세스 토큰을 요청하지 않으므로 앱 전용 인증에는 영향을 주지 않습니다. 사용자 자격 증명이 공유되고 있는 경우 CPV(제어판 공급업체)는 [Secure Application Model framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)(보안 애플리케이션 모델 프레임워크)를 채택하고 보유하고 있는 기존 파트너 자격 증명을 모두 제거해야 합니다.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV는 앱 전용 인증 스타일을 활용하여 액세스 토큰을 받을 수 있나요?

아니요, 제어판 공급업체 파트너는 앱 전용 인증 스타일을 활용하여 파트너 대신 액세스 토큰을 요청할 수 없습니다. 보안 애플리케이션 모델을 구현하여 앱 + 사용자 인증 스타일을 활용해야 합니다.

## <a name="technical-enforcement"></a>기술 적용

### <a name="what-is-the-activation-of-security-safeguards"></a>보안 보호 기능의 활성화는 무엇인가요?

CSP(클라우드 솔루션 공급자) 프로그램, CPV(제어판 공급업체) 및 관리자에 참여하는 모든 파트너는 규정을 준수하기 위한 필수 보안 요구 사항을 구현해야 합니다.

Microsoft는 추가 보호 기능을 제공하기 위해 보안 보호 기능의 활성화를 시작했습니다. 그러면 파트너가 MFA(다단계 인증) 확인을 위임하여 무단 액세스를 방지함으로써 테넌트와 고객의 보안을 유지할 수 있습니다.  

모든 파트너 테넌트에 대한 AOBO(관리자 위임) 기능의 활성화를 성공적으로 완료했습니다. 2020년 2분기를 목표로 하여 파트너와 고객을 보호하기 위해 CSP에서 파트너 센터 트랜잭션에 대한 활성화를 시작하여 파트너가 비즈니스와 고객을 ID 도용 관련 인시던트로부터 보호할 수 있도록 지원합니다.

자세한 내용은 [파트너 테넌트에 대한 MFA(Multi-Factor Authentication) 위임](partner-security-requirements-mandating-mfa.md) 페이지를 참조하세요.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>타사 MFA 솔루션을 사용 중인데 차단되었습니다. 어떻게 해야 하나요?

리소스에 액세스하는 계정에 다단계 인증이 필요한지 확인하기 위해 [인증 방법 참조](https://tools.ietf.org/html/rfc8176) 클레임을 확인하여 MFA가 나열되어 있는지 확인합니다. 일부 타사 솔루션은 이 클레임을 발급하거나 MFA 값을 포함하고 있지 않습니다. 클레임이 없거나 MFA 값이 나열되지 않은 경우 인증된 계정에 다단계 인증이 필요한지 확인할 수 있는 방법이 없습니다. 타사 솔루션의 공급업체와 협력하여 솔루션에서 인증 방법 참조 클레임을 발급하는 데 필요한 작업을 확인해야 합니다.

타사 솔루션에서 예상 클레임을 발급하는지 확실하지 않은 경우 [파트너 보안 요구 사항 테스트](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0)를 참조하세요.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>AOBO를 사용하여 고객을 지원하지 못하게 MFA가 차단하고 있습니다. 어떻게 해야 하나요?

파트너 보안 요구 사항을 충족하기 위한 기술을 적용할 때 인증된 계정에 다단계 인증이 필요한지 확인하는 작업이 수행됩니다. 계정이 없으면 로그인 페이지로 리디렉션되고 다시 인증하라는 메시지가 표시됩니다. 이 [파트너 테넌트에 대한 MFA(Multi-Factor Authentication) 위임](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) 설명서의 자세한 환경과 지침을 확인합니다. 도메인이 페더레이션되지 않은 시나리오의 경우 성공적으로 인증되면 다단계 인증을 설정하라는 메시지가 표시됩니다. 이 작업이 완료되면 AOBO를 사용하여 고객을 관리할 수 있습니다. 도메인이 페더레이션된 시나리오의 경우 계정에 다단계 인증에 대한 문제가 있는지 확인해야 합니다.

## <a name="security-defaults-transition"></a>보안 기본값 전환

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>기준 정책에서 보안 기본값 또는 기타 MFA 솔루션으로 전환하려면 어떻게 해야 하나요?

Azure AD(Azure Active Directory) ["기준" 정책이 제거되고 "보안 기본값"으로 바뀝니다](https://docs.microsoft.com/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults). 이는 사용자와 고객에 대한 더 포괄적인 보호 정책 세트입니다. [보안 기본값](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)은 조직을 ID 도용 관련 보안 공격으로부터 보호하는 데 도움이 됩니다.

기준 정책에서 보안 기본값 정책 또는 [다른 MFA 구현 옵션](partner-security-requirements.md#actions-that-you-need-to-take)으로 전환하지 않은 경우 기본 정책 사용 중지로 인해 MFA(다단계 인증) 구현이 제거됩니다. MFA로 보호되는 작업을 수행하는 파트너 테넌트의 모든 사용자는 MFA 확인을 완료하도록 요청받습니다. [여기서](partner-security-requirements-mandating-mfa.md) 자세한 지침을 검토하세요.
규정을 준수하고 중단을 최소화하려면 다음 작업 중 하나를 수행합니다.

- 보안 기본값으로 전환
    - 보안 기본값 정책은 파트너가 MFA를 구현하는 데 선택할 수 있는 옵션 중 하나입니다. 이는 추가 비용 없이 사용 가능한 기본 보안 수준을 제공합니다.
    - Azure AD를 사용하여 조직에서 MFA를 사용하도록 설정하는 방법에 대해 알아보고, [보안 기본값 주요 고려 사항](partner-security-requirements.md#security-defaults)을 검토합니다.
    - 비즈니스 요구 사항을 충족하는 경우 보안 기본값 정책을 사용하도록 설정합니다.
- 조건부 액세스로 전환
    - 보안 기본 정책이 요구 사항을 충족하지 않는 경우 조건부 액세스를 사용하도록 설정합니다. 자세한 내용은 Azure AD 조건부 액세스 설명서를 검토하세요.

## <a name="key-resources"></a>주요 리소스

### <a name="how-to-get-started"></a>시작하는 방법

- [파트너 보안 요구 사항: 단계별 가이드](https://docs.microsoft.com/partner-center/partner-security-requirements)를 참조합니다.
- 질문과 피드백을 이 [Partner Center Security Guidance Group](https://aka.ms/MPCSecurityGuidance)(파트너 센터 보안 지침 그룹)으로 보냅니다.
- 예정된 파트너 업무 시간 및 웨비나에 참여합니다. [여기서 자세한 일정 및 리소스를 확인](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)하세요.

### <a name="resources-for-adopting-secure-application-model"></a>보안 애플리케이션 모델 채택에 대한 리소스

- [보안 애플리케이션 모델 개요](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [파트너 센터: 보안 애플리케이션 모델 가이드](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP 프로그램의 파트너: 보안 애플리케이션 모델을 활성화하는 .NET 샘플 코드](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP 프로그램의 파트너: 보안 애플리케이션 모델을 활성화하는 Java 샘플 코드](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [파트너 센터 인증 문서](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [파트너 센터 PowerShell MFA(Multi-Factor Authentication) 문서](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>지원

### <a name="where-can-i-get-support"></a>어디에서 지원을 받을 수 있나요?

보안 요구 사항을 충족하기 위한 지원 리소스를 받으려면 ASfP(파트너에 대한 고급 지원)인 경우에는 서비스 계정 관리자에게 문의하고, PSfP(파트너에 대한 프리미어 지원) 계약인 경우에는 서비스 계정 관리자 및 기술 담당 관리자에게 문의하세요.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>보안 애플리케이션 모델 프레임워크를 채택하는 데 도움이 되는 기술 정보 및 지원을 받으려면 어떻게 해야 하나요?

Azure Active Directory에 대한 기술 제품 지원 옵션은 MPN 혜택을 통해 사용할 수 있습니다. 활성 ASfP 또는 PSfP 구독에 대한 액세스 권한이 있는 파트너는 연관된 계정 관리자(SAM/TAM)와 협력하여 사용 가능한 옵션을 가장 잘 파악할 수 있습니다.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>파트너 센터에 대한 액세스 권한이 손실된 경우 지원 담당자에게 어떻게 연락해야 하나요?

[Microsoft 파트너 지원](https://partner.microsoft.com/support)으로 이동한 다음, **모든 지원 옵션 표시**를 선택합니다. 그러면 Microsoft 파트너 지원에 연락할 수 있는 옵션이 표시될 것입니다. 여기에는 지원을 요청하는 전화 번호 및 고객 지원 팀과 채팅하는 옵션이 포함됩니다. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>일반적인 기술 문제에 대한 자세한 내용은 어디에서 확인할 수 있나요?

일반적인 기술 문제에 대한 정보는 [여기](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)에서 확인할 수 있습니다.
