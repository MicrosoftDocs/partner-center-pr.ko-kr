---
title: Salesforce CRM 파트너 센터 대한 공동 판매 커넥터
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 조회를 Salesforce CRM과 동기화합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173673"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM용 공동 판매 커넥터 – 개요

**적절한 역할:** 조회 관리자 | CRM의 시스템 관리자 또는 시스템 사용자 지정자

파트너 센터 공동 판매 커넥터를 사용하면 판매자가 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다. 공동 판매 거래를 관리하는 데 파트너 센터 사용하도록 학습할 필요가 없습니다. 공동 판매 커넥터를 사용하여 새 공동 판매 추천을 만들어 Microsoft 판매자에게 참여시키고, Microsoft 판매자로부터 추천을 받고, 조회를 수락/거부하며, 거래 가치와 같은 거래 데이터를 수정하고, 종료 날짜를 만들 수 있습니다.  이러한 공동 판매 거래에 대한 Microsoft 판매자의 업데이트를 받을 수도 있습니다. 파트너 센터 대신 선택한 CRM 내에서 작업하는 동안 모든 조회 작업을 수행할 수 있습니다.

솔루션은 Microsoft Power Automate Solution을 기반으로 하며 파트너 센터 API를 사용합니다.

## <a name="before-you-install---pre-requisites"></a>설치하기 전에 - 필수 조건

