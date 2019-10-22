---
title: Azure 플랜 가격표 | 파트너 센터
ms.topic: article
ms.date: 10/15/2019
description: Azure 플랜이 적용되는 구독의 가격표를 보는 방법
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 64f7b6930f31afc63397ae3ed0e0dba2357b0f1e
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171281"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Azure용 CSP의 새로운 상거래 환경에 대한 가격표 

CSP의 새로운 Azure 상거래 환경에 대한 가격표는 파트너 센터에 게시되어 있습니다. 가격표는 정확한 실시간 파일을 통해 동적으로 제공되며 가격은 USD로만 표시됩니다. 그러나 청구는 고객의 통화 위치에서 지원하는 통화로 수행됩니다. 고객의 통화 위치에서 요금을 청구하는 방법에 대한 자세한 내용은 [Azure 플랜 - 청구](azure-plan-billing.md)를 참조하세요.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Azure 플랜 가격 책정이 적용되는 구독의 가격표 보기

1. 왼쪽의 파트너 센터 메뉴에서 **판매**를 선택한 다음, **Marketplace**를 선택합니다.

2. **내보내기 형식** 옆에서 **Azure 플랜 사용 가격**을 선택합니다.

3. **날짜 가격 책정** 옆에서 원하는 날짜를 선택합니다(예: **현재**). 참고: **환율**을 선택하여 현재 환율을 내보낼 수도 있습니다.

![azure 가격 책정 2](images/azure/pricelist2.jpg)

4. **Marketplace**에서 제품의 **유형** 및 **범주**를 선택하거나 제품을 검색합니다. 검색 내용에 따라 사용 가능한 제품이 표시됩니다.

![pricing](images/azure/Azurepricelist1.jpg)

5. **Azure 플랜 가격표 내보내기**를 선택하여 선택한 제품의 Azure 플랜 가격을 다운로드합니다.


![가격표 내보내기](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Azure 가격표 세부 정보

- Azure 플랜 가격 책정은 파트너 센터 Marketplace 페이지의 **판매**에 제공됩니다.

- 내보내기는 Azure 플랜 사용 서비스, Azure Reservations 및 환율에 사용할 수 있습니다.

- 다음과 같은 내보내기 옵션이 있습니다.

    - **오늘 가격**: 해당 월의 1일부터 현재 날짜까지 모든 미터와 가격이 포함됩니다. 여기에는 새 가격, 변경된 가격 또는 제거된 가격이 포함됩니다. 모든 가격은 해당 가격이 신규 가격인지 아니면 제거된 가격인지 설명하는 유효 시작 날짜 및 종료 날짜가 있습니다.

    - **이전 달 가격**: 각 유형의 리소스를 월별로 다운로드합니다. 가격 책정 파일의 경우 해당 월에 사용 가능한 모든 미터가 포함됩니다. 월 중간에 새로운 미터가 나타나면 가용성을 반영하는 유효 날짜를 사용하여 미터가 표시됩니다. 할인된 가격과 마찬가지로, 더 이상 사용할 수 없게 되는 시기를 알리는 유효 종료 날짜를 사용하여 표시합니다.

    - **환율**: 환율은 매월 1일의 전날 6pm PST에 다운로드할 수 있습니다. 예를 들어 11월 환율을 원하는 경우 10월 31일의 환율을 다운로드합니다. 이전 달의 환율도 사용할 수 있습니다.

    - **적격 서비스**: 파트너 획득 크레딧은 파트너가 Azure 플랜 가격 책정 페이지에서 내보낼 수 있는 **Azure 플랜 사용량 가격 책정**에 나열된 서비스에 적용됩니다. 타사 및 Azure Reservations을 포함하여(이에 국한되지 않음) 예외가 있습니다.

- 가격표의 가격은 직접 가격입니다. 일부 파트너는 파트너 획득 크레딧을 받을 수 있습니다. 파트너 획득 크레딧을 계산하는 방법에 대한 자세한 내용은 [파트너 획득 크레딧을 계산 및 지불하는 방법](partner-earned-credit-explanation.md)을 참조하세요.


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
|지역/국가|가격 책정 시장|
|Currency|가격 책정 통화|
|UnitPrice|단가|
|PricingTierRangeMin|계층형 가격 책정의 경우 최소 가격 적용|
|PricingTierRangeMax|계층형 가격 책정의 경우 최대 가격 적용|
|EffectiveStartDate|가격 책정 시작 날짜|
|EffectiveEndDate|가격 책정 종료 날짜|
|MeterIds|제품 sku의 미터 ID|
|MeterType|미터 유형|
|태그|항목의 속성. Azure 플랜 가격 책정의 경우 Azure 또는 Azure Reservations(구체적으로 예약의 경우)|

자세한 내용은 [가격표 정보](https://partner.microsoft.com/commerce/sales?type=Any&category=Any) 참조  
