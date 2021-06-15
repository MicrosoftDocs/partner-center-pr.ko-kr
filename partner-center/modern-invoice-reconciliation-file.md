---
title: CSP 일회성 구매에 대한 다시 파일 필드
ms.topic: conceptual
ms.date: 01/29/2021
description: 샘플 값을 포함하여 파트너 센터 CSP 일회성 구매 조정 파일의 모든 항목에 대해 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073801"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP 일회성 구매 조정 파일 필드

**적절한 역할:** 계정 관리자 | 청구 에이전트

## <a name="using-the-recon-file"></a>recon 파일 사용
아래 표에서는 CSP 일회성 구매에 대한 조정 파일의 필드에 대한 설명 및 샘플 값을 제공합니다.

조정 파일에 대한 자세한 내용은 [조정 파일 사용을 참조하세요.](use-the-reconciliation-files.md)

| 열 | Description | 샘플 값 |
| ------ | ----------- | ------------ |
| PartnerId | 특정 청구 엔터티에 대한 GUID 형식의 고유 식별자입니다. 조정에 필요하지 않습니다. 모든 행에서 동일합니다. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | GUID 형식의 고객에 대한 고유한 Microsoft 식별자입니다. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | 파트너 센터에 보고된 고객의 조직 이름입니다. 이 열은 청구서를 시스템 정보와 조정하는 데 중요합니다. | *Johnny Modern Cust DE2* |
| CustomerDomainName | 고객의 도메인 이름입니다. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | 고객이 있는 국가입니다. 해당 지역의 전체 [국가 목록을](./regional-authorization-overview.md) 참조하세요.  | *드* |
| InvoiceNumber | 조정 파일과 연결된 청구서 번호입니다.  | *G002297372* |
| MpnId | CSP 파트너의 MPN 식별자입니다. 자세한 내용은 [파트너별로 항목을 지정하는 방법을 참조하세요.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | 구독에 대한 레코드의 대리점에 대한 MPN 식별자입니다. | *6048879* |
| OrderID | Microsoft 청구 플랫폼에서 사용되는 주문의 고유 식별자입니다. 지원 담당자에게 문의할 때 주문을 식별하는 데 유용할 수 있습니다. 조정에 사용되지 않습니다. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | 주문이 배치된 UTC 날짜입니다. | *10/3/2020* |
| ProductId | 제품의 고유 식별자입니다. | *DZH318Z0BNZ5* |
| SkuId | SKU 고유 식별자입니다. | *006G* |
| AvailabilityId | 가용성 고유 식별자입니다. | *DZH318Z08B80* |
| SkuName | SKU 이름입니다. | *테이블 - LRS* |
| ProductName | 제품 이름입니다. | *테이블* |
| ChargeType | 요금 또는 조정 [유형입니다.](./recon-file-charge-types.md) | *새로 만들기* |
| UnitPrice | 구매 시 가격표에 게시된 라이선스당 가격입니다. 조정하는 동안 청구 시스템에 저장된 정보와 일치하는지 확인합니다. | *0.045* |
| 수량 | 라이선스 수입니다. 조정하는 동안 청구 시스템에 저장된 정보와 일치하는지 확인합니다. | *1* |
| 소계 | 세금 이전의 합계입니다. 소계는 유효 단가를 곱한 청구 가능 수량과 같아야 합니다. | *0* |
| TaxTotal | 세금 금액 청구. 시장의 세금 규칙 및 특정 상황에 따라 | *0* |
| 합계 | 총 금액은 소계에 세금 금액을 더한 금액과 같습니다. | *0* |
| 통화 | 청구서는 고객 통화의 컨텍스트에서 생성됩니다. 즉, 청구 가능한 통화가 다른 고객과 거래하는 파트너인 경우 각 고객 통화 형식에 대한 청구서를 받습니다.  | *Eur* |
| PriceAdjustmentDescription | 단가 조정 이유입니다. 이것이 주요 이유이지만 유효 단가를 결정하는 데만 국한되지는 않습니다. | *["관리되는 서비스에 대한 15.0% 파트너 획득 크레딧"]* |
| PublisherName | 제품의 게시자입니다.  | *Microsoft* |
| PublisherId | 파트너 센터 게시자를 식별하는 데 사용하는 고유 식별자입니다. | *Na* |
| SubscriptionDescription | 가격표에 정의된 대로 고객이 구매한 서비스 제품의 이름입니다. 이 열은 OfferName과 동일한 필드입니다. | *Azure 플랜* |
| SubscriptionId | Microsoft 청구 플랫폼에서 사용되는 구독의 고유 식별자입니다. 조정에 사용되지 않습니다. 이 식별자는 파트너 관리 콘솔의 구독 ID와 동일하지 않습니다. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | 구독의 청구 기간이 시작되는 날짜입니다. | *9/1/2020* |
| ChargeEndDate | 구독의 청구 기간이 종료된 날짜입니다. | *2020년 9월 30일* |
| TermAndBillingCycle | 구매 시 구독을 계속하기 위한 기간 약정입니다. | *저장된 데이터(GB/월)* |
| EffectiveUnitPrice | 청구 주기에 대한 비용을 계산하기 위한 비례 배분 단가입니다. 할인, 청구 일수 조정 및 기타 요인에 따라 유효 단가가 결정됩니다. 자세한 내용은 [유효 단가 계산을 참조하세요.](./effective-unit-price-calculation.md)  | *0.03825* |
| UnitType | 미터 요금이 청구되는 단위의 유형입니다. | *1GB/월* |
| AlternateId | 참조된 주문 줄 항목의 대체 ID입니다. | *6dc5c039750a* |
| BillableQuantity | 청구되는 총 수량입니다.  | *0.005001* |
| BillingFrequency | 구매 시 선택한 청구 플랜입니다. | *Na*  |
| PricingCurrency | 가격표의 통화입니다. | *USD* |
| PCToBCExchangeRate | 가격 책정 통화에 청구 통화에 적용되는 환율입니다. | *0.846202666* |
| PCToBCExchangeRateDate | 청구 통화의 가격 책정 통화가 결정되는 날짜입니다. | *2020년 9월 30일* |
| MeterDescription | 미터 설명입니다.  | *테이블 - LRS 데이터 저장(GB/월)* |
| ReservationOrderId | 예약 주문 ID입니다. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | 크레딧 설명입니다. | *Azure Consumption Credit* |
| SubscriptionStartDate | 구독을 구매한 날짜입니다. | *5/1/2021* |
| SubscriptionEndDate | 구독이 만료된 날짜입니다. | *4/30/2022* |
| ReferenceID | 업그레이드하는 동안 발생하는 모든 트랜잭션에 대한 링크입니다. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | 추가 기능 또는 평가판 구매를 알 수 있는 식별자입니다. | *["추가 기능"]* |
| PromotionID | 승격 정보를 가져오는 데 사용할 식별자입니다. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>일회성 구매 조정 파일에서 Azure 사용량을 조정할 수 있습니다. 이렇게 하려면 일일 등급 사용량 정찰 파일로 이동하여 SubscriptionID를 검색합니다. 그러면 Azure 플랜 ID와 관련된 모든 비용이 표시됩니다. Azure SubscriptionID가 EntitlementID로 표시됩니다.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>기본 구독을 업그레이드된 구독과 연결하는 방법

기본 제품의 구독 ID를 사용하여 해당 참조 ID를 찾고 이를 사용하여 연결된 모든 트랜잭션을 페치해야 합니다. 구독 ID 및 참조 ID와 함께 단일 이벤트에서 발생한 모든 업그레이드를 연결할 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [청구 및 세금](billing.md)
