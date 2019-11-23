---
title: Monthly and annual billing differences | Partner Center
ms.topic: article
ms.date: 11/21/2019
Description: Differences between monthly and annual billing cycles in Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 4d6b316f55a6d2cd84959d60feed666d657893b8
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389771"
---
# <a name="monthly-and-annual-billing-differences"></a>Monthly and annual billing differences

적용 대상:

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

This topic explains the differences between **monthly billing** and **annual billing** in Partner Center, including benefits and use cases. You have the option to pay for certain Cloud Solution Provider (CSP) subscriptions on a monthly or annual basis.

## <a name="applicability"></a>적용 가능성

Most licensed-based subscriptions have the option for either monthly or annual billing option. 사용량 기준 구독에는 월별 청구 옵션만 있습니다.

Both annual and monthly billing are **per subscription**, ***not* per license**.

### <a name="find-subscription-applicability"></a>Find subscription applicability

You can identify the available billing frequencies for each offer by using column J in the offer matrix. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="applicable-partners"></a>Applicable partners

All partners and partner types can choose monthly or annual billing.

### <a name="applicable-markets"></a>Applicable markets

Monthly and annual billing (for applicable offers) are available in all markets where the CSP program is currently available.

## <a name="change-billing-frequency"></a>Change billing frequency

You can switch between monthly and annual billing at any time. You may want to change your billing frequency if your business needs change.

When you change the billing frequency to annual, the annual term is updated to reflect the date you changed the billing frequency. A new renewal date is also established.

### <a name="monthly-to-annual-billing"></a>Monthly to annual billing

Switching from monthly billing to annual billing may be useful if you have numerous subscriptions that are billed monthly. When you switch to annual billing, you can align the subscriptions to a common billing date.

### <a name="annual-to-monthly-billing"></a>Annual to monthly billing

Switching from annual billing to monthly billing may be useful if you want to adjust your billing dates to those of your individual customers.

## <a name="annual-billing"></a>Annual billing

연간 청구는 다음과 같은 이점이 있습니다.

- 결제 옵션의 유연성 증가
- 고객의 청구서 발행에 맞게 조정
- 환율 변동의 영향력 감소
- 청구 운영 비용 절감

### <a name="configure-annual-billing"></a>Configure annual billing

If you're planning to switch to annual billing in Partner Center, be sure to consider how your sales motion will be affected. You should inform your team and update your internal processes as necessary. You should also review changes to your invoice and license-based reconciliation file. 

