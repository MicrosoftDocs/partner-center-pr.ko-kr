---
title: 파트너 계정의 위치 관리
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 새 위치를 추가하는 방법 및 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276827"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>MPN 계정 위치 관리 및 새 위치 추가(삭제)


**적절한 역할**: 전역 관리자 | 계정 관리자

위치 MPN ID는 회사의 각 특정 위치를 식별합니다. 위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스와 기타 비즈니스 트랜잭션을 처리합니다. 글로벌 MPN ID는 지원 요청과 같은 비 트랜잭션 작업에 사용됩니다.

## <a name="the-following-scenario-is-typical"></a>다음 시나리오가 일반적입니다.

Contoso는 영국에 PGA(파트너 글로벌 계정)를 가지고 있습니다. PGA는 등록된 합법적인 사업이며 이 회사의 글로벌 MPN ID는 모든 비 트랜잭션 비즈니스를 관리하는 데 사용됩니다. 또한 Contoso는 영국, 프랑스 및 미국의 다른 위치에 있는 자회사 또는 사업부에 해당하는 PLA(파트너 위치 계정)를 가지고 있습니다. MPN 계정 구조에서 이러한 PLA는 고유한 위치 MPN ID로 표시됩니다. PLA는 CSP 또는 인센티브 프로그램과 같은 트랜잭션 비즈니스에 사용됩니다. 결제는 특정 위치에 연결됩니다. 

>[!NOTE]
>CSP 테넌트와 MPN 위치 ID 사이에는 일대일 관계가 있습니다.

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 위치 구조.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>CSP 비즈니스에 대한 새 위치를 추가하기 위한 필수 구성 요소

새 CSP 비즈니스 계정을 추가하려면 먼저 사전 요구 사항을 충족했는지 확인합니다.

1. CSP 비즈니스를 수행하려는 국가에 위치 MPN ID가 있어야 합니다. 새 MPN 위치를 만들려면 아래의 "MPN 위치 추가"를 참조하세요.
  
1. 새 CSP 간접 재판매인 등록을 만들려면 [간접 공급자와 협력](indirect-reseller-tasks-in-partner-center.md#get-started)을 읽어보세요. 

>[!NOTE] 
 >**새** CSP 계정에 대해서는 **새** 자격 증명을 사용하여 로그인해야 합니다. 파트너 센터에서 이미 계정이 있는 것으로 인식하므로 기존 자격 증명을 사용하지 마세요.

2. Microsoft 파트너 계약에 동의하고 계정을 활성화합니다.

1. 직접 청구 파트너로 등록하려면 [직접 청구 파트너 요구 사항](direct-partner-new-requirements.md)을 참조하세요.

## <a name="view-and-update-your-mpn-locations"></a>MPN 위치 보기 및 업데이트

1. MPN 계정 자격 증명으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home)에 로그인합니다. (MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.) 
 
1. **설정** 아이콘에서 **계정 설정** 을 선택한 다음, **조직 프로필**, **법무** 를 선택합니다. 

1. **파트너** 탭에서, PMC에서 마이그레이션된 위치를 수정하라는 배너 오류 메시지가 없는지 확인합니다.  PMC에서 위치가 올바르게 설정되지 않았거나 PC로 아직 전환되지 않은 경우 해당 위치를 업데이트해야 합니다.

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap은 위치를 업데이트하는 방법을 보여줍니다.":::
 
4.  **PMC 위치 검토** 화면에서 **업데이트** 를 선택합니다.
다음 필드를 업데이트합니다.

- **이름 필드**: 회사 위치 이름이 올바른지 확인합니다. 중복 오류가 표시되는 경우, 예를 들어 Contoso에서 Contoso, Inc.로 변경해 보세요.

- **법인 필드**: 위치가 연결된 법인을 선택했는지 확인합니다.

- **주소란 1 및 2** : 주소가 정확한지 확인합니다.

- **시 및 주/도 필드**: 시와 주/도의 조합이 올바른지 확인합니다. 주/도를 선택하는 드롭다운 메뉴가 표시되는 국가가 있고 필드를 수동으로 입력해야 하는 국가도 있습니다.

- **우편 번호 필드**: 우편 번호 필드가 표시된 국가, 지역, 시 또는 주소와 일치하는지 확인합니다.

- **기본 연락처 정보 필드**: 이름과 성 필드가 채워져 있고 표시된 이메일 주소가 개인 이메일이 아닌 업무용 이메일 주소(예: @outlook.com, @live.com 등)인지 확인합니다.

