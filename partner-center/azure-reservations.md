---
title: 고객 Microsoft Azure 예약 판매
description: 클라우드 솔루션 공급자는 고객에 대 한 Azure 예약을 구입, 판매 또는 관리할 수 있습니다. 파트너 센터, Azure Portal 또는 파트너 센터 API를 사용 합니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000237"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a>파트너 센터, Azure Portal 또는 Api를 사용 하 여 고객에 게 Microsoft Azure 예약 판매

**적용 대상**

- 파트너 센터
- Microsoft Azure Portal
- CSP 프로그램의 파트너

**적절한 역할**

- 관리 에이전트
- 글로벌 관리자
- 기술 지원팀 상담원
- 영업 상담원
- 사용자 관리 담당자

> [!NOTE]
> 이 문서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너에만 적용 됩니다. 다른 유형의 구독 (예: 종 량 제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용 하는 고객은 [이 Azure 예약 설명서](/azure/cost-management-billing/reservations)를 대신 읽어야 합니다.

CSP 프로그램의 파트너는 고객에 게 Microsoft Azure 예약을 제공할 수 있습니다. 고객은 사전에 대비 하 여 상당한 비용을 절감할 수 있습니다. Azure 예약은 다음과 같은 방식으로 고객의 단순성 및 유연성을 제공 합니다.

- 1 년 또는 3 년 예약 용어
- 쉽게 시작할 수 있습니다. 설치가 완료 된 시간 (초)
- 조정 된 환불을 위해 언제 든 지 예약 된 인스턴스 취소 또는 교환
- 조직 또는 개별 부서 수준에서 예약 인스턴스 사용을 관리 합니다.

Azure 예약은 다음과 같은 방식으로 고객에 게 더욱 매력적인 효과를 가질 수 있습니다.

- 예약은 PAYG (종 량 제) 가격에 비해 상당한 절감 효과를 제공할 수 있습니다.
- 1 년 또는 3 년 조건에 대 한 선불 결제로 더 나은 예산 및 예측
- 사무실에 가장 가까운 Azure 지역에서 우선 순위가 지정 된 컴퓨팅 용량
- Azure 예약은 Microsoft Windows Server 및 Azure SQL Database와 같은 소프트웨어와 함께 사용할 경우 종단 간 인프라 솔루션에 대 한 기초를 제공 합니다.

>[!NOTE]
> 파트너 센터와 Azure Portal 파트너 센터 API를 사용 하 여 Azure 예약을 구입, 판매 및 관리할 수 있습니다. 구매한 Azure 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공할 수도 있습니다. 방법에 대 한 자세한 내용은 아래 링크를 참조 하세요.

## <a name="azure-reservations-resources"></a>Azure 예약 리소스

|**원하는 정보**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
| 고객을 위한 Azure 예약 설명서 | [Azure 예약은 무엇인가요?](/azure/billing/billing-save-compute-costs-reservations)
|파트너 센터에서 고객에 대 한 Azure 예약 구매   |[Azure 예약 구입](azure-reservations-buying.md)
|파트너 센터에서 Azure 예약 관리 | [파트너 센터에서 Azure 예약 관리](azure-reservations-manage.md)
|올바른 VM 크기 확인 및 고객 VM 사용 확인   |[최대 Azure 예약 사용에 대 한 VM 크기 조정](azure-usage.md)   |
|파트너 센터 API를 사용 하 여 Azure 예약 구매 | 파트너 센터 개발자 설명서에서 [Azure Reserved VM Instances 구매](/partner-center/develop/purchase-azure-reservations)   |
|CSP 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공 합니다. | [고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여](give-customers-permission.md)   |