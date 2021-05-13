---
title: 고객에 대한 Azure 지출 예산 설정
ms.topic: how-to
ms.date: 03/17/2021
description: 고객에 대한 월간 Azure 지출 예산을 설정하거나 제거하는 방법과 Azure 지출 데이터를 보고 예산 관련 알림을 설정하는 방법을 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855355"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="bdd8f-103">파트너 센터 고객에 대한 월간 Azure 지출 예산 설정, 확인 또는 제거</span><span class="sxs-lookup"><span data-stu-id="bdd8f-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="bdd8f-104">**적절한 역할:** 관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="bdd8f-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="bdd8f-105">파트너 센터 [고객에 대한 월간 Azure 지출 예산을 설정할](#set-azure-spending-budget) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="bdd8f-106">이렇게 하면 고객이 Azure 지출을 관리하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="bdd8f-107">이 옵션을 사용하면 고객의 Azure 지출을 해당 월의 예산과 비교할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="bdd8f-108">또한 월별 청구서가 예상보다 높지 않도록 고객이 Azure 지출을 예산으로 책정하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="bdd8f-109">이 기능은 샌드박스 또는 TIP(프로덕션에서 테스트) 계정에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="bdd8f-110">[고객에 대한 Azure 지출 예산을 설정한](#set-azure-spending-budget)후 다음과 같은 방법으로 고객 사용량을 검토할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="bdd8f-111">이러한 옵션은 잘못 구성된 서비스 또는 사기 행위가 발생할 수 있는 비정상적인 추세를 파악하는 데 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="bdd8f-112">그런 다음 고객과 협력하여 근본 원인을 파악하고 비용을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="bdd8f-113">필요한 경우 고객의 [예산을](#set-azure-spending-budget) 더 높은 금액으로 변경할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="bdd8f-114">현재 Azure 지출 확인</span><span class="sxs-lookup"><span data-stu-id="bdd8f-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="bdd8f-115">고객의 지출이 예산 한도에 근접하는 경우에 대한 이메일 알림을 켭니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="bdd8f-116">사용량 기반 구독에 대한 서비스별 항목별 비용 보기</span><span class="sxs-lookup"><span data-stu-id="bdd8f-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="bdd8f-117">언제든지 [고객에](#remove-azure-spending-budget) 대한 Azure 지출 예산을 제거할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="bdd8f-118">Azure 지출 데이터</span><span class="sxs-lookup"><span data-stu-id="bdd8f-118">Azure spending data</span></span>

<span data-ttu-id="bdd8f-119">Azure 지출 데이터는 *예상* 금액이며 *실제 청구 금액은 달라질 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="bdd8f-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="bdd8f-120">데이터 값은 세금, 크레딧, 조정 또는 적용할 수 있는 기타 요금을 *반영하지 않습니다.*</span><span class="sxs-lookup"><span data-stu-id="bdd8f-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="bdd8f-121">지출 데이터는 *하루에 한 번 새로 고쳐집니다.*</span><span class="sxs-lookup"><span data-stu-id="bdd8f-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="bdd8f-122">Azure Portal에서 계정 설정을 변경 하지 않는 한 고객은 Azure 서비스 및 리소스에 대 한 사용을 계속 하 고 요금이 부과 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="bdd8f-123">Azure 지출 예산 설정</span><span class="sxs-lookup"><span data-stu-id="bdd8f-123">Set Azure spending budget</span></span>

