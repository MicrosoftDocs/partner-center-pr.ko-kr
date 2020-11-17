---
title: Azure 예약 & 서버 구독
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객에 대 한 Azure 예약 및 서버 구독을 획득, 프로 비전 및 관리 하기 위한 클라우드 솔루션 공급자 기회에 대해 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0434ad2e6494f5efc1b1e5e2aa003dc6587d7b4e
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691353"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="432b7-103">Azure reserved VM instances (RI) + 고객을 위한 서버 구독 획득, 프로 비전, & 관리</span><span class="sxs-lookup"><span data-stu-id="432b7-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="432b7-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="432b7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="432b7-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="432b7-105">Admin agent</span></span>
- <span data-ttu-id="432b7-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="432b7-106">Global admin</span></span>
- <span data-ttu-id="432b7-107">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="432b7-107">Helpdesk agent</span></span>
- <span data-ttu-id="432b7-108">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="432b7-108">Sales agent</span></span>
- <span data-ttu-id="432b7-109">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="432b7-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="432b7-110">Azure Reservations란?</span><span class="sxs-lookup"><span data-stu-id="432b7-110">What are Azure Reservations?</span></span>

<span data-ttu-id="432b7-111">Azure Reservations 1 년 또는 3 년간의 가상 머신에 대해 사전 지불 하 여 비용을 절감 하는 데 도움을 줍니다. 계산 용량, Azure Cosmos DB 처리량 또는 기타 Azure 리소스를 SQL Database 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="432b7-112">선결제하면 사용하는 리소스 요금에 대한 할인을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="432b7-113">예약은 종 량 제 가격과 비교 하 여 가상 머신, SQL database 계산, Azure Cosmos DB 및 기타 리소스 비용을 최대 72%까지 크게 줄일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="432b7-114">예약은 청구 할인을 제공하며, 리소스의 런타임 상태에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="432b7-115">자세한 내용은 [Azure Reservations 정의](/azure/billing/billing-save-compute-costs-reservations) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="432b7-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="432b7-116">고객이 예약을 구매 해야 하는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="432b7-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="432b7-117">고객에 게 오랜 시간 동안 실행 되는 가상 머신, Azure Cosmos DB 또는 SQL 데이터베이스가 있는 경우 예약을 구매 하면 가장 비용 효율적인 옵션이 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="432b7-118">예를 들어 고객이 예약 없이 서비스의 4 개 인스턴스를 지속적으로 실행 하는 경우 종 량 제 요금으로 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="432b7-119">해당 리소스에 대 한 예약을 구매 하는 경우 즉시 예약 할인을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="432b7-120">리소스 요금이 더 이상 종량제로 청구되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="432b7-121">CSP의 새로운 Azure 제품</span><span class="sxs-lookup"><span data-stu-id="432b7-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="432b7-122">Microsoft는 CSP 프로그램에 대 한 Azure Reservations 및 서버 구독을 제공 하 여 높은 예측 가능 하 고 지속적인 클라우드 워크 로드를 지원 하기 위해 더 비용 효율적인 솔루션에 대해 신속 하 게 성장 하는 고객의 요구를 해결 하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="432b7-123">CSP 프로그램을 통해 파트너는 Microsoft 파트너 센터 및 Azure Portal를 통해 상용 고객을 대신 하 여 Azure Reservations 및 서버 구독을 얻고 프로 비전 하 고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="432b7-124">Azure 예약을 구매 하는 방법에 대 한 CSP 프로그램 선택 항목에서 파트너에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="432b7-125">CSP 파트너는 [고객을 대신 하 여 Azure 예약을 구매할](azure-reservations-buying.md) 수 있으며, 고객이 파트너가 구매한 이전 azure 구독에서 [자신의 예약을 구매할](give-customers-permission.md) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="432b7-126">Azure Reservations는 개발 및 테스트, 응용 프로그램 실행, 데이터 센터 확장을 비롯 한 광범위 한 컴퓨팅 솔루션을 위한 유연성을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="432b7-127">예를 들어, 상용 고객은 이제 1 년 또는 3 년 동안 가상 머신을 구매 하거나 "예약" 하 여 간단 하 게 최대 72% 및 종 량 제 Azure VM 가격 책정을 절감할 수 있습니다. [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/)</span><span class="sxs-lookup"><span data-stu-id="432b7-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="432b7-128">소프트웨어 보증에 포함 된 Azure 하이브리드 혜택 포함 된 Windows Server 고객은 최대 80% 대비 종 량 제 가격 책정을 절감할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="432b7-129">뛰어난 가격과 일치 하지 않는 배포 유연성의 조합을 사용 하는 경우 고객은 Azure Reservations를 선택할 때 최상의 전체 가치를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="432b7-130">Azure Portal에서 [구매 예약](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="432b7-130">See [Purchase Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="432b7-131">소프트웨어 구독 및 Linux ISV 연간 구독에 대 한 파트너 센터의 [가격 책정 및 제품](https://partner.microsoft.com/dashboard/sell/pricingandoffers) 페이지에서 **Microsoft Azure 예약 인스턴스** 범주 아래의 **Azure RI CSP 상용 가격 목록을** 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="432b7-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="432b7-132">**Linux ISV 연간 구독**</span><span class="sxs-lookup"><span data-stu-id="432b7-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="432b7-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="432b7-133">SUSE Linux</span></span>
- <span data-ttu-id="432b7-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="432b7-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="432b7-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="432b7-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="432b7-136">**ISV 연간 구독**</span><span class="sxs-lookup"><span data-stu-id="432b7-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="432b7-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="432b7-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="432b7-138">시작</span><span class="sxs-lookup"><span data-stu-id="432b7-138">Getting started</span></span>

<span data-ttu-id="432b7-139">고객과의 Azure Reservations 배치 하 고 최대한 빨리 운영상을 실행 하는 방법을 이해 하려면 준비 자료를 검토 하는 다음과 같은 방법을 사용 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="432b7-140">[파트너 센터 새 상거래 운영 가이드](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)를 검토 하 고 이해 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="432b7-141">[파트너 센터 api (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)의 Azure Reservations 및 서버 구독에 대 한 업데이트를 이해 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="432b7-142">판매 준비</span><span class="sxs-lookup"><span data-stu-id="432b7-142">Sales readiness</span></span>

- [<span data-ttu-id="432b7-143">RDS (원격 데스크톱 서비스) CAL (클라이언트 액세스 라이선스) (알림)</span><span class="sxs-lookup"><span data-stu-id="432b7-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="432b7-144">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="432b7-144">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="432b7-145">서버 구독</span><span class="sxs-lookup"><span data-stu-id="432b7-145">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)

- [<span data-ttu-id="432b7-146">SQL DB 예약 (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="432b7-146">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="432b7-147">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="432b7-147">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="432b7-148">SQL Managed Instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="432b7-148">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="432b7-149">SUSE 및 Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="432b7-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="432b7-150">Azure의 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="432b7-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="432b7-151">Azure의 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="432b7-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="432b7-152">Azure의 Linux</span><span class="sxs-lookup"><span data-stu-id="432b7-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="432b7-153">Azure 가격 책정 개요</span><span class="sxs-lookup"><span data-stu-id="432b7-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="432b7-154">Azure 가격 계산기</span><span class="sxs-lookup"><span data-stu-id="432b7-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="432b7-155">Azure Databricks 단위 예약</span><span class="sxs-lookup"><span data-stu-id="432b7-155">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="432b7-156">학습</span><span class="sxs-lookup"><span data-stu-id="432b7-156">Training</span></span>

<span data-ttu-id="432b7-157">등록 하 여 [상업적 라이선스 준비 웹 세미나](https://commercial-licensing.eventbuilder.com/FY2019_ALL) 및 주문형 이벤트를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="432b7-158">이전에 기록 된 라이선스 준비 요청 시 이벤트에는 다음과 같은 항목이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="432b7-159">CSP Online Services, CSP Azure 및 Azure를 포함 한 일반 라이선스 업데이트 (11 월 2018)</span><span class="sxs-lookup"><span data-stu-id="432b7-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="432b7-160">SQL DB 예약 용량 & 인스턴스 크기 유연성 (8 월 2018 일)</span><span class="sxs-lookup"><span data-stu-id="432b7-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="432b7-161">CSP의 서버 구독 (7 월 2018)</span><span class="sxs-lookup"><span data-stu-id="432b7-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="432b7-162">CSP의 Azure Reservations 개요 (2018 년 5 월)</span><span class="sxs-lookup"><span data-stu-id="432b7-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="432b7-163">작업</span><span class="sxs-lookup"><span data-stu-id="432b7-163">Operations</span></span>

<span data-ttu-id="432b7-164">[파트너 센터 새 상거래 운영 가이드](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): 규약, 파트너 센터의 주문, 송장, 가격 목록 세부 정보, 성과급, 조정 파일, API/SDK, 샌드박스 및 Azure 파트너 공유 서비스와 같은 주요 정책 및 운영 측면을 다루는 포괄적인 가이드입니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="432b7-165">Azure 하이브리드 혜택</span><span class="sxs-lookup"><span data-stu-id="432b7-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="432b7-166">[Azure 하이브리드 혜택](https://azure.microsoft.com/pricing/hybrid-benefit) 은 소프트웨어 보증을 포함 하는 라이선스가 있는 고객에 대 한 가격 책정으로, 기존 온-프레미스 Windows Server의 가치를 최대화 하는 데 도움이 되며, Azure로 마이그레이션할 때 라이선스 투자를 SQL Server 합니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="432b7-167">적격 고객은 azure Virtual Machines (infrastructure as a service 또는 IaaS)에서 최대 40% \*의 비용을 절감 하 55 고, Azure SQL Database (platform as a service) 및 Azure 하이브리드 혜택를 사용 하 여 Azure Virtual Machines (IaaS)에서 SQL Server 수 있으며, Azure Reserved Instances와 함께 사용할 경우 최대 80%까지 늘어납니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="432b7-168">다음 단계</span><span class="sxs-lookup"><span data-stu-id="432b7-168">Next steps</span></span>

- [<span data-ttu-id="432b7-169">Azure 하이브리드 혜택 FAQ</span><span class="sxs-lookup"><span data-stu-id="432b7-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="432b7-170">\* 실제 절감 액은 지역, 인스턴스 유형 또는 사용량에 따라 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="432b7-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>
