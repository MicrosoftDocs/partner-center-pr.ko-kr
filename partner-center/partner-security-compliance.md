---
title: 파트너 보안 요구 사항 상태
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 클라우드 솔루션 공급자 프로그램에서 관리자, 제어판 공급업체 및 파트너의 보안을 강화하는 새로운 필수 요구 사항에 대해 알아보세요.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 79fd61827f64a060da2b1ecd8f7eeceedb2fcdc5
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220201"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>파트너 보안 요구 사항 상태 - 답변을 받고 현재 상태에 대한 보고서 확인

**적용 대상**

- 클라우드 솔루션 공급자 프로그램의 모든 파트너
  - 직접 청구
  - 간접 공급자
  - 간접 재판매인
- 모든 제어판 공급업체
- 모든 관리자

**적절한 사용자**
- 사용하도록 설정된 모든 사용자(게스트 사용자 포함)

개인 정보 보호 및 보안 강화는 최우선 순위입니다. 최선의 방어는 예방이며, 가장 약한 링크를 강화해야 한다는 것을 알고 있습니다. 따라서 에코시스템의 모든 사람이 조치를 취하고, 적절한 보안 기능을 마련해야 합니다. Microsoft에서는 파트너와 고객을 보호하기 위해 클라우드 솔루션 공급자 프로그램에 참여하는 관리자, 제어판 공급업체 및 파트너에 대한 일련의 필수 보안 요구 사항을 도입하고 있습니다.

2019년 8월 1일부터 모든 파트너는 서비스 계정을 비롯한 모든 사용자의 파트너 테넌트에 다단계 인증을 적용해야 합니다. 새로운 보안 정책에 대한 자세한 내용은 [파트너 보안 요구 사항](partner-security-requirements.md)을 참조하세요.

각 사용자가 인증할 때마다 MFA가 필요한지 확인하려고 합니다. 이 환경은 다음 방법 중 하나를 통해 수행할 수 있습니다.

- Azure AD Premium을 구현하여 MFA가 각 사용자에게 적용되는지 확인
- [Azure AD 보안 기본값](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)을 구현하는지 확인
- 타사 솔루션을 구현하여 MFA가 각 사용자에게 적용되는지 확인

## <a name="partner-security-requirements-status"></a>파트너 보안 요구 사항 상태

이 보고서는 보안이 약한 위치를 파악하는 방법을 제공하여 보안 요구 사항 상태를 확인하는 데 도움이 됩니다. 추적이 정기적으로 업데이트됩니다.

>[!NOTE]
>파트너 보안 요구 사항 상태 보고서는 파트너 센터에서만 지원됩니다. Microsoft Cloud for US Government 또는 Microsoft 클라우드 독일에서는 사용할 수 없습니다. 소버린 클라우드(21Vianet, 미국 정부 및 독일)를 통해 거래하는 모든 파트너는 이러한 새 보안 요구 사항을 즉시 채택할 것을 강력하게 권장합니다. 그러나 이러한 파트너는 2019년 8월 1일부터 적용되는 새로운 보안 요구 사항을 충족할 필요가 없습니다. Microsoft에서는 나중에 소버린 클라우드에 대한 이러한 보안 요구 사항의 적용과 관련된 추가 세부 정보를 제공할 예정입니다.

## <a name="multi-factor-authentication-mfa-report"></a>"MFA(다단계 인증)" 보고서

파트너 센터 MFA 보고서는 CSP 테넌트의 MFA 구성 및 파트너 센터 활동을 기반으로 두 가지 유형의 메트릭을 제공하여 파트너 MFA 구현에 대한 인사이트를 제공합니다. 

### <a name="mfa-configuration-on-a-csp-tenant"></a>CSP 테넌트의 MFA 구성

