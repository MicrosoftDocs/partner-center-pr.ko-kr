---
title: 제한된 직접 청구 기능
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP(클라우드 솔루션 공급자) 직접 청구 파트너 요구 사항 및 기능이 제한되지 않도록 하기 위해 수행할 작업을 알아봅니다. 기능이 제한되었는지 확인합니다.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551421"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>제한된 직접 청구 기능 및 CSP 직접 청구 파트너에 필요한 요구 사항

**적절한 역할**: 전역 관리자

## <a name="overview"></a>개요

직접 청구 파트너는 CSP(클라우드 솔루션 공급자) 직접 청구 파트너 프로그램에 남아 있는 새로운 [요구 사항을](direct-partner-new-requirements.md) 충족해야 합니다. 충족하지 못하면 직접 청구 기능에 대한 액세스 권한이 제한되며 고객의 신규 구매와 같은 특정 작업을 더 이상 수행할 수 없습니다.

> [!Note]
> CSP 직접 청구 파트너 프로그램에 대한 새로운 요구 사항을 충족하지 않는 직접 청구 파트너는 직접 청구 기능이 제한될 때 Microsoft에서 알 수 있습니다. 이는 직접 청구 파트너에서 간접 대리점으로의 전환을 선택했는지 여부에 관계없이 모든 [직접 청구 파트너에게 적용됩니다.](transition-direct-to-indirect.md)  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>직접 청구 기능이 제한되었는지를 알려주는 방법

직접 청구 파트너 테넌트에서 직접 청구 기능으로의 액세스가 제한되었는지 확인하려면 다음 단계를 수행합니다.

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 계정 **설정** 법적 프로필 로  >  이동합니다.

3. **프로그램 정보** 에서 **Microsoft 클라우드 솔루션 공급자 상태를** 찾습니다.

4. 프로그램 상태에 값이 **제한된** 경우 직접 청구 파트너 테넌트의 직접 청구 기능에 대한 액세스가 제한되었습니다.

## <a name="affected-direct-bill-capabilities"></a>영향을 받는 직접 청구 기능

직접 청구 기능이 제한된 경우 더 이상 파트너 센터 고객을 위해 새 구매를 할 수 없습니다. 이 제한에는 다음이 포함됩니다.

- Azure 구독

- 라이선스 기반 구독

- 기존 라이선스 기반 구독에 새 추가 기능 추가

- 소프트웨어 및 예약 제품(예: 소프트웨어 구독, 영구 소프트웨어 및 Azure Reserved Virtual Machine 인스턴스)을 한 번 구매합니다.

또한 CSP 프로그램에서 [Azure 파트너 공유 서비스 제안을](shared-services.md) 사용하여 사용자 고유의 용도로 새 Azure 구독을 구매할 수 없습니다.

기존 직접 청구 구독은 영향을 받지 않습니다. 유효한 상태로 유지되고 자동 새로 고침됩니다. 취소될 때까지 Microsoft에서 직접 요금이 계속 청구됩니다. 다음과 같은 방법으로 기존 구독을 계속 관리할 수 있습니다.

- 기존 구독 일시 중단

- 기존 라이선스 기반 구독의 라이선스 수 조정

- 구독에 대한 기존 추가 기능의 라이선스 수를 조정합니다. 

    >[!Note]
    >새 구매로 처리되는 기존 구독에는 새 추가 기능 을 추가할 수 없습니다.

- 새 Azure 리소스를 배포하고 기존 Azure 구독에서 기존 Azure 리소스를 관리합니다. 여기에는 Azure Marketplace 및 Visual Studio 구독을 통해 사용할 수 있는 리소스가 포함됩니다.

새 구매 외에도 파트너 센터 다음과 같은 직접 청구 기능에 액세스할 수 없습니다.

- 새 고객 테넌트는 만들 수 없습니다. 파트너 센터 **고객** 페이지에서 **고객 만들기** 옵션을 사용할 수 없습니다.

- 직접 대리점 관계를 요청하는 고객에게 초대를 생성할 수 없습니다. 파트너 센터 **고객** 페이지의 **대리점 관계 요청** 옵션을 사용할 수 없습니다.

    >[!NOTE]
    >직접 청구 파트너에서 간접 대리점으로 전환하는 과정의 일환으로 직접 청구 파트너 테넌트를 간접 대리점으로 이미 등록한 경우 간접 대리점 관계를 요청하는 고객에게 초대를 대신 생성할 수 있습니다.

- 새 샌드박스 테넌트는 만들 수 없습니다. 각 직접 청구 파트너 테넌트는 직접 청구 API 통합을 위해 하나의 샌드박스 테넌트만 만들 수 있습니다. 이전에 만들지 않은 경우 직접 청구 파트너 기능이 제한된 후에는 만들 수 없습니다.  

## <a name="next-steps"></a>다음 단계

- [간접 재판매인이 되기 위한 추가 정보](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP 직접 파트너 새로운 요구 사항](direct-partner-new-requirements.md)
