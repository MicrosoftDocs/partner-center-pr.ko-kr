---
title: 관리형 서비스에 대한 파트너 획득 크레딧
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 관리형 서비스에 대해 Microsoft 파트너 획득 크레딧(PEC)을 계산하고 지불하는 방법과 자격을 갖추는 방법에 대해 알아봅니다.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: db2dc98d3f40dbb29bd00111d8787a4a8cb0e082
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943620"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="bf614-103">파트너 획득 크레딧을 계산 및 지불하는 방법</span><span class="sxs-lookup"><span data-stu-id="bf614-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="bf614-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="bf614-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bf614-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="bf614-105">Global admin</span></span>
- <span data-ttu-id="bf614-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="bf614-106">User admin</span></span>
- <span data-ttu-id="bf614-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="bf614-107">Admin agent</span></span>
- <span data-ttu-id="bf614-108">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="bf614-108">Billing admin</span></span>
- <span data-ttu-id="bf614-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="bf614-109">Sales agent</span></span>

<span data-ttu-id="bf614-110">관리형 서비스에 대한 PEC(파트너 획득 크레딧)는 고객의 Azure 환경 일부 또는 전체에 대한 연중무휴 IT 운영 제어 및 관리를 담당하는 파트너를 알아내서 보상하는 제도입니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="bf614-111">기본적으로 CSP에서는 파트너가 연중무휴 운영을 관리하고 구독의 리소스를 제어할 수 있도록 파트너에게 고객의 구독에 대한 필수 액세스 권한을 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="bf614-112">고객이 거래 파트너에 대한 액세스를 프로비저닝하는 추가적인 방법은 다음 섹션에 설명되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="bf614-113">월별 청구서 금액은 순 파트너 획득 크레딧입니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="bf614-114">파트너는 월별 조정 파일에서 PEC 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="bf614-115">고객이 거래 파트너에 대한 액세스를 프로비저닝하는 추가적인 방법은 [Azure 플랜에서 구독 및 리소스 관리](azure-plan-manage.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bf614-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="bf614-116">또한 [Azure CSP 구독에 대한 관리자 권한 복구](revoke-reinstate-csp.md)도 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bf614-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="bf614-117">중요한 자격 및 계산 정보</span><span class="sxs-lookup"><span data-stu-id="bf614-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="bf614-118">파트너는 관리하는 Azure 자산에 대한 획득 크레딧을 받으려면 활성 MPN 계약과 유효한 RBAC 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="bf614-119">간접 공급자와 간접 재판매인 중에서 둘 중 하나 또는 둘 모두가 CSP에서 고객의 Azure 리소스에 대해 연중무휴로 운영을 제어하고 관리하는 경우 간접 공급자에게는 PEC 자격이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="bf614-120">PEC는 파트너가 관리하는 CSP에서 고객의 Azure 자산에 대해 청구된(청구 가능) 사용량과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="bf614-121">PEC는 Microsoft에서 요금을 청구하는 CSP 파트너(간접 공급자 및 직접 청구 파트너)만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="bf614-122">적격 서비스: 파트너 획득 크레딧은 [Azure 플랜 가격 책정](https://partner.microsoft.com/commerce/sales) 페이지에서 파트너가 내보낼 수 있는 **Azure 플랜 사용량 가격 책정**에 나열된 서비스에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="bf614-123">참고: Azure 플랜 사용량 가격표 및 Azure 플랜 예약의 **태그** 열에서 **타사**로 식별된 타사 제품 및 Marketplace 가격표의 제품을 포함하지만 이에 국한되지 않는 예외가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-123">Note, there are exceptions including, but not limited to, third-party products identified as **Third Party** in  the **Tags** column of the Azure plan consumption price list and Azure Plan reservations, and products in the Marketplace price list.</span></span>

- <span data-ttu-id="bf614-124">PEC는 매일 계산되며 일별 사용량 파일 및 월별 청구서 조정 파일에서 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-124">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="bf614-125">파트너(간접 공급자 또는 간접 재판매인)에게는 전체 기간 동안(연중무휴) PEC를 획득할 수 있는 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-125">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>  

- <span data-ttu-id="bf614-126">PEC는 Azure 리소스 수준에서 획득됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-126">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="bf614-127">파트너에게 구독 또는 리소스 그룹 수준의 유효한 액세스 권한이 있는 경우 역할이 상위 엔터티까지 적용되는 각 리소스에서 PEC를 획득합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-127">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="bf614-128">또한 [Azure Cost Management](https://go.microsoft.com/fwlink/?linkid=2106482)에서 PEC 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-128">PEC details will also be available on [Azure Cost management](https://go.microsoft.com/fwlink/?linkid=2106482)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="bf614-129">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="bf614-129">Azure Cost Management</span></span>

<span data-ttu-id="bf614-130">비용 분석을 사용하는 ACM(Azure Cost Management)을 통해 파트너는 PEC의 혜택을 받은 비용을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-130">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="bf614-131">[Azure Portal](https://portal.azure.com)에서 파트너 테넌트에 로그인하고, **Cost Management + 청구**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-131">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="bf614-132">**Cost Management**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-132">Select **Cost management**</span></span>

3. <span data-ttu-id="bf614-133">**비용 분석**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-133">Select **Cost Analysis**</span></span>

   <span data-ttu-id="bf614-134">비용 분석 보기에는 Microsoft에 지불하는 가격으로 구입하고 사용하는 모든 서비스에 대한 청구 계정 비용이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-134">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="bf614-135">피벗 차트의 드롭다운에서 **PartnerEarnedCreditApplied**를 선택하여 PEC가 적용된 비용을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-135">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="bf614-136">**PartnerEarnedCreditApplied** 속성이 True이면 관련 비용에는 파트너 획득 크레딧의 혜택이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-136">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="bf614-137">PartnerEarnedCreditApplied 속성이 False이면 관련 비용이 필요한 크레딧 자격을 충족하지 못하거나 구입한 서비스가 파트너 획득 크레딧에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-137">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="bf614-138">일반적으로 서비스 사용량은 **Cost Management**에 표시되는 데 8-24시간이 걸리고, PEC 크레딧은 Azure Cost Management에 액세스한 이후 48시간 내에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-138">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="bf614-139">**Group by 및 Add** 필터 기능을 사용하여 **PartnerEarnedCreditApplied** 속성을 기준으로 그룹화하고 필터링하여 PEC가 적용된 비용과 PEC가 적용되지 않은 비용을 자세히 살펴볼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-139">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bf614-140">다음 단계</span><span class="sxs-lookup"><span data-stu-id="bf614-140">Next steps</span></span>

- [<span data-ttu-id="bf614-141">파트너 획득 크레딧 - 개요</span><span class="sxs-lookup"><span data-stu-id="bf614-141">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="bf614-142">파트너 획득 크레딧 계산의 자세한 예는 파트너 센터 대시보드(로그인 필요)를 통해 확인할 수 있는 가격표에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf614-142">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="bf614-143">Azure 플랜으로 이동 - 시작</span><span class="sxs-lookup"><span data-stu-id="bf614-143">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="bf614-144">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="bf614-144">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="bf614-145">Azure CSP 구독에 대한 관리자 권한 철회 또는 복구</span><span class="sxs-lookup"><span data-stu-id="bf614-145">Revoke or re-instate admin privileges for Azure CSP subscriptions  </span></span>](revoke-reinstate-csp.md)

