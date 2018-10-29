---
title: Office 365 E4 구독을 Office 365 최신 버전으로 마이그레이션 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: Microsoft Office 365 Enterprise E4 버전은 2017년 4월 7일부로 사용 중지되었습니다. 고객 구독을 Office 365 최신 버전으로 마이그레이션하는 방법을 알아보세요.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 1dc3957d6abe4069f3868d49e92a458d20e7fbec
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796107"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Office 365 Enterprise E4 구독을 Office 365 최신 버전으로 마이그레이션

**적용 대상**

-  파트너 센터

Office 365 Enterprise E4 요금제가 2017년 4월 7일부로 사용 중지되었습니다. 이 날짜 이후로는 더 이상 새 Office 365 E4 구독을 구입할 수 없으며, 기존 E4 구독은 만료 시 자동으로 갱신되지 않습니다.

E4 구독이 만료되면 구독이 취소됩니다. 고객에게 연속성을 보장하기 위해, E4 구독이 곧 만료되는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다. 고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다. 

> [!NOTE]  
>  Office 365 Enterprise E4 상업용 및 정부용 Sku 모두 사용 중지 됩니다.
 
구독의 세부 정보 페이지에서 E4 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경되었습니다. 

API(CREST 또는 파트너 센터)를 사용하는 경우 auto renew = False 속성과 함께 구독의 종료 날짜를 확인하여 곧 만료되는 구독을 검색할 수 있습니다. 

E4 구독은 2017년 4월 7일에 auto renew=False로 설정됩니다. 언제든지 고객을 새 요금제로 이동할 수 있습니다. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4 버전 교체 요금제

E4와 같은 기능을 그대로 유지할 수도 있고 고객이 Office 365 및 비즈니스용 Skype Online의 새로운 기능을 활용하게 할 수도 있습니다. 가격 정보는 가격 목록에서 찾을 수 있으며 파트너 센터에 목록표가 제공됩니다. Secure Product Enterprise E3 또는 Secure Productive Enterprise E5는 각각 Office 365 Enterprise E3 또는 Office 365 Enterprise E5에 대한 다음 옵션에서 대체될 수 있습니다.

- 옵션 1: Office 365 Enterprise E5

- 옵션 2: Office 365 Enterprise E3 + 비즈니스용 Skype 클라우드 PBX

- 옵션 3: Office 365 Enterprise E3 + 비즈니스용 Skype Plus CAL(E4와 가격 및 기능이 동일)

- 옵션 4: Office 365 Enterprise E3


| 특징 | 옵션 1 | 옵션 2 | 옵션 3 | 옵션 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Office 365 Enterprise E4의 모든 기능을 제공하나요? | 예 | 예 | 예 | 아니요 |
| 전화 번호를 Office 365에서 관리하나요? | 예 | 예 | 아니요 | 아니요 |
| 전화 번호를 온-프레미스와 Office 365 모두에서 관리하나요(하이브리드 배포)? | 예 | 예 | 아니요 | 아니요 |
| PSTN 음성 통화 요금제를 추가할 수 있나요? | 예 | 예 | 아니요 | 아니요 |
| PSTN 회의가 가능한가요? | 예 | 아니요 | 아니요 | 아니요 |
| 공동 작업, 분석 및 보안을 위한 고급 도구가 제공되나요? | 예 | 아니요 | 아니요 | 아니요 |
| 대화형 보고서, 대시보드 및 데이터 시각화가 제공되나요? | 예 | 아니요 | 아니요 | 아니요 | 
| 기본 프라이버시, 투명성 및 정교한 사용자 컨트롤로 데이터 보안과 규정 준수를 보다 철저하게 제어할 수 있나요? | 예 | 아니요 | 아니요 | 아니요 | 

## <a name="transition-customers-to-new-product-plans"></a>새 제품 요금제로 고객 전환

Microsoft는 지속적으로 파트너에게 새 제품 및 서비스를 제공합니다. 다음과 같은 경우 파트너는 고객을 새 서비스로 업그레이드하거나 결국 종료될 SKU의 구독을 마이그레이션해야 할 수 있습니다. 사용 중지된 SKU에서 새 SKU로 고객을 마이그레이션하려면 다음 단계를 따라야 합니다.

-   새 구독 구매
-   현재 사용자 라이선스 다시 할당
-   이전 구독 취소

다음 단계에 따라 고객의 Office 365 Enterprise E4 구독을 아래 표의 옵션 중 하나로 마이그레이션합니다.

### <a name="step-1---purchase-the-new-subscription"></a>1단계 - 새 구독 구매

1. **파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동 하려는 고객을 선택한 다음 **구독 추가**선택 합니다.

2. 카탈로그에서 구매할 구독을 선택하고(이 경우 아래 옵션 중 하나), 라이선스 수를 입력한 다음 **제출**을 선택합니다.

   이제 고객은 기존 구독과 새 구독, 다시 말해서 기존 Office 365 엔터프라이즈 E4 구독과 새로운 '대상' 구독(예: 옵션 1 - Office 365 Enterprise E5)을 모두 갖고 있습니다.

### <a name="step-2---reassign-the-customers-users-licenses"></a>2단계 - 고객의 사용자 라이선스 다시 할당

1. **파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동 하려는 고객 선택한 다음 **사용자 및 라이선스를**선택 합니다. 고객의 사용자 및 라이선스 페이지가 열립니다.

2. 사용자 라이선스를 다시 할당하려면 다시 할당할 사용자를 선택한 다음 **라이선스 관리**를 선택합니다.

3. **라이선스 관리** 페이지에서 **Office 365 Enterprise E4** 라이선스 확인란의 선택을 취소한 다음 고객을 이동할 구독의 새로운 서비스 요금제를 선택합니다.

4. **제출**을 선택합니다. 확인 페이지에 새 라이선스 할당이 나열됩니다.

5. 라이선스 다시 할당이 필요한 다른 모든 고객 사용자에 대해 같은 단계를 계속합니다.

사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.

### <a name="step-3---cancel-the-old-subscription"></a>3단계 - 이전 구독 취소

1. **파트너 센터** 메뉴에서 **고객**을 선택 합니다. 이동하려는 고객을 선택하고, 취소할 구독을 선택합니다.

2. 구독 세부 정보 페이지에서 구독 상태를 **일시 중단됨**으로 설정합니다.

3. **제출**을 선택합니다.

이전 구독이 일시 중단되고 새 구독이 활성화됩니다. 일시 중단된 구독은 120일 후 자동으로 프로비전이 해제됩니다. 이전 구독에 대해서는 고객에게 추가 비용이 발생하지 않습니다.



 



