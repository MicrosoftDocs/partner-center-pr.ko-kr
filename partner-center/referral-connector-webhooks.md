---
title: 웹 후크를 사용 하 여 리소스 변경 이벤트 가져오기
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 웹 후크 Api를 사용 하 여 조회 리소스 변경이 발생 하는 경우를 확인 합니다.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 조회, webhook api, 리소스 변경 이벤트
ms.localizationpriority: medium
ms.openlocfilehash: 4e1eb2e9bd8ceb4f8c4bf43684305504c8594e5c
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145087"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook Api를 사용 하 여 리소스 변경 이벤트 등록

### <a name="appropriate-roles"></a>적절한 역할

- 조회 관리자
- Dynamics 365 CRM 또는 Salesforce CRM에 대 한 시스템 관리자 또는 시스템 사용자 지정자


파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다. 이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.

>[!NOTE]
>이 항목에서는 Dynamics 365 CRM 및 Salesforce CRM의 Webhook Api에 대해 설명 합니다.

1. Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.

2. (A.)에 대 한 연결을 추가 합니다. 조회 관리자 자격 증명이 있는 파트너 센터 사용자 (b.) 아래 강조 표시 된 파트너 센터 이벤트

![트리거](images/cosellconnectors/triggerflow.png)

3. 이러한 업데이트를 수행 하면 다음과 같이 표시 됩니다.

![Webhook](images/cosellconnectors/webhook1.png)

4. 변경 내용을 저장 하 고 **켜기**를 선택 합니다. 

파트너 센터 웹 후크가 파트너 센터 및 CRM 시스템의 IP 공동 판매/독립적인 조회 개체에서 이벤트 변경 내용을 수신 대기 하도록 설정 하려면 다음 단계를 수행 합니다.

5. **파트너 센터에서 Dynamics 365 (Insider preview)** 또는 **파트너 센터를 Salesforce (insider preview)** 로 선택 합니다.

6. **편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때**를 선택 합니다.

7. **복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.

![URL 복사](images/cosellconnectors/copyurl.png)

8. 이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행**을 선택 합니다.

9. 오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속**을 클릭 합니다.

10. 다음 세부 정보를 입력합니다. 

    a. **Http 트리거 끝점**: 이전 단계에서 복사한 URL

    b. **등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"

    다. **기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)

이제 webhook에서 변경 내용 (이벤트 만들기 및 업데이트)을 수신할 수 있습니다. 

11. **실행** 을 선택한 다음 완료를 선택 **합니다.**

 ## <a name="customize-synchronization-steps"></a>동기화 단계 사용자 지정

공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.

CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다. 전원 자동화 흐름을 사용자 지정할 수 있습니다. 필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.  CRM에 대 한 Microsoft 파트너 센터 매핑을 제공 하지만 CRM 환경을 기반으로 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.

각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다. 사용 가능한 사용자 지정의 예는 다음과 같습니다.

1. 파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다. 

    a. 파트너 센터에서 Dynamics 365 (Insider Preview) 또는 파트너 센터를 Salesforce (Insider preview)로 선택 합니다.

    b. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

    다. 선택 **(범위) 잠재 고객 또는 기회를 동기화**합니다.

2. 만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **새 공유 기회 인지 여부**를 선택 합니다. **예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기**를 확장 합니다. 필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.

    d. 업데이트 이벤트의 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 "(범위) 잠재 고객 또는 기회 동기화" 단계를 클릭 합니다.

    e. **기회를 업데이트 하는 경우를**선택 합니다. **예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를**확장 합니다.  

    f. **예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.
       
3. 업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:

    a. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

    b. **기회 동기화를 선택 (범위)** 합니다.

    다. 업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우**를 선택 합니다. 

    d. **예 인 경우** 하위 단계을 선택 하 고 **기회 데이터를 사용 하 여 조회 업데이트**단계를 확장 합니다.

필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.

4. 만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면

   a. **편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.

   b. **조회 동기화를 선택 (범위) 합니다.**

   다. 만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기**를 선택 합니다. 

필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>종단 간 양방향 공동 판매 참조 동기화

전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하 고 나면 Dynamics 365 또는 Salesforce와 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.

### <a name="pre-requisites"></a>필수 구성 요소

파트너 센터 및 Dynamics 365 CRM에서 또는 파트너 센터와 Salesforce CRM 간에 조회를 동기화 하려면 전원 자동화 솔루션이 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다. 이를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유할 조회를 결정할 수 있습니다.

사용자 지정 필드 집합은 Dynamics 365 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다. CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.

다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.

- **파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부

- **참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드

- **참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크

- **Microsoft에서 microsoft의 도움**을 받아야 하는 방법: microsoft에서 조회에 대 한 도움말

- **제품**:이 기회와 관련 된 제품 목록

- **감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역

### <a name="scenarios"></a>에서는

1. CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:

    a. CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 DYNAMICS 365 crm 환경에 로그인 합니다.

    b. Dynamics 365 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.

   ![기회](images/cosellconnectors/opportunity.png)

    다. 이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.

    - "파트너 센터와 동기화": 예

    - "Microsoft의 도움을 주는 방법": 다음 중에서 선택 합니다.

    ![도움말 선택](images/cosellconnectors/help.png)

    - 제품: 제품의 솔루션 Id

    d. **파트너 센터** 옵션을 **예**로 설정 하 여 Dynamics 365에서 통합 기회가 만들어지면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다. 사용자의 조회가 Dynamics 365와 동기화 됩니다.

    e. 따라서 "파트너 센터와 동기화" 옵션을 "예"로 설정 하는 기회에 대해 Dynamics 365 CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정에서 동기화 됩니다.

    f. 파트너 센터와 성공적으로 동기화 되는 기회는 Dynamics 365의 ✔ 아이콘으로 식별 됩니다.

2. Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Dynamics 365 환경에서 동기화 할 때 조회 동기화: 

    a. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.

    b. 왼쪽 메뉴에서 **조회** 를 선택 합니다.

    다. "새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.

    d. Dynamics 365 CRM 환경에 로그인 합니다. 

    e. **오픈 기회**로 이동 합니다. Microsoft Partner Center에서 만든 조회는 이제 Dynamics 365 CRM에서 동기화 됩니다.

    f. 동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.

 ### <a name="next-steps"></a>다음 단계

- [Microsoft Power 자동화 플랫폼에 대 한 자세한 정보](https://docs.microsoft.com/power-automate/)

- [파트너 센터 webhook 이벤트](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [잠재 고객 관리](manage-leads.md)

- [공동 판매 기회 관리](manage-co-sell-opportunities.md)
