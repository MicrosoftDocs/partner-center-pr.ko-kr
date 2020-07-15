---
title: 최대 예약 사용량에 대 한 Azure VM 크기 조정
ms.topic: article
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: VM에 대 한 Microsoft Azure 예약을 구매할 때 고객의 컴퓨팅 요구에 따라 VM (가상 머신)의 크기를 조정 하는 방법을 알아봅니다.
author: BillLinzbach
ms.author: BillLi
keywords: azure, 예약, vm, 관리, 사용량, 크기 조정
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 00da6723fc8aa4a5b3f1e0f747cb63acc1a504a8
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377657"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="69355-104">최대 예약 사용에 대한 Microsoft Azure VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="69355-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="69355-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="69355-105">**Applies to**</span></span>

- <span data-ttu-id="69355-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="69355-106">Partner Center</span></span>
- <span data-ttu-id="69355-107">Azure portal</span><span class="sxs-lookup"><span data-stu-id="69355-107">Azure portal</span></span>
- <span data-ttu-id="69355-108">CSP의 파트너</span><span class="sxs-lookup"><span data-stu-id="69355-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="69355-109">고객의 Azure 예약에 대 한 VM 크기 결정</span><span class="sxs-lookup"><span data-stu-id="69355-109">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="69355-110">고객을 대신 하 여 Microsoft Azure 예약을 구입 하는 경우 고객의 컴퓨팅 요구에 맞게 VM (가상 머신) 크기를 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="69355-111">다음 방법 중 하나를 사용 하 여이 정보를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="69355-112">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="69355-112">Azure utilization API</span></span>
- <span data-ttu-id="69355-113">Azure 포털</span><span class="sxs-lookup"><span data-stu-id="69355-113">The Azure portal</span></span>
- <span data-ttu-id="69355-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="69355-114">Azure PowerShell</span></span>
- <span data-ttu-id="69355-115">ARM (Azure Resource Manager) API</span><span class="sxs-lookup"><span data-stu-id="69355-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="69355-116">이러한 각 메서드를 사용 하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="69355-117">예약을 구매한 후 예약 할인은 예약의 특성과 수량과 일치 하는 가상 컴퓨터에 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69355-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="69355-118">VM에 예약을 할당할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="69355-119">클래식 또는 프로 모션 Vm에는 예약 할인이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="69355-120">고객을 대신 하 여 구매할 VM의 유형과 크기를 올바르게 식별 하려면 파트너 센터 조정 파일에 VM 시리즈 유형이 올바르게 표시 되지 않으므로 아래 설명 된 방법 중 하나를 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="69355-121">Azure 사용률 API를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="69355-121">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="69355-122">API 응답에서 additionalInfo의 ServiceType 특성에 대 한 값을 사용 하 여 구매할 VM 크기를 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="69355-123">자세한 내용은 [파트너 센터 API](https://docs.microsoft.com/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="69355-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="69355-124">Microsoft Azure portal를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="69355-124">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="69355-125">파트너 센터에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-125">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="69355-126">Azure VM 예약을 구입 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="69355-127">**Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="69355-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="69355-128">포털 메뉴에서 **Virtual machines** 를 선택 하 고 예약을 구입할 VM을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="69355-129">VM의 세부 정보 페이지에서 아래 그림과 같이 크기 및 지역 정보를 확인 하 고이 정보를 사용 하 여 파트너 센터에서 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="세부 정보 페이지의 크기 및 지역 정보":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="69355-131">Microsoft Azure PowerShell를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="69355-131">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="69355-132">아래 이미지의 정보를 사용 하 여 예약을 구매 하려는 VM의 위치 및 크기를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="69355-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM 위치 및 크기":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="69355-134">ARM (Azure Resource Manager) API를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="69355-134">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="69355-135">ARMClient 또는 ARM Api를 사용 하 여 예약을 구매 하려는 VM에 대 한 ARM 클라이언트를 호출 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="69355-136">/subscriptions/ <Subscription ID> /Ssourceg/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? api-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="69355-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="69355-137">이 호출은 아래 그림과 같이 **Vmsize** 및 **location**에 대 한 값을 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 값":::
    :::image type="content" source="images/usage4.png" alt-text="위치 값":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="69355-140">Azure VM 사용 및 예약 할인 확인</span><span class="sxs-lookup"><span data-stu-id="69355-140">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="69355-141">고객을 대신 하 여 Azure 예약 VM 인스턴스를 구매한 후에는 VM 공간에 대 한 요금 지불 할인이 고객 예약의 특성 및 수량과 일치 하는 가상 머신에 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69355-141">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="69355-142">다음 방법 중 하나를 사용 하 여 고객의 예약 사용량을 확인 하 고 예약 할인이 적용 되는 가상 컴퓨터를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-142">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="69355-143">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="69355-143">The Azure portal</span></span>
