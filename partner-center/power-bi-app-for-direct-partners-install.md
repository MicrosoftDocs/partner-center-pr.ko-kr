---
title: Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기 | 파트너 센터
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 다음 단계를 수행 하 여 파트너 센터 분석 Power BI 앱 (CSP의 직접 파트너)을 설치 하 고 미리 봅니다.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: cd328ce8afed02af377a94b40fcf75125b008d1f
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004972"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기

**적용 대상**

- 파트너 센터

**적절한 역할**
-   전역 관리자
-   사용자 관리자
-   영업 에이전트
-   관리자 에이전트

## <a name="before-you-begin"></a>시작하기 전에

사용 가능한 Power BI 앱의 다음 목록에서 비즈니스에 가장 적합 한 응용 프로그램을 선택 합니다.
- [직접 파트너](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [간접 파트너](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [간접 재판매인](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

파트너 센터 분석 앱 미리 보기 버전을 설치하기 전에 다음 요구 사항을 충족하는지 확인하세요.

- 비즈니스에 적합 한 Power BI 앱을 선택 합니다.

- Microsoft Power BI Professional 또는 Microsoft Power BI Premium 중 하나에 활성 구독이 있습니다.

- Power BI에 로그인할 수 있습니다.

- 전역 관리자, 관리 에이전트 또는 청구 관리자로 [회사의 Azure Active Directory (AZURE AD) 테 넌 트](azure-active-directory-tenants-and-partner-center.md)에 로그인 할 수 있습니다.

## <a name="to-install-the-app"></a>앱을 설치하려면

1. [설치 프로세스](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)를 시작합니다.

2. **이미 계정이 있으십니까?** 아래에서 **로그인**을 선택합니다. 

3. 다음 페이지에서 Power BI 사용자 이름 및 암호를 입력한 다음 **로그인**을 선택합니다. 

4. **파트너 센터 분석에 연결** 팝업 창에서 **인증 방법이** **oAuth2** 으로 설정 되어 있는지 확인 하 고 그렇지 않은 경우 목록에서 **oAuth2** 를 선택 합니다. 

> [!NOTE]  
>  이 창이 표시되는 데 몇 분 정도 걸릴 수 있습니다.

5. **파트너 센터 분석 커넥터** 페이지에서 회사의 Azure AD 테 넌 트에 대 한 전역 관리자, 관리 에이전트 또는 청구 관리자 자격 증명을 사용 하 여 로그인 한 다음 **로그인**을 선택 합니다.
 
6. 액세스에 대한 메시지가 표시되면 **수락**을 선택합니다. 

파트너 센터 분석 서비스가 Power BI에 연결되면 데이터가 로드되기 시작합니다. 데이터의 양에 따라 이 작업에는 최대 10분이 걸릴 수 있습니다. 

데이터 로드가 완료된 후 Power BI에서 파트너 센터 분석 앱 대시보드와 보고서를 사용할 수 있습니다.

## <a name="next-steps"></a>다음 단계

[Microsoft Power BI 파트너 센터 분석 앱을 사용 하 여 비즈니스 데이터 보기](power-bi-app-for-direct-partners-use.md)
