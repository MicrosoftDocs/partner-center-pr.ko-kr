---
title: Csp에 대 한 Azure Cost Management Cloudyn
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn 웹 앱을 등록 하 고 파트너 센터에서 비밀 키를 사용 하는 방법을 알아보고, 앱을 사용 하 여 고객 Azure 사용량 및 비용을 추적할 수 있습니다.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435912"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>CSP 파트너를 위한 Azure cost management 앱을 사용 하 여 고객 Azure 사용량 및 비용 추적  

**적용 대상**

- 파트너 센터
- 클라우드 솔루션 공급자 프로그램 파트너

**적절한 역할**

- 글로벌 관리자
- 관리 에이전트

[Azure Cost Management에 대 한 자세한 정보 보기](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>시작하기 전에
Azure Cost Management를 사용 하려면 먼저 다음 요구 사항을 충족 해야 합니다.

- 클라우드 솔루션 공급자 프로그램의 파트너입니다.
- 파트너 센터 API 웹 앱을 만들 수 있습니다.

## <a name="overview"></a>개요

Cloudyn는 고객이 얼마나 많은 Azure를 사용 하 고 있는지를 추적 하 고 관리 하는 데 사용할 수 있는 웹 앱입니다. 파트너 센터 API를 통해 사용 합니다.

## <a name="register-your-web-app-in-the-partner-center"></a>파트너 센터에 웹 앱 등록
파트너 센터에 Azure Active Directory 웹 앱을 등록 하면 파트너 센터 API에 액세스할 수 있습니다. 
1.  [전역 관리자 또는 관리 에이전트 계정을](create-user-accounts-and-set-permissions.md)사용 하 여 [파트너 센터](https://partnercenter.microsoft.com/pcv/dashboard/overview) 에 로그인 합니다.
2.  **파트너 센터**에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** 를 선택 합니다.
3.  **웹 앱** 섹션에서 **새 웹 앱 추가**를 클릭 합니다.
<br> **참고**: 이전에 웹 앱을 만든 경우 3 단계를 건너뛸 수 있습니다.
4.  웹 앱에 대 한 **상거래 id** Guid 및 **앱 id** guid를 복사 하 고 저장 합니다. Azure cost management 앱의 30 일 무료 평가판을 사용 하려면 두 Id가 모두 필요 합니다.

## <a name="add-a-secret-key-to-your-app"></a>앱에 비밀 키 추가
1. **키 추가** 단추 옆의 드롭다운에서 기간을 1 또는 2 년으로 선택 합니다.
2. **키 추가**를 클릭 합니다. 
3. 비밀 키 값을 복사 하 고 저장 합니다. 이는 30 일 무료 평가판에 필요 합니다.<br>
   > [!NOTE]  
   > 응용 프로그램 비밀 키는 만료 날짜가 긴 암호와 같습니다. 나중에 사용 하기 위해 키 값을 안전한 위치에 저장 하세요.

## <a name="next-steps"></a>다음 단계
[30 일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작 합니다.
평가판을 시작 하려면 다음 정보가 필요 합니다.
- 파트너 센터 로그인 자격 증명
- 상거래 ID GUID
- 앱 ID GUID
- 응용 프로그램 비밀 키 값
