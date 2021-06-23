---
title: 고객 제휴 만들기
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: CPOR(Claiming Partner of Record) 모델을 사용하여 고객 연결을 만듭니다. Microsoft 365 & Dynamics 365 고객에 대한 판매, 사용량, 인센티브 관리를 지원합니다.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489954"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a>Microsoft 365 및 Dynamics 365에 대해 CPOR(클레임된 파트너) 모델을 통한 고객 연결


**적절한 역할:** 인센티브 관리자

2019년 10월 1일에 Microsoft는 CPOR(Claiming Partner of Record) 모델을 사용하여 OSA(온라인 서비스 권고) 판매, OSU(온라인 서비스 사용) Microsoft 365 및 OSU-Business 애플리케이션 인센티브와 관련하여 Microsoft 365 및 Dynamics 365 고객과의 관계를 관리하기 시작했습니다.

>[!Important]
> CPOR(고객 연결) 클레임은 OSA(Online Services Advisory) 판매, OSU(온라인 서비스 사용) Microsoft 365 및 OSU-Business 애플리케이션 인센티브 프로그램에만 적용됩니다. CSP(클라우드 솔루션 공급자), Managed Reseller, 호스팅 또는 Surface와 같은 다른 프로그램에 대한 공동 클레임을 제출하는 경우 여기에 설명된 공동 클레임 프로세스를 참조하세요. <br><br>클레임을 제출하면 Microsoft에서 유효성을 검사합니다. 이 시점에서 자세한 정보를 요청할 수 있습니다. 또한 고객에게 연결 요청을 알립니다. 고객은 영업일 5일 동안 옵트아웃해야 합니다. 옵트아웃하지 않으면 이 특정 테넌트 및 워크로드와의 연결이 공식이 됩니다. 이 시점에서 고객의 사용량 현황 데이터에 액세스할 수 있습니다. 

클레임을 완료하려면 다음 정보가 필요합니다.

- 클레임을 만드는 엔터티의 **MPN ID(Microsoft 파트너 네트워크** ID)

- 고객의 **도메인 이름(자세한** 내용은 [테넌트 ID 찾기, 도메인 이름, 사용자 개체 ID](find-ids-and-domain-names.md)참조)

- 고객의 **디렉터리 ID** 또는 **테넌트 ID(자세한** 내용은 [테넌트 ID 찾기, 도메인 이름, 사용자 개체 ID](find-ids-and-domain-names.md)참조)

- **솔루션** 영역(예: Business Applications 또는 Microsoft 365)

- 수행한 **활동** 및 수행하려는 클레임 유형(예: 판매 전, 사용량 또는 수익 연결)

- 고객의 연락처 **이름,** 제목 및 이메일 주소

- Dynamics 365의 경우 고객의 **기술 연락처** 이름, 직위 및 이메일 주소도 제공해야 합니다.

- 회사의 **연락처 이름** 및 이메일 주소

- 이 클레임에 대한 **이름을** 만듭니다.

- 클레임하는 **제품** 또는 워크로드

- **PoE(실행 증명)(예:** 고객이 서명한 작업 명세서) 사용할 PoE 템플릿을 다운로드할 수도 있습니다.

- 수익 연결을 클레임하는 파트너의 **경우: Dynamics 솔루션 판매자 이름,** **고객 이름** 및 **ISV 제품/솔루션의 이름입니다.** 

또한 다음 사항을 이해해야 합니다.

- 기존 Microsoft 365 고객이 있는 경우 이 프로세스를 사용하여 OSU 인센티브 획득을 계속하려는 고객과 다시 연결을 끊어야 합니다.

- Dynamics 365 또는 Power BI 고객과 기존 연결이 있는 경우 구독이 만료될 때까지 이러한 연결은 유효한 상태로 유지됩니다.

- 고객은 여러 파트너를 가질 수 있지만 각 워크로드(OSU-Microsoft 365용) 또는 구독(OSA-Sell 및 OSU-Business 애플리케이션의 경우)은 한 파트너와만 연결될 수 있습니다.

## <a name="create-a-customer-association"></a>고객 제휴 만들기

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. **인센티브** 탭을 선택하고 **개요** 를 선택한 **다음, 고객 연결을** 선택합니다.

3. 고객 연결 페이지의 맨 위에서 **+ 고객 연결** 을 선택합니다.

4. 고객과 연결할 파트너 위치의 **MPN ID** 를 선택한 다음 고객의 도메인 이름과 디렉터리 ID를 추가합니다. [다음을 찾습니다.](find-ids-and-domain-names.md)

5. **계속** 을 선택합니다.

6. 솔루션 **영역** 및 **작업 을** 선택합니다. 

   >[!Note]
   >
   >Business Applications 선택하는 경우 **사용량 및/또는 판매 전** 또는 **수익 연결** 를 선택한 **다음, 계속을** 선택합니다. 
   <br><br>수익 연결을 선택하는 경우 아래 나열된 것과 약간 다른 정보를 묻는 메시지가 표시됩니다.

7. **고객 연결** 페이지에서 적절한 정보를 입력한 다음 클레임 **만들기를** 선택합니다.

8. 이 고객 연결과 연결된 제품을 선택한 다음, **계속을** 선택합니다.

9. 고객 연락처 정보 및 회사의 연락처 정보 입력을 완료합니다. 모든 필드는 필수입니다. 

   >[!NOTE]
   >제품이 Dynamics 365이고 선택한 제품에 이 특정 고객에 대한 여러 구독이 있는 경우 구독 ID도 입력해야 합니다.

10. PoE를 입력합니다. 이를 상자로 끌거나, 고유한 지원 설명서를 찾아보거나, **템플릿 다운로드** 를 선택하여 템플릿을 사용할 수 있습니다. 

11. 원하는 경우 설명을 추가하여 저장한 다음 **클레임 제출** 을 선택합니다. 고객 연결에 대한 승인을 요청하는 고객에게 이메일이 전송됩니다.

   >[!NOTE]
   >고객 연결을 제출한 후에는 편집할 수 없습니다.

고객 연결의 상태가 **상태** 필드에 표시됩니다.

**기록** 을 선택하여 고객 연결 기록을 볼 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [고객 제휴 보기](incentives-manage-customer-associations.md)