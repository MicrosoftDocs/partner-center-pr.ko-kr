---
title: 고객을 위한 Azure 예약 관리
description: 예약을 취소하거나, 예약을 교환하거나, 환불을 요청하는 방법을 포함하여 고객에 대한 Azure 예약을 관리하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149488"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>고객 예약 관리, 취소, 교환 또는 환불 Microsoft Azure

**적절한 역할:** 관리 에이전트 | 전역 관리자 | Helpdesk 에이전트 | 영업 에이전트 | 사용자 관리 관리자

이 문서에서는 예약을 취소하거나, 예약을 교환하거나, 환불을 요청하는 방법을 포함하여 고객에 대한 Azure 예약을 관리하는 방법을 설명합니다.

> [!NOTE]
> 이 문서는 CSP(클라우드 솔루션 공급자) 프로그램의 파트너에게만 적용됩니다. 다른 유형의 구독(예: 종량제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용하는 고객은 대신 [이 Azure 예약 설명서를](/azure/cost-management-billing/reservations)읽어야 합니다.

구매 후 고객의 Azure 예약을 관리하려면 파트너 센터 관리할 고객 및 예약을 선택한 다음, Azure Portal 예약을 변경합니다.

1. 시작하려면 파트너 센터 메뉴에서 **고객을** 선택한 다음, 예약을 관리할 고객을 선택합니다. 

2. 고객의 세부 정보 페이지 메뉴에서 **Azure 예약을** 선택한 다음, 관리하려는 특정 예약을 선택합니다.  

3. **작업에서** **관리를** 선택하여 Azure Portal 고객의 예약 레코드로 이동합니다. 예약 세부 정보 페이지에서 아래 단계에 따라 작업을 완료합니다.  

    | **Select**   | **수행할 작업**    |
    |:-----------------------------|:-----------------|
    | **개요**   | 만료 날짜, 범위 및 사용률 데이터를 포함하여 고객의 예약 세부 정보를 봅니다. **참고** **환불을** 선택하여 비례 배분 환불에 대한 지원 요청을 만듭니다. **Exchange를** 선택하여 예약 기간의 사용되지 않는 부분을 교환하는 지원 요청을 만듭니다.  
    | **Access Control(IAM)**   | 고객의 예약 정보에 대한 액세스를 관리합니다.|
    | **Configuration**   | 예약의 범위 및/또는 예약이 연결된 Azure 구독을 변경합니다.    |
    | **속성**   | 예약의 속성을 보고 예약 ID 및 예약 주문 ID를 클립보드로 복사 합니다. **참고** 고객을 대신 하 여 지원을 요청할 때 지원에서 예약 ID 및 예약 주문 ID를 요청할 수 있습니다.    |
    | **새 지원 요청**    | Microsoft 지원에서 도움을 요청 합니다.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>예약 취소 또는 교환

언제 든 지 고객의 비즈니스 요구 사항이 변경 되 면 예약을 취소 하 고 환불을 받을 수 있으며 새 예약 가격에 사용 될 예약의 비례 상환 금액을 교환할 수 있습니다.

이러한 두 시나리오에서 Microsoft는 고객에 게 환불 된 재무 거래를 관리할 수 있도록 용량을 자동으로 계산 합니다. Microsoft는 대금 청구, 취소 또는 환불에 대해 직접 고객에 게 연락 하지 않습니다.

### <a name="how-cancellations-work"></a>취소 작업 방법

고객은 언제 든 지 예약을 취소 하도록 요청할 수 있습니다 (환불 금액은 연간 $5만). 예약을 취소 하면 고객이 조기 종료 요금으로 Azure 예약의 남은 개월 수를 반환할 수 있습니다. 초기 종료 수수료를 제외 하 고 남은 비례 잔액은 사용자 계정에 환불 고객의 계정을 환불 받을 수 있습니다. 

취소 세부 정보 및 수수료는 아래를 참조 하세요.


|**취소 날짜**<br> 일별로   |**사용 현황**    |**크레딧**  |**조기 종료**<br> 수수료    |**환불 캡** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 개 미만                         | 예          | 100%       | 예                              | $5만 USD   |
|5 개 미만                         | 예         | 전문 등급  | 예                              | $5만 USD   |
|5 개 이상                        | 예          | 전문 등급  | 12%                             | $5만 USD   |
|5 개 이상                        | 예         | 전문 등급  | 12%                             | $5만 USD   |

### <a name="how-exchanges-work"></a>교환 작동 방법 

고객이 원래 구매한 사용자와 다른 예약을 구입 하려는 경우 exchange를 요청할 수 있습니다. 예약을 교환 하면 고객이 새 예약 가격에 비례하여 비례 하는 환불 금액을 사용할 수 있으므로 예약을 취소 하는 것이 좋은 대안이 될 수 있습니다. 

고객에 게 exchange를 제공할 수 있도록 비례 하는 환불 금액은 계정에 제공한 됩니다.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>고객을 대신 하 여 환불 또는 교환 요청

고객을 대신 하 여 환불 또는 교환에 대 한 지원 요청을 파일 하려면 파트너 센터에서 고객 및 예약을 선택한 후 Azure Portal에서 지원 요청을 만듭니다. 

>[!NOTE]
>Microsoft 지원 에이전트에서 예약 ID 및 예약 주문 ID를 제공 하도록 요청할 수 있습니다. 이 정보는 Azure Portal의 예약 **속성** 페이지에서 찾을 수 있습니다.

1. 시작 하려면 파트너 센터 메뉴에서 **고객** 을 선택한 다음 환불 하려는 고객을 선택 합니다. 

2. 고객의 세부 정보 페이지에서 **Azure 예약** 을 선택한 후 고객이 환불 하려는 특정 예약을 선택 합니다.  

3. **작업** 에서 **환불** 을 선택 하 여 Azure Portal에서 고객의 예약 레코드로 이동 하 고 지원 요청을 시작 합니다.  

4. **새 지원 요청** 페이지에서 아래 단계를 수행 하 여 환불을 요청 합니다. 각 단계 후에 **다음을** 선택합니다. 

   |**Step**                    |**선택**    |
   |:---------------------------|:-----------------|
   |**1가지 기본 사항**                |문제 유형: 청구.  |
   |**2 문제**               |문제 유형: 예약 관리. 범주: 교환 및 환불. |
   |**3 연락처 정보**   |기본 설정을 선택하고 필요한 정보를 입력합니다. 

5. 완료되면 **만들기** 를 선택합니다.

## <a name="azure-reservations-resources"></a>Azure 예약 리소스

|**원하는 정보**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
|CSP의 Azure 예약 개요  | [Microsoft Azure 예약 인스턴스 판매](azure-reservations.md) |
|파트너 센터 고객에 대한 Azure 예약 구매   | [Azure 예약 구입](azure-reservations-buying.md) |
|올바른 VM 크기 확인 및 고객 VM 사용량 확인   | [최대 Azure 예약 사용량에 대한 VM 크기 조정](azure-usage.md)   |
|파트너 센터 API를 사용하여 Azure 예약 구매 | [파트너 센터](/partner-center/develop/purchase-azure-reservations) 개발자 설명서의 구매 Azure Reserved VM Instances   |
|고객이 구매한 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에게 부여합니다. | [고객에게 자신의 Azure 예약을 구매할 수 있는 권한 부여](give-customers-permission.md)   |