---
title: 최대 예약 사용량에 맞게 Azure VM 크기 조정
description: 고객의 컴퓨팅 요구 사항에 맞게 VM(가상 머신)의 크기를 Microsoft Azure 예약을 구매하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149454"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="ca436-103">최대 예약 사용에 대한 Microsoft Azure VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="ca436-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="ca436-104">**적절한 역할:** 관리 에이전트 | 판매 에이전트</span><span class="sxs-lookup"><span data-stu-id="ca436-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="ca436-105">이 문서에서는 고객의 컴퓨팅 요구 사항에 맞게 VM(가상 머신)의 크기를 Microsoft Azure 예약을 구매하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="ca436-106">이 문서는 CSP(클라우드 솔루션 공급자) 프로그램의 파트너에게만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="ca436-107">다른 유형의 구독(예: 종량제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용하는 고객은 대신 [이 Azure 예약 설명서를](/azure/cost-management-billing/reservations)읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="ca436-108">고객의 Azure 예약에 대한 VM 크기 결정</span><span class="sxs-lookup"><span data-stu-id="ca436-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="ca436-109">고객을 대신하여 Microsoft Azure 예약을 구입하는 경우 고객의 컴퓨팅 요구 사항에 맞게 크기가 인 VM(가상 머신)을 선택해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="ca436-110">다음 방법 중 하나를 사용하여 이 정보를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="ca436-111">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="ca436-111">Azure utilization API</span></span>
- <span data-ttu-id="ca436-112">Azure 포털</span><span class="sxs-lookup"><span data-stu-id="ca436-112">The Azure portal</span></span>
- <span data-ttu-id="ca436-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ca436-113">Azure PowerShell</span></span>
- <span data-ttu-id="ca436-114">Azure Resource Manager(ARM) API</span><span class="sxs-lookup"><span data-stu-id="ca436-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="ca436-115">이러한 각 메서드를 사용하기 위한 지침은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="ca436-116">예약을 구매하면 예약 할인이 예약의 특성 및 수량과 일치하는 가상 머신에 자동으로 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="ca436-117">VM에 예약을 할당할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="ca436-118">예약 할인은 클래식 또는 프로모션 VM에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="ca436-119">고객을 대신하여 구매할 VM의 유형과 크기를 올바르게 식별하려면 아래에 설명된 방법 중 하나를 사용해야 합니다. VM 시리즈 형식이 파트너 센터 조정 파일에 올바르게 표시되지 않기 때문에 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="ca436-120">Azure 사용률 API를 사용하여 VM 크기 조정 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="ca436-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="ca436-121">API 응답에서 additionalInfo의 ServiceType 특성 값을 사용하여 구입할 VM 크기를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="ca436-122">자세한 내용은 [파트너 센터 API에서](/partner-center/develop/) [Azure에 대한 고객의 사용률 레코드 얻기를 참조하세요.](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)</span><span class="sxs-lookup"><span data-stu-id="ca436-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="ca436-123">Microsoft Azure portal 사용하여 VM 크기 조정 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="ca436-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="ca436-124">파트너 센터 **고객** 페이지로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="ca436-125">Azure VM 예약을 구입 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="ca436-126">**Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="ca436-127">포털 메뉴에서 **Virtual machines** 를 선택 하 고 예약을 구입할 VM을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="ca436-128">VM의 세부 정보 페이지에서 아래 그림과 같이 크기 및 지역 정보를 확인 하 고이 정보를 사용 하 여 파트너 센터에서 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="세부 정보 페이지의 크기 및 지역 정보":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="ca436-130">Microsoft Azure PowerShell를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="ca436-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="ca436-131">아래 이미지의 정보를 사용 하 여 예약을 구매 하려는 VM의 위치 및 크기를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM 위치 및 크기":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="ca436-133">ARM (Azure Resource Manager) API를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="ca436-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="ca436-134">ARMClient 또는 ARM Api를 사용 하 여 예약을 구매 하려는 VM에 대 한 ARM 클라이언트를 호출 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="ca436-135">/subscriptions/ <Subscription ID> /Ssourceg/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? api-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="ca436-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="ca436-136">이 호출은 아래 그림과 같이 **Vmsize** 및 **location** 에 대 한 값을 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 값":::
    :::image type="content" source="images/usage4.png" alt-text="위치 값":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="ca436-139">Azure VM 사용 및 예약 할인 확인</span><span class="sxs-lookup"><span data-stu-id="ca436-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="ca436-140">고객을 대신 하 여 Azure 예약 VM 인스턴스를 구매한 후에는 VM 공간에 대 한 요금 지불 할인이 고객 예약의 특성 및 수량과 일치 하는 가상 머신에 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="ca436-141">다음 방법 중 하나를 사용 하 여 고객의 예약 사용량을 확인 하 고 예약 할인이 적용 되는 가상 컴퓨터를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="ca436-142">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ca436-142">The Azure portal</span></span>
