---
title: 라이선스 기반 조정 파일
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 라이선스 기반 조정 파일을 읽는 방법을 알아봅니다. 이 문서에서는 라이선스 기반 정찰 파일에서 각 필드의 의미를 설명합니다.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 041f0fadfea107027ae1d9796d235700e66e6834
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146581"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>파트너 센터 라이선스 기반 조정 파일의 필드 이해

**적용된 내용:** 파트너 센터 | Microsoft Cloud for US Government 대한 파트너 센터

**적절한 역할:** 전역 관리자 | 사용자 관리 관리자 | 청구 관리자 | 관리 에이전트

고객의 주문과 변경 내용을 조정하려면 조정 파일의 **Syndication_Partner_Subscription_Number 파트너 센터** 구독 **ID와** 비교합니다.

## <a name="fields-in-license-based-reconciliation-files"></a>라이선스 기반 조정 파일의 필드

| 열 | Description | 샘플 값 |
| ------ | ----------- | ------------ |
| PartnerId | 특정 청구 엔터티에 대한 GUID 형식의 고유 식별자입니다. 조정에 필요하지 않습니다. 모든 행에서 동일합니다. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | GUID 형식의 고객에 대한 고유한 Microsoft 식별자입니다. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | 파트너 센터 보고된 고객의 조직 이름입니다. *청구서를 시스템 정보와 조정하기 위한 매우 중요한 필드입니다.* | *테스트 고객 A* |
| MpnId | CSP 파트너의 MPN 식별자입니다. [파트너별로 항목을 지정하는 방법을](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)참조하세요. | *4390934* |
| ResellerMpnId | 구독에 대한 레코드의 대리점에 대한 MPN 식별자입니다.  |
| OrderID | Microsoft 청구 플랫폼에서 사용되는 주문의 고유 식별자입니다. 지원 담당자에게 문의할 때 주문을 식별하는 데 유용할 수 있습니다. 조정에 사용 되지 않습니다. | *566890604832738111* |
| SubscriptionId | Microsoft 청구 플랫폼에서 사용되는 구독의 고유 식별자입니다. 지원에 문의할 때 구독을 식별 하는 데 유용할 수 있습니다. 조정에 사용 되지 않습니다. *이 값은 파트너 관리 콘솔의 **구독 ID** 와 동일 하지 않습니다. 대신 **SyndicationPartnerSubscriptionNumber** 를 참조 하세요.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | 구독에 대 한 고유 식별자입니다. 고객은 동일한 계획에 대해 여러 구독을 가질 수 있습니다. 이 열은 조정 파일 분석에 중요 합니다. 이 필드는 파트너 관리 콘솔의 **구독 ID** 에 매핑됩니다. | *fb977ab5-24c8d9591708* |
| OfferId | 고유 제품 식별자입니다. 가격 목록에 정의 된 표준 제품 식별자입니다. *이 값은 가격 목록의 **제품 ID** 와 일치 하지 않습니다. 대신 **DurableOfferID** 를 참조 하세요.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | 가격 목록에 정의 된 고유한 지 속성 제공 식별자입니다. *이 값은 가격 목록의 **제품 ID** 와 일치 합니다.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 가격 목록에 정의 된 대로 고객이 구매한 서비스 제공 서비스의 이름입니다. | *Microsoft Office 365 (E3 계획)* |
| SubscriptionStartDate | 구독 시작 날짜(UTC)입니다. 시간은 항상 하루의 시작인 0:00입니다. 이 필드는 주문이 제출된 다음 날로 설정됩니다. **SubscriptionEndDate와** 함께 사용하여 고객이 아직 구독의 첫 번째 연도 내에 있는지 또는 다음 연도에 대해 구독이 갱신되었는지 확인합니다. | *2/1/2019 0:00* |
| SubscriptionEndDate | 구독 종료 날짜(UTC)입니다. 시간은 항상 하루의 시작인 0:00입니다. 파트너의 청구 날짜와 일치하도록 *시작 날짜 이후 12개월+ **x일*** 또는 *갱신 날짜로부터 12개월입니다.* 갱신 시 가격은 현재 가격 목록으로 업데이트됩니다. 자동 갱신 전에 고객 통신이 필요할 수 있습니다. | *2/1/2019 0:00* |
| ChargeStartDate | 요금의 시작일입니다. 시간은 항상 하루의 시작인 0:00입니다. 고객이 라이선스 번호를 변경할 때 일별 *요금(pro-pro-charges)을* 계산하는 데 사용됩니다. | *2/1/2019 0:00* |
| ChargeEndDate | 요금의 종료일입니다. 시간은 항상 하루의 끝인 23:59입니다. 고객이 라이선스 번호를 변경할 때 일별 *요금(pro-pro-charges)을* 계산하는 데 사용됩니다. | *2/28/2019 23:59* |
| ChargeType | 요금 또는 조정 [유형입니다.](recon-file-charge-types.md) | [요금 유형을](recon-file-charge-types.md)참조하세요. |
| 단가 | 구매 시 가격 목록에 게시 된 라이선스 당 가격입니다. 조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다. | *6.82* |
| 수량 | 라이선스의 수입니다. 조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다. | *2* |
| Amount | 수량에 대 한 가격의 합계입니다. 금액 계산이 고객에 대해이 값을 계산 하는 방법과 일치 하는지 확인 하는 데 사용 됩니다. | *13.32* |
| TotalOtherDiscount | 이러한 요금에 적용 되는 할인 금액입니다. 역량 또는 맵과 함께 제공 되는 제품 라이선스 또는 동기에 적합 한 새 구독은이 열에 할인 금액을 포함 합니다. | *2.32* |
| 소계 | 세금 앞의 합계입니다. 할인이 예상 합계와 일치 하는지 확인 합니다. | *11* |
| 세금 | 세금 금액 요금. 시장의 세금 규칙 및 특정 상황을 기준으로 합니다. | *0* |
| TotalForCustomer | 세금 이후의 합계입니다. 청구서에 세금이 부과 되는지 확인 합니다. | *11* |
| 통화 | 통화 형식입니다. 각 청구 엔터티에는 하나의 통화가 적용됩니다. 첫 번째 청구서와 일치 하는지 확인 합니다. 주요 청구 플랫폼이 업데이트된 후 다시 확인합니다. | *EUR* |
| DomainName | 고객의 도메인 이름입니다. 이 필드는 두 번째 청구 주기까지 비어 있을 수 있습니다. *이 필드를 고객의 고유 식별자로 사용하지 마세요. 고객/파트너는 Office 365 포털을 통해 베니티 또는 기본 도메인을 업데이트할 수 있습니다.* | *example.onmicrosoft.com* |
| SubscriptionName | 구독 애칭입니다. 애칭을 지정하지 않으면 파트너 센터 **OfferName** 을 사용합니다. | *PROJECT ONLINE* |
| SubscriptionDescription | 가격표에 정의된 대로 고객이 구매한 서비스 제품의 이름입니다. **(OfferName** 과 동일한 필드입니다.) | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
| BillingCycleType | 일회성 청구 빈도입니다.| *매월* |
