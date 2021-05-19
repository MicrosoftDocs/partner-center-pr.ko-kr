---
title: 개요 - CSP 마켓플레이스
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 마켓플레이스의 ISV(Independent Software Vendor)에서 고객에게 SaaS(Software as a Service) 제품 구독을 판매하는 방법을 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7c18f69a62e8f8d126a0756911d2fbcdfdb85d8d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147873"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>파트너 센터의 상업용 Marketplace 개요

**적절한 역할**: 전역 관리자

CSP(클라우드 솔루션 공급자) 프로그램의 파트너가 되면 타사 ISV(Independent Software Vendor)에서 게시한 솔루션과 함께 Microsoft 제품을 번들로 묶고 판매할 수 있습니다. 이러한 방식으로 솔루션을 번들로 묶을 수 있으면 최종 고객에게 더 나은 서비스를 제공하고 CSP 서비스 비즈니스를 성장시킬 수 있습니다.

CSP 프로그램의 파트너는 파트너 센터 사용하여 Microsoft 상업용 Marketplace에서 많은 ISV 솔루션을 구매할 수 있습니다. 이렇게 하면 사용자와 고객에게 다음과 같은 몇 가지 주요 이점이 있습니다.

- Microsoft 기술 및 환경에 최적화된 소프트웨어 솔루션 카탈로그에 액세스합니다.
- 간소화된 계약 및 단축된 조달 주기.
- 파트너 센터 API와 단일 통합. (이러한 통합을 통해 ISV 솔루션 카탈로그에 액세스하고, 운영 및 엔지니어링 비용을 절감하고, 단일 공급자를 통해 여러 공급업체 구독 및 청구 관리를 간소화할 수 있습니다.)
- 고객의 Azure 테넌트에서 간소화된 배포 및 프로비전(Virtual Machine 기반 솔루션용).
- 직접 ISV 구매 또는 계약, Microsoft 솔루션 구성 및 통합, 여러 공급업체의 반복 청구서를 관리 또는 통합해야 할 필요성과 관련된 잠재적인 문제를 줄입니다.

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>상업용 Marketplace의 CSP 제안 개요

CSP 프로그램의 파트너인 경우 ISV 제안과 관련하여 수행할 수 있는 많은 상업용 Marketplace 활동이 있습니다. 각 활동에 대해 자세히 알아보려면 다음 표를 참조하세요.

|**원하는 경우**  |**읽기**   |
|:------------------------------------|:------------------|
|사용 가능한 제품, 가격 책정, 제품 세부 정보 또는 게시자 연락처 정보를 보거나 검색하는 방법을 알아봅니다. | [제안 검색](csp-commercial-marketplace-discover.md) | 
|제안을 구매하고 배포하는 방법 알아보기   | [구매 제안](csp-commercial-marketplace-purchase.md)   | 
|구독을 취소 또는 갱신하거나 라이선스를 추가 또는 제거하는 방법 알아보기  | [제품 관리](csp-commercial-marketplace-manage.md) |
|상업적 marketplace 구매 요금 청구 방식에 대해 알아보기 | [청구 이해](csp-commercial-marketplace-billing.md) |
|ISV 구매에 대 한 지원 유형을 담당 하는 사용자에 대해 알아보기 | [지원 이해](csp-commercial-marketplace-support.md) |
|상업적 marketplace에서 CSP 파트너 및 Isv의 계약 및 책임에 대해 알아봅니다. | [계약 이해](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> 이 개요에서는 CSP 프로그램의 파트너가 파트너 센터의 특정 상업적 marketplace 기능을 사용할 수 있는 방법을 설명 합니다. CSP 프로그램의 파트너와 달리 ISV 게시자에는 다른 마켓플레이스 역할이 있습니다. 파트너 센터 내에서 다른 상업적 Marketplace 기능을 사용할 수도 있습니다. ISV 게시자의 역할에 대해 자세히 알아보려면 [Azure 상용 Marketplace 개요](/azure/marketplace/partner-center-portal/commercial-marketplace-overview)를 참조 하세요.

## <a name="where-to-complete-commercial-marketplace-activities"></a>상업적 marketplace 활동을 완료 하는 위치

CSP 프로그램의 파트너는 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard) 또는 [파트너 센터 api](/partner-center/develop/)를 사용 하 여 ISV SaaS 제품에 대 한 많은 상업적 marketplace 활동을 직접 완료할 수 있습니다. 그러나 다른 marketplace 활동을 완료 하려면 다음으로 이동 해야 할 수 있습니다.

- [Microsoft Azure 관리 포털](https://portal.azure.com/)

    또는

- 타사 ISV 게시자의 시스템 또는 웹 사이트

완료 된 작업으로 이동 하는 대부분은 선택한 제품의 형식으로 시작 합니다. CSP 프로그램의 파트너는 현재 타사 ISV 게시자를 사용 하 여 두 가지 유형의 제품을 제공할 수 있습니다.

1. 라이선스 기반 SaaS 제안  
2. 사용 빈도 기반 제공 (가상 머신, 컨테이너 또는 Azure 응용 프로그램을 기반으로 하는 제품 포함)

청구 [기본 사항](billing-basics.md) 으로 이동 하 여 라이선스 기반 제품 및 사용량 기반 제품 간의 요금이 어떻게 다른 지에 대해 자세히 알아보세요.  

라이선스 기반 또는 사용량 기반 ISV 제안에 대한 특정 마켓플레이스 활동을 완료할 위치를 알아보려면 다음 표를 참조하세요.

|**ISV의 라이선스 기반 또는 요금제 SaaS 제안의 경우**  |**사용**  |
|:------------------------------------|:------------------|
|사용 가능한 제안을 검색하거나 검색하려면  | 대시보드 또는 파트너 센터 API 파트너 센터  |
|제안을 구매하려면  | 대시보드 또는 파트너 센터 API 파트너 센터  |
|구매한 제안(고객의 AAD 테넌트에서 계정 설정, 소프트웨어 관리 또는 배포)을 배포하려면  | ISV 게시자의 시스템 또는 웹 사이트  |
|제품 구독을 취소/갱신하거나 라이선스를 추가/제거하려면 | 대시보드 또는 파트너 센터 API 파트너 센터  |
|사용자를 만들거나 사용 권한을 관리하려면  | ISV 게시자의 시스템 또는 웹 사이트  |

|**ISV의 사용량 기반 제안**  |**사용**  |
|:------------------------------------|:------------------|
|사용 가능한 제안을 검색하거나 검색하려면  | 대시보드, 파트너 센터 API 또는 Azure Portal 파트너 센터  |
|제안을 구매하려면  | Azure Portal  |
|구매한 제안(고객의 AAD 테넌트에서 계정 설정, 소프트웨어 관리 또는 배포)을 배포하려면  | Azure Portal  |
|제품 구독을 취소/갱신하거나 라이선스를 추가/제거하려면 | Azure Portal  |
|사용자를 만들거나 사용 권한을 관리하려면  | Azure portal  |

## <a name="next-steps"></a>다음 단계

- [상업용 Marketplace 제안 검색 또는 보기](csp-commercial-marketplace-discover.md)
- [상업적 marketplace 제품 구매](csp-commercial-marketplace-purchase.md)
