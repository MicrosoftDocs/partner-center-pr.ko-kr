---
title: Salesforce CRM 파트너 센터에 대 한 공동 판매 커넥터
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 조회를 Salesforce CRM과 동기화
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b96be195788ccc8b82aafd0bddb90dd34a672f9
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422449"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM용 공동 판매 커넥터 – 개요

### <a name="appropriate-roles"></a>적절한 역할

- 조회 관리자
- CRM에서 시스템 관리자 또는 시스템 사용자 지정자

파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다. 파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다. 공동 판매 커넥터를 사용 하 여 Microsoft 판매자를 참여 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 하는 새 공동 판매 참조를 만들 수 있습니다.  이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다. 파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안 모든 조회 작업을 수행할 수 있습니다. 

이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.

## <a name="before-you-install---pre-requisites"></a>설치 전-필수 구성 요소

|**토픽**   |**세부 정보**   |**연결**   |
|--------------|--------------------|------|
|Microsoft 파트너 네트워크 ID |유효한 MPN ID가 필요 합니다.|[MPN](https://partner.microsoft.com/) 에 조인 하려면|
|공동 판매 준비|I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.|[Microsoft와 판매](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|파트너 센터 계정|파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다. 커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.|[계정 관리](create-user-accounts-and-set-permissions.md)|
|파트너 센터 사용자 역할|커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.|[사용자 역할 및 권한 할당](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.|[Salesforce CRM에서 역할 할당](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|전원 자동화 흐름 계정|CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정 사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft 사용자 지정 필드에 대 한 Salesforce 패키지 설치 

파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 특정 조회 필드를 명확 하 게 식별 해야 합니다. 이 경계 파트너 판매자 팀에 게 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.

1. Salesforce에서 **메모** 를 활성화 하 고 기회 관련 목록에 추가 합니다. 
[참조](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. 다음 단계를 수행 하 여 **기회 팀** 을 활성화 합니다. 
    - 설치에서 **빠른 찾기** 상자를 사용 하 여 기회 팀 설정을 찾습니다.
    - 필요에 따라 설정을 정의 합니다.
[참조](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Salesforce에서 아래 패키지 설치 관리자를 사용 하 여 사용자 지정 필드 및 개체를 설치 합니다.
  
회사에 패키지를 설치 하려면 [여기](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) 로 이동 하세요.


참고: sandbox에를 설치 하는 경우 URL의 초기 부분을 다음으로 바꾸어야 합니다. http://test.salesforce.com

4. Salesforce에서 **기회** 관련 목록에 Microsoft 솔루션을 추가 합니다. 추가 된 후에는 **렌치** 아이콘을 클릭 하 고 속성을 업데이트 합니다.

## <a name="best-practice-test-before-you-go-live"></a>모범 사례: 라이브 상태로 전환 하기 전에 테스트

프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.

- 스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.

- 솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 실행 합니다.

- 스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.

- 성공할 경우 프로덕션 인스턴스에 대 한 관리 솔루션으로 가져옵니다.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM에 대 한 파트너 센터 조회 동기화 설치

1. [전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다. 그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.

2. 오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.

3. 왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.

4. 상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. 팝업 화면에서 **Salesforce에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. **지금 가져오기** 단추를 클릭 한 다음 **계속**합니다.

7. 그러면 Salesforce CRM 환경을 선택 하 여 응용 프로그램을 설치할 수 있는 페이지가 열립니다.  사용 약관에 동의 합니다.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="사용 가능한 CRMS":::

8. 그런 다음 **솔루션 관리** 페이지로 이동 합니다.  페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다. 파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다. 설치는 10-15 분 정도 걸립니다.

9. 설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다. **Salesforce에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 사용할 수 있습니다.

10. **Salesforce에 대 한 파트너 센터 조회 동기화를**선택 합니다. 다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 흐름":::



## <a name="configure-the-solution"></a>솔루션 구성

1. CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.

2. 오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.
3. 세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.
    - 조회 관리자 자격 증명이 있는 파트너 센터 사용자
    - 파트너 센터 이벤트
    - 솔루션에서 흐름을 자동화 하는 CRM admin
4. 왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.

5. **연결 만들기**를 클릭 하 여 연결을 만듭니다.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="연결 만들기":::

- 오른쪽 위 모서리의 검색 창에서 파트너 센터 조회 (미리 보기)를 검색 합니다.

- 조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.

-  다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.

- CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.

-  모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="연결 관찰":::

### <a name="edit-the-connections"></a>연결 편집

1. 솔루션 페이지로 돌아가서 **기본 솔루션**을 선택 합니다.  **모두**를 클릭 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="커넥터 편집 시작":::

2. 세 개의 점 아이콘을 선택 하 여 각 연결을 하나씩 편집 합니다. 관련 연결을 추가 합니다.

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

4. 변경 내용을 저장 하 고 **켜기**를 선택 합니다.

   파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.

5. **파트너 센터에서 SALESFORCE CRM (Insider preview)을**선택 합니다.

6. **편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때**를 선택 합니다.

7. **복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 복사":::

8. 이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행**을 선택 합니다.

9. 오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속**을 클릭 합니다.

10. 다음 세부 정보를 입력합니다.

    1. **Http 트리거 끝점**: 이전 단계에서 복사한 URL

    2. **등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"

    3. **기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)

11. **실행** 을 선택한 다음 완료를 선택 **합니다.**

이제 웹 후크를 수신 대기 하 여 이벤트를 만들고 업데이트할 수 있습니다.

## <a name="customize-synchronization-steps"></a>동기화 단계 사용자 지정

공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.

CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다. 전원 자동화 흐름을 사용자 지정할 수 있습니다. 필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.  CRM에 대 한 Microsoft 파트너 센터 매핑이 제공 되지만 CRM 환경에 따라 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.

각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다. 사용 가능한 사용자 지정의 예는 다음과 같습니다.

1. 파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다.

   1. 파트너 센터에서 Salesforce CRM (Insider Preview)을 선택 합니다.

   2. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   3. 선택 **(범위) 잠재 고객 또는 기회를 동기화**합니다.

2. 이벤트 만들기에 대 한 CRM 필드 매핑을 사용자 지정 하려면 **새 공유 기회 인지 여부**를 선택 합니다. **예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기**를 확장 합니다. 필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.

   1. 업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 "(범위) 잠재 고객 또는 기회 동기화" 단계를 클릭 합니다.

   2. **기회를 업데이트 하는 경우를**선택 합니다. **예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를**확장 합니다.  

   3. **예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.

3. 업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:

   1. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   2. **기회 동기화를 선택 (범위)** 합니다.

   3. 업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우**를 선택 합니다.

   4. **예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트**단계를 확장 합니다.

   필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.

4. 만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면

   1. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   2. **조회 동기화를 선택 (범위) 합니다.**

   3. 만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기**를 선택 합니다.

필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>종단 간 양방향 공동 판매 참조 동기화

전원 자동화 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.

### <a name="pre-requisites"></a>필수 구성 요소

파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다. 이 id는 판매자 팀에 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.

사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다. CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.

다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.

- **파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부

- **참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드

- **참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크

- Microsoft의 도움을 주는 **방법**: microsoft에서 조회에 필요한 도움말

- **제품**:이 기회와 관련 된 제품 목록

- **감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역

### <a name="scenarios"></a>에서는

1. CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:

   1. CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 Salesforce crm 환경에 로그인 합니다.

   2. Salesforce CRM 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 환경":::

   3. 이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.

       - "파트너 센터와 동기화": 예
       - "Microsoft의 도움을 주는 방법": 다음 옵션 중에서 선택 합니다.
       - 제품: 제품의 솔루션 Id

   4. **파트너 센터와의 동기화 기회 센터** 옵션을 **예**로 설정 했으면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다. 조회가 Salesforce CRM과 동기화 됩니다.

   5. "파트너 센터와 동기화" 옵션이 "예"로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.

   6. 파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.

2. Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:

    1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.

    2. 왼쪽 메뉴에서 **조회** 를 선택 합니다.

    3. "새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.

    4. Salesforce CRM 환경에 로그인 합니다.

    5. **오픈 기회**로 이동 합니다. Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 기회 화면":::

    6. 동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)

- [공동 판매 기회 관리](manage-co-sell-opportunities.md)

- [파트너 센터 웹후크](/partner-center/develop/partner-center-webhooks)