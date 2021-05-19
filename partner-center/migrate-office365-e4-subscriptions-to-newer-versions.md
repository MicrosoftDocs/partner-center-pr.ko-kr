---
title: Office 365 E4 구독 마이그레이션
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 edition은 2017 년 4 월 7 일에 사용 중지 됩니다. 최신 버전의 Office 365로 고객 구독을 마이그레이션하는 방법에 대해 알아봅니다.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151562"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Office 365 E4 구독을 최신 Office 365 버전으로 마이그레이션

**적절 한 역할**: 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트 | 판매 에이전트

Office 365 Enterprise E4 요금제는 2017 년 4 월 7 일부 터 사용 중지 됩니다. 이 날짜 이후에는 새 Office 365 E4 구독을 더 이상 구매할 수 없으며 기존 E4 구독은 만료 될 때 자동으로 갱신 되지 않습니다.

E4 구독이 종료 되 면 취소 됩니다. 고객의 연속성을 보장 하려면 다음에 나열 된 지원 되는 SKU 옵션을 만료 하는 E4 구독이 있는 고객을 전환 해야 합니다. 고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다. 

> [!NOTE]  
> Office 365 Enterprise E4 상용 및 정부 Sku는 모두 사용이 중지 됩니다.
 
구독의 세부 정보 페이지에서 E4 구독 상태가 "[date]에 대 한 자동 갱신 [date]"에서 "Expires on [date]"로 변경 되었습니다. 

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 검색할 수 있습니다. 

E4 구독은 2017 년 4 월 7 일에 자동 갱신 = False로 설정 됩니다. 언제 든 지 새 요금제로 고객을 이동할 수 있습니다. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4 버전 교체 계획

E4와 동일한 기능을 유지 하거나 고객이 Office 365 및 비즈니스용 Skype Online에서 최신 기능과 기능을 활용할 수 있도록 선택할 수 있습니다. 가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다. Office 365 Enterprise E3 또는 Office 365 Enterprise E5의 다음 옵션에서는 보안 제품 Enterprise E3 또는 안전한 생산적인 Enterprise E5를 각각 대체할 수 있습니다.

- 옵션 1: Office 365 Enterprise E5

- 옵션 2: Office 365 Enterprise E3 + 비즈니스용 Skype 클라우드 PBX

- 옵션 3: Office 365 Enterprise E3 + 비즈니스용 Skype Plus CAL(E4의 가격 및 기능 패리티)

- 옵션 4: Office 365 Enterprise E3


| 기능 | 옵션 1 | 옵션 2 | 옵션 3 | 옵션 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Office 365 Enterprise E4에 포함된 모든 기능을 사용하세요? | 예 | 예 | 예 | 예 |
| Office 365에서 관리되는 전화 번호 | 예 | 예 | 예 | 예 |
| 온-프레미스와 Office 365(하이브리드 배포)에서 모두 관리되는 전화 번호는 무엇인가요? | 예 | 예 | 예 | 예 |
| PSTN 음성 통화 계획을 추가하는 옵션 | 예 | 예 | 예 | 예 |
| PSTN 회의? | 예 | 예 | 예 | 예 |
| 협업, 분석 및 보안을 위한 고급 도구는 무엇인가요? | 예 | 예 | 예 | 예 |
| 대화형 보고서, 대시보드 및 데이터 시각화 | 예 | 예 | 예 | 예 | 
| 기본 제공 개인 정보 보호, 투명성 및 구체화된 사용자 정의 컨트롤을 통해 데이터 보안 및 규정 준수를 더 자세히 제어할 수 있나요? | 예 | 예 | 예 | 예 | 

## <a name="transition-customers-to-new-product-plans"></a>고객을 새 제품 플랜으로 전환

Microsoft는 파트너에게 지속적으로 새 제품 및 서비스를 제공합니다. 이러한 경우 고객을 새 서비스로 업그레이드하거나 최종적으로 종료될 S SKU에서 구독을 마이그레이션해야 할 수 있습니다. 사용 중지된 S SKU에서 최신 S SKU로 고객을 마이그레이션하려면 다음 단계가 필요합니다.

-   새 구독 구매
-   현재 사용자 라이선스 재할당
-   이전 구독 취소

다음 단계에 따라 고객의 Office 365 Enterprise E4 구독을 위 표의 옵션 중 하나로 마이그레이션합니다.

### <a name="step-1---purchase-the-new-subscription"></a>1단계 - 새 구독 구매

1. **파트너 센터** 메뉴에서 **고객을** 선택하고 이동하려는 고객을 선택한 다음 구독 **추가를** 선택합니다.

2. 카탈로그에서 구매할 구독(이 경우 위의 옵션 중 하나)을 선택하고 라이선스 수를 입력한 다음, **제출을** 선택합니다.

   이제 고객에게 이전 및 새 구독, 이전 Office 365 Enterprise E4 구독 및 새 '대상' 구독(예: 옵션 1 - Office 365 Enterprise E5)이 있어야 합니다.

### <a name="step-2---reassign-the-customers-users-licenses"></a>2단계 - 고객의 사용자 라이선스 재할당

1. **파트너 센터** 메뉴에서 **고객을** 선택하고 이동하려는 고객을 선택한 다음, 사용자 및 **라이선스를** 선택합니다. 고객의 사용자 및 라이선스 페이지가 열립니다.

2. 사용자 라이선스를 다시 할당하려면 재할당할 사용자를 선택한 **다음, 라이선스 관리를 선택합니다.**

3. 라이선스 **관리** 페이지에서 **Office 365 Enterprise E4** 라이선스 확인란의 선택을 취소하고 고객이 이동하는 구독에 대한 새 서비스 계획을 선택합니다.

4. **제출** 을 선택합니다. 확인 페이지에 새 라이선스 할당이 나열됩니다.

5. 라이선스 재할당이 필요한 다른 고객 사용자와 동일한 단계를 계속합니다.

사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.

### <a name="step-3---cancel-the-old-subscription"></a>3단계 - 이전 구독 취소

1. **파트너 센터** 메뉴에서 **고객을** 선택합니다. 이동하려는 고객을 선택하고 취소할 구독을 선택합니다.

2. 구독 세부 정보 페이지에서 구독 상태를 **일시 중단 으로** 설정합니다.

3. **제출** 을 선택합니다.

이전 구독이 일시 중단되고 새 구독이 활성 상태입니다. 일시 중단된 구독은 120일 후에 자동으로 프로비저닝이 해제됩니다. 고객은 이전 구독에 대한 추가 비용이 발생하지 않습니다.



 



