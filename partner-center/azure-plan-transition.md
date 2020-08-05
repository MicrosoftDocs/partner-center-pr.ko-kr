---
title: 현재 Azure 제품에서 Azure 플랜으로 고객 이동
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 파트너가 파트너 센터를 사용하여 Azure 플랜에서 기존 CSP Azure 제품에서 Azure 서비스로 고객을 이동하는 방법을 알아봅니다.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: bcc6534995a7550f0f09d1da2d52cbf676b66c40
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527509"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a><span data-ttu-id="fca52-103">기존 CSP Azure 제품에서 Azure 플랜으로 고객 전환</span><span class="sxs-lookup"><span data-stu-id="fca52-103">Transition customers to Azure plan from existing CSP Azure offers</span></span>

<span data-ttu-id="fca52-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="fca52-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fca52-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="fca52-105">Admin agent</span></span>
- <span data-ttu-id="fca52-106">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="fca52-106">Billing admin</span></span>
- <span data-ttu-id="fca52-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="fca52-107">Global admin</span></span>
- <span data-ttu-id="fca52-108">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="fca52-108">Helpdesk agent</span></span>
- <span data-ttu-id="fca52-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="fca52-109">Sales agent</span></span>
- <span data-ttu-id="fca52-110">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="fca52-110">User management admin</span></span>

<span data-ttu-id="fca52-111">간접 공급자와 직접 청구 파트너는 Azure용 CSP(클라우드 서비스 공급자) 프로그램에서 사용할 수 있는 새로운 상거래 환경으로 전환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-111">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="fca52-112">(직접 재판매인은 간접 공급자를 통해 작업해야 합니다.) 고객은 파트너 또는 Microsoft 판매자에게 구입하든 아니면 웹에서 직접 구입하든, 간편하게 클라우드 서비스를 구입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-112">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="fca52-113">전환 기능은 Azure의 새로운 상거래 환경으로 전환하는 고객과 Microsoft 고객 계약에 서명한 고객을 위한 것이며, Office 365 또는 Dynamics 365와 같은 CSP의 다른 제품을 위한 것이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-113">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement and not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="fca52-114">기존 CSP 제품을 Azure 플랜으로 전환</span><span class="sxs-lookup"><span data-stu-id="fca52-114">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="fca52-115">파트너 센터 내에서 고객을 기존 CSP Azure 제품에서 CSP 프로그램의 새로운 상거래 환경에서 제공하는 Azure 플랜 하의 Azure 서비스로 전환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-115">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="fca52-116">이렇게 하려면 파트너와 고객에게 파트너 센터를 통해 설정된 재판매인 관계가 있어야 하고, 고객은 Microsoft 고객 계약에 서명해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-116">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="fca52-117">Azure 플랜으로 전환 선택</span><span class="sxs-lookup"><span data-stu-id="fca52-117">Select transition to Azure plan</span></span>

1. <span data-ttu-id="fca52-118">고객에게 Azure 플랜을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-118">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="fca52-119">**청구를 Azure 플랜으로 전환**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-119">Select **Transition billing to Azure plan**.</span></span>

   :::image type="content" source="images/azure/transition1.png" alt-text="사용량 기반 구독 정보를 보여주는 스크린샷으로 다음과 같은 선택 가능한 옵션으로 표시됩니다. Azure 구독 청구를 Azure 플랜으로 전환":::

3. <span data-ttu-id="fca52-121">**계속**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-121">Select **Continue**</span></span>

   :::image type="content" source="images/azure/transition2.png" alt-text="Azure 플랜으로 전환이라는 대화 상자에는 전환에 대한 의미와 선택할 수 있는 두 가지 옵션(계속 또는 취소)이 포함되어 있습니다.":::

   <span data-ttu-id="fca52-123">고객이 Azure 플랜으로 전환됩니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-123">Your customer will be transitioned to the Azure plan.</span></span>

   <span data-ttu-id="fca52-124">**전환 워크플로는 다음과 같은 필수 조건 단계를 자동화합니다**.</span><span class="sxs-lookup"><span data-stu-id="fca52-124">**The transition workflow automates the pre-requisite steps**:</span></span>

   - <span data-ttu-id="fca52-125">Azure 플랜 구입</span><span class="sxs-lookup"><span data-stu-id="fca52-125">Purchase of Azure plan(s)</span></span>
   - <span data-ttu-id="fca52-126">직접 CSP 시나리오에서는 고객당 플랜 하나</span><span class="sxs-lookup"><span data-stu-id="fca52-126">One plan per customer in Direct CSP scenarios</span></span>  
   - <span data-ttu-id="fca52-127">재판매인당 플랜 하나</span><span class="sxs-lookup"><span data-stu-id="fca52-127">One plan per reseller</span></span>  

   <span data-ttu-id="fca52-128">예를 들어 파트너가 Microsoft Azure 제품을 2개 구입하고 별도의 POR 2개를 구매에 포함했습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-128">For an example, a partner has purchased two Microsoft Azure offers and has    included two distinct POR in the purchase.</span></span> <span data-ttu-id="fca52-129">이 경우 전환 워크플로에서는 Azure 플랜을 2개 구입하고(재판매인당 하나) Azure 플랜에 따라 각 Azure 구독을 자동으로 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-129">In this case, the transition    workflow will purchase two Azure plans (one per reseller) and map the    respective Azure subscriptions under the Azure plans automatically.</span></span>  

   <span data-ttu-id="fca52-130">**Azure 구독을 Azure 플랜에 매핑**</span><span class="sxs-lookup"><span data-stu-id="fca52-130">**Mapping Azure subscription to Azure plan**</span></span>

   <span data-ttu-id="fca52-131">Azure 플랜을 구입한 후에는 시스템에서 기존 Azure 구독을 Azure 플랜에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-131">After your purchase of Azure plan(s), our system will map the existing Azure    subscriptions to the Azure plans.</span></span> <span data-ttu-id="fca52-132">진행률은 Azure Portal과 파트너 센터에서 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-132">The progress can be viewed in Azure portal as    well as in Partner center.</span></span>

