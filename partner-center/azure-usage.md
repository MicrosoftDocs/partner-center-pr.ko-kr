---
title: 최대 예약 사용량에 맞게 Azure VM 크기 조정
description: Microsoft Azure 예약을 구매할 때 고객의 컴퓨팅 요구 사항에 맞게 VM(가상 머신)의 크기를 정하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510196"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>최대 예약 사용에 대한 Microsoft Azure VM 크기 조정

**적절한 역할:** 관리 에이전트 | 판매 에이전트

이 문서에서는 고객의 컴퓨팅 요구 사항에 맞게 VM(가상 머신)의 크기를 Microsoft Azure 예약을 구매하는 방법을 설명합니다.
 
> [!NOTE]
> 이 문서는 CSP(클라우드 솔루션 공급자) 프로그램의 파트너에게만 적용됩니다. 다른 유형의 구독(예: 종량제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용하는 고객은 대신 이 Azure [예약 설명서를](/azure/cost-management-billing/reservations)읽어야 합니다.

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>고객의 Azure 예약에 대한 VM 크기 결정

고객을 대신하여 Microsoft Azure 예약을 구입하는 경우 고객의 컴퓨팅 요구 사항에 맞게 크기가 인 VM(가상 머신)을 선택해야 합니다. 다음 방법 중 하나를 사용하여 이 정보를 찾을 수 있습니다.

- Azure 사용률 API
- Azure 포털
- Azure PowerShell
- Azure Resource Manager(ARM) API

이러한 각 메서드를 사용하기 위한 지침은 다음과 같습니다. 예약을 구매하면 예약 할인이 예약의 특성 및 수량과 일치하는 가상 머신에 자동으로 적용됩니다. VM에 예약을 할당할 필요가 없습니다.

>[!NOTE]
>예약 할인은 클래식 또는 프로모션 VM에는 적용되지 않습니다.

>[!IMPORTANT]
>고객을 대신하여 구매할 VM의 유형과 크기를 올바르게 식별하려면 아래에 설명된 방법 중 하나를 사용해야 합니다. VM 시리즈 형식이 파트너 센터 조정 파일에 올바르게 표시되지 않기 때문에 이 방법 중 하나를 사용해야 합니다.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Azure 사용률 API를 사용하여 VM 크기 조정 정보 얻기

1. API 응답에서 additionalInfo의 ServiceType 특성 값을 사용하여 구입할 VM 크기를 식별합니다.

2. 자세한 내용은 [파트너 센터 API에서](/partner-center/develop/) [Azure에 대한 고객의 사용률 레코드 얻기를 참조하세요.](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Microsoft Azure 포털을 사용하여 VM 크기 조정 정보 얻기

1. 파트너 센터 **고객** 페이지로 이동합니다.

2. Azure VM 예약을 구입하려는 고객을 찾은 다음, 아래쪽 화살표를 선택하여 고객의 정보를 확장합니다. **Microsoft Azure 관리 포털** 선택하여 Azure Portal 고객의 레코드를 엽니다.

3. 포털 메뉴에서 **가상 머신을** 선택한 다음 예약을 구매할 VM을 선택합니다.

4. VM의 세부 정보 페이지에서 아래 그림과 같이 크기 및 지역 정보를 찾고 이 정보를 사용하여 파트너 센터 예약을 구매합니다.  

   :::image type="content" source="images/usage1.png" alt-text="세부 정보 페이지의 크기 및 지역 정보입니다.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Microsoft Azure PowerShell 사용하여 VM 크기 조정 정보 얻기

아래 이미지의 정보를 사용하여 예약을 구매할 VM의 위치와 크기를 확인할 수 있습니다. 

:::image type="content" source="images/usage2.png" alt-text="VM 위치 및 크기.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>ARM(Azure Resource Manager) API를 사용하여 VM 크기 조정 정보 얻기

1. ARMClient 또는 ARM API를 사용하여 예약을 구입하려는 VM에 대해 ARM 클라이언트를 호출합니다.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. 호출은 아래 그림과 같이 **vmSize** 및 **위치** 에 대한 값을 반환합니다.

    :::image type="content" source="images/usage3.png" alt-text="vmSize 값입니다.":::
    :::image type="content" source="images/usage4.png" alt-text="위치 값입니다.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM 사용량 및 예약 할인 확인

고객을 대신하여 Azure Reserved VM Instance를 구매한 후에는 고객의 예약 특성 및 수량과 일치하는 가상 머신에 미리 VM 공간 요금을 지불하는 할인이 자동으로 적용됩니다.

다음 방법 중 하나를 사용하여 고객의 예약 사용량을 확인하고 예약 할인이 적용되는 가상 머신을 확인할 수 있습니다.

- Azure Portal
- Azure 사용률 API

이러한 각 메서드를 사용하기 위한 지침은 다음과 같습니다.

>[!NOTE]
>Azure 사용률 API만 할인이 적용되는 가상 머신을 표시합니다.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Microsoft Azure Portal에서 고객의 예약 사용량 확인

1. 파트너 센터 **고객** 페이지로 이동합니다.

2. 확인하려는 예약 할인 및 사용량을 가진 고객을 찾은 다음, 아래쪽 화살표를 선택하여 고객의 정보를 확장합니다. **Microsoft Azure 관리 포털** 선택하여 Azure Portal 고객의 레코드를 엽니다.
3. 포털 메뉴에서 **예약을** 선택한 다음, 사용량을 확인하려는 예약을 선택합니다.
4. **개요** 페이지에서 예약의 사용률 그래프를 확인합니다. 이 그래프는 가상 머신에 적용된 예약의 양을 보여줍니다.

    >[!NOTE]
    >사용률 데이터는 최대 8시간까지 지연될 수 있습니다.

    a. 예약 사용률이 100%이면 고객은 예약 구매에서 제공할 수 있는 가능한 모든 절감액을 얻게 됩니다.
    b. 예약 사용량이 0%이면 할인이 가상 머신에 적용되지 않습니다.
    c. 예약 사용량이 1%에서 99% 사이인 경우 사용되지 않는 이점이 있습니다.

5. 이러한 상황을 방지하려면 구매하기 전에 고객의 컴퓨팅 요구 사항을 지원하기 위해 올바른 크기의 VM을 결정합니다.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Azure 사용률 API를 통해 고객의 예약 사용량 확인

>[!NOTE]
>Azure 사용률 API만 할인이 적용되는 가상 머신을 표시합니다.  

Azure 사용률 API를 사용하여 예약 사용량 데이터를 통해 고객이 예약 할인을 받고 있는지 확인하고 할인이 적용되는 VM(가상 머신)을 확인할 수 있습니다. 예제 A와 예제 B를 비교하여 고객의 예약 사용량을 확인하는 방법을 확인합니다.

:::image type="content" source="images/usage5.png" alt-text="예약 사용 예제.":::

- reservationId는 VM에 할인을 적용하는 데 사용된 Azure 예약을 식별합니다.
- consumptionMeter는 예약 할인이 적용된 VM의 MeterId입니다.
- ReservationMeter는 예약 할인이 적용된 이후 $0 비용을 표시합니다.

자세한 내용은 [파트너 센터 API에서](/partner-center/develop/) [Azure에 대한 고객의 사용률 레코드 얻기를 참조하세요.](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)

>[!IMPORTANT]
>Microsoft Windows Server와 같은 소프트웨어 비용은 현재 VM 예약 가격에 포함되지 않으며 주문 레코드 및 청구서에 별도의 품목으로 표시됩니다. 그러나 고객에게 Azure 하이브리드 사용 혜택이 있는 경우 소프트웨어 비용이 적용되지 않습니다. 자세한 내용은 [reserved Instances에 포함되지 않은 소프트웨어 비용 Windows 참조하세요.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>다음 단계

|**원하는 정보**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
|CSP의 Azure 예약 개요  | [Microsoft Azure 예약 VM 인스턴스 판매](azure-reservations.md)
|파트너 센터 고객에 대한 Azure 예약 구매   | [Azure 예약 구입](azure-reservations-buying.md)
|파트너 센터 Azure 예약 관리 | [파트너 센터 Azure 예약 관리](azure-reservations-manage.md)
|Azure Portal Azure 예약 구매 | Azure [도움말에서 Azure Reserved VM Instances 가상 머신에 대한 선불](/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|Azure Portal Azure 예약 관리   | Azure 도움말에서 [예약된 VM 인스턴스 관리](/azure/billing/billing-manage-reserved-vm-instance)  |
|파트너 센터 API를 사용하여 Azure 예약 구매 | [파트너 센터](/partner-center/develop/purchase-azure-reservations) 개발자 설명서의 구매 Azure Reserved VM Instances   |
|고객이 구매한 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에게 부여합니다. | [고객에게 자신의 Azure 예약을 구매할 수 있는 권한 부여](give-customers-permission.md)   |