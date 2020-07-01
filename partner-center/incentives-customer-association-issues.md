---
title: 고객 연결 문제
description: 요청 받은 레코드 파트너 (CPOR) 고객 연결을 사용할 때 발생 하는 문제를 해결 하는 방법을 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: e5ad52e128aba9884fafea3900a3c03d31d4868f
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719422"
---
# <a name="customer-association-issues"></a>고객 연결 문제

적용 대상:

- 파트너 센터

아래 콘텐츠를 통해 고객 연결을 사용할 때 발생 하는 문제를 해결할 수 있습니다.

적절 한 역할:

- 청구 관리자
- 글로벌 관리자
- 인센티브 관리자

## <a name="domain-tenant-mismatch"></a>도메인-테 넌 트 불일치

요청 받은 레코드 파트너 (CPOR) 연결 클레임 흐름에서 고객 테 넌 트 ID 및 하위 도메인을 제공 하 라는 메시지가 표시 됩니다. 일치 하지 않는다는 오류 메시지가 표시 되 면 고객에 게 문의 하 여 올바른 세부 정보를 확인 합니다.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR association 클레임 흐름의 구독 오류

CPOR association 클레임 흐름에서 Business Applications (Dynamics 365)를 통해 클레임 하려는 제품에 대 한 구독을 제공 하 라는 메시지가 표시 될 수 있습니다. 제품 및 구독이에 대해 요청 되는 테 넌 트에 속하는지 여부를 동적으로 확인 하는 중 이므로 구독을 요청 합니다. 구독이 활성/유예 상태 인지 확인 하 고 있습니다.

오류가 발생 하는 경우 다음과 같은 여러 가지 이유가 있을 수 있습니다.

- 선택한 제품이 고객의 테넌트에 없음
- 제공 된 구독은 Dynamics에 대해 제공 되지 않습니다.
- 제공된 구독이 CSP용임
- 고객은 해당 구독에 대 한 제품을 아직 활성화/프로 비전 하지 않았습니다.
- 구독이 이미 클레임됨
- 제공 된 식별자가 구독 ID가 아닙니다.

구독의 정확성에 대 한 질문이 있는 경우 고객과 협력 하 여 구독이 올바르고 올바른 테 넌 트 ID를 사용 하 고 있는지 확인 합니다.

이 경로에서 문제가 해결 되지 않으면 [지원](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)담당자에 게 문의 하세요.

## <a name="when-subscriptions-will-be-available-to-claim"></a>구독을 클레임에 사용할 수 있는 경우

구독을 요청 하는 경우 구독이 아직 프로 비전 되지 않은 경우 오류를 받게 됩니다. CPOR 플랫폼에서 구독을 선택 하 고 클레임을 제공 하는 데 사용할 수 있도록 고객이 수행 해야 하는 몇 가지 단계가 있습니다. 구독을 요청 하는 동안 오류가 발생 하는 경우 고객에 게 연락 하 여 프로 비전 되었으며 주장 하는 구독이 올바른지 확인 합니다. 이 경로를 이미 만든 경우 [지원](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)담당자에 게 문의 하세요.

## <a name="which-activity-do-i-choose"></a>어떤 작업을 선택 해야 하나요?

CPOR 클레임 플랫폼은 Business Applications 및 Microsoft 365 솔루션 영역과 관련 된 CPOR association 클레임을 허용 합니다. 각 솔루션 영역에 적용할 수 있는 작업은 다음과 같습니다. 설명에 따라 올바른 활동을 선택 하 여 나중에 회수할 필요가 없도록 합니다. 잘못 된 작업으로 주장 하면 자격 및 동기 소득이 누락 될 수 있습니다.


