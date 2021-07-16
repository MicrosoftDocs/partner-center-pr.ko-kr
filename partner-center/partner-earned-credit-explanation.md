---
title: 관리형 서비스에 대한 파트너 획득 크레딧
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 관리형 서비스에 대해 Microsoft PEC(파트너 획득 크레딧)를 계산하고 지불하는 방법과 자격을 갖추는 방법에 대해 알아봅니다.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145867"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>파트너 획득 크레딧을 계산 및 지불하는 방법

**적절한 역할**: 전역 관리자 | 사용자 관리 관리자 | 관리자 에이전트 | 청구 관리자 | 영업 에이전트

관리형 서비스에 대한 PEC(파트너 획득 크레딧)는 고객의 Azure 환경 일부 또는 전체에 대한 연중무휴 IT 운영 제어 및 관리를 담당하는 파트너를 알아내서 보상하는 제도입니다. 기본적으로 CSP에서는 파트너가 연중무휴 운영을 관리하고 구독의 리소스를 제어할 수 있도록 파트너에게 고객의 구독에 대한 필수 액세스 권한을 부여합니다. 고객이 거래 파트너에 대한 액세스를 프로비저닝하는 다른 방법은 다음 섹션에 설명되어 있습니다. 월별 청구서 금액은 순 파트너 획득 크레딧입니다. 파트너는 월별 조정 파일에서 PEC 세부 정보를 볼 수 있습니다. 고객이 거래 파트너에 대한 액세스를 프로비저닝하는 추가적인 방법은 [Azure 플랜에서 구독 및 리소스 관리](azure-plan-manage.md)를 참조하세요.

또한 [Azure CSP 구독에 대한 관리자 권한 복구](revoke-reinstate-csp.md)도 참조하세요.

## <a name="eligibility"></a>자격

PEC(파트너 획득 크레딧)를 받으려면 다음 요구 사항이 적용됩니다. 

- 관리하는 Azure 자산에 대해 획득되는 크레딧을 받으려면 활성 MPN 계약 및 유효한 RBAC(역할 기반 액세스 제어) 역할이 있어야 합니다.

- CSP에서 고객의 Azure 리소스 운영을 연중무휴로 제어하고 관리해야 합니다. 즉, 고객의 Azure 구독, Azure 리소스 그룹, Azure 리소스에 대한 관리자 권한이 있어야 합니다. 간접 공급자 및 해당 간접 재판매인의 경우 둘 중 하나 또는 둘 모두에 이 운영에 대한 제어 권한이 있으면 간접 공급자에게 PEC를 받을 자격이 있습니다. 이에 대한 자세한 내용은 [Azure CSP 구독에 대한 관리자 권한 복구](./revoke-reinstate-csp.md)를 참조하세요.

- 위의 요구 사항 외에도, PEC는 [Azure 플랜 가격 책정](https://partner.microsoft.com/commerce/sales) 페이지에서 내보낼 수 있는 Azure 플랜 사용량 가격 책정에 나열된 서비스에만 적용됩니다.

- PEC가 적용되지 **않는** 서비스는 다음과 같습니다.
    - Azure 플랜 예약
    - Azure 플랜 사용량 가격의 [태그] 열에서 [타사]로 식별된 타사 제품
    - Marketplace 가격 목록의 제품
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC는 Azure 리소스 수준에서 획득됩니다. 구독 또는 리소스 그룹 수준에서 유효한 액세스 권한이 있는 경우 더 높은 엔터티로 롤업되는 각 리소스에서 PEC를 획득합니다.

- PEC에 대한 자세한 내용은 [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) 페이지에서도 확인할 수 있습니다.

### <a name="calculation"></a>계산

PEC는 매일 계산되며 일별 사용량 파일 및 월별 청구서 조정 파일에서 볼 수 있습니다. 파트너(간접 공급자 또는 간접 재판매인)에게는 전체 기간 동안(연중무휴) PEC를 획득할 수 있는 액세스 권한이 있어야 합니다. PEC는 관리되는 Azure 자산을 기준으로 매일 계산됩니다. 해당 월(액세스 범위) 및 모든 적격 리소스(액세스 범위)에 대해 권한 있는 영구 액세스를 유지하는 파트너는 전체 PEC를 획득합니다. 범위 및 범위 축소로 인해 해당 월의 PEC 비율이 낮아집니다. Azure 자산에 대한 일일 정격 사용량 파일은 PEC 적용 여부에 관계없이 매일 표시됩니다. 파트너는 경고에 등록하여 권한 있는 영구 액세스에 대한 변경 내용을 모니터링할 수도 있습니다.

## <a name="azure-cost-management"></a>Azure Cost Management

비용 분석을 사용하는 ACM(Azure Cost Management)을 통해 파트너는 PEC의 혜택을 받은 비용을 확인할 수 있습니다.  

1. [Azure Portal](https://portal.azure.com)에서 파트너 테넌트에 로그인하고, **Cost Management + 청구** 를 선택합니다.

2. **Cost Management** 를 선택합니다.

3. **비용 분석** 을 선택합니다.

   비용 분석 보기에는 Microsoft에 지불하는 가격으로 구입하고 사용하는 모든 서비스에 대한 청구 계정 비용이 표시됩니다.

4. 피벗 차트의 드롭다운 목록에서 **PartnerEarnedCreditApplied** 를 선택하여 PEC가 적용된 비용을 확인합니다. **PartnerEarnedCreditApplied** 속성이 True이면 관련 비용에는 파트너 획득 크레딧의 혜택이 적용됩니다. 

   PartnerEarnedCreditApplied 속성이 False이면 관련 비용이 필요한 크레딧 자격을 충족하지 못하거나 구입한 서비스가 파트너 획득 크레딧에 적합하지 않습니다.

   >[!NOTE] 
   >일반적으로 서비스 사용량은 **Cost Management** 에 표시되는 데 8-24시간이 걸리고, PEC 크레딧은 Azure Cost Management에 액세스한 이후 48시간 내에 표시됩니다.

5. **Group by 및 Add** 필터 기능을 사용하여 **PartnerEarnedCreditApplied** 속성을 기준으로 그룹화하고 필터링하여 PEC가 적용된 비용과 PEC가 적용되지 않은 비용을 자세히 살펴볼 수도 있습니다.

## <a name="next-steps"></a>다음 단계

- [파트너 획득 크레딧 - 개요](partner-earned-credit.md)

- 파트너 획득 크레딧 계산의 자세한 예는 파트너 센터 대시보드(로그인 필요)를 통해 확인할 수 있는 가격표에 있습니다.

- [Azure 플랜으로 이동 - 시작](azure-plan-get-started.md)

- [Azure 플랜 하에서 구독 및 리소스 관리](azure-plan-manage.md)

- [Azure CSP 구독에 대한 관리자 권한 철회 또는 복구](revoke-reinstate-csp.md)
