---
title: 라이선스 기반 조정 파일
ms.topic: article
ms.date: 05/18/2020
description: 파트너 센터에서 라이선스 기반 조정 파일을 읽는 방법에 대해 알아봅니다. 이 문서에서는 라이선스 기반 정찰 파일에 있는 각 필드의 의미에 대해 설명 합니다.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 86581db73f1bf2b6660af45aca4747a5db779bbe
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444919"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>파트너 센터 라이선스 기반 조정 파일의 필드 이해

**적용 대상**

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

**적절한 역할**
- 전역 관리자
- 사용자 관리자
- 청구 관리자
- 관리 에이전트

고객의 주문에 대 한 변경 내용을 조정 하려면 조정 파일의 **Syndication_Partner_Subscription_Number** 파트너 센터의 **구독 ID** 와 비교 합니다.

## <a name="fields-in-license-based-reconciliation-files"></a>라이선스 기반 조정 파일의 필드

| 열 | Description | 샘플 값 |
| ------ | ----------- | ------------ |
| PartnerId | 특정 청구 엔터티에 대 한 GUID 형식의 고유 식별자입니다. 조정에는 필요 하지 않습니다. 모든 행에서 동일 합니다. | *8ddd03642-테스트-테스트* |
| CustomerId | GUID 형식의 고객에 대 한 고유한 Microsoft 식별자입니다. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | 파트너 센터에 보고 된 고객의 조직 이름입니다. *시스템 정보를 사용 하 여 송장을 조정 하기 위한 매우 중요 한 필드입니다.* | *테스트 고객 A* |
| MpnId | CSP 파트너의 MPN 식별자입니다. 파트너를 기준으로 항목별로 항목을 표시 하 [는 방법을](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)참조 하세요. | *4390934* |
| ResellerMpnId | 구독에 대 한 레코드 대리점의 MPN 식별자입니다.  |
| OrderID | Microsoft 청구 플랫폼에서 사용되는 주문의 고유 식별자입니다. 지원에 문의할 때 주문을 식별 하는 데 유용할 수 있습니다. 조정에 사용 되지 않습니다. | *566890604832738111* |
| SubscriptionId | Microsoft 청구 플랫폼에서 사용되는 구독의 고유 식별자입니다. 지원에 문의할 때 구독을 식별 하는 데 유용할 수 있습니다. 조정에 사용 되지 않습니다. *이 값은 파트너 관리 콘솔의 **구독 ID** 와 동일 하지 않습니다. 대신 **SyndicationPartnerSubscriptionNumber** 를 참조 하세요.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | 구독에 대 한 고유 식별자입니다. 고객은 동일한 계획에 대해 여러 구독을 가질 수 있습니다. 이 열은 조정 파일 분석에 중요 합니다. 이 필드는 파트너 관리 콘솔의 **구독 ID** 에 매핑됩니다. | *fb977ab5-24c8d9591708* |
| OfferId | 고유 제품 식별자입니다. 가격 목록에 정의 된 표준 제품 식별자입니다. *이 값은 가격 목록의 **제품 ID** 와 일치 하지 않습니다. 대신 **DurableOfferID** 를 참조 하세요.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | 가격 목록에 정의 된 고유한 지 속성 제공 식별자입니다. *이 값은 가격 목록의 **제품 ID** 와 일치 합니다.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 가격 목록에 정의 된 대로 고객이 구매한 서비스 제공 서비스의 이름입니다. | *Microsoft Office 365 (E3 계획)* |
| Subscription.subscriptionstartdate | 구독 시작 날짜입니다. 시간은 항상 하루의 시작인 0:00입니다. 이 필드는 주문이 제출 된 후의 일로 설정 됩니다. **Subscription.subscriptionenddate** 와 함께 사용 되어 고객이 아직 구독의 첫 번째 연도 내에 있는지 또는 구독이 다음 연도에 대해 갱신 되었는지 여부를 확인 합니다. | *2/1/2019 0:00* |
| Subscription.subscriptionenddate | 구독 종료 날짜입니다. 시간은 항상 하루의 시작인 0:00입니다. *시작 날짜 로부터 12 개월 + **x** 일을 더한* 날짜에서 파트너의 청구 날짜 또는 *12 개월을 기준*으로 합니다. 갱신 시 가격은 현재 가격 목록으로 업데이트 됩니다. 자동 갱신을 사전에 수행 해야 하는 고객 통신 | *2/1/2019 0:00* |
| ChargeStartDate | 요금 시작 날짜입니다. 시간은 항상 하루의 시작인 0:00입니다. 고객이 라이선스 번호를 변경 하는 경우 일별 요금 (*pro 게 유리 하도록* 요금)을 계산 하는 데 사용 됩니다. | *2/1/2019 0:00* |
| ChargeEndDate | 요금 종료 날짜입니다. 시간은 항상 일의 끝 인 23:59입니다. 고객이 라이선스 번호를 변경 하는 경우 일별 요금 (*pro 게 유리 하도록* 요금)을 계산 하는 데 사용 됩니다. | *2/28/2019 23:59* |
| ChargeType | 요금 또는 조정 [의 유형](recon-file-charge-types.md) 입니다. | [요금 청구 유형](recon-file-charge-types.md)을 참조 하세요. |
| UnitPrice | 구매 시 가격표에 게시 된 라이선스 당 가격입니다. 조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다. | *6.82* |
| 수량 | 라이선스의 수입니다. 조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다. | *2* |
| 금액 | 수량에 대 한 가격의 합계입니다. 금액 계산이 고객에 대해이 값을 계산 하는 방법과 일치 하는지 확인 하는 데 사용 됩니다. | *13.32* |
| TotalOtherDiscount | 이러한 요금에 적용 되는 할인 금액입니다. 역량 또는 맵과 함께 제공 되는 제품 라이선스 또는 동기에 적합 한 새 구독은이 열에 할인 금액을 포함 합니다. | *2.32* |
| 소계 | 세금 앞의 합계입니다. 할인이 예상 합계와 일치 하는지 확인 합니다. | *11* |
| 세금 | 세금 금액 요금. 시장의 세금 규칙 및 특정 상황을 기준으로 합니다. | *0* |
| TotalForCustomer | 세금 이후의 합계입니다. 청구서에 세금이 부과 되는지 확인 합니다. | *11* |
| Currency | 통화 형식입니다. 각 청구 엔터티에는 하나의 통화가 적용됩니다. 첫 번째 청구서와 일치 하는지 확인 합니다. 주요 청구 플랫폼을 업데이트 한 후에 다시 확인 합니다. | *EUR* |
| DomainName | 고객의 도메인 이름입니다. 이 필드는 두 번째 청구 주기까지 공백으로 표시 될 수 있습니다. *이 필드를 고객에 대 한 고유 식별자로 사용 하지 마세요. 고객/파트너는 Office 365 포털을 통해 베 니 티 또는 기본 도메인을 업데이트할 수 있습니다.* | *example.onmicrosoft.com* |
| SubscriptionName | 구독 애칭. 애칭을 지정 하지 않으면 파트너 센터는 **OfferName**을 사용 합니다. | *PROJECT ONLINE* |
| SubscriptionDescription | 가격 목록에 정의 된 대로 고객이 구매한 서비스 제공 서비스의 이름입니다. 이는 **OfferName**에 대 한 동일한 필드입니다. | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
| BillingCycleType | 일회성 청구 빈도입니다.| *매월* |