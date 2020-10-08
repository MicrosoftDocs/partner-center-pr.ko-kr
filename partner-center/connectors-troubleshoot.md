---
title: 공동 판매 추천 커넥터 문제 해결
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 공동 판매 커넥터 문제를 해결 하는 방법에 대 한 FAQ입니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 312ff9155ab4c2d84fb38bb6ccd093505e628832
ms.sourcegitcommit: df7643f3b7978e164e419e447a4dc3c163cb3bd2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/08/2020
ms.locfileid: "91844657"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>공동 판매 추천 커넥터 문제 해결

**적용 대상:**

- 파트너 센터
- Dynamics 365 CRM
- Salesforce CRM

**적절한 역할**

- 조회 관리자
- CRM에서 시스템 관리자 또는 시스템 사용자 지정자

 ## <a name="questions-and-answers-about-pre-requisites"></a>필수 조건에 대 한 질문과 대답

1. 사용자 환경에 대 한 평가판 공동 판매 조회 커넥터 솔루션을 사용할 수 있나요?

테스트/스테이징 환경을 사용할 경우 평가판 솔루션을 선택할 수 있습니다. 유료 버전의 커넥터는 AppSource에서 미국 $15/월에 사용할 수 있습니다. 유료 연결을 사용 하면 하루에 10K API 호출을 받게 됩니다. 커넥터는 파트너 센터 조회 Api 위에 있는 래퍼입니다. 커넥터 솔루션이 파트너 센터나 CRM 쪽의 기회에서 **만들기** 또는 **업데이트** 이벤트에 대해 실행 될 때마다 API 호출이 수행 됩니다.

2. CRM 환경에서 섹션을 만드는 데 필요한 역할은 무엇 인가요?

시스템 관리자 또는 시스템 사용자 지정자 인 사용자는 모든 사용자에 대 한 변경 내용을 적용할 수 있습니다. 그러나 모든 앱 사용자는 시스템을 개인 설정 하 고 일부 사용자 지정 항목을 다른 사용자와 공유할 수도 있습니다. 

3. 파트너 판매자는 파트너 센터에서 작업 하는 데 특별 한 역할이 필요 한가요?
 
파트너 판매자에 게는 "조회 관리자" 역할을 할당 해야 합니다. 자세한 내용은 다음을 참조 하십시오. [사용 권한 개요) (사용자-계정 및 설정-권한)

4. CRM 환경에서 먼저 설정 해야 하는 필드는 무엇입니까? 

• 통화가 사용자의 위치에 적합 하 고 CRM 환경에서 정확 하 게 사용 되는지 확인 합니다. • 영업 팀이 crm 환경에 CRM 사용자로 나열 되어야 합니다.

5. 전원 자동화 환경 만들기에 필요한 필수 구성 요소는 무엇 인가요?

전원 자동화 환경을 사용 하려면 다음이 필요 합니다.

- 전원 자동화 라이선스가 필요 합니다.
- 최소 1gb의 저장소가 필요 합니다.

6.  Salesforce 커넥터 솔루션을 사용 하려면 Dynamics 365 구독이 필요 한가요?

Salesforce 커넥터 솔루션은 다른 CRM 시스템과의 동기화를 지 원하는 "Dynamics Flow" 유형입니다. 이 솔루션에는 Dynamics 365 인스턴스 또는 구독이 필요 하지 않습니다. Salesforce 솔루션을 설치 하는 동안 회사에서 기존 CD 환경을 사용한 드롭다운이 표시 될 수 있습니다. 해당 환경을 선택 해야 합니다. 또한 "로그인 한 사용자에 게 연결 된 Dynamics 365 조직을 찾을 수 없습니다." 라는 오류 메시지가 표시 되 면 커넥터에 대 한 새 환경을 만들어야 합니다.

## <a name="questions-and-answers-about-configuration"></a>구성에 대 한 질문과 대답

1. 전원 자동화 플랫폼에서 흐름을 활성화 하는 동안 다음 오류가 발생 하는 경우 어떻게 해야 하나요?

오류: ' {"error": {"code": "WorkflowTriggerNotFound", "message": "workflow ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' 트리거 ' manual ' 트리거를 찾을 수 없습니다."}} ' 오류로 인해 Azure Resource Manager 요청이 실패 했습니다. 

다음 문제 해결 단계를 수행 합니다.

- CD 연결을 삭제 한 다음 CD 연결을 다시 만듭니다.
- 자식 흐름을 끄고 설정 
- 솔루션을 삭제 한 다음 솔루션을 다시 설치 합니다. 

2.  전원 자동화 플랫폼에서 파트너 센터 커넥터를 추가 하는 동안 "로그인" 오류가 발생 하는 경우 어떻게 해야 하나요?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="로그인을 요구 하는 오류 메시지":::

