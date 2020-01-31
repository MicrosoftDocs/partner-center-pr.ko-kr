---
title: 제한 된 직접 청구 기능 | 파트너 센터
ms.topic: article
ms.date: 01/24/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 새 요구 사항을 충족 하지 않는 직접 청구 파트너는 직접적인 청구 기능이 제한 됩니다.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: 직접 청구, 제한
ms.openlocfilehash: 7f2dae72edff59b3e6d84c74f93bae437be4ce30
ms.sourcegitcommit: d11c52e1386c181e177df72d6c7244508f1d6c0e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/29/2020
ms.locfileid: "76860504"
---
# <a name="restricted-direct-bill-capabilities"></a>제한 된 직접 청구 기능  

**개요**

직접 청구 파트너는 CSP 직접 청구 파트너 프로그램에 남아 있어야 하는 새 [요구 사항을](direct-partner-new-requirements.md) 충족 해야 합니다. 그렇지 않으면 직접 청구 기능에 대 한 액세스 권한이 결국 제한 되며 고객에 게 새로운 구매와 같은 특정 작업을 수행할 수 있습니다. 

>[!Note]
>CSP 직접 청구 파트너 프로그램에 대 한 새로운 요구 사항을 충족 하지 않는 직접 청구 파트너는 직접적인 청구 기능을 제한할 때 Microsoft에서 알려줍니다. 이는 [직접 청구 파트너에서 간접 대리점으로의 전환이](transition-direct-to-indirect.md) 옵트인 되었는지 여부에 관계 없이 모든 직접 청구 파트너에 적용 됩니다.  
 
## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>직접 청구 기능이 제한 되었는지 여부를 확인 하는 방법 

직접 청구 기능에 대 한 직접 청구 파트너 테 넌 트의 액세스가 제한 되었는지 여부를 확인 하려면 다음을 수행 합니다. 

1. [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다. 

2. 파트너 **설정** -> **파트너 프로필**로 이동 합니다. 

3. **프로그램 정보**에서 **Microsoft 클라우드 솔루션 공급자 상태**를 찾습니다. 

4. 프로그램 상태에 값이 **제한**되어 있는 경우 직접 청구 기능에 대 한 직접 청구 파트너 테 넌 트의 액세스가 제한 되어 있음을 의미 합니다. 
 
## <a name="affected-direct-bill-capabilities"></a>영향을 받는 직접 청구 기능 

직접 청구 기능이 제한 된 경우 더 이상 파트너 센터에서 고객에 대 한 새로운 구매를 수행할 수 없습니다. 여기에는 다음이 포함됩니다. 

- Azure 구독 
- 사용자 기반 구독 
- 기존 사용자 기반 구독에 새 추가 기능을 추가 합니다. 
- 소프트웨어 및 예약 제품 (예: 소프트웨어 구독, 영구 소프트웨어 및 Azure 예약 가상 컴퓨터 인스턴스)에 대 한 일회성 구매 

CSP 프로그램 아래에서 [azure partner shared services 제품](shared-services.md) 을 사용 하 여 사용자의 고유한 용도에 대 한 새 azure 구독을 구매할 수도 없습니다. 

기존 직접 청구 구독은 영향을 받지 않습니다. 이는 유효한 상태로 유지 되 고 자동 갱신 됩니다. 취소 될 때까지 Microsoft에서 직접 청구 됩니다. 다음과 같은 방법으로 기존 구독을 계속 관리할 수 있습니다. 

- 기존 구독 일시 중단 
- 기존 사용자 기반 구독의 좌석 수 조정 
- 구독에 대 한 기존 추가 기능의 수를 조정 합니다. 참고: 새 구입으로 처리 되므로 기존 구독에 새 추가 기능을 추가할 수 없습니다. 
- 기존 azure 구독에서 새 Azure 리소스를 배포 하 고 기존 Azure 리소스를 관리 합니다. 여기에는 Azure marketplace 및 Visual Studio 구독을 통해 사용할 수 있는 리소스가 포함 됩니다. 

새 구매 외에도 파트너 센터에서 다음과 같은 직접 청구 기능에 액세스할 수 없습니다. 

- 새 고객 테 넌 트를 만들 수 없습니다. 파트너 센터의 **고객** 페이지에서 **고객 만들기** 옵션을 사용할 수 없습니다. 
- 고객에 게 직접 재판매인 관계를 요청 하는 초대를 생성할 수 없습니다. 파트너 센터의 **고객** 페이지에서 **재판매인 관계 요청** 옵션은 사용할 수 없습니다. 

    >[!Note]
    >직접 청구 파트너에서 간접 재판매인으로 전환 하는 과정의 일환으로, 직접 청구 파트너 테 넌 트를 간접 재판매인으로 등록 한 경우 대신 간접 대리점 관계를 요청 하는 고객에 게 초대를 생성할 수 있습니다. 
 
- 새 샌드박스 테 넌 트를 만들 수 없습니다. 각 직접 청구 파트너 테 넌 트는 직접 청구 API 통합을 위해 하나의 샌드박스 테 넌 트를 만들 수 있습니다. 이전에 만든 적이 없는 경우 청구서 파트너 기능이 제한 된 후에는이 작업을 수행할 수 없습니다.  

## <a name="see-also"></a>참고 항목 
- [간접 재판매인의 추가 정보](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf) 
- [CSP 직접 파트너 새로운 요구 사항](direct-partner-new-requirements.md)