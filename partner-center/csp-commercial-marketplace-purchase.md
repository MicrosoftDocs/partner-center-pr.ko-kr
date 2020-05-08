---
title: 상업적 marketplace 제품 구매
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 프로그램 파트너가 파트너 센터 마켓플레이스를 사용 하 여 Isv (독립 소프트웨어 공급 업체)의 SaaS 제품을 고객에 게 구매할 수 있는 방법에 대해 알아봅니다.
author: LauraBrenner
ms.author: labrenne
keywords: 구독, marketplace, 상용 마켓플레이스, 타사, ISV, SaaS 제품, 클라우드 솔루션 공급자 프로그램, 제품 구매, 구독 구매
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c740ae823670644cb1f81c0a667d1fb48fc873ae
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908084"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>파트너 센터에서 고객을 위한 상용 마켓플레이스 제품 구매

**적용 대상**

- 파트너 센터
- CSP 프로그램의 파트너

**적절한 역할**

- 글로벌 관리자
- 관리 에이전트

CSP (클라우드 솔루션 공급자) 프로그램의 파트너는 상업적 marketplace를 사용 하 여 Isv (독립 소프트웨어 공급 업체)에서 제공 하는 특정 SaaS (Software as a Service) 제품에 대 한 고객의 구독을 구매할 수 있습니다. 

ISV SaaS 구독을 고객에 게 제공 하 여 비즈니스를 차별화 하는 데 도움을 받을 수 있습니다. 또한 고객에 게 특정 비즈니스 요구 사항을 충족 하는 소프트웨어 번들에 대 한 액세스 권한을 제공할 수 있습니다. Microsoft 제품에 대 한 라이선스 및 구독을 관리 하는 것 처럼 ISV 게시자의 이러한 marketplace SaaS 제품에 대 한 라이선스 및 구독을 관리 합니다.

**라이선스 기반** SaaS 구독 또는 **사용 빈도 기반** 구독 중 하나를 구입할 수 있습니다. 라이선스 기반 및 사용량 기준 청구의 차이점에 대해 자세히 알아보려면 [청구 기본 사항](billing-basics.md)을 참조 하세요.

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>파트너 센터에서 라이선스 기반 SaaS 구독 구매

Microsoft 제품에 대 한 구독을 구매 하는 데 사용한 것과 동일한 프로세스를 사용 하 여 ISV 게시자가 제공 하는 라이선스 기반 SaaS 제품에 대 한 구독을 구입 합니다

파트너 센터에서 라이선스 기반 SaaS 구독을 구매 하려면 [고객 구독 만들기, 일시 중단 또는 취소](create-a-new-subscription.md#create-a-new-subscription)를 참조 하세요.

또한 [Partner Center API](https://docs.microsoft.com/partner-center/develop/)를 사용하여 고객을 위한 상업용 마켓플레이스 구독을 만들 수도 있습니다. 파트너 센터 Api를 사용 하는 방법에 대 한 자세한 내용은 [상용 marketplace 제품에 대 한 구독 만들기](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)를 참조 하세요.

>[!IMPORTANT]
> CSP 프로그램의 파트너는 파트너 센터 내에서 ISV 게시자의 **라이선스 기반** SaaS 구독만 구매할 수 있습니다. 즉, 사용자가 액세스할 수 있는 [전용 제품](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 을 비롯 하 여 ISV 게시자가 사용할 수 있도록 설정한 모든 **라이선스 기반** SaaS 제품을 구매할 수 있습니다. Isv (Azure 응용 프로그램, 컨테이너 또는 Vm과 관련 된 **사용량 기반**, 요금제 또는 소비 기반 제품)에서 기타 상업적 marketplace 제품을 구매 하거나 관리 하려면 [Azure Portal](https://portal.azure.com/)으로 이동 해야 합니다. 자세한 내용은 다음 항목을 참조 하세요.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Azure Portal에서 사용 빈도 기반 구독 구매

타사 ISV 게시자의 라이선스 기반 SaaS 구독과 달리, 사용 빈도 기반 구독에는 먼저 고객이 Azure 구독을 보유 해야 합니다. 상용 marketplace에 대 한 청구, 사용량 기반 리소스는 고객의 Azure 구독에 속합니다. 고객이 Azure 구독을 보유 하 고 있는 경우 CSP 프로그램의 파트너는 다음 단계를 수행 하 여 상업적 marketplace 구독을 구매할 수 있습니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 한 후 왼쪽 메뉴에서 **고객** 을 선택 합니다.

2. 특정 고객을 선택한 다음 **구독**을 선택 합니다.  

3. **사용 빈도 기반 구독**에서 **모든 리소스**를 선택 합니다. Azure 관리 포털로 이동 합니다.

4. Azure 관리 포털의 왼쪽 메뉴에서 **리소스 만들기** 를 선택 합니다.

5. Azure Marketplace 목록의 맨 위에 있는 **모두 보기** 를 선택 합니다.

6. 목록을 좁히려면 Marketplace 목록 위쪽의 필터를 사용 합니다. 예를 들어 **게시자** 드롭다운 목록에서 **microsoft** 또는 **Partner** 를 선택 하 여 microsoft 또는 ISV 게시자의 제품을 볼 수 있습니다.

7. 특정 제품을 선택 하 고 **만들기**를 선택 합니다.

## <a name="next-steps"></a>다음 단계

- [상업적 마켓플레이스 제품 관리](csp-commercial-marketplace-purchase.md)