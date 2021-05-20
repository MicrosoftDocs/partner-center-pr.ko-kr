---
title: Dynamics 365 CRM 파트너 센터 공동 판매 커넥터
description: 파트너 센터 조회를 Dynamics 365 CRM용 공동 판매 커넥터와 동기화합니다. 그런 다음 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 035a819020097ddee2230b5541e1b477d4b34c14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148468"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Dynamics 365 CRM용 공동 판매 커넥터 개요

**적절한 역할:** 조회 관리자 | CRM의 시스템 관리자 또는 시스템 사용자 지정자

파트너 센터 공동 판매 커넥터를 사용하면 판매자가 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다. 공동 판매 거래를 관리하는 데 파트너 센터 사용하도록 학습할 필요가 없습니다. 공동 판매 커넥터를 사용하여 새 공동 판매 추천을 만들어 Microsoft 판매자에게 참여시키고, Microsoft 판매자로부터 추천을 받고, 추천을 수락 또는 거부하며, 거래 가치 및 마감 날짜와 같은 거래 데이터를 수정합니다. 이러한 공동 판매 거래에 대한 Microsoft 판매자의 업데이트를 받을 수도 있습니다. 모든 조회 작업은 파트너 센터 대신 선택한 CRM에서 관리할 수 있습니다.

솔루션은 Power Automate 기반으로 하며 파트너 센터 API를 사용합니다.

## <a name="prerequisites"></a>필수 조건

솔루션을 설치하기 전에 다음 필수 구성을 충족해야 합니다.

