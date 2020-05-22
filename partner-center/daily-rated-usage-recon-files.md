---
title: 매일 등급 사용 조정 파일
ms.topic: article
ms.date: 05/15/2020
description: 파트너 센터에서 매일 등급 사용 조정 파일을 읽는 방법에 대해 알아봅니다.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3536b1b71dd8378e88ac14726adcca7fa0e08530
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795591"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>파트너 센터에서 매일 등급 사용 조정 파일을 읽는 방법에 대해 알아봅니다.

**적용 대상**

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 영업 상담원
- 기술 지원팀 상담원

이 항목에서는 매일 등급 사용 조정 파일을 읽는 방법에 대해 설명 합니다.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>매일 등급 사용 조정 파일의 필드

| 열 | Description |
| ------ | ----------- |
| PartnerId | GUID 형식의 파트너 식별자입니다. |
| PartnerName | 파트너 이름입니다. |
| CustomerId | GUID 형식의 고객에 대 한 고유한 Microsoft 식별자입니다. |
| CustomerName | 파트너 센터에 보고된 고객의 조직 이름입니다. *이 열은 시스템 정보를 사용 하 여 송장을 조정 하는 데 매우 중요 합니다.* |
| CustomerDomainName | 고객의 도메인 이름입니다. |
| CustomerCountry | 고객이 있는 국가입니다. |
| MpnId | CSP 파트너의 MPN 식별자입니다. |
| Tier2MpnId | 구독에 대 한 레코드 대리점의 MPN 식별자입니다. |
| InvoiceNumber | 지정된 거래가 표시되는 청구서 번호입니다. |
| ProductId | 제품의 식별자입니다. |
| SkuId | 특정 SKU에 대 한 식별자입니다. |
| AvailabilityId | 특정 SKU의 가용성에 대 한 식별자입니다. 지정 된 국가, 통화, 산업 부문 등에서 SKU를 구매할 수 있는지 여부를 표시 합니다. |
| SkuName | 특정 SKU의 제목입니다. |
| ProductName | 제품의 이름입니다. |
| PublisherName | 게시자 이름입니다. |
| PublisherId | GUID 형식의 게시자 식별자입니다. |
| SubscriptionDescription | 가격 목록에 정의 된 대로 고객이 구매한 서비스 제공 서비스의 이름입니다. 이는 **OfferName**에 대 한 동일한 필드입니다. |
| SubscriptionId | Microsoft 청구 플랫폼에서 사용되는 구독의 고유 식별자입니다. 조정에 사용 되지 않습니다. *이 식별자는 파트너 관리 콘솔의 **구독 ID** 와 동일 하지 않습니다.* |
| ChargeStartDate | 청구 주기의 시작 날짜입니다 (이전 청구 주기에서 이전에 청구 되지 않은 잠재 사용량 데이터의 날짜를 제시 하는 경우 제외). 시간은 항상 하루의 시작인 0:00입니다. |
| ChargeEndDate | 청구 주기의 종료 날짜입니다 (이전 biling 주기에서 이전에 청구 되지 않은 잠재 사용량 데이터의 날짜를 제시 하는 경우 제외). 시간은 항상 일의 끝 인 23:59입니다. |
| UsageDate | 서비스 사용 날짜입니다. |
| MeterType | 측정기의 유형입니다. |
| MeterCategory | 사용에 대한 최상위 서비스입니다. |
| MeterId | 사용 되는 측정기의 식별자입니다. |
| MeterSubCategory | 요금에 영향을 줄 수 있는 Azure 서비스의 유형입니다. |
| MeterName | 사용 되는 측정기에 대 한 측정 단위입니다. |
| MeterRegion | 이 열은 해당 지역 내에서 서비스에 대 한 데이터 센터의 위치를 식별 하 고 해당 위치를 채웁니다. |
| 단위 | 리소스 **이름의**단위입니다. |
| ResourceLocation | 측정기가 실행 되 고 있는 데이터 센터입니다. |
| ConsumedService | 사용한 Azure 플랫폼 서비스입니다. |
| ResourceGroup | Azure 솔루션에 관련 된 리소스를 보유 하는 컨테이너를 나타냅니다. |
| ResourceURI | 사용 되는 리소스의 URI입니다. |
| ChargeType | 요금 또는 조정의 유형입니다.  |
| UnitPrice | 구매 시 가격 목록에 게시 된 라이선스 당 가격입니다. 조정 하는 동안이 가격이 청구 시스템에 저장 된 정보와 일치 하는지 확인 합니다. |
| 수량 | 라이선스의 수입니다. 조정 하는 동안이 가격이 청구 시스템에 저장 된 정보와 일치 하는지 확인 합니다. |
| (Unittype.pixel) | 미터의 요금이 청구 되는 단위 유형입니다.  |
| BillingPreTaxTotal | 세금 전 총 청구 금액입니다. |
| BillingCurrency | 고객 지역의 통화입니다. |
| PricingPreTaxTotal | 세금이 추가 되기 전의 가격 책정입니다. |
| PricingCurrency | 가격표의 통화입니다. |
| ServiceInfo1 | 지정 된 날짜에 프로 비전 되 고 사용 된 Service Bus 연결의 수입니다. |
| ServiceInfo2 | 선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다. |
| 태그들 | 사용자가 설정 하는 Azure 리소스의 논리적 구성을 나타냅니다. |
| AdditionalInfo | 다른 열에서 다루지 않은 추가 정보입니다. |
| EffectiveUnitPrice | 할인, 획득 크레딧을 비롯 하 여 단위당 청구 되는 실제 값입니다. |
| PCToBCExchangeRate | 가격 책정 통화에서 청구 통화로 적용 되는 환율 |
| PCToBCExchangeRateDate | 청구 통화에 대 한 가격 책정 통화를 결정 하는 날짜입니다. |
| EntitlementId | Azure 구독 ID를 나타냅니다. |
| EntitlementDescription | Azure 구독 ID의 이름을 나타냅니다. |
| PartnerEarnedCreditPercentage | 줄 항목에 대 한 표시 크레딧을 표시 합니다. 획득 크레딧은 0 또는 15%입니다. |
