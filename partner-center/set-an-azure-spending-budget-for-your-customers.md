---
title: 고객에 대 한 Azure 지출 예산 설정
ms.topic: how-to
ms.date: 06/03/2020
description: 고객에 대 한 월간 Azure 지출 예산을 설정 또는 제거 하는 방법과 Azure 지출 데이터를 보고 예산 관련 알림을 설정 하는 방법을 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 982d4ed310415349acde3d260afce04eb0d55ac5
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811253"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="dfaac-103">파트너 센터에서 고객에 대 한 월간 Azure 지출 예산 설정, 확인 또는 제거</span><span class="sxs-lookup"><span data-stu-id="dfaac-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="dfaac-104">적용 대상:</span><span class="sxs-lookup"><span data-stu-id="dfaac-104">Applies to:</span></span>

- <span data-ttu-id="dfaac-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="dfaac-105">Partner Center</span></span>
- <span data-ttu-id="dfaac-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="dfaac-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="dfaac-107">파트너 센터에서 [고객에 대 한 월간 Azure 지출 예산을 설정할](#set-azure-spending-budget) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="dfaac-108">이렇게 하면 고객이 Azure 지출를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="dfaac-109">이 옵션을 사용 하면 고객의 Azure 지출를 해당 월의 예산과 비교할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="dfaac-110">또한 고객은 자신의 Azure 지출에 대 한 비용을 청구 하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="dfaac-111">이 기능은 샌드박스 또는 프로덕션 (TIP) 계정의 테스트에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="dfaac-112">[고객에 대 한 Azure 지출 예산을 설정한](#set-azure-spending-budget)후에는 다음과 같은 방법으로 고객 사용량을 검토할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="dfaac-113">이러한 옵션은 잘못 구성 된 서비스 또는 사기 행위를 제안할 수 있는 비정상적인 추세를 찾는 데 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="dfaac-114">그런 다음 고객을 사용 하 여 근본 원인을 파악 하 고 비용을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="dfaac-115">필요한 경우 [고객의 예산을](#set-azure-spending-budget) 더 높은 값으로 변경할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="dfaac-116">현재 Azure 지출 확인</span><span class="sxs-lookup"><span data-stu-id="dfaac-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="dfaac-117">고객의 예산이 예산 제한에 근접 한 경우에 대 한 전자 메일 알림 설정</span><span class="sxs-lookup"><span data-stu-id="dfaac-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="dfaac-118">사용량 기반 구독에 대해 서비스 별로 항목별 비용 보기</span><span class="sxs-lookup"><span data-stu-id="dfaac-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="dfaac-119">또한 언제 든 지 고객에 대 한 [Azure 지출 예산을 제거할](#remove-azure-spending-budget) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="dfaac-120">Azure 지출 데이터</span><span class="sxs-lookup"><span data-stu-id="dfaac-120">Azure spending data</span></span>

<span data-ttu-id="dfaac-121">Azure 지출 데이터는 *예상치* 이며 *실제 청구 금액은 다를 수 있습니다*.</span><span class="sxs-lookup"><span data-stu-id="dfaac-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="dfaac-122">데이터 값에는 세금, 크레딧, 조정 또는 적용 될 수 있는 기타 요금이 *반영 되지 않습니다* .</span><span class="sxs-lookup"><span data-stu-id="dfaac-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="dfaac-123">지출 데이터는 *하루에 한 번 새로 고쳐집니다*.</span><span class="sxs-lookup"><span data-stu-id="dfaac-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="dfaac-124">Azure Portal에서 계정 설정을 변경 하지 않는 한 고객은 Azure 서비스 및 리소스에 대 한 사용을 계속 하 고 요금이 부과 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="dfaac-125">Azure 지출 예산 설정</span><span class="sxs-lookup"><span data-stu-id="dfaac-125">Set Azure spending budget</span></span>

<span data-ttu-id="dfaac-126">파트너 센터에서 여러 고객에 대 한 *월간 Azure 지출 예산을 설정할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="dfaac-127">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dfaac-128">**CSP**의 왼쪽 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dfaac-129">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객**에서 예산을 설정 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="dfaac-130">**월별 예산**에 대 한 값을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="dfaac-131">**적용** 을 선택 하 여 변경 내용을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="dfaac-132">구독 설정에서 *개별 고객에 대 한 예산을 설정할* 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="dfaac-133">파트너 센터 대시보드에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="dfaac-134">**CSP**의 왼쪽 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="dfaac-135">**고객** 페이지에서 고객의 **회사 이름을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="dfaac-136">고객의 **구독** 페이지의 **사용량 기반 구독**에서 **예산 변경**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="dfaac-137">예산 값을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="dfaac-138">**적용** 을 선택 하 여 변경 내용을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="dfaac-139">Azure 지출 예산 제거</span><span class="sxs-lookup"><span data-stu-id="dfaac-139">Remove Azure spending budget</span></span>

<span data-ttu-id="dfaac-140">파트너 센터에서 고객에 대 한 *월간 Azure 지출 예산을 제거할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="dfaac-141">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dfaac-142">**CSP**의 왼쪽 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dfaac-143">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객**에서 예산을 제거 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="dfaac-144">**예산 제거**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="dfaac-145">현재 Azure 지출 확인</span><span class="sxs-lookup"><span data-stu-id="dfaac-145">Check current Azure spending</span></span>

<span data-ttu-id="dfaac-146">언제 든 지 *고객의 현재 Azure 지출 및 월별 예산을 추적할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="dfaac-147">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dfaac-148">**CSP**의 왼쪽 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dfaac-149">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객**에서 고객의 월간 예산, 현재 지출 예상 및 사용 된 예산 백분율에 대 한 개요를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="dfaac-150">예산 제한에 대 한 알림</span><span class="sxs-lookup"><span data-stu-id="dfaac-150">Notifications for budget limits</span></span>

<span data-ttu-id="dfaac-151">고객의 월간 지출을 예산 제한에 근접 한 경우에 대 한 *전자 메일 알림을 켤* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="dfaac-152">이 옵션을 켜면 고객이 매월 예산 중 80% 이상을 사용할 때 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="dfaac-153">이 옵션을 사용 하면 Azure 청구서에 대 한 정보를 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="dfaac-154">전자 메일 알림을 구성 하려면:</span><span class="sxs-lookup"><span data-stu-id="dfaac-154">To configure email notifications:</span></span>

1. <span data-ttu-id="dfaac-155">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dfaac-156">**CSP**의 왼쪽 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dfaac-157">**Azure 지출** 페이지의 **전자 메일 알림**에서 **전자 메일 가져오기** 설정을 **켜기**로 전환 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>

4. <span data-ttu-id="dfaac-158">**전자 메일 주소 변경** 을 선택 하 여 알림의 전자 메일 주소를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="dfaac-159">전자 메일 주소가 *올바르지*않으면 올바른 전자 메일 주소를 입력 하 고 **업데이트**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="dfaac-160">전자 메일 주소가 *올바르면* **취소**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="dfaac-161">서비스 별로 항목별 비용</span><span class="sxs-lookup"><span data-stu-id="dfaac-161">Itemized costs by service</span></span>

<span data-ttu-id="dfaac-162">*사용량 기반 구독에 대해 서비스 별로 항목별 비용 (및 예상 사용량)을 볼*수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="dfaac-163">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dfaac-164">**CSP**의 왼쪽 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="dfaac-165">**고객** 페이지에서 고객의 **회사 이름을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="dfaac-166">고객의 **구독** 페이지의 **사용량 기반 구독**에서 **구독의**이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="dfaac-167">구독 페이지에서 서비스 별로 **항목별 비용** 및 현재 달의 **예상 사용량** 을 검토할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dfaac-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
