---
title: 파트너 센터에서 청구 유형 이해 | 파트너 센터
ms.topic: article
ms.date: 03/01/2019
Description: 다른 형식 청구, 청구 기간 및 청구 날짜에 대 한 정보
author: MaggiePucciEvans
ms.author: evansma
keywords: 대금 청구, 결제, orders, 조정 파일, 여러 파일
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 4b2b42c0d9bbb2654bbd486f987e3d5da9c562a2
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135383"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>파트너 센터의 청구 유형 이해

**적용 대상**

-  파트너 센터
-  CSP 프로그램의 파트너

고객을 위해 구입 하는 제품 유형의 경우에 따라 다양 한 청구 기간 있을 수 있습니다 하 고 같은 달의 다른 일에 청구 됩니다. 이 문서는 2019 년 3 월 1 일 시작 변경 내용 및 변경 영향 됩니다 하는 방법을 설명 합니다.

## <a name="billing-for-recurring-charges"></a>반복 청구 요금에 대 한 청구

라이선스 기반 및 사용량 기반 구독 반복 청구 요금에 대 한 청구 환경을 변경 되지 않음. 계속 하면 청구 날짜로 선택한 월의 일에 청구 및에 청구 기간 계속 해당 날짜 이전 달 수 있습니다. 청구 날짜에 대해 월의 15 일을 선택 하면 다음 달의 14th 1 개월간의 15 일에서 모든 작업에 대 한 청구 합니다. 청구서 및 조정 파일은 일반 공급 2 ~ 4 일에 청구 날짜 후 합니다.

이전에 거주 하는 국가/지역의 통화에서 이러한 제품에 대 한 청구 수에 따라 고객의 위치에 관계 없이 판매한 제품입니다.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>일회용 선택한 반복 청구 요금에 대 한 청구

Microsoft 및 타사 ISV 제품에 대 한 되풀이 및 1 회 요금 청구 새로운 환경이 도입 2019 년 3 월 1 일을 시작 했습니다.

이러한 제품에 대 한 청구 기간은 달력 월의 첫째 날에 시작 되며 달력 월의 마지막 날에 끝납니다. 다음 달의 8 번째 날에 청구서를 사용할 수 있도록 하겠습니다 했습니다. 

즉, 월 1 및 2019 년 5 월 31 일 사이의 모든 트랜잭션 수는 청구서에 표시 년 6 월 8입니다. 6 월 1 일 및 2019 년 6 월 30 일 간의 모든 트랜잭션 수 년 7 월 8 청구서에 표시 됩니다. 수 요금이 청구 됩니다 동일한 청구서의 일회성 및 되풀이 구매에 대 한 합니다. 

또한 입력 (예를 들어 1 월 및 7 월) 및 청구서를 기다릴 필요 없이 최근 계정 활동을 참조 하세요. 때마다 계정 잔액/청구서를 확인할 수 있습니다. 참고는 청구서에는 8 일에 게시 되 면 포함 됩니다 세금 및 기타 적용 가능한 요금 및 크레딧, 청구 기간 동안 표시 되는 내용에서 최종 수량 다를 수 있도록 합니다. 

청구서 수행한 이제 파트너 센터에서 또는 API에서 동일한 방식으로 액세스할 수 있습니다. 해당 월의 8 번째 날에 자정 UTC 전에 나타납니다. 

|**청구 경험**|**제품 유형**|**청구 날짜**|**청구 기간**|**청구 통화**|**현재 활동을 사용할 수 있습니까?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|라이선스 및 사용량 기반 구독에 대 한 반복 청구 요금 |모든 제품을 [온라인 서비스 카탈로그](https://partner.microsoft.com/commerce/preferredoffers/list)합니다. 예를 들어 Office 365, Microsoft 365, Azure Active Directory, Azure (종 량 제), Dynamics 365, PowerBI Pro |파트너 센터 계정을 만들 때 선택한 날짜 |청구 날짜에 이전 월입니다. |거주 하는 국가/지역의 통화입니다. 예를 들어, 회사 United Kingdom에 있으면 영국 파운드 (GBP)에서 청구 됩니다. 회사 인도 있으면 인도 루피 (INR)에서 청구 됩니다.  |아니오 |
|Microsoft 및 타사 Isv 제품에 대 한 되풀이 및 1 회 요금 |모든 SaaS 구독, Azure 예약 및 Microsoft 및 타사 Isv에서 제공 하는 소프트웨어 (영구 및 구독 기반) 제품입니다. 사용 가능한 제품 참조는 [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)합니다. 예로 SUSE Linux 소프트웨어 (소프트웨어 구독), Windows Server 2019 Essentials (영구 소프트웨어), Azure ISV SaaS 제품 구독 합니다. |각 월의 8 번째 날 |첫 번째 날짜 각 월의 마지막 날 |고객에 위치한 국가/지역의 통화입니다. 이 받게 별도 청구서와 조정 파일 국가/지역의 통화로 청구 기간에 판매 된 각 고객을 의미 합니다. |예 |
