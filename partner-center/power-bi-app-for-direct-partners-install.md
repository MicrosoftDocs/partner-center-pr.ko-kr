---
title: Power BI에 대 한 파트너 센터 분석 설치
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 문서의 단계를 수행 하 여 Power BI에 대 한 파트너 센터 분석 앱 (CSP의 직접 파트너)을 설치 하 고 미리 봅니다.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854488"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기


**적절 한 역할**: 전역 관리자 | 사용자 관리 관리자 | 판매 에이전트 | 관리 에이전트

## <a name="before-you-begin"></a>시작하기 전에

사용 가능한 Power BI 앱의 다음 목록에서 비즈니스에 가장 적합 한 응용 프로그램을 선택 합니다.

- [직접 공급자](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [간접 공급자](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [간접 재판매인](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

파트너 센터 분석 앱 미리 보기 버전을 설치 하기 전에 다음 요구 사항을 충족 해야 합니다.

- 비즈니스에 적합 한 Power BI 앱을 선택 합니다.

- Power BI pro 라이선스가 있습니다.

- 테 넌 트에서 템플릿 앱을 설치할 수 있는 권한이 있습니다.

- Power BI에 로그인 할 수 있습니다.

- 전역 관리자, 관리 에이전트 또는 청구 관리자로 [회사의 Azure Active Directory (AZURE AD) 테 넌 트](azure-active-directory-tenants-and-partner-center.md)에 로그인 할 수 있습니다.

## <a name="to-install-the-app"></a>앱을 설치 하려면

1. 위의 섹션에서 제공 된 앱 소스 링크 (Direct Provider/간접 공급자/i a t e r/간접 재판매인)를 선택 합니다.

2. **지금 가져오기** 를 선택합니다. 

3. **계속** 을 선택 하 여 사용 약관에 동의 합니다.

4. 에 이미 계정이 있나요? **로그인** 을 선택 합니다.

5. 다음 페이지에서 Power BI 사용자 이름 및 암호를 입력 한 다음 **로그인** 을 선택 합니다.

6. 작업 영역 이름을 제공 하 여 작업 영역을 설치 합니다.

7. 앱 섹션 아래에 설치 된 템플릿 앱을 찾을 수 있습니다.

8. **앱을** 선택하고 설치된 앱을 선택합니다.

9. 새 앱 시작 화면이 열립니다.

10. 데이터에 연결하려면 **연결을** 선택합니다.

11. 파트너 센터 **Analytics에 연결** 팝업 창에서 **인증 방법이** **oAuth2로** 설정되어 있는지 확인하거나, 그렇지 않은 경우 목록에서 **oAuth2를** 선택합니다. 

> [!NOTE]  
>  이 창이 나타나려면 몇 분 정도 걸릴 수 있습니다.

12. 파트너 센터 **Analytics Connector** 페이지에서 회사의 Azure AD 테넌트의 전역 관리자, 관리 에이전트 또는 청구 관리자 자격 증명으로 **로그인한** 다음 로그인을 선택합니다.
 
13. 액세스하라는 메시지가 표시되면 **동의를** 선택합니다. 

파트너 센터 Analytics 서비스가 Power BI 연결되면 데이터가 로드되기 시작합니다. 데이터 양에 따라 최대 10분이 걸릴 수 있습니다. 

데이터 로드가 완료되면 Power BI 파트너 센터 Analytics 앱 대시보드 및 보고서를 사용할 수 있습니다.

## <a name="next-steps"></a>다음 단계

[Microsoft Power BI 파트너 센터 Analytics 앱을 사용하여 비즈니스 데이터 보기](power-bi-app-for-direct-partners-use.md)
