---
title: Azure 플랜 가격표 | 파트너 센터
ms.topic: article
ms.date: 01/24/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터를 사용하여 Azure 플랜이 적용되는 구독의 가격표를 보는 방법을 알아봅니다.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 2d69fb316f2451b57af1e6e850d676c67cde5fa3
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2020
ms.locfileid: "76812645"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Azure용 CSP의 새로운 상거래 환경에 대한 가격표 

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 글로벌 관리자
- 기술 지원팀 상담원
- 영업 상담원
- 사용자 관리 담당자

CSP의 새로운 Azure 상거래 환경에 대한 가격표는 파트너 센터에 게시되어 있습니다. 가격표는 정확한 실시간 파일을 통해 동적으로 제공되며 가격은 USD로만 표시됩니다. 그러나 청구는 고객의 통화 위치에서 지원하는 통화로 수행됩니다. 고객의 통화 위치에서 요금을 청구하는 방법에 대한 자세한 내용은 [Azure 플랜 - 청구](azure-plan-billing.md)를 참조하세요.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Azure 플랜 가격 책정이 적용되는 구독의 가격표 보기

1. 왼쪽의 파트너 센터 메뉴에서 **판매**를 선택한 다음, **Marketplace**를 선택합니다.

2. Azure 플랜 가격 책정에서 가격을 책정하려는 국가를 선택합니다.

3. **내보내기 유형** 옆에서 **Azure 플랜 사용 가격**, **Azure 플랜 예약 가격 책정** 또는 **환율**을 선택합니다. 참고: **환율**은 국가별로 다릅니다.

3. **날짜 가격 책정** 옆에서 원하는 날짜를 선택합니다(예: **현재**). 


![국가별](images/azure/pricingnew.png)

참고: Azure 플랜 가격 책정과 마켓플레이스 타사 가격 책정이라는 두 가지 가격표를 내보낼 수 있습니다. 

## <a name="azure-price-list-specifics"></a>Azure 가격표 세부 정보

- Azure 플랜 가격 책정은 파트너 센터 Marketplace 페이지의 **판매**에 제공됩니다.

- 내보내기는 Azure 플랜 사용 서비스, Azure Reservations 및 환율에 사용할 수 있습니다.

- 다음과 같은 내보내기 옵션이 있습니다.

    - **오늘 가격**: 해당 월의 1일부터 현재 날짜까지 모든 미터와 가격이 포함됩니다. 여기에는 새 가격, 변경된 가격 또는 제거된 가격이 포함됩니다. 모든 가격은 해당 가격이 신규 가격인지 아니면 제거된 가격인지 설명하는 유효 시작 날짜 및 종료 날짜가 있습니다.

    - **이전 달 가격**: 각 유형의 리소스를 월별로 다운로드합니다. 가격 책정 파일의 경우 해당 월에 사용 가능한 모든 미터가 포함됩니다. 월 중간에 새로운 미터가 나타나면 가용성을 반영하는 유효 날짜를 사용하여 미터가 표시됩니다. 할인된 가격과 마찬가지로, 더 이상 사용할 수 없게 되는 시기를 알리는 유효 종료 날짜를 사용하여 표시합니다.

    - **환율**: 환율은 매월 1일의 전날 6pm PST에 다운로드할 수 있습니다. 예를 들어 11월 환율을 원하는 경우 10월 31일의 환율을 다운로드합니다. 이전 달의 환율도 사용할 수 있습니다.

- 가격표의 가격은 직접 가격입니다. 일부 파트너는 파트너 획득 크레딧을 받을 수 있습니다. 파트너 획득 크레딧을 계산하는 방법에 대한 자세한 내용은 [파트너 획득 크레딧을 계산 및 지불하는 방법](partner-earned-credit-explanation.md)을 참조하세요.

- **적격 서비스**: 파트너 획득 크레딧은 파트너가 [Azure 플랜 가격 책정](https://partner.microsoft.com/commerce/sales) 페이지에서 내보낼 수 있는 **Azure 플랜 사용량 가격 책정**에 나열된 서비스에 적용됩니다. 참고: Azure 플랜 사용량 가격표 및 Azure 플랜 예약의 태그 열에서 "타사"로 식별된 타사 제품을 포함하지만 이에 국한되지 않는 예외가 있습니다.

## <a name="price-list-data"></a>가격표 데이터

|**필드**   |**설명**   |
|--------------------------|:---------------------------|
|ProductTitle  |제품의 제목 또는 이름|
|ProductID   |제품 ID|
|SKuId|SKU의 ID|
|SkuTitle|SKU의 제목 또는 이름|
|게시자|첫 번째 당사자는 항상 Microsoft|
|SkuDescription|SKU에 대한 설명|
|UnitOfMeasure|요금이 청구되는 단위|
|TermDuration|기간 기반 제품의 경우 예약에 적용되는 기간의 길이|
|시장|가격 책정 시장|
|Currency|가격 책정 통화|
|UnitPrice|단가|
|PricingTierRangeMin|계층형 가격 책정의 경우 최소 가격 적용|
|PricingTierRangeMax|계층형 가격 책정의 경우 최대 가격 적용|
|EffectiveStartDate|가격 책정 시작 날짜|
|EffectiveEndDate|가격 책정 종료 날짜|
|MeterIds|제품 sku의 미터 ID|
|MeterType|미터 유형|
|태그|항목의 속성. Azure 플랜 가격 책정의 경우 Azure 또는 Azure Reservations(구체적으로 예약의 경우)|

Azure 플랜 가격표는 [Azure 플랜 가격 책정 및 Marketplace 페이지](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)에서 내보낼 수 있습니다.

## <a name="pricing-api-for-azure-plan"></a>Azure 플랜 가격 책정 API

[가격 책정 API](https://docs.microsoft.com/partner/develop/pricing)를 사용하여 사용량 및 예약에 대한 Azure 플랜 가격 책정을 프로그래밍 방식으로 검색할 수 있습니다. 환율도 검색할 수 있습니다. 

가격 책정 API는 다른 파트너 센터 API와 다른 엔드포인트에 있습니다. 가격 책정 정보에는 Azure 플랜 리소스에 대한 미터 가격 책정(USD)과 Azure 플랜 구독에 적용되는 예약 가격 책정이 포함됩니다.

또한 Azure 플랜 가격이 USD로만 책정되므로 이 API를 사용하면 파트너가 월별 환율을 검색할 수 있습니다. API를 사용하여 이번 달 또는 이전 달의 가격 책정 및 환율을 모두 검색할 수 있습니다.

>[!NOTE]
> 가격 책정 API는 Azure 플랜 가격 책정에만 적용됩니다. Azure 플랜 이외의 구독에 배포된 Azure 리소스 또는 예약의 경우 파트너 센터의 "가격 책정 및 제품" 페이지에 게시된 기존 RateCard API 및 가격표를 계속 사용해야 합니다. Azure 플랜 가격 책정 API는 Microsoft 365 또는 Dynamics 365와 같은 소프트웨어, 마켓플레이스 또는 사용자 기반 가격 책정을 지원하지 않습니다.

Azure 플랜 가격 책정 및 환율 API에 대한 자세한 내용은 전체 [가격 책정 API 설명서](https://docs.microsoft.com/partner/develop/pricing)를 참조하세요.
