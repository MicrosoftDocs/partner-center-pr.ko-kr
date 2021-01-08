---
title: 관리형 서비스에 대한 파트너 획득 크레딧
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 관리형 서비스에 대해 Microsoft PEC(파트너 획득 크레딧)를 계산하고 지불하는 방법과 자격을 갖추는 방법에 대해 알아봅니다.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3acc078b3de3c0443ee64fdaaba2d486d9c466c8
ms.sourcegitcommit: e9066768ab8e242c03f0a7e3ce460ae8cd2e3fda
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/17/2020
ms.locfileid: "97622170"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="52014-103">파트너 획득 크레딧을 계산 및 지불하는 방법</span><span class="sxs-lookup"><span data-stu-id="52014-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="52014-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="52014-104">**Appropriate roles**</span></span>

- <span data-ttu-id="52014-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="52014-105">Global admin</span></span>
- <span data-ttu-id="52014-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="52014-106">User admin</span></span>
- <span data-ttu-id="52014-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="52014-107">Admin agent</span></span>
- <span data-ttu-id="52014-108">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="52014-108">Billing admin</span></span>
- <span data-ttu-id="52014-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="52014-109">Sales agent</span></span>

<span data-ttu-id="52014-110">관리형 서비스에 대한 PEC(파트너 획득 크레딧)는 고객의 Azure 환경 일부 또는 전체에 대한 연중무휴 IT 운영 제어 및 관리를 담당하는 파트너를 알아내서 보상하는 제도입니다.</span><span class="sxs-lookup"><span data-stu-id="52014-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="52014-111">기본적으로 CSP에서는 파트너가 연중무휴 운영을 관리하고 구독의 리소스를 제어할 수 있도록 파트너에게 고객의 구독에 대한 필수 액세스 권한을 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="52014-112">고객이 거래 파트너에 대한 액세스를 프로비저닝하는 추가적인 방법은 다음 섹션에 설명되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="52014-113">월별 청구서 금액은 순 파트너 획득 크레딧입니다.</span><span class="sxs-lookup"><span data-stu-id="52014-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="52014-114">파트너는 월별 조정 파일에서 PEC 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="52014-115">고객이 거래 파트너에 대한 액세스를 프로비저닝하는 추가적인 방법은 [Azure 플랜에서 구독 및 리소스 관리](azure-plan-manage.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="52014-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="52014-116">또한 [Azure CSP 구독에 대한 관리자 권한 복구](revoke-reinstate-csp.md)도 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="52014-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="52014-117">자격</span><span class="sxs-lookup"><span data-stu-id="52014-117">Eligibility</span></span>

<span data-ttu-id="52014-118">PEC(파트너 획득 크레딧)를 받으려면 다음 요구 사항이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="52014-119">관리하는 Azure 자산에 대해 획득되는 크레딧을 받으려면 활성 MPN 계약 및 유효한 RBAC(역할 기반 액세스 제어) 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="52014-120">CSP에서 고객의 Azure 리소스 운영을 연중무휴로 제어하고 관리해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="52014-121">즉, 고객의 Azure 구독, Azure 리소스 그룹, Azure 리소스에 대한 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="52014-122">간접 공급자 및 해당 간접 재판매인의 경우 둘 중 하나 또는 둘 모두에 이 운영에 대한 제어 권한이 있으면 간접 공급자에게 PEC를 받을 자격이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="52014-123">이에 대한 자세한 내용은 [Azure CSP 구독에 대한 관리자 권한 복구](https://docs.microsoft.com/partner-center/revoke-reinstate-csp)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="52014-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](https://docs.microsoft.com/partner-center/revoke-reinstate-csp).</span></span>

- <span data-ttu-id="52014-124">위의 요구 사항 외에도, PEC는 [Azure 플랜 가격 책정](https://partner.microsoft.com/commerce/sales) 페이지에서 내보낼 수 있는 Azure 플랜 사용량 가격 책정에 나열된 서비스에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="52014-125">PEC가 적용되지 **않는** 서비스는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="52014-126">Azure 플랜 예약</span><span class="sxs-lookup"><span data-stu-id="52014-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="52014-127">Azure 플랜 사용량 가격의 [태그] 열에서 [타사]로 식별된 타사 제품</span><span class="sxs-lookup"><span data-stu-id="52014-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="52014-128">Marketplace 가격 목록의 제품</span><span class="sxs-lookup"><span data-stu-id="52014-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="52014-129">Azure Spot Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="52014-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="52014-130">PEC는 Azure 리소스 수준에서 획득됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="52014-131">구독 또는 리소스 그룹 수준에서 유효한 액세스 권한이 있는 경우 더 높은 엔터티로 롤업되는 각 리소스에서 PEC를 획득합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="52014-132">PEC에 대한 자세한 내용은 [Azure Cost Management](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners) 페이지에서도 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-132">Details on PEC are also available on the [Azure Cost management](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="52014-133">계산</span><span class="sxs-lookup"><span data-stu-id="52014-133">Calculation</span></span>

<span data-ttu-id="52014-134">PEC는 매일 계산되며 일별 사용량 파일 및 월별 청구서 조정 파일에서 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="52014-135">파트너(간접 공급자 또는 간접 재판매인)에게는 전체 기간 동안(연중무휴) PEC를 획득할 수 있는 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="52014-136">PEC는 관리되는 Azure 자산을 기준으로 매일 계산됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="52014-137">주어진 청구 기간(월)의 최대 PEC는 15%입니다.</span><span class="sxs-lookup"><span data-stu-id="52014-137">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="52014-138">해당 월(액세스 범위) 및 모든 적격 리소스(액세스 범위)에 대해 권한 있는 영구 액세스를 유지하는 파트너는 15%의 전체 PEC를 획득합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-138">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="52014-139">범위 및 범위 축소로 인해 해당 월의 PEC 비율이 낮아집니다.</span><span class="sxs-lookup"><span data-stu-id="52014-139">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="52014-140">Azure 자산에 대한 일일 정격 사용량 파일은 PEC 적용 여부에 관계없이 매일 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-140">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="52014-141">파트너는 경고에 등록하여 권한 있는 영구 액세스에 대한 변경 내용을 모니터링할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-141">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="52014-142">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="52014-142">Azure Cost Management</span></span>

<span data-ttu-id="52014-143">비용 분석을 사용하는 ACM(Azure Cost Management)을 통해 파트너는 PEC의 혜택을 받은 비용을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-143">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="52014-144">[Azure Portal](https://portal.azure.com)에서 파트너 테넌트에 로그인하고, **Cost Management + 청구** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-144">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="52014-145">**Cost Management** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-145">Select **Cost management**</span></span>

3. <span data-ttu-id="52014-146">**비용 분석** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-146">Select **Cost Analysis**</span></span>

   <span data-ttu-id="52014-147">비용 분석 보기에는 Microsoft에 지불하는 가격으로 구입하고 사용하는 모든 서비스에 대한 청구 계정 비용이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-147">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="52014-148">피벗 차트의 드롭다운에서 **PartnerEarnedCreditApplied** 를 선택하여 PEC가 적용된 비용을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="52014-148">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="52014-149">**PartnerEarnedCreditApplied** 속성이 True이면 관련 비용에는 파트너 획득 크레딧의 혜택이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-149">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="52014-150">PartnerEarnedCreditApplied 속성이 False이면 관련 비용이 필요한 크레딧 자격을 충족하지 못하거나 구입한 서비스가 파트너 획득 크레딧에 적합하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-150">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="52014-151">일반적으로 서비스 사용량은 **Cost Management** 에 표시되는 데 8-24시간이 걸리고, PEC 크레딧은 Azure Cost Management에 액세스한 이후 48시간 내에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="52014-151">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="52014-152">**Group by 및 Add** 필터 기능을 사용하여 **PartnerEarnedCreditApplied** 속성을 기준으로 그룹화하고 필터링하여 PEC가 적용된 비용과 PEC가 적용되지 않은 비용을 자세히 살펴볼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-152">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="52014-153">다음 단계</span><span class="sxs-lookup"><span data-stu-id="52014-153">Next steps</span></span>

- [<span data-ttu-id="52014-154">파트너 획득 크레딧 - 개요</span><span class="sxs-lookup"><span data-stu-id="52014-154">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="52014-155">파트너 획득 크레딧 계산의 자세한 예는 파트너 센터 대시보드(로그인 필요)를 통해 확인할 수 있는 가격표에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52014-155">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="52014-156">Azure 플랜으로 이동 - 시작</span><span class="sxs-lookup"><span data-stu-id="52014-156">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="52014-157">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="52014-157">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="52014-158">Azure CSP 구독에 대한 관리자 권한 철회 또는 복구</span><span class="sxs-lookup"><span data-stu-id="52014-158">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
