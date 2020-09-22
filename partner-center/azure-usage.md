---
title: 최대 예약 사용량에 맞게 Azure VM 크기 조정
description: VM에 대 한 Microsoft Azure 예약을 구매할 때 고객의 컴퓨팅 요구에 따라 VM (가상 머신)의 크기를 조정 하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000189"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="23fba-103">최대 예약 사용에 대한 Microsoft Azure VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="23fba-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="23fba-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="23fba-104">**Applies to**</span></span>

- <span data-ttu-id="23fba-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="23fba-105">Partner Center</span></span>
- <span data-ttu-id="23fba-106">Azure portal</span><span class="sxs-lookup"><span data-stu-id="23fba-106">Azure portal</span></span>
- <span data-ttu-id="23fba-107">CSP 프로그램의 파트너</span><span class="sxs-lookup"><span data-stu-id="23fba-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="23fba-108">이 문서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너에만 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="23fba-109">다른 유형의 구독 (예: 종 량 제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용 하는 고객은 [이 Azure 예약 설명서](/azure/cost-management-billing/reservations)를 대신 읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="23fba-110">고객의 Azure 예약에 대 한 VM 크기 결정</span><span class="sxs-lookup"><span data-stu-id="23fba-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="23fba-111">고객을 대신 하 여 Microsoft Azure 예약을 구입 하는 경우 고객의 컴퓨팅 요구에 맞게 VM (가상 머신) 크기를 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="23fba-112">다음 방법 중 하나를 사용 하 여이 정보를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="23fba-113">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="23fba-113">Azure utilization API</span></span>
- <span data-ttu-id="23fba-114">Azure 포털</span><span class="sxs-lookup"><span data-stu-id="23fba-114">The Azure portal</span></span>
- <span data-ttu-id="23fba-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="23fba-115">Azure PowerShell</span></span>
- <span data-ttu-id="23fba-116">ARM (Azure Resource Manager) API</span><span class="sxs-lookup"><span data-stu-id="23fba-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="23fba-117">이러한 각 메서드를 사용 하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="23fba-118">예약을 구매한 후 예약 할인은 예약의 특성과 수량과 일치 하는 가상 컴퓨터에 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="23fba-119">VM에 예약을 할당할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="23fba-120">클래식 또는 프로 모션 Vm에는 예약 할인이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="23fba-121">고객을 대신 하 여 구매할 VM의 유형과 크기를 올바르게 식별 하려면 파트너 센터 조정 파일에 VM 시리즈 유형이 올바르게 표시 되지 않으므로 아래 설명 된 방법 중 하나를 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="23fba-122">Azure 사용률 API를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="23fba-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="23fba-123">API 응답에서 additionalInfo의 ServiceType 특성에 대 한 값을 사용 하 여 구매할 VM 크기를 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="23fba-124">자세한 내용은 [파트너 센터 API](/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="23fba-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="23fba-125">Microsoft Azure portal를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="23fba-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="23fba-126">파트너 센터에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="23fba-127">Azure VM 예약을 구입 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="23fba-128">**Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="23fba-129">포털 메뉴에서 **Virtual machines** 를 선택 하 고 예약을 구입할 VM을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="23fba-130">VM의 세부 정보 페이지에서 아래 그림과 같이 크기 및 지역 정보를 확인 하 고이 정보를 사용 하 여 파트너 센터에서 예약을 구매 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="세부 정보 페이지의 크기 및 지역 정보":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="23fba-132">Microsoft Azure PowerShell를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="23fba-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="23fba-133">아래 이미지의 정보를 사용 하 여 예약을 구매 하려는 VM의 위치 및 크기를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM 위치 및 크기":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="23fba-135">ARM (Azure Resource Manager) API를 사용 하 여 VM 크기 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="23fba-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="23fba-136">ARMClient 또는 ARM Api를 사용 하 여 예약을 구매 하려는 VM에 대 한 ARM 클라이언트를 호출 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="23fba-137">/subscriptions/ <Subscription ID> /Ssourceg/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? api-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="23fba-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="23fba-138">이 호출은 아래 그림과 같이 **Vmsize** 및 **location**에 대 한 값을 반환 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 값":::
    :::image type="content" source="images/usage4.png" alt-text="위치 값":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="23fba-141">Azure VM 사용 및 예약 할인 확인</span><span class="sxs-lookup"><span data-stu-id="23fba-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="23fba-142">고객을 대신 하 여 Azure 예약 VM 인스턴스를 구매한 후에는 VM 공간에 대 한 요금 지불 할인이 고객 예약의 특성 및 수량과 일치 하는 가상 머신에 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="23fba-143">다음 방법 중 하나를 사용 하 여 고객의 예약 사용량을 확인 하 고 예약 할인이 적용 되는 가상 컴퓨터를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="23fba-144">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="23fba-144">The Azure portal</span></span>
- <span data-ttu-id="23fba-145">Azure 사용률 API</span><span class="sxs-lookup"><span data-stu-id="23fba-145">Azure utilization API</span></span>

<span data-ttu-id="23fba-146">이러한 각 메서드를 사용 하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="23fba-147">Azure 사용률 API에만 할인이 적용 되는 가상 머신이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="23fba-148">Microsoft Azure portal에서 고객의 예약 사용 현황을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="23fba-149">파트너 센터에서 **고객** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="23fba-150">예약 할인 및 사용량을 확인 하려는 고객을 찾은 다음 아래쪽 화살표를 선택 하 여 고객의 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="23fba-151">**Microsoft Azure 관리 포털** 를 선택 하 여 Azure Portal에서 고객의 레코드를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="23fba-152">포털 메뉴에서 **예약** 을 선택 하 고 사용량을 확인 하려는 예약을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="23fba-153">**개요** 페이지에서 가상 컴퓨터에 적용 된 예약의 양을 보여 주는 예약 사용률 그래프를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="23fba-154">사용률 데이터는 최대 8 시간까지 지연 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="23fba-155">a.</span><span class="sxs-lookup"><span data-stu-id="23fba-155">a.</span></span> <span data-ttu-id="23fba-156">예약의 사용률이 100% 인 경우 고객은 예약 구매가 제공할 수 있는 모든 절감 액을 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="23fba-157">b.</span><span class="sxs-lookup"><span data-stu-id="23fba-157">b.</span></span> <span data-ttu-id="23fba-158">예약의 사용량이 0% 이면 모든 가상 머신에 할인이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="23fba-159">다.</span><span class="sxs-lookup"><span data-stu-id="23fba-159">c.</span></span> <span data-ttu-id="23fba-160">예약의 사용량이 1%에서 99% 사이인 경우 사용 하지 않는 이점이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="23fba-161">이러한 상황을 방지 하려면 구매를 수행 하기 전에 고객의 컴퓨팅 요구를 지원 하도록 올바른 크기의 VM을 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="23fba-162">Azure 사용량 API를 사용 하 여 고객의 예약 사용 확인</span><span class="sxs-lookup"><span data-stu-id="23fba-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="23fba-163">Azure 사용률 API에만 할인이 적용 되는 가상 머신이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="23fba-164">Azure 사용률 API를 사용 하 여 예약 사용 데이터를 가져와 고객이 예약 할인을 받고 할인이 적용 되는 Vm (가상 머신)을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="23fba-165">예 A를 예 2와 비교 하 여 고객의 예약 사용량을 확인 하는 방법을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="예약 사용 예":::

- <span data-ttu-id="23fba-167">ReservationId는 VM에 할인을 적용 하는 데 사용 된 Azure 예약을 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="23fba-168">consumptionMeter는 예약 할인이 적용 된 VM의 MeterId입니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="23fba-169">ReservationMeter는 예약 할인이 적용 된 이후 $0 비용을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="23fba-170">자세한 내용은 [파트너 센터 API](/partner-center/develop/)에서 [Azure에 대 한 고객의 사용률 레코드 가져오기](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="23fba-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="23fba-171">Microsoft Windows Server와 같은 소프트웨어 비용은 현재 VM 예약 가격에 포함 되지 않으며 주문 레코드 및 청구서에 별도의 품목으로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="23fba-172">그러나 고객이 Azure 하이브리드 사용 혜택을 사용 하는 경우 소프트웨어 비용이 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="23fba-173">자세한 내용은 [예약 된 인스턴스에 포함 되지 않는 Windows 소프트웨어 비용](/azure/billing/billing-reserved-instance-windows-software-costs)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="23fba-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="23fba-174">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="23fba-174">Azure reservations resources</span></span>

|<span data-ttu-id="23fba-175">**원하는 정보**</span><span class="sxs-lookup"><span data-stu-id="23fba-175">**For information about**</span></span>   |<span data-ttu-id="23fba-176">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="23fba-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="23fba-177">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="23fba-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="23fba-178">Microsoft Azure 예약 VM 인스턴스 판매</span><span class="sxs-lookup"><span data-stu-id="23fba-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="23fba-179">파트너 센터에서 고객에 대 한 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="23fba-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="23fba-180">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="23fba-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="23fba-181">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="23fba-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="23fba-182">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="23fba-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="23fba-183">Azure Portal에서 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="23fba-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="23fba-184">Azure 도움말의 [Azure Reserved VM Instances를 사용 하는 가상 머신의 선불](/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="23fba-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="23fba-185">Azure Portal에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="23fba-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="23fba-186">Azure 도움말에서 [예약 VM 인스턴스 관리](/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="23fba-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="23fba-187">파트너 센터 API를 사용 하 여 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="23fba-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="23fba-188">파트너 센터 개발자 설명서에서 [Azure Reserved VM Instances 구매](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="23fba-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="23fba-189">구매한 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="23fba-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="23fba-190">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="23fba-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |