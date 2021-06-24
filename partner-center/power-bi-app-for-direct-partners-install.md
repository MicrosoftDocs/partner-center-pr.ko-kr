---
title: Power BI 파트너 센터 Analytics 설치
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 문서의 단계에 따라 CSP의 직접 파트너를 위해 Power BI용 파트너 센터 분석 앱 설치하고 미리 봅니다.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ff95f989ac847bd2c17558d062c86a52110b2ddf
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565046"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기


**적절한 역할**: 전역 관리자 | 사용자 관리 관리자 | 판매 에이전트 | 관리자 에이전트

## <a name="before-you-begin"></a>시작하기 전에

사용 가능한 다음 Microsoft Power BI 앱 목록에서 비즈니스와 가장 관련된 애플리케이션을 선택합니다.

- [직접 공급자](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [간접 공급자](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [간접 대리점](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

파트너 센터 Analytics 앱 미리 보기 버전을 설치하기 전에 다음 요구 사항을 충족해야 합니다.

- 비즈니스에 적합한 Power BI 앱을 선택합니다.

- Power BI pro 라이선스가 있습니다.

- 테넌트에서 템플릿 앱을 설치할 수 있는 권한이 있습니다.

- Power BI 로그인할 수 있습니다.

- [회사의 Azure AD(Azure Active Directory) 테넌트](azure-active-directory-tenants-and-partner-center.md)에 전역 관리자, 관리 에이전트 또는 청구 관리자로 로그인할 수 있습니다.

## <a name="to-install-the-app"></a>앱을 설치하려면

1. 위의 섹션에서 지정된 앱 원본 링크(직접 공급자/간접 공급자/간접 대리점)를 선택합니다.

2. **지금 가져오기** 를 선택합니다. 

3. **계속을** 선택하여 약관에 동의합니다.

4. 계정이 이미 있나요? **로그인을** 선택합니다.

5. 다음 페이지에서 Power BI 사용자 이름 및 암호를 입력한 **다음, 로그인을** 선택합니다.

6. 작업 영역 이름을 제공하여 작업 영역을 설치합니다.

7. 앱 섹션 아래에 설치된 템플릿 앱을 찾을 수 있습니다.

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
