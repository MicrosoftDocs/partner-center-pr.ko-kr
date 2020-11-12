---
title: Microsoft 상업적 marketplace에 대 한 지급 FAQ
description: 상업적 marketplace에서 지급에 대 한 일반적인 질문에 대 한 답변을 받으세요. 소득가 예상과 다른 이유에 대 한 답을 포함 합니다.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532024"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>상업적 marketplace 지급에 대 한 일반적인 질문

이 문서에서는 상업적 marketplace의 지급에 대 한 자주 묻는 질문에 답변 합니다.

## <a name="earnings-incorrect-or-missing"></a>소득이 잘못 되었거나 없습니다.

#### <a name="why-are-my-earnings-missing"></a>소득이 누락된 이유는 무엇인가요?

- 고객 주문이 아직 지급될 상태가 아닐 수 있습니다. 기업이 아닌 고객 주문의 경우 Microsoft는 고객 지불을 받아야 게시자에게 소득을 표시합니다. 기업 고객 주문의 경우 구매 주문 날짜로부터 1~2일 후 소득을 확인할 수 있습니다. [주문 보고서](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)의 주문 상태를 확인합니다.
- 2019년 7월 이전의 거래 소득은 거래 기록 보고서에 표시되지 않을 수 있습니다. [지급 다운로드](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)에서 기록 명세서를 확인합니다.
- [지급 cycle의 시간 프레임](payment-thresholds-methods-timeframes.md) 을 확인 하 고 수입을 지급 문에 표시할지 여부를 파악 합니다.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>수익 금액이 예상한 것과 다른 이유는 무엇 인가요?

- 주문이 부분적으로 고객에 게 지불 된 경우 빼는 요금 및 적절 한 세금 후에 부분적으로 유료 금액을 기반으로 하 게 됩니다.
- 국가별 세금을 확인 하세요. 세금을 Microsoft에서 책임지는 국가의 경우 Microsoft는 게시자 소득에서 세금을 수집하고 공제합니다. 명세서에 표시된 거래 금액은 세후 금액입니다. [세금 세부 정보](tax-details-marketplace.md)를 참조하세요.
- SaaS 및 IaaS 제품은 표준 20% 대신 10%에서 할인 된 에이전시 요금을 부과 하며, 90%의 소득 요금을 유지 합니다. 이 프로모션은 2021년 6월 30일까지 적용됩니다.

