---
title: Azure 계획의 Azure 구독을 다른 CSP 파트너에 게 전송
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure 요금제에서 고객의 Azure 구독과 연결 된 클라우드 솔루션 공급자 프로그램 파트너를 변경 하는 방법에 대해 알아봅니다.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/13/2020
ms.locfileid: "91980264"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="1e5e4-103">고객의 Azure 계획 구독을 다른 파트너에 게 전송</span><span class="sxs-lookup"><span data-stu-id="1e5e4-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

## <a name="applies-to"></a><span data-ttu-id="1e5e4-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="1e5e4-104">Applies to</span></span>

- <span data-ttu-id="1e5e4-105">CSP(클라우드 솔루션 공급자) 프로그램의 파트너</span><span class="sxs-lookup"><span data-stu-id="1e5e4-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="1e5e4-106">이 문서에서는 고객이 Azure 계획을 통해 azure 구독을 한 클라우드 솔루션 공급자 (CSP)에서 다른 클라우드 솔루션 공급자로 전환할 수 있는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="1e5e4-107">다른 파트너에서 고객의 Azure 구독을 전환 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="1e5e4-108">파트너와 고객 모두 완료 하는 단계가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="1e5e4-109">Microsoft와 직접 청구 관계가 있는 파트너만 전환 도구에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="1e5e4-110">간접 재판매인은 간접 공급자와 협력 하 여이 전환 도구를 활용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="1e5e4-111">이 도구를 사용 하기 전에 고객은 파트너 (현재 및 미래)를 모두 사용 하 여 대화에 속해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="1e5e4-112">혼동 및 변동 방지를 방지 하려면 오프 라인 대화를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="1e5e4-113">또한 파트너와 고객은 전환을 시작 하기 전에 이러한 고려 사항 및 필수 구성 요소를 이해 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="1e5e4-114">**주요 고려 사항:**</span><span class="sxs-lookup"><span data-stu-id="1e5e4-114">**Key considerations:**</span></span>

- <span data-ttu-id="1e5e4-115">Azure Reservations는 이후 파트너에 대 한 구독과 함께 이동 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="1e5e4-116">현재 파트너의 Azure 서비스에 대 한 CSP 가격은 전환 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="1e5e4-117">고객에 대 한 지원 책임이 이후 파트너로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="1e5e4-118">전송 시 청구 및 청구는 이후 파트너로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="1e5e4-119">Azure Role-Based Access Control (RBAC)는 전송의 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="1e5e4-120">(AOBO)를 대신 하 여 관리자는 이후 파트너에 게 기본적으로 부여 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="1e5e4-121">타사 marketplace 제품은 제품이 Marketplace 자격 검사를 통과 하는 동안 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="1e5e4-122">특별 한 할인이 나 지역 제한은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="1e5e4-123">제품이 비등록 기반입니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="1e5e4-124">이후 파트너는 게시자와 협력 하 여 제품 배포에 대 한 허용 목록에 있는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="1e5e4-125">Marketplace 제품을 전송 하기 위해 이러한 조건을 모두 충족 하지 않는 경우 Azure 구독을 전송 하 고 새 파트너와 마켓플레이스 제품을 다시 구매 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="1e5e4-126">**사전 요구 사항:**</span><span class="sxs-lookup"><span data-stu-id="1e5e4-126">**Prerequisites:**</span></span>

- <span data-ttu-id="1e5e4-127">고객은 자신의 의도에 따라 현재 CSP 파트너를 전환 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="1e5e4-128">향후 CSP 파트너는 고객과 협력 하 여 고객의 요구 사항을 충족할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="1e5e4-129">이후 CSP 파트너가 전환 시작 전에 고객과의 관계를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="1e5e4-130">고객이 향후 CSP 파트너와 Microsoft 고객 계약에 서명 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="1e5e4-131">이 도구를 사용 하려면 향후 CSP 파트너가 Microsoft 파트너 계약에 서명 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="1e5e4-132">완료할 고객 작업</span><span class="sxs-lookup"><span data-stu-id="1e5e4-132">Customer tasks to be completed</span></span>

<span data-ttu-id="1e5e4-133">Azure 계획에 따라 Azure 구독을 전송 하려면 고객이 현재 파트너에 게 연락 하 여 프로세스를 시작 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="1e5e4-134">현재 파트너의 회사 이름 및 도메인을 수집 하 여 이후 파트너가 전송 요청 양식을 대신 완료할 수 있도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="1e5e4-135">또한 고객은 현재 파트너 로부터 전송 하려는 구독을 식별 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="1e5e4-136">Office 365, Enterprise Mobility Suite 또는 Microsoft Dynamics CRM 구독의 파트너를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="1e5e4-137">전송 프로세스를 시작 하는 전송 요청 양식을 완료 하는 것은 향후 파트너의 책임입니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="1e5e4-138">Microsoft는 고객 또는 현재 파트너를 대신 하 여 개입 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="1e5e4-139">고객은 이후 및 현재 파트너와 긴밀 하 게 협력 하 여 전환을 원활 하 게 진행할 수 있도록 계획 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="1e5e4-140">완료할 이후 파트너 작업</span><span class="sxs-lookup"><span data-stu-id="1e5e4-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="1e5e4-141">이후 구독 파트너는 파트너 센터에서 전송 요청 양식을 완료 하 여 구독 전송을 요청 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="1e5e4-142">파트너 센터 메뉴에서 **고객**을 선택한 다음 대신 전송 요청 양식을 완료 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="1e5e4-143">고객 메뉴에서 **구독**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="1e5e4-144">**전송 요청** 섹션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="1e5e4-145">**전송 요청 섹션**에서 **새 요청 추가**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="전송 섹션":::

