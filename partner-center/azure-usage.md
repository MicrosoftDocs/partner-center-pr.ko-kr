---
title: Microsoft Azure VM sizing for maximum reservation usage  | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.
author: LauraBrenner
ms.author: labrenne
keywords: azure, 예약, vm, 관리, 사용량, 크기 조정
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2b8148d66be8a439056efa41eccb60cbc3e4274b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253252"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>최대 예약 사용량에 맞게 Microsoft Azure VM 크기 조정

**적용 대상**

- 파트너 센터
- Azure Portal
- CSP 파트너

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determine the VM size for a customer's Azure reservation 

When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs. 다음 방법 중 하나를 사용하여 이 정보를 찾을 수 있습니다.

- Azure 사용률 API
- Azure Portal
- Azure PowerShell
- Azure Resource Manager(ARM) API

이러한 각 방법의 사용 지침은 아래와 같습니다. 예약을 구입하고 나면 예약의 속성 및 수량과 일치하는 가상 컴퓨터에 예약 할인이 자동으로 적용됩니다. You don't need to assign the reservation to a VM.

>[!NOTE]
>Reservation discounts don't apply to classic or promotional VMs.

>[!IMPORTANT]
>고객을 대신하여 구입하기 위해 VM의 유형 및 크기를 올바르게 파악하려면 VM 시리즈 유형이 파트너 센터 조정 파일에 올바르게 표시되지 않을 때 아래에 설명된 방법 중 하나를 사용해야 합니다.

**Get VM sizing information using the Azure utilization API**

1. API 응답 시 additionalInfo에서 ServiceType 속성의 값을 사용하여 구입할 VM 크기를 식별합니다.
2. For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

**Get VM sizing information using the Microsoft Azure portal**

1. In Partner Center, go to your **Customers** page.
2. Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. 포털 메뉴에서 **가상 컴퓨터**를 선택한 다음, 예약을 구입하고 싶은 VM을 선택합니다.
4. On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.  

    ![Size and region information on detail page](images/usage1.png)

**Get VM sizing information using Microsoft Azure PowerShell**

아래 이미지에서 이 정보를 사용하여 예약을 구입하고 싶은 VM의 크기와 위치를 파악합니다. 

![VM location and size](images/usage2.png)

**Get VM sizing information using the Azure Resource Manager (ARM) API**

1. ARMClient 또는 ARM API를 이용해 예약을 구입하고 싶은 VM에 대한 ARM 클라이언트를 호출합니다.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 호출을 하면 아래 그림에서와 같이 **vmSize** 및 **location**에 대한 값이 반환됩니다.

    ![vmSize value](images/usage3.png) ![location value](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM 사용량 및 예약 할인 확인

After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.

You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:

- Azure Portal
- Azure 사용률 API

이러한 각 방법의 사용 지침은 아래와 같습니다.

>[!NOTE]
>Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verify the customer's reservation usage in the Microsoft Azure portal

1. In Partner Center, go to your **Customers** page.

2. Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. 포털 메뉴에서 **예약**을 선택한 다음, 사용량을 확인하고 싶은 예약을 선택합니다.
4. On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.

    >[!NOTE]
    >사용률 데이터는 최대 8시간까지 지연될 수 있습니다.

    a. If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.
    b. If the reservation's usage is 0%, the discount is not being applied to any virtual machine.
    c. If the reservation's usage is between 1% and 99%, there are unused benefits.

5. To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verify the customer's reservation usage with the Azure utilization API

>[!NOTE]
>Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.  

Azure 활용률 API를 통해 예약 사용량 데이터를 얻어서 고객이 예약 할인을 받고 있는지 확인하고 할인이 적용되는 가상 컴퓨터(VM)를 확인할 수 있습니다. Compare Example A to Example B to see how to verify a customer's reservation usage.

![Reservation usage examples](images/usage5.png)

- reservationId는 VM에 할인을 적용하는 데 사용된 Azure 예약을 식별합니다.
- consumptionMeter는 예약 할인이 적용되는 VM의 MeterId입니다.
- 예약 할인이 적용되었기 때문에 ReservationMeter는 0달러로 표시됩니다.

For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Microsoft Windows Server 등의 소프트웨어 비용은 현재 VM 예약 가격에 포함되어 있지 않으며, 주문 기록 및 송장에 개별 품목으로 표시됩니다. 그러나 고객이 Azure 하이브리드 사용 혜택을 이용하고 있는 경우에는 소프트웨어 비용이 적용되지 않습니다. 자세한 내용은 [예약 인스턴스에 포함되어 있지 않은 Windows 소프트웨어 비용](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)을 참조하세요.  

## <a name="azure-reservations-resources"></a>Azure 예약 리소스

|**For information about**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
|CSP의 Azure 예약 개요  | [Sell Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Purchasing Azure reservations for your customers in Partner Center   |[Buy Azure reservations](azure-reservations-buying.md)
|Managing Azure reservations in Partner Center | [Managing Azure reservations in Partner Center](azure-reservations-manage.md)
|Azure Portal에서 Azure 예약 구입 | Azure 도움말의 [Azure Reserved VM Instances에서 가상 컴퓨터에 대한 사전 지불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)을 참조하세요. |
|Azure Portal에서 Azure 예약 관리   |Azure 도움말의 [예약된 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)를 참조하세요.  |
|파트너 센터 API를 사용하여 Azure 예약 구입 | 파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.
