---
title: 파트너 계정의 위치 관리
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 새 위치를 추가하는 방법 및 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/15/2020
ms.locfileid: "92100773"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>MPN 계정 위치 관리 및 새 위치 추가

**적용 대상**

- 파트너 센터

**적절한 역할**

- 글로벌 관리자
- 계정 관리자

위치 MPN ID는 회사의 각 특정 위치를 식별합니다. 위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스와 기타 비즈니스 트랜잭션을 처리합니다. 글로벌 MPN ID는 지원 요청과 같은 비 트랜잭션 작업에 사용됩니다.

## <a name="the-following-is-a-typical-scenario"></a>다음은 일반적인 시나리오입니다.

Contoso는 영국에 PGA(파트너 글로벌 계정)를 가지고 있습니다. 이는 이 업체의 등록된 합법적인 사업이며 이 회사의 글로벌 MPN ID는 모든 비 트랜잭션 비즈니스를 관리하는 데 사용됩니다. 또한 Contoso는 영국, 프랑스 및 미국의 다른 위치에 있는 자회사 또는 사업부에 해당하는 PLA(파트너 위치 계정)를 가지고 있습니다. MPN 계정 구조에서 이러한 PLA는 고유한 위치 MPN ID로 표시됩니다. PLA는 CSP 또는 인센티브 프로그램과 같은 트랜잭션 비즈니스에 사용됩니다. 결제는 특정 위치에 연결됩니다. 

>[!NOTE]
>CSP 테넌트와 MPN 위치 ID 사이에는 일대일 관계가 있습니다.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 위치 구조":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>새 CSP 비즈니스 위치를 추가하기 위한 필수 구성 요소

새 CSP 비즈니스 위치를 추가하려면 다음과 같은 몇 가지 필수 구성 요소가 있습니다.

1. 비즈니스를 수행하려는 국가에 위치 MPN ID가 있어야 합니다.

1. 아직 CSP에 등록되지 않은 [비즈니스 지역](regional-authorization-overview.md)에 새 Azure AD 테넌트가 필요합니다. 이 테넌트는 CSP에 등록할 때 만듭니다.
 
3. 새 AAD 테넌트를 사용하여 해당 지역의 CSP 프로그램에 등록합니다.
법적 회사 이름, 주소, 기본 연락처 세부 정보를 포함한 법적 회사 세부 정보를 제공합니다. 이 계정에는 확인 프로세스가 수행되므로 유효한 정보를 추가해야 합니다.

>[!NOTE] 
 >**새** Azure AD 테넌트에 대한 **새** 자격 증명을 사용하여 로그인해야 합니다. 파트너 센터에서 이미 계정이 있는 것으로 인식하므로 기존 자격 증명을 사용하지 마세요.

4. Microsoft 파트너 계약에 동의하고 계정을 활성화합니다.

## <a name="add-an-mpn-location"></a>MPN 위치 추가

1. 파트너 센터에서 MPN 계정을 사용하여 로그인합니다. MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다. 

1. **설정 아이콘**에서 **파트너 설정**을 선택합니다.

2. **위치**를 선택합니다.

3. **위치 추가**를 선택하고 회사에 추가하려는 위치의 주소 정보와 위치의 기본 연락처를 입력합니다.

> [!NOTE]
> 파트너 센터에서 추가한 위치는 제거할 수 없습니다. 올바른 MPN ID를 사용하여 로그인한 경우 파트너 센터의 왼쪽 메뉴에 **MPN**이 표시됩니다.

## <a name="change-global-partner-account-location"></a>글로벌 파트너 계정 위치 변경

1. **[위치](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** 페이지에서 위치 목록을 검사하여 법인으로 사용할 위치가 나열되는지 확인합니다. 그렇지 않은 경우 추가합니다.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN 위치 구조":::

2. **파트너 프로필**, **법적 비즈니스 프로필 업데이트**를 차례로 선택합니다.

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN 위치 구조":::

3. 지역 및 법인을 선택하고 **제출**을 선택합니다.

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN 위치 구조":::

## <a name="next-steps"></a>다음 단계

- [확인 프로세스](verification-responses.md)에 대해 알아보세요.
