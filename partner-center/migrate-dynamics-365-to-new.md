---
title: Dynamics 365 Business Edition 제품을 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dynamics 365 Business Edition 제품이 만료 되기 전에 최신 버전으로 마이그레이션하는 방법에 대해 알아봅니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 제안, 갱신 제안, 새 Dynamics 365 Sku
ms.openlocfilehash: d4efd051b4d237eac5b766ed1aedc432e8b93ecc
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75005122"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition 제안을 최신 버전으로 마이그레이션 

**적용 대상**

- 파트너 센터

**적절한 역할**
-   전역 관리자
-   사용자 관리자
-   관리자 에이전트
-   영업 에이전트

2019 년 1 월 1 일부 터 Dynamics 365 Business Edition 구독이 있는 고객은 더 이상 이러한 레거시 제품으로 갱신할 수 없습니다. 기존 구독은 만료 될 때 자동으로 갱신 되지 않습니다. 구독의 세부 정보 페이지에서 구독 상태는 "[date]에 대 한 자동 갱신 [날짜]"에서 "만료 날짜 [날짜]"로 변경 됩니다.

고객의 연속성을 보장 하려면 구독 만료를 포함 하는 항목을 아래 나열 된 지원 되는 옵션으로 전환 해야 합니다. 고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾을 수 있습니다. 문제의 구독은 1 월 1 일 2019에 자동 갱신 = False로 설정 됩니다. 언제든지 고객을 새 요금제로 이동할 수 있습니다. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Dynamics 365 비즈니스 버전이 사용 중지 됨

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central-Dynamics 365 비즈니스 버전 새 제품

새 Dynamics Business Central 제품을 통해 고객은 financials, 영업, 서비스 및 작업을 연결 하 여 비즈니스 프로세스를 간소화 하 고 고객 상호 작용을 개선 하 고 더 나은 결정을 내릴 수 있습니다. Dynamics 365 비즈니스 중부는 클라우드를 기반으로 하며, CSP (클라우드 솔루션 공급자) 프로그램 파트너를 통해서만 사용할 수 있습니다.
Dynamics 365 Business Edition 고객은 2020 30 년 6 월 30 일까 지 새로운 비즈니스 중앙 제품에 대해 할인 된 전환 가격을 받을 수 있습니다.

## <a name="transition-customers-to-new-product-plans"></a>새 제품 요금제로 고객 전환

 사용 중지 된 Sku에서 최신 버전으로 고객을 이동 하려면 다음 단계를 순서 대로 수행 해야 합니다.

- 새 구독 구매
- 현재 사용자 라이선스 다시 할당
- 이전 구독 취소

## <a name="purchase-the-new-plan-for-your-customer"></a>고객에 대 한 새 요금제 구매

1. 왼쪽 탐색 창에서 **고객** 을 선택한 다음 새 구독으로 이동할 고객을 선택 합니다.
2. **구독 추가**를 선택 합니다.
3. 카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다. 

이제 고객에 게 이전 구독과 새 구독이 모두 포함 됩니다. 다음 단계는 고객의 사용자에 게 라이선스를 다시 할당 하는 것입니다.

1. 왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.
2. **사용자 및 라이선스**를 선택합니다.
3. 사용자에 게 라이선스를 재할당 하려면 사용자를 선택한 다음 **라이선스 관리**를 선택 합니다. 
4. **라이선스 관리** 페이지에서 기본 (우량 제안) 라이선스에서 판매/고객 지원 계획에 대 한 Dynamics 365을 지우고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다. 
5. **제출**을 선택합니다. 새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다. 

새 구독으로 라이선스를 이동한 후에는 이전 구독을 취소할 수 있습니다. 

1. 왼쪽 탐색 창에서 **고객** 을 선택한 다음 이동 하는 고객을 선택 합니다.
2. 구독 정보 페이지에서 이전 구독을 **일시 중단 됨** 으로 설정 하 고 **제출**을 선택 합니다.

이제 이전 구독이 일시 중단 되 고 새 구독이 활성화 됩니다. 일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다. 고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.
