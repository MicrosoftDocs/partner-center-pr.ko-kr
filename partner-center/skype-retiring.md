---
title: 비즈니스용 Skype 구독 마이그레이션
description: 비즈니스용 Skype Online 요금제 1 구독을 만료 하는 특정 고객을 새 Office 365 버전으로 마이그레이션하는 방법 및 시기에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: f395987ef647fa6f7ed264c6476ddae419eabc34
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002861"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>비즈니스용 Skype Online 계획 1 구독을 최신 Office 365 버전으로 마이그레이션

**적절한 역할**

- 영업 상담원

비즈니스용 Skype Online 요금제 1은 2018 년 8 월 1 일부 터 사용이 중지 됩니다. 이 날짜 이후에는 고객이 새 비즈니스용 Skype 요금제 1 구독을 더 이상 구매할 수 없으며 기존 구독은 만료 될 때 자동으로 갱신 되지 않으며 갱신 옵션을 제공 하지 않습니다. 구독의 세부 정보 페이지에서 비즈니스용 Skype Online 계획 1 구독 상태가 "만료 날짜 [날짜]"로 변경 되었습니다.  

고객의 연속성을 보장 하려면 아래에 나열 된 지원 되는 SKU 옵션에 대해 비즈니스용 Skype Online 요금제 1 구독을 만료 하는 고객을 전환 해야 합니다. 고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다. 

>[!NOTE]
>비즈니스용 Skype Online 요금제 1 상용 및 정부 Sku는 모두 사용이 중지 됩니다.

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 = False 속성과 함께 구독의 종료 날짜를 평가 하 여 만료 된 구독을 찾습니다. 비즈니스용 Skype Online 계획 1 구독은 2018 년 9 월 1 일에 자동 갱신 = False로 설정 됩니다. 언제 든 지 새 요금제로 고객을 이동할 수 있습니다. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>비즈니스용 Skype Online 요금제 1 교체 계획

새로운 요금제를 사용 하 여 고객이 Office 365의 새로운 기능과 기능을 활용할 수 있습니다. 가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다. 

- 옵션 1: Office 365 Enterprise F1
- 옵션 2: Microsoft 365 Enterprise F1
- 옵션 3: 다른 Office 365 요금제

|**기능**    |**옵션 1**   |**옵션 2**   |**옵션 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|비즈니스용 Skype Online 요금제 1에 포함 된 모든 기능을 가져옵니다.|예   |예   |예   |
|IM 및 현재 상태 |예   |예   |예   |
|IP를 통한 피어 투 피어 오디오 및 비디오|예   |예   |예   
|인증 된 사용자로 모임 참여| 예   |예   |예   |

## <a name="transition-customers-to-new-product-plans"></a>고객을 새 제품 요금제로 전환

Microsoft는 파트너에 게 새로운 제품과 서비스를 지속적으로 제공 합니다. 이러한 경우 고객을 새 서비스로 업그레이드 하거나 결국 종료 될 Sku에서 구독을 마이그레이션해야 할 수 있습니다. 사용 중지 된 Sku에서 최신 버전으로 고객을 마이그레이션하려면 다음 단계를 수행 해야 합니다.

- 새 구독 구매
- 현재 사용자 라이선스 다시 할당
- 이전 구독 취소

### <a name="migrate-your-customers-to-new-plans"></a>고객을 새 요금제로 마이그레이션

1. 새 구독을 구입 하려면 **파트너 센터 메뉴** 에서 **고객** 을 선택 하 고 이동할 고객을 선택한 다음 **구독 추가** 를 선택 합니다.

2. 카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출** 을 선택 합니다. 

이제 고객에 게 이전 구독과 새 구독, 이전에는 비즈니스용 Skype Online 계획 1 구독 및 새 ' 대상 ' 구독이 모두 포함 되어 있어야 합니다 (예: 옵션 1-Office 365 Enterprise F1).

3. 고객의 사용자 라이선스를 재할당 하려면 **파트너 센터** 메뉴에서 **고객** 을 선택 하 고 이동 하는 고객을 선택한 다음 **사용자 및 라이선스** 를 선택 합니다. 고객의 사용자 및 라이선스 페이지가 열립니다.

4. 사용자 라이선스를 다시 할당 하려면 재할당할 사용자를 선택한 다음 **라이선스 관리를 선택 합니다.**

5. **라이선스 관리** 페이지에서 비즈니스용 Skype Online 요금제 1 라이선스 확인란의 선택을 취소 하 고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.

6. **제출** 을 선택합니다. 확인 페이지에 새 라이선스 할당이 나열 됩니다. 라이선스를 할당 해야 하는 다른 사용자에 대해 동일한 프로세스를 계속 합니다.

사용자 라이선스를 새 서비스로 이동한 후에는 고객 수준에서 사용 중지 된 구독을 안전 하 게 취소할 수 있습니다.

7. **파트너 센터** 메뉴에서 **고객** 을 선택 합니다. 취소할 구독이 있는 고객을 선택 합니다.

8. 구독 세부 정보 페이지에서 구독을 **일시 중단 됨** 으로 설정 합니다.

9. **제출을 선택 합니다.**

이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다. 일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다. 고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.

## <a name="next-steps"></a>다음 단계

- [Advisor: 클라이언트에서 Office 365을 사용해 볼 수 있는 평가판 초대 만들기 및 보내기](advisors-create-a-trial-invitation.md)
- [Advisor: Office 365 평가판 초대 및 구매 제안을 사용 하 여 클라이언트 기반 빌드](advisors-build-your-business.md)
- [관리자: 구매 제안 만들기](advisor-create-a-purchase-offer.md)
