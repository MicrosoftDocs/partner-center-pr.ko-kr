---
title: 지급 일정 및 정책 세부 정보-Azure marketplace
description: 일정 및 recoupment를 포함 하 여 상업적 marketplace 지급 정책과 관련 된 세부 정보에 대해 알아봅니다.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: bd8153ffd368c1f67b27eaeb44d383409bd59e97
ms.sourcegitcommit: 2e880efb02a48afc4f234ec27da34519407f87c6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96513300"
---
# <a name="payout-schedules-and-policy-details"></a>지급 일정 및 정책 세부 정보

이 문서에서는 Microsoft의 지급 process, 지급 schedule, 지급 상태를 찾을 수 있는 위치 및 고객 지불 하지 않는 프로세스에 대해 설명 합니다.

## <a name="payment-schedules"></a>지불 일정

다음 섹션에서는 **기업계약** 및 **신용 카드/송장** 거래에 대 한 지급 프로세스를 설명 합니다.

### <a name="enterprise-agreement-transactions"></a>기업계약 트랜잭션

고객이 기존 Microsoft 기업계약 거래를 사용 하 여 Microsoft AppSource 또는 Azure Marketplace에서 제품을 구매 하는 경우 30 일 후에 다음 지급 주기 고객 청구서에서 지급를 발급 합니다. 고객이 신용 카드를 사용 하는 트랜잭션은 지급 이전에 30 일의 기간을 보유 하 고 있습니다.

