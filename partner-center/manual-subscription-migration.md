---
title: 기본 (정규화 된 제안)에서 최신 버전으로 Dynamics 365 및 고객 참여 계획 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 기존 구독을 만료 하기 전에 구매한 후 사용자 라이선스를 다시 할당 하 고 이전 구독을 취소 하는 방법을 알아봅니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 제안, 갱신 제안, 새 Dynamics 365 Sku
ms.openlocfilehash: 466f954af05a266fccba587007565e5d19d3af15
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004593"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 및 Customer Engagement Plan을 기본 (정규화된 제안)에서 새 버전으로 마이그레이션

**적용 대상**

-  파트너 센터

**적절한 역할**
-   전역 관리자
-   사용자 관리자
-   관리자 에이전트
-   영업 에이전트

2019 년 1 월 1 일부 터 기본 (우량 제안) 구독의 판매/고객 참여 요금제에 대 한 Dynamics 365이 있는 고객은 이러한 레거시 제안을 더 이상 갱신할 수 없습니다. 기존 구독은 만료 될 때 자동으로 갱신 되지 않습니다. 구독의 세부 정보 페이지에서 구독 상태는 "[date]에 대 한 자동 갱신 [날짜]"에서 "만료 날짜 [날짜]"로 변경 됩니다. 


고객의 연속성을 보장 하려면 구독 만료를 포함 하는 항목을 아래 나열 된 지원 되는 옵션으로 전환 해야 합니다. 고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾을 수 있습니다. 문제의 구독은 1 월 1 일 2019에 자동 갱신 = False로 설정 됩니다. 언제든지 고객을 새 요금제로 이동할 수 있습니다. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 제공이 사용 중지 됨

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (정규화 된 제품)
- 교직원 용 Dynamics 365 for Sales Enterprise Edition CRMOL 기본 (우량 제안)
- 학생을 위한 Dynamics 365 for Sales Enterprise Edition CRMOL Basic (우량 제안)
- Dynamics 365 for Sales Enterprise Edition (정부 가격) CRMOL 기본 (정규화 된 제품)
- CRM Basic (정규화 된 제품)의 경우 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365
- 교직원 용 Dynamics 365 for CRM Basic (우량 제안) for 교직원
- 학생의 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise 버전용 Dynamics 365
- CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 for Sales Enterprise Edition (정부 가격)
- CRM Basic (정규화 된 제품) 용 Dynamics 365 for Sales Enterprise Edition 추가 기능
- 교직원 용 Dynamics 365 for CRM Basic (우량 제안) for 교직원
- 학생용 CRM Basic (우량 제안) 용 Dynamics 365 for Sales Enterprise Edition 추가 기능
- CRM Basic (정규화 된 제품) 용 Dynamics 365 for Sales Enterprise Edition (정부 가격) 추가 기능
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (정규화 된 제품)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (정부 가격) CRMOL 기본 (적격 제안)
- 학생용 Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (우량 제안)
- 교직원 용 Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL 기본 (적격 제안)
- Dynamics 365 Customer Engagement Plan for SA에서 CRM Basic (정규화 된 제품)에 대 한 엔터프라이즈 버전
- CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 요금제 Enterprise Edition (정부 가격)
- Dynamics 365 Customer Engagement Plan for SA에서 학생용 CRM Basic (정규화 된 제품)
- Dynamics 365 고객 Engagement 요금제의 SA에서 교직원 용 CRM Basic (정규화 된 제품)에 대 한 엔터프라이즈 버전
- CRM Basic (정규화 된 제품) 용 Dynamics 365 Customer Engagement Plan Enterprise Edition 추가 기능
- CRM Basic (정규화 된 제품) 용 Dynamics 365 고객 Engagement 계획 Enterprise Edition (정부 가격) 추가 기능
- 학생용 CRM Basic (정규화 된 제품) 용 Dynamics 365 고객 Engagement 계획 Enterprise Edition 추가 기능
- 교직원 용 Dynamics 365 Customer Engagement 계획 Enterprise Edition 추가 기능 (교직원 용 정규화 된 제품)



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>기본 (우량 제안) 대체 요금제에서 판매/고객 참여 요금제에 대 한 Dynamics 365

**사용 중지 된 제안**   

- CRM Basic 또는 CRMOL Basic (정규화 된 제안)에서 판매에 대 한 Dynamics 365
- CRM Basic 또는 CRMOL Basic (정규화 된 제품)의 Dynamics 365 Customer Engagement 계획

**대체 옵션**
- Dynamics 365 for Sales Professional (신규)
- Dynamics 365 for Sales Professional (신규)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement 요금제 또는
- Dynamics 365 팀 멤버



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
 

 



