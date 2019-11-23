---
title: License-based reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand license-based reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 617b49556851a4d9999e6294d61d79c4fe1befa1
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389821"
---
# <a name="license-based-reconciliation-files"></a>라이선스 기준 조정 파일

적용 대상:

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

To reconcile your changes against a customer's orders, compare the **Syndication_Partner_Subscription_Number** from the reconciliation file against the **Subscription ID** from Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Fields in license-based reconciliation files

| Column | 설명 | 샘플 값 |
| ------ | ----------- | ------------ |
| PartnerId | Unique identifier in GUID format for a specific billing entity. Not required for reconciliation. 모든 행에서 같습니다. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerID | Unique Microsoft identifier for the customer in GUID format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| OrderID | Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다. May be useful to identify the order when contacting support. Not used for reconciliation. | *566890604832738111* |
| SubscriptionID | Microsoft 청구 플랫폼에서 구독의 고유 식별자. May be useful to identify the subscription when contacting support. Not used for reconciliation. *This value is not the same as the **Subscription ID** on the Partner Admin Console. Please see **SyndicationPartnerSubscriptionNumber** instead.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | 구독의 고유 식별자. A customer can have multiple subscriptions for the same plan. This column is important for reconciliation file analysis. This field maps to the **Subscription ID** in the Partner Admin Console. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferID | Unique offer identifier. Standard offer identifier, as defined in the price list. *This value does not match **Offer ID** from the price list. See **DurableOfferID** instead.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Unique durable offer identifier, as defined in the price list. *This value matches the **Offer ID** from the price list.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 고객이 구매한 서비스 제품의 이름(가격표에 정의됨). | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | The subscription start date. 시간은 항상 해당하는 날의 시작인 0:00입니다. This field is set to the day after the order was submitted. Used in conjunction with the **SubscriptionEndDate** to determine: if the customer is still within the first year of the subscription, or if the subscription has been renewed for the following year. | *2/1/2019 0:00* |
| SubscriptionEndDate | The subscription end date. 시간은 항상 해당하는 날의 시작인 0:00입니다. Either *12 months plus **x** days after the start date* to align with the partner's billing date or *12 months from the renewal date*. 갱신 시 가격은 현재 가격표로 업데이트됩니다. 자동 갱신에 앞서 고객과 연락해야 할 수 있습니다. | *2/1/2019 0:00* |
| ChargeStartDate | 요금 시작일. 시간은 항상 해당하는 날의 시작인 0:00입니다. Used to calculate daily charges (*pro rata* charges) when a customer changes seat numbers. | *2/1/2019 0:00* |
| ChargeEndDate | 요금 종료일. 시간은 항상 해당 일의 마지막인 23:59입니다. Used to calculate daily charges (*pro rata* charges) when a customer changes seat numbers. | *2/28/2019 23:59* |
| ChargeType | The [type of charge](recon-file-charge-types.md) or adjustment. | See [charge types](recon-file-charge-types.md). |
| UnitPrice | 실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음. Be sure this matches the information stored in your billing system during reconciliation. | *6.82* |
| Quantity | 실제 사용자 수. Be sure this matches the information stored in your billing system during reconciliation. | *2* |
| 합계 | 수량의 가격 합계. Used to check if the amount calculation matches how you calculate this value for your customers. | *13.32* |
| TotalOtherDiscount | 이러한 요금에 적용된 할인 금액. Product licenses included with a competency or MAPS, or new subscriptions eligible for an incentive, will also contain a discount amount in this column. | *2.32* |
| Subtotal | 세금을 적용하기 전의 총액. Checks if your subtotal matches your expected total, in case of a discount. | *11* |
| Tax | Tax amount charge. Based on your market's tax rules and specific circumstances. | *0* |
| TotalForCustomer | 세금을 적용한 후의 총액. 송장에 세금이 부과되었는지 확인합니다. | *11* |
| Currency | 통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. Check if it matches your first invoice. Check again after any major billing platform updates. | *EUR* |
| CustomerName | Customer's organization name, as reported in Partner Center. *Very important field for reconciling the invoice with your system information.* | *Test Customer A* |
| MPNID | MPN identifier of the CSP partner. See [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMPNID | MPN identifier of the reseller of record for the subscription. See [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| DomainName | Customer's domain name. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다. *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* | *example.onmicrosoft.com* |
| SubscriptionName | 구독 애칭. If no nickname is specified, Partner Center uses the **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | 고객이 구매한 서비스 제품의 이름(가격표에 정의됨). (This is an identical field to **OfferName**.) | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
