---
title: 일회성 및 되풀이 조정 파일 | 파트너 센터
ms.topic: article
ms.date: 01/03/2020
description: 파트너 센터에서 일회성 및 되풀이 조정 파일을 이해 합니다.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6f381189fc1d8fad692ef248dcdcbf5ab8b0af43
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757236"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>일회성 및 되풀이 조정 파일

**적용 대상**

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

**적절한 역할**
-   전역 관리자
-   사용자 관리자
-   청구 관리자
-   관리자 에이전트
-   영업 에이전트

이 항목에서는 파트너 센터에서 일회성 및 되풀이 조정 파일을 읽는 방법에 대해 설명 합니다.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>일회성 및 되풀이 조정 파일의 필드

| Column | 설명 |
| ------ | ----------- |
| PartnerId | 특정 청구 엔터티에 대 한 고유 Azure Active Directory (Azure AD) 테 넌 트 식별자 (GUID 형식)입니다. 조정에는 필요 하지 않습니다. 모든 행에서 같습니다. |
| CustomerId | GUID 형식의 고유한 Azure AD 테 넌 트 식별자입니다. 고객을 식별합니다. |
| CustomerName | 파트너 센터에 보고 된 고객의 조직 이름입니다. |
| CustomerDomainName | 고객의 도메인 이름입니다. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다. *이 필드를 고객에 대 한 고유 식별자로 사용 하지 마세요. 고객/파트너는 Office 365 포털을 통해 베 니 티 또는 기본 도메인을 업데이트할 수 있습니다.* |
| CustomerCountry | 고객이 위치한 국가입니다. |
| InvoiceNumber | 지정한 트랜잭션이 표시되는 송장 번호입니다. |
| MpnId | CSP 파트너의 MPN 식별자입니다. |
| OrderId | Microsoft commerce platform의 주문에 대 한 고유 식별자입니다. 조정에 사용 되지 않습니다. |
| OrderDate | 주문이 이루어진 날짜입니다. |
| ProductId | 제품의 식별자입니다. |
| SkuId | 특정 SKU에 대 한 식별자입니다 (재고 유지 단위). |
| AvailabilityId | 특정 SKU의 가용성에 대 한 식별자입니다. 지정 된 국가, 통화, 산업 부문 등에서 SKU를 구매할 수 있는지 여부를 표시 합니다. |
| SkuName | 특정 SKU의 제목입니다. |
| ProductName | 제품 이름입니다. |
| ChargeType | 요금 또는 조정 유형입니다. |
| UnitPrice | 구입 시 가격 목록에 게시 된 단가입니다. *조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다.* |
| Quantity | 단위 수입니다. *조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다.* |
| SubTotal | 세금을 적용하기 전의 총액. 할인이 예상 합계와 일치 하는지 확인 합니다. |
| TaxTotal | 세금 금액 요금. 시장의 세금 규칙 및 특정 상황을 기준으로 합니다. |
| 총액 | 세금을 적용한 후의 총액. 송장에 세금이 부과되었는지 확인합니다. |
| Currency | 통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. 첫 번째 청구서와 일치 하는지 확인 하 고 주요 청구 플랫폼 업데이트 후에 다시 확인 합니다. |
| PriceAdjustmentDescription | 해당 할인에 대 한 설명입니다. |
| PublisherName | 제품 게시자의 이름입니다.
| PublisherId | 특정 게시자에 대 한 고유 식별자입니다. |
| SubscriptionDescription | 구독의 이름입니다. |
| SubscriptionId | Microsoft commerce platform의 구독에 대 한 고유 식별자입니다. 조정에 사용 되지 않습니다. *이 식별자는 파트너 관리 콘솔의 **구독 ID** 와 동일 하지 않습니다.* |
| ChargeStartDate | 요금 시작일. 시간은 항상 해당하는 날의 시작인 0:00입니다. |
| ChargeEndDate | 요금 종료일. 시간은 항상 해당 일의 마지막인 23:59입니다. |
| TermAndBillingcycle | 구매의 기간 및 청구 주기 (예: *1 년, 매월*). |
| EffectiveUnitPrice | 조정을 수행한 후 단가입니다. |
| (Unittype.pixel) | 구입할 단위의 유형입니다. |
| AlternateId | **주문 ID**에 대 한 대체 식별자입니다. |
| BillableQuantity | 구입 하거나 사용한 총 단위를 나타냅니다. |
| BillingFrequency | 품목을 월별 또는 일회성 청구 빈도로 설명 합니다. *이는 현재 지원 되는 값이 있는 Azure RI에 대해서만 지원 됩니다. 1 회 청구 빈도를 사용 하 여 RI를 구매한 경우 정찰 파일의이 필드가 빈 상태로 표시 됩니다.* |
| PricingCurrency | 리소스 또는 제품의 정가입니다. |
| PCToBCExchangeRate | 가격 책정 통화에서 청구 통화로 적용 되는 환율 |
| PCToBCExchangeRateDate | 청구 통화에 대 한 가격 책정 통화를 결정 하는 날짜입니다. |
| MeterDescription | 소비 라인 항목에 대 한 측정기 설명입니다. |


