---
title: Azure 예약 & 서버 구독
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객에 대 한 Azure 예약 및 서버 구독을 획득, 프로 비전 및 관리 하기 위한 클라우드 솔루션 공급자 기회에 대해 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b8a9cf07f8dace47346c68ade3707d6b12a1532
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900091"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="ab38e-103">Azure reserved VM instances (RI) + 고객을 위한 서버 구독 획득, 프로 비전, & 관리</span><span class="sxs-lookup"><span data-stu-id="ab38e-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="ab38e-104">적용 대상:</span><span class="sxs-lookup"><span data-stu-id="ab38e-104">Applies to:</span></span>

- <span data-ttu-id="ab38e-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="ab38e-105">Partner Center</span></span>

<span data-ttu-id="ab38e-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="ab38e-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ab38e-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="ab38e-107">Admin agent</span></span>
- <span data-ttu-id="ab38e-108">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="ab38e-108">Global admin</span></span>
- <span data-ttu-id="ab38e-109">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="ab38e-109">Helpdesk agent</span></span>
- <span data-ttu-id="ab38e-110">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="ab38e-110">Sales agent</span></span>
- <span data-ttu-id="ab38e-111">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="ab38e-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="ab38e-112">이 문서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너에만 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="ab38e-113">다른 유형의 구독 (예: 종 량 제, 개인, Microsoft 고객 계약 또는 기업계약 구독)을 사용 하는 고객은 [이 Azure 예약 설명서](https://docs.microsoft.com/azure/cost-management-billing/reservations)를 대신 읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="ab38e-114">Azure Reservations란?</span><span class="sxs-lookup"><span data-stu-id="ab38e-114">What are Azure Reservations?</span></span>