| 솔루션 영역 | 활동 | 적용 가능 |
| ------ | ----------- | ----------- |
| 비즈니스 애플리케이션      | 예약 판매   | 적격 제품의 구매에 영향을 준 경우 사전 판매 성과급을 적용 하려는 경우에 선택 합니다. 이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용할 수 있습니다. |
|    |  사용량  | 적합 한 워크 로드의 도입 및 사용을 추진 하 고 사용 성과급을 적용 하려는 경우에 선택 합니다. 이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용할 수 있습니다. |
|    | 수익 연결   | 적격 제품의 선택에 영향을 주는 비즈니스 주는 요인은 선택 합니다. 이 옵션은 동기 지불액이 아닌 수익 연결에만 적용 됩니다. 이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용할 수 있습니다.   |
| Microsoft 365   | 사용량   | 적합 한 워크 로드의 도입 및 사용을 추진 하 고 사용 성과급을 적용 하려는 경우에 선택 합니다. |

## <a name="which-mpn-do-i-choose"></a>어떤 MPN를 선택 하나요?

CPOR association 클레임 흐름에서 최종 고객에 게 요청 하는 작업에 연결 해야 하는 회사 MPN을 선택 하 라는 메시지가 표시 됩니다. 회사에는 여러 MPNs가 있을 수 있으며, 그 중 일부는 동기 프로그램에 등록 될 수 있으며, 다른 일부는 FRP FastTrack 같은 파트너 유형과 연결 되어 있을 수 있습니다. CPOR association 클레임 흐름은 동기 프로그램에 등록 된 MPNs를 식별 하지만 MPN 특정 파트너 유형인 경우에는 알 수 없습니다. 나중에 회수할 필요가 없도록 올바른 MPN를 선택 하는 것이 중요 합니다. 잘못 된 MPN를 사용 하 여 주장 하면 자격 및 동기 소득이 누락 될 수 있습니다.

사용할 MPN를 모르는 경우 전역 관리자에 게 문의 하세요.

사용 하려는 MPN이 등록 되지 않은 경우에는 [성과급 개요 탭](https://partner.microsoft.com/dashboard/incentives/enrollment/summary)에서 관리할 수 있습니다.

## <a name="choosing-a-product-vs-entering-a-subscription"></a>제품 선택 및 구독 입력

Dynamics 제품이 요청 및 승인 되 면 파트너는 CPOR association 클레임 자체에서 구독 ID를 볼 수 있습니다. 이 구독을 요청 하면 활성 또는 유예 상태 이지만 구독이 종료 되는 시간이 있을 수 있으며 새 구독은 별도의 CPOR 연결 클레임에서 요청 해야 합니다.

## <a name="competing-claims"></a>경쟁 하는 클레임

다른 파트너와 이미 연결 되어 있는 고객 및 해당 제품에 대 한 CPOR association 클레임을 만드는 경우 클레임은 중재를 통해 수행 됩니다.

1. 파트너가 새 고객 연결을 만들면 Microsoft가 정확성을 보장하기 위해 제공된 연결 및 실행 증명의 세부 정보를 확인합니다.

2. 사용자와 다른 파트너가 동일한 고객 및 제품/작업을 클레임 하는 경우 Microsoft는 각 파트너의 실행 설명서를 검토 하 여 승인할 파트너를 결정 합니다.

3. 두 파트너 모두에서 추가 정보를 요청할 수 있으며,이로 인해 연결 요청 처리가 지연 될 수 있습니다.

4. CPOR association 클레임은 계속 해 서 5 영업일 이내에 검토 됩니다. 단, 그 상태는 더 오랜 기간 동안 _검토_ 하는 것으로 유지 될 수 있습니다. 이 시나리오는 Microsoft가 현재 제품/워크 로드를 소유 하 고 있는 파트너와 함께 작업 하는 경우에 발생할 수 있습니다. 해당 하는 경우에는 클레임의 설명 섹션에서 알림이 표시 됩니다. 

>[!IMPORTANT]
>CPOR association PoE를 확인 하기 위해 추가 정보가 필요한 경우 CPOR association 클레임 설명 섹션을 통해 연락 드리겠습니다.
