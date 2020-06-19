---
title: 파트너의 획득 크레딧을 계산 하는 방법
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure 계획의 PEC (파트너 획득 크레딧) 측면이 계산 되는 방법에 대해 알아봅니다. 여기에는 파트너 및 간접 공급자에 대 한 자격 요구 사항이 포함 됩니다.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 437d1bbd6a5ef3a18d149df2b533fdd2d0ed735d
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/17/2020
ms.locfileid: "84908901"
---
# <a name="how-partner-earned-credit-pec-is-calculated-for-partners-in-the-cloud-solution-provider-program"></a><span data-ttu-id="1540d-104">클라우드 솔루션 공급자 프로그램에서 파트너에 대해 PEC (파트너 획득 크레딧)를 계산 하는 방법</span><span class="sxs-lookup"><span data-stu-id="1540d-104">How partner earned credit (PEC) is calculated for partners in the Cloud Solution Provider program</span></span>

<span data-ttu-id="1540d-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="1540d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="1540d-106">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="1540d-106">Global admin</span></span>
- <span data-ttu-id="1540d-107">대금 청구 관리자</span><span class="sxs-lookup"><span data-stu-id="1540d-107">Billing admin</span></span>

<span data-ttu-id="1540d-108">IT의 연중 무휴 IT 운영 관리 나 CSP에서 고객의 전체 Azure 환경을 소유한 파트너는 PEC의 보상을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-108">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="1540d-109">PEC는 Microsoft와 직접 청구 되는 파트너를 위한 송장의 일부로 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-109">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="1540d-110">크레딧은 매일 계산 되 고 월별 청구서에 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-110">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="1540d-111">기본적으로 CSP에서 파트너는 고객의 구독에 대 한 필수 액세스 권한을 부여 하 여 구독에 대 한 리소스를 연중 무휴 운영 관리 하 고 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="1540d-112">고객이 거래 파트너에 대 한 액세스를 프로 비전 할 수 있는 추가 방법은 다음 섹션에 설명 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-112">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="1540d-113">중요 한 자격 및 계산 요구 사항:</span><span class="sxs-lookup"><span data-stu-id="1540d-113">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="1540d-114">파트너는 자신이 관리 하는 azure 자산에 대해 획득 크레딧을 받으려면 활성 MPN 계약 및 유효한 RBAC (규칙 기반 계정 컨트롤) 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-114">A partner should have an active MPN agreement and a valid Rules Based Account Control (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="1540d-115">[유효한 RBAC 역할]에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="1540d-115">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="1540d-116">간접 공급자는 해당 사용자 또는 간접 재판매인 또는 둘 다가 CSP에서 고객의 Azure 리소스를 연중 무휴 운영 하 고 관리 하는 경우 PEC에 적합 합니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-116">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="1540d-117">PEC는 파트너가 관리하는 CSP에서 고객의 Azure 자산에 대해 청구된(청구 가능) 사용량과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-117">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="1540d-118">PEC는 Microsoft (간접 공급자 및 다이렉트 청구 파트너)가 청구 하는 CSP의 파트너 에게만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-118">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="1540d-119">적격 서비스: 파트너의 획득 크레딧을 가격 목록에 제공 된 모든 Azure 1PP Azure 사용량에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-119">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="1540d-120">3PP 및 Azure Reservations을 포함 하지만이에 국한 되지 않는 예외도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-120">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="1540d-121">PEC는 매일 계산 되며 일일 정찰 파일에서 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-121">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="1540d-122">파트너 (공급자를 통해)는 전체 영업일 (연중 무휴)에 대 한 액세스 권한이 있어야 PEC를 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-122">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="1540d-123">PEC는 Azure 리소스 수준에서 획득됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-123">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="1540d-124">파트너에 게 구독 또는 리소스 그룹 수준에서 유효한 액세스 권한이 있는 경우 해당 역할이 상위 엔터티에 속하는 각 리소스는 PEC를 얻게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-124">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="1540d-125">PEC는 파트너의 월간 청구서에 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-125">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="1540d-126">청구서에는 요금이 부과 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-126">The invoice is net of charges.</span></span> <span data-ttu-id="1540d-127">세부 정보는 invoice 정찰 파일에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1540d-127">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="1540d-128">Azure 구독 관리에 대 한 액세스 권한을 얻는 방법 및 MPN ID를 RBAC 역할에 연결 하는 방법에 대 한 자세한 내용은 [azure 계획에서 구독 및 리소스 관리](azure-plan-manage.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="1540d-128">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="1540d-129">참조 항목</span><span class="sxs-lookup"><span data-stu-id="1540d-129">For more information</span></span>

- [<span data-ttu-id="1540d-130">Azure 계획-청구</span><span class="sxs-lookup"><span data-stu-id="1540d-130">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="1540d-131">CSP의 새로운 상거래 환경에 대한 가격표</span><span class="sxs-lookup"><span data-stu-id="1540d-131">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)