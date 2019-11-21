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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="489f4-104">최대 예약 사용량에 맞게 Microsoft Azure VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="489f4-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="489f4-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="489f4-105">**Applies to**</span></span>

- <span data-ttu-id="489f4-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="489f4-106">Partner Center</span></span>
- <span data-ttu-id="489f4-107">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="489f4-107">Azure portal</span></span>
- <span data-ttu-id="489f4-108">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="489f4-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="489f4-109">Determine the VM size for a customer's Azure reservation</span><span class="sxs-lookup"><span data-stu-id="489f4-109">Determine the VM size for a customer's Azure reservation</span></span> 

<span data-ttu-id="489f4-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span><span class="sxs-lookup"><span data-stu-id="489f4-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="489f4-111">다음 방법 중 하나를 사용하여 이 정보를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="489f4-112">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="489f4-112">Azure utilization API</span></span>
- <span data-ttu-id="489f4-113">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="489f4-113">The Azure portal</span></span>
- <span data-ttu-id="489f4-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="489f4-114">Azure PowerShell</span></span>
- <span data-ttu-id="489f4-115">Azure Resource Manager(ARM) API</span><span class="sxs-lookup"><span data-stu-id="489f4-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="489f4-116">이러한 각 방법의 사용 지침은 아래와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="489f4-117">예약을 구입하고 나면 예약의 속성 및 수량과 일치하는 가상 컴퓨터에 예약 할인이 자동으로 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="489f4-118">You don't need to assign the reservation to a VM.</span><span class="sxs-lookup"><span data-stu-id="489f4-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="489f4-119">Reservation discounts don't apply to classic or promotional VMs.</span><span class="sxs-lookup"><span data-stu-id="489f4-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="489f4-120">고객을 대신하여 구입하기 위해 VM의 유형 및 크기를 올바르게 파악하려면 VM 시리즈 유형이 파트너 센터 조정 파일에 올바르게 표시되지 않을 때 아래에 설명된 방법 중 하나를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="489f4-121">**Get VM sizing information using the Azure utilization API**</span><span class="sxs-lookup"><span data-stu-id="489f4-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="489f4-122">API 응답 시 additionalInfo에서 ServiceType 속성의 값을 사용하여 구입할 VM 크기를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="489f4-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="489f4-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="489f4-124">**Get VM sizing information using the Microsoft Azure portal**</span><span class="sxs-lookup"><span data-stu-id="489f4-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="489f4-125">In Partner Center, go to your **Customers** page.</span><span class="sxs-lookup"><span data-stu-id="489f4-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="489f4-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span><span class="sxs-lookup"><span data-stu-id="489f4-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="489f4-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="489f4-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="489f4-128">포털 메뉴에서 **가상 컴퓨터**를 선택한 다음, 예약을 구입하고 싶은 VM을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="489f4-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="489f4-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Size and region information on detail page](images/usage1.png)

<span data-ttu-id="489f4-131">**Get VM sizing information using Microsoft Azure PowerShell**</span><span class="sxs-lookup"><span data-stu-id="489f4-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="489f4-132">아래 이미지에서 이 정보를 사용하여 예약을 구입하고 싶은 VM의 크기와 위치를 파악합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![VM location and size](images/usage2.png)

<span data-ttu-id="489f4-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span><span class="sxs-lookup"><span data-stu-id="489f4-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="489f4-135">ARMClient 또는 ARM API를 이용해 예약을 구입하고 싶은 VM에 대한 ARM 클라이언트를 호출합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="489f4-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="489f4-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="489f4-137">호출을 하면 아래 그림에서와 같이 **vmSize** 및 **location**에 대한 값이 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="489f4-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="489f4-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span></span>

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="489f4-139">Azure VM 사용량 및 예약 할인 확인</span><span class="sxs-lookup"><span data-stu-id="489f4-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="489f4-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span><span class="sxs-lookup"><span data-stu-id="489f4-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="489f4-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span><span class="sxs-lookup"><span data-stu-id="489f4-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="489f4-142">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="489f4-142">The Azure portal</span></span>
- <span data-ttu-id="489f4-143">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="489f4-143">Azure utilization API</span></span>