이 메트릭은 매일 캡처하고 보고한 CSP 테넌트의 MFA 구성과 관련이 있습니다. [MFA 옵션](https://aka.ms/partner-mfa-get-started)을 사용하여 MFA를 적용한 사용자 계정의 비율을 측정합니다. 예:

- Contoso는 테넌트에 110개의 사용자 계정이 있는 CSP 파트너이며, 해당 사용자 계정 중 10개는 사용하지 않도록 설정되어 있습니다. 
- 나머지 100개의 사용자 계정 중 90개는 제공된 [MFA 옵션](https://aka.ms/partner-mfa-get-started)을 사용하여 MFA가 적용됩니다. 따라서 메트릭은 90%를 표시합니다. 

### <a name="partner-center-activities-with-mfa"></a>MFA를 통한 파트너 센터 활동

직원이 파트너 센터에 로그인하여 작업하거나 API를 통해 파트너 센터에서 데이터를 가져오거나 전송할 때마다 보안 상태가 검사 및 추적됩니다. 또한 보안 상태 추적에는 파트너의 애플리케이션과 제어판 공급업체 애플리케이션이 포함됩니다. 이전 7일의 상태가 표시됩니다.

#### <a name="mfa-verification-completed-by-users"></a>사용자가 완료한 MFA 확인

이 메트릭은 파트너 센터 대시보드 내의 활동과 관련이 있습니다. MFA 확인을 완료한 사용자가 수행한 작업의 비율을 측정합니다. 예:

- Contoso는 두 명의 관리 에이전트 Jane과 John이 있는 CSP 파트너입니다.
- 첫 번째 날에 Jane이 MFA 확인 없이 파트너 센터 대시보드에 로그인하여 3가지 작업을 수행했습니다.
- 두 번째 날에 John이 MFA 확인 없이 파트너 센터 대시보드에 로그인하여 5가지 작업을 수행했습니다.
- 세 번째 날에 Jane이 MFA 확인을 통해 파트너 센터 대시보드에 로그인하여 2가지 작업을 수행했습니다.
- 나머지 4일 동안은 두 에이전트가 어떤 작업도 수행하지 않았습니다.
- MFA 확인을 사용하는 사용자가 7일 동안 수행된 10가지 작업 중 두 가지를 수행했습니다. 따라서 메트릭은 20%를 표시합니다.

**MFA 없이 포털 요청** 파일을 사용하여 MFA 확인 없이 파트너 센터 대시보드에 로그인한 사용자 및 보고 기간 동안 마지막으로 방문한 시간을 파악합니다.

#### <a name="appuser-authentication"></a>앱+사용자 인증

이 메트릭은 앱+사용자 인증을 사용하여 작성된 파트너 센터 API 사용 요청과 관련이 있습니다. 이 메트릭은 MFA 클레임이 포함된 액세스 토큰을 사용하여 작성된 API 요청 비율을 측정합니다. 예:

- Fabrikam은 CSP 파트너이며 앱+사용자 인증과 앱 전용 인증 방법을 혼합해서 사용하는 CSP 애플리케이션을 보유하고 있습니다.
- 첫 번째 날에 애플리케이션에서 API 요청을 3개 만들었고, 이 요청은 MFA 확인 없이 앱+사용자 인증 방법을 통해 얻은 액세스 토큰을 통해 지원됩니다.
- 두 번째 날에 애플리케이션에서 5개의 API 요청을 수행했으며, 이러한 요청은 앱 전용 인증을 사용하여 얻은 액세스 토큰을 통해 지원되었습니다.
- 세 번째 날에 애플리케이션에서 2개의 API 요청을 수행했으며, 이러한 요청은 MFA 확인을 사용하는 앱+사용자 인증 방법을 사용하여 얻은 액세스 토큰을 통해 지원되었습니다.
- 나머지 4일 동안은 두 에이전트가 어떤 작업도 수행하지 않았습니다.
- 두 번째 날에 앱 전용 인증을 통해 얻은 액세스 토큰으로 지원된 5개의 API 요청은 사용자 자격 증명을 사용하지 않으므로 메트릭에서 생략됩니다. 나머지 5개 작업 중 2개는 MFA 확인으로 얻은 액세스 토큰을 통해 지원됩니다. 따라서 메트릭은 40%를 표시합니다.

이 메트릭에서 100%가 아닌 앱+사용자 활동의 결과를 이해하려면 다음 파일을 사용합니다.

- **API 요청 요약** - 애플리케이션별 전체 MFA 상태를 파악할 수 있습니다.
- **모든 API 요청** - 테넌트 사용자가 수행한 각 API 요청의 세부 정보를 파악할 수 있습니다. 더 효율적인 다운로드 환경을 위해 결과가 최대 10,000개의 최신 요청으로 제한됩니다.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>MFA 보고서의 메트릭이 100%가 아닌 경우 어떻게 해야 하나요?

MFA를 구현한 파트너의 경우 파트너 센터 MFA 보고서의 메트릭이 100%가 아닐 수 있습니다. 이유를 이해하려면 몇 가지 요소를 고려해야 합니다.

> [!NOTE]
> 파트너 테넌트의 ID 관리 및 MFA 구현에 익숙한 조직 내 직원과 협력해야 합니다.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>파트너 테넌트에 대한 MFA를 구현했습니까?

구현하지 않은 경우 먼저 파트너 테넌트에 대한 MFA를 구현해야 합니다. MFA를 구현하는 방법에 대한 자세한 내용은 [파트너 보안 요구 사항](partner-security-requirements.md) 문서를 참조하세요.

### <a name="have-you-only-recently-completed-mfa-implementation"></a>최근에 MFA 구현을 완료했습니까?

메트릭은 매일 계산되며, 지난 7일 동안 수행된 작업이 계산에 반영됩니다. 파트너 테넌트에 대한 MFA 구현을 최근에 완료한 경우 메트릭은 100%가 아닐 수 있습니다.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>일부 사용자 계정이 MFA 구현에서 제외되었습니까?

현재 MFA 구현에 모든 사용자 계정이 포함되는지 아니면 일부만 포함되는지 확인하세요. 어떤 MFA 솔루션은 정책 기반이며 사용자 제외를 지원하고, 어떤 솔루션은 사용자마다 명시적으로 MFA를 사용하도록 요구할 수 있습니다. 현재 MFA 구현에서 사용자를 제외하지 않았는지 확인하세요. 제외된 후 CSP 관련 활동을 수행하기 위해 파트너 센터에 로그인하는 사용자 계정 때문에 메트릭이 100%가 아닐 수 있습니다.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>MFA는 특정 조건이 충족되는 경우에만 필요한가요?

현재 구현이 특정 조건에서만 MFA를 적용하는지 여부를 파악합니다. 일부 MFA 솔루션은 특정 조건이 충족될 때만 MFA를 적용하도록 유연성을 제공합니다. 사용자가 알 수 없는 디바이스 또는 알 수 없는 위치에서 액세스하는 경우를 예로 들 수 있습니다. MFA를 사용하도록 설정되었지만 파트너 센터에 액세스할 때 꼭 MFA 확인을 완료하지 않아도 되는 사용자 때문에 메트릭이 100%가 아닐 수 있습니다.

>[!NOTE]
>Azure AD 보안 기본값을 사용하여 MFA를 구현한 파트너의 경우, 관리 사용자 계정이 아니면 위험에 따라 다단계 인증이 적용됩니다. 위험한 로그인을 시도하는 경우에만 MFA가 적용된다는 메시지가 표시됩니다(예: 다른 위치에서 로그인하는 경우). 또한 사용자는 최대 14일 동안 MFA에 등록할 수 있습니다. MFA 등록을 완료하지 않은 사용자는 14일 동안 MFA 확인을 요청하는 문제가 발생하지 않습니다. 따라서 Azure AD 보안 기본값을 사용하여 MFA를 구현한 파트너의 경우 메트릭이 100%가 아닐 수 있습니다.

### <a name="are-you-using-third-party-mfa-solution"></a>타사 MFA 솔루션을 사용하고 있나요?

타사 MFA 솔루션을 사용하는 경우 이를 Azure AD와 통합하는 방법을 확인합니다. 일반적으로 페더레이션 및 사용자 지정 컨트롤을 포함한 두 가지 방법이 있습니다.

* **ID 페더레이션** – Azure AD가 인증 요청을 수신하면 Azure AD는 인증을 위해 사용자를 페더레이션된 ID 공급자로 리디렉션합니다. 성공적으로 인증되면 페더레이션된 ID 공급자는 SAML 토큰을 사용하여 사용자를 Azure AD로 다시 리디렉션합니다. 사용자가 페더레이션된 ID 공급자에 인증할 때 MFA 확인을 완료한 것으로 Azure AD에서 인식하려면 SAML 토큰에 *authenticationmethodsreferences* 클레임(값은 *multipleauthn*)이 포함되어야 합니다. 페더레이션된 ID 공급자가 이러한 클레임 발급을 지원하는지 확인하세요. 지원한다면 페더레이션된 ID 공급자가 이러한 클레임 발급을 지원하도록 구성되었는지 확인하세요. 클레임이 없는 경우 Azure AD(및 이에 따라 파트너 센터)에서는 사용자가 MFA 확인을 완료했고 클레임이 누락되어 메트릭이 100%가 되지 않을 수 있음을 인식할 수 없습니다.

* **사용자 지정 컨트롤** – Azure AD 사용자 지정 컨트롤을 사용하여 사용자가 타사 MFA 솔루션을 통해 MFA 확인을 완료했는지 여부를 확인할 수 없습니다. 따라서 사용자 지정 컨트롤을 통해 MFA 확인을 완료한 사용자는 항상 Azure AD에(그리고 파트너 센터에) MFA 확인을 완료하지 않는 것으로 나타납니다. 가능하다면 Azure AD와 통합할 때 사용자 지정 컨트롤과 반대로 ID 페더레이션을 사용하도록 전환하는 것이 좋습니다.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>MFA를 사용하지 않고 파트너 센터에 로그인한 사용자 식별

MFA 확인 없이 파트너 센터에 로그인한 사용자를 파악하여 현재 MFA 구현과 대조한다면 도움이 될 수 있습니다. [Azure AD 로그인 보고서](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)를 사용하여 사용자가 MFA 확인을 완료했는지 확인할 수 있습니다. Azure AD 로그인 보고서는 현재 Azure AD Premium 또는 Azure AD Premium이 포함된 O365 SKU(예: EMS)를 구독한 파트너만 사용할 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [파트너 센터 보안 지침 그룹 커뮤니티](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [파트너 센터 보안 요구 사항](partner-security-requirements.md)
- [파트너 센터 보안 요구 사항 FAQ](partner-security-requirements-faq.md)
