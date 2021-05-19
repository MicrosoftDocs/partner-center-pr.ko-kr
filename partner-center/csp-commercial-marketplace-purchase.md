---
title: 상업용 마켓플레이스 제안 구매
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 프로그램 파트너가 파트너 센터 Marketplace를 사용하여 ISV(Independent Software Vendor)에서 고객이 SaaS를 구매하는 방법을 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147856"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>파트너 센터 고객을 위한 상업용 마켓플레이스 제품 구매


**적절한 역할:** 전역 관리자 | 관리 에이전트

CSP(클라우드 솔루션 공급자) 프로그램의 파트너는 상업용 Marketplace를 사용하여 ISV(Independent Software Vendors)에서 제공하는 특정 SaaS(Software as a Service) 제품에 대한 고객의 구독을 구매할 수 있습니다.

고객에게 ISV SaaS 구독을 제공하여 비즈니스를 차별화할 수 있습니다. 특정 비즈니스 요구 사항을 해결하는 소프트웨어 번들에 대한 액세스 권한을 고객에게 제공할 수도 있습니다. Microsoft 제품에 대한 라이선스 및 구독을 관리하는 것처럼 ISV 게시자에서 이러한 마켓플레이스 SaaS 제품에 대한 라이선스 및 구독을 관리합니다.

**라이선스 기반** SaaS 구독 또는 **사용량 기반** 구독을 구매할 수 있습니다. 라이선스 기반 청구와 사용량 기반 청구의 차이점에 대한 자세한 내용은 [청구 기본 사항 을 참조하세요.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>파트너 센터 라이선스 기반 및 요금제 SaaS 구독 구매

Microsoft 제품에 대한 구독을 구매하는 데 사용하는 것과 동일한 프로세스를 사용하여 ISV 게시자가 제공하는 라이선스 기반 또는 요금제 SaaS 제품에 대한 구독을 구매합니다.

파트너 센터 라이선스 기반 또는 요금제 SaaS 구독을 구매하려면 [고객 구독 만들기, 일시 중단 또는 취소를 참조하세요.](create-a-new-subscription.md#create-a-new-subscription)

또한 [Partner Center API](/partner-center/develop/)를 사용하여 고객을 위한 상업용 마켓플레이스 구독을 만들 수도 있습니다. (파트너 센터 API 사용에 대한 자세한 내용은 [상업용 Marketplace 제품에 대한 구독 만들기를 참조하세요.](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> CSP 프로그램의 파트너는 파트너 센터 내에서 ISV 게시자로부터 **라이선스 기반** 또는 **요금제** SaaS 구독을 구매할 수 있습니다. 즉, 액세스 권한이 있는 단독 제안을 포함하여 ISV 게시자가 제공하는 **라이선스 기반** 또는 **요금제** SaaS [제안을](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 구매할 수 있습니다. ISV에서 다른 상업용 Marketplace 제안(예: Azure 애플리케이션, 컨테이너 또는 VM과 관련된 사용량 기반 제안)을 구매하거나 관리하려면 [Azure Portal](https://portal.azure.com/)이동해야 합니다.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Azure Portal 사용량 기반 구독 구매

타사 ISV 게시자의 라이선스 기반 SaaS 구독과 달리 사용량 기반 구독은 먼저 고객에게 Azure 구독이 있어야 합니다. 상업용 Marketplace에 대한 청구, 사용량 기반 리소스는 고객의 Azure 구독에 속합니다. 고객에게 Azure 구독이 있으면 CSP 프로그램의 파트너가 다음 단계에 따라 상업용 Marketplace 구독을 구매할 수 있습니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인한 다음, 왼쪽 메뉴에서 **고객을** 선택합니다.

2. 특정 고객을 선택한 다음, **구독을 선택합니다.**  

3. **사용량 기반 구독** 아래에서 **모든 리소스를 선택합니다.** 그러면 Azure 관리 포털로 이동합니다.

4. Azure 관리 포털의 왼쪽 메뉴에서 **리소스 만들기를** 선택합니다.

5. Azure Marketplace 목록 맨 위에서 **모두 보기를** 선택합니다.

6. 목록 범위를 좁히려면 Marketplace 목록의 맨 위에 있는 필터를 사용합니다. 예를 들어 **게시자** 드롭다운 목록에서 **Microsoft** 또는 **파트너를** 선택하여 Microsoft 또는 ISV 게시자의 제안만 볼 수 있습니다.

7. 특정 제안을 선택한 다음, **만들기를** 선택합니다.

## <a name="next-steps"></a>다음 단계

- [상업용 Marketplace 제안 관리](csp-commercial-marketplace-purchase.md)