다음 문제 해결 단계를 수행 합니다.

- 파트너 센터 자격 증명을 사용 하 여 흐름 환경에 한 번 로그인 합니다 (flow.microsoft.com).


3. 전원 자동화 플랫폼에서 파트너 센터를 CRM 흐름으로 활성화 하는 동안 다음과 같은 오류가 표시 되 면 어떻게 해야 하나요?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="로그인을 요구 하는 오류 메시지":::

다음 문제 해결 단계를 수행 합니다.

- 파트너 센터를 CRM flow로 활성화 하기 전에 먼저 다음 두 자식 흐름을 활성화 합니다.
      - 파트너 센터-CRM-도우미 (Insider Preview)
      - 파트너 센터 Microsoft에서 CRM (Insider Preview)에 대 한 조회 업데이트를 공동 판매

4. 흐름을 편집 하려고 할 때 흐름에 대 한 연결을 추가할 수 없는 경우 어떻게 해야 하나요?

흐름이 실행 되는 동안 흐름에 연결을 추가 하 고 각 흐름에 개별적으로 추가 합니다.  흐름을 편집 하는 동안 연결을 추가 하는 대화 상자가 자동으로 열리지 않는 경우 흐름의 각 단계와 하위 단계를 개별적으로 편집할 수 있습니다.

- 각 흐름을 선택 하 고 개별적으로 편집 합니다.
- 흐름의 모든 단계를 확장 합니다. 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="로그인을 요구 하는 오류 메시지":::

- 연결을 연결 하 고 연결을 추가 하 라는 경고 아이콘이 표시 되는 단계를 선택 합니다. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="로그인을 요구 하는 오류 메시지":::


5. 공동 판매 된 조회 커넥터 솔루션의 흐름이 켜지 지 않으면 어떻게 해야 하나요?

A. 전원 자동화에서 다음과 같은 순서로 흐름을 편집 하 고 올바른 연결을 사용 하도록 업데이트 해야 합니다.

- 파트너 센터 Webhook 등록 (Insider Preview)
- 공동 판매 참조-Salesforce를 파트너 센터 (Insider Preview)에 만듭니다.
- 파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매
- 파트너 센터를 Salesforce로 (Insider Preview)
- Salesforce에서 파트너 센터로 (Insider Preview)
- Salesforce 기회와 파트너 센터 간 (Insider Preview)
- 파트너 센터 (Insider Preview)에 대 한 Salesforce Microsoft 솔루션

 B. 각 흐름에 대해 **실행만 사용자** 옵션을 선택 합니다. **실행 전용 사용자가 제공 하**는 대신 **연결 사용** 을 선택 합니다.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="로그인을 요구 하는 오류 메시지":::


C. 아래에서 언급 한 흐름을 활성화 합니다.

 - 파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매

- Salesforce에서 파트너 센터로 (Insider Preview)

    
D. 나머지 흐름을 모두 활성화 합니다.

E. Flow 파트너 센터 Webhook 등록에서 **실행**을 선택 합니다. **파트너 센터** 의 첫 번째 작업에서 Salesforce 흐름으로의 **http url** 을 제공 합니다. **등록할 이벤트** 에서 네 가지 옵션을 모두 선택 하 고 덮어쓰기에 대해 **예** 를 선택 합니다.

## <a name="questions-and-answers-about-runmaintenance"></a>실행/유지 관리에 대 한 질문과 대답

1. 전원 자동화 흐름을 실행 하는 동안 오류가 발생 하는 경우 문제를 어떻게 해결 하나요?

전원 자동화 흐름이 기대한 대로 실행 되도록 하 고 실행 중에 오류를 해결 하려면 [흐름 오류 수정](/power-automate/fix-flow-failures)을 참조 하세요.

2. 파트너 센터 또는 CRM 환경에서 제대로 동기화 되지 않는 조회가 표시 되는 경우 어떻게 해야 하나요?
 
조회 동기화 상태를 확인 하려면 **감사**를 선택 합니다. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="로그인을 요구 하는 오류 메시지":::

다음 조건이 충족 되는지 확인 합니다.

- 솔루션 id는 기회의 일부로 제공 됩니다.

- 두 자로 된 국가 코드가 필요 합니다.

- Microsoft의 도움을 기회에 대해 선택 하는 경우 고객 연락처 정보가 필요 합니다.

3. 조회가 양방향를 동기화 하는지 확인 하는 방법

다음 단계를 수행합니다.

- 파트너 판매자는 CRM 섹션에서 **파트너 센터와 동기화** 를 사용 하도록 설정 했는지 확인 해야 합니다.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="로그인을 요구 하는 오류 메시지" 또는 "손실"로 인해 실수로 닫히지 않았는지 확인 합니다.

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)
 
- [공동 판매 기회 관리](manage-co-sell-opportunities.md)