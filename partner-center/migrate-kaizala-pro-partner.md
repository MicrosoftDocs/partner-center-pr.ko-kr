---
title: Microsoft365로 Kaizala Pro 구독 마이그레이션
description: Microsoft365 또는 Office 365 버전으로 Kaizala Pro 구독을 마이그레이션하는 방법에 대해 알아봅니다. 고객 전환에 대 한 자세한 내용은이 문서를 참조 하세요.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175177"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Microsoft365 또는 Office 365 버전으로 Kaizala Pro 독립 실행형 구독 마이그레이션

2020 년 7 월 1 일부 터 Microsoft는 Kaizala Pro 독립 실행형 서비스의 판매를 종료 합니다. 이 날짜 이후에는 고객이 새 Kaizala Pro 구독을 더 이상 구매할 수 없으며 기존 Kaizala Pro 구독은 만료 될 때 자동으로 갱신 되지 않습니다.

고객의 연속성을 보장 하려면 Kaizala Pro 독립 실행형 구독이 만료 된 고객을 아래에 나열 된 지원 되는 SKU 옵션으로 전환 해야 합니다. 고객에 대 한 서비스 중단을 방지 하려면 구독의 연간 종료 날짜 이전에 새 구독으로 고객을 이동 하는 것이 좋습니다.

API (CREST 또는 파트너 센터)를 사용 하는 경우 자동 갱신 속성과 false로 설정 된 구독의 종료 날짜를 평가 하 여 만료 된 구독을 검색할 수 있습니다 `auto renew = False` .

E4 구독은 `auto renew=False` 2020 년 7 월 1 일에 설정 됩니다. 언제 든 지 새 요금제로 고객을 이동할 수 있습니다.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro 독립 실행형 교체 계획

새로운 요금제를 사용 하 여 고객은 Microsoft 365의 새로운 기능을 활용할 수 있습니다. 가격 책정 정보는 파트너 센터의 가격 목록 및 제품 목록 행렬에 있습니다.

- 다음을 포함 한 [**비즈니스 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Frontline에 대 한 Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)다음을 포함 합니다.
   - Microsoft 365 F3(이전의 Microsoft 365 F1) 및 Office 365 F3
    
- 다음을 포함 한 [**Enterprise Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans) 
   - Office 365 E1
   - Microsoft 365 E3 및 Office 365 E3
   - Microsoft 365 E5 및 Office 365 E5

- 다음을 포함 하 여 [**교육용 Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365) 
    - Microsoft 365 A1 및 Office 365 A1
    - Microsoft 365 A3 및 Office 365 A3
    - Microsoft 365 A5 및 Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>고객을 새 제품 요금제로 전환

Microsoft는 파트너에 게 새로운 제품과 서비스를 지속적으로 제공 합니다. 이러한 경우 고객을 새 서비스로 업그레이드 하거나 결국 종료 될 Sku에서 구독을 마이그레이션해야 할 수 있습니다. 사용 중지 된 Sku에서 최신 버전으로 고객을 마이그레이션하려면 다음 단계를 수행 해야 합니다.

A. 새 구독 구매

B. 현재 사용자 라이선스 다시 할당

C. 이전 구독 취소


## <a name="migrate-your-customers-to-new-plans"></a>고객을 새 요금제로 마이그레이션

### <a name="a-purchase-the-new-subscription"></a>A. 새 구독 구매

1. 새 구독을 구입 하려면 **파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동할 고객을 선택한 다음 **구독 추가**를 선택 합니다.

2. 카탈로그에서 구입할 구독 (이 경우 위의 옵션 중 하나)을 선택 하 고 라이선스 수를 입력 한 다음 **제출**을 선택 합니다.

이제 고객에 게 이전 구독과 새 구독, 이전 Kaizala Pro 독립 실행형 구독 및 새로운 ' 대상 ' 구독이 모두 포함 되어 있어야 합니다 (예: 옵션 1-Office 365 Enterprise F1).

### <a name="b-reassign-current-user-licenses"></a>B. 현재 사용자 라이선스 다시 할당

1. 고객의 사용자 라이선스를 재할당 하려면 **파트너 센터** 메뉴에서 **고객**을 선택 하 고 이동 하는 고객을 선택한 다음 **사용자 및 라이선스**를 선택 합니다. 고객의 사용자 및 라이선스 페이지가 열립니다.

2. 사용자 라이선스를 다시 할당 하려면 재할당할 사용자를 선택한 다음 **라이선스 관리**를 선택 합니다.

3. **라이선스 관리** 페이지에서 Kaizala Pro 독립 실행형 라이선스 확인란의 선택을 취소 하 고 고객이 이동 하는 구독에 대 한 새 서비스 계획을 선택 합니다.

4.  **제출**을 선택합니다. 확인 페이지에 새 라이선스 할당이 나열 됩니다. 라이선스를 할당 해야 하는 다른 사용자에 대해 동일한 프로세스를 계속 합니다.

### <a name="c-cancel-old-subscription"></a>C. 이전 구독 취소

사용자 라이선스를 새 서비스로 이동한 후에는 고객 수준에서 사용 중지 된 구독을 안전 하 게 취소할 수 있습니다.

1.  **파트너 센터** 메뉴에서 **고객**을 선택 합니다. 취소할 구독이 있는 고객을 선택 합니다.

2.  구독 세부 정보 페이지에서 구독을 **일시 중단 됨**으로 설정 합니다.

3.  **제출**을 선택합니다.

이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다. 일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다. 고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.