- <span data-ttu-id="ca436-143">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="ca436-143">Azure utilization API</span></span>

<span data-ttu-id="ca436-144">이러한 각 메서드를 사용 하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="ca436-145">Azure 사용률 API에만 할인이 적용 되는 가상 머신이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="ca436-146">Microsoft Azure portal에서 고객의 예약 사용 현황을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="ca436-147">파트너 센터에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="ca436-148">예약 할인 및 사용량을 확인 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="ca436-149">**Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="ca436-150">포털 메뉴에서 **예약** 을 선택 하 고 사용량을 확인 하려는 예약을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="ca436-151">**개요** 페이지에서 가상 컴퓨터에 적용 된 예약의 양을 보여 주는 예약 사용률 그래프를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ca436-152">사용률 데이터는 최대 8 시간까지 지연 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="ca436-153">a.</span><span class="sxs-lookup"><span data-stu-id="ca436-153">a.</span></span> <span data-ttu-id="ca436-154">예약의 사용률이 100% 인 경우 고객은 예약 구매가 제공할 수 있는 모든 절감 액을 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="ca436-155">b.</span><span class="sxs-lookup"><span data-stu-id="ca436-155">b.</span></span> <span data-ttu-id="ca436-156">예약의 사용량이 0% 이면 모든 가상 머신에 할인이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="ca436-157">다.</span><span class="sxs-lookup"><span data-stu-id="ca436-157">c.</span></span> <span data-ttu-id="ca436-158">예약의 사용량이 1%에서 99% 사이인 경우 사용 하지 않는 이점이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="ca436-159">이러한 상황을 방지 하려면 구매를 수행 하기 전에 고객의 컴퓨팅 요구를 지원 하도록 올바른 크기의 VM을 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="ca436-160">Azure 사용량 API를 사용 하 여 고객의 예약 사용 확인</span><span class="sxs-lookup"><span data-stu-id="ca436-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="ca436-161">Azure 사용률 API에만 할인이 적용 되는 가상 머신이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="ca436-162">Azure 사용률 API를 사용 하 여 예약 사용 데이터를 가져와 고객이 예약 할인을 받고 할인이 적용 되는 Vm (가상 머신)을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="ca436-163">예 A를 예 2와 비교 하 여 고객의 예약 사용량을 확인 하는 방법을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="예약 사용 예":::

- <span data-ttu-id="ca436-165">ReservationId는 VM에 할인을 적용 하는 데 사용 된 Azure 예약을 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="ca436-166">consumptionMeter는 예약 할인이 적용 된 VM의 MeterId입니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="ca436-167">ReservationMeter는 예약 할인이 적용 된 이후 $0 비용을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="ca436-168">자세한 내용은 [파트너 센터 API](/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ca436-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="ca436-169">Microsoft Windows Server와 같은 소프트웨어 비용은 현재 VM 예약 가격에 포함되지 않으며 주문 레코드 및 청구서에 별도의 품목으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="ca436-170">그러나 고객에게 Azure 하이브리드 사용 혜택이 있는 경우 소프트웨어 비용이 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="ca436-171">자세한 내용은 [Reserved Instances에 포함되지 않은 Windows 소프트웨어 비용을 참조하세요.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="ca436-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="ca436-172">다음 단계</span><span class="sxs-lookup"><span data-stu-id="ca436-172">Next steps</span></span>

|<span data-ttu-id="ca436-173">**원하는 정보**</span><span class="sxs-lookup"><span data-stu-id="ca436-173">**For information about**</span></span>   |<span data-ttu-id="ca436-174">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="ca436-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="ca436-175">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="ca436-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="ca436-176">예약 VM 인스턴스 Microsoft Azure 판매</span><span class="sxs-lookup"><span data-stu-id="ca436-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="ca436-177">파트너 센터 고객에 대한 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="ca436-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="ca436-178">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="ca436-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="ca436-179">파트너 센터 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="ca436-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="ca436-180">파트너 센터 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="ca436-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="ca436-181">Azure Portal Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="ca436-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="ca436-182">Azure [도움말에서 Azure Reserved VM Instances 가상 머신에 대한 선불](/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="ca436-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="ca436-183">Azure Portal Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="ca436-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="ca436-184">Azure 도움말에서 [예약된 VM 인스턴스 관리](/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="ca436-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="ca436-185">파트너 센터 API를 사용하여 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="ca436-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="ca436-186">[파트너 센터](/partner-center/develop/purchase-azure-reservations) 개발자 설명서의 구매 Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="ca436-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="ca436-187">고객이 구매한 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에게 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="ca436-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="ca436-188">고객에게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="ca436-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |