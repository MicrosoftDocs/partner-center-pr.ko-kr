---
title: 지급 일정 및 프로세스
description: Azure Marketplace 및 기타 트랜잭션의 지불 일정 및 recoupment 프로세스와 같은 지급 및 트랜잭션에 대해 알아봅니다.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582426"
---
# <a name="payout-schedules-and-processes"></a>지급 일정 및 프로세스

**적절 한 역할**: 계정 관리자 | 전역 관리자

이 문서에서는 Microsoft의 지불 일정, 지급의 상태를 찾을 수 있는 위치 및 고객 지불 하지 않는 프로세스에 대해 설명 합니다.

## <a name="payment-schedules"></a>지불 일정

다음 섹션에서는 **기업계약** 및 **Microsoft 고객 계약 또는 CSP** 트랜잭션에 대 한 지급 프로세스를 설명 합니다.

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>고객이 기업계약 경우의 트랜잭션

고객이 기존 Microsoft 기업계약 거래를 사용 하 여 Microsoft AppSource 또는 Azure Marketplace에서 제품을 구매 하는 경우 30 일 후에 다음 지급 주기 고객 청구서에서 지급를 발급 합니다. 고객이 신용 카드를 사용 하는 트랜잭션은 지급 이전에 30 일의 기간을 보유 하 고 있습니다.

지급는 Microsoft가 고객의 지불을 수집 하기 전에 종종 발생 합니다. 고객이 Microsoft 지불에 실패 했지만 이미 지급를 발급 한 경우 수행 하는 작업에 대해서는 아래에서 [지불 하지 않는 고객에 대 한 프로세스](#process-for-customer-non-payment) 를 참조 하세요.

| 이벤트 | 설명 | 보고 표시 유형 | 타이밍 |
| --- | --- | --- | --- |
| 트랜잭션 사용량 또는 월 | 고객은 서비스를 사용 하거나 구매 합니다. | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 1** |
| Microsoft에서 청구 금액을 계산 합니다. | 총 사용량, 총 트랜잭션 확인 | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 2** |
| 지급 게시 됨 | 에이전시 요금 및 지급 소득 결정 | [지급 명세서의](payout-statement.md) 트랜잭션 기록에 처리되지 않은 것으로 표시 | **3개월(첫 번째 주)** |
| 지급 준비 | 월별 지급을 위해 소득이 준비됩니다. | [지급 명세서의](payout-statement.md) 트랜잭션 기록에 예정된 것으로 표시 | **3개월(첫 번째 주)** |
| **지급 송신** | **결제가 게시자에게 전송됩니다.** | **거래 내역 및 지급 명세서의 [](payout-statement.md) 결제 섹션에 전송된 것으로 표시** | **3개월(15일 이후)** |
| 고객이 결제한 청구서 | Microsoft는 고객으로부터 결제를 수집합니다. | 변경 내용 없음 | **4개월에서 12개월** |
|

\* 지급 날짜는 태평양 표준시(PST)입니다.

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="기업계약 고객에 대한 지불 타임라인입니다.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>고객에게 Microsoft 고객 계약 또는 CSP가 있는 경우의 트랜잭션

신용 카드 또는 월별 청구서가 있는 모든 구매에는 고객으로부터 자금을 수금하기 위한 30일의 보유 기간이 있습니다.

| 이벤트 | 설명 | 보고 표시 유형 | 타이밍* |
| --- | --- | --- | --- |
| 트랜잭션 사용량 또는 월 | 고객은 서비스를 사용 하거나 구매 합니다. | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 1** |
| 고객별로 지불 된 송장 | 총 사용량, 총 트랜잭션 값 및 고객의 지불 청구서를 확인 합니다. | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 2** |
| 지급 게시 됨 | 에이전시 요금 및 지급 수익 결정 | [지급 문의](payout-statement.md) 트랜잭션 기록에서 처리 되지 않은 것으로 표시 됨 | **월 2** |
| 30 일 보관 기간 | 자금, 가능한 지불 거절 및 환불 요청 수집 보장 | [지급 문의](payout-statement.md) 트랜잭션 기록에서 처리 되지 않은 것으로 표시 됨 | **월 3** |
| 지급 준비 | 수익을 월간 지불에 대비 합니다. | [지급 문의](payout-statement.md) 트랜잭션 기록에 예정 된 것으로 표시 됨 | **월 4 (1 주)** |
| **지급 송신** | **결제가 게시자에게 전송됩니다.** | **거래 내역 및 지급 명세서의 [](payout-statement.md) 결제 섹션에 전송된 것으로 표시** | **4개월(15일 이후)** |
|

\* 지급 날짜는 태평양 표준시(PST)입니다.

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="신용 카드 및 청구서 고객에 대한 결제 타임라인입니다.":::

## <a name="process-for-customer-non-payment"></a>고객 미결제 프로세스

드문 경우지만 Microsoft는 상업용 마켓플레이스 구매에 대한 고객의 결제를 수집할 수 없습니다. 고객이 청구 일정에 따라 Microsoft에 요금을 지불하지 못하면 컬렉션 프로세스를 시작합니다. 이 프로세스는 약 4개월 정도 걸리며 Microsoft의 지속적인 통신을 포함합니다. 이 프로세스가 끝날 때까지 지불이 수신되지 않으면 Microsoft는 자금을 수집할 수 없는 금액으로 써 씁니다.

여기에 명시된 지급 프로세스에 따라 Microsoft는 궁극적으로는 수집할 수 없는 게시자(귀하)에게 이미 자금을 지급했을 수 있습니다. 따라서 이러한 금액을 조정하는 프로세스가 있습니다.

Microsoft는 다음 방법 중 하나를 사용하여 이미 지급된 모든 지급액을 회수합니다. (1) Microsoft는 향후 지급액에서 미지불 금액을 뺄 수 있습니다. 예를 들어$ 1,000달러의 지급액이 수집할 수 없는 것으로 간주되어 상환되는 경우 향후 지급액은 $1,000가 복구될 때까지 보류되거나 (2) Microsoft에서 수집되지 않은 금액에 대해 환불 또는 청구서 게시자를 요청할 수 있습니다.

다음 일정은 예제입니다.

| 이벤트 | 대략적 날짜* | 파트너 가시성 |
| --- | --- | --- |
| 지급 날짜 예 | 10/15/2020 | 지급 대시보드의 트랜잭션 기록 및 지불 섹션에 **전송으로** 표시 |
| <font color="red">고객이 Microsoft에 요금을 지불 하지 않는 경우</font> | 12/2/2020 – 12/5/2020 | 위와 동일한 변경 내용 없음 |
| 고객이 최초 지연 지불 전자 메일을 받습니다. | 12/6/2020 | 없음 |
| 고객은 긴급 한 긴급 한 전자 메일을 받습니다. | 12/7/2020 – 1/31/2021 | 없음 |
| 게시자에 게 쓰기 해제 알림이 표시 될 가능성이 있습니다. | 1/7/2021 | - |
| 고객이 종료 알림 받기 | 2/1/2021 | 없음 |
| 수집 프로세스 종료/자금을 기록 합니다. | 2/15/2021 | 금액이 쓰여진 게시자에 게 전자 메일 알림이 전송 되었습니다. |
| 지급 공제 | 3/1/2021 | 파트너 센터 지급에서 부정적 트랜잭션이 표시 됩니다. |
| 지급 보안상 이유로 | 3/15/2021 | 이후 지급는 Partner Center 지급 문에 표시 됩니다. 잔액을 더 이상 음수일 때까지 게시자는 지불을 받지 않습니다.  |
|||

\* 지급 날짜는 태평양 표준시(PST)입니다.

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>지급 계정에 도달하는 지급 일수

일반적으로 해당 월의 15일에 지정된 월의 지급액을 보내지만 결제가 계정에 도달하는 데는 또 다른 시간이 걸립니다. 일 수는 아래 설명된 대로 계정에 사용하는 결제 방법에 따라 달라집니다.

> [!NOTE]
> 아래 표시된 일수는 근사치입니다. 모든 결제는 계정에 도달하는 데 다소 시간이 걸릴 수 있습니다.

| 결제 방법     | 지급 계정에 도달할 일 수     |
|--------------------|--------------------------------------------|
| PayPal             | 영업일 기준 1일                             |
| ACH/SEPA           | 영업일 기준 2-3일                          |
| 송금      | 영업일 기준 7-10일                         |
|

## <a name="next-steps"></a>다음 단계

- [세금 세부 정보](tax-details-marketplace.md)