- **전화 번호 필드**: 전화 번호에 특수 문자, 공백 또는 국가 코드가 포함되어 있지 않은지 확인합니다. 전화 번호 필드에 입력할 수 있는 값은 항상 최대 10자입니다.

5. 오류 메시지가 없는 경우 **설정** 에서 **계정 설정**, **조직 프로필**, **식별자** 를 선택합니다.

6. 이 CSP 계정의 국가와 일치하는 "위치" 유형의 MPN ID를 찾아 연결을 완료하는 데 사용합니다.

7. 사용하려는 CSP 계정과 일치하는 위치 MPN ID를 찾을 수 없는 경우 새 위치를 추가하여 새 MPN ID를 만들 수 있습니다. 아래 **MPN 위치 추가** 를 참조하세요.

## <a name="add-an-mpn-location"></a>MPN 위치 추가

1. 파트너 센터에서 MPN 계정을 사용하여 로그인합니다. (MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.) MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다. 

1. **설정 아이콘** 에서 **계정 설정** 을 선택한 다음, **조직 프로필** 을 선택합니다.

2. **법무** 를 선택한 다음, **파트너** 탭에서 **비즈니스 위치** 를 선택하고 **위치 추가** 를 선택합니다.

3. 회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다.
 
1. **위치 추가** 를 선택합니다. 그러면 CSP 트랜잭션 및 성과급에 사용할 수 있는 새 위치에 대한 새 MPN ID가 만들어집니다.

:::image type="content" source="images/legal-biz.png" alt-text="새로운 법적 비즈니스 추가.":::

> [!NOTE]
> 파트너 센터에서 추가한 위치는 제거할 수 없습니다. 올바른 MPN ID를 사용하여 로그인한 경우 파트너 센터의 왼쪽 메뉴에 **MPN** 이 표시됩니다.

## <a name="add-the-registration-number-id"></a>등록 번호 ID 추가

간접 공급자, 직접 청구 파트너 또는 간접 재판매인이고 다음 국가의 신규 또는 기존 고객과 사업을 수행하는 경우 비즈니스 등록 ID 번호를 제공해야 합니다. 비즈니스를 수행하는 국가가 아래에 나열되지 않은 경우 등록 ID는 선택 사항입니다.

- 아르메니아 
- 아제르바이잔 
- 벨라루스 
- 브라질 
- 헝가리 
- 인도 
- 이라크 
- 카자흐스탄 
- 키르기스스탄 
- 몰도바 
- 미얀마 
- 폴란드 
- 러시아 
- 사우디아라비아 
- 남아프리카 공화국 
- 남수단  
- 타지키스탄 
- 태국
- 터키 
- 우크라이나 
- 아랍에미리트연합국 
- 우즈베키스탄 
- 베네수엘라
- 베트남 


자세한 내용은 [등록 ID 번호 정보](reg-number-id.md)를 참조하세요.

## <a name="delete-a-location"></a>위치 삭제

계정에서 위치를 삭제하려면 [파트너 지원](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)에 문의해야 합니다. 이 작업이 미치는 영향을 이해했는지 확인합니다. 삭제된 위치는 검색할 수 없으며 특정 MPN ID에 연결된 모든 항목은 더 이상 인식되지 않거나 회사에 대해 활성화되지 않습니다.

## <a name="change-country-of-partner-global-account"></a>파트너 전역 계정의 국가 변경 

1. 파트너 센터에서 MPN 계정을 사용하여 로그인합니다. (MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.) MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다. 

2. **파트너** 탭에서 **비즈니스 위치** 에서 위치 목록을 확인하여 법인으로 원하는 위치가 나열되는지 확인합니다. 
 
1. 위치를 추가하려면 **위치 추가** 를 클릭하고, 플라이 아웃에서 회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다. 
 
1. **국가/지역** 드롭다운 목록 옆에 있는 **국가 변경** 을 선택하고 단계를 따릅니다. 

:::image type="content" source="images/lbp.png" alt-text="법적 비즈니스 프로필 데이터 플라이 아웃.":::

5. **저장** 을 선택합니다.

6. MPN 전역 계정 국가는 새로운 법적 국가로 변경됩니다.
  
## <a name="next-steps"></a>다음 단계

- [확인 프로세스](verification-responses.md)에 대해 알아보세요.