|**토픽**|**세부 정보**|**연결**|
|--------------|--------------------|------|
|Microsoft 파트너 네트워크 ID |유효한 MPN ID가 필요합니다.|[MPN을](https://partner.microsoft.com/) 조인하려면|
|공동 판매 준비|IP/서비스 솔루션은 공동 판매 준비가 되어 있어야 합니다.|[Microsoft로 판매](https://partner.microsoft.com/membership/sell-with-microsoft)|
|파트너 센터 계정|파트너 센터 테넌트와 연결된 MPN ID는 공동 판매 솔루션과 연결된 MPN ID와 동일해야 합니다. 커넥터를 배포하기 전에 파트너 센터 Portal에서 공동 판매 추천을 볼 수 있는지 확인합니다.|[계정 관리](create-user-accounts-and-set-permissions.md)|
|파트너 센터 사용자 역할|커넥터를 설치하고 사용할 직원은 조회 관리자여야 합니다.|[사용자 역할 및 권한 할당](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.|[Salesforce CRM에서 역할 할당](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow 계정|테스트, 스테이징 및 프로덕션을 위한 데이터베이스를 사용하여 새 프로덕션 환경을 만듭니다. 데이터베이스가 있는 기존 프로덕션 환경이 있는 경우 다시 사용할 수 있습니다. 커넥터 솔루션을 설치하려는 사용자에게는 Power Automate 라이선스와 이 환경에 대한 액세스 권한이 있어야 합니다. 설치가 실패하면 진행 상황을 모니터링하고 [Power Automate](https://flow.microsoft.com/) 자세한 정보를 얻을 수 있습니다. 솔루션 에서 **기록 보기를** **선택합니다.**|[환경 만들기 또는 관리](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft 사용자 지정 필드용 Salesforce 패키지 설치

파트너 센터 및 Salesforce CRM에서 조회를 동기화하려면 Power Automate 솔루션이 Microsoft 특정 조회 필드를 명확하게 식별해야 합니다. 이 구분은 파트너 판매자 팀이 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있는 기능을 제공합니다.

1. Salesforce에서 **메모를** 활성화하고 기회 관련 목록에 추가합니다. [참조](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. 다음 단계에 따라 **기회 팀을** 활성화합니다.
    - 설치 프로그램에서 **빠른 찾기** 상자를 사용하여 기회 팀 설정 찾습니다.
    - 필요에 따라 설정을 정의합니다. [참조](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Salesforce에서 패키지 설치 관리자 를 사용하여 사용자 지정 필드 및 개체를 [설치합니다.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) 이 설치 관리자를 사용하여 모든 회사에 패키지를 설치합니다.

    >[!NOTE]
    >샌드박스에 를 설치하는 경우 URL의 초기 부분을 로 바꾸어야 `http://test.salesforce.com` 합니다.

1. Salesforce에서 **기회** 관련 목록에 Microsoft 솔루션을 추가합니다. 추가되면 **렌치** 아이콘을 선택하고 속성을 업데이트합니다.

## <a name="best-practice-test-before-you-go-live"></a>모범 사례: 라이브로 진행하기 전에 테스트

프로덕션 환경에서 Power Automate 솔루션을 설치, 구성 및 사용자 지정하기 전에 준비 CRM 인스턴스에서 솔루션을 테스트해야 합니다.

- 스테이징 환경/CRM 인스턴스에 Microsoft Power Automate 솔루션을 설치합니다.

- 솔루션의 복사본을 만들고 스테이징 환경에서 구성 및 Power Automate 흐름 사용자 지정을 실행합니다.

- 스테이징/CRM 인스턴스에서 솔루션을 테스트합니다.

- 성공하면 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM에 대한 파트너 센터 조회 동기화 설치

1. [Power Automate](https://flow.microsoft.com) 이동하여 오른쪽 위 모서리에서 **환경을** 선택합니다. 그러면 사용 가능한 CRM 인스턴스가 표시됩니다.

1. 오른쪽 위 모서리의 드롭다운 목록에서 적절한 CRM 인스턴스를 선택합니다.

1. 왼쪽 탐색 모음에서 **솔루션을** 선택합니다.

1. 위쪽 메뉴에서 **AppSource 열기** 링크를 선택합니다.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="AppSource를 엽니다.":::

1. 팝업 화면에서 **salesforce에 대한 파트너 센터 조회 커넥터를** 검색합니다.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="지금 받기의 스크린샷.":::

1. 지금 **받기** 단추를 선택한 다음, **계속을** 선택합니다.

1. 다음 페이지에서 Salesforce CRM 환경을 선택하여 애플리케이션을 설치합니다. 약관에 동의합니다.

1. 그런 다음 솔루션 관리 페이지로 **안내됩니다.**  페이지 아래쪽의 화살표 단추를 사용하여 "파트너 센터 조회"로 이동합니다. 파트너 센터 조회 솔루션 옆에 **설치가 예약되어** 있어야 합니다. 설치하는 데 10-15분이 걸립니다.

1. 설치가 완료되면 [Power Automate](https://flow.microsoft.com) 다시 이동하고 왼쪽 탐색 영역에서 **솔루션을** 선택합니다. 이제 솔루션 목록에서 **Salesforce에 대한 파트너 센터 조회 동기화를** 사용할 수 있습니다.

1. **Salesforce에 파트너 센터 조회 동기화를** 선택합니다. 다음 Power Automate 흐름 및 엔터티를 사용할 수 있습니다.

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce 흐름.":::

## <a name="configure-the-solution"></a>솔루션 구성

1. CRM 인스턴스에 솔루션을 설치한 후 [Power Automate](https://flow.microsoft.com/)으로 다시 이동합니다.

1. 오른쪽 위 모서리의 **환경** 드롭다운에서 Power Automate 솔루션을 설치한 CRM 인스턴스를 선택합니다.

1. 세 개의 사용자 계정을 연결하는 연결을 만들어야 합니다.

   - 조회 관리자 자격 증명을 사용하여 사용자 파트너 센터
   - 파트너 센터 이벤트
   - 솔루션의 Power Automate 흐름을 가진 CRM 관리자

   1. 왼쪽 탐색 모음에서 **연결을** 선택하고 목록에서 **파트너 센터 조회** 솔루션을 선택합니다.

   1. 연결 만들기를 선택하여 **연결을 만듭니다.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="연결 만들기를 보여 주는 스크린샷.":::

   1. 오른쪽 위 모서리의 검색 표시줄에서 **파트너 센터 조회(미리 보기)를** 검색합니다.

   1. 조회 관리자의 자격 증명 역할을 사용하여 파트너 센터 사용자에 대한 연결을 만듭니다.

   1. 다음으로, 조회 관리자의 자격 증명을 사용하여 파트너 센터 사용자에 대한 파트너 센터 이벤트 연결을 만듭니다.

   1. CRM 관리자 사용자에 대한 Salesforce에 대한 연결을 만듭니다.
  
   1. CRM 관리자 사용자에 대한 Microsoft Dataverse에 대한 연결을 만듭니다.

   1. 모든 연결을 추가한 후 사용자 환경에 다음 연결이 표시됩니다.

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="연결을 관찰하는 방법을 보여 주는 스크린샷":::

### <a name="edit-the-connections"></a>연결 편집

1. **솔루션** 페이지로 돌아가서 **기본 솔루션** 을 선택합니다. **모든** 를 클릭하여 **연결 참조(미리 보기)를** 선택합니다.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="연결 편집을 보여 주는 스크린샷":::

1. 줄임표 아이콘을 선택 하 여 각 연결을 개별적으로 편집 합니다. 관련 연결을 추가 합니다.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="스크린샷 atht 커넥터를 편집 하는 방법을 보여 줍니다.":::

1. 다음 순서로 흐름을 설정 합니다.
   - 파트너 센터 Webhook 등록 (Insider Preview)
   - 대로 Salesforce에서 세부 정보 만들기 또는 가져오기
   - 파트너 센터에 공동 판매 Referral-Salesforce 만들기 (Insider Preview)
   - 파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매  
   - 파트너 센터를 Salesforce로 (Insider Preview)
   - Salesforce에서 파트너 센터로 (Insider Preview)
   - Salesforce 기회와 파트너 센터 간 (Insider Preview)
   - 파트너 센터 (Insider Preview)에 대 한 Salesforce Microsoft 솔루션

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook Api를 사용 하 여 리소스 변경 이벤트 등록

파트너 센터 webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다. 이러한 변경 이벤트는 HTTP 게시로 URL에 전송 됩니다.

1. **파트너 센터에서 SALESFORCE CRM (Insider preview)을** 선택 합니다.

1. **편집 아이콘** 을 선택 하 고 **HTTP 요청을 받을 때** 를 선택 합니다.

1. **복사** 아이콘을 선택 하 여 제공 된 **HTTP POST URL** 을 복사 합니다.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL을 복사 하는 방법을 보여 주는 스크린샷":::

1. **파트너 센터 Webhook 등록 (Insider preview)** Power Automate flow를 선택 하 고 **실행** 을 선택 합니다.

1. 오른쪽 창에서 **흐름 실행** 창이 열려 있는지 확인 하 고 **계속** 을 선택 합니다.

1. 다음 세부 정보를 입력합니다.

   - **Http 트리거 끝점**:이 URL은 이전 단계에서 복사 되었습니다.
   - **등록할 이벤트**: 사용 가능한 모든 이벤트 (**조회 생성**, **조회-업데이트**, **관련-조회 생성** 및 **관련 조회-업데이트 됨**)를 선택 합니다.
   - **기존 트리거 끝점이 있으면 덮어쓰시겠습니까?**: 예. 지정 된 webhook 이벤트에 대해 하나의 URL만 등록할 수 있습니다.

1. **흐름 실행** 을 선택한 다음 **완료** 를 선택 합니다.

이제 웹 후크는 이벤트를 수신 하 고, 만들고, 업데이트할 수 있습니다.

## <a name="customize-synchronization-steps"></a>동기화 단계 사용자 지정

crm 시스템은 고도로 사용자 지정 되며 crm 설정에 따라 Power Automate 솔루션을 사용자 지정할 수 있습니다. 공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 [사용자 지정 필드 매핑 가이드](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)에 나열 됩니다.

필드 매핑 가이드에 따라 필요한 경우 [사용자 지정]에서 적절 하 게 변경 하 여 Salesforce 또는 환경 변수 **에서 세부 정보를 만들거나 가져옵니다** . 이후 솔루션 업그레이드에 영향을 줄 수 있으므로 Power Automate 솔루션에서 다른 흐름을 업데이트 하지 마세요.

다음 사용자 지정을 사용할 수 있습니다.

- **기회 이름에 확인 표시 표시**: 기본적으로 파트너 센터와 Salesforce CRM 간의 동기화가 성공적으로 수행 되 고 있음을 나타내기 위해 기회 이름 옆에 확인 표시가 표시 됩니다. 마찬가지로 동기화가 실패할 경우 십자 표시가 표시 됩니다. 기회 이름에 check 또는 cross mark를 추가 하지 않으려면 **기회 이름 환경 변수에서 표시 확인 표시** 의 현재 값을 아니요로 설정 합니다.

- **단계 이름**:

  - **활성 단계 이름**: Salesforce의 영업 기회 영업 파이프라인 단계입니다.  활성 단계를 나타내며 파트너 센터에서 수락 됨 상태의 조회와 동일 합니다. 이는 보류 단계 후 판매 파이프라인의 다음 단계 일 수 있습니다. 영업 기회의 영업 스테이지를 대기 중인 활성 단계로 이동 하면 파트너 센터의 조회가 수락 되 고 변경 내용이 동기화 되기 시작 합니다.

  - **보류 중인 단계 이름**: Salesforce의 영업 기회 영업 파이프라인에 있는 단계의 이름입니다. 보류 중인 단계를 나타냅니다. 아직 수락 되지 않은 Microsoft에서 공유 하는 새 공동 판매 조회는 Salesforce에서이 단계로 설정 됩니다. 보류 중인 기회의 모든 변경 내용은 파트너 센터에 동기화 되지 않습니다. 이 온-보류 단계에서 기회의 영업 스테이지를 이동 하면 파트너 센터의 조회가 수락 되 고 변경 내용이 동기화 되기 시작 합니다.

- **고객 계정 국가 코드**: 새 조회를 만들 때 두 문자로 된 국가 코드 (ISO 3166)를 제공 해야 합니다. 기본적으로 국가 코드는 Salesforce의 계정 **BillingCountry** 필드와 동기화 됩니다. Salesforce에서 동기화 할 국가 코드에 대 한 다른 필드가 있는 경우:

  - 두 문자로 된 코드를 포함 하는 계정에 있는 비 조회 국가 코드 필드:

    - Salesforce 환경 변수의 **고객 계정 국가 코드** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다. 표시 이름이 아니라 필드 이름을 제공 해야 합니다.

    - 편집 **[사용자 지정] Salesforce에서 세부 정보를 만들거나 가져온** 다음 crm에서 **고객 계정 만들기 또는 가져오기** 작업으로 이동 하 여 crm의 올바른 필드에 **국가** 값을 할당 합니다. 또한 **BillingCountry** 에서 **Country** value 할당을 제거 합니다.

  - 계정에서 조회 기반 국가 코드 필드:

    - 계정에 새 사용자 지정 필드를 추가 하 고 조회 기반 필드에서 선택한 값을 기준으로 두 자로 된 국가 코드 (ISO 3166)로 자동으로 채우거 나 그 반대의 경우도 마찬가지입니다.

    - 비 조회 국가 코드 필드에 대해 앞의 단계를 수행 하 여 CRM과 파트너 센터 간에 새 사용자 지정 필드를 동기화 합니다.

- **거래 값**: 기본적으로 파트너 센터의 거래 값은 CRM의 **양과** 동기화 됩니다. CRM에서 동기화 할 거래 값에 다른 필드가 있는 경우:

  - Salesforce 환경 변수의 **거래 값** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다. 표시 이름이 아니라 필드 이름을 제공 해야 합니다.

  - **[사용자 지정] 편집 [사용자 지정] salesforce에서 세부 정보를 만들거나 가져온** 후 CRM에서 **영업 기회 만들기 또는 업데이트** 로 이동 하 여 **새 기회 만들기** 및 **기존 기회 업데이트** 작업을 모두 업데이트 하 여 salesforce의 올바른 필드에 **DealValue** 를 할당 합니다.

- **거래 값 통화 코드**: Salesforce의 거래 가치 통화 코드 필드 이름입니다. 이 필드 API 이름은 Microsoft 파트너 센터에서 조회를 만들거나 업데이트할 때 기회의 거래 가치 통화 코드를 가져오는 데 사용 됩니다. 통화 값 통화 코드 필드가 기본 필드인 **CurrencyIsoCode** 와 다른 경우이 환경 변수의 현재 값을 업데이트 합니다.

  - Salesforce 환경 변수의 **거래 값 통화** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다. 표시 이름이 아니라 필드 이름을 제공 해야 합니다.

  - **[사용자 지정] 편집 [사용자 지정] salesforce에서 세부 정보를 만들거나 가져온** 후 CRM에서 **영업 기회 만들기 또는 업데이트** 로 이동 하 여 **새 기회 만들기** 및 **기존 기회 업데이트** 작업을 모두 업데이트 하 여 salesforce의 올바른 필드에 **DealValueCurrency** 를 할당 합니다.

- **공동 판매 기회 동기화**: **예** 로 설정 된 경우 공동 판매 및 파이프라인 공유 기회만 파트너 센터에서 Salesforce로 동기화 됩니다. **아니요** 로 설정 하면 잠재 고객, 공동 판매 및 파이프라인 공유 기회가 파트너 센터에서 Salesforce로 동기화 됩니다. 이 변수는 Salesforce에서 파트너 센터로 동기화 된 기회에 영향을 주지 않습니다.

## <a name="update-environment-variable"></a>환경 변수 업데이트

환경 변수 값을 업데이트 하려면:

1. **솔루션** 페이지로 이동 하 여 **기본 솔루션** 을 선택 합니다. **모두** 를 선택 하 여 **환경 변수** 를 선택 합니다.

1. 업데이트 해야 하는 값에 대 한 환경 변수를 선택 하 고 줄임표 아이콘을 사용 하 여 **편집** 을 선택 합니다.

1. **새 값** 옵션을 사용 하 고 값을 제공 하 여 **현재 값** 을 업데이트 합니다 ( **기본값** 업데이트 안 함). 값은 변수의 데이터 형식과 일치 해야 합니다. 예를 들어 예 또는 아니요 데이터 형식은 예 또는 아니요 값을 허용 합니다.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="환경 변수 업데이트를 보여 주는 스크린샷":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>종단 간 양방향 공동 판매 참조 동기화

Power Automate 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.

### <a name="pre-requisites"></a>필수 구성 요소

파트너 센터 및 Salesforce CRM에서 조회를 동기화 하려면 Power Automate 솔루션이 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다. 이 id는 판매자 팀에 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.

사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다. CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.

다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.

- **파트너 센터와 동기화**: 파트너 센터와 기회를 동기화할지 여부를 결정 합니다. 기본적으로이 필드의 값은 아니요 이며 판매자가 Microsoft와의 기회를 공유 하도록 명시적으로 예로 설정 해야 합니다. 파트너 센터에서 CRM으로 공유 되는 새 조회는이 필드 값을 예로 설정 합니다.

- **참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드입니다.

- **참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크입니다.

- Microsoft의 도움을 주는 **방법**: microsoft에서 조회에 대 한 도움을 요청 합니다. 공동 판매 조회를 만들려면 Microsoft에서 필요한 적절 한 도움말을 선택 합니다. 고객 연락처를 공동 판매 참조를 만들 수 있는 기회에 연결 해야 합니다. 비 공동 판매 조회를 만들려면이 필드를 선택 하지 마세요. 비 공동 판매 조회는 적절 한 도움말-필수 옵션을 선택 하 여 언제 든 지 공동 판매 조회로 변환할 수 있습니다.

- **Microsoft 파트너 센터 조회 표시 유형**: 파트너 센터 조회에 대 한 표시 유형을 선택 합니다. Microsoft 판매자에게 표시하면 공동 판매가 아닌 추천이 공동 판매로 전환될 수 있습니다. Microsoft 도움말이 필요한 경우 추천은 기본적으로 Microsoft 판매자에게 표시됩니다. 이 필드가 표시되는 것으로 표시되면 되돌릴 수 없습니다.

- **Microsoft CRM 식별자:** 공동 판매 조회를 만들고 Microsoft에서 수락하면 이 필드에 Microsoft의 CRM 식별자가 채워집니다.

- **Microsoft 파트너 센터 Solutions:** 공동 판매 준비 솔루션 또는 Microsoft 솔루션을 기회와 연결하는 사용자 지정 개체입니다. 기회에서 하나 이상의 솔루션을 추가하거나 제거할 수 있습니다. Microsoft와 공유하기 전에 적어도 하나의 공동 판매 준비 또는 Microsoft 솔루션을 영업 기회로 추가해야 합니다. 이 개체를 영업 기회와 연결하려면 CRM에서 **기회** 양식을 업데이트합니다.

- **감사:** 파트너 센터 조회와 동기화하기 위한 읽기 전용 감사 내역

### <a name="scenarios"></a>시나리오

1. CRM에서 조회를 만들거나 업데이트하고 파트너 센터 동기화할 때 조회 동기화:

   1. CRM의 **기회** 섹션에서 가시성이 있는 사용자로 Salesforce CRM 환경에 로그인합니다.

   1. Salesforce CRM 환경에서 **새 기회를** 만들 때 **Microsoft 파트너 센터** 섹션이 있는지 확인합니다.

   1. 파트너 센터 성공적으로 동기화되는 기회가 Salesforce CRM의 ✔ 아이콘으로 식별됩니다.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce 환경의 스크린샷.":::

   1. 이 기회를 Microsoft 파트너 센터 동기화하려면 카드 보기에서 다음 필드를 설정해야 합니다.

      - **Microsoft에서 어떻게 도움을 줄 수 있나요?**: 공동 판매 추천을 만들려면 적절한 도움말 옵션을 선택합니다.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="카드 보기에서 적절한 필드를 얻는 방법을 보여 주는 스크린샷":::

      - **파트너 센터 동기화:** 예
      - **고객 연락처:** 공동 판매 추천을 만들려면 영업 기회에 고객 연락처를 추가합니다.
      - **Microsoft 솔루션:** Microsoft와 추천을 공유하려면 영업 기회에서 유효한 공동 판매 준비 또는 Microsoft 솔루션을 추가합니다.

   1. 파트너 센터 동기화 옵션을 **예로** 설정한 후 10분 동안 기다린 후 파트너 센터 계정에 로그인합니다.  조회가 Salesforce CRM과 동기화되고 조회 링크가 채워집니다. 오류가 발생하면 감사 필드가 오류 정보로 채워집니다.

   1. 마찬가지로 **파트너 센터 동기화** 옵션이 **예** 로 설정된 경우 Salesforce CRM에서 기회를 업데이트하면 변경 내용이 파트너 센터 계정과 동기화됩니다.

2. Microsoft 파트너 센터 조회를 만들거나 업데이트하고 Salesforce CRM 환경에서 동기화할 때 조회 동기화:

    1. 파트너 센터 [대시보드에 로그인합니다.](https://partner.microsoft.com/dashboard/home)

    1. 왼쪽 메뉴에서 **조회를** 선택합니다.

    1. "새 거래" 옵션을 클릭하여 파트너 센터 새 공동 판매 조회를 만듭니다.

    1. Salesforce CRM 환경에 로그인합니다.

    1. 기회 **열기로** 이동합니다. 이제 Microsoft 파트너 센터 만든 조회가 Salesforce CRM에서 동기화됩니다.

    1. 동기화된 조회를 선택하면 카드 보기 세부 정보가 채워집니다.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce 기회 페이지의 스크린샷.":::

>[!NOTE]
>**배포에 대한 도움이 필요하세요?**
>공동 판매 추천 커넥터 배포에 대한 지원을 받으시면 파트너 기술 컨설턴트를 참여시킬 수 있습니다. 성공적인 구현을 위한 배포 지원 및 모범 사례를 제공할 수 있습니다.
>
>자세한 내용은 [기술 사전 판매 및 배포 서비스 요청을 제출하는 방법을 참조하세요.](technical-benefits.md)

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)

- [공동 판매 기회 관리](manage-co-sell-opportunities.md)

- [파트너 센터 웹후크](/partner-center/develop/partner-center-webhooks)
