---
title: 고객에 대 한 Azure 예약 관리
description: 예약을 취소 하거나, 예약을 교환 하거나, 환불을 요청 하는 방법을 비롯 하 여 고객에 대 한 Azure 예약을 관리 하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: c377fca3e38161258c836d14202ac4db21484526
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534763"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a><span data-ttu-id="25827-103">고객에 대 한 Microsoft Azure 예약 관리, 취소, 교환 또는 환불</span><span class="sxs-lookup"><span data-stu-id="25827-103">Manage, cancel, exchange, or refund Microsoft Azure reservations for customers</span></span>

<span data-ttu-id="25827-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="25827-104">**Appropriate roles**</span></span>

- <span data-ttu-id="25827-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="25827-105">Admin agent</span></span>
- <span data-ttu-id="25827-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="25827-106">Global admin</span></span>
- <span data-ttu-id="25827-107">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="25827-107">Helpdesk agent</span></span>
- <span data-ttu-id="25827-108">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="25827-108">Sales agent</span></span>
- <span data-ttu-id="25827-109">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="25827-109">User management admin</span></span>

<span data-ttu-id="25827-110">이 문서에서는 예약을 취소 하거나, 예약을 교환 하거나, 환불을 요청 하는 방법을 비롯 하 여 고객에 대 한 Azure 예약을 관리 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-110">This article explains how to manage Azure reservations for a customer, including how to cancel a reservation, exchange a reservation, or request a refund.</span></span>

