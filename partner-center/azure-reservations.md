---
title: 고객 Microsoft Azure 예약 판매
description: 클라우드 솔루션 공급자는 고객에 대 한 Azure 예약을 구입, 판매 또는 관리할 수 있습니다. 파트너 센터, Azure Portal 또는 파트너 센터 API를 사용 합니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534899"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="83ae3-104">파트너 센터, Azure Portal 또는 Api를 사용 하 여 고객에 게 Microsoft Azure 예약 판매</span><span class="sxs-lookup"><span data-stu-id="83ae3-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="83ae3-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="83ae3-105">**Appropriate roles**</span></span>

- <span data-ttu-id="83ae3-106">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="83ae3-106">Admin agent</span></span>
- <span data-ttu-id="83ae3-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="83ae3-107">Global admin</span></span>
- <span data-ttu-id="83ae3-108">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="83ae3-108">Helpdesk agent</span></span>
- <span data-ttu-id="83ae3-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="83ae3-109">Sales agent</span></span>
- <span data-ttu-id="83ae3-110">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="83ae3-110">User management admin</span></span>

<span data-ttu-id="83ae3-111">CSP (클라우드 솔루션 공급자 프로그램)의 파트너는 고객에 대 한 Azure 예약을 구입, 판매 또는 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="83ae3-112">파트너 센터, Azure Portal 또는 파트너 센터 API를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="83ae3-113">이 문서는 CSP의 파트너 에게만 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="83ae3-114">다른 유형의 구독 (예: 종 량 제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용 하는 고객은 [이 Azure 예약 설명서](/azure/cost-management-billing/reservations)를 대신 읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="83ae3-115">CSP 프로그램의 파트너는 고객에 게 Microsoft Azure 예약을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="83ae3-116">고객은 사전에 대비 하 여 상당한 비용을 절감할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="83ae3-117">Azure 예약은 다음과 같은 방식으로 고객의 단순성 및 유연성을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="83ae3-118">1 년 또는 3 년 예약 용어</span><span class="sxs-lookup"><span data-stu-id="83ae3-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="83ae3-119">쉽게 시작할 수 있습니다. 설치가 완료 된 시간 (초)</span><span class="sxs-lookup"><span data-stu-id="83ae3-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="83ae3-120">조정 된 환불을 위해 언제 든 지 예약 된 인스턴스 취소 또는 교환</span><span class="sxs-lookup"><span data-stu-id="83ae3-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="83ae3-121">조직 또는 개별 부서 수준에서 예약 인스턴스 사용을 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="83ae3-122">Azure 예약은 다음과 같은 방식으로 고객에 게 더욱 매력적인 효과를 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="83ae3-123">예약은 PAYG (종 량 제) 가격에 비해 상당한 절감 효과를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="83ae3-124">1 년 또는 3 년 조건에 대 한 선불 결제로 더 나은 예산 및 예측</span><span class="sxs-lookup"><span data-stu-id="83ae3-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="83ae3-125">사무실에 가장 가까운 Azure 지역에서 우선 순위가 지정 된 컴퓨팅 용량</span><span class="sxs-lookup"><span data-stu-id="83ae3-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="83ae3-126">Azure 예약은 Microsoft Windows Server 및 Azure SQL Database와 같은 소프트웨어와 함께 사용할 경우 종단 간 인프라 솔루션에 대 한 기초를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="83ae3-127">파트너 센터와 Azure Portal 파트너 센터 API를 사용 하 여 Azure 예약을 구입, 판매 및 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="83ae3-128">구매한 Azure 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="83ae3-129">방법에 대 한 자세한 내용은 아래 링크를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="83ae3-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="83ae3-130">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="83ae3-130">Azure reservations resources</span></span>

|<span data-ttu-id="83ae3-131">**원하는 정보**</span><span class="sxs-lookup"><span data-stu-id="83ae3-131">**For information about**</span></span>   |<span data-ttu-id="83ae3-132">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="83ae3-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="83ae3-133">고객을 위한 Azure 예약 설명서</span><span class="sxs-lookup"><span data-stu-id="83ae3-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="83ae3-134">Azure 예약은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="83ae3-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="83ae3-135">파트너 센터에서 고객에 대 한 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="83ae3-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="83ae3-136">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="83ae3-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="83ae3-137">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="83ae3-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="83ae3-138">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="83ae3-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="83ae3-139">올바른 VM 크기 확인 및 고객 VM 사용 확인</span><span class="sxs-lookup"><span data-stu-id="83ae3-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="83ae3-140">최대 Azure 예약 사용에 대 한 VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="83ae3-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="83ae3-141">파트너 센터 API를 사용 하 여 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="83ae3-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="83ae3-142">파트너 센터 개발자 설명서에서 [Azure Reserved VM Instances 구매](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="83ae3-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="83ae3-143">CSP 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="83ae3-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="83ae3-144">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="83ae3-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |