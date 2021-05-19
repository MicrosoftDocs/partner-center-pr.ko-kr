---
title: 인센티브 고객 제휴 문제
description: CPOR(클레임된 레코드 파트너) 고객 연결을 사용하여 작업할 때 제기되는 문제를 해결하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152174"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>CPOR(클레임된 레코드 파트너) 고객 연결 관련 문제

**적절한 역할:** 청구 관리자 | 전역 관리자 | 인센티브 관리자

아래 콘텐츠는 고객 연결을 사용할 때 제기될 수 있는 문제를 해결하는 데 도움이 됩니다.

## <a name="domain-tenant-mismatch"></a>도메인 테넌트 불일치

CPOR(Claim Partner of Record) 연결 클레임 흐름에서 고객 테넌트 ID 및 하위 도메인을 제공하라는 메시지가 표시됩니다. 일치하지 않는다는 오류가 표시되면 고객에게 문의하여 올바른 세부 정보가 있는지 확인합니다.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR 연결 클레임 흐름의 구독 오류

CPOR 연결 클레임 흐름에서 Business Applications 통해 클레임하려는 제품에 대한 구독을 제공하라는 메시지가 나타날 수 있습니다(Dynamics 365). 제품 및 구독이 클레임되는 테넌트의 구독에 속하는지 동적으로 확인하므로 구독을 요청합니다. 또한 구독이 활성/유예 상태인지 확인합니다.

오류가 발생하면 다음과 같은 여러 가지 이유가 있을 수 있습니다.

- 선택한 제품이 고객의 테넌트에 없음
- 제공된 구독이 Dynamics용이 아님
- 제공된 구독이 CSP용임
- 고객이 해당 구독에 대한 제품을 아직 활성화/프로비저닝하지 않았습니다.
- 구독이 이미 클레임됨
- 제공된 식별자가 구독 ID가 아닙니다.

구독의 정확도에 대한 질문이 있는 경우 고객과 협력하여 구독이 올바르고 올바른 테넌트 ID를 사용하고 있는지 확인합니다.

이 경로가 문제를 해결하지 못한 경우 [지원 에](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)문의하세요.

## <a name="when-subscriptions-will-be-available-to-claim"></a>구독을 클레임할 수 있는 경우

구독에 대해 클레임할 때 구독이 아직 프로비전되지 않은 경우 오류가 발생합니다. CPOR 플랫폼에서 구독을 선택하고 클레임할 수 있도록 하려면 고객이 구독을 사용할 수 있도록 몇 가지 단계를 수행해야 합니다. 구독을 클레임하려고 할 때 오류가 발생하면 고객에게 문의하여 프로비전되었고 클레임하는 구독이 올바른지 확인합니다. 이 경로를 이미 이용한 경우 [지원 에 문의합니다.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>어떤 활동을 선택해야 합니까?

CPOR 클레임 플랫폼을 사용하면 Business Applications 및 Microsoft 365 솔루션 영역과 관련된 CPOR 연결 클레임을 허용합니다. 각 솔루션 영역에 적용할 수 있는 활동은 다음과 같습니다. 나중에 회수할 필요가 없도록 설명에 따라 올바른 활동을 선택합니다. 잘못된 활동으로 클레임하면 자격 및 인센티브 소득이 누락됩니다.


| 솔루션 영역 | 작업 | 적용할 수 있는 경우 |
| ------ | ----------- | ----------- |
| 비즈니스 애플리케이션      | 사전 판매   | 적격 제품 구매에 영향을 주고 사전 판매 인센티브에 신청할 것인지 선택합니다. 이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용됩니다. |
|    |  사용량  | 적격 워크로드의 채택 및 사용을 유도하고 사용 인센티브에 적용할 것인지 선택합니다. 이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용됩니다. |
|    | 수익 연결   | 비즈니스 영향 주체로 적합한 제품을 선택하는 데 영향을 주었는지 여부를 선택합니다. 이 옵션은 인센티브 지급이 아닌 수익 연결 전용입니다. 이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용됩니다.   |
| Microsoft 365   | 사용량   | 적격 워크로드의 채택 및 사용을 유도하고 사용 인센티브에 적용할 것인지 선택합니다. |

## <a name="which-mpn-do-i-choose"></a>어떤 MPN을 선택해야 합니까?

CPOR 연결 클레임 흐름에서 최종 고객에 대해 클레임하는 작업에 연결되어야 하는 회사 MPN을 선택하라는 메시지가 표시됩니다. 회사에는 여러 MPNs가 있을 수 있으며, 그 중 일부는 동기 프로그램에 등록 될 수 있으며, 다른 일부는 FRP FastTrack 같은 파트너 유형과 연결 되어 있을 수 있습니다. CPOR association 클레임 흐름은 동기 프로그램에 등록 된 MPNs를 식별 하지만 MPN 특정 파트너 유형인 경우에는 알 수 없습니다. 나중에 회수할 필요가 없도록 올바른 MPN를 선택 하는 것이 중요 합니다. 잘못 된 MPN를 사용 하 여 주장 하면 자격 및 동기 소득이 누락 될 수 있습니다.

사용할 MPN를 모르는 경우 전역 관리자에 게 문의 하세요.

사용 하려는 MPN이 등록 되지 않은 경우에는 [성과급 개요 탭](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (로그인 필요)에서 관리할 수 있습니다.

## <a name="choosing-a-product-vs-entering-a-subscription"></a>제품 선택 및 구독 입력

Dynamics 제품이 요청 및 승인 되 면 파트너는 CPOR association 클레임 자체에서 구독 ID를 볼 수 있습니다. 이 구독을 요청 하면 활성 또는 유예 상태 이지만 구독이 종료 되는 시간이 있을 수 있으며 새 구독은 별도의 CPOR 연결 클레임에서 요청 해야 합니다.

## <a name="competing-claims"></a>경쟁 하는 클레임

다른 파트너와 이미 연결 되어 있는 고객 및 해당 제품에 대 한 CPOR association 클레임을 만드는 경우 클레임은 중재를 통해 수행 됩니다.

1. 파트너가 새 고객 연결을 만들면 Microsoft가 정확성을 보장하기 위해 제공된 연결 및 실행 증명의 세부 정보를 확인합니다.

2. 사용자와 다른 파트너가 동일한 고객 및 제품/작업을 클레임 하는 경우 Microsoft는 각 파트너의 실행 설명서를 검토 하 여 승인할 파트너를 결정 합니다.

3. 두 파트너 모두에서 추가 정보를 요청할 수 있으며,이로 인해 연결 요청 처리가 지연 될 수 있습니다.

4. CPOR association 클레임은 계속 해 서 5 영업일 이내에 검토 됩니다. 단, 그 상태는 더 오랜 기간 동안 _검토_ 하는 것으로 유지 될 수 있습니다. 이 시나리오는 Microsoft가 현재 제품/워크 로드를 소유 하 고 있는 파트너와 함께 작업 하는 경우에 발생할 수 있습니다. 해당 하는 경우에는 클레임의 설명 섹션에서 알림이 표시 됩니다. 

>[!IMPORTANT]
>CPOR PoE(연결 실행 증명)를 확인하기 위해 추가 정보가 필요한 경우 CPOR 연결 클레임 주석 섹션을 통해 연락을 드립니다.

## <a name="next-steps"></a>다음 단계

- [인센티브 시작](incentives-get-started-intro.md)
