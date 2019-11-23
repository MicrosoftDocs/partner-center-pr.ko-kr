---
title: 고객에게 Microsoft 제품 평가판 제공 | 파트너 센터
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객은 30일 동안 Microsoft 구독 제품을 시험 사용할 수 있습니다. You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384838"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>고객에게 Microsoft 제품의 평가판 제공

적용 대상:

- 파트너 센터

고객에게 Microsoft 신제품을 소개하는 좋은 방법은 30일 무료 평가판을 제공하는 것입니다. 여러 다른 온라인 서비스와 마찬가지로 카탈로그에서 평가판을 등록할 수 있습니다. 모든 파트너가 참여할 수 있습니다.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. 예를 들어 고객은 Office 365 Business Premium 및 Office 365 E3의 평가판을 각각 한 번씩 받을 수 있습니다. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

평가판은 다음 제품에 제공됩니다.

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility 및 Security E5
- Dynamics 365 고객 참여 계획 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Microsoft는 가장 광범위하게 인기를 끌고 있는 비즈니스 제품의 평가판을 제공합니다. 앞으로 평가판 제품이 더 추가될 가능성이 있습니다.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. 카탈로그에서 **청구 주기**에 있는 **평가판 제품**을 클릭합니다. 이렇게 하면 무료 평가판만 표시되고 무료가 아닌 제품은 표시되지 않습니다. 평가판은 카탈로그의 **평가판** 탭에 표시됩니다.
3. 제공할 무료 평가판을 선택한 다음 **제출**을 선택합니다. 모든 평가판은 30일 동안 요금이 청구되지 않습니다. 또한 평가판 기간 중 언제든지 유료 구독으로 변환할 수 있습니다.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. 고객의 구독 페이지로 이동하여 무료 평가판을 선택합니다.
2. **무료 평가판을 유료 구독으로 전환**을 선택합니다.
3. 원하는 라이선스 수량 및 청구 주기를 입력하고 **적용**을 선택합니다.
4. 유료 구독에 대한 청구는 전환 날짜부터 시작되고, 구독은 전환 날짜로부터 12개월 후 자동 갱신됩니다. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [평가판 구독을 유료로 전환](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [사용 가능한 평가판 전환 목록 보기](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. 고객의 결정 시점이 다가오면 적절한 후속 조치를 취할 수 있도록 이러한 날짜를 자주 모니터링하는 것이 좋습니다.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>청구

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. 평가판이 연간 청구를 통한 유료 제품으로 전환되는 경우 구독 갱신 날짜는 전환 날짜로부터 12개월 이후입니다. 평가판이 월별 청구를 통한 유료 제품으로 전환되는 경우 구독 갱신 날짜는 전환 날짜 이후 청구 날짜로부터 12개월 이후입니다.

### <a name="invoices"></a>송장

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>인센티브

Free trials do not have an impact on incentives.

## <a name="support"></a>지원

For support on free trials, submit a service request through Partner Center.
