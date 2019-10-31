---
title: CPOR 모델을 사용 하 여 고객 연결 만들기 | 파트너 센터
ms.topic: article
ms.date: 10/29/2019
description: CPOR 모델을 사용 하 여 고객 연결 만들기
author: LauraBrenner
ms.author: labrenne
keywords: 성과급 청구, 공동 op 클레임, 공동 작동 자금, OSU, OSA, ISV, 수익 연결
ms.localizationpriority: medium
ms.openlocfilehash: 9acac203d44e3942f9a07bc5af90528e558bce39
ms.sourcegitcommit: 014669c26592a3ab35c2aa7f3ff615f5f1091752
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/30/2019
ms.locfileid: "73083863"
---
**적용 대상**

-  파트너 센터

# <a name="create-a-customer-association-using-the-cpor-model"></a>CPOR 모델을 사용 하 여 고객 연결 만들기

2019 년 10 월 1 일부 터 Microsoft는 Microsoft에서 Microsoft의 Microsoft 서비스 자문 (온라인 서비스 자문) 판매, OSU (온라인 서비스 사용)와 관련 하 여 Microsoft 365 및 Dynamics 365 고객과의 연결을 관리 하기 위해 CPOR (Record Partner of Record) 모델을 사용 하기 시작 했습니다. Microsoft 365 및 OSU-비즈니스 응용 프로그램의 성과급입니다.

클레임을 제출 하면 Microsoft에서 유효성을 검사 합니다. 이 시점에서 추가 정보를 요청할 수 있습니다. 또한 고객의 연결 요청에 대해 알려줍니다. 고객은 옵트아웃 (opt out)을 5 영업일 이내에 사용할 수 있습니다. 옵트아웃 (opt out) 하지 않으면이 특정 테 넌 트 및 워크 로드와의 연결이 공식적으로 적용 됩니다. 이 시점에서 고객의 사용 현황 데이터에 액세스할 수 있습니다. 

클레임을 완료 하려면 다음 정보가 필요 합니다.

- 클레임을 만드는 엔터티의 **MPN ID**

- 고객의 **도메인 이름** [이를 찾습니다](https://docs.microsoft.com/partner-center/find-customer-domain-name) .

- 고객의 **디렉터리 id** 또는 **테 넌 트 id** 를 [찾습니다](https://docs.microsoft.com/partner-center/find-customer-domain-name) .

- Business Applications 또는 Microsoft 365와 같은 **솔루션 영역**

- 수행 된 **작업** 및 수행 하려는 클레임 유형 (예: 판매 전, 사용량 또는 수입 연결)

- 고객의 **연락처 이름**, 제목 및 전자 메일 주소

- Dynamics 365의 경우 고객의 **기술 담당자** 이름, 제목 및 전자 메일 주소도 제공 해야 합니다.

- 회사의 **연락처 이름** 및 전자 메일 주소

- 이 클레임에 대 한 **이름을** 만듭니다.

- 주장 하는 **제품** 또는 워크 로드

- **POE (실행 증명) (** 예: 고객이 서명한 작업의 문) POE 템플릿을 다운로드 하 여 사용할 수도 있습니다.

- 수익 연결만을 주장 하는 파트너의 경우: **Dynamics solution 판매자 이름**, **고객 이름**및 **ISV 제품/솔루션의 이름**입니다. 

또한 다음 사항을 이해 해야 합니다.
- 기존 Microsoft 365 고객이 있는 경우이 프로세스를 사용 하 여 계속 해 서 OSU의 성과급을 얻을 수 있도록 다시 연결 해야 합니다.
- Dynamics 365 또는 Power BI 고객에 대 한 기존 연결이 있는 경우 구독이 만료 될 때까지 이러한 연결은 유효한 상태로 유지 됩니다.
- 고객은 여러 파트너를 가질 수 있지만 각 워크 로드 (OSU Microsoft 365의 경우) 또는 구독 (OSA-판매 및 OSU-Business Applications)은 한 파트너에만 연결 될 수 있습니다.

## <a name="create-a-customer-association"></a>고객 연결 만들기
1.  파트너 센터 대시보드의 **성과급**아래에서 **개요**를 선택한 다음, **고객 연결**을 선택 합니다. 

2.  고객 연결 페이지의 맨 위에서 **+ 고객 연결**을 선택 합니다.

3.  고객과 연결할 파트너 위치의 **MPN id** 를 선택 하 고 고객의 도메인 이름과 디렉터리 id를 추가 합니다. [어디에 있나요?](https://docs.microsoft.com/partner-center/find-customer-domain-name)

**계속**을 선택합니다.

4.  **솔루션 영역** 및 **활동**을 선택 합니다. 

>[!Note]

>Business Applications를 선택 하는 경우 **사용량 및/또는 판매 전**또는 **수입 연결**중 하나를 선택한 다음 **계속**을 선택 합니다. 

>수익 연결을 선택 하는 경우 아래 나열 된 것과 약간 다른 정보를 묻는 메시지가 표시 됩니다. 

5.  **고객 연결** 페이지에 적절 한 정보를 입력 하 고 **클레임 만들기**를 선택 합니다.

6.  이 고객 연결과 관련 된 제품을 선택 하 고 **계속**을 선택 합니다.

7.  고객 연락처 정보 및 회사의 연락처 정보를 입력 합니다. 모든 필드가 필수 필드입니다. 

>[!Note]

제품이 Dynamics 365이 고 선택한 제품에이 특정 고객에 대 한 구독이 여러 개 있는 경우 구독 ID도 입력 해야 합니다.

8.  실행 증명 (POE)을 제공 합니다. 이 상자를 상자로 끌거나, 고유한 지원 설명서를 찾아보거나, **템플릿 다운로드**를 선택 하 여 템플릿을 사용할 수 있습니다. 

9.  원하는 경우 주석을 추가 하 고 저장 한 다음 **클레임 제출**을 선택 합니다. 고객 연결에 대 한 승인을 요청 하는 고객에 게 전자 메일을 보냅니다. 

>[!NOTE]

>고객 연결을 제출한 후에는 편집할 수 없습니다. 

고객 연결의 상태가 **상태** 필드에 표시 됩니다. 

**기록** 을 선택 하 여 고객 연결 기록을 봅니다.