- <span data-ttu-id="69355-144">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="69355-144">Azure utilization API</span></span>

<span data-ttu-id="69355-145">이러한 각 메서드를 사용 하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-145">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="69355-146">Azure 사용률 API에만 할인이 적용 되는 가상 머신이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69355-146">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="69355-147">Microsoft Azure portal에서 고객의 예약 사용 현황을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-147">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="69355-148">파트너 센터에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-148">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="69355-149">예약 할인 및 사용량을 확인 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-149">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="69355-150">**Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="69355-150">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="69355-151">포털 메뉴에서 **예약** 을 선택 하 고 사용량을 확인 하려는 예약을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-151">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="69355-152">**개요** 페이지에서 가상 컴퓨터에 적용 된 예약의 양을 보여 주는 예약 사용률 그래프를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-152">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="69355-153">사용률 데이터는 최대 8 시간까지 지연 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-153">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="69355-154">a.</span><span class="sxs-lookup"><span data-stu-id="69355-154">a.</span></span> <span data-ttu-id="69355-155">예약의 사용률이 100% 인 경우 고객은 예약 구매가 제공할 수 있는 모든 절감 액을 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-155">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="69355-156">b.</span><span class="sxs-lookup"><span data-stu-id="69355-156">b.</span></span> <span data-ttu-id="69355-157">예약의 사용량이 0% 이면 모든 가상 머신에 할인이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-157">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="69355-158">다.</span><span class="sxs-lookup"><span data-stu-id="69355-158">c.</span></span> <span data-ttu-id="69355-159">예약의 사용량이 1%에서 99% 사이인 경우 사용 하지 않는 이점이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-159">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="69355-160">이러한 상황을 방지 하려면 구매를 수행 하기 전에 고객의 컴퓨팅 요구를 지원 하도록 올바른 크기의 VM을 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-160">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="69355-161">Azure 사용량 API를 사용 하 여 고객의 예약 사용 확인</span><span class="sxs-lookup"><span data-stu-id="69355-161">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="69355-162">Azure 사용률 API에만 할인이 적용 되는 가상 머신이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69355-162">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="69355-163">Azure 사용률 API를 사용 하 여 예약 사용 데이터를 가져와 고객이 예약 할인을 받고 할인이 적용 되는 Vm (가상 머신)을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-163">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="69355-164">예 A를 예 2와 비교 하 여 고객의 예약 사용량을 확인 하는 방법을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-164">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="예약 사용 예":::

- <span data-ttu-id="69355-166">ReservationId는 VM에 할인을 적용 하는 데 사용 된 Azure 예약을 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-166">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="69355-167">consumptionMeter는 예약 할인이 적용 된 VM의 MeterId입니다.</span><span class="sxs-lookup"><span data-stu-id="69355-167">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="69355-168">ReservationMeter는 예약 할인이 적용 된 이후 $0 비용을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="69355-168">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="69355-169">자세한 내용은 [파트너 센터 API](https://docs.microsoft.com/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="69355-169">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="69355-170">Microsoft Windows Server와 같은 소프트웨어 비용은 현재 VM 예약 가격에 포함 되지 않으며 주문 레코드 및 청구서에 별도의 품목으로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69355-170">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="69355-171">그러나 고객이 Azure 하이브리드 사용 혜택을 사용 하는 경우 소프트웨어 비용이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="69355-171">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="69355-172">자세한 내용은 [예약 된 인스턴스에 포함 되지 않는 Windows 소프트웨어 비용](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="69355-172">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="69355-173">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="69355-173">Azure reservations resources</span></span>

|<span data-ttu-id="69355-174">**원하는 정보**</span><span class="sxs-lookup"><span data-stu-id="69355-174">**For information about**</span></span>   |<span data-ttu-id="69355-175">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="69355-175">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="69355-176">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="69355-176">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="69355-177">Microsoft Azure 예약 VM 인스턴스 판매</span><span class="sxs-lookup"><span data-stu-id="69355-177">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="69355-178">파트너 센터에서 고객에 대 한 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="69355-178">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="69355-179">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="69355-179">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="69355-180">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="69355-180">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="69355-181">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="69355-181">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="69355-182">Azure Portal에서 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="69355-182">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="69355-183">Azure 도움말의 [Azure Reserved VM Instances를 사용 하는 가상 머신의 선불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="69355-183">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="69355-184">Azure Portal에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="69355-184">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="69355-185">Azure 도움말에서 [예약 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="69355-185">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="69355-186">파트너 센터 API를 사용 하 여 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="69355-186">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="69355-187">파트너 센터 개발자 설명서에서 [Azure Reserved VM Instances 구매](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="69355-187">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="69355-188">구매한 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="69355-188">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="69355-189">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="69355-189">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
