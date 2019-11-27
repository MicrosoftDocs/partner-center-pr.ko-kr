---
title: CSP 파트너 | 파트너 센터용 Cloudyn의 Azure 비용 관리
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn 웹 앱을 등록 하 고 파트너 센터에서 비밀 키를 사용 하는 방법을 알아보고, 앱을 사용 하 여 고객 Azure 사용량 및 비용을 추적할 수 있습니다.
author: Janet
ms.author: janet
Keywords: Azure cost management 앱, 비용 관리, 웹 앱
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253303"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Azure CSP 파트너용 Azure 비용 관리 앱  

**적용 대상**

- 파트너 센터
- 클라우드 솔루션 공급자 프로그램 파트너

**적절 한 역할**

- 전역 관리자
- 관리자 에이전트

[Azure Cost Management에 대 한 자세한 정보 보기](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>시작하기 전 주의 사항
Azure 비용 관리를 사용하려면 먼저 다음 요구 사항을 충족해야 합니다.

- 클라우드 솔루션 공급자 프로그램의 파트너여야 합니다.
- 파트너 센터 API 웹 앱을 만들 수 있어야 합니다.

## <a name="overview"></a>개요

Cloudyn는 고객이 얼마나 많은 Azure를 사용 하 고 있는지를 추적 하 고 관리 하는 데 사용할 수 있는 웹 앱입니다. 파트너 센터 API를 통해 사용합니다.

## <a name="register-your-web-app-in-the-partner-center"></a>파트너 센터에서 웹 앱 등록
파트너 센터에서 Azure Active Directory 웹 앱을 등록하면 파트너 센터 API에 액세스할 수 있습니다. 
1.  [전역 관리자 또는 관리자 에이전트 계정](https://partnercenter.microsoft.com/pcv/dashboard/overview)을 사용하여 [파트너 센터](create-user-accounts-and-set-permissions.md)에 로그인합니다.
2.  **파트너 센터**에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** 를 선택 합니다.
3.  **Web App** 섹션에서 **Add new web app**를 클릭합니다.
<br> **참고**: 이전에 웹 앱을 만든 경우 3단계를 건너뛸 수 있습니다.
4.  웹 앱의 **Commerce ID** GUID 및 **App ID** GUID를 복사하고 저장합니다. 30일 무료 평가판 Azure 비용 관리 앱을 사용하려면 두 ID가 모두 필요합니다.

## <a name="add-a-secret-key-to-your-app"></a>앱에 비밀 키를 추가합니다.
1. **Add key** 버튼 옆에 있는 드롭다운 목록에서 기간을 1년 또는 2년으로 선택합니다.
2. **Add key**를 클릭합니다. 
3. 비밀 키 값을 복사하고 저장합니다. 30일 무료 평가판을 사용하려면 이 키가 필요합니다.<br>
   > [!NOTE]  
   > 응용 프로그램 비밀 키는 만료 날짜가 긴 암호와 같습니다. 나중에 사용할 수 있도록 키 값을 안전한 위치에 저장하십시오.

## <a name="next-steps"></a>다음 단계
[30일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작합니다.
평가판을 시작하려면 다음 세부 정보가 필요합니다.
- 파트너 센터 로그인 자격 증명
- Commerce ID GUID
- App ID GUID
- 응용 프로그램 비밀 키 값
