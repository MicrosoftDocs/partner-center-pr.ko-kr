---
title: 정규화 된 Dynamics 365 구독 마이그레이션
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 기존 구독이 만료 되기 전에 정규화 된 기본 Dynamics 365 구독에서 새 구독으로 마이그레이션하는 방법에 대해 알아봅니다.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151647"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 및 Customer Engagement 플랜을 기본(제한된 제품)에서 새 버전으로 마이그레이션

**적절 한 역할**: 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트 | 판매 에이전트

2019 년 1 월 1 일부 터 기본 (우량 제안) 구독의 판매/고객 참여 요금제에 대 한 Dynamics 365이 있는 고객은 이러한 레거시 제안을 더 이상 갱신할 수 없습니다. 기존 구독은 만료 될 때 자동으로 갱신 되지 않습니다. 구독의 세부 정보 페이지에서 구독 상태는 "[date]에 대 한 자동 갱신 [날짜]"에서 "만료 날짜 [날짜]"로 변경 됩니다. 

고객의 연속성을 보장 하려면 구독 만료를 포함 하는 항목을 아래 나열 된 지원 되는 옵션으로 전환 해야 합니다. 고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾을 수 있습니다. 문제의 구독은 2019 년 1 월 1 일에 자동 갱신 = False로 설정 됩니다. 언제 든 지 새 요금제로 고객을 이동할 수 있습니다. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 제공이 사용 중지 됨

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (정규화 된 제품)
- 교직원 용 Dynamics 365 for Sales Enterprise Edition CRMOL 기본 (우량 제안)
- 학생을 위한 Dynamics 365 for Sales Enterprise Edition CRMOL Basic (우량 제안)
- Dynamics 365 for Sales Enterprise Edition (정부 가격) CRMOL 기본 (정규화 된 제품)
- CRM Basic (정규화 된 제품)의 경우 SA에서 판매 Enterprise 버전에 대 한 Dynamics 365
- 교직원 용 Dynamics 365 for CRM Basic (우량 제안) for 교직원
- 학생의 CRM Basic (정규화 된 제품)에 대 한 SA의 판매 Enterprise 버전용 Dynamics 365
- CRM Basic (정규화 된 제품)에 대 한 SA의 Dynamics 365 for Sales Enterprise Edition (정부 가격)
- DYNAMICS 365 for Sales Enterprise Edition Add-On for CRM Basic(정규화된 제안)
- 교직원용 DYNAMICS 365 for Sales Enterprise Edition Add-On(정규화된 제안)
- 학생용 DYNAMICS 365 for Sales Enterprise Edition Add-On(정규화된 제안)
- CRM Basic용 Dynamics 365 for Sales Enterprise Edition(정부 가격 책정) Add-On(적격 제품)
- Dynamics 365 고객 참여 계획 Enterprise Edition CRMOL Basic(정규화된 제안)
- Dynamics 365 Customer Engagement 플랜 Enterprise Edition(정부 가격 책정) CRMOL Basic(적격 제품)
- 학생용 CRMOL Basic(정규화된 제안)을 Enterprise Edition Dynamics 365 고객 참여 계획
- 교직원용 CRMOL Basic(정규화된 제안)을 Enterprise Edition Dynamics 365 Customer Engagement 플랜
- CRM Basic(정규화된 제안)에 대한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition
- CRM Basic에 대한 SA의 Dynamics 365 고객 참여 계획 Enterprise Edition(정부 가격 책정) (적격 제품)
- 학생용 CRM 기본(적격 제안)용 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition
- 교직원용 CRM 기본(적격 제안)에 대한 SA에서 Dynamics 365 고객 참여 계획 Enterprise Edition
- CRM Basic용 Dynamics 365 고객 참여 계획 Enterprise Edition Add-On(적격 제안)
- CRM Basic용 Dynamics 365 고객 참여 플랜 Enterprise Edition(정부 가격 책정) Add-On(적격 제품)
- 학생용 CRM Basic(정규화된 제안)을 위한 Dynamics 365 고객 참여 계획 Enterprise Edition Add-On
- 교직원용 CRM 기본(적격 제안)에 대한 Dynamics 365 고객 참여 계획 Enterprise Edition Add-On



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>기본(적격 제안) 교체 계획의 Dynamics 365 for Sales/Customer Engagement 플랜

**사용 중지된 제안**   

- CRM Basic 또는 CRMOL Basic의 Dynamics 365 for Sales(정규화된 제안)
- CRM Basic 또는 CRMOL Basic의 Dynamics 365 고객 참여 계획(적격 제안)

**대체 옵션**
- Dynamics 365 for Sales Professional (신규)
- Dynamics 365 for Sales Professional (신규)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement 요금제 또는
- Dynamics 365 팀 멤버



## <a name="transition-customers-to-new-product-plans"></a>고객을 새 제품 요금제로 전환

사용 중지 된 Sku에서 최신 버전으로 고객을 이동 하려면 다음 단계를 순서 대로 수행 해야 합니다.

- 새 구독 구매
- 현재 사용자 라이선스 다시 할당
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
5. **제출** 을 선택합니다. 새 라이선스가 필요한 각 사용자에 대해 이 작업을 수행합니다. 

라이선스를 새 구독으로 이동한 후에는 이전 구독을 취소할 수 있습니다. 

1. 왼쪽 탐색에서 **고객을** 선택한 다음, 이동 중인 고객을 선택합니다.
2. 구독 세부 정보 페이지에서 이전 구독을 **일시 중단으로** 설정하고 **제출을** 선택합니다.

이제 이전 구독이 일시 중단되고 새 구독이 활성화됩니다. 일시 중단된 구독은 120일 후에 자동으로 프로비저닝이 해제됩니다. 고객은 이전 구독에 대한 추가 비용이 발생하지 않습니다.
 

 