4. <span data-ttu-id="fca52-133">고객의 파트너 센터 **구독** 페이지로 돌아와서 고객의 예산 한도를 고객의 현지 통화로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-133">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span>

   :::image type="content" source="images/azure/transition3.png" alt-text="청구 기간 동안 현지 통화로 예산 한도가 설정된 파트너 센터 구독 페이지의 부분 보기입니다.":::

   >[!NOTE]
   ><span data-ttu-id="fca52-135">파트너 센터에서 설정한 예산이 Azure Portal로 전달되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-135">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="fca52-136">Azure Portal에서도 예산과 경고를 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-136">You should also set the budget and alert in Azure portal.</span></span>

   <span data-ttu-id="fca52-137">Azure 플랜으로 이동하면 더 이상 이 고객에 대한 Azure 구독을 구매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-137">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="fca52-138">Azure Portal에서 Azure 플랜에 따라 구독을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-138">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

   >[!NOTE]
   > <span data-ttu-id="fca52-139">Azure 플랜에서 RBAC를 통해 구입한 모든 Azure 구독은 현지 통화로 가격이 책정되고 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-139">All Azure subscriptions purchased through RBAC under the Azure plan will be    priced and billed in local currency.</span></span> <span data-ttu-id="fca52-140">환율은 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-140">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="fca52-141">전환 세부 정보 추적</span><span class="sxs-lookup"><span data-stu-id="fca52-141">Track your transition details</span></span>

<span data-ttu-id="fca52-142">Azure Portal과 파트너 센터에서 전환 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="fca52-142">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

:::image type="content" source="images/azure/details1.png" alt-text="구독당 전환 세부 정보 목록이 있는 표를 보여주는 스크린샷 - 구독 ID, 전환 날짜 및 전환 상태가 포함되어 있습니다.":::

### <a name="billing-impact-to-partners"></a><span data-ttu-id="fca52-144">파트너에게 미치는 청구 영향</span><span class="sxs-lookup"><span data-stu-id="fca52-144">Billing impact to partners</span></span>

<span data-ttu-id="fca52-145">기존 CSP Azure 제품을 사용하는 고객을 전환하면 다음과 같은 청구 영향이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-145">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="fca52-146">원래의 CSP Azure 구독이 종료될 때까지의 모든 사용량에 대한 요금은 기존 CSP 청구서로 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-146">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="fca52-147">기존 CSP 구독에 대한 관리자 액세스 권한이 있는 경우 해당 구독이 마이그레이션되어도 계속 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-147">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="fca52-148">직접 기업 계약을 CSP로 전환하고 서버 및 클라우드 등록을 Azure 서비스로 전환하려면 [Microsoft 파트너 계약에 대한 Azure 구독의 청구 소유권 얻기](https://docs.microsoft.com/azure/billing/mpa-request-ownership)를 읽어 보세요.</span><span class="sxs-lookup"><span data-stu-id="fca52-148">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](https://docs.microsoft.com/azure/billing/mpa-request-ownership)</span></span>

### <a name="audit-log"></a><span data-ttu-id="fca52-149">감사 로그</span><span class="sxs-lookup"><span data-stu-id="fca52-149">Audit log</span></span>

<span data-ttu-id="fca52-150">청구를 조정하려면 **구독** 페이지에서 "Microsoft Azure"(0145P) 구독의 기록을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="fca52-150">To reconcile billing, view your history of "Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span>

<span data-ttu-id="fca52-151">"Microsoft Azure"(0145P) 구독은 다음과 같은 두 부분으로 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-151">"Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>

1. <span data-ttu-id="fca52-152">상거래 구독</span><span class="sxs-lookup"><span data-stu-id="fca52-152">Commerce subscription</span></span>
2. <span data-ttu-id="fca52-153">Azure 구독(자격)</span><span class="sxs-lookup"><span data-stu-id="fca52-153">Azure subscription (entitlement)</span></span>

<span data-ttu-id="fca52-154">전환이 완료되면 Azure 구독이 새 Azure 플랜으로 이동되고 상거래 구독이 일시 중단되어 더 이상 서비스 사용이 보고되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-154">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

>[!NOTE]
><span data-ttu-id="fca52-155">CSP에서 Microsoft Azure(0145P) 구독을 구매한 경우 상거래 구독과 Azure 구독(자격)의 가격이 동일합니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-155">When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="fca52-156">청구 소유권이 변경되거나 이전되는 경우에만 가격이 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-156">It is only in the case of billing ownership changes or transfers do the values differ.</span></span>

### <a name="transition-issues"></a><span data-ttu-id="fca52-157">전환 문제</span><span class="sxs-lookup"><span data-stu-id="fca52-157">Transition issues</span></span>

<span data-ttu-id="fca52-158">전환하는 동안에는 문제가 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-158">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="fca52-159">만약 오류가 발생할 경우 전환 워크플로 자체에서 업데이트해 드리겠습니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-159">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="fca52-160">Azure 사용에 방해가 되는 일은 없을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="fca52-160">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="fca52-161">다음 단계</span><span class="sxs-lookup"><span data-stu-id="fca52-161">Next steps</span></span>

- [<span data-ttu-id="fca52-162">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="fca52-162">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="fca52-163">파트너 획득 크레딧 - 개요</span><span class="sxs-lookup"><span data-stu-id="fca52-163">Partner earned credit - overview</span></span>](partner-earned-credit.md)