지급는 Microsoft가 고객의 지불을 수집 하기 전에 종종 발생 합니다. 고객이 Microsoft 지불에 실패 했지만 이미 지급를 발급 한 경우 수행 하는 작업에 대해서는 아래에서 [지불 하지 않는 고객에 대 한 프로세스](#process-for-customer-non-payment) 를 참조 하세요.

| 이벤트 | Description | 보고 표시 유형 | 타이밍 |
| --- | --- | --- | --- |
| 트랜잭션 사용량 또는 월 | 고객은 서비스를 사용 하거나 구매 합니다. | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 1** |
| Microsoft에서 청구 금액을 계산 합니다. | 총 사용량, 총 트랜잭션 확인 | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 2** |
| 지급 게시 됨 | 에이전시 요금 및 지급 수익 결정 | [지급 문의](payout-statement.md) 트랜잭션 기록에서 처리 되지 않은 것으로 표시 됨 | **월 3 (1 주)** |
| 지급 준비 | 수익을 월간 지불에 대비 합니다. | [지급 문의](payout-statement.md) 트랜잭션 기록에 예정 된 것으로 표시 됨 | **월 3 (1 주)** |
| **지급 전송** | **지불은 게시자에 게 전송 됩니다.** | **트랜잭션 기록에 전송 됨으로 표시 되 고 [지급 문의](payout-statement.md) 지불액 섹션에** | **월 3 (15 분 이후)** |
| 고객별로 지불 된 송장 | Microsoft는 고객의 지불을 수집 합니다. | 변경 내용 없음 | **월 4 ~ 12** |
|

\* 지급 날짜는 태평양 표준시 (PST)입니다.

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="기업 계약 고객의 지불 타임 라인입니다.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>신용 카드 또는 송장이 있는 트랜잭션 (확인/유선)

신용 카드나 월간 청구서를 사용 하는 모든 구매 기간은 고객 으로부터 자금을 수집할 수 있도록 30 일 동안 유지 됩니다.

| 이벤트 | Description | 보고 표시 유형 | 타이밍 |
| --- | --- | --- | --- |
| 트랜잭션 사용량 또는 월 | 고객은 서비스를 사용 하거나 구매 합니다. | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 1** |
| 고객별로 지불 된 송장 | 총 사용량, 총 트랜잭션 값 및 고객의 지불 청구서를 확인 합니다. | [사용량](/azure/marketplace/partner-center-portal/usage-dashboard) 또는 [주문](/azure/marketplace/partner-center-portal/orders-dashboard) 대시보드 | **월 2** |
| 지급 게시 됨 | 에이전시 요금 및 지급 수익 결정 | [지급 문의](payout-statement.md) 트랜잭션 기록에서 처리 되지 않은 것으로 표시 됨 | **월 2** |
| 30 일 보관 기간 | 자금, 가능한 지불 거절 및 환불 요청 수집 보장 | [지급 문의](payout-statement.md) 트랜잭션 기록에서 처리 되지 않은 것으로 표시 됨 | **월 3** |
| 지급 준비 | 수익을 월간 지불에 대비 합니다. | [지급 문의](payout-statement.md) 트랜잭션 기록에 예정 된 것으로 표시 됨 | **월 4 (1 주)** |
| **지급 전송** | **지불은 게시자에 게 전송 됩니다.** | **트랜잭션 기록에 전송 됨으로 표시 되 고 [지급 문의](payout-statement.md) 지불액 섹션에** | **월 4 (15 분 이후)** |
|

\* 지급 날짜는 태평양 표준 시간 (PST)입니다.

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="신용 카드 및 청구서 고객에 대 한 지불 타임 라인입니다.":::

## <a name="process-for-customer-non-payment"></a>고객이 지불 하지 않는 프로세스

드문 경우 지만 Microsoft는 상업적 marketplace 구매에 대 한 고객의 지불을 수집할 수 없습니다. 고객이 청구 일정에 따라 Microsoft를 지불 하지 못할 경우 수집 프로세스를 시작 합니다. 이 프로세스는 약 4 개월 후 Microsoft의 지속적인 통신을 포함 합니다. 이 프로세스의 끝에서 지불을 받지 못한 경우 Microsoft는 자금을 수집 안 함으로 작성 합니다.

여기에서 지급 프로세스에 따라 Microsoft는 궁극적으로 수집 되지 않는 게시자 (사용자)에 게 자금을 이미 지불 했을 수 있습니다. 따라서 이러한 크기를 조정 하는 프로세스가 있습니다. (이미 받은) 지불이 조정 될 수 있다는 경고를 표시 하기 위해 고객이 컬렉션 프로세스에 있을 때 구매할 가능성이 있는 경우 알림이 표시 됩니다.

Microsoft는 다음 방법 중 하나를 사용 하 여 이미 지불한 모든 지급을 recoup 합니다. (1) Microsoft는 향후 지급에서 미지불 금액을 뺄 수 있습니다. 예를 들어 지급의 $1000이 수집 되지 않는 것으로 간주 되는 경우 $1000이 복구 될 때까지 이후 지급 보안상 이유로, (2) Microsoft는 수집 되지 않은 금액에 대해 환불 또는 송장 게시자를 요청할 수 있습니다.

예제 일정은 다음과 같습니다.

| 이벤트 | 대략적인 날짜 * | 파트너 표시 유형 |
| --- | --- | --- |
| 예제 지급 날짜 | 10/15/2020 | 트랜잭션 기록에 **전송** 됨으로 표시 되 고 지급 대시보드의 지불 섹션 |
| <font color="red">고객이 Microsoft에 요금을 지불 하지 않는 경우</font> | 12/2/2020 – 12/5/2020 | 위와 동일한 변경 내용 없음 |
| 고객이 최초 지연 지불 전자 메일을 받습니다. | 12/6/2020 | None |
| 고객은 긴급 한 긴급 한 전자 메일을 받습니다. | 12/7/2020 – 1/31/2021 | None |
| 게시자에 게 쓰기 해제 알림이 표시 될 가능성이 있습니다. | 1/7/2021 | 고객이 결제를 아직 보내지 않은 게시자에 게 전자 메일 알림이 전송 되었습니다. 트랜잭션 ID 및 달러 금액이 포함 됩니다. |
| 고객이 종료 알림 받기 | 2/1/2021 | None |
| 수집 프로세스 종료/자금을 기록 합니다. | 2/15/2021 | 금액이 쓰여진 게시자에 게 전자 메일 알림이 전송 되었습니다. 트랜잭션 ID 및 달러 금액이 포함 됩니다. |
| 지급 공제 | 3/1/2021 | 파트너 센터 지급에서 부정적 트랜잭션이 표시 됩니다. |
| 지급 보안상 이유로 | 3/15/2021 | 이후 지급는 Partner Center 지급 문에 표시 됩니다. 잔액을 더 이상 음수일 때까지 게시자는 지불을 받지 않습니다.  |
|||

\* 지급 날짜는 태평양 표준 시간 (PST)입니다.

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>지급 계정에 도달 하기 위한 지불 일 수

일반적으로 해당 월의 15 일에 지정 된 월에 지불을 전송 하지만 계정에 도달 하는 데는 추가 시간이 소요 됩니다. 일 수는 아래에 설명 된 대로 계정에 사용 하는 결제 방법에 따라 달라 집니다.

> [!NOTE]
> 아래 표시 된 일은 대략적입니다. 결제는 계정에 도달 하는 데 시간이 오래 걸릴 수 있습니다.

| 결제 방법     | 지급 계정에 도달할 일 수     |
|--------------------|--------------------------------------------|
| PayPal             | 영업일 기준 1일                             |
| ACH/SEPA           | 영업일 기준 2-3일                          |
| 회선 전송      | 영업일 기준 7-10일                         |
|

## <a name="next-steps"></a>다음 단계

- [세금 세부 정보](tax-details-marketplace.md)
