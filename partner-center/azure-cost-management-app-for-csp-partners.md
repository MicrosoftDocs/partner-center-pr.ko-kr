---
title: CSP 파트너 | 파트너 센터용 Cloudyn의 Azure 비용 관리
ms.topic: article
ms.date: 03/15/2019
description: Cloudyn의 Azure 비용 관리를 사용하려면 파트너 센터 API에 프로비전된 액세스가 필요합니다.
author: Janet
ms.author: janet
Keywords: Azure 비용 관리 앱에 비용을 관리, 웹 앱
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 14b94e94c349fa142cb6bd37ed4ca94f7a9397b6
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134673"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Azure CSP 파트너용 Azure 비용 관리 앱  

**적용 대상**

-  파트너 센터

[Azure Cost Management에 대 한 자세한 정보](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>시작하기 전 주의 사항
Azure 비용 관리를 사용하려면 먼저 다음 요구 사항을 충족해야 합니다.

- 클라우드 솔루션 공급자 프로그램의 파트너여야 합니다.
- 파트너 센터 API 웹 앱을 만들 수 있어야 합니다.

## <a name="overview"></a>개요

Cloudyn은 추적 하 고 얼마나 고객에 게는 및 사용 하 여 Azure 사용량 비용을 관리할 수 있는 웹 앱. 파트너 센터 API를 통해 사용합니다.

## <a name="register-your-web-app-in-the-partner-center"></a>파트너 센터에서 웹 앱 등록
파트너 센터에서 Azure Active Directory 웹 앱을 등록하면 파트너 센터 API에 액세스할 수 있습니다. 
1.  [전역 관리자 또는 관리자 에이전트 계정](create-user-accounts-and-set-permissions.md)을 사용하여 [파트너 센터](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)에 로그인합니다.
2.  **파트너 센터**를 선택 **계정 설정** &gt;  **[앱 관리](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** 합니다.
3.  **Web App** 섹션에서 **Add new web app**를 클릭합니다.
<br> **참고**: 웹 앱을 이전에 만든 경우 3 단계를 건너뛸 수 있습니다.
4.  웹 앱의 **Commerce ID** GUID 및 **App ID** GUID를 복사하고 저장합니다. 30일 무료 평가판 Azure 비용 관리 앱을 사용하려면 두 ID가 모두 필요합니다.

## <a name="add-a-secret-key-to-your-app"></a>앱에 비밀 키를 추가합니다.
1. **Add key** 버튼 옆에 있는 드롭다운 목록에서 기간을 1년 또는 2년으로 선택합니다.
2. **Add key**를 클릭합니다. 
3. 비밀 키 값을 복사하고 저장합니다. 30일 무료 평가판을 사용하려면 이 키가 필요합니다.<br>
   > [!NOTE]  
   > 응용 프로그램 비밀 키 긴 만료 날짜를 사용 하 여 암호와 같습니다. 나중에 사용할 수 있도록 키 값을 안전한 위치에 저장하십시오.

## <a name="next-steps"></a>다음 단계
[30일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작합니다.
평가판을 시작하려면 다음 세부 정보가 필요합니다.
- 파트너 센터 로그인 자격 증명
- Commerce ID GUID
- App ID GUID
- 응용 프로그램 비밀 키 값
