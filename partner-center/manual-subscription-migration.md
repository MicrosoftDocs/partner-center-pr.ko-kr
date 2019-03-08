---
title: Basic (정규화 된 제품)에서 Dynamics 365 Customer Engagement 계획 하 고를 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Basic (정규화 된 제공) 구독에서 고객 참여 계획 갱신할 수 없습니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 제품의 제품에 새 Dynamics 365 Sku 갱신
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586946"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 및 Customer Engagement Plan을 기본 (정규화된 제안)에서 새 버전으로 마이그레이션

**적용 대상**

-  파트너 센터

Dynamics 365 for Sales 사용 하 여 효과적인 2019 년 1 월 1 일 고객 / Basic (정규화 된 제공) 구독에서 고객 참여 계획 수 이러한 레거시 제품; 갱신할 이상 만료 시 기존 구독을 자동으로 갱신 되지 않습니다. 구독 세부 정보 페이지에서 구독 상태를 "[date]에 자동 갱신"에서 "[date]에 만료"에 변경 됩니다. 


고객에 대 한 연속성을 위해 아래에 나열 된 지원 되는 옵션에 대 한 구독을 만료를 사용 하 여 해당 전환 해야 합니다. 고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.

자동 함께 구독 종료 날짜를 평가 하 여 만료 구독을 갱신 찾을 수 있습니다 (CREST 또는 파트너 센터) API를 사용 하는 경우 = False 속성입니다. 해당 구독이 자동으로 설정 됩니다 갱신 2019 년 1 월 1 일에서 = False. 언제든지 고객을 새 요금제로 이동할 수 있습니다. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 사용이 중지 되는 제공

- Dynamics 365 for Sales Enterprise Edition CRMOL 기본 (정규화 된 제품)
- 교직원 용 판매 Enterprise Edition CRMOL Basic (정규화 된 제품)에 대 한 Dynamics 365
- 학생을 위한 판매 Enterprise Edition CRMOL Basic (정규화 된 제품)에 대 한 Dynamics 365
- Dynamics 365 for Sales Enterprise Edition (정부 기관용 가격 책정) CRMOL 기본 (정규화 된 제품)
- CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise Edition 용 Dynamics 365
- 교직원 용 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise Edition 용 Dynamics 365
- 학생을 위한 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise Edition 용 Dynamics 365
- CRM Basic (정규화 된 제품)에 대 한 SA의 (정부 기관용 가격 책정) 판매 Enterprise Edition 용 Dynamics 365
- CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365
- 교직원 용 CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365
- 학생을 위한 CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365
- CRM Basic (정규화 된 제품)에 대 한 판매 Enterprise Edition (정부 기관용 가격 책정) 추가 기능에 대 한 Dynamics 365
- Dynamics 365 Customer Engagement 계획 Enterprise Edition CRMOL Basic (정규화 된 제품)
- Dynamics 365 Customer Engagement 계획 Enterprise Edition (정부 기관용 가격 책정) CRMOL Basic (정규화 된 제품)
- Dynamics 365 Customer Engagement 계획 Enterprise Edition CRMOL Basic (정규화 된 제품) 학생용
- Dynamics 365 Customer Engagement 계획 Enterprise Edition CRMOL Basic (정규화 된 제품) 교직원 용
- CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 계획 Enterprise Edition
- Dynamics 365 Customer Engagement 계획 Enterprise Edition (정부 기관용 가격 책정) CRM Basic (정규화 된 제품)에 대 한 SA의
- 학생을 위한 CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 계획 Enterprise Edition
- 교직원 용 CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 Customer Engagement 계획 Enterprise Edition
- Dynamics 365 Customer Engagement 계획 Enterprise Edition 용 추가 기능 CRM Basic (정규화 된 제품)
- Dynamics 365 Customer Engagement 계획 Enterprise Edition (정부 기관용 가격 책정) 용 추가 기능 CRM Basic (정규화 된 제품)
- Dynamics 365 Customer Engagement 계획 Enterprise Edition 용 추가 기능 학생용 CRM Basic (정규화 된 제품)
- Dynamics 365 Customer Engagement 계획 Enterprise Edition 용 추가 기능 교직원 용 CRM Basic (정규화 된 제품)



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / 계획 (정규화 된 제공) 하는 기본 대체에서 고객 참여 계획

**중단된 제안**   

- Dynamics 365 판매 CRM Basic 또는 CRMOL Basic (정규화 된 제품)
- CRM Basic 또는 CRMOL Basic (정규화 된 제품)에서 Dynamics 365 Customer Engagement 요금제

**대체 옵션**
- Dynamics 365 판매 professional (신규)
- Dynamics 365 판매 professional (신규)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement 요금제 또는
- Dynamics 365 팀 멤버



## <a name="transition-customers-to-new-product-plans"></a>새 제품 계획으로 고객 전환

사용 중지 된 Sku에서 새 버전을 고객에 게 이동이 순서로 다음 단계를 필요 합니다.

- 새 구독 구매
- 현재 사용자 라이선스 다시 할당
- 이전 구독 취소

## <a name="purchase-the-new-plan-for-your-customer"></a>고객을 위해 새 계획을 구입

1. 선택 **고객** 왼쪽된 탐색 창에서 새 구독으로 이동 하려는 고객을 선택 합니다.
2. 선택 **구독 추가**합니다.
3. 카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다. 

이전 구독 및 새 고객에 게 이제 됩니다. 다음 단계 고객에 게 라이선스를 다시 할당 하는 것입니다.

1. 선택 **고객** 왼쪽된 탐색 창에서 선택 된 고객 이동 하는 합니다.
2. **사용자 및 라이선스**를 선택합니다.
3. 사용자에 게 라이선스를 할당할 사용자를 선택 하 고 선택한 **라이선스 관리**합니다. 
4. 에 **라이선스 관리** 페이지, Dynamics 365 for Sales 지우기 / Basic (정규화 된 제공)에서 Customer Engagement 요금제 확인란 라이선스,로 이동 하는 고객 구독에 대 한 새 서비스 계획을 선택 합니다. 
5. **제출**을 선택합니다. 새 라이선스를 필요로 하는 각 사용자에 대 한이 작업을 수행 합니다. 

새 구독에 라이선스를 통해 이동한 후에 이전 구독을 취소할 수 있습니다. 

1. 선택 **고객** 왼쪽된 탐색 창에서 선택 된 고객 이동 하는 합니다.
2. 구독 세부 정보 페이지에서 이전 구독을 설정 **Suspended** 선택한 **제출**합니다.

이전 구독 이제 일시 중단 및 새 구독이 활성화 되어 있습니다. 일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다. 고객에 게 기존 구독에 대 한 추가 비용 없이 발생 합니다.
 

 



