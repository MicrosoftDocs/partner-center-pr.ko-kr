---
title: 제어판 공급 업체로 등록
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 파트너 센터에서 CPV (제어판 공급 업체)로 등록 하는 방법에 대해 알아봅니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b6258f54120e0a40f94ad74a76821c4222eb0ef4
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87545894"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>CSP 파트너 시스템을 파트너 센터 Api와 통합 하는 데 도움이 되는 제어판 공급 업체로 등록

**적용 대상**

- 파트너 센터

**적절한 역할**

- 전역 관리자

CPV (제어판 공급 업체)는 CSP (클라우드 솔루션 공급자) 파트너가 시스템을 파트너 센터 Api와 통합할 수 있도록 응용 프로그램을 개발 하는 독립 소프트웨어 공급 업체입니다. 제어판 공급 업체는 파트너 센터 대시보드 또는 파트너 센터 Api에 직접 액세스할 수 있는 CSP 파트너가 아닙니다.

현재는 CPV (현재 제어판 공급 업체) 또는 Microsoft 파트너와 함께 작업 하고자 하는 새 CPV를 사용 하 여 응용 프로그램을 등록 하 고 클라우드 솔루션 공급자 파트너를 지원 하기 위해 이제 파트너 센터에 등록 해야 합니다. 계정을 만들기 위해 CPV 파트너는 기존 CSP 파트너 테 넌 트 또는 기존 CPV 테 넌 트를 사용 하거나 온 보 딩 프로세스의 일부로 새 테 넌 트를 만들 수 있습니다. CPV 파트너가 기존 CSP 테 넌 트를 사용 하도록 선택 하는 경우 별도의 다중 테 넌 트 응용 프로그램을 만들고이를 CPV 활동의 파트너 센터에 등록 해야 합니다. 응용 프로그램을 CSP 및 CPV 응용 프로그램으로 등록할 수 없습니다. 파트너 센터에 등록 하 고 응용 프로그램을 등록 한 후에는 파트너 센터 Api에 액세스할 수 있습니다.  Microsoft는 샌드박스 정보를 사용 하 여 파트너 센터 알림을 통해 사용자에 게 연락 합니다. 샌드박스 계정이 이미 있는 경우 계속 사용 합니다. 새 샌드박스가 필요 하지 않습니다.

[Microsoft 제어판 공급 업체 규약](https://go.microsoft.com/fwlink/?linkid=2055198) 검토


## <a name="working-in-partner-center"></a>파트너 센터에서 작업
파트너 센터 CPV 환경을 등록 하 고 CPV 규약을 승인한 후 다음을 수행할 수 있습니다.

- 다중 테 넌 트 응용 프로그램을 관리 합니다 (파트너 센터에서 응용 프로그램을 Azure Portal, 등록 및 등록 취소 하는 응용 프로그램 추가).

    >[!Note] 
    >CPVs는 파트너 센터 Api에 대 한 권한을 부여 받으려면 파트너 센터에서 해당 응용 프로그램을 등록 해야 합니다. Azure Portal에 애플리케이션을 추가하는 것만으로는 파트너 센터 API에 대한 권한이 CPV 애플리케이션에 부여되지 않습니다. 

- CPV 프로필을 보고 관리합니다. 

- CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다. 전역 관리자는 CPV가 가질 수 있는 유일한 역할입니다.


