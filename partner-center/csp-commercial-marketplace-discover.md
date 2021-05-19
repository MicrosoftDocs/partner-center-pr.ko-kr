---
title: 제품 검색-상업적 marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 파트너가 파트너 센터를 사용 하 여 Isv (독립 소프트웨어 공급 업체)의 SaaS 제품 또는 가격 책정을 보거나 검색 하는 방법에 대해 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147975"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>파트너 센터 상업적 marketplace에서 제품 및 가격 책정 검색

**적절 한 역할**: 전역 관리자 | 관리 에이전트

Isv (독립 소프트웨어 공급 업체)가 상업적 marketplace에서 제품을 게시 하도록 선택할 때 CSP 프로그램에서 제품을 사용할 수 있도록 할지 여부를 결정할 수도 있습니다. CSP 프로그램을 통해 제품을 판매 하도록 선택 하는 경우 CSP 파트너는 파트너 센터 마켓플레이스 영역에 제품을 표시 해야 합니다.

ISV 제품이 파트너 센터에서 기대한 대로 표시 되지 않는 경우 다음 때문일 수 있습니다.

- ISV는 CSP 프로그램을 통해 제품을 판매 하지 않기로 결정 했습니다. 예를 들어 일부 ISV 제품은 상용 marketplace의 다른 영역 (예: [Microsoft AppSource](https://appsource.microsoft.com/) 및 [Azure Marketplace](https://azuremarketplace.microsoft.com/))에서 사용할 수 있었지만 파트너 센터 marketplace의 CSP 프로그램에서 파트너에 게 표시 되지 않을 수 있습니다.

- ISV는 선택 된 수의 CSP 파트너만이 제품을 독점적으로 만들도록 결정 했습니다. 독점적 제공에 대 한 자세한 내용은이 도움말 항목의 뒷부분에 나오는을 참조 하세요.

- 제품 유형이 파트너 센터 또는 Azure Portal (예: 컨테이너 또는 일부 사용량 기반 제품)를 통해 불가능 않을 수 있습니다.

- 연결 된 고객의 청구 국가는이 ISV 제품에 대해 지원 되지 않을 수 있습니다.

## <a name="view-marketplace-offers-in-partner-center"></a>파트너 센터에서 Marketplace 제품 보기

CSP 프로그램에서 사용 가능한 상용 marketplace 제품을 보려면 다음을 수행 합니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 한 다음, 왼쪽 탐색 메뉴에서 **CSP** 를 선택 합니다.

2. **판매** 를 선택 하 고 **Marketplace** 를 선택 합니다. 기본적으로 모든 형식 및 범주의 제품이 표시 됩니다.

3. 유형 또는 범주별로 필터를 선택 합니다. 또한 **검색** 을 사용 하 여 특정 키워드, 제품 이름 또는 ISV 게시자의 이름을 찾을 수 있습니다.

4. 목록에서 특정 제품 제품을 선택합니다. 그러면 제품에 대해 자세히 알아볼 수 있는 제품 개요 탭으로 이뤄질 수 있습니다. 이 탭의 정보에는 다음이 포함될 수 있습니다. 

    - 제품 또는 제품에 대한 설명

    - ISV 게시자에 대한 자세한 정보

    - ISV 게시자가 업로드한 설명서 또는 마케팅 자료에 대한 링크

    - 고객 지원, 엔지니어링 또는 CSP 프로그램에 대한 연락처에 대한 기타 가능한 ISV 연락처

5. 제안의 사용 가능한 플랜, S SKU 또는 가격 책정에 대한 자세한 내용을 보려면 **계획 + 가격 책정** 탭을 선택합니다. 이 탭에는 다음이 표시됩니다.

    - 이 제안을 사용할 수 있는 시장

    - 제안에 사용할 수 있는 S SKU 또는 플랜 목록

    - 사용 가능한 각 SKU 또는 플랜에 대한 가격 책정

## <a name="view-marketplace-offers-via-partner-center-apis"></a>파트너 센터 API를 통해 Marketplace 제안 보기

CSP 프로그램 파트너는 API를 사용하여 적격 제안 목록을 반환할 수도 있습니다. 적격 제안은 파트너가 마켓플레이스를 통해 판매할 수 있는 SaaS ISV 제품만 파트너 센터. API를 사용하여 카탈로그에서 제안을 식별하는 파트너의 경우 지침을 참조하여 [시장 에 대한 제품 목록을 가져옵니다.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>파트너 센터 최신 Marketplace 제품 가격 책정 보기

제품과 관련된 최신 가격 책정 세부 정보는 다음 단계를 수행합니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인한 다음, 왼쪽 탐색 메뉴에서 **CSP를** 선택합니다.

2. **판매를** 선택한 **다음, 가격 책정 및 제안을** 선택합니다.

3. **Marketplace** 섹션으로 Scroll down 위치를 선택하고 **Marketplace 가격 책정** 을 다운로드합니다. 그러면 SaaS, 라이선스 기반 제품 및 ISV 게시자 로부터 제공 되는 요금제에 대 한 최신 가격 책정 데이터가 포함 된 스프레드시트가 생성 됩니다. 일부 Azure 응용 프로그램 가격은 여기에 표시 될 수 있습니다. 이 정보는 매일 업데이트 되므로 선택 하는 빈도에 따라 현재 가격을 확인할 수 있습니다.

4. ISV 제품에 무료 평가 기간이 포함 되어 있으면 스프레드시트에 해당 제품에 대 한 두 개의 행이 표시 됩니다.

    - 한 행은 무료 평가판 가격 (0)을 표시 합니다. 즉, 무료 평가판 기간이 제공 됩니다.

    - 다른 행에는 무료 평가 기간이 끝난 후에 적용 되는 가격 및 약관이 표시 됩니다.

CSP 프로그램 파트너는 특정 상업적 marketplace 제품에 연결 된 다른 성과급을 받을 수 있습니다. 다른 성과급에 대 한 자세한 내용은 [csp 동기 가이드](https://aka.ms/partnerincentives) (csp 로그인 필요)를 참조 하세요.

## <a name="learn-about-marketplace-exclusive-offers"></a>Marketplace 독점 제품에 대해 알아보기

Isv는 CSP 프로그램의 특정 파트너만 해당 제품을 사용할 수 있도록 하는 옵션을 제공 합니다. 이를 독점적인 제안 이라고 합니다. CSP 프로그램의 모든 파트너는 독점적으로 표시 된 제품을 비롯 하 여 파트너 센터 상업적 marketplace의 모든 ISV 제품을 볼 수 있습니다.

제품이 단독으로 표시 **되지 않은** 경우 모든 파트너는 해당 제품을 구매할 수 있습니다 (선택한 고객의 청구 국가가 ISV 제품의 국가 가용성과 일치 하는 것으로 가정).

그러나 단독으로 표시 된 모든 제품의 경우 ISV에서 선택한 파트너만 해당 제품을 구매할 수 있습니다.

> [!NOTE]
> 고객에 게 판매할 것으로 표시 된 제품이 독점적으로 표시 되는 경우 ISV에 게 직접 연락 하 여 독점적인 제품을 판매할 수 있는 권한을 요청 합니다. 독점 제품의 세부 정보를 볼 때 사용자가 선택할 수 있는 **ISV** 링크를 볼 수 있습니다.

상업적 marketplace의 ISV 환경에 대해 자세히 알아보려면 [클라우드 솔루션 공급자](/azure/marketplace/cloud-solution-providers)를 참조 하세요.

Marketplace의 CSP 환경에 대 한 자세한 내용은 [상용 마켓플레이스 개요](csp-commercial-marketplace-overview.md)를 참조 하세요.

## <a name="next-steps"></a>다음 단계

- [상업적 marketplace 제품 구매](csp-commercial-marketplace-purchase.md)