---
title: 파트너 계정의 위치 관리
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 새 위치를 추가하는 방법 및 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925046"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>MPN 계정 위치 관리 및 새 위치 추가


**적절한 역할**

- 전역 관리자
- 계정 관리자

위치 MPN ID는 회사의 각 특정 위치를 식별합니다. 위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스와 기타 비즈니스 트랜잭션을 처리합니다. 글로벌 MPN ID는 지원 요청과 같은 비 트랜잭션 작업에 사용됩니다.

## <a name="the-following-is-a-typical-scenario"></a>다음은 일반적인 시나리오입니다.

Contoso는 영국에 PGA(파트너 글로벌 계정)를 가지고 있습니다. 이는 이 업체의 등록된 합법적인 사업이며 이 회사의 글로벌 MPN ID는 모든 비 트랜잭션 비즈니스를 관리하는 데 사용됩니다. 또한 Contoso는 영국, 프랑스 및 미국의 다른 위치에 있는 자회사 또는 사업부에 해당하는 PLA(파트너 위치 계정)를 가지고 있습니다. MPN 계정 구조에서 이러한 PLA는 고유한 위치 MPN ID로 표시됩니다. PLA는 CSP 또는 인센티브 프로그램과 같은 트랜잭션 비즈니스에 사용됩니다. 결제는 특정 위치에 연결됩니다. 

>[!NOTE]
>CSP 테넌트와 MPN 위치 ID 사이에는 일대일 관계가 있습니다.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 위치 구조":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>CSP 비즈니스에 대한 새 위치를 추가하기 위한 필수 구성 요소

새 CSP 비즈니스 계정을 추가하려면 먼저 사전 요구 사항을 충족했는지 확인합니다.

1. CSP 비즈니스를 수행하려는 국가에 위치 MPN ID가 있어야 합니다. 새 MPN 위치를 만들려면 아래의 "MPN 위치 추가"를 참조하세요.
  
1. 새 CSP 간접 재판매인 등록을 만들려면 [간접 공급자와 협력](indirect-reseller-tasks-in-partner-center.md#get-started)을 읽어보세요. 

>[!NOTE] 
 >**새** CSP 계정에 대해서는 **새** 자격 증명을 사용하여 로그인해야 합니다. 파트너 센터에서 이미 계정이 있는 것으로 인식하므로 기존 자격 증명을 사용하지 마세요.

2. Microsoft 파트너 계약에 동의하고 계정을 활성화합니다.

## <a name="add-an-mpn-location"></a>MPN 위치 추가

1. 파트너 센터에서 MPN 계정을 사용하여 로그인합니다. (MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.) MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다. 

1. **설정 아이콘** 에서 **계정 설정** 을 선택한 다음, **조직 프로필** 을 선택합니다.

2. **법무** 를 선택한 다음, **파트너** 탭에서 **비즈니스 위치** 를 선택하고 **위치 추가** 를 클릭합니다.

3. 회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다.
 
1. **위치 추가** 를 클릭합니다. 그러면 CSP 트랜잭션 및 성과급에 사용할 수 있는 새 위치에 대한 새 MPN ID가 만들어집니다.

:::image type="content" source="images/legal-biz.png" alt-text="새로운 법적 비즈니스 추가":::

> [!NOTE]
> 파트너 센터에서 추가한 위치는 제거할 수 없습니다. 올바른 MPN ID를 사용하여 로그인한 경우 파트너 센터의 왼쪽 메뉴에 **MPN** 이 표시됩니다.

## <a name="change-country-of-partner-global-account"></a>파트너 전역 계정의 국가 변경 

1. 파트너 센터에서 MPN 계정을 사용하여 로그인합니다. (MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.) MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다. 

2. **파트너** 탭에서 **비즈니스 위치** 에서 위치 목록을 확인하여 법인으로 원하는 위치가 나열되는지 확인합니다. 
 
1. 위치를 추가하려면 **위치 추가** 를 클릭하고, 플라이 아웃에서 회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다. 
 
1. **국가/지역** 드롭다운 옆에 있는 **국가 변경** 을 선택하고 단계를 따릅니다. 

:::image type="content" source="images/lbp.png" alt-text="법적 비즈니스 프로필 데이터 플라이 아웃":::

5. **저장** 을 클릭합니다.

6. MPN 전역 계정 국가는 새로운 법적 국가로 변경됩니다.
  
## <a name="next-steps"></a>다음 단계

- [확인 프로세스](verification-responses.md)에 대해 알아보세요.