<span data-ttu-id="ab38e-115">Azure Reservations 1 년 또는 3 년간의 가상 머신에 대해 사전 지불 하 여 비용을 절감 하는 데 도움을 줍니다. 계산 용량, Azure Cosmos DB 처리량 또는 기타 Azure 리소스를 SQL Database 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="ab38e-116">선결제하면 사용하는 리소스 요금에 대한 할인을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="ab38e-117">예약은 종 량 제 가격과 비교 하 여 가상 머신, SQL database 계산, Azure Cosmos DB 및 기타 리소스 비용을 최대 72%까지 크게 줄일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="ab38e-118">예약은 청구 할인을 제공하며, 리소스의 런타임 상태에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="ab38e-119">자세한 내용은 [Azure Reservations 정의](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ab38e-119">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="ab38e-120">고객이 예약을 구매 해야 하는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="ab38e-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="ab38e-121">고객에 게 오랜 시간 동안 실행 되는 가상 머신, Azure Cosmos DB 또는 SQL 데이터베이스가 있는 경우 예약을 구매 하면 가장 비용 효율적인 옵션이 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="ab38e-122">예를 들어 고객이 예약 없이 서비스의 4 개 인스턴스를 지속적으로 실행 하는 경우 종 량 제 요금으로 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="ab38e-123">해당 리소스에 대 한 예약을 구매 하는 경우 즉시 예약 할인을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="ab38e-124">리소스 요금이 더 이상 종량제로 청구되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="ab38e-125">CSP의 새로운 Azure 제품</span><span class="sxs-lookup"><span data-stu-id="ab38e-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="ab38e-126">Microsoft는 CSP 프로그램에 대 한 Azure Reservations 및 서버 구독을 제공 하 여 높은 예측 가능 하 고 지속적인 클라우드 워크 로드를 지원 하기 위해 더 비용 효율적인 솔루션에 대해 신속 하 게 성장 하는 고객의 요구를 해결 하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="ab38e-127">CSP 프로그램을 통해 파트너는 Microsoft 파트너 센터 및 Azure Portal를 통해 상용 고객을 대신 하 여 Azure Reservations 및 서버 구독을 얻고 프로 비전 하 고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="ab38e-128">Azure 예약을 구매 하는 방법에 대 한 CSP 프로그램 선택 항목에서 파트너에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="ab38e-129">CSP 파트너는 [고객을 대신 하 여 Azure 예약을 구매할](azure-reservations-buying.md) 수 있으며, 고객이 파트너가 구매한 이전 azure 구독에서 [자신의 예약을 구매할](give-customers-permission.md) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="ab38e-130">Azure Reservations는 개발 및 테스트, 응용 프로그램 실행, 데이터 센터 확장을 비롯 한 광범위 한 컴퓨팅 솔루션을 위한 유연성을 고객에 게 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="ab38e-131">예를 들어, 상용 고객은 이제 1 년 또는 3 년 동안 가상 머신을 구매 하거나 "예약" 하 여 간단 하 게 최대 72% 및 종 량 제 Azure VM 가격 책정을 절감할 수 있습니다. [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/)</span><span class="sxs-lookup"><span data-stu-id="ab38e-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="ab38e-132">소프트웨어 보증에 포함 된 Azure 하이브리드 혜택 포함 된 Windows Server 고객은 최대 80% 대비 종 량 제 가격 책정을 절감할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="ab38e-133">뛰어난 가격과 일치 하지 않는 배포 유연성의 조합을 사용 하 여 고객은 Azure Reservations 선택 하는 경우 가장 적합 한 전체 값을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="ab38e-134">Azure 예약</span><span class="sxs-lookup"><span data-stu-id="ab38e-134">Azure reservations</span></span>

- <span data-ttu-id="ab38e-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="ab38e-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="ab38e-136">SQL DB 예약</span><span class="sxs-lookup"><span data-stu-id="ab38e-136">SQL DB Reservations</span></span>
- <span data-ttu-id="ab38e-137">SQL Managed Instance</span><span class="sxs-lookup"><span data-stu-id="ab38e-137">SQL Managed Instance</span></span>
- <span data-ttu-id="ab38e-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ab38e-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="ab38e-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="ab38e-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="ab38e-140">App Services</span><span class="sxs-lookup"><span data-stu-id="ab38e-140">App Services</span></span>
- <span data-ttu-id="ab38e-141">Azure Databricks 단위 예약</span><span class="sxs-lookup"><span data-stu-id="ab38e-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="ab38e-142">관리 디스크:</span><span class="sxs-lookup"><span data-stu-id="ab38e-142">Managed Disk</span></span>
- <span data-ttu-id="ab38e-143">블록 Blob</span><span class="sxs-lookup"><span data-stu-id="ab38e-143">Block blob</span></span>
- <span data-ttu-id="ab38e-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="ab38e-144">MySQL</span></span>
- <span data-ttu-id="ab38e-145">Azure 데이터 탐색기</span><span class="sxs-lookup"><span data-stu-id="ab38e-145">Azure Data explorer</span></span>
- <span data-ttu-id="ab38e-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="ab38e-146">MariaDB</span></span>
- <span data-ttu-id="ab38e-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="ab38e-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="ab38e-148">서버 구독</span><span class="sxs-lookup"><span data-stu-id="ab38e-148">Server subscriptions</span></span>

- <span data-ttu-id="ab38e-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="ab38e-149">Windows Server</span></span>
- <span data-ttu-id="ab38e-150">RDS (원격 데스크톱 서비스) Cal</span><span class="sxs-lookup"><span data-stu-id="ab38e-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="ab38e-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="ab38e-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="ab38e-152">Linux ISV 연간 구독</span><span class="sxs-lookup"><span data-stu-id="ab38e-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="ab38e-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="ab38e-153">SUSE Linux</span></span>
- <span data-ttu-id="ab38e-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="ab38e-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="ab38e-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="ab38e-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="ab38e-156">ISV 연간 구독</span><span class="sxs-lookup"><span data-stu-id="ab38e-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="ab38e-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="ab38e-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="ab38e-158">시작</span><span class="sxs-lookup"><span data-stu-id="ab38e-158">Getting started</span></span>

<span data-ttu-id="ab38e-159">고객과의 Azure Reservations 배치 하 고 최대한 빨리 운영상을 실행 하는 방법을 이해 하려면 준비 자료를 검토 하는 다음과 같은 방법을 사용 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="ab38e-160">개요 프레젠테이션 및 관련 웹 세미나에서 고객의 가치 제안 및 위치를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="ab38e-161">최신 상거래 운영 가이드 검토 및 이해</span><span class="sxs-lookup"><span data-stu-id="ab38e-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="ab38e-162">Azure RI 및 서버 구독 FAQ 검토</span><span class="sxs-lookup"><span data-stu-id="ab38e-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="ab38e-163">파트너 센터 API의 Azure Reservations 및 서버 구독에 대 한 업데이트 이해 [(API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="ab38e-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="ab38e-164">리소스</span><span class="sxs-lookup"><span data-stu-id="ab38e-164">Resources</span></span>

<span data-ttu-id="ab38e-165">다음은 파트너 센터를 통해 거래 Azure Reservations에 신속 하 게 등록 하는 데 도움이 되는 포괄적인 리소스 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="ab38e-166">판매 준비</span><span class="sxs-lookup"><span data-stu-id="ab38e-166">Sales readiness</span></span>

- [<span data-ttu-id="ab38e-167">Azure 하이브리드 혜택 개요를 사용 하 여 Azure Reservations 및 서버 구독</span><span class="sxs-lookup"><span data-stu-id="ab38e-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="ab38e-168">판매 시트</span><span class="sxs-lookup"><span data-stu-id="ab38e-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="ab38e-169">Azure Reservations에 대 한 파트너 FAQ</span><span class="sxs-lookup"><span data-stu-id="ab38e-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="ab38e-170">Azure Reservations 및 SQL DB에 대 한 파트너 FAQ</span><span class="sxs-lookup"><span data-stu-id="ab38e-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="ab38e-171">RDS (원격 데스크톱 서비스) CAL (클라이언트 액세스 라이선스) (알림)</span><span class="sxs-lookup"><span data-stu-id="ab38e-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="ab38e-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="ab38e-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="ab38e-173">서버 구독</span><span class="sxs-lookup"><span data-stu-id="ab38e-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="ab38e-174">Azure의 SQL DB 개요</span><span class="sxs-lookup"><span data-stu-id="ab38e-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="ab38e-175">SQL DB 예약 (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="ab38e-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="ab38e-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="ab38e-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="ab38e-177">SQL Managed Instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="ab38e-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="ab38e-178">SUSE 및 Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="ab38e-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="ab38e-179">Azure의 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="ab38e-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="ab38e-180">Azure의 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="ab38e-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="ab38e-181">Azure의 Linux</span><span class="sxs-lookup"><span data-stu-id="ab38e-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="ab38e-182">Azure 가격 책정 개요</span><span class="sxs-lookup"><span data-stu-id="ab38e-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="ab38e-183">Azure 가격 계산기</span><span class="sxs-lookup"><span data-stu-id="ab38e-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="ab38e-184">Azure Databricks 단위 예약</span><span class="sxs-lookup"><span data-stu-id="ab38e-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="ab38e-185">CSP 가격 목록: **Microsoft Azure 예약 인스턴스** 및 **소프트웨어 구독** 가격표는 파트너 센터 [가격 책정 & 제품](https://partner.microsoft.com/pcv/sales) 페이지에 모두 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="ab38e-186">학습</span><span class="sxs-lookup"><span data-stu-id="ab38e-186">Training</span></span>

<span data-ttu-id="ab38e-187">등록 하 여 [상업적 라이선스 준비 웹 세미나](https://commercial-licensing.eventbuilder.com/FY2019_ALL) 및 주문형 이벤트를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="ab38e-188">라이선스 준비 주문형 이벤트에는 다음과 같은 항목이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="ab38e-189">CSP Online Services, CSP Azure 및 Azure를 포함 한 일반 라이선스 업데이트 (11 월 2018)</span><span class="sxs-lookup"><span data-stu-id="ab38e-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="ab38e-190">SQL DB 예약 용량 & 인스턴스 크기 유연성 (8 월 2018 일)</span><span class="sxs-lookup"><span data-stu-id="ab38e-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="ab38e-191">CSP의 서버 구독 (7 월 2018)</span><span class="sxs-lookup"><span data-stu-id="ab38e-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="ab38e-192">CSP의 Azure Reservations 개요 (2018 년 5 월)</span><span class="sxs-lookup"><span data-stu-id="ab38e-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="ab38e-193">기타 유용한 학습에는 [파트너 대학의 Azure 라이선스 모듈이](https://aka.ms/azure_partner_licensing)포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="ab38e-194">작업</span><span class="sxs-lookup"><span data-stu-id="ab38e-194">Operations</span></span>

- <span data-ttu-id="ab38e-195">[최신 상거래 운영 가이드](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (업데이트 됨): 규약, 파트너 센터의 주문, 송장, 가격 목록 정보, 성과급, 조정 파일, API/SDK, 샌드박스 및 Azure 파트너 공유 서비스와 같은 주요 정책 및 운영 측면을 다루는 포괄적인 가이드입니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="ab38e-196">최신 국가 가용성 및 고객 통화 행렬 제공</span><span class="sxs-lookup"><span data-stu-id="ab38e-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="ab38e-197">Microsoft Azure 예약 인스턴스 판매</span><span class="sxs-lookup"><span data-stu-id="ab38e-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="ab38e-198">고객을 대신하여 Microsoft Azure 예약 구입</span><span class="sxs-lookup"><span data-stu-id="ab38e-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="ab38e-199">고객을 대신 하 여 Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="ab38e-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="ab38e-200">Azure 예약에 대 한 청구</span><span class="sxs-lookup"><span data-stu-id="ab38e-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="ab38e-201">최대 예약 사용량에 맞게 VM 크기 조정</span><span class="sxs-lookup"><span data-stu-id="ab38e-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="ab38e-202">파트너 센터 API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="ab38e-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="ab38e-203">원격 데스크톱 서비스</span><span class="sxs-lookup"><span data-stu-id="ab38e-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="ab38e-204">Azure 하이브리드 혜택</span><span class="sxs-lookup"><span data-stu-id="ab38e-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="ab38e-205">[Azure 하이브리드 혜택](https://azure.microsoft.com/pricing/hybrid-benefit) 를 사용 하면 Windows Server 라이선스에서 더 많은 가치를 얻을 수 있으며 가상 컴퓨터에서 최대 \* 47%까지 절감할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="ab38e-206">Software Assurance에서 적용되는 Windows Server Datacenter 및 Standard 버전 라이선스를 통해 이 혜택을 이용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="ab38e-207">버전에 따라 라이선스를 변환 하거나 다시 사용 하 여 Azure에서 Windows Server 가상 머신을 실행 하 고 저렴 한 기본 계산 요금 (Linux 가상 머신 요금)을 지불할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="ab38e-208">[AZURE 하이브리드 혜택 FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/) 도 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ab38e-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="ab38e-209">\* 실제 절감 액은 지역, 인스턴스 유형 또는 사용량에 따라 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab38e-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