<span data-ttu-id="bdd8f-124">파트너 센터에서 여러 고객에 대 한 *월간 Azure 지출 예산을 설정할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="bdd8f-125">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bdd8f-126">**CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="bdd8f-127">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 설정 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="bdd8f-128">**월별 예산** 에 대 한 값을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="bdd8f-129">**적용** 을 선택 하 여 변경 내용을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="bdd8f-130">구독 설정에서 *개별 고객에 대 한 예산을 설정할* 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="bdd8f-131">파트너 센터 대시보드에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="bdd8f-132">**CSP** 의 왼쪽 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="bdd8f-133">**고객** 페이지에서 고객의 **회사 이름을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="bdd8f-134">고객의 **구독** 페이지의 **사용량 기반 구독** 에서 **예산 변경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="bdd8f-135">예산 값을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="bdd8f-136">**적용** 을 선택 하 여 변경 내용을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="bdd8f-137">Azure 지출 예산 제거</span><span class="sxs-lookup"><span data-stu-id="bdd8f-137">Remove Azure spending budget</span></span>

<span data-ttu-id="bdd8f-138">파트너 센터에서 고객에 대 한 *월간 Azure 지출 예산을 제거할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="bdd8f-139">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bdd8f-140">**CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="bdd8f-141">**Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 제거 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="bdd8f-142">**예산 제거** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="bdd8f-143">현재 Azure 지출 확인</span><span class="sxs-lookup"><span data-stu-id="bdd8f-143">Check current Azure spending</span></span>

<span data-ttu-id="bdd8f-144">언제 든 지 *고객의 현재 Azure 지출 및 월별 예산을 추적할* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="bdd8f-145">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bdd8f-146">**CSP** 아래의 왼쪽 메뉴에서 **Azure 지출을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="bdd8f-147">Azure **지출** 페이지의 Microsoft Azure **구독이 있는 고객** 아래에서 고객의 월별 예산 개요, 현재 지출 예측 및 사용된 예산의 백분율을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="bdd8f-148">예산 한도에 대한 알림</span><span class="sxs-lookup"><span data-stu-id="bdd8f-148">Notifications for budget limits</span></span>

<span data-ttu-id="bdd8f-149">고객의 월별 *지출이* 예산 한도에 근접하는 경우에 대한 이메일 알림을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="bdd8f-150">이 옵션을 켜면 고객이 월간 예산의 80% 이상을 사용할 때 알림이 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="bdd8f-151">이 옵션을 사용하면 Azure 청구서를 계속 감시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="bdd8f-152">이메일 알림을 구성하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-152">To configure email notifications:</span></span>

1. <span data-ttu-id="bdd8f-153">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="bdd8f-154">**설정** 으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="bdd8f-155">**내 기본 설정을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="bdd8f-156">기본 설정 이메일 주소를 구성하지 않은 경우 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="bdd8f-157">알림에 대한 기본 설정 언어를 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="bdd8f-158">알림 기본 설정 섹션에서 **CSP** **탭을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="bdd8f-159">**Azure 지출** 알림에 대한 이메일 옵션을 확인하고 **을 저장합니다.**</span><span class="sxs-lookup"><span data-stu-id="bdd8f-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="bdd8f-160">서비스별 항목별 비용</span><span class="sxs-lookup"><span data-stu-id="bdd8f-160">Itemized costs by service</span></span>

<span data-ttu-id="bdd8f-161">*사용량 기반 구독에 대한 서비스별로 항목별 비용(및 예상 사용량)을 볼* 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="bdd8f-162">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="bdd8f-163">**CSP** 아래의 왼쪽 메뉴에서 **고객을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="bdd8f-164">**고객** 페이지에서 고객의 **회사 이름** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="bdd8f-165">고객의 **구독** 페이지의 **사용량 기반 구독에서 구독의** 이름을 선택합니다. </span><span class="sxs-lookup"><span data-stu-id="bdd8f-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="bdd8f-166">구독 페이지에서 서비스별 **항목별 비용** 및 이번 달의 **예상 사용량을** 검토할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bdd8f-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="bdd8f-167">다음 단계</span><span class="sxs-lookup"><span data-stu-id="bdd8f-167">Next steps</span></span>

- [<span data-ttu-id="bdd8f-168">CSP의 새로운 상거래 환경 - Azure 청구</span><span class="sxs-lookup"><span data-stu-id="bdd8f-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
