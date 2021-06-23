---
title: Azure Partner Shared Services 추가
description: Azure Partner Shared Services 사용하여 고유한 용도로 Azure 구독을 구입하고 Azure를 구매, 추적 및 관리하기 위한 균일한 방법을 갖습니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551608"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>파트너가 자신의 용도로 Azure 구독을 구매할 수 있도록 Azure Partner Shared Services 추가

**적절한 역할:** 전역 관리자 | 관리 에이전트 | 판매 에이전트

APSS(Azure Partner Shared Services)는 CSP(클라우드 솔루션 공급자) 프로그램의 파트너를 위한 새로운 제품 유형으로, 파트너가 자신의 용도로 Azure 구독을 구매할 수 있도록 합니다.파트너가 Azure 라이선스 및 재판매 계약을 Microsoft와 통합하는 기능 외에도 Azure 구매, 추적 및 관리를 위한 균일한 방법을 사용할 수 있는 기회를 만듭니다. APSS를 사용하면 파트너는 이제 Microsoft 기업계약 및 Web Direct 프로그램에서와 마찬가지로 CSP에서 Azure 구독을 사용할 수 있는 동일한 유연성을 갖게 되며, 개발 및 테스트 환경 빌드, 내부 워크로드 배포, 공유 서비스 또는 다중 테넌트 애플리케이션 호스트와 같은 시나리오를 열 수 있습니다.  

## <a name="create-the-shared-services-tenant"></a>공유 서비스 테넌트 만들기

1. 설정   >  **계정 설정**  >  **공유 서비스 로 이동합니다.**

   :::image type="content" source="images/sharedservices2.png" alt-text="계정 설정 > 공유 서비스":::

2. 공유 서비스 테넌트 가 없는 경우 **공유 서비스 만들기를 선택합니다.**

   :::image type="content" source="images/sharedservices3.png" alt-text="공유 서비스를 만듭니다.":::

3. 이렇게 하면 공유 서비스 테넌트는 생성되고 공유 리소스 및 내부 워크로드에 사용할 Azure CSP 공유 서비스 구독을 구매합니다.

   :::image type="content" source="images/sharedservices5.png" alt-text="테넌트 만들기 및 구독 구매":::

## <a name="about-the-azure--internalshared-services-offer"></a>Azure - Internal/Shared Services 제안 정보

- Azure - Internal/Shared Services 구독은 파트너가 자체 Azure 사용을 위해 얻는 파트너 센터 통해 액세스되는 CSP의 새로운 Azure 제품 유형입니다.

- Azure Partner Shared Services 구독은 적격하며 RIS를 구매하는 데 사용할 수 있습니다.

- Azure - Internal/Shared Services 제안은 공유 서비스 테넌트만 적용할 수 있습니다.

- Azure - Internal/Shared Services 구독의 기본 용도는 자체 개발 목적으로 Azure를 사용할 수 있도록 하는 것입니다. 이 제안을 프로비전하는 데 사용하는 공유 테넌트는 Office 365 또는 Dynamics 라이선스와 같은 다른 서비스에 사용할 수 없습니다.

- 다른 구독처럼 구독을 취소할 수 있습니다. **모든 설정**  >  **보기**  >  **공유 서비스 설정으로 이동합니다.** Azure - Internal/Shared Services 구독을 선택하고 취소합니다.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Azure Partner Shared Services 사용량 세부 정보 액세스

CSP 청구서 및 조정 파일에서 Azure 사용량을 찾을 수 있습니다. 청구서에 Microsoft Azure 품목의 일부로 포함됩니다. 자세한 사용량 정보는 이 제안에 대해 생성된 테넌트에 대해 기록된 조정 파일에서 사용할 수 있습니다.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services 가격 책정

APSS에 대한 새 가격 책정 파일을 보려면 가격 책정 및 제품 **판매로** 이동하여  >   이번 달의 가격 목록을 선택합니다. 앞으로 몇 주 안에 특정 요율 카드 API도 릴리스될 예정입니다.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace 제안 및 Azure Partner Shared Services

2019년 3월 1일부터 APSS는 Marketplace 제안을 더 이상 지원하지 않습니다.

|**Marketplace 지원**   |**2019년 3월 1일 이전에 지원되는 APSS**|**2019년 3월 1일 이후**|
|---------------------------|:----------------------------|:-------------------|
|BYOL(사용자 라이선스 가져오기) 및 무료 서비스   | 예   | 아니요|
|기타 타사 마켓플레이스 제안   | 아니요   |아니요|

APSS를 사용하여 BYOL 또는 무료 서비스를 배포한 파트너는 영향을 받지 않습니다. 그러나 2019년 3월 1일 이후에는 새 BYOL 또는 무료 서비스를 구매할 수 없습니다.

사용 가능한 Marketplace 제품(BYOL 및 무료 서비스뿐만 아니라)의 전체 카탈로그를 활용하려면 CSP 파트너가 웹 직접 Azure 구독을 사용하여 공유 서비스를 배포하는 것이 좋습니다.  이전에 Marketplace에서 타사 BYOL 및 무료 서비스 리소스를 배포했으며 계속 사용하고 더 많은 타사 제품을 배포하려는 CSP 파트너는 APSS 구독을 웹 다이렉트 기존 [Azure 구독 마이그레이션으로 마이그레이션하는](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)것이 좋습니다.

2019년 3월 1일 이후에 APSS 구독을 계속 사용할 계획이며 새로운 타사 [BYOL 서비스](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) 또는 무료 서비스를 배포하려는 파트너는 ISV의 지침에 따라 APSS 구독에 배포할 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [CSP를 통해 소프트웨어 구독 판매](csp-software-subscriptions.md)