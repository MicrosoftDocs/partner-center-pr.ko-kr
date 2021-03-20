---
title: 고객에 대한 Azure 지출 예산 설정
ms.topic: how-to
ms.date: 03/17/2021
description: 고객에 대 한 월간 Azure 지출 예산을 설정 또는 제거 하는 방법과 Azure 지출 데이터를 보고 예산 관련 알림을 설정 하는 방법을 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712752"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="0d775-103">파트너 센터에서 고객에 대 한 월간 Azure 지출 예산 설정, 확인 또는 제거</span><span class="sxs-lookup"><span data-stu-id="0d775-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="0d775-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="0d775-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0d775-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="0d775-105">Admin agent</span></span>

<span data-ttu-id="0d775-106">파트너 센터에서 [고객에 대 한 월간 Azure 지출 예산을 설정할](#set-azure-spending-budget) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="0d775-107">이렇게 하면 고객이 Azure 지출를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="0d775-108">이 옵션을 사용 하면 고객의 Azure 지출를 해당 월의 예산과 비교할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="0d775-109">또한 고객은 자신의 Azure 지출에 대 한 비용을 청구 하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="0d775-110">이 기능은 샌드박스 또는 프로덕션 (TIP) 계정의 테스트에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="0d775-111">[고객에 대 한 Azure 지출 예산을 설정한](#set-azure-spending-budget)후에는 다음과 같은 방법으로 고객 사용량을 검토할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="0d775-112">이러한 옵션은 잘못 구성 된 서비스 또는 사기 행위를 제안할 수 있는 비정상적인 추세를 찾는 데 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="0d775-113">그런 다음 고객을 사용 하 여 근본 원인을 파악 하 고 비용을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="0d775-114">필요한 경우 [고객의 예산을](#set-azure-spending-budget) 더 높은 값으로 변경할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="0d775-115">현재 Azure 지출 확인</span><span class="sxs-lookup"><span data-stu-id="0d775-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="0d775-116">고객의 예산이 예산 제한에 근접 한 경우에 대 한 전자 메일 알림 설정</span><span class="sxs-lookup"><span data-stu-id="0d775-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="0d775-117">사용량 기반 구독에 대해 서비스 별로 항목별 비용 보기</span><span class="sxs-lookup"><span data-stu-id="0d775-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="0d775-118">또한 언제 든 지 고객에 대 한 [Azure 지출 예산을 제거할](#remove-azure-spending-budget) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="0d775-119">Azure 지출 데이터</span><span class="sxs-lookup"><span data-stu-id="0d775-119">Azure spending data</span></span>

<span data-ttu-id="0d775-120">Azure 지출 데이터는 *예상치* 이며 *실제 청구 금액은 다를 수 있습니다*.</span><span class="sxs-lookup"><span data-stu-id="0d775-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="0d775-121">데이터 값에는 세금, 크레딧, 조정 또는 적용 될 수 있는 기타 요금이 *반영 되지 않습니다* .</span><span class="sxs-lookup"><span data-stu-id="0d775-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="0d775-122">지출 데이터는 *하루에 한 번 새로 고쳐집니다*.</span><span class="sxs-lookup"><span data-stu-id="0d775-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="0d775-123">Azure Portal에서 계정 설정을 변경 하지 않는 한 고객은 Azure 서비스 및 리소스에 대 한 사용을 계속 하 고 요금이 부과 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="0d775-124">Azure 지출 예산 설정</span><span class="sxs-lookup"><span data-stu-id="0d775-124">Set Azure spending budget</span></span>

<span data-ttu-id="0d775-125">파트너 센터에서 여러 고객에 대 한 *월간 Azure 지출 예산을 설정할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="0d775-126">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0d775-127">**CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0d775-128">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 설정 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="0d775-129">**월별 예산** 에 대 한 값을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="0d775-130">**적용** 을 선택 하 여 변경 내용을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="0d775-131">구독 설정에서 *개별 고객에 대 한 예산을 설정할* 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="0d775-132">파트너 센터 대시보드에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="0d775-133">**CSP** 의 왼쪽 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="0d775-134">**고객** 페이지에서 고객의 **회사 이름을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="0d775-135">고객의 **구독** 페이지의 **사용량 기반 구독** 에서 **예산 변경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="0d775-136">예산 값을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="0d775-137">**적용** 을 선택 하 여 변경 내용을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="0d775-138">Azure 지출 예산 제거</span><span class="sxs-lookup"><span data-stu-id="0d775-138">Remove Azure spending budget</span></span>

<span data-ttu-id="0d775-139">파트너 센터에서 고객에 대 한 *월간 Azure 지출 예산을 제거할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="0d775-140">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0d775-141">**CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0d775-142">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 제거 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="0d775-143">**예산 제거** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="0d775-144">현재 Azure 지출 확인</span><span class="sxs-lookup"><span data-stu-id="0d775-144">Check current Azure spending</span></span>

<span data-ttu-id="0d775-145">언제 든 지 *고객의 현재 Azure 지출 및 월별 예산을 추적할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="0d775-146">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0d775-147">**CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0d775-148">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 고객의 월간 예산, 현재 지출 예상 및 사용 된 예산 백분율에 대 한 개요를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="0d775-149">예산 제한에 대 한 알림</span><span class="sxs-lookup"><span data-stu-id="0d775-149">Notifications for budget limits</span></span>

<span data-ttu-id="0d775-150">고객의 월간 지출을 예산 제한에 근접 한 경우에 대 한 *전자 메일 알림을 켤* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="0d775-151">이 옵션을 켜면 고객이 매월 예산 중 80% 이상을 사용할 때 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="0d775-152">이 옵션을 사용 하면 Azure 청구서에 대 한 정보를 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="0d775-153">전자 메일 알림을 구성 하려면:</span><span class="sxs-lookup"><span data-stu-id="0d775-153">To configure email notifications:</span></span>

1. <span data-ttu-id="0d775-154">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="0d775-155">**설정** 으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="0d775-156">**내 기본 설정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="0d775-157">없는 경우 기본 설정 전자 메일 주소를 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="0d775-158">알림의 기본 설정 언어를 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="0d775-159">**알림 기본 설정** 섹션에서 **CSP** 탭을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="0d775-160">**Azure 지출** 알림에 대 한 전자 메일 옵션을 확인 하 고 **저장** 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="0d775-161">서비스 별로 항목별 비용</span><span class="sxs-lookup"><span data-stu-id="0d775-161">Itemized costs by service</span></span>

<span data-ttu-id="0d775-162">*사용량 기반 구독에 대해 서비스 별로 항목별 비용 (및 예상 사용량)을 볼* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="0d775-163">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="0d775-164">**CSP** 의 왼쪽 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="0d775-165">**고객** 페이지에서 고객의 **회사 이름을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="0d775-166">고객의 **구독** 페이지의 **사용량 기반 구독** 에서 **구독의** 이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="0d775-167">구독 페이지에서 서비스 별로 **항목별 비용** 및 현재 달의 **예상 사용량** 을 검토할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d775-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="0d775-168">다음 단계</span><span class="sxs-lookup"><span data-stu-id="0d775-168">Next steps</span></span>

- [<span data-ttu-id="0d775-169">CSP의 새로운 상거래 환경 - Azure 청구</span><span class="sxs-lookup"><span data-stu-id="0d775-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