|**토픽**   |**세부 정보**   |**연결**   |
|--------------|--------------------|------|
|MPN(Microsoft 파트너 네트워크) ID |유효한 MPN ID가 필요합니다.|[파트너 네트워크 가입](https://partner.microsoft.com/)|
|공동 판매 준비|IP/서비스 솔루션은 공동 판매 준비가 되어 있어야 합니다.|[Microsoft로 판매](https://partner.microsoft.com/membership/sell-with-microsoft)|
|파트너 센터 계정|파트너 센터 테넌트와 연결된 MPN ID는 공동 판매 솔루션과 연결된 MPN ID와 동일해야 합니다. 커넥터를 배포하기 전에 파트너 센터 포털에서 공동 판매 추천을 볼 수 있는지 확인합니다.|[계정 관리](create-user-accounts-and-set-permissions.md)|
|파트너 센터 사용자 역할|커넥터를 설치하고 사용할 직원은 조회 관리자여야 합니다.|[사용자 역할 및 권한 할당](create-user-accounts-and-set-permissions.md)|
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

   1. 오른쪽 위 모서리의 검색 표시줄에서 **파트너 센터 조회(미리 보기)를** 검색합니다.

   1. 조회 관리자의 자격 증명 역할을 사용하여 파트너 센터 사용자에 대한 연결을 만듭니다.

   1. 다음으로, 조회 관리자 자격 증명을 사용하여 파트너 센터 사용자에 대한 파트너 센터 이벤트 연결을 만듭니다.

   1. CRM 관리자 사용자에 대한 Common Data Service(현재 환경)에 대한 연결을 만듭니다.
     
   1. 모든 연결을 추가한 후에는 사용자 환경에서 다음 연결이 표시됩니다.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="연결을 보여 주는 스크린샷":::

## <a name="edit-the-connections"></a>연결 편집

1. **솔루션** 페이지로 돌아가서 **기본 솔루션** 을 선택합니다. **모든** 를 선택하여 **연결 참조(미리 보기)를** 선택합니다.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="연결 편집을 보여 주는 스크린샷":::

1. 말줄임표 아이콘을 선택하여 각 연결을 개별적으로 편집합니다. 관련 연결을 추가합니다.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="나열된 연결을 보여 주는 스크린샷.":::

1.  **솔루션** 페이지로 돌아가서 **dynamics 365에 대한 파트너 센터 조회 동기화를** 선택하고 다음 시퀀스의 각 흐름 옆에 있는 말줄임표 아이콘을 선택하여 흐름을 켭니다. 흐름을 설정하는 동안 문제가 발생하는 경우 [사용자 지정 단계](connector-dynamics.md#customize-synchronization-steps) 및 문제 해결 단계를 [참조하세요.](connectors-troubleshoot.md)

다음 순서로 흐름을 켭니다.

- 파트너 센터 Webhook 등록(Insider Preview)
- 공동 판매 조회 만들기 – Dynamics 365 to 파트너 센터(Insider Preview)
- [사용자 지정] Dynamics 365 흐름에서 세부 정보 만들기 또는 얻기
- Dynamics 365 - Helper에 파트너 센터(Insider Preview)
- Dynamics 365에 대한 Microsoft 공동 판매 조회 업데이트 파트너 센터(Insider Preview)
- Dynamics 365로 파트너 센터(Insider Preview)
- Dynamics 365 to 파트너 센터(Insider Preview)
- Dynamics 365 파트너 센터 기회(Insider Preview)
- Dynamics 365 Microsoft Solutions to 파트너 센터(Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>webhook API를 사용하여 리소스 변경 이벤트 등록

파트너 센터 webhook API를 사용하여 리소스 변경 이벤트를 등록할 수 있습니다. 이러한 변경 이벤트는 URL에 HTTP 게시물로 전송됩니다.

1. **Dynamics 365에 파트너 센터(Insider Preview) 를** 선택합니다.

1. **편집** 아이콘을 선택하고 **HTTP 요청을 받은 경우를** 선택합니다.

1. **복사** 아이콘을 선택하여 제공된 HTTP POST URL을 복사합니다.

   :::image type="content" source="images/webhook-video.gif" alt-text="webhook를 사용하여 리소스 변경 내용을 등록하는 방법을 보여 주는 스크린샷":::

1. 파트너 센터 **Webhook 등록(Insider Preview)** Power Automate 흐름을 선택한 다음, **실행을** 선택합니다.

1. 오른쪽 창에서 **실행 흐름** 창이 열리는지 확인하고 **계속을** 선택합니다.

1. 다음 세부 정보를 입력합니다.

   - **Http 트리거 엔드포인트:** 이 URL은 이전 단계에서 복사되었습니다.
   - **등록할 이벤트:** 사용 가능한 **이벤트(조회 생성, 조회** **업데이트,** **related-referral-created** 및 **related-referral-updated)를** Select all.
   - **있는 경우 기존 트리거 엔드포인트를 덮어쓰시겠습니까?**: 예. 지정된 웹후크 이벤트에 대해 하나의 URL만 등록할 수 있습니다.

1. **흐름 실행을** 선택한 **다음, 완료를 선택합니다.**

이제 webhook는 이벤트를 수신 대기, 생성 및 업데이트할 수 있습니다.

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
- **고객 계정:** 새 조회가 파트너 센터 CRM으로 동기화되면 Power Automate 솔루션은 고객 회사 이름 및 우편번호를 사용하여 CRM에서 기존 계정을 검색하려고 시도합니다. 찾을 수 없는 경우 CRM에 새 고객 계정이 만들어집니다. 검색 조건 및 새 계정 만들기 세부 정보를 업데이트하려면 **[사용자 지정] Dynamics 365 흐름에서 세부 정보 만들기 또는 받기를** 편집하고 CRM 및 **고객 계정 만들기 작업에서** **고객 계정 만들기 또는 받기로** 이동합니다.

## <a name="update-environment-variable"></a>환경 변수 업데이트

환경 변수 값을 업데이트하려면 다음을 수행합니다.

1. **솔루션** 페이지로 이동하여 기본 **솔루션** 을 선택합니다. **모두** 를 선택하여 **환경 변수를** 선택합니다.

1. 업데이트해야 하는 값에 대한 환경 변수를 선택하고, 말줄임표 아이콘을 사용하여 **편집을** 선택합니다.

1. 새 값 옵션을 사용하고 값을 제공하여 **현재** 값을 업데이트합니다(기본값은 업데이트하지 마세요).   값은 변수의 데이터 형식과 일치해야 합니다. 예를 들어 예 또는 아니요 데이터 형식은 예 또는 아니요 값을 허용합니다.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="환경 변수 업데이트를 보여 주는 스크린샷":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>엔드투엔드 양방향 공동 판매 조회 동기화

Power Automate 솔루션을 설치, 구성 및 사용자 지정한 후에는 Dynamics 365와 파트너 센터 간의 공동 판매 조회 동기화를 테스트할 수 있습니다.

### <a name="prerequisites"></a>필수 조건

파트너 센터 및 Dynamics 365 CRM에서 조회를 동기화하기 위해 Power Automate 솔루션은 Microsoft 관련 조회 필드를 명확하게 구분합니다. 이 ID를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있습니다.

사용자 지정 필드 및 개체 집합이 솔루션 설치의 일부로 추가됩니다. CRM 관리자 사용자는 **기회** 사용자 지정 필드를 사용하여 별도의 CRM 섹션을 만들어야 합니다.

다음 사용자 지정 필드는 CRM 섹션의 일부여야 합니다.

- **파트너 센터와 동기화**: 파트너 센터와 기회를 동기화할지 여부를 결정 합니다. 기본적으로이 필드의 값은 아니요 이며 판매자가 Microsoft와의 기회를 공유 하도록 명시적으로 예로 설정 해야 합니다. 파트너 센터에서 CRM으로 공유 되는 새 조회는이 필드 값을 예로 설정 합니다.
- **조회 식별자**: 파트너 센터 조회에 대 한 읽기 전용 식별자 필드입니다.
- **조회 링크**: 파트너 센터에서 조회에 대 한 읽기 전용 링크입니다.
- **Microsoft에서 microsoft에 어떤 도움을 주는 것이 있나요?**: microsoft에서 조회에 대해 도움을 요청 합니다. 공동 판매 조회를 만들려면 Microsoft에서 필요한 적절 한 도움말을 선택 합니다. 고객 연락처를 공동 판매 참조를 만들 수 있는 기회에 연결 해야 합니다. 비 공동 판매 조회를 만들려면이 필드를 선택 하지 마세요. 비 공동 판매 조회는 적절 한 도움말-필수 옵션을 선택 하 여 언제 든 지 공동 판매 조회로 변환할 수 있습니다.
- **Microsoft 파트너 센터 조회 표시 유형**: 파트너 센터 조회에 대 한 표시 유형을 선택 합니다. Microsoft 판매자에 게 표시 하면 비 공동 판매 조회가 공동 판매로 전환 될 수 있습니다. Microsoft 도움말이 필요한 경우 기본적으로 Microsoft 판매자에 게 조회를 표시 합니다. 이 필드가 표시 된 것으로 표시 된 후에는 되돌릴 수 없습니다.
- **MICROSOFT CRM identifier**: 공동 판매 조회가 microsoft에서 만들어지고 수락 되는 경우이 필드는 MICROSOFT의 CRM 식별자로 채워집니다.
- **제품: 사용 되지** 않음:이 필드를 사용 하지 않거나 CRM 섹션에 추가 하지 마세요. 이전 버전과의 호환성을 위해서만 사용할 수 있습니다. 파트너 센터 솔루션을 대신 사용 합니다.
- **감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역입니다.
- **Microsoft 파트너 센터 솔루션**: 공동 판매 준비 된 솔루션 또는 Microsoft 솔루션을 기회와 연결 하는 사용자 지정 개체입니다. 기회에서 하나 이상의 솔루션을 추가하거나 제거할 수 있습니다. Microsoft와 공유하기 전에 공동 판매 준비 또는 Microsoft 솔루션을 하나 이상 영업 기회로 추가해야 합니다. 이 개체를 영업 기회와 연결하려면 CRM에서 **기회** 양식을 업데이트합니다.

  **기회** 양식에서 적절한 탭을 선택하고 여기에 표시된 대로 하위 그리드를 추가합니다.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="기회 양식을 보여 주는 스크린샷.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft 솔루션을 보여 주는 스크린샷.":::

- Microsoft 솔루션을 추가한 후에는 판매자가 추가할 필요가 없도록 공동 판매 준비 솔루션 세부 정보를 미리 채우면 됩니다. 새 솔루션 세부 정보를 추가하려면 CRM의 Microsoft 솔루션 세부 정보 개체로 이동하고 **레코드 추가를** 선택하여 하나의 항목을 추가하거나 **Excel 업로드를** 사용하여 여러 항목을 추가합니다.

  :::image type="content" source="images/dynamic-1a.png" alt-text="새 Microsoft 솔루션 세부 정보를 보여 주는 스크린샷":::

### <a name="scenarios"></a>시나리오

1. CRM에서 조회를 만들거나 업데이트하고 파트너 센터 동기화할 때 조회 동기화:

   1. CRM의 **기회** 섹션에서 가시성이 있는 사용자로 Dynamics 365 CRM 환경에 로그인합니다.

   1. Dynamics 365 환경에서 새 기회를 만들 때 **Microsoft 파트너 센터** 섹션이 있는지 확인합니다.

      :::image type="content" source="images/dynamic-2a.png" alt-text="새 기회를 보여 주는 스크린샷.":::

   1. 이 기회를 파트너 센터 동기화하려면 카드 보기에서 다음 필드를 설정해야 합니다.

      - **Microsoft에서 어떻게 도움을 줄 수 있나요?**: 공동 판매 추천을 만들려면 적절한 도움말 옵션을 선택합니다.

         :::image type="content" source="images/dynamic-3a.png" alt-text="카드 보기에서 적절한 필드를 얻는 방법을 보여 주는 스크린샷":::

      - **고객 연락처:** 공동 판매 추천을 만들려면 영업 기회에 고객 연락처를 추가합니다.
      - **sync with 파트너 센터:** 예.
      - **Microsoft 솔루션:** Microsoft와 추천을 공유하려면 유효한 공동 판매 준비 또는 Microsoft 솔루션을 이 기회에 추가합니다.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="솔루션 ID를 보여 주는 스크린샷.":::

   1. Dynamics 365에서 파트너 센터 동기화 옵션이 **예로** 설정된 기회를 만든 후 10분 동안 기다립니다. 그런 다음, 파트너 센터 계정에 로그인합니다. 조회는 Dynamics 365 및 조회 **식별자** 와 동기화됩니다. **조회 링크가** 채워집니다. 오류가 발생하면 **감사** 필드가 오류 정보로 채워집니다.
     
    1. 마찬가지로 파트너 센터 동기화 옵션이 **예로** 설정된 기회의 경우 Dynamics 365 CRM에서 기회를 업데이트하면 변경 내용이 파트너 센터 계정에서 동기화됩니다.

    1. 파트너 센터 성공적으로 동기화되는 기회가 Dynamics 365의 ✔icon으로 식별됩니다.

1. 파트너 센터 조회를 만들거나 업데이트하고 Dynamics 365 환경에서 동기화할 때 조회 동기화:

   1. 파트너 센터 [대시보드에 로그인합니다.](https://partner.microsoft.com/dashboard/home)

   1. 왼쪽 메뉴에서 **조회를** 선택합니다.

   1. **새 거래** 옵션을 선택하여 파트너 센터 새 공동 판매 추천을 만듭니다.

   1. Dynamics 365 CRM 환경에 로그인합니다.

   1. 기회 **열기로** 이동합니다. 파트너 센터 만든 조회는 이제 Dynamics 365 CRM에서 동기화됩니다.

   1. 동기화된 조회를 선택하면 카드 보기 세부 정보가 채워집니다.

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)
- [공동 판매 기회 관리](manage-co-sell-opportunities.md)
- [Microsoft Power Automate 플랫폼에 대한 자세한 정보](/power-automate/)
- [파트너 센터 웹후크](/partner-center/develop/partner-center-webhooks)
