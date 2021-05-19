---
title: Salesforce CRM 파트너 센터 대한 공동 판매 커넥터
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 조회를 Salesforce CRM과 동기화합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148417"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM용 공동 판매 커넥터 – 개요

**적절한 역할:** 조회 관리자 | CRM의 시스템 관리자 또는 시스템 사용자 지정자

파트너 센터 공동 판매 커넥터를 사용하면 판매자가 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다. 공동 판매 거래를 관리하는 데 파트너 센터 사용하도록 학습할 필요가 없습니다. 공동 판매 커넥터를 사용하여 새 공동 판매 추천을 만들어 Microsoft 판매자에게 참여시키고, Microsoft 판매자로부터 추천을 받고, 추천을 수락/거부하고, 거래 가치와 같은 거래 데이터를 수정하고, 종료 날짜를 만들 수 있습니다.  이러한 공동 판매 거래에 대한 Microsoft 판매자의 업데이트를 받을 수도 있습니다. 파트너 센터 대신 선택한 CRM 내에서 작업하는 동안 모든 조회 작업을 수행할 수 있습니다. 

솔루션은 Microsoft Power Automate Solution을 기반으로 하며 파트너 센터 API를 사용합니다.

## <a name="before-you-install---pre-requisites"></a>설치하기 전에 - 필수 조건

