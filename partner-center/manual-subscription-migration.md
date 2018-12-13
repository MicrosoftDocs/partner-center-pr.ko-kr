---
title: Dynamics 365 고객 참여 계획 하 고 기본 (자격 갖춘된 제공)을 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / 고객 참여 계획 (자격을 갖춘 제공)는 기본 구독에서 더 이상 갱신할 수 없습니다.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968273"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 고객 참여 계획 하 고 기본 (자격 갖춘된 제공)을 최신 버전으로 마이그레이션

**적용 대상**

-  파트너 센터

Dynamics 365 for Sales 사용 하 여 유효 2019 년 1 월 1 일, 고객 / 고객 참여 계획 (자격을 갖춘 제공)는 기본 구독에서 이러한 레거시 제품; 더 이상 갱신할 수 기존 구독 만료 시 자동으로 갱신 되지 않습니다. 구독의 세부 정보 페이지에서 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경 됩니다. 


고객에 대 한 연속성을 보장 하려면 아래에 나열 된 지원 되는 옵션으로 구독이 곧 만료 되 있는 사용자를 전환 해야 합니다. 고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다.

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 함께 구독의 종료 날짜를 확인 하 여 곧 만료 되 구독 찾을 수 = False 속성과 합니다. 해당 구독을 자동으로 설정 됩니다 갱신 2019 년 1 월 1 일에 = False입니다. 언제든지 고객을 새 요금제로 이동할 수 있습니다. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 사용 중지 되 고 제공

- Dynamics 365 판매 Enterprise Edition CRMOL basic (자격 갖춘된 제품)
- Dynamics 365 교직원에 대 한 판매 Enterprise Edition CRMOL basic (자격 갖춘된 제품)
- Dynamics 365 학생에 대 한 판매 Enterprise Edition CRMOL basic (자격 갖춘된 제품)
- Dynamics 365 판매 Enterprise Edition (정부 가격) CRMOL basic (자격 갖춘된 제품)
- CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365
- 교직원 용 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365
- 학생 들을 위한 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365
- CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 판매 Enterprise Edition (정부 가격)에 대 한 Dynamics 365
- CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365
- 교직원 용 CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365
- 학생 들을 위한 CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition 추가 기능에 대 한 Dynamics 365
- CRM Basic (자격 갖춘된 제품)에 대 한 판매 Enterprise Edition (정부 가격) 추가 기능에 대 한 Dynamics 365
- Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic (자격 갖춘된 제품)
- Dynamics 365 고객 참여 계획 Enterprise Edition (정부 가격) CRMOL Basic (자격 갖춘된 제품)
- Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic (자격 갖춘된 제품) 학생
- Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic (자격 갖춘된 제품) 교직원
- CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition
- Dynamics 365 고객 참여 계획 Enterprise Edition (정부 가격)에서 SA CRM basic (자격 갖춘된 제품)
- 학생 들을 위한 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition
- 교직원 용 CRM Basic (자격 갖춘된 제품)에 대 한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition
- Dynamics 365 고객 참여 계획 Enterprise Edition의 추가 기능 CRM Basic (자격 갖춘된 제품)
- Dynamics 365 고객 참여 계획 Enterprise Edition (정부 가격) 추가 기능 CRM basic (자격 갖춘된 제품)
- Dynamics 365 고객 참여 계획 Enterprise Edition의 추가 기능 학생에 대 한 CRM Basic (자격 갖춘된 제품)
- Dynamics 365 고객 참여 계획 Enterprise Edition의 추가 기능 교직원 용 CRM Basic (자격 갖춘된 제품)



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / 계획 (자격을 갖춘 제공) 기본 대체에서 고객 참여 계획

**사용 중지 된 제품**   

- Dynamics 365 for Sales CRM Basic 또는 CRMOL (자격 갖춘된 제품)에서
- CRM Basic 또는 CRMOL (자격 갖춘된 제품)에서 Dynamics 365 고객 참여 계획

**대체 옵션**
- Dynamics 365 판매 professional (신규)
- Dynamics 365 판매 professional (신규)
- Dynamics 365 for Customer Service
- Dynamics 365 고객 참여 계획 또는
- Dynamics 365 팀 구성원



## <a name="transition-customers-to-new-product-plans"></a>새 제품 요금제로 고객 전환

고객에 게 사용 중지 된 Sku에서 최신 패키지로 이동 순서로 다음 단계를 따라야 합니다.

- 새 구독 구매
- 현재 사용자 라이선스 다시 할당
- 이전 구독 취소

## <a name="purchase-the-new-plan-for-your-customer"></a>구매 고객에 대 한 새 계획

1. 왼쪽된 탐색에서 **고객** 을 선택 하 고 새 구독으로 이동 하려는 고객을 선택 합니다.
2. **구독 추가**선택 합니다.
3. 카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다. 

이전 구독와 새 고객에 게 이제 생깁니다. 다음 단계는 고객의 사용자에 게 라이선스 할당 하는 것입니다.

1. 왼쪽된 탐색에서 **고객** 을 선택 하 고 이동 하려는 고객을 선택 합니다.
2. **사용자 및 라이선스**를 선택합니다.
3. 사용자에 게 라이선스를 할당 하는 사용자를 선택 하 고 **라이선스 관리를**선택 합니다. 
4. **라이선스 관리** 페이지에서 Dynamics 365 for Sales의 선택을 취소/고객 참여 계획 (자격을 갖춘 제공) 기본에서 라이선스 확인란을 선택 하 고 고객을 이동할 구독의 새로운 서비스 요금제를 선택 합니다. 
5. **제출**을 선택합니다. 새 라이선스를 필요로 하는 각 사용자에 대해이 작업을 수행 합니다. 

새 구독에 라이선스를 이동한 후에 이전 구독을 취소할 수 있습니다. 

1. 왼쪽된 탐색에서 **고객** 을 선택 하 고 이동 하려는 고객을 선택 합니다.
2. 구독 세부 정보 페이지에서 이전 구독 **일시 중단 됨** 을 설정 하 고 **제출**을 선택 합니다.

이전 구독이 이제 일시 중단 하 고 새 구독이 활성화 됩니다. 일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다. 고객에 게 이전 구독에 대 한 추가 비용 없이 발생 됩니다.
 

 



