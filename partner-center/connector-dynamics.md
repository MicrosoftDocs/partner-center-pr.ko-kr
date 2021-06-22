---
title: Dynamics 365 CRM 파트너 센터 용 공동 판매 커넥터
description: Dynamics 365 CRM 용 공동 판매 커넥터와 파트너 센터의 조회를 동기화 합니다. 그런 다음 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425084"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Dynamics 365 용 공동 판매 커넥터 CRM 개요

**적절 한 역할**: 조회 관리자 | CRM에서 시스템 관리자 또는 시스템 사용자 지정자

파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다. 파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다. 공동 판매 커넥터를 사용 하 여 Microsoft 판매자를 참여 시키고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락 또는 거부 하 고, 거래 가치 및 마감 날짜와 같은 거래 데이터를 수정 하는 새 공동 판매 참조를 만듭니다. 이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다. 파트너 센터가 아닌 선택한 CRM의 모든 조회 작업을 관리할 수 있습니다.

이 솔루션은 전원 자동화를 기반으로 하며 파트너 센터 Api를 사용 합니다.

## <a name="prerequisites"></a>필수 조건

솔루션을 설치 하기 전에 다음 필수 구성 요소를 충족 하는지 확인 합니다.

|**토픽**   |**세부 정보**   |**연결**   |
|--------------|--------------------|------|
|MPN(Microsoft 파트너 네트워크) ID |유효한 MPN ID가 필요 합니다.|[파트너 네트워크에 가입](https://partner.microsoft.com/)|
|공동 판매 준비|I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.|[Microsoft와 판매](https://partner.microsoft.com/membership/sell-with-microsoft)|
|파트너 센터 계정|파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다. 커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.|[계정 관리](create-user-accounts-and-set-permissions.md)|
|파트너 센터 사용자 역할|커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.|[사용자 역할 및 권한 할당](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.|[Dynamics 365에서 역할 할당](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|전원 자동화 흐름 계정|테스트, 준비 및 프로덕션을 위해 데이터베이스를 사용 하 여 새 프로덕션 환경을 만듭니다. 데이터베이스를 사용 하는 기존 프로덕션 환경이 있는 경우 다시 사용할 수 있습니다. 커넥터 솔루션을 설치 하려는 사용자에 게는 전원 자동화 라이선스와이 환경에 대 한 액세스 권한이 있어야 합니다. 설치에 실패 하는 경우 진행 상황을 모니터링 하 고 [전원 자동화](https://flow.microsoft.com/) 에서 자세한 정보를 얻을 수 있습니다. **솔루션** 에서 **기록 보기** 를 선택 합니다.|[환경 만들기 또는 관리](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365에 대 한 파트너 센터 조회 동기화 설치 (전원 자동화 솔루션)

1. [전원 자동화](https://flow.microsoft.com)로 이동 하 고 오른쪽 위 모서리에서 **환경** 을 선택 합니다. 이 단계에서는 사용 가능한 CRM 인스턴스를 보여 줍니다.

1. 오른쪽 위 모서리의 드롭다운 목록에서 적절 한 CRM 인스턴스를 선택 합니다.

1. 왼쪽에서 **솔루션** 을 선택 합니다.

1. 상단 메뉴에서 **AppSource 열기** 링크를 선택 합니다.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="오픈 AppSource를 보여 주는 스크린샷":::

1. 팝업 화면에서 **Dynamics 365에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.  

1. **지금 가져오기** 단추를 선택한 다음 **계속** 을 선택 합니다.

1. CRM (Dynamics 365) 환경을 선택 하 여 응용 프로그램을 설치할 수 있는 페이지가 나타납니다. 사용 약관에 동의 합니다.

1. 진행률을 모니터링 하 고 설치에 실패 하는 경우 **솔루션** 에서 **기록 보기** 를 선택 하 여 전원 자동화에서 자세한 정보를 얻을 수 있습니다.

1. 설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 돌아가서 왼쪽에 있는 **솔루션** 을 선택 합니다. **Dynamics 365에 대 한 파트너 센터 조회 동기화** 는 이제 **솔루션** 목록에서 사용할 수 있습니다.

1. **Dynamics 365에 대 한 파트너 센터 조회 동기화를** 선택 합니다. 다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="사용 가능한 CRMs를 보여 주는 스크린샷":::

## <a name="test-before-you-go-live"></a>라이브 상태로 전환 하기 전에 테스트

프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다. 다음 작업이 필요합니다.

- 스테이징 환경 CRM 인스턴스에 전원 자동화 솔루션을 설치 합니다.
- 스테이징 환경에서 전원 자동화 솔루션을 구성 하 고 사용자 지정 합니다.
- 스테이징 CRM 인스턴스에서 솔루션을 테스트 합니다.
- 성공적으로 테스트 한 후에는를 프로덕션 인스턴스에 관리 솔루션으로 가져옵니다.

## <a name="configure-the-solution"></a>솔루션 구성

1. CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 돌아갑니다.

1. 오른쪽 위 모서리의 **환경** 드롭다운 목록에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.

1. 세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.

   - 조회 관리자 자격 증명이 있는 파트너 센터 사용자
   - 파트너 센터 이벤트
   - 솔루션의 전원 자동화 흐름을 사용 하는 CRM 관리자

   1. 왼쪽에서 **연결** 을 선택 하 고 목록에서 **파트너 센터 조회** 솔루션을 선택 합니다.

   1. **연결 만들기** 를 선택 하 여 연결을 만듭니다.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="연결 만들기를 보여 주는 스크린샷":::

   1. 오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.

   1. 조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.

   1. 다음으로, 조회 관리자 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.

   1. CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.
     
   1. 모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="연결을 보여 주는 스크린샷":::

## <a name="edit-the-connections"></a>연결 편집

1. **솔루션** 페이지로 돌아가서 **기본 솔루션** 을 선택 합니다. **모두** 를 선택 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="연결 편집을 보여 주는 스크린샷":::

1. 줄임표 아이콘을 선택 하 여 각 연결을 개별적으로 편집 합니다. 관련 연결을 추가 합니다.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="나열 된 연결을 보여 주는 스크린샷":::

1. **솔루션** 페이지로 돌아가서, **Dynamics 365에 대 한 파트너 센터 조회 동기화** 를 선택 하 고, 다음 시퀀스의 각 흐름 옆에 있는 줄임표 아이콘을 선택 하 여 흐름을 설정 합니다. 흐름을 설정 하는 동안 문제가 발생 하는 경우 [사용자 지정 단계](connector-dynamics.md#customize-synchronization-steps) 및 [문제 해결 단계](connectors-troubleshoot.md)를 참조 하세요.

다음 순서로 흐름을 설정 합니다.

- 파트너 센터 Webhook 등록 (Insider Preview)
- 공동 판매 조회 – Dynamics 365을 파트너 센터 (Insider Preview)에 만듭니다.
- 대로 Dynamics 365 flow에서 세부 정보를 만들거나 가져옵니다.
- 파트너 센터-Dynamics 365-도우미 (Insider Preview)
- 파트너 센터 Microsoft가 Dynamics 365 (Insider Preview)에 대 한 참조 업데이트를 공동 판매
- 파트너 센터에서 Dynamics 365로 (Insider Preview)
- Dynamics 365-파트너 센터 (Insider Preview)
- Dynamics 365 기회 파트너 센터 (Insider Preview)
- Dynamics 365 Microsoft Solutions 파트너 센터 (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook Api를 사용 하 여 리소스 변경 이벤트 등록

파트너 센터 webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다. 이러한 변경 이벤트는 HTTP 게시로 URL에 전송 됩니다.

1. **파트너 센터에서 Dynamics 365 (Insider preview)을** 선택 합니다.

1. **편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때** 를 선택 합니다.

1. **복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.

   :::image type="content" source="images/webhook-video.gif" alt-text="웹 후크를 사용 하 여 리소스 변경 내용을 등록 하는 방법을 보여 주는 스크린샷":::

1. **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 하 고 **실행** 을 선택 합니다.

1. 오른쪽 창에서 **흐름 실행** 창이 열려 있는지 확인 하 고 **계속** 을 선택 합니다.

1. 다음 세부 정보를 입력합니다.

   - **Http 트리거 끝점**:이 URL은 이전 단계에서 복사 되었습니다.
   - **등록할 이벤트**: 사용 가능한 모든 이벤트 (**조회 생성**, **조회-업데이트**, **관련-조회 생성** 및 **관련 조회-업데이트 됨**)를 선택 합니다.
   - **기존 트리거 끝점이 있으면 덮어쓰시겠습니까?**: 예. 지정 된 webhook 이벤트에 대해 하나의 URL만 등록할 수 있습니다.

1. **흐름 실행** 을 선택한 다음 완료를 선택 **합니다.**

이제 웹 후크는 이벤트를 수신 하 고, 만들고, 업데이트할 수 있습니다.

## <a name="customize-synchronization-steps"></a>동기화 단계 사용자 지정

CRM 시스템은 고도로 사용자 지정 되며 CRM 설정에 따라 전원 자동화 솔루션을 사용자 지정할 수 있습니다. 공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 [사용자 지정 필드 매핑 가이드](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)에 나열 됩니다.

필드 매핑 가이드에 따라 필요한 경우 [사용자 지정]에서 적절 하 게 변경 하 여 **Dynamics 365 flow 또는 환경 변수에서 세부 정보를 만들거나 가져옵니다** . 이후 솔루션 업그레이드에 영향을 줄 수 있으므로 전원 자동화 솔루션에서 다른 흐름을 업데이트 하지 마세요.

다음 사용자 지정을 사용할 수 있습니다.

- **기회 이름에 확인 표시 표시**: 기본적으로 파트너 센터와 DYNAMICS 365 CRM 간의 동기화가 성공적으로 수행 되 고 있음을 나타내기 위해 기회 이름 옆에 확인 표시가 표시 됩니다. 마찬가지로 동기화가 실패할 경우 십자 표시가 표시 됩니다. 기회 이름에 check 또는 cross mark를 추가 하지 않으려면 **기회 이름 환경 변수에서 표시 확인 표시** 의 현재 값을 아니요로 설정 합니다.
- **거래 값**: 기본적으로 파트너 센터의 거래 값은 CRM의 **estimatedvalue** 와 동기화 됩니다. CRM에서 동기화 할 거래 값에 다른 필드가 있는 경우:

  - Dynamics 365 환경 변수의 **거래 값** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다. 표시 이름이 아니라 필드 이름을 제공 해야 합니다.
  - **[사용자 지정] 편집 [사용자 지정] Dynamics 365 flow에서 세부 정보를 만들거나** 업데이트 하 고, Crm에서 **만들기 또는 업데이트 기회** 로 이동 하 고, **새 기회 만들기** 및 업데이트 **기존 기회** 작업을 업데이트 하 여 **DealValue** 값을 crm의 올바른 필드에 할당 합니다. 또한 **예상 수익** 필드에서 **DealValue** 할당을 제거 합니다.

- **고객 계정 국가 코드**: 새 조회를 만들 때 두 문자로 된 국가 코드 (ISO 3166)를 제공 해야 합니다. 기본적으로 국가 코드는 CRM의 계정 **address1_country** 필드와 동기화 됩니다. CRM에서 동기화 할 국가 코드에 대 한 다른 필드가 있는 경우:

  - 두 문자로 된 코드를 포함 하는 계정에 있는 비 조회 국가 코드 필드:
    - Dynamics 365 환경 변수의 **고객 계정 국가 코드** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다. 표시 이름이 아니라 필드 이름을 제공 해야 합니다.
    - 편집 **[사용자 지정] Dynamics 365 flow에서 세부 정보를 만들거나 가져온** 다음 crm 작업에서 **고객 계정 만들기 또는 가져오기** 로 이동 하 여 crm의 올바른 필드에 **국가** 값을 할당 합니다. 또한 **Address 1: country/region** 필드에서 **country** value 할당을 제거 합니다.

  - 계정에서 조회 기반 국가 코드 필드:
    - 계정에 새 사용자 지정 필드를 추가 하 고 조회 기반 필드에서 선택한 값을 기준으로 두 자로 된 국가 코드 (ISO 3166)로 자동으로 채우거 나 그 반대의 경우도 마찬가지입니다.
    - 비 조회 국가 코드 필드에 대해 앞의 단계를 수행 하 여 CRM과 파트너 센터 간에 새 사용자 지정 필드를 동기화 합니다.

- **기회 필드**: 채워야 하는 **기회** 에 필수 필드가 있는 경우 **[사용자 지정]을 편집 하 여 Dynamics 365 Flow에서 세부 정보를 만들거나** 확인 하 고 CRM에서 **만들기 또는 업데이트 기회** 로 이동 및 업데이트 비즈니스 요구 사항에 따라 필수 필드에 값을 할당 하는 **새 기회 작업을 만듭니다** .
- **잠재 고객 필드**: 채워야 하는 **선행** 의 필수 필드가 있는 경우 [사용자 지정]을 편집 하 여 **Dynamics 365 Flow에서 세부 정보를 만들거나** 업데이트 하 고, CRM에서 **잠재 고객을 만들거나** 업데이트 하 고, 비즈니스 요구 사항에 따라 필수 필드에 값을 할당 하는 **새 잠재 고객 작업을 만듭니다** .
- **고객 계정**: 파트너 센터에서 crm으로 새 조회를 동기화 할 경우, 전원 자동화 솔루션은 고객 회사 이름 및 우편 번호를 사용 하 여 CRM에서 기존 계정을 검색 하려고 시도 합니다. 하나를 찾지 못하면 CRM에 새 고객 계정이 생성 됩니다. 검색 조건 및 새 계정 만들기 정보를 업데이트 하려면 **[사용자 지정]을 편집 하 여 Dynamics 365 flow에서 세부 정보를 만들거나 가져온** 다음 CRM에서 고객 **계정 만들기 또는 가져오기** 및 **고객 계정 만들기 작업** 으로 이동 합니다.

## <a name="update-environment-variable"></a>환경 변수 업데이트

환경 변수 값을 업데이트 하려면:

1. **솔루션** 페이지로 이동 하 여 **기본 솔루션** 을 선택 합니다. **모두** 를 선택 하 여 **환경 변수** 를 선택 합니다.

1. 업데이트 해야 하는 값에 대 한 환경 변수를 선택 하 고 줄임표 아이콘을 사용 하 여 **편집** 을 선택 합니다.

1. **새 값** 옵션을 사용 하 고 값을 제공 하 여 **현재 값** 을 업데이트 합니다 ( **기본값** 업데이트 안 함). 값은 변수의 데이터 형식과 일치 해야 합니다. 예를 들어 예 또는 아니요 데이터 형식은 예 또는 아니요 값을 허용 합니다.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="환경 변수 업데이트를 보여 주는 스크린샷":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>종단 간 양방향 공동 판매 참조 동기화

전원 자동화 솔루션을 설치, 구성 및 사용자 지정한 후 Dynamics 365 및 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.

### <a name="prerequisites"></a>필수 조건

파트너 센터 및 Dynamics 365 CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 정하는 합니다. 이 id는 판매자 팀이 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.

솔루션 설치의 일부로 사용자 지정 필드 및 개체 집합이 추가 됩니다. CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.

다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.

- **파트너 센터와 동기화**: 파트너 센터와 기회를 동기화할지 여부를 결정 합니다. 기본적으로이 필드의 값은 아니요 이며 판매자가 Microsoft와의 기회를 공유 하도록 명시적으로 예로 설정 해야 합니다. 파트너 센터에서 CRM으로 공유 되는 새 조회는이 필드 값을 예로 설정 합니다.
- **조회 식별자**: 파트너 센터 조회에 대 한 읽기 전용 식별자 필드입니다.
- **조회 링크**: 파트너 센터에서 조회에 대 한 읽기 전용 링크입니다.
- **Microsoft에서 microsoft에 어떤 도움을 주는 것이 있나요?**: microsoft에서 조회에 대해 도움을 요청 합니다. 공동 판매 조회를 만들려면 Microsoft에서 필요한 적절 한 도움말을 선택 합니다. 고객 연락처를 공동 판매 참조를 만들 수 있는 기회에 연결 해야 합니다. 비 공동 판매 조회를 만들려면이 필드를 선택 하지 마세요. 비 공동 판매 조회는 적절 한 도움말-필수 옵션을 선택 하 여 언제 든 지 공동 판매 조회로 변환할 수 있습니다.
- **Microsoft 파트너 센터 조회 표시 유형**: 파트너 센터 조회에 대 한 표시 유형을 선택 합니다. Microsoft 판매자에 게 표시 하면 비 공동 판매 조회가 공동 판매로 전환 될 수 있습니다. Microsoft 도움말이 필요한 경우 기본적으로 Microsoft 판매자에 게 조회를 표시 합니다. 이 필드가 표시 된 것으로 표시 된 후에는 되돌릴 수 없습니다.
- **MICROSOFT CRM identifier**: 공동 판매 조회가 microsoft에서 만들어지고 수락 되는 경우이 필드는 MICROSOFT의 CRM 식별자로 채워집니다.
- **제품: 사용 되지** 않음:이 필드를 사용 하지 않거나 CRM 섹션에 추가 하지 마세요. 이전 버전과의 호환성을 위해서만 사용할 수 있습니다. 파트너 센터 솔루션을 대신 사용 합니다.
- **감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역입니다.
- **Microsoft 파트너 센터 솔루션**: 공동 판매 준비 된 솔루션 또는 Microsoft 솔루션을 기회와 연결 하는 사용자 지정 개체입니다. 하나 이상의 솔루션을 기회에서 추가 하거나 제거할 수 있습니다. Microsoft와 공유 하기 전에 하나 이상의 공동 판매 준비 또는 Microsoft 솔루션을 기회에 추가 해야 합니다. 이 개체를 기회에 연결 하려면 CRM에서 **기회** 양식을 업데이트 합니다.

  **기회** 양식에서 적절 한 탭을 선택 하 고 여기에 표시 된 대로 subgrid를 추가 합니다.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="기회 양식을 보여 주는 스크린샷":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft 솔루션을 보여 주는 스크린샷":::

- Microsoft 솔루션을 추가한 후에 판매자가 추가할 필요가 없도록 공동 판매 준비 솔루션 세부 정보를 미리 채울 수 있습니다. 새 솔루션 세부 정보를 추가 하려면 CRM의 Microsoft Solution Details 개체로 이동 하 고 **레코드 추가** 를 선택 하 여 항목을 하나 추가 하거나 **Excel 업로드** 를 사용 하 여 여러 항목을 추가 합니다.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="새로운 Microsoft 솔루션 세부 정보를 보여 주는 스크린샷":::

### <a name="scenarios"></a>시나리오

1. CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:

   1. CRM의 **기회** 섹션에 표시 되는 사용자를 사용 하 여 DYNAMICS 365 CRM 환경에 로그인 합니다.

   1. Dynamics 365 환경에서 새로운 기회를 만들 때 **Microsoft 파트너 센터** 섹션이 있는지 확인 합니다.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="새 기회를 보여 주는 스크린샷":::

   1. 파트너 센터와이 기회를 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.

      - **Microsoft에서 어떻게 도울 수 있나요?**: 공동 판매 조회를 만들려면 적절 한 도움말 옵션을 선택 합니다.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="카드 보기에서 적절 한 필드를 가져오는 방법을 보여 주는 스크린샷":::

      - **고객 연락처**: 공동 판매 리퍼럴을 만들려면 기회에 고객 연락처를 추가 합니다.
      - **파트너 센터와 동기화**: 예.
      - **Microsoft 솔루션**: microsoft와의 조회를 공유 하려면 올바른 공동 판매 준비 또는 microsoft 솔루션을 기회에 추가 합니다.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="솔루션 ID를 보여 주는 스크린샷":::

   1. **파트너 센터에 동기화** 옵션을 예로 설정 하 여 Dynamics 365에서 기회가 생성 된 후 10 분 정도 기다립니다. 파트너 센터 계정에 로그인 합니다. 사용자의 조회가 Dynamics 365 및 **조회 식별자** 와 동기화 됩니다. **조회 링크** 를 채웁니다. 오류가 있으면 **감사** 필드가 오류 정보로 채워집니다.

      1. 마찬가지로, **파트너 센터와 동기화** 옵션을 예로 설정 하는 기회에 대해 DYNAMICS 365 CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정에서 동기화 됩니다.

      1. 파트너 센터와 성공적으로 동기화 되는 기회는 Dynamics 365의 ✔ 아이콘으로 식별 됩니다.

1. 조회가 파트너 센터에서 만들어지거나 업데이트 된 후 Dynamics 365 환경에서 동기화 되는 경우의 조회 동기화:

   1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.

   1. 왼쪽 메뉴에서 **조회** 를 선택 합니다.

   1. **새 거래** 옵션을 선택 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.

   1. Dynamics 365 CRM 환경에 로그인 합니다.

   1. **오픈 기회** 로 이동 합니다. 이제 파트너 센터에서 만든 조회가 Dynamics 365 CRM에서 동기화 됩니다.

   1. 동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)
- [공동 판매 기회 관리](manage-co-sell-opportunities.md)
- [Microsoft Power 자동화 플랫폼에 대 한 자세한 정보](/power-automate/)
- [파트너 센터 웹후크](/partner-center/develop/partner-center-webhooks)
