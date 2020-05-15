---
title: 현재 Azure 제품에서 Azure 플랜으로 고객 이동
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 파트너가 파트너 센터를 사용하여 Azure 플랜에서 기존 CSP Azure 제품에서 Azure 서비스로 고객을 이동하는 방법을 알아봅니다.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 05c28b852935dbce88d9f64c86b7c87fcbdc05cc
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908329"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>기존 CSP Azure 제품에서 Azure 플랜으로 고객 전환

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 글로벌 관리자
- 기술 지원팀 상담원
- 영업 상담원
- 사용자 관리 담당자

간접 공급자와 직접 청구 파트너는 Azure용 CSP(클라우드 서비스 공급자) 프로그램에서 사용할 수 있는 새로운 상거래 환경으로 전환할 수 있습니다. (직접 재판매인은 간접 공급자를 통해 작업해야 합니다.) 고객은 파트너 또는 Microsoft 판매자에게 구입하든 아니면 웹에서 직접 구입하든, 간편하게 클라우드 서비스를 구입할 수 있습니다.

전환 기능은 Azure의 새로운 상거래 환경으로 전환하는 고객과 Microsoft 고객 계약에 서명한 고객을 위한 것이며, Office 365 또는 Dynamics 365와 같은 CSP의 다른 제품을 위한 것이 아닙니다.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>기존 CSP 제품을 Azure 플랜으로 전환

파트너 센터 내에서 고객을 기존 CSP Azure 제품에서 CSP 프로그램의 새로운 상거래 환경에서 제공하는 Azure 플랜 하의 Azure 서비스로 전환할 수 있습니다. 이렇게 하려면 파트너와 고객에게 파트너 센터를 통해 설정된 재판매인 관계가 있어야 하고, 고객은 Microsoft 고객 계약에 서명해야 합니다.

### <a name="select-transition-to-azure-plan"></a>Azure 플랜으로 전환 선택

1. 고객에게 Azure 플랜을 선택합니다.

2. **청구를 Azure 플랜으로 전환**을 선택합니다.

![전환](images/azure/transition1.png)

3. **계속**을 선택합니다.

![전환](images/azure/transition2.png)

고객이 Azure 플랜으로 전환됩니다.

**전환 워크플로는 다음과 같은 필수 조건 단계를 자동화합니다**.

- Azure 플랜 구입
- 직접 CSP 시나리오에서는 고객당 플랜 하나  
- 재판매인당 플랜 하나  

예를 들어 파트너가 Microsoft Azure 제품을 2개 구입하고 별도의 POR 2개를 구매에 포함했습니다. 이 경우 전환 워크플로에서는 Azure 플랜을 2개 구입하고(재판매인당 하나) Azure 플랜에 따라 각 Azure 구독을 자동으로 매핑합니다.  

**Azure 구독을 Azure 플랜에 매핑**

Azure 플랜을 구입한 후에는 시스템에서 기존 Azure 구독을 Azure 플랜에 매핑합니다. 진행률은 Azure Portal과 파트너 센터에서 볼 수 있습니다. 

4. 고객의 파트너 센터 **구독** 페이지로 돌아와서 고객의 예산 한도를 고객의 현지 통화로 업데이트합니다. 

![전환](images/azure/transition3.png)

>[!NOTE]
>파트너 센터에서 설정한 예산이 Azure Portal로 전달되지 않습니다. Azure Portal에서도 예산과 경고를 설정해야 합니다.

Azure 플랜으로 이동하면 더 이상 이 고객에 대한 Azure 구독을 구매할 수 없습니다. Azure Portal에서 Azure 플랜에 따라 구독을 만들어야 합니다.

>[!NOTE]
> Azure 플랜에서 RBAC를 통해 구입한 모든 Azure 구독은 현지 통화로 가격이 책정되고 요금이 청구됩니다. 환율은 사용되지 않습니다.

### <a name="track-your-transition-details"></a>전환 세부 정보 추적

Azure Portal과 파트너 센터에서 전환 단계를 수행하세요.

![세부 정보 표시](images/azure/details1.png)

**파트너에게 미치는 청구 영향**

기존 CSP Azure 제품을 사용하는 고객을 전환하면 다음과 같은 청구 영향이 있습니다.

- 원래의 CSP Azure 구독이 종료될 때까지의 모든 사용량에 대한 요금은 기존 CSP 청구서로 청구됩니다.

- 기존 CSP 구독에 대한 관리자 액세스 권한이 있는 경우 해당 구독이 마이그레이션되어도 계속 액세스할 수 있습니다.

직접 기업 계약을 CSP로 전환하고 서버 및 클라우드 등록을 Azure 서비스로 전환하려면 [Microsoft 파트너 계약에 대한 Azure 구독의 청구 소유권 얻기](https://docs.microsoft.com/azure/billing/mpa-request-ownership)를 읽어 보세요.

**감사 로그**:

청구를 조정하려면 **구독** 페이지에서 "Microsoft Azure"(0145P) 구독의 기록을 확인하세요. 

"Microsoft Azure"(0145P) 구독은 다음과 같은 두 부분으로 구성됩니다.
1. 상거래 구독 
2. Azure 구독(자격)

전환이 완료되면 Azure 구독이 새 Azure 플랜으로 이동되고 상거래 구독이 일시 중단되어 더 이상 서비스 사용이 보고되지 않습니다.  

>[참고]\: CSP에서 Microsoft Azure(0145P) 구독을 구매한 경우 상거래 구독과 Azure 구독(자격)의 가격이 동일합니다. 청구 소유권이 변경되거나 이전되는 경우에만 가격이 달라집니다. 

**전환 문제**

전환하는 동안에는 문제가 발생하지 않습니다. 만약 오류가 발생할 경우 전환 워크플로 자체에서 업데이트해 드리겠습니다. Azure 사용에 방해가 되는 일은 없을 것입니다.  

## <a name="next-steps"></a>다음 단계

- [Azure 플랜 하에서 구독 및 리소스 관리](azure-plan-manage.md)

- [파트너 획득 크레딧 - 개요](partner-earned-credit.md)



