---
title: 고객을 대신하여 Azure 예약 구입 | 파트너 센터
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to manage Azure reservations on behalf of a customer, including how to cancel a reservation, exchange a reservation, or request a refund.
author: LauraBrenner
ms.author: labrenne
keywords: azure, reservations, manage, billing, buying, cancel, exchange, early termination fee
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b71457f0bd75008db9ed704784a39b082983501d
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252635"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>고객을 대신하여 Microsoft Azure Reservations 관리       

**적용 대상**

-  파트너 센터
-  Microsoft Azure portal 
-  CSP 파트너

To manage your customers' Azure reservations post-purchase, you'll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal. 

1. To get started, select **Customers** from the Partner Center menu and then select the customer whose reservations you want to manage. 

2. On the customer's detail page menu, select **Azure reservations** and then select the specific reservation you want to manage.  

3. Under **Actions**, select **Manage** to go to the customer's reservation record in the Azure portal. 예약 세부 정보 페이지에서 작업을 완료 하려면 다음 단계를 수행합니다.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **개요**   | View details of a customer's reservation, including expiration date, scope, and utilization data. **참고** **환불**을 선택하여 비례 배분 방식 환불을 위한 지원 요청을 만듭니다. **교환**을 선택하여 예약 기간 중 미사용 부분을 교환하기 위한 지원 요청을 만듭니다.  
    | **Access Control (IAM)**   | Manage access to the customer's reservation information.|
    | **구성**   | Change the reservation's scope and/or the Azure subscription the reservation is associated with.    |
    | **속성**   | View the reservation's properties and copy to the clipboard the reservation ID and reservation order ID. **참고** 고객을 대신하여 지원을 요청하면 지원 팀에서 예약 ID 및 예약 주문 ID를 물어볼 것입니다.    |
    | **New support request**    | Microsoft 지원 팀에 도움을 요청합니다.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>예약 취소 또는 교환 

If at any point a customer's business needs change, they may want to cancel a reservation and get a refund or exchange a reservation's prorated refund amount to be used toward the price of a new reservation.

In both of these scenarios, Microsoft refunds the amount to you so that you can then manage the resulting financial transactions with your customers. Microsoft does not contact customers directly about billing, cancellations, or refunds.   
 

**How cancellations work**

Customers can request to cancel a reservation at any time (refund amount capped at $50,000 per year). Cancelling a reservation allows the customer to return the amount of the remaining months of an Azure reservation for an early termination fee. The remaining prorated balance, minus the early termination fee, is refunded to your account so that you can refund the customer's account. 

See below for cancellation details and fees.


|**Cancellation date**<br> (days)   |**Usage**    |**Credit**  |**Early termination**<br> 요금    |**Refund cap** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 or fewer                         | 아니요          | 100%       | 아니요                              | $50,000 USD   |
|5 or fewer                         | 예         | Pro-rated  | 아니요                              | $50,000 USD   |
|More than 5                        | 아니요          | Pro-rated  | 12%                             | $50,000 USD   |
|More than 5                        | 예         | Pro-rated  | 12%                             | $50,000 USD   |


**How exchanges work** 

If a customer wants to buy a different reservation than the one they originally bought from you, they can request an exchange. Exchanging a reservation can be an attractive alternative to cancelling a reservation because it allows the customer to use the prorated refund amount toward the price of the new reservation. 

The prorated refund amount is credited to your account so that you can offer the customer an exchange.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>고객을 대신하여 환불 또는 교환 요청 

To file a support request for a refund or exchange on behalf of your customers, you'll select the customer and reservation in Partner Center, and then create the support request in the Azure portal. 

>[!NOTE]
>Microsoft 지원 상담원이 예약 ID와 예약 주문 ID를 물어볼 수 있습니다. You can find this information on the reservation's **Properties** page in the Azure portal. 

1. To get started, select **Customers** from the Partner Center menu and then select the customer who wants a refund. 

2. On the customer's detail page, select **Azure reservations** and then select the specific reservation the customer wants refunded.  

3. Under **Actions**, select **Refund** to go to the customer's reservation record in the Azure portal and initiate a support request.  

4. **새 지원 요청** 페이지에서 다음 단계에 따라 환불을 요청합니다. 각 단계를 수행한 후 **다음**을 선택합니다. 

    |**Step**                    |**Selections**    |
    |:---------------------------|:-----------------|
    |**1 Basics**                |발행 유형: 청구  |
    |**2 Problem**               |문제 유형: 예약 관리 범주: 교환 및 환불 |
    |**3 Contact information**   |기본 설정을 선택하고 필요한 정보를 입력합니다. 

5.  입력을 마쳤으면 **생성**을 선택합니다.

## <a name="azure-reservations-resources"></a>Azure 예약 리소스
|**For information about**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
|CSP의 Azure 예약 개요  | [Sell Microsoft Azure Reserved Instances](azure-reservations.md) |
|Purchasing Azure reservations for your customers in Partner Center   |[Buy Azure reservations](azure-reservations-buying.md) |
|올바른 VM 크기를 확인하고 고객 VM 사용량 확인   |[VM sizing for maximum Azure reservation usage](azure-usage.md)   |
|파트너 센터 API를 사용하여 Azure 예약 구입 | 파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.

