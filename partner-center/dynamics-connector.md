---
title: Dynamics 365 CRM 파트너 센터 용 공동 판매 커넥터
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dynamics 365 커넥터를 사용 하 여 Microsoft에서 조회를 가져옵니다.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: bddd29e9136d998ef8a25616d2058d1380b36665
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825690"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM 용 공동 판매 커넥터-개요

### <a name="appropriate-roles"></a>적절한 역할

- 조회 관리자
- CRM에서 시스템 관리자 또는 시스템 사용자 지정자

파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다. 파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다. 공동 판매 커넥터를 사용 하 여 microsoft 판매자와 협력 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 가치, 마감 날짜 등의 거래 데이터를 수정 하 고, 이러한 공동 판매 거래에 대 한 Microsoft 판매자의 업데이트를 받을 수 있는 새로운 공동 판매 참조를 만들 수 있습니다. 파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안이 모든 작업을 수행할 수 있습니다. 

이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 Microsoft 파트너 센터 Api를 사용 합니다.

## <a name="before-you-install---pre-requisites"></a>설치 전-필수 구성 요소

|**토픽**   |**세부 정보**   |**링크**   |
|--------------|--------------------|------|
|Microsoft 파트너 네트워크 ID |유효한 MPN ID가 필요 합니다.|[MPN](https://partner.microsoft.com/) 에 조인 하려면|
|공동 판매 준비|I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.|[Microsoft와 판매](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|파트너 센터 계정|파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다. 커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.|[계정 관리](create-user-accounts-and-set-permissions.md)|
|파트너 센터 사용자 역할|커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.|[사용자 역할 및 권한 할당](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.|[Dynamics 365에서 역할 할당](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|전원 자동화 흐름 계정|CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정 사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365에 대 한 파트너 센터 조회 동기화 설치 (전원 자동화 솔루션) 

1. [전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다. 그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.

2. 오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다. 

3. 왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.

4. 상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.

![AppSource 열기](images/cosellconnectors/openappsource.png)

5. **Dynamics365에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.  

6. **지금 가져오기** 단추를 클릭 한 다음 **계속**합니다. 

7. 그러면 응용 프로그램을 설치할 CRM (Dynamics 365) 환경을 선택할 수 있는 페이지가 열립니다.  사용 약관에 동의 합니다. 

8. 그런 다음 **솔루션 관리** 페이지로 이동 합니다.  페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다. 파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다. 설치는 10-15 분 정도 걸립니다. 

9. 설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다. **Dynamics 365에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 확인할 수 있습니다.

10. **Dynamics 365에 대 한 파트너 센터 조회 동기화를**선택 합니다. 다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.

![사용 가능한 CRMS](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>모범 사례: 라이브 상태로 전환 하기 전에 테스트

프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.

- 스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.
- 솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 수행 합니다.
- 스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다. 
- 성공할 경우 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다. 

## <a name="configure-the-solution"></a>솔루션 구성

1. CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.

2. 오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.

3. 세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다. 

- 조회 관리자 자격 증명이 있는 파트너 센터 사용자 
- 파트너 센터 이벤트
- 솔루션에서 흐름을 자동화 하는 CRM admin 

    a. 왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.
    b. **연결 만들기**를 클릭 하 여 연결을 만듭니다. 

    ![연결 만들기](images/cosellconnectors/createconnection.png)
    
    c. 오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.
    d. 조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다. 우표. 다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다. 350. CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.

4. 전원 자동화 흐름을 연결과 연결 하려면 각 전원 자동화 흐름을 편집 하 여 Common Data Service 및 파트너 센터 조회에 연결 합니다. 변경 내용을 저장합니다.

5. 전원 자동화 흐름을 **켭니다** .

## <a name="next-steps"></a>다음 단계

- [웹 후크를 사용 하 여 리소스 변경 이벤트 가져오기](referral-connector-webhooks.md)

- [Microsoft Power 자동화 플랫폼에 대 한 자세한 정보](https://docs.microsoft.com/power-automate/)

- [잠재 고객 관리](manage-leads.md)

- [공동 판매 기회 관리](manage-co-sell-opportunities.md)