**추가** 정보: [상업적 마켓플레이스 게시자 계약](https://go.microsoft.com/fwlink/p/?LinkID=699560), [지급 정책 정보](payout-policy-details.md), [지불 임계값, 방법 및 시간 프레임](payment-thresholds-methods-timeframes.md), [상용 marketplace에서 유료](marketplace-get-paid.md), [세금 세부 정보](tax-details-marketplace.md), [지급 문](payout-statement.md), [상용 marketplace 분석의 주문 대시보드](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>소득 조정
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>지급 명세서를 분석의 주문 또는 사용 보고서에 맞게 조정하려면 어떻게 해야 하나요?
분석 주문 및 사용 현황 보고서를 사용 하 여 지급 트랜잭션 기록 보고서에 표시 되는 AssetID, orderID 및 line item ID를 사용 합니다. 이 매핑을 사용 합니다.

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>고객 주문에 대한 지불이 언제 지급될지 어떻게 알 수 있나요?
- 먼저 assetID를 사용 하 여 [주문 보고서](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)에서 고객 주문을 확인 합니다.
- 고객 [보고서](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)에서 고객 구독에 대 한 고객 채널을 확인 합니다.
- 기업 고객의 경우 게시자 소득이 구매 주문 날짜의 1-2 일 후에 표시 됩니다.
- 기업 외 고객의 경우 고객 지불을 받은 후 1-2 일 후에 게시자 소득이 표시 됩니다.

**추가** 정보: [지급 문](payout-statement.md), [상용 marketplace 분석의 주문 대시보드](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>지급 정책

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>현재 에이전시 수수료 및 지급율을 찾으려면 어떻게 해야 하나요?

- 상업용 Marketplace 게시자 계약을 확인합니다. 표준 에이전시 수수료는 20%입니다. SaaS Co-Sell 적격 트랜잭션에는 10% 할인 된 요금이 부과 됩니다. 프로모션 에이전시 수수료에 대한 공지를 확인합니다.
- 지급 문에서 Rate는 지정 된 트랜잭션에 대 한 실제 지급 rate를 지정 합니다.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>내 명세서에 소득이 표시되면 언제 Microsoft로부터 지불을 받을 수 있나요?
- 소득이 처리되지 않음 상태이면 소득이 지불 처리될 달의 만기일을 확인할 수 있습니다. 지불이 준비 되 면 획득 상태는 "처리 됨"으로 변경 됩니다.  Microsoft는 만기월 15일까지 지불을 지급합니다.
- 신용 카드로 요금을 지불 하는 주문의 경우 Microsoft는 획득이 성숙 될 때까지 30 일간 지불 합니다.

 **추가** 정보: [상업적 마켓플레이스 게시자 계약](https://go.microsoft.com/fwlink/p/?LinkID=699560), [지급 정책 세부 정보](payout-policy-details.md), [세금 정보](tax-details-marketplace.md), [지불 임계값, 방법 및 시간 프레임](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>지불 및 조정

#### <a name="why-is-my-payment-missing"></a>지불이 누락된 이유는 무엇인가요?

- [개요 페이지](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)에서 지급 상태 및 세금 프로필 상태가 *유효한* 것으로 표시 되는지 확인 합니다.
- 지불의 최소 임계값을 충족하지 못했을 수 있습니다. 지불을 받으려면 소득이 $50 USD 이상이어야 합니다.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>결제를 수신 하지 않으려면 내 계정을 설정 어떻게 할까요??
[지급 Profile](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)에서 지불을 유지할 수 있습니다. **보류** 중을 선택 하기만 하면 됩니다. Microsoft는 보류를 해제할 때까지 지불을 보유 합니다.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>구매 통화와 다른 통화로 받는 이유는 무엇인가요?

지급 통화는 지급 프로필에서 선택한 통화를 기준으로 합니다. 구매 통화는 고객이 지불한 통화를 기준으로 합니다.

#### <a name="how-do-i-reconcile-adjustments"></a>조정은 어떻게 수정하나요?

지불 조정은 시스템 문제와 같은 보정 조정을 수용하기 위한 지불 수정입니다. 지급 명세서에서 ReasonCode에는 조정 이유를 지정합니다. 이는 개별 거래에 직접 조정하기 위한 것이 아닙니다.

**추가** 정보: [상업적 마켓플레이스 게시자 계약](https://go.microsoft.com/fwlink/p/?LinkID=699560), [지급 정책 세부 정보](payout-policy-details.md), [세금 정보](tax-details-marketplace.md), [지불 임계값, 방법 및 시간 프레임](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>세금

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>지급 명세서에서 Microsoft 또는 게시자 간의 세금 납부 책임을 식별하려면 어떻게 해야 하나요?

거래 내역 다운로드에서 세금 모델 열을 찾습니다. MS 관리 또는 ISV 관리가 표시됩니다. [세금 세부 정보](tax-details-marketplace.md)에서 국가별 세금 규칙 및 지급 관련 사항을 참조하세요.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>서비스 수수료 세금 양식을 다운로드하려면 어떻게 해야 하나요?

**지급 결제** 페이지의 **지불 목록** 섹션으로 이동합니다. 서비스 수수료 세금이 있는 지불의 경우 서비스 수수료 세금 양식에 대한 링크가 나타납니다.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>원천징수세 양식을 PDF로 다운로드하려면 어떻게 해야 하나요?

*지급 결제* 페이지의 **지불 목록** 섹션으로 이동합니다. 원천징수세 양식에 대한 링크가 지불 옆에 표시됩니다.

#### <a name="where-do-i-find-year-end-tax-forms"></a>연말 세금 양식은 어디에서 찾을 수 있나요?

연말 세금 양식을 보려면 [프로필 페이지](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)로 이동합니다.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>거래에 대한 원천징수세는 어떻게 찾을 수 있나요?
원천징수세는 W-9 양식을 제출한 미국 게시자에게 적용됩니다. 원천징수세는 월별 지불로 계산됩니다.

**추가** 정보: [상업적 마켓플레이스 게시자 계약](https://go.microsoft.com/fwlink/p/?LinkID=699560), [지급 정책 세부 정보](payout-policy-details.md)

## <a name="payout-statement-access"></a>지급 문 액세스

#### <a name="how-do-i-access-a-payout-statement"></a>지급 명세서에 액세스하려면 어떻게 해야 하나요?

1. 사용자의 역할을 확인합니다. 지급 명세서에 액세스하려면 *금융 기여자* 또는 *계정 소유자* 역할이 있어야 합니다.
2. 오른쪽 위 탐색에서 **지급** 아이콘을 선택 하 여 지급 문을 확인 합니다. **트랜잭션 기록** , **지불** 및 **다운로드** 중에서 선택 합니다.

**추가** 정보: [지급 roles and permissions](payout-statement.md#roles-and-permissions), [지급 문](payout-statement.md) 

## <a name="payout-statement-report"></a>지급 문 보고서

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>거래 다운로드의 각 필드는 무엇을 의미하나요?

특성 및 해당 의미에 대 한 자세한 목록은 [지급 문을](payout-statement.md) 참조 하세요.

#### <a name="what-is-earning-status"></a>소득 상태는 무엇인가요?

그러면 수익을 처리 되지 않음, 처리 됨 또는 전송 됨으로 표시 합니다.

- **처리** 되지 않음-수입은 만기일까지 에스크로 기간에 있습니다.
- **처리** 됨 – 소득은 성숙 되며 월별 지불로 준비 됩니다. 지불액은 매월 15 일에 릴리스됩니다.
- **Sent** – 지급 프로필을 기반으로 하 여 은행이 성공적으로 출시 되었습니다.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>서비스 수수료 세금 양식을 다운로드하려면 어떻게 해야 하나요?

**지급 결제** 페이지의 **지불 목록** 섹션으로 이동합니다. 서비스 수수료 세금이 있는 지불의 경우 서비스 수수료 세금 양식에 대한 링크가 나타납니다.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>PDF로 원천 세금 양식을 다운로드 하는 어떻게 할까요?

**지급 결제** 페이지의 **지불 목록** 섹션으로 이동합니다. 원천징수세 양식에 대한 링크가 지불 옆에 표시됩니다.

#### <a name="where-do-i-find-year-end-tax-forms"></a>연말 세금 양식은 어디에서 찾을 수 있나요?

연말 세금 양식을 보려면 [프로필 페이지](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)로 이동합니다.

**추가** 정보: [지급 문](payout-statement.md), [트랜잭션 기록 다운로드](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>거래 기록 명세서

#### <a name="how-do-i-view-historical-information"></a>기록 정보를 어떻게 할까요? 볼 까 요?

기록 명세서는 2019년 10월의 지급 데이터 스냅샷을 표시합니다. 그러나 여기에서 지급 정보는 새로 고쳐지지 않습니다. 최신 정보를 받으려면 최신 데이터에 대 한 지원 티켓을 제출 합니다.

**추가** 정보: [지급 문](payout-statement.md), [트랜잭션 기록 다운로드](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>지급 내보내기 API

#### <a name="how-do-i-download-payout-data"></a>지급 데이터를 다운로드하려면 어떻게 해야 하나요?

[Partner 지급 API](https://apidocs.microsoft.com/services/partnerpayouts)를 사용 합니다.

## <a name="next-steps"></a>다음 단계

- [상업용 마켓플레이스에서 지급 받기](marketplace-get-paid.md)
