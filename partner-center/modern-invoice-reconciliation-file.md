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
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146258"
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
| CustomerCountry | 고객이 있는 국가입니다. 해당 지역의 전체 [국가 목록을](./regional-authorization-overview.md) 확인 하세요.  | *취소* |
| InvoiceNumber | 조정 파일에 연결 된 청구서 번호입니다.  | *G002297372* |
| MpnId | CSP 파트너의 MPN 식별자입니다. 자세한 내용은 파트너를 기준으로 항목별로 항목을 표시 하 [는 방법](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)을 참조 하세요. | *6034453* |
| ResellerMpnId | 구독에 대 한 레코드 대리점의 MPN 식별자입니다. | *6048879* |
| OrderID | Microsoft 청구 플랫폼에서 사용되는 주문의 고유 식별자입니다. 지원에 문의할 때 주문을 식별 하는 데 유용할 수 있습니다. 조정에 사용 되지 않습니다. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | 주문이 배치 된 UTC 날짜입니다. | *10/3/2020* |
| ProductId | 제품의 고유 식별자입니다. | *DZH318Z0BNZ5* |
| SkuId | SKU 고유 식별자입니다. | *006G* |
| AvailabilityId | 가용성 고유 식별자입니다. | *DZH318Z08B80* |
| SkuName | SKU 이름입니다. | *테이블 - LRS* |
| ProductName | 제품 이름입니다. | *테이블* |
| ChargeType | 요금 또는 조정 [유형입니다.](./recon-file-charge-types.md) | *새로 만들기* |
| 단가 | 구매 시 가격표에 게시된 라이선스당 가격입니다. 조정하는 동안 청구 시스템에 저장된 정보와 일치하는지 확인합니다. | *0.045* |
| 수량 | 라이선스 수입니다. 조정하는 동안 청구 시스템에 저장된 정보와 일치하는지 확인합니다. | *1* |
| 소계 | 세금 전 합계입니다. 소계는 유효 단가를 곱한 청구 가능 수량과 같아야 합니다. | *0* |
| TaxTotal | 세금 금액 청구. 시장의 세금 규칙 및 특정 상황에 따라 | *0* |
| 합계 | 총 금액은 소계에 세금 금액을 더한 금액과 같습니다. | *0* |
| 통화 | 청구서는 고객 통화의 컨텍스트에서 생성됩니다. 즉, 청구 가능한 통화가 다른 고객과 거래하는 파트너인 경우 각 고객 통화 형식에 대한 청구서를 받습니다.  | *EUR* |
| PriceAdjustmentDescription | 단가 조정 이유입니다. 이것이 주요 이유이지만 유효 단가 결정으로 제한되지는 않습니다. | *["서비스에서 관리 되는 서비스에 대 한" 15.0% 파트너 획득 크레딧 "]* |
| PublisherName | 제품의 게시자입니다.  | *Microsoft* |
| PublisherId | 파트너 센터가 게시자를 식별 하는 데 사용 하는 고유 식별자입니다. | *수치* |
| SubscriptionDescription | 가격 목록에 정의 된 대로 고객이 구매한 서비스 제공 서비스의 이름입니다. 이 열은 OfferName와 동일한 필드입니다. | *Azure 플랜* |
| SubscriptionId | Microsoft 청구 플랫폼에서 사용되는 구독의 고유 식별자입니다. 조정에 사용 되지 않습니다. 이 식별자는 파트너 관리 콘솔의 구독 ID와 동일 하지 않습니다. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | 구독의 청구 기간이 시작 되는 날짜입니다. | *9/1/2020* |
| ChargeEndDate | 구독의 청구 기간이 종료 되는 날짜입니다. | *2020년 9월 30일* |
| TermAndBillingCycle | 구매 시 구독을 계속 하는 기간입니다. | *저장 된 데이터 (g b/월)* |
| EffectiveUnitPrice | 청구 주기에 대 한 비용을 계산 하는 데 비례 하는 단가입니다. 할인, 청구 일의 조정 및 기타 요소는 유효 단가를 결정 합니다. 자세한 내용은 [유효 단위 가격 계산](./effective-unit-price-calculation.md)을 참조 하세요.  | *0.03825* |
| (Unittype.pixel) | 미터의 요금이 부과 되는 단위 유형입니다. | *1GB/월* |
| AlternateId | 참조 된 주문 라인 항목의 대체 ID입니다. | *6dc5c039750a* |
| BillableQuantity | 청구 되는 총 수량입니다.  | *0.005001* |
| BillingFrequency | 구매할 때 선택한 청구 계획입니다. | *수치*  |
| PricingCurrency | 가격표의 통화입니다. | *USD* |
| PCToBCExchangeRate | 요금 청구 통화에 대 한 가격 책정 통화에 적용 되는 환율입니다. | *0.846202666* |
| PCToBCExchangeRateDate | 청구 통화에 대 한 가격 책정 통화를 결정 하는 날짜입니다. | *2020년 9월 30일* |
| MeterDescription | 측정기 설명입니다.  | *테이블-저장 된 LRS 데이터 (g b/월)* |
| ReservationOrderId | 예약 주문 ID입니다. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | 크레딧 설명입니다. | *Azure Consumption Credit* |

>[!NOTE]
>일회성 구매 조정 파일에서 Azure 사용량을 조정할 수 있습니다. 이렇게 하려면 일일 등급 사용량 정찰 파일로 이동하여 SubscriptionID를 검색합니다. 그러면 Azure 플랜 ID와 관련된 모든 비용이 표시됩니다. Azure SubscriptionID가 EntitlementID로 표시됩니다.

## <a name="next-steps"></a>다음 단계

- [청구 및 세금](billing.md)