> [!NOTE]
> <span data-ttu-id="25827-111">이 문서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너에만 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="25827-111">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="25827-112">다른 유형의 구독 (예: 종 량 제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용 하는 고객은 [이 Azure 예약 설명서](/azure/cost-management-billing/reservations)를 대신 읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-112">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="25827-113">고객의 Azure 예약 사후 구매를 관리 하려면 파트너 센터에서 관리 하려는 고객 및 예약을 선택한 다음 Azure Portal 예약을 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-113">To manage your customers' Azure reservations post-purchase, you'll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal.</span></span>

1. <span data-ttu-id="25827-114">시작 하려면 파트너 센터 메뉴에서 **고객** 을 선택 하 고 해당 예약을 관리 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-114">To get started, select **Customers** from the Partner Center menu and then select the customer whose reservations you want to manage.</span></span> 

2. <span data-ttu-id="25827-115">고객의 세부 정보 페이지 메뉴에서 **Azure 예약** 을 선택 하 고 관리 하려는 특정 예약을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-115">On the customer's detail page menu, select **Azure reservations** and then select the specific reservation you want to manage.</span></span>  

3. <span data-ttu-id="25827-116">**작업** 아래에서 **관리** 를 선택 하 여 Azure Portal에서 고객의 예약 레코드로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-116">Under **Actions**, select **Manage** to go to the customer's reservation record in the Azure portal.</span></span> <span data-ttu-id="25827-117">예약 세부 정보 페이지에서 다음 단계를 수행 하 여 작업을 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-117">On the reservation detail page, follow the steps below to complete tasks.</span></span>  

    | <span data-ttu-id="25827-118">**Select**</span><span class="sxs-lookup"><span data-stu-id="25827-118">**Select**</span></span>   | <span data-ttu-id="25827-119">**수행할 작업**</span><span class="sxs-lookup"><span data-stu-id="25827-119">**To**</span></span>    |
    |:-----------------------------|:-----------------|
    | <span data-ttu-id="25827-120">**개요**</span><span class="sxs-lookup"><span data-stu-id="25827-120">**Overview**</span></span>   | <span data-ttu-id="25827-121">만료 날짜, 범위 및 사용률 데이터를 포함 하 여 고객 예약의 세부 정보를 봅니다.</span><span class="sxs-lookup"><span data-stu-id="25827-121">View details of a customer's reservation, including expiration date, scope, and utilization data.</span></span> <span data-ttu-id="25827-122">**참고** **환불** 을 선택 하 여 등급이 지정 된 환불에 대 한 지원 요청을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="25827-122">**NOTE** Select **Refund** to create a support request for a pro-rated refund.</span></span> <span data-ttu-id="25827-123">예약 기간 중 사용 되지 않은 부분을 교환 하는 지원 요청을 만들려면 **exchange** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-123">Select **Exchange** to create a support request to exchange the unused portion of your reservation term.</span></span>  
    | <span data-ttu-id="25827-124">**Access Control (IAM)**</span><span class="sxs-lookup"><span data-stu-id="25827-124">**Access Control (IAM)**</span></span>   | <span data-ttu-id="25827-125">고객의 예약 정보에 대 한 액세스를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-125">Manage access to the customer's reservation information.</span></span>|
    | <span data-ttu-id="25827-126">**Configuration**</span><span class="sxs-lookup"><span data-stu-id="25827-126">**Configuration**</span></span>   | <span data-ttu-id="25827-127">예약의 범위 및/또는 예약에 연결 된 Azure 구독을 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-127">Change the reservation's scope and/or the Azure subscription the reservation is associated with.</span></span>    |
    | <span data-ttu-id="25827-128">**속성**</span><span class="sxs-lookup"><span data-stu-id="25827-128">**Properties**</span></span>   | <span data-ttu-id="25827-129">예약의 속성을 보고 예약 ID 및 예약 주문 ID를 클립보드로 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-129">View the reservation's properties and copy to the clipboard the reservation ID and reservation order ID.</span></span> <span data-ttu-id="25827-130">**참고** 고객을 대신 하 여 지원을 요청할 때 지원에서 예약 ID 및 예약 주문 ID를 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-130">**NOTE** Support may ask you for the reservation ID and reservation order ID when you request support on behalf of a customer.</span></span>    |
    | <span data-ttu-id="25827-131">**새 지원 요청**</span><span class="sxs-lookup"><span data-stu-id="25827-131">**New support request**</span></span>    | <span data-ttu-id="25827-132">Microsoft 지원에서 도움을 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-132">Request help from Microsoft Support.</span></span>   |
 
## <a name="cancel-or-exchange-a-reservation"></a><span data-ttu-id="25827-133">예약 취소 또는 교환</span><span class="sxs-lookup"><span data-stu-id="25827-133">Cancel or exchange a reservation</span></span>

<span data-ttu-id="25827-134">언제 든 지 고객의 비즈니스 요구 사항이 변경 되 면 예약을 취소 하 고 환불을 받을 수 있으며 새 예약 가격에 사용 될 예약의 비례 상환 금액을 교환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-134">If at any point a customer's business needs change, they may want to cancel a reservation and get a refund or exchange a reservation's prorated refund amount to be used toward the price of a new reservation.</span></span>

<span data-ttu-id="25827-135">이러한 두 시나리오에서 Microsoft는 고객에 게 환불 된 재무 거래를 관리할 수 있도록 용량을 자동으로 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-135">In both of these scenarios, Microsoft refunds the amount to you so that you can then manage the resulting financial transactions with your customers.</span></span> <span data-ttu-id="25827-136">Microsoft는 대금 청구, 취소 또는 환불에 대해 직접 고객에 게 연락 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-136">Microsoft does not contact customers directly about billing, cancellations, or refunds.</span></span>

### <a name="how-cancellations-work"></a><span data-ttu-id="25827-137">취소 작업 방법</span><span class="sxs-lookup"><span data-stu-id="25827-137">How cancellations work</span></span>

<span data-ttu-id="25827-138">고객은 언제 든 지 예약을 취소 하도록 요청할 수 있습니다 (환불 금액은 연간 $5만).</span><span class="sxs-lookup"><span data-stu-id="25827-138">Customers can request to cancel a reservation at any time (refund amount capped at $50,000 per year).</span></span> <span data-ttu-id="25827-139">예약을 취소 하면 고객이 조기 종료 요금으로 Azure 예약의 남은 개월 수를 반환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-139">Canceling a reservation allows the customer to return the amount of the remaining months of an Azure reservation for an early termination fee.</span></span> <span data-ttu-id="25827-140">초기 종료 수수료를 제외 하 고 남은 비례 잔액은 사용자 계정에 환불 고객의 계정을 환불 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-140">The remaining prorated balance, minus the early termination fee, is refunded to your account so that you can refund the customer's account.</span></span> 

<span data-ttu-id="25827-141">취소 세부 정보 및 수수료는 아래를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="25827-141">See below for cancellation details and fees.</span></span>


|<span data-ttu-id="25827-142">**취소 날짜**</span><span class="sxs-lookup"><span data-stu-id="25827-142">**Cancellation date**</span></span><br> <span data-ttu-id="25827-143">일별로</span><span class="sxs-lookup"><span data-stu-id="25827-143">(days)</span></span>   |<span data-ttu-id="25827-144">**사용법**</span><span class="sxs-lookup"><span data-stu-id="25827-144">**Usage**</span></span>    |<span data-ttu-id="25827-145">**크레딧**</span><span class="sxs-lookup"><span data-stu-id="25827-145">**Credit**</span></span>  |<span data-ttu-id="25827-146">**조기 종료**</span><span class="sxs-lookup"><span data-stu-id="25827-146">**Early termination**</span></span><br> <span data-ttu-id="25827-147">수수료</span><span class="sxs-lookup"><span data-stu-id="25827-147">fee</span></span>    |<span data-ttu-id="25827-148">**환불 캡**</span><span class="sxs-lookup"><span data-stu-id="25827-148">**Refund cap**</span></span> | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|<span data-ttu-id="25827-149">5 개 미만</span><span class="sxs-lookup"><span data-stu-id="25827-149">5 or fewer</span></span>                         | <span data-ttu-id="25827-150">아니요</span><span class="sxs-lookup"><span data-stu-id="25827-150">No</span></span>          | <span data-ttu-id="25827-151">100%</span><span class="sxs-lookup"><span data-stu-id="25827-151">100%</span></span>       | <span data-ttu-id="25827-152">아니요</span><span class="sxs-lookup"><span data-stu-id="25827-152">No</span></span>                              | <span data-ttu-id="25827-153">$5만 USD</span><span class="sxs-lookup"><span data-stu-id="25827-153">$50,000 USD</span></span>   |
|<span data-ttu-id="25827-154">5 개 미만</span><span class="sxs-lookup"><span data-stu-id="25827-154">5 or fewer</span></span>                         | <span data-ttu-id="25827-155">예</span><span class="sxs-lookup"><span data-stu-id="25827-155">Yes</span></span>         | <span data-ttu-id="25827-156">전문 등급</span><span class="sxs-lookup"><span data-stu-id="25827-156">Pro-rated</span></span>  | <span data-ttu-id="25827-157">아니요</span><span class="sxs-lookup"><span data-stu-id="25827-157">No</span></span>                              | <span data-ttu-id="25827-158">$5만 USD</span><span class="sxs-lookup"><span data-stu-id="25827-158">$50,000 USD</span></span>   |
|<span data-ttu-id="25827-159">5 개 이상</span><span class="sxs-lookup"><span data-stu-id="25827-159">More than 5</span></span>                        | <span data-ttu-id="25827-160">아니요</span><span class="sxs-lookup"><span data-stu-id="25827-160">No</span></span>          | <span data-ttu-id="25827-161">전문 등급</span><span class="sxs-lookup"><span data-stu-id="25827-161">Pro-rated</span></span>  | <span data-ttu-id="25827-162">12%</span><span class="sxs-lookup"><span data-stu-id="25827-162">12%</span></span>                             | <span data-ttu-id="25827-163">$5만 USD</span><span class="sxs-lookup"><span data-stu-id="25827-163">$50,000 USD</span></span>   |
|<span data-ttu-id="25827-164">5 개 이상</span><span class="sxs-lookup"><span data-stu-id="25827-164">More than 5</span></span>                        | <span data-ttu-id="25827-165">예</span><span class="sxs-lookup"><span data-stu-id="25827-165">Yes</span></span>         | <span data-ttu-id="25827-166">전문 등급</span><span class="sxs-lookup"><span data-stu-id="25827-166">Pro-rated</span></span>  | <span data-ttu-id="25827-167">12%</span><span class="sxs-lookup"><span data-stu-id="25827-167">12%</span></span>                             | <span data-ttu-id="25827-168">$5만 USD</span><span class="sxs-lookup"><span data-stu-id="25827-168">$50,000 USD</span></span>   |

### <a name="how-exchanges-work"></a><span data-ttu-id="25827-169">교환 작동 방법</span><span class="sxs-lookup"><span data-stu-id="25827-169">How exchanges work</span></span> 

<span data-ttu-id="25827-170">고객이 원래 구매한 사용자와 다른 예약을 구입 하려는 경우 exchange를 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-170">If a customer wants to buy a different reservation than the one they originally bought from you, they can request an exchange.</span></span> <span data-ttu-id="25827-171">예약을 교환 하면 고객이 새 예약 가격에 비례하여 비례 하는 환불 금액을 사용할 수 있으므로 예약을 취소 하는 것이 좋은 대안이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-171">Exchanging a reservation can be an attractive alternative to canceling a reservation because it allows the customer to use the prorated refund amount toward the price of the new reservation.</span></span> 

<span data-ttu-id="25827-172">고객에 게 exchange를 제공할 수 있도록 비례 하는 환불 금액은 계정에 제공한 됩니다.</span><span class="sxs-lookup"><span data-stu-id="25827-172">The prorated refund amount is credited to your account so that you can offer the customer an exchange.</span></span>

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a><span data-ttu-id="25827-173">고객을 대신 하 여 환불 또는 교환 요청</span><span class="sxs-lookup"><span data-stu-id="25827-173">Request a refund or exchange on behalf of a customer</span></span>

<span data-ttu-id="25827-174">고객을 대신 하 여 환불 또는 교환에 대 한 지원 요청을 파일 하려면 파트너 센터에서 고객 및 예약을 선택한 후 Azure Portal에서 지원 요청을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="25827-174">To file a support request for a refund or exchange on behalf of your customers, you'll select the customer and reservation in Partner Center, and then create the support request in the Azure portal.</span></span> 

>[!NOTE]
><span data-ttu-id="25827-175">Microsoft 지원 에이전트에서 예약 ID 및 예약 주문 ID를 제공 하도록 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-175">Microsoft Support agents may ask you to provide the reservation ID and reservation order ID.</span></span> <span data-ttu-id="25827-176">이 정보는 Azure Portal의 예약 **속성** 페이지에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25827-176">You can find this information on the reservation's **Properties** page in the Azure portal.</span></span>

1. <span data-ttu-id="25827-177">시작 하려면 파트너 센터 메뉴에서 **고객** 을 선택한 다음 환불 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-177">To get started, select **Customers** from the Partner Center menu and then select the customer who wants a refund.</span></span> 

2. <span data-ttu-id="25827-178">고객의 세부 정보 페이지에서 **Azure 예약** 을 선택한 후 고객이 환불 하려는 특정 예약을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-178">On the customer's detail page, select **Azure reservations** and then select the specific reservation the customer wants refunded.</span></span>  

3. <span data-ttu-id="25827-179">**작업** 에서 **환불** 을 선택 하 여 Azure Portal에서 고객의 예약 레코드로 이동 하 고 지원 요청을 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-179">Under **Actions**, select **Refund** to go to the customer's reservation record in the Azure portal and initiate a support request.</span></span>  

4. <span data-ttu-id="25827-180">**새 지원 요청** 페이지에서 아래 단계를 수행 하 여 환불을 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-180">On the **New support request** page, follow the steps below to request a refund.</span></span> <span data-ttu-id="25827-181">각 단계 후에 **다음** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-181">Select **Next** after each step.</span></span> 

   |<span data-ttu-id="25827-182">**Step**</span><span class="sxs-lookup"><span data-stu-id="25827-182">**Step**</span></span>                    |<span data-ttu-id="25827-183">**선택할**</span><span class="sxs-lookup"><span data-stu-id="25827-183">**Selections**</span></span>    |
   |:---------------------------|:-----------------|
   |<span data-ttu-id="25827-184">**1 기본 사항**</span><span class="sxs-lookup"><span data-stu-id="25827-184">**1 Basics**</span></span>                |<span data-ttu-id="25827-185">문제 유형: 청구</span><span class="sxs-lookup"><span data-stu-id="25827-185">Issue type: Billing.</span></span>  |
   |<span data-ttu-id="25827-186">**2 문제**</span><span class="sxs-lookup"><span data-stu-id="25827-186">**2 Problem**</span></span>               |<span data-ttu-id="25827-187">문제 유형: 예약 관리.</span><span class="sxs-lookup"><span data-stu-id="25827-187">Problem type: Reservation management.</span></span> <span data-ttu-id="25827-188">범주: 교환 및 환불.</span><span class="sxs-lookup"><span data-stu-id="25827-188">Category: Exchanges and refunds.</span></span> |
   |<span data-ttu-id="25827-189">**3 연락처 정보**</span><span class="sxs-lookup"><span data-stu-id="25827-189">**3 Contact information**</span></span>   |<span data-ttu-id="25827-190">기본 설정을 선택 하 고 필요한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-190">Select your preferences and enter the required information.</span></span> 

5. <span data-ttu-id="25827-191">완료되면 **만들기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-191">Select **Create** when done.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="25827-192">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="25827-192">Azure reservations resources</span></span>

|<span data-ttu-id="25827-193">**원하는 정보**</span><span class="sxs-lookup"><span data-stu-id="25827-193">**For information about**</span></span>   |<span data-ttu-id="25827-194">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="25827-194">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="25827-195">CSP의 Azure 예약 개요</span><span class="sxs-lookup"><span data-stu-id="25827-195">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="25827-196">Microsoft Azure 예약 인스턴스 판매</span><span class="sxs-lookup"><span data-stu-id="25827-196">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="25827-197">파트너 센터에서 고객에 대 한 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="25827-197">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="25827-198">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="25827-198">Buy Azure reservations</span></span>](azure-reservations-buying.md) |
|<span data-ttu-id="25827-199">올바른 VM 크기를 확인 하 고 고객 VM 사용 확인</span><span class="sxs-lookup"><span data-stu-id="25827-199">Determine the correct VM size and verify customer VM usage</span></span>   | [<span data-ttu-id="25827-200">최대 Azure 예약 사용에 대 한 VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="25827-200">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="25827-201">파트너 센터 API를 사용 하 여 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="25827-201">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="25827-202">파트너 센터 개발자 설명서에서 [Azure Reserved VM Instances 구매](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="25827-202">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="25827-203">구매한 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="25827-203">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="25827-204">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="25827-204">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |