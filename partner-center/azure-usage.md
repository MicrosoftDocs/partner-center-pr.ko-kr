---
title: 최대 예약 사용에 대 한 Microsoft Azure VM 크기 조정 | 파트너 센터
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: VM에 대 한 Microsoft Azure 예약을 구매할 때 고객의 컴퓨팅 요구에 따라 VM (가상 머신)의 크기를 조정 하는 방법을 알아봅니다.
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

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>고객의 Azure 예약에 대 한 VM 크기 결정 

고객을 대신 하 여 Microsoft Azure 예약을 구입 하는 경우 고객의 컴퓨팅 요구에 맞게 VM (가상 머신) 크기를 선택 해야 합니다. 다음 방법 중 하나를 사용하여 이 정보를 찾을 수 있습니다.

- Azure 사용률 API
- Azure Portal
- Azure PowerShell
- Azure Resource Manager(ARM) API

이러한 각 방법의 사용 지침은 아래와 같습니다. 예약을 구입하고 나면 예약의 속성 및 수량과 일치하는 가상 컴퓨터에 예약 할인이 자동으로 적용됩니다. VM에 예약을 할당할 필요가 없습니다.

>[!NOTE]
>클래식 또는 프로 모션 Vm에는 예약 할인이 적용 되지 않습니다.

>[!IMPORTANT]
>고객을 대신하여 구입하기 위해 VM의 유형 및 크기를 올바르게 파악하려면 VM 시리즈 유형이 파트너 센터 조정 파일에 올바르게 표시되지 않을 때 아래에 설명된 방법 중 하나를 사용해야 합니다.

**Azure 사용률 API를 사용 하 여 VM 크기 정보 가져오기**

1. API 응답 시 additionalInfo에서 ServiceType 속성의 값을 사용하여 구입할 VM 크기를 식별합니다.
2. 자세한 내용은 [파트너 센터 API](https://docs.microsoft.com/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.

**Microsoft Azure portal를 사용 하 여 VM 크기 정보 가져오기**

1. 파트너 센터에서 **고객** 페이지로 이동 합니다.
2. Azure VM 예약을 구입 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다. **Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.
3. 포털 메뉴에서 **가상 컴퓨터**를 선택한 다음, 예약을 구입하고 싶은 VM을 선택합니다.
4. VM의 세부 정보 페이지에서 아래 그림과 같이 크기 및 지역 정보를 확인 하 고이 정보를 사용 하 여 파트너 센터에서 예약을 구매 합니다.  

    ![세부 정보 페이지의 크기 및 지역 정보](images/usage1.png)

**Microsoft Azure PowerShell를 사용 하 여 VM 크기 정보 가져오기**

아래 이미지에서 이 정보를 사용하여 예약을 구입하고 싶은 VM의 크기와 위치를 파악합니다. 

![VM 위치 및 크기](images/usage2.png)

**ARM (Azure Resource Manager) API를 사용 하 여 VM 크기 정보 가져오기**

1. ARMClient 또는 ARM API를 이용해 예약을 구입하고 싶은 VM에 대한 ARM 클라이언트를 호출합니다.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 호출을 하면 아래 그림에서와 같이 **vmSize** 및 **location**에 대한 값이 반환됩니다.

    ![vmSize 값](images/usage3.png) ![위치 값](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM 사용량 및 예약 할인 확인

고객을 대신 하 여 Azure 예약 VM 인스턴스를 구매한 후에는 VM 공간에 대 한 요금 지불 할인이 고객 예약의 특성 및 수량과 일치 하는 가상 머신에 자동으로 적용 됩니다.

다음 방법 중 하나를 사용 하 여 고객의 예약 사용량을 확인 하 고 예약 할인이 적용 되는 가상 컴퓨터를 확인할 수 있습니다.

- Azure Portal
- Azure 사용률 API

이러한 각 방법의 사용 지침은 아래와 같습니다.

>[!NOTE]
>Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Microsoft Azure portal에서 고객의 예약 사용 현황을 확인 합니다.

1. 파트너 센터에서 **고객** 페이지로 이동 합니다.

2. 예약 할인 및 사용량을 확인 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다. **Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.
3. 포털 메뉴에서 **예약**을 선택한 다음, 사용량을 확인하고 싶은 예약을 선택합니다.
4. **개요** 페이지에서 가상 컴퓨터에 적용 된 예약의 양을 보여 주는 예약 사용률 그래프를 확인 합니다.

    >[!NOTE]
    >사용률 데이터는 최대 8시간까지 지연될 수 있습니다.

    a. 예약의 사용률이 100% 인 경우 고객은 예약 구매가 제공할 수 있는 모든 절감 액을 얻을 수 있습니다.
    b. 예약의 사용량이 0% 이면 모든 가상 머신에 할인이 적용 되지 않습니다.
    c. 예약의 사용량이 1%에서 99% 사이인 경우 사용 하지 않는 이점이 있습니다.

5. 이러한 상황을 방지 하려면 구매를 수행 하기 전에 고객의 컴퓨팅 요구를 지원 하도록 올바른 크기의 VM을 결정 합니다.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Azure 사용량 API를 사용 하 여 고객의 예약 사용 확인

>[!NOTE]
>Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.  

Azure 활용률 API를 통해 예약 사용량 데이터를 얻어서 고객이 예약 할인을 받고 있는지 확인하고 할인이 적용되는 가상 컴퓨터(VM)를 확인할 수 있습니다. 예 A를 예 2와 비교 하 여 고객의 예약 사용량을 확인 하는 방법을 확인 합니다.

![예약 사용 예](images/usage5.png)

- reservationId는 VM에 할인을 적용하는 데 사용된 Azure 예약을 식별합니다.
- consumptionMeter는 예약 할인이 적용되는 VM의 MeterId입니다.
- 예약 할인이 적용되었기 때문에 ReservationMeter는 0달러로 표시됩니다.

자세한 내용은 [파트너 센터 API](https://docs.microsoft.com/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.

>[!IMPORTANT]
>Microsoft Windows Server 등의 소프트웨어 비용은 현재 VM 예약 가격에 포함되어 있지 않으며, 주문 기록 및 송장에 개별 품목으로 표시됩니다. 그러나 고객이 Azure 하이브리드 사용 혜택을 이용하고 있는 경우에는 소프트웨어 비용이 적용되지 않습니다. 자세한 내용은 [예약 인스턴스에 포함되어 있지 않은 Windows 소프트웨어 비용](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)을 참조하세요.  

## <a name="azure-reservations-resources"></a>Azure 예약 리소스

|**에 대 한 자세한 내용**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
|CSP의 Azure 예약 개요  | [Microsoft Azure 예약 VM 인스턴스 판매](azure-reservations.md)
|파트너 센터에서 고객에 대 한 Azure 예약 구매   |[Azure 예약 구입](azure-reservations-buying.md)
|파트너 센터에서 Azure 예약 관리 | [파트너 센터에서 Azure 예약 관리](azure-reservations-manage.md)
|Azure Portal에서 Azure 예약 구입 | Azure 도움말의 [Azure Reserved VM Instances에서 가상 컴퓨터에 대한 사전 지불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)을 참조하세요. |
|Azure Portal에서 Azure 예약 관리   |Azure 도움말의 [예약된 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)를 참조하세요.  |
|파트너 센터 API를 사용하여 Azure 예약 구입 | 파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.
