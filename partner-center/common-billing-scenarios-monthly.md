---
title: Common monthly billing scenarios | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common scenarios in Partner Center when you use monthly billing (such as adding new subscriptions, changing license quantity, and suspending subscriptions.)
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, monthly billing, subscriptions, reconciliation file
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389621"
---
# <a name="monthly-billing-scenarios"></a>Monthly billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable if you use monthly billing in Partner Center.

## <a name="new-monthly-subscription"></a>New monthly subscription

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2018년 2월 12일    |주기 수수료   |4.00       |1        |4.00 |

2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018년 2월 13일         |2018년 3월 12일    |주기 수수료   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Change license quantity

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2018년 2월 12일    |주기 수수료   |4.00       |1        |4.00    |

2월 1일에 라이선스 수량을 1개에서 2개로 늘립니다. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2018년 2월 12일    |주기 인스턴스 비례 배분   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | 주기 인스턴스 비례 배분   |2.45       |1        |2.45    |
|2018년 2월 1일         |2018년 2월 12일    | 주기 인스턴스 비례 배분   |1.55       |2        |3.10    |
|2018년 2월 13일         |2018년 3월 12일    | 주기 인스턴스 비례 배분   |4.00       |2        |8.00    |

월별 가격은 4.00달러이고 서비스 기간(2018년 1월 13일 ~ 2018년 2월 12일)은 31일입니다. 따라서 일별 가격은 0.129달러입니다(4월 31일).

비례 배분 기간(2018년 1월 13일 ~ 2018년 1월 31일)은 19일입니다.

배분 단가 = 2.451 = 19 x 0.129

배분 기간(2018년 2월 1일 ~ 2018년 2월 12일)은 12일입니다.

배분 단가 = 1.54 = 12 x 0.129

## <a name="suspend-before-30-days"></a>Suspend before 30 days

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2018년 2월 12일    |주기 수수료   |4.00       |1        |4.00    |

On February 1 you suspend a subscription. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2018년 2월 12일|취소 요금|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Suspend after 30 days

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2018년 2월 12일|주기 수수료|4.00|1|4.00

2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018년 2월 13일|2018년 3월 12일|주기 수수료|4.00|1|4.00

3월 1일, 구독을 일시 중단합니다. 3월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018년 3월 1일|2018년 3월 12일|취소 요금|-1.72|1|-1.72

월별 가격은 4.00달러이고, 서비스 기간(2018년 2월 13일 ~ 2018년 3월 12일)은 28일입니다. 따라서 일별 가격은 0.143달러입니다(4월 28일).

단가는 서비스 기간의 일 수 x 일별 가격 x 라이선스 수입니다.

취소 기간(2018년 3월 1일 ~ 2018년 3월 12일)은 12일입니다.

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).