5.  <span data-ttu-id="1e5e4-147">**새 전송 요청** 양식을 작성 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="1e5e4-148">**전송 전송 요청**  >  **보내기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="전송 섹션":::

7.  <span data-ttu-id="1e5e4-150">전송 요청 확인 검토</span><span class="sxs-lookup"><span data-stu-id="1e5e4-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="전송 섹션":::

    >[!Note]
    ><span data-ttu-id="1e5e4-152">이후 파트너는 전송 요청 상태가 "보류 중" 인 경우에만 오른쪽 위 모서리에서 **요청 취소** 를 선택 하 여 전송 요청을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="1e5e4-153">전송 요청 상태가 "진행 중" 또는 "완료" 이면 취소가 가능 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="1e5e4-154">완료할 현재 파트너 작업</span><span class="sxs-lookup"><span data-stu-id="1e5e4-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="1e5e4-155">현재 파트너의 고객 관리 에이전트는 고객의 구독 전송을 요청 하는 전자 메일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="전송 섹션":::

<span data-ttu-id="1e5e4-157">파트너 센터에서 전송 요청 양식을 검토 하 고 수락 하 여 구독 이전을 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="1e5e4-158">현재 파트너가 30 일 내에 작업을 수행 하지 않으면 요청이 만료 되 고 이후 파트너는 새 전송 요청을 만들기 위한를 갖게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="1e5e4-159">전자 메일에서 **전송 요청 검토** 를 선택 하거나</span><span class="sxs-lookup"><span data-stu-id="1e5e4-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="1e5e4-160">파트너 센터 메뉴에서 **고객**을 선택한 다음를 대신 하 여 전송 요청을 제출 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="1e5e4-161">고객 메뉴에서 **구독**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="1e5e4-162">**전송 요청** 섹션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="1e5e4-163">**받은 요청** 에서 선택한 **전송 요청 ID** 를 선택 하 여 전송 정보를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="전송 섹션":::

5.  <span data-ttu-id="1e5e4-165">전송 요청을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-165">Review transfer request.</span></span> <span data-ttu-id="1e5e4-166">전송할 요청 된 Azure 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="1e5e4-167">계속 하기 전에 선택한 구독에 대 한 액세스 권한이 더 이상 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="1e5e4-168">추가 사용을 위해 송장이 청구 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="1e5e4-169">Azure 예약은 구독과 함께 전송 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="1e5e4-170">그런 다음 **수락 및 전송** 을 선택 하 여 전송 프로세스를 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="전송 섹션":::

7.  <span data-ttu-id="1e5e4-172">전송 승인 확인을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="1e5e4-173">이 시점에서 이후 파트너, 고객 및 현재 파트너는 전자 메일을 통해 수락 된 전송 요청에 대 한 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="1e5e4-174">이후 전환이 수락 되 면 시스템이 업데이트 되는 동안 최대 15 분 동안 보류 중 상태가 유지 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="1e5e4-175">시간이 더 오래 걸리면 시스템은 3 일 동안 계속 시도 하 게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="1e5e4-176">전송 상태가 여전히 보류 중으로 유지 되 면 파트너는 서비스 요청을 제출 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="1e5e4-177">전송이 완료 되 면 요청에 포함 된 구독이 향후 파트너의 Azure 계획에 표시 되며 더 이상 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="1e5e4-178">간접 공급자의 경우: 전송 요청이 수락 되었음을 간접 재판매인에 게 알려 주세요.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="1e5e4-179">전송 된 고객 구독 관리</span><span class="sxs-lookup"><span data-stu-id="1e5e4-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="1e5e4-180">Azure RBAC(역할 기반 액세스 제어)를 사용하여 할당된 기존 사용자, 그룹 또는 서비스 주체에 대한 액세스는 전환 중에 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="1e5e4-181">Azure [RBAC (](/azure/role-based-access-control/overview) 역할 기반 액세스 제어)를 통해 고객은 azure 리소스에 액세스할 수 있는 사용자, 해당 리소스에서 수행할 수 있는 작업 및 액세스할 수 있는 영역을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="1e5e4-182">새 파트너에 게는 구독 이전에 고객의 리소스에 대 한 RBAC 액세스 권한이 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="1e5e4-183">고객의 이전 파트너는 RBAC 액세스를 유지 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="1e5e4-184">고객에 게 문의 하 여 구독에 대 한 통찰력을 보유 하 고 있는 사람을 파악 하 고 원하는 변경 작업을 수행 하세요.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="1e5e4-185">따라서 고객이 이전 파트너에 대 한 Azure RBAC 액세스를 제거 하 고 새 파트너에 대 한 액세스를 추가 하는 것이 중요 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="1e5e4-186">고객이 새 액세스 권한을 부여 하는 방법에 대 한 자세한 내용은 [azure 역할 기반 액세스 제어 란? (AZURE RBAC)](/azure/role-based-access-control/overview) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="1e5e4-187">사용자가 이전 파트너의 RBAC 액세스를 제거 하는 방법에 대 한 자세한 내용은 [역할 할당 제거](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="1e5e4-188">또한 구독에 대 한 액세스 권한 [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 을 자동으로 가져오지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="1e5e4-189">AOBO는 파트너의 고객을 대신 하 여 고객의 Azure 구독을 관리 하는 데 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="1e5e4-190">Azure 권한에 대 한 자세한 내용은 [고객의 서비스 또는 구독을 관리할 수 있는 권한 얻기](./customers-revoke-admin-privileges.md) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="1e5e4-191">다음 단계:</span><span class="sxs-lookup"><span data-stu-id="1e5e4-191">Next steps:</span></span>

- [<span data-ttu-id="1e5e4-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="1e5e4-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="1e5e4-193">고객의 서비스 또는 구독을 관리할 수 있는 권한을 획득 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e5e4-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)