<span data-ttu-id="489f4-144">이러한 각 방법의 사용 지침은 아래와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="489f4-145">Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="489f4-146">Verify the customer's reservation usage in the Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="489f4-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="489f4-147">In Partner Center, go to your **Customers** page.</span><span class="sxs-lookup"><span data-stu-id="489f4-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="489f4-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span><span class="sxs-lookup"><span data-stu-id="489f4-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="489f4-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="489f4-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="489f4-150">포털 메뉴에서 **예약**을 선택한 다음, 사용량을 확인하고 싶은 예약을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="489f4-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span><span class="sxs-lookup"><span data-stu-id="489f4-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="489f4-152">사용률 데이터는 최대 8시간까지 지연될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="489f4-153">a.</span><span class="sxs-lookup"><span data-stu-id="489f4-153">a.</span></span> <span data-ttu-id="489f4-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span><span class="sxs-lookup"><span data-stu-id="489f4-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="489f4-155">b.</span><span class="sxs-lookup"><span data-stu-id="489f4-155">b.</span></span> <span data-ttu-id="489f4-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span><span class="sxs-lookup"><span data-stu-id="489f4-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="489f4-157">c.</span><span class="sxs-lookup"><span data-stu-id="489f4-157">c.</span></span> <span data-ttu-id="489f4-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span><span class="sxs-lookup"><span data-stu-id="489f4-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="489f4-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span><span class="sxs-lookup"><span data-stu-id="489f4-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="489f4-160">Verify the customer's reservation usage with the Azure utilization API</span><span class="sxs-lookup"><span data-stu-id="489f4-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="489f4-161">Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="489f4-162">Azure 활용률 API를 통해 예약 사용량 데이터를 얻어서 고객이 예약 할인을 받고 있는지 확인하고 할인이 적용되는 가상 컴퓨터(VM)를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="489f4-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span><span class="sxs-lookup"><span data-stu-id="489f4-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

![Reservation usage examples](images/usage5.png)

- <span data-ttu-id="489f4-165">reservationId는 VM에 할인을 적용하는 데 사용된 Azure 예약을 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="489f4-166">consumptionMeter는 예약 할인이 적용되는 VM의 MeterId입니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="489f4-167">예약 할인이 적용되었기 때문에 ReservationMeter는 0달러로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="489f4-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="489f4-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="489f4-169">Microsoft Windows Server 등의 소프트웨어 비용은 현재 VM 예약 가격에 포함되어 있지 않으며, 주문 기록 및 송장에 개별 품목으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="489f4-170">그러나 고객이 Azure 하이브리드 사용 혜택을 이용하고 있는 경우에는 소프트웨어 비용이 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="489f4-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="489f4-171">자세한 내용은 [예약 인스턴스에 포함되어 있지 않은 Windows 소프트웨어 비용](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="489f4-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="489f4-172">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="489f4-172">Azure reservations resources</span></span>

|<span data-ttu-id="489f4-173">**For information about**</span><span class="sxs-lookup"><span data-stu-id="489f4-173">**For information about**</span></span>   |<span data-ttu-id="489f4-174">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="489f4-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="489f4-175">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="489f4-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="489f4-176">Sell Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="489f4-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="489f4-177">Purchasing Azure reservations for your customers in Partner Center</span><span class="sxs-lookup"><span data-stu-id="489f4-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="489f4-178">Buy Azure reservations</span><span class="sxs-lookup"><span data-stu-id="489f4-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="489f4-179">Managing Azure reservations in Partner Center</span><span class="sxs-lookup"><span data-stu-id="489f4-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="489f4-180">Managing Azure reservations in Partner Center</span><span class="sxs-lookup"><span data-stu-id="489f4-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="489f4-181">Azure Portal에서 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="489f4-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="489f4-182">Azure 도움말의 [Azure Reserved VM Instances에서 가상 컴퓨터에 대한 사전 지불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="489f4-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="489f4-183">Azure Portal에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="489f4-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="489f4-184">Azure 도움말의 [예약된 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="489f4-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="489f4-185">파트너 센터 API를 사용하여 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="489f4-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="489f4-186">파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="489f4-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
