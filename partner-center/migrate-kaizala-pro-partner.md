---
title: Microsoft 365로 Kaizala Pro 구독 마이그레이션
description: Kaizala Pro 구독을 Microsoft 365 또는 Office 365 버전으로 마이그레이션하는 방법을 알아봅니다. 고객 전환에 대한 자세한 내용은 이 문서를 읽어보세요.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146428"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Kaizala Pro 독립 실행형 구독을 Microsoft 365 또는 Office 365 버전으로 마이그레이션

**적절한 역할:** 영업 에이전트

2020년 7월 1일부터 Microsoft는 Kaizala Pro 독립 실행형 서비스의 판매를 종료합니다. 고객은 이 날짜 이후에 더 이상 새 Kaizala Pro 구독을 구매할 수 없으며 기존 Kaizala Pro 구독은 만료되면 자동으로 갱신되지 않습니다.

고객의 연속성을 보장하려면 만료된 Kaizala Pro 독립 실행형 구독이 있는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다. 고객의 서비스 중단을 방지하려면 구독의 연간 종료 날짜 이전에 고객을 새 구독으로 이동하는 것이 좋습니다.

API(CREST 또는 파트너 센터)를 사용하는 경우 false로 설정된 자동 갱신 속성과 함께 구독의 종료 날짜를 평가하여 만료되는 구독을 검색할 수 `auto renew = False` 있습니다.

E4 구독은 `auto renew=False` 2020년 7월 1일에 로 설정됩니다. 언제든지 고객을 새 플랜으로 이동할 수 있습니다.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro 독립 실행형 교체 계획

새 플랜을 통해 고객은 Microsoft 365 새로운 기능과 기능을 활용할 수 있습니다. 가격 책정 세부 정보는 파트너 센터 가격표 및 제품 목록 매트릭스에 있습니다.

- [**다음을 포함하여 비즈니스용 Microsoft 365.**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**다음을 포함하여 Frontline에 대한 Microsoft 365.**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)
   - Microsoft 365 F3(이전의 Microsoft 365 F1) 및 Office 365 F3
    
- [**엔터프라이즈용 Microsoft 365:**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans) 
   - Office 365 E1
   - Microsoft 365 E3 및 Office 365 E3
   - Microsoft 365 E5 및 Office 365 E5

- [**교육용 Microsoft 365:**](https://www.microsoft.com/education/buy-license/microsoft365) 
    - Microsoft 365 A1 및 Office 365 A1
    - Microsoft 365 A3 및 Office 365 A3
    - Microsoft 365 A5 및 Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>고객을 새 제품 플랜으로 전환

Microsoft는 파트너에게 지속적으로 새 제품 및 서비스를 제공합니다. 이러한 경우 고객을 새 서비스로 업그레이드하거나 최종적으로 종료될 S SKU에서 구독을 마이그레이션해야 할 수 있습니다. 사용 중지된 S SKU에서 최신 S SKU로 고객을 마이그레이션하려면 다음 단계가 필요합니다.

A. 새 구독 구매

B. 현재 사용자 라이선스 재할당

C. 이전 구독 취소


## <a name="migrate-your-customers-to-new-plans"></a>고객을 새 플랜으로 마이그레이션

### <a name="a-purchase-the-new-subscription"></a>A. 새 구독 구매

1. 새 구독을 구매하려면 **파트너 센터** 메뉴에서 **고객을** 선택하고 이동하려는 고객을 선택한 다음 구독 **추가를 선택합니다.**

2. 카탈로그에서 구매할 구독(이 경우 위의 옵션 중 하나)을 선택하고 라이선스 수를 입력한 다음, **제출을** 선택합니다.

이제 고객에게 이전 및 새 구독, 이전 Kaizala Pro 독립 실행형 구독 및 새 '대상' 구독(예: 옵션 1 - Office 365 Enterprise F1)이 있어야 합니다.

### <a name="b-reassign-current-user-licenses"></a>B. 현재 사용자 라이선스 재할당

1. 고객의 라이선스를 다시 할당하려면 **파트너 센터** 메뉴에서 **고객을** 선택하고 이동 중인 고객을 선택한 다음 사용자 **및 라이선스를** 선택합니다. 고객의 사용자 및 라이선스 페이지가 열립니다.

2. 사용자 라이선스를 다시 할당하려면 재할당할 사용자를 선택한 **다음, 라이선스 관리를 선택합니다.**

3. 라이선스 **관리** 페이지에서 Kaizala Pro 독립 실행형 라이선스 확인란의 선택을 취소하고 고객이 이동하는 구독에 대한 새 서비스 계획을 선택합니다.

4.  **제출** 을 선택합니다. 확인 페이지에 새 라이선스 할당이 나열됩니다. 라이선스 할당이 필요한 다른 사용자에 대해 동일한 프로세스를 계속합니다.

### <a name="c-cancel-old-subscription"></a>C. 이전 구독 취소

사용자 라이선스를 새 서비스로 이동한 후 고객 수준에서 사용 중지된 구독을 안전하게 취소할 수 있습니다.

1.  **파트너 센터** 메뉴에서 **고객을** 선택합니다. 취소할 구독이 있는 고객을 선택 합니다.

2.  구독 세부 정보 페이지에서 구독을 **일시 중단 됨** 으로 설정 합니다.

3.  **제출** 을 선택합니다.

이전 구독이 일시 중단 되었고 새 구독은 활성 상태입니다. 일시 중단 된 구독은 120 일 후에 자동으로 프로 비전 해제 됩니다. 고객은 이전 구독에 대 한 추가 비용 없이 발생 합니다.
