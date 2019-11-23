---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389681"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

적용 대상:

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| Column | 설명 |
| ------ | ----------- |
| PartnerId | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. 모든 행에서 같습니다. |
| Customer Id | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| 고객 이름 | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다. *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Customer Country | 고객이 위치한 국가입니다. |
| 송장 번호 | 지정한 트랜잭션이 표시되는 송장 번호입니다. |
| MpnId | MPN identifier of the CSP partner. |
| Reseller MpnId | MPN identifier of the reseller of record for the subscription. |
| 주문 ID | Unique identifier for an order in the Microsoft commerce platform. Not used for reconciliation. |
| 주문 날짜 | 주문이 이루어진 날짜입니다. |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | 특정 SKU의 제목입니다. |
| 제품 이름 | 제품 이름입니다. |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Subscription Description | Friendly name of a subscription. |
| 구독 ID | Unique identifier for a subscription in the Microsoft commerce platform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | 요금 시작일. 시간은 항상 해당하는 날의 시작인 0:00입니다. |
| ChargeEndDate | 요금 종료일. 시간은 항상 해당 일의 마지막인 23:59입니다. |
| Term and Billingcycle | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| 청구 유형 | 요금 또는 조정 유형입니다. |
| 단가 | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effective Unit Price | The unit price after adjustments have been made. |
| Quantity | Number of units. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Unit type | The type of unit being purchased. |
| DiscountDetails | An explanation of any applicable discount. |
| Sub Total | 세금을 적용하기 전의 총액. Checks if your subtotal matches your expected total, in case of a discount. |
| Tax Total | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| 총액 | 세금을 적용한 후의 총액. 송장에 세금이 부과되었는지 확인합니다. |
| Currency | 통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