You will also need to [update your APIs for annual billing](#required-api-changes).

#### <a name="required-api-changes"></a>Required API changes

연간 청구를 활용하기 위해 사용자 API에 필요한 변경 사항이 있습니다.

- [Order.BillingCycle property](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Create an order](https://docs.microsoft.com/partner-center/develop/create-an-order)

For more information about Partner Center APIs, see all [Partner Center developer resources and documentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placing orders

The billing frequency type, including the annual billing option, is assigned to the **Offer** as an attribute. There is not a unique offer specifically for orders with annual billing. 그러나 쉽게 구별할 수 있도록 고객에게 친숙한 이름을 사용하여 제품의 이름을 변경할 수 있습니다.

### <a name="select-annual-billing"></a>Select annual billing

When you add a new subscription, you will be prompted to choose the billing frequency. 이때 연간 청구 옵션을 선택할 수 있습니다. When you select annual billing,all available offers will be displayed.

### <a name="billing-time"></a>Billing time

다음 청구 날짜에 대금이 청구됩니다. For example, if your billing date is the 1st of the month and you purchase an annually billed subscription on October 29, 2019, you will be billed on November 1, 2019. Assuming that you make no license changes, you will be billed again on November 1, 2020. If you make a license change you will receive a credit and rebill on your next billing date.

### <a name="annual-renewals"></a>Annual renewals

Your subscription renewal date will be twelve months after the service start date. 서비스 기간은 구독을 만든 날짜에 시작됩니다.  For example, a subscription created on January 10, 2019, will be renewed on January 10, 2020.

구독 갱신 날짜 이후 다음 청구 날짜에 대금이 청구됩니다. 예를 들어 2018년 1월 15일에 연간 청구 구독을 구매하고 청구 날짜가 1월 20일인 경우 구독은 2019년 1월 15일에 갱신됩니다. 그리고 2019년 1월 20일에 갱신 대금이 청구됩니다.

### <a name="split-subscription-billing-frequency"></a>Split subscription billing frequency

It isn't possible to split a **single subscription** so that one part is billed monthly and the other part is billed annually. The entire subscription must have the same billing frequency (either monthly or annual billing).

For customers with **multiple subscriptions** of the same offer, it may be possible to have different billing frequencies per subscription. 일부 제품은 고객당 구독 하나로 제한됩니다. 제한이 없는 제품의 경우 고객은 동일한 제품으로 구성되어 있지만 청구 주기가 서로 다른 여러 구독을 구입할 수 있습니다. 제품표의 I열에서 모든 제품의 제약 및 제한 사항에 대한 세부 정보를 찾을 수 있습니다. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="free-subscription-period"></a>Free subscription period

Subscriptions with annual billing frequency do not receive a free period. The twelve-month paid term begins on the purchase date. 구매 날짜부터 다음 청구 날짜까지 무료 기간이 제공되는 월간 청구 구독과는 다릅니다.

### <a name="adding-and-removing-licenses"></a>Adding and removing licenses

언제든지 구독의 라이선스 수량을 변경할 수 있습니다. 라이선스를 추가해도 대금 청구 주기에 영향을 주지 않습니다.

언제든 라이선스 수를 추가하거나 제거할 수 있습니다.  You will receive a credit and prorated rebill on your next billing date after you change the number of licenses.

If your existing subscription has annual billing, it's not possible to add licenses with monthly billing to that subscription. 고객이 연간 청구를 사용하는 구독을 구매하면 추가 라이선스는 동일한 청구 주기를 따릅니다. 월별 구독을 사용하는 라이선스를 구매해야 하는 경우 새 구독을 구매해야 합니다.

### <a name="add-on-offers"></a>Add-on offers

추가 기능 구독에는 자동으로 상위 구독과 동일한 청구 주기가 적용됩니다. Annual billing is available for add-on offers. 

### <a name="cancelling-subscriptions"></a>Cancelling subscriptions

취소 정책은 모든 청구 주기에 동일하게 적용됩니다.

For annual billing, if the subscription is cancelled in the first 30 days of the twelve-month paid term you will receive a 100 percent credit on your next billing date. If the subscription is cancelled after 30 days of the twelve-month paid term you will receive a prorated credit on your next billing date.

### <a name="moving-subscriptions-between-partners"></a>Moving subscriptions between partners

Customers can't move subscriptions between from one partner to another. 이것은 월별 및 연간 청구 구독에 똑같이 적용됩니다.

새 파트너가 고객을 대신하여 새 구독을 구입해야 합니다. It's not possible to move subscriptions between partners.

### <a name="reactivating-subscriptions"></a>Reactivating subscriptions

You can reactivate a subscription for up to 90 days after the suspension date. 다음 청구 날짜에 비례 배분 요금이 청구됩니다. 구독 갱신 날짜는 동일하게 유지됩니다.

## <a name="pricing"></a>가격 책정

### <a name="offer-pricing"></a>Offer pricing

The offer price at time of purchase is guaranteed for the full billed subscription term (one month for monthly billing, twelve months for annual billing). 구독이 갱신되면 가격은 갱신 날짜 기준 현재 가격표에 따라 재설정됩니다. The new price is guaranteed for the next subscription term.

If an offer price decreases during the billing period, the amount you are billed for doesn't change. The price is set for the full billing period at the time of purchase. This applies to both monthly and annual billing.

### <a name="cancellation-credits"></a>Cancellation credits

Credit for a cancelled license or subscription is calculated as follows:

**Cancellation credit** = ((**monthly price***12)/365) \* **days remaining in the twelve-month term** \* number of licenses cancelled.

## <a name="reconciliation-file"></a>Reconciliation file

### <a name="find-subscriptions-billing-frequency"></a>Find subscription's billing frequency

Review your license-based reconciliation file for information on whether your subscription is billed monthly or annually. This information is in column **AA**.

To find out whether you can change a monthly subscription to annual billing, see [Find subscription applicability](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Reconciliation file changes for annual billing

When you purchase or renew a subscription with annual billing, your license-based reconciliation file will change as follows.

A new row on the license-based reconciliation file on the first billing date following the purchase or a new subscription.

구독에서 변경된 내용이 없으면 구독 기간 2~12월의 조정 파일에 아무 행도 표시되지 않습니다. If a change is made to the subscription during the twelve-month term, a credit and prorated rebill will appear on the next reconciliation file after the change is made.

The next change to the reconciliation file will appear when the subscription is renewed. 이는 갱신 이후 첫 번째 청구 날짜에 표시됩니다.

### <a name="usage-file-changes-for-annual-billing"></a>Usage file changes for annual billing

The following annually billed subscription changes appear in column P of your usage file.

- **Prorate Fees When Purchase**: the initial purchase of an annual subscription.
- **Cycle Instance Prorate**: license changes that result in credit and rebilling.
- **Cancel Fee**: the [cancellation of an annual subscription](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancellation of annual subscription

When an annually billed subscription is cancelled, the reconciliation file will contain one line item for a cancellation credit.

If the cancellation occurs in the first 30 days of the twelve-month term, the subscription will be credited at 100 percent. 처음 30일 이후에 구독을 취소할 경우 비례 배분 방식으로 계산한 금액이 환불됩니다.

### <a name="adding-licenses-to-annual-subscription"></a>Adding licenses to annual subscription

When you add licenses to a subscription, the reconciliation file will contain a credit and prorated rebill. This applies to monthly and annually billed subscriptions.

### <a name="price-lists-for-annual-billing"></a>Price lists for annual billing

Partner Center price lists show the monthly prices. There is no annual price listed. 월별 가격에 12를 곱하여 연간 가격을 계산할 수 있습니다.

### <a name="offer-matrix"></a>Offer matrix

Offer IDs in the offer matrix are the same for all billing frequencies. There are no unique IDs for offers that can be billed annually.

## <a name="incentives"></a>인센티브

### <a name="incentives-calculation"></a>Incentives calculation

Incentives are calculated based on **billed revenue**, ***not* adjusted revenue**. 획득한 인센티브는 CSP 인센티브 가이드에서 찾을 수 있는 정책에 따라 지급됩니다.

When an annually billed subscription is sold, that subscription's revenue is recognized for the calculation of incentives based on billed revenue.

### <a name="payout"></a>지급

Currently, all incentive payments are made twice a year. 분기가 끝나고 45일 이후에 지급됩니다.

### <a name="rates"></a>요금

Partners earn incentives on all eligible transactions, regardless of how a subscription is billed. Incentive earnings are calculated based on the global incentive rate (which is applied to the billed revenue for the period), the local accelerator (for all geographies in which there are local accelerators), and any global campaigns (where applicable).

### <a name="contacts"></a>연락처

For questions about incentives, contact the appropriate regional incentives support team:

| 국가 | 이메일 주소 |
| ------ | ------------- |
| 북아메리카 | <ocina@microsoft.com> |
|Latin America & Brazil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excluding Japan) | <ociapgc@microsoft.com> |
| 일본 | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspension

If you suspend an subscription (in Partner Center or through the APIs) within 30 days of purchase, you will receive a 100% credit, regardless of billing frequency.

For annual billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to December 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to December 31st.
3. The reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to December 31st.

For monthly billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to January 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to January 31st.
3. The partner reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to January 31st.