|**토픽**   |**세부 정보**   |**연결**   |
|--------------|--------------------|------|
|Microsoft 파트너 네트워크 ID |유효한 MPN ID가 필요합니다.|[MPN을](https://partner.microsoft.com/) 조인하려면|
|공동 판매 준비|IP/서비스 솔루션은 공동 판매 준비가 되어 있어야 합니다.|[Microsoft로 판매](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|파트너 센터 계정|파트너 센터 테넌트와 연결된 MPN ID는 공동 판매 솔루션과 연결된 MPN ID와 동일해야 합니다. 커넥터를 배포하기 전에 파트너 센터 Portal에서 공동 판매 추천을 볼 수 있는지 확인합니다.|[계정 관리](create-user-accounts-and-set-permissions.md)|
|파트너 센터 사용자 역할|커넥터를 설치하고 사용할 직원은 조회 관리자여야 합니다.|[사용자 역할 및 권한 할당](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.|[Salesforce CRM에서 역할 할당](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow 계정|CRM 시스템 관리자 또는 시스템 사용자 지정자의 활성 [Power Automate](https://flow.microsoft.com) 계정입니다. 해당 사용자는 설치 전에 한 번 이상 [Power Automate](https://flow.microsoft.com) 로그인해야 합니다.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft 사용자 지정 필드용 Salesforce 패키지 설치 

파트너 센터 및 Salesforce CRM에서 조회를 동기화하려면 Power Automate 솔루션이 Microsoft 특정 조회 필드를 명확하게 식별해야 합니다. 이 구분은 파트너 판매자 팀이 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있는 기능을 제공합니다.

1. Salesforce에서 **메모를** 활성화하고 기회 관련 목록에 추가합니다. 
[참조](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. 다음 단계에 따라 **기회 팀을** 활성화합니다. 
    - 설치 프로그램에서 **빠른 찾기** 상자를 사용하여 기회 팀 설정을 찾습니다.
    - 필요에 따라 설정을 정의합니다.
[참조](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Salesforce에서 패키지 설치 관리자 를 사용하여 사용자 지정 필드 및 개체를 [설치합니다.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) 이 방법을 사용하여 모든 회사에 패키지를 설치합니다.

>[!NOTE]
>샌드박스에 설치하는 경우 URL의 초기 부분을 로 바꾸어야 합니다. http://test.salesforce.com

4. Salesforce에서 **기회** 관련 목록에 Microsoft 솔루션을 추가합니다. 추가되면 **렌치** 아이콘을 선택하고 속성을 업데이트합니다.

## <a name="best-practice-test-before-you-go-live"></a>모범 사례: 라이브로 진행하기 전에 테스트

프로덕션 환경에서 Power Automate 솔루션을 설치, 구성 및 사용자 지정하기 전에 준비 CRM 인스턴스에서 솔루션을 테스트해야 합니다.

- 스테이징 환경/CRM 인스턴스에 Microsoft Power Automate 솔루션을 설치합니다.

- 솔루션의 복사본을 만들고 스테이징 환경에서 구성 및 Power Automate 흐름 사용자 지정을 실행합니다.

- 스테이징/CRM 인스턴스에서 솔루션을 테스트합니다.

- 성공하면 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM에 대한 파트너 센터 조회 동기화 설치

1. [Power Automate](https://flow.microsoft.com) 이동하여 오른쪽 위 모서리에서 **환경을** 선택합니다. 그러면 사용 가능한 CRM 인스턴스가 표시됩니다.

2. 오른쪽 위 모서리의 드롭다운에서 적절한 CRM 인스턴스를 선택합니다.

3. 왼쪽 탐색 모음에서 **솔루션을** 선택합니다.

4. 위쪽 메뉴에서 **AppSource 열기** 링크를 선택합니다.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. 팝업 화면에서 **salesforce에 대한 파트너 센터 조회 커넥터를** 검색합니다.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. 지금 **받기** 단추를 선택한 **다음, 계속을** 선택합니다.

7. 그러면 Salesforce CRM 환경을 선택하여 애플리케이션을 설치할 수 있는 페이지가 열립니다.  약관에 동의합니다.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="사용 가능한 CRM":::

8. 그런 다음 솔루션 관리 페이지로 **안내됩니다.**  페이지 아래쪽의 화살표 단추를 사용하여 "파트너 센터 조회"로 이동합니다. 파트너 센터 조회 솔루션 옆에 **설치가 예약되어** 있어야 합니다. 설치하는 데 10-15분이 걸립니다.

9. 설치가 완료되면 [Power Automate](https://flow.microsoft.com) 다시 이동하고 왼쪽 탐색 영역에서 **솔루션을** 선택합니다. **Salesforce에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 사용할 수 있습니다.

10. **Salesforce에 대 한 파트너 센터 조회 동기화를** 선택 합니다. 다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 흐름":::



## <a name="configure-the-solution"></a>솔루션 구성

1. CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.

2. 오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.
3. 세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.
    - 조회 관리자 자격 증명이 있는 파트너 센터 사용자
    - 파트너 센터 이벤트
    - 솔루션에서 흐름을 자동화 하는 CRM admin
4. 왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.

5. **연결 만들기** 를 클릭 하 여 연결을 만듭니다.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="연결 만들기":::

- 오른쪽 위 모서리의 검색 창에서 파트너 센터 조회 (미리 보기)를 검색 합니다.

- 조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.

-  다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.

- CRM 관리자 사용자에 대 한 Salesforce에 대 한 연결을 만듭니다.

-  모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="연결 관찰":::

### <a name="edit-the-connections"></a>연결 편집

1. 솔루션 페이지로 돌아가서 **기본 솔루션** 을 선택 합니다.  **모두** 를 클릭 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="커넥터 편집 시작":::

2. 세 개의 점 아이콘을 선택 하 여 각 연결을 개별적으로 편집 합니다. 관련 연결을 추가 합니다.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="커넥터 편집":::

3. 다음 순서로 흐름을 설정 합니다.

- 파트너 센터 Webhook 등록 (Insider Preview)
- 공동 판매 참조-Salesforce를 파트너 센터 (Insider Preview)에 만듭니다.
- 파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매
- 파트너 센터를 Salesforce로 (Insider Preview)
- Salesforce에서 파트너 센터로 (Insider Preview)
- Salesforce 기회와 파트너 센터 간 (Insider Preview)
- 파트너 센터 (Insider Preview)에 대 한 Salesforce Microsoft 솔루션

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook Api를 사용 하 여 리소스 변경 이벤트 등록

파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다. 이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.

1. Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.

2. 아래 강조 표시 된 대로 조회 관리자 자격 증명 (b.) 파트너 센터 이벤트를 사용 하 여 (a.) 파트너 센터 사용자에 대 한 연결을 추가 합니다.

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="트리거":::

3. 이러한 업데이트를 만들면 다음과 같이 표시 됩니다.

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 변경 내용을 저장 하 고 **켜기** 를 선택 합니다.

   파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.

5. **Salesforce CRM에 파트너 센터(Insider Preview)** 를 선택합니다.

6. **편집** 아이콘을 선택하고 **HTTP 요청을 받은 경우를** 선택합니다.

7. **복사** 아이콘을 선택하여 제공된 HTTP POST URL을 복사합니다.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 복사":::

8. 이제 "파트너 센터 Webhook 등록(Insider Preview)" Power Automate 흐름을 선택하고 **실행을** 선택합니다.

9. 오른쪽 창에서 "흐름 실행" 창이 열리는지 확인하고 **계속을** 선택합니다.

10. 다음 세부 정보를 입력합니다.

    1. **Http 트리거 엔드포인트:** 이전 단계에서 복사한 URL입니다.

    2. **등록할 이벤트:**"조회가 생성됨" 및 "조회 업데이트됨"

    3. **기존 트리거 엔드포인트(있는 경우)를 덮어씁니다.** 예(기존 엔드포인트를 덮어씁니다.)

11. **실행을** 선택한 **다음, 완료를 선택합니다.**

이제 webhook는 이벤트를 만들고 업데이트하기 위해 수신 대기할 수 있습니다.

## <a name="customize-synchronization-steps"></a>동기화 단계 사용자 지정

파트너 센터 CRM 시스템 간에 공동 판매 조회가 동기화되면 파트너 센터 PC에서 동기화되는 필드가 여기에 나열됩니다.

CRM 시스템은 종종 고도로 사용자 지정됩니다. Power Automate 흐름을 사용자 지정할 수 있습니다. 필드 매핑 가이드에 따라 필요한 경우 Power Automate 흐름의 단계를 적절하게 변경합니다.  CRM에 대한 Microsoft 파트너 센터 매핑이 제공되지만 CRM 환경에 따라 필드를 추가로 사용자 지정하도록 선택할 수 있습니다.

각 Power Automate 흐름의 여러 단계를 필요에 따라 사용자 지정할 수 있습니다. 다음은 사용 가능한 사용자 지정의 예입니다.

1. crm 조회 동기화에 대한 파트너 센터 만들기 또는 업데이트 이벤트에 대한 필드를 사용자 지정하려면 다음을 수행합니다.

   1. Salesforce CRM에 파트너 센터 선택합니다(Insider Preview).

   2. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   3. 선택 **(범위) 잠재 고객 또는 기회를 동기화** 합니다.

2. 이벤트 만들기에 대 한 CRM 필드 매핑을 사용자 지정 하려면 **새 공유 기회 인지 여부** 를 선택 합니다. **예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기** 를 확장 합니다. 필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.

   1. 업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 "(범위) 리드 또는 기회 동기화" 단계를 선택 합니다.

   2. **기회를 업데이트 하는 경우를** 선택 합니다. **예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를** 확장 합니다.  

   3. **예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.

3. 업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:

   1. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   2. **기회 동기화를 선택 (범위)** 합니다.

   3. 업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우** 를 선택 합니다.

   4. **예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트** 단계를 확장 합니다.

   필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.

4. 만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면

   1. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   2. **조회 동기화를 선택 (범위) 합니다.**

   3. 만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기** 를 선택 합니다.

필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>엔드투엔드 양방향 공동 판매 조회 동기화

Power Automate 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간의 공동 판매 조회 동기화를 테스트할 수 있습니다.

### <a name="pre-requisites"></a>필수 구성 요소

파트너 센터 및 Salesforce CRM에서 조회를 동기화하려면 Power Automate 솔루션이 Microsoft 특정 조회 필드를 명확하게 구분해야 합니다. 이 ID를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있습니다.

사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다. CRM 관리자 사용자는 **기회** 사용자 지정 필드를 사용하여 별도의 CRM 섹션을 만들어야 합니다.

다음 사용자 지정 필드는 CRM 섹션의 일부여야 합니다.

- **파트너 센터 동기화:** 기회를 Microsoft 파트너 센터 동기화할지 여부

- **조회 식별자:** Microsoft 파트너 센터 조회에 대한 읽기 전용 식별자 필드입니다.

- **조회 링크:** Microsoft 파트너 센터 조회에 대한 읽기 전용 링크입니다.

- **Microsoft 도움말** 방법: 추천을 위해 Microsoft에서 필요한 도움말

- **제품:** 이 기회와 관련된 제품 목록

- **감사:** 파트너 센터 조회와 동기화하기 위한 읽기 전용 감사 내역

### <a name="scenarios"></a>시나리오:

1. CRM에서 조회를 만들거나 업데이트하고 파트너 센터 동기화할 때 조회 동기화:

   1. CRM의 **기회** 섹션에서 가시성이 있는 사용자로 Salesforce CRM 환경에 로그인합니다.

   2. Salesforce CRM 환경에서 "새 기회"를 만들 때 다음 섹션이 있는지 확인합니다.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 환경":::

   3. 이 기회를 Microsoft 파트너 센터 동기화하려면 카드 보기에서 다음 필드를 설정해야 합니다.

       - "파트너 센터 동기화": 예
       - "Microsoft의 도움을 주는 방법": 다음 옵션 중에서 선택 합니다.
       - 제품: 제품의 솔루션 Id

   4. **파트너 센터와의 동기화 기회 센터** 옵션을 **예** 로 설정 했으면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다. 조회가 Salesforce CRM과 동기화 됩니다.

   5. "파트너 센터와 동기화" 옵션이 "예"로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.

   6. 파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.

2. Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:

    1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.

    2. 왼쪽 메뉴에서 **조회** 를 선택 합니다.

    3. "새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.

    4. Salesforce CRM 환경에 로그인 합니다.

    5. **오픈 기회** 로 이동 합니다. Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 기회 화면":::

    6. 동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)

- [공동 판매 기회 관리](manage-co-sell-opportunities.md)

- [파트너 센터 웹후크](/partner-center/develop/partner-center-webhooks)
