---
title: 고객 Microsoft Azure 예약 판매
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 클라우드 솔루션 공급자는 고객에 대 한 Azure 예약을 구입, 판매 또는 관리할 수 있습니다. 파트너 센터, Azure Portal 또는 파트너 센터 API를 사용 합니다.
author: LauraBrenner
ms.author: labrenne
keywords: azure, 예약, 관리, 청구, 구매, Azure RI, Azure Reserved Instances
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19c156f0b47ccb39bc678cdd2ae9cce9db5c5ebd
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908296"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="8f45e-105">파트너 센터, Azure Portal 또는 Api를 사용 하 여 고객에 게 Microsoft Azure 예약 판매</span><span class="sxs-lookup"><span data-stu-id="8f45e-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<!--Maggie, 12/7/18 - Added "Partner Center" to metadata title and H1 title as per Catherine Watson in bug #19868631-->

<span data-ttu-id="8f45e-106">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="8f45e-106">**Applies to**</span></span>

- <span data-ttu-id="8f45e-107">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="8f45e-107">Partner Center</span></span>
- <span data-ttu-id="8f45e-108">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="8f45e-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="8f45e-109">CSP의 파트너</span><span class="sxs-lookup"><span data-stu-id="8f45e-109">Partners in CSP</span></span>

<span data-ttu-id="8f45e-110">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="8f45e-110">**Appropriate roles**</span></span>

- <span data-ttu-id="8f45e-111">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="8f45e-111">Admin agent</span></span>
- <span data-ttu-id="8f45e-112">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="8f45e-112">Global admin</span></span>
- <span data-ttu-id="8f45e-113">기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="8f45e-113">Helpdesk agent</span></span>
- <span data-ttu-id="8f45e-114">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="8f45e-114">Sales agent</span></span>
- <span data-ttu-id="8f45e-115">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="8f45e-115">User management admin</span></span>

<span data-ttu-id="8f45e-116">CSP (클라우드 솔루션 공급자 프로그램)의 파트너는 고객에 게 Microsoft Azure 예약을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="8f45e-117">고객은 사전에 대비 하 여 상당한 비용을 절감할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="8f45e-118">Azure 예약은 다음과 같은 방식으로 고객의 단순성 및 유연성을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="8f45e-119">1 년 또는 3 년 예약 용어</span><span class="sxs-lookup"><span data-stu-id="8f45e-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="8f45e-120">쉽게 시작할 수 있습니다. 설치가 완료 된 시간 (초)</span><span class="sxs-lookup"><span data-stu-id="8f45e-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="8f45e-121">조정 된 환불을 위해 언제 든 지 예약 된 인스턴스 취소 또는 교환</span><span class="sxs-lookup"><span data-stu-id="8f45e-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="8f45e-122">조직 또는 개별 부서 수준에서 예약 인스턴스 사용을 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="8f45e-123">Azure 예약은 다음과 같은 방식으로 고객에 게 더욱 매력적인 효과를 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="8f45e-124">예약은 PAYG (종 량 제) 가격에 비해 상당한 절감 효과를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="8f45e-125">1 년 또는 3 년 조건에 대 한 선불 결제로 더 나은 예산 및 예측</span><span class="sxs-lookup"><span data-stu-id="8f45e-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="8f45e-126">사무실에 가장 가까운 Azure 지역에서 우선 순위가 지정 된 컴퓨팅 용량</span><span class="sxs-lookup"><span data-stu-id="8f45e-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="8f45e-127">Azure 예약은 Microsoft Windows Server 및 Azure SQL Database와 같은 소프트웨어와 함께 사용할 경우 종단 간 인프라 솔루션에 대 한 기초를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="8f45e-128">파트너 센터와 Azure Portal 파트너 센터 API를 사용 하 여 Azure 예약을 구입, 판매 및 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="8f45e-129">구매한 Azure 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="8f45e-130">방법에 대 한 자세한 내용은 아래 링크를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="8f45e-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="8f45e-131">Azure 예약 리소스</span><span class="sxs-lookup"><span data-stu-id="8f45e-131">Azure reservations resources</span></span>

|<span data-ttu-id="8f45e-132">**원하는 정보**</span><span class="sxs-lookup"><span data-stu-id="8f45e-132">**For information about**</span></span>   |<span data-ttu-id="8f45e-133">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="8f45e-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="8f45e-134">고객을 위한 Azure 예약 설명서</span><span class="sxs-lookup"><span data-stu-id="8f45e-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="8f45e-135">Azure 예약이란?</span><span class="sxs-lookup"><span data-stu-id="8f45e-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="8f45e-136">파트너 센터에서 고객에 대 한 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="8f45e-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="8f45e-137">Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="8f45e-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="8f45e-138">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="8f45e-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="8f45e-139">파트너 센터에서 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="8f45e-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="8f45e-140">올바른 VM 크기 확인 및 고객 VM 사용 확인</span><span class="sxs-lookup"><span data-stu-id="8f45e-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="8f45e-141">최대 Azure 예약 사용에 대 한 VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="8f45e-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="8f45e-142">파트너 센터 API를 사용 하 여 Azure 예약 구매</span><span class="sxs-lookup"><span data-stu-id="8f45e-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="8f45e-143">파트너 센터 개발자 설명서에서 [Azure Reserved VM Instances 구매](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="8f45e-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="8f45e-144">CSP 구독에서 자신의 Azure 예약을 구매할 수 있는 권한을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f45e-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="8f45e-145">고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="8f45e-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
