---
title: Common billing scenarios for one-time and select recurring purchases | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common billing scenarios in Partner Center for one-time and select recurring purchases (such as purchasing subscriptions, adding more subscriptions, adding and removing seats).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, one-time purchase, recurring purchase, subscriptions, seats
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389641"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>One-time and select recurring purchase billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable to [one-time and select recurring charges](one-time-and-recurring-billing.md) in Partner Center.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Purchase a subscription and add a seat on the same day

시나리오 1에서 6월 11일에 단가 $4로 구독을 하나 구매합니다. 이후에 같은 날짜에 같은 구독을 같은 가격으로 하나 더 구매합니다.

조정 파일에는 다음 정보가 포함됩니다.

- 서비스 기간 6월 10일 - 7월 9일의 요금 $4 청구
- 서비스 기간 6월 11일 - 6월 11일의 비례 배분 요금 $-4.00 재청구 이 기간에는 라이선스가 1개 있습니다. 계산 = (월 가격/총 서비스 기간 일 수) x 비례 배분 서비스 기간 일 수 x 라이선스 수량 = (4/30) x 30 x 1 = 4.00.
- 서비스 기간 6월 10일 - 7월 9일의 비례 배분 요금 $8.00 재청구 이 기간에는 라이선스가 2개 있습니다. 계산 = (4/30) x 30 x 2 = 8.00.

|**구매 날짜**   |**청구 시작** |**청구 종료**  |**단가**  |**수량**  |**합계** |**청구 유형** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/09         |$4                |1                 |$4            |신규 항목         |
|2019/6/11     | 2019/6/10    |2019/7/09        |$4        |1        | -$4       |addQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/09        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Purchase a subscription and add more subscriptions later

시나리오 2에서는 6월 11일에 단가 $4로 구독을 하나 구매하고, 6월 12일에 같은 제품의 구독을 같은 가격으로 하나 더 구매합니다.

조정 파일에는 다음 정보가 포함됩니다.

- 서비스 기간 6월 10일 - 7월 9일의 요금 $4 청구
- 서비스 기간 6월 11일 - 6월 12일의 비례 배분 요금 $-3.87 재청구 이 기간에는 라이선스가 1개 있습니다. 계산 = (월 가격/총 서비스 기간 일 수) x 비례 배분 서비스 기간 일 수 x 라이선스 수량 = (4/30) x 29 x 1 = 3.87.
- 서비스 기간 6월 12일 - 7월 9일의 비례 배분 요금 $7.74 재청구 이 기간에는 라이선스가 2개 있습니다. 계산 = (4/30) x 29 x 2 = 7.74.

|**구매 날짜**   |**청구 시작** |**청구 종료**  |**단가**  |**수량**  |**합계** |**청구 유형** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11(라이선스 1개)     |2019/6/10   |2019/7/09         |$4         |1        |$4            |신규 항목         |
|2019/6/12     | 2019/6/10    |2019/7/09        |$4        |1        | -$3.87       |addQuantity           |
|2019/6/12     | 2019/6/10    |2019/7/09        |$4        | 2      |$7.74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Purchase a subscription and remove a seat on the same day

시나리오 3에서는 6월 11일에 동일한 제품의 구독 2개를 단가 $4에 구매합니다. 이후에 같은 날짜에 시트 중 하나를 제거합니다.  

조정 파일에는 다음 정보가 포함됩니다.

- 서비스 기간 6월 10일 - 7월 9일의 2개 라이선스 요금 $8 청구
- 서비스 기간 6월 11일 - 6월 11일의 비례 배분 요금 $-8.00 재청구 이 기간에는 라이선스가 2개 있습니다. 계산 = (월 가격/총 서비스 기간 일 수) x 비례 배분 서비스 기간 일 수 x 라이선스 수량 = (4/30) x 30 x 2 = 8.00.
- 서비스 기간 6월 11일 - 7월 9일의 비례 배분 요금 $4.00 재청구 이 기간에는 라이선스가 1개 있습니다. 계산 = (4/30) x 30 x 1 = 4.00.

|**구매 날짜**   |**청구 시작** |**청구 종료**  |**단가**  |**수량**  |**합계** |**청구 유형** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/09         |$4                |2                 |$8            |신규 항목         |
|2019/6/11     | 2019/6/10    |2019/7/09        |$4        |2        | -$8       |removeQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/09        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Purchase a subscription and remove seats later

시나리오 4에서는 6월 11일에 구독 2개를 단가 $4에 구매하고, 6월 12일에 시트 중 하나를 제거합니다.

조정 파일에는 다음 정보가 포함됩니다.

- 서비스 기간 6월 10일 - 7월 9일의 요금 $8 청구
- 서비스 기간 6월 11일 - 6월 12일의 비례 배분 요금 $-7.74 재청구 이 기간에는 라이선스가 2개 있습니다. 계산 = (월 가격/총 서비스 기간 일 수) x 비례 배분 서비스 기간 일 수 x 라이선스 수량 = (4/30) x 29 x 2 = 7.74.
- 서비스 기간 6월 12일 - 7월 9일의 비례 배분 요금 $3.87 재청구 이 기간에는 라이선스가 1개 있습니다. 계산 = (4/30) x 29 x 1 = 3.87.

|**구매 날짜**   |**청구 시작** |**청구 종료**  |**단가**  |**수량**  |**합계** |**청구 유형** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11(라이선스 2개)     |2019/6/10   |2019/7/09         |$4         |2        |$8       |신규 항목       |
|2019/6/12     | 2019/6/10    |2019/7/09        |$4        |2        | -$7.74       |removeQuantity           |
|2019/6/12(라이선스 1개)    | 2019/6/10    |2019/7/09   |$4    |1      |$3.87    |removeQuantity |
