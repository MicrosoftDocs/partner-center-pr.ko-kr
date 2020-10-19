---
title: 고객 제휴 만들기
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 클레임 파트너 (CPOR) 모델을 사용 하 여 고객 연결을 만듭니다. Microsoft 365 & Dynamics 365 고객에 대 한 판매, 사용량, 성과급을 관리 하는 데 도움이 됩니다.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92174996"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Microsoft 365 및 Dynamics 365에 대해 요청 된 CPOR (레코드 파트너) 모델을 통한 고객 연결

**적용 대상**

- 파트너 센터

**적절한 역할:**

- 인센티브 관리자

2019 년 10 월 1 일부 터 Microsoft는 Microsoft에서 Microsoft의 Microsoft Microsoft 365 및 Dynamics 365 고객과의 연결을 관리 하기 위해 Microsoft의 OSA (온라인 서비스 자문) 판매, OSU (온라인 서비스 사용) Microsoft 365 및 OSU-Business 응용 프로그램에 대 한 사용과 관련 된 연결을 관리 하기 시작 했습니다.

>[!Important]
> CPOR (고객 연결) 클레임은 OSA (Online services Advise) 판매, OSU (온라인 서비스 사용) Microsoft 365 및 OSU-Business 응용 프로그램 동기 프로그램에만 적용 됩니다. 클라우드 솔루션 공급자, 관리 재판매인, 호스팅 또는 화면과 같은 다른 프로그램에 대 한 공동 작업 클레임을 제출 하는 경우 여기에 설명 된 Co op 클레임 프로세스를 참조 하세요. <br><br>클레임을 제출 하면 Microsoft에서 유효성을 검사 합니다. 이 시점에서 추가 정보를 요청할 수 있습니다. 또한 고객의 연결 요청에 대해 알려줍니다. 고객은 옵트아웃 (opt out)을 5 영업일 이내에 사용할 수 있습니다. 옵트아웃 (opt out) 하지 않으면이 특정 테 넌 트 및 워크 로드와의 연결이 공식적으로 적용 됩니다. 이 시점에서 고객의 사용 현황 데이터에 액세스할 수 있습니다. 

클레임을 완료 하려면 다음 정보가 필요 합니다.

- 클레임을 만드는 엔터티의 **MPN ID**

- 고객의 **도메인 이름** [이를 찾습니다](find-domain-name.md) .

- 고객의 **디렉터리 id** 또는 **테 넌 트 id** 를 [찾습니다](find-domain-name.md) .

- Business Applications 또는 Microsoft 365와 같은 **솔루션 영역**

- 수행 된 **작업** 및 수행 하려는 클레임 유형 (예: 판매 전, 사용량 또는 수입 연결)

- 고객의 **연락처 이름**, 제목 및 전자 메일 주소

- Dynamics 365의 경우 고객의 **기술 담당자** 이름, 제목 및 전자 메일 주소도 제공 해야 합니다.

- 회사의 **연락처 이름** 및 전자 메일 주소

- 이 클레임에 대 한 **이름을** 만듭니다.

- 주장 하는 **제품** 또는 워크 로드

- **PoE (실행 증명) (** 예: 고객이 서명한 작업의 문) PoE 템플릿을 다운로드 하 여 사용할 수도 있습니다.

- 수익 연결만을 주장 하는 파트너의 경우: **Dynamics solution 판매자 이름**, **고객 이름**및 **ISV 제품/솔루션의 이름**입니다. 

또한 다음 사항을 이해 해야 합니다.

- 기존 Microsoft 365 고객이 있는 경우이 프로세스를 사용 하 여 계속 해 서 OSU의 성과급을 얻을 수 있도록 다시 연결 해야 합니다.

- Dynamics 365 또는 Power BI 고객에 대 한 기존 연결이 있는 경우 구독이 만료 될 때까지 이러한 연결은 유효한 상태로 유지 됩니다.

- 고객은 여러 파트너를 가질 수 있지만 각 작업 (OSU-Microsoft 365의 경우) 또는 구독 (OSA-Sell 및 OSU-Business 응용 프로그램의 경우)은 한 파트너에만 연결 될 수 있습니다.

## <a name="create-a-customer-association"></a>고객 제휴 만들기

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. **성과급** 탭을 선택 하 고 **개요**를 선택한 다음 **고객 연결**을 선택 합니다.

3. 고객 연결 페이지의 맨 위에서 **+ 고객 연결**을 선택 합니다.

4. 고객과 연결할 파트너 위치의 **MPN ID**를 선택한 다음 고객의 도메인 이름과 디렉터리 ID를 추가합니다. [찾을](find-domain-name.md)

5. **계속**을 선택합니다.

6. **솔루션 영역** 및 **활동**을 선택 합니다. 

   >[!Note]
   >
   >Business Applications를 선택 하는 경우 **사용량 및/또는 판매 전**또는 **수입 연결**중 하나를 선택한 다음 **계속**을 선택 합니다. 
   <br><br>수익 연결을 선택하는 경우 아래 나열된 것과 약간 다른 정보를 묻는 메시지가 표시됩니다.

7. **고객 연결** 페이지에 적절 한 정보를 입력 하 고 **클레임 만들기**를 선택 합니다.

8. 이 고객 연결과 관련 된 제품을 선택 하 고 **계속**을 선택 합니다.

9. 고객 연락처 정보 및 회사의 연락처 정보 입력을 완료합니다. 모든 필드는 필수입니다. 

   >[!NOTE]
   >제품이 Dynamics 365이 고 선택한 제품에이 특정 고객에 대 한 구독이 여러 개 있는 경우 구독 ID도 입력 해야 합니다.

10. 실행 증명 (PoE)을 제공 합니다. 이를 상자로 끌거나, 고유한 지원 설명서를 찾아보거나, **템플릿 다운로드**를 선택하여 템플릿을 사용할 수 있습니다. 

11. 원하는 경우 설명을 추가하여 저장한 다음 **클레임 제출**을 선택합니다. 고객 연결에 대한 승인을 요청하는 고객에게 이메일이 전송됩니다.

   >[!NOTE]
   >고객 연결을 제출한 후에는 편집할 수 없습니다.

고객 연결의 상태가 **상태** 필드에 표시됩니다.

**기록**을 선택하여 고객 연결 기록을 볼 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [고객 제휴 보기](incentives-manage-customer-associations.md)