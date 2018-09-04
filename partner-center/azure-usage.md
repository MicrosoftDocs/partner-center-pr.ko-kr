---
title: 최대 예약 사용량에 맞게 Microsoft Azure VM 크기 조정 | 파트너 대시보드
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: azure, 예약, vm, 관리, 사용량, 크기 조정
ms.localizationpriority: medium
ms.openlocfilehash: bb7d022ba45462db313a9f4e16cc47e4550dbef6
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/31/2018
ms.locfileid: "2875783"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="9c9b6-103">최대 예약 사용량에 맞게 Microsoft Azure VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="9c9b6-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="9c9b6-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="9c9b6-104">Applies to</span></span>**

-  <span data-ttu-id="9c9b6-105">파트너 대시보드</span><span class="sxs-lookup"><span data-stu-id="9c9b6-105">Partner dashboard</span></span>
-  <span data-ttu-id="9c9b6-106">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="9c9b6-106">Azure portal</span></span>
-  <span data-ttu-id="9c9b6-107">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="9c9b6-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="9c9b6-108">고객의 Azure 예약에 대한 VM 크기 결정</span><span class="sxs-lookup"><span data-stu-id="9c9b6-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="9c9b6-109">고객을 대신하여 Microsoft Azure 예약을 구입하는 경우에는 고객의 컴퓨팅 요구를 충족하도록 크기가 조정된 가상 컴퓨터(VM)를 선택해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="9c9b6-110">다음 방법 중 하나를 사용하여 이 정보를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="9c9b6-111">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="9c9b6-111">Azure utilization API</span></span>
-   <span data-ttu-id="9c9b6-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="9c9b6-112">The Azure portal</span></span>
-   <span data-ttu-id="9c9b6-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="9c9b6-113">Azure PowerShell</span></span>
-   <span data-ttu-id="9c9b6-114">Azure Resource Manager(ARM) API</span><span class="sxs-lookup"><span data-stu-id="9c9b6-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="9c9b6-115">이러한 각 방법의 사용 지침은 아래와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="9c9b6-116">예약을 구입하고 나면 예약의 속성 및 수량과 일치하는 가상 컴퓨터에 예약 할인이 자동으로 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="9c9b6-117">VM에 예약을 할당할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="9c9b6-118">예약 할인은 클래식 또는 프로모션 VM에 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="9c9b6-119">고객을 대신하여 구입하기 위해 VM의 유형 및 크기를 올바르게 파악하려면 VM 시리즈 유형이 파트너 센터 조정 파일에 올바르게 표시되지 않을 때 아래에 설명된 방법 중 하나를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="9c9b6-120">Azure 사용률 API를 이용해 VM 크기 조정 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="9c9b6-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="9c9b6-121">API 응답 시 additionalInfo에서 ServiceType 속성의 값을 사용하여 구입할 VM 크기를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="9c9b6-122">자세한 내용은 [Azure에 대 한 고객 사용률 기록 얻기](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [파트너 대시보드 API](https://docs.microsoft.com/partner-center/develop/)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="9c9b6-123">Microsoft Azure Portal을 이용해 VM 크기 조정 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="9c9b6-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="9c9b6-124">파트너 대시보드에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-124">In your Partner dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="9c9b6-125">VM 예약을 구입하려는 고객을 찾고 아래쪽 화살표를 선택하여 고객의 정보를 펼쳐봅니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="9c9b6-126">**Microsoft Azure 관리 포털**을 선택하여 Azure Portal에서 고객의 기록을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="9c9b6-127">포털 메뉴에서 **가상 컴퓨터**를 선택한 다음, 예약을 구입하고 싶은 VM을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="9c9b6-128">VM의 세부 정보 페이지에서 아래 그림에서와 같이 크기 및 지역 정보를 찾고 이 정보를 이용해 파트너 센터에서 예약을 구입합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![](images/usage1.png)

**<span data-ttu-id="9c9b6-129">Microsoft Azure PowerShell을 이용해 VM 크기 조정 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="9c9b6-129">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="9c9b6-130">아래 이미지에서 이 정보를 사용하여 예약을 구입하고 싶은 VM의 크기와 위치를 파악합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-130">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![](images/usage2.png)

**<span data-ttu-id="9c9b6-131">Azure Resource Manager(ARM) API를 이용해 VM 크기 조정 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="9c9b6-131">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="9c9b6-132">ARMClient 또는 ARM API를 이용해 예약을 구입하고 싶은 VM에 대한 ARM 클라이언트를 호출합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-132">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="9c9b6-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="9c9b6-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="9c9b6-134">호출을 하면 아래 그림에서와 같이 **vmSize** 및 **location**에 대한 값이 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-134">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="9c9b6-135">Azure VM 사용량 및 예약 할인 확인</span><span class="sxs-lookup"><span data-stu-id="9c9b6-135">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="9c9b6-136">고객을 대신하여 Azure Reserved VM Instances를 구입하고 나면 VM 공간 요금 선납에 대한 할인 혜택이 고객의 예약 속성 및 수량과 일치하는 가상 컴퓨터에 자동으로 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-136">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="9c9b6-137">고객의 예약 사용량을 확인하고 다음 방법 중 하나를 사용하여 예약 할인이 적용되는 가상 컴퓨터를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-137">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="9c9b6-138">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="9c9b6-138">The Azure portal</span></span>
-   <span data-ttu-id="9c9b6-139">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="9c9b6-139">Azure utilization API</span></span>

<span data-ttu-id="9c9b6-140">이러한 각 방법의 사용 지침은 아래와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-140">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="9c9b6-141">Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-141">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="9c9b6-142">Microsoft Azure Portal에서 고객의 예약 사용량 확인</span><span class="sxs-lookup"><span data-stu-id="9c9b6-142">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="9c9b6-143">파트너 대시보드에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-143">In your Partner dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="9c9b6-144">예약 할인 및 사용률을 확인하고 싶은 고객을 찾고 아래쪽 화살표를 선택하여 고객의 정보를 펼쳐봅니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-144">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="9c9b6-145">**Microsoft Azure 관리 포털**을 선택하여 Azure Portal에서 고객의 기록을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-145">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="9c9b6-146">포털 메뉴에서 **예약**을 선택한 다음, 사용량을 확인하고 싶은 예약을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-146">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="9c9b6-147">**개요** 페이지에서 가상 컴퓨터에 얼마나 많은 예약이 적용되었는지 보여주는 예약의 사용률 그래프를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-147">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="9c9b6-148">사용률 데이터는 최대 8시간까지 지연될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-148">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="9c9b6-149">a.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-149">a.</span></span>  <span data-ttu-id="9c9b6-150">예약의 사용률이 100%인 경우에는 예약 구입이 제공할 수 있는 가능한 모든 절감 혜택을 고객이 누리게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-150">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="9c9b6-151">b.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-151">b.</span></span>  <span data-ttu-id="9c9b6-152">예약 사용률이 0%인 경우에는 어떤 가상 컴퓨터에도 할인이 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-152">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="9c9b6-153">c.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-153">c.</span></span>  <span data-ttu-id="9c9b6-154">예약의 사용률이 1% ~ 99%인 경우에는 미사용 혜택이 존재합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-154">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="9c9b6-155">이런 상황을 방지하려면 구입에 앞서 고객의 컴퓨팅 요구를 지원할 수 있는 올바른 크기의 VM을 결정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-155">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="9c9b6-156">Azure 사용률 API를 통해 고객의 예약 사용량 확인</span><span class="sxs-lookup"><span data-stu-id="9c9b6-156">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="9c9b6-157">Azure 사용률 API에는 할인이 적용 중인 가상 컴퓨터만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-157">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="9c9b6-158">Azure 활용률 API를 통해 예약 사용량 데이터를 얻어서 고객이 예약 할인을 받고 있는지 확인하고 할인이 적용되는 가상 컴퓨터(VM)를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-158">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="9c9b6-159">예제 A와 예제 B를 비교하여 고객의 예약 사용량을 확인하는 방법을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-159">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![](images\usage5.png)

-   <span data-ttu-id="9c9b6-160">reservationId는 VM에 할인을 적용하는 데 사용된 Azure 예약을 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-160">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="9c9b6-161">consumptionMeter는 예약 할인이 적용되는 VM의 MeterId입니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-161">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="9c9b6-162">예약 할인이 적용되었기 때문에 ReservationMeter는 0달러로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-162">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="9c9b6-163">자세한 내용은 [파트너 센터 API](https://docs.microsoft.com/partner-center/develop/)의 [Azure에 대한 고객 사용률 기록 얻기](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-163">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="9c9b6-164">Microsoft Windows Server 등의 소프트웨어 비용은 현재 VM 예약 가격에 포함되어 있지 않으며, 주문 기록 및 송장에 개별 품목으로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-164">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="9c9b6-165">그러나 고객이 Azure 하이브리드 사용 혜택을 이용하고 있는 경우에는 소프트웨어 비용이 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-165">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="9c9b6-166">자세한 내용은 [예약 인스턴스에 포함되어 있지 않은 Windows 소프트웨어 비용](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-166">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="9c9b6-167">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="9c9b6-167">Azure reservations resources</span></span>
|**<span data-ttu-id="9c9b6-168">자세한 내용</span><span class="sxs-lookup"><span data-stu-id="9c9b6-168">For information about</span></span>**   |**<span data-ttu-id="9c9b6-169">이 글 읽기</span><span class="sxs-lookup"><span data-stu-id="9c9b6-169">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="9c9b6-170">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="9c9b6-170">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="9c9b6-171">Microsoft Azure Reserved VM Instances 판매</span><span class="sxs-lookup"><span data-stu-id="9c9b6-171">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="9c9b6-172">파트너 대시보드에서 고객을 위한 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="9c9b6-172">Purchasing Azure reservations for your customers in your Partner dashboard</span></span>   |[<span data-ttu-id="9c9b6-173">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="9c9b6-173">Buy Azure reservations</span></span>](azure-reservations-buying.md)
| <span data-ttu-id="9c9b6-174">파트너 대시보드에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="9c9b6-174">Managing Azure reservations in your Partner dashboard</span></span> | [<span data-ttu-id="9c9b6-175">파트너 대시보드에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="9c9b6-175">Managing Azure reservations in your Partner dashboard</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="9c9b6-176">Azure Portal에서 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="9c9b6-176">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="9c9b6-177">Azure 도움말의 [Azure Reserved VM Instances에서 가상 컴퓨터에 대한 사전 지불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-177">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="9c9b6-178">Azure Portal에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="9c9b6-178">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="9c9b6-179">Azure 도움말의 [예약된 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-179">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="9c9b6-180">파트너 센터 API를 사용하여 Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="9c9b6-180">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="9c9b6-181">파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9c9b6-181">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



