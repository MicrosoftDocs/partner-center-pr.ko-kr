---
title: Dynamics 365 Business Edition 마이그레이션
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 정규화된 Dynamics 365 Business Edition 제안을 만료되기 전에 최신 버전으로 마이그레이션하는 방법을 알아봅니다.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151528"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition 제품을 최신 버전으로 마이그레이션

**적절한 역할:** 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트 | 판매 에이전트

2019년 1월 1일부터 Dynamics 365 Business Edition 구독을 보유한 고객은 더 이상 이러한 레거시 제품으로 갱신할 수 없습니다. 기존 구독은 만료될 때 자동으로 갱신되지 않습니다. 구독의 세부 정보 페이지에서 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료됨"으로 변경됩니다.

고객의 연속성을 보장하려면 만료된 구독이 있는 고객을 아래에 나열된 지원되는 옵션으로 전환해야 합니다. 고객의 서비스 중단을 방지하려면 구독의 연간 종료 날짜 이전에 고객을 새 구독으로 이동하는 것이 좋습니다.

API(CREST 또는 파트너 센터)를 사용하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가하여 만료되는 구독을 찾을 수 있습니다. 해당 구독은 2019년 1월 1일에 자동 갱신=False로 설정됩니다. 언제든지 고객을 새 플랜으로 이동할 수 있습니다. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>사용 중지 중인 Dynamics 365 Business Edition

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - Dynamics 365 Business Edition 새 제안

새 Dynamics Business Central 제안을 통해 고객은 재무, 영업, 서비스 및 운영을 연결하여 비즈니스 프로세스를 간소화하고, 고객 상호 작용을 개선하고, 더 나은 의사 결정을 내릴 수 있습니다. Dynamics 365 Business Central은 클라우드 기반이며 CSP(클라우드 솔루션 공급자) 프로그램 파트너를 통해서만 사용할 수 있습니다.
Dynamics 365 Business Edition 고객은 2020년 6월 30일까지 새 Business Central 제품에서 할인된 전환 가격을 받을 수 있습니다.

## <a name="transition-customers-to-new-product-plans"></a>고객을 새 제품 플랜으로 전환

 사용 중지된 S SKU에서 최신 S SKU로 고객을 이동하려면 다음 단계를 순서대로 수행해야 합니다.

- 새 구독 구매
- 현재 사용자 라이선스 재할당
- 이전 구독 취소

## <a name="purchase-the-new-plan-for-your-customer"></a>고객에 대 한 새 요금제 구매

1. 왼쪽 탐색 창에서 **고객** 을 선택한 다음 새 구독으로 이동할 고객을 선택 합니다.
2. **구독 추가** 를 선택 합니다.
3. 카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출** 을 선택 합니다. 

이제 고객에 게 이전 구독과 새 구독이 모두 포함 됩니다. 다음 단계는 고객의 사용자에 게 라이선스를 다시 할당 하는 것입니다.

1. 왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.
2. **사용자 및 라이선스** 를 선택 합니다.
3. 사용자에 게 라이선스를 재할당 하려면 사용자를 선택한 다음 **라이선스 관리** 를 선택 합니다. 
4. **라이선스 관리** 페이지에서 기본 (우량 제안) 라이선스에서 판매/고객 지원 계획에 대 한 Dynamics 365을 지우고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다. 
5. **제출** 을 선택합니다. 새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다. 

새 구독으로 라이선스를 이동한 후에는 이전 구독을 취소할 수 있습니다. 

1. 왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.
2. 구독 정보 페이지에서 이전 구독을 **일시 중단 됨** 으로 설정 하 고 **제출** 을 선택 합니다.

이제 이전 구독이 일시 중단 되 고 새 구독이 활성화 됩니다. 일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다. 고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.
