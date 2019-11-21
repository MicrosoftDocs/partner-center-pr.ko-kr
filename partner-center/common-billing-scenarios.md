---
title: 일반적인 청구 시나리오 | 파트너 센터
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn what you will see on your bill after you add new subscriptions, adjust the number of licenses in a subscription, or cancel a subscription.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.localizationpriority: medium
ms.openlocfilehash: d8afffa1dd11e386b03548c8f10e5490e6db5894
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253402"
---
# <a name="common-billing-scenarios"></a>일반적인 청구 시나리오

**적용 대상**

-   Cloud Solution Provider program billing

이 항목에서는 새 구독을 추가한 후, 구독의 라이선스 수를 조정한 후 또는 구독을 취소한 후 청구서에 표시되는 내용에 대해 설명합니다. 사용량 기준 및 라이선스 기준 구독에 미치는 영향은 각기 다릅니다.

## <a name="in-this-section"></a>이 섹션의 내용

-   [Usage-based billing](#usagebased)

-   [License-based billing](#licensebased)

## <a href="" id="usagebased"></a>Usage-based billing

사용량 기준 구독은 구독 연주기일에 매월 후불로 요금이 청구됩니다. For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period December 15 - January 14. You will be charged again on February 15 for the service period January 15 - February 14, etc. The charges that are generated on the subscription anniversary day will appear on the following invoice and reconciliation file.

You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice. This is not an error; it simply means that the service was timestamped after the services occurred. Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill. 

Usage-based subscriptions may be suspended at any time. 

Azure CSP 가격 목록은 매월 게시되며 파트너 센터 판매 -> 가격 책정 및 제품 페이지에서 확인할 수 있습니다. 가격은 매일 변경이 가능하며 가격 목록의 변경 기록 탭에 반영됩니다.

사용 요금은 일일 가격을 기준으로 합니다. 서비스 기간 동안 가격이 변경되면 각 비례 배분 방식 서비스 기간에 대한 청구 항목과 해당 가격이 표시됩니다.

## <a href="" id="licensebased"></a>License-based billing

**청구:** 라이선스 기준 구독은 구독 연주기일에 사전 청구됩니다.

**연주기일:** 연주기일은 구독을 구입한 달의 해당 일입니다. 예를 들어, 1월 15일에 구독을 구입했다면 매달 15일이 연주기일이 됩니다.

**기간:** 모든 라이선스 기준 구독의 결제 기간은 12개월입니다(구입 날짜부터 시작).

**취소:** 첫 달에 일시 중단된 구독은 100% 환불됩니다. 2 ~ 12개월 내에 일시 중단된 구독은 비례 배분 방식으로 환불됩니다.

**갱신:** 모든 라이선스 기준 구독은 결제 기간 시작 12개월 이후 자동 갱신됩니다.

## <a href="" id="licensebasedmonthly"></a>Monthly billing scenarios

**Scenario 1: New subscription**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2018년 2월 12일    |주기 수수료   |4.00       |1        |4.00    

2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018년 2월 13일         |2018년 3월 12일    |주기 수수료   |4.00       |1        |4.00    

**Scenario 2: Change license quantity**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2018년 2월 12일    |주기 수수료   |4.00       |1        |4.00    

2월 1일에 라이선스 수량을 1개에서 2개로 늘립니다. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2018년 2월 12일    |주기 인스턴스 비례 배분   |-4.00       |1        |-4.00    
|1/13/2018         |1/31/2018    | 주기 인스턴스 비례 배분   |2.45       |1        |2.45    
|2018년 2월 1일         |2018년 2월 12일    | 주기 인스턴스 비례 배분   |1.55       |2        |3.10    
|2018년 2월 13일         |2018년 3월 12일    | 주기 인스턴스 비례 배분   |4.00       |2        |8.00    

**Unit Price Formulas:**

The monthly price is 4.00 and there are 31 days in the service period 1/13/2018 - 2/12/2018. 따라서 일별 가격은 0.129달러입니다(4월 31일).

There are 19 days in the proration period 1/13/2018 - 1/31/2018.

배분 단가 = 2.451 = 19 x 0.129

There are 12 days in the proration period 2/1/2018 - 2/12/2018.

배분 단가 = 1.54 = 12 x 0.129

**Scenario 3: Suspend before 30 days**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 월별 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2018년 2월 12일    |주기 수수료   |4.00       |1        |4.00    

On February 1 you suspend a subscription. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2018년 2월 12일|취소 요금|-4.00|1|-4.00

**Scenario 4: Suspend after 30 days**

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

**Unit Price Formulas:**

The monthly price is 4.00 and there are 28 days in the service period 2/13/2018 - 3/12/2018. 따라서 일별 가격은 0.143달러입니다(4월 28일).

단가는 서비스 기간의 일 수 x 일별 가격 x 라이선스 수입니다.

There are 12 days in the cancellation period 3/1/2018 - 3/12/2018. 

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).

## <a name="annual-billing-scenarios"></a>연간 청구 시나리오

**Scenario 1: New subscription**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 연간 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|구매 시 비례 배분 방식 요금|48.00|1|48.00

**Scenario 2: Add license after subscription anniversary date but before billing date**

귀하가 17/2/11에 $211.20/년에 대한 라이선스 1개와 함께 새 구독을 구입합니다. 구독 연주기일은 매월 11일로 설정됩니다. Microsoft 청구 시스템에서 다음 청구 항목을 생성합니다. 

-   $211.20 charge for period 2/11/17 - 2/10/18. 

17/2/12에 두 번째 라이선스를 구입합니다. 청구 날짜는 17/2/14입니다. 송장 및 조정 파일이 생성됩니다. 조정 파일에 다음 청구 항목이 포함됩니다. 

|청구 시작 날짜  |청구 종료 날짜  |청구 유형  |단가 |Quantity | 합계 |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2017/2/11 |2018/2/10 |구매 시 비례 배분 방식 요금 |211.20 |1 | 211.20 |

구독 연주기일인 17/3/11에 Microsoft 청구 시스템은 17/2/12에 라이선스 증대에 대한 다음 청구 줄을 생성합니다. 
-   -$211.20 credit for period 2/11/17 - 2/10/18. 
-   $0.58 prorated charge per license for 1 license for period 2/11/17 - 2/11/17. 
-   $15.62 prorated charge per license for 2 licenses for period 2/12/17 - 3/10/2017. 
-   $195.00 prorated charge per license for 2 licenses for period 3/11/2017 - 2/10/2018. 

귀하가 17/2/11에 구독을 구입합니다. 17/2/12에 라이선스를 추가합니다. 청구 날짜는 17/2/14입니다. 18/2/11에 구독 갱신합니다.

다음 청구 날짜는 17/3/14이며 송장 및 조정 파일 생성됩니다. 조정 파일에 다음 청구 항목이 포함됩니다. 

|청구 시작 날짜  |청구 종료 날짜  |청구 유형  |단가 |Quantity | 합계 |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2017/2/11 |2018/2/10 |주기 인스턴스 비례 배분 |-211.20 |1 |-211.20 |
|2017/2/11 |2017/2/11 |주기 인스턴스 비례 배분 |0.58 |1 |0.58 |
|2017/2/12 |2017/3/10 |주기 인스턴스 비례 배분 |15.62 |2 |31.25 |
|2017/3/11 |2018/2/10 |주기 인스턴스 비례 배분 |195.00 |2 |390.00 |

18/2/11에는 구독이 12개월 더 갱신됩니다.


**Scenario 3: Change license quantity**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 연간 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|구매 시 비례 배분 방식 요금|48.00|1|48.00

2월 1일에 라이선스 수량을 1개에서 2개로 늘립니다. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
1/13/2018|1/12/2019|주기 인스턴스 비례 배분|-48.00|1|-48.00
1/13/2018|1/31/2018|주기 인스턴스 비례 배분|2.47|1|2.47
2018년 2월 1일|1/12/2019|주기 인스턴스 비례 배분|44.98|2|89.96

**Unit Price Formulas:**

연간 가격이 48.00이므로 일별 가격은 0.13(48.00/365)입니다.

단가는 서비스 기간의 일 수 x 일별 가격 x 라이선스 수입니다.

There are 19 days in service period 1/13/2018 - 1/31/2018. 

따라서 단위 가격 = 2.47 (19x0.13x1)입니다.

There are 346 days in service period 2/1/2018 - 1/12/2019. 

따라서 단위 가격 = 44.98 (346x0.13x2)입니다.

**Scenario 4: Suspend before 30 days**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 연간 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|구매 시 비례 배분 방식 요금|48.00|1|48.00

2월 1일, 구독을 일시 중단합니다. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|취소 요금|-48.00|1|-48.00

**Scenario 5: Suspend after 30 days**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 연간 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|구매 시 비례 배분 방식 요금|48.00|1|48.00

2월 15일 라이선스 기준 조정 파일은 이 구독에 대한 어떠한 청구 항목도 포함하지 않습니다.
3월 1일, 구독을 일시 중단합니다. 3월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018년 3월 1일|1/12/2019|취소 요금|-41.34|1|-41.34

**Unit Price Formulas:**

연간 가격이 48.00이므로 일별 가격은 0.13(48.00/365)입니다.

단가는 서비스 기간의 일 수 x 일별 가격 x 라이선스 수입니다.

There are 318 days in service period 3/1/2018 - 1/12/2019. 

따라서 단위 가격 = 41.34 (318x0.13x1)입니다. 이는 환불이므로 단가는 -41.34입니다.

**Scenario 6: Suspend and reactivate**

청구 날짜는 매월 15일입니다. 1월 13일에 $4/월에 라이선스가 하나인 새 구독을 구매하고, 연간 청구를 선택합니다. 1월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|구매 시 비례 배분 방식 요금|48.00|1|48.00

2월 1일, 구독을 일시 중단합니다. 2월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|취소 요금|-48.00|1|-48.00

3월 1일, 구독을 다시 활성화합니다. 3월 15일 라이선스 기준 조정 파일은 다음 청구 항목을 포함합니다.

|청구 시작 날짜 |청구 종료 날짜 |청구 유형 |단가 |Quantity |합계 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018년 3월 1일|1/12/2019|구매 시 비례 배분 방식 요금|41.34|1|41.34

**Unit Price Formulas:**

연간 가격이 48.00이므로 일별 가격은 0.13(48.00/365)입니다.

단가는 서비스 기간의 일 수 x 일별 가격 x 라이선스 수입니다.

There are 318 days in service period 3/1/2018 - 1/12/2019. 

따라서 단위 가격 = 41.34 (318x0.13x1)입니다.
