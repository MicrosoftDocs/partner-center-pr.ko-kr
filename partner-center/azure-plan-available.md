---
title: Azure CSP에서 사용 가능한 Azure 서비스
description: 이 문서에서는 Azure CSP(클라우드 솔루션 공급자) 프로그램에서 사용할 수 있는 Azure 서비스와 사용할 수 없는 Azure 서비스에 대해 설명합니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: da97dded531b6792a4468d9be9b63367f818b352
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149743"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a><span data-ttu-id="649eb-103">Azure CSP(클라우드 솔루션 공급자) 프로그램에서 사용할 수 있는 Azure 서비스</span><span class="sxs-lookup"><span data-stu-id="649eb-103">Azure services available in the Azure Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="649eb-104">**적절한 역할**: 관리 에이전트 | 청구 관리자 | 전역 관리자 | Helpdesk 에이전트 | 영업 에이전트 | 사용자 관리 관리자</span><span class="sxs-lookup"><span data-stu-id="649eb-104">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

## <a name="available-azure-services-in-azure-csp"></a><span data-ttu-id="649eb-105">Azure CSP에서 사용 가능한 Azure 서비스</span><span class="sxs-lookup"><span data-stu-id="649eb-105">Available Azure services in Azure CSP</span></span>

<span data-ttu-id="649eb-106">이 문서에는 Azure CSP(클라우드 솔루션 공급자) 프로그램에서 사용할 수 있거나 사용할 수 없는 Azure 서비스가 나열되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-106">This article lists the Azure services that are and are not available in the Azure Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="649eb-107">또한 [Microsoft Azure 독일](https://azure.microsoft.com/overview/clouds/germany/) 및 [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) 국가 클라우드의 서비스 가용성에 대해서도 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-107">It also discusses service availability in the national clouds [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) and [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).</span></span>

>[!Note]
> <span data-ttu-id="649eb-108">[Azure 중국](https://www.azure.cn/)은 Azure CSP 프로그램에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-108">[Azure China](https://www.azure.cn/) is not available in the Azure CSP program.</span></span>

## <a name="global-cloud"></a><span data-ttu-id="649eb-109">글로벌 클라우드</span><span class="sxs-lookup"><span data-stu-id="649eb-109">Global Cloud</span></span>

<span data-ttu-id="649eb-110">Azure Resource Manager 모델 기반의 모든 서비스는 CSP 프로그램에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-110">All services based on Azure Resource Manager model are available in CSP Program.</span></span>  <span data-ttu-id="649eb-111">Azure Resource Manager 기반 이외의 서비스는 CSP 프로그램에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-111">Non-Azure Resource Manager services are not available in CSP program.</span></span>  

## <a name="csp-specific-service-configurations"></a><span data-ttu-id="649eb-112">CSP 특정 서비스 구성</span><span class="sxs-lookup"><span data-stu-id="649eb-112">CSP-Specific Service Configurations</span></span>

<span data-ttu-id="649eb-113">특수한 CSP 구성이 필요한 서비스는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-113">The following services require special configurations in CSP:</span></span>

- [<span data-ttu-id="649eb-114">StorSimple</span><span class="sxs-lookup"><span data-stu-id="649eb-114">StorSimple</span></span>](/azure/storsimple/storsimple-partner-csp-overview)

- [<span data-ttu-id="649eb-115">Azure Active Directory Domain Services</span><span class="sxs-lookup"><span data-stu-id="649eb-115">Azure Active Directory Domain Services</span></span>](/azure/active-directory-domain-services/active-directory-ds-csp)

- [<span data-ttu-id="649eb-116">Key Vault</span><span class="sxs-lookup"><span data-stu-id="649eb-116">Key Vault</span></span>](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- <span data-ttu-id="649eb-117">[Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) - 고객 테넌트의 사용자만 Time Series Insight 환경의 데이터에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-117">[Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Only users from the customer tenant can access data in their Time Series Insights environment.</span></span> <span data-ttu-id="649eb-118">파트너는 기본적으로 고객의 Time Series Insights 환경을 관리할 수 있지만, 이 환경의 데이터에 액세스해야 하는 경우 해당 환경을 고객 테넌트에 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-118">Partners can manage their customer's Time Series Insights environment by default, but if they need access to the data in it, they must be added to the customer tenant.</span></span>

## <a name="visual-studio-marketplace"></a><span data-ttu-id="649eb-119">Visual Studio Marketplace</span><span class="sxs-lookup"><span data-stu-id="649eb-119">Visual Studio Marketplace</span></span>

<span data-ttu-id="649eb-120">이제 타사 확장을 제외하고 Visual Studio Marketplace에서 아래에 나열된 항목을 구입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-120">You can now purchase the items listed below from Visual Studio Marketplace, with the exception of third-party extensions.</span></span>

- [<span data-ttu-id="649eb-121">Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="649eb-121">Azure DevOps</span></span>](https://www.visualstudio.com/team-services/)

- [<span data-ttu-id="649eb-122">Visual Studio 구독</span><span class="sxs-lookup"><span data-stu-id="649eb-122">Visual Studio subscriptions</span></span>](https://www.visualstudio.com/subscriptions/)

- [<span data-ttu-id="649eb-123">Xamarin University 교육</span><span class="sxs-lookup"><span data-stu-id="649eb-123">Xamarin University training</span></span>](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

<span data-ttu-id="649eb-124">시작하는 데 도움이 되도록 CSP에서 [Azure DevOps를 설정, 구매 및 관리하는 방법](/vsts/billing/csp/set-up-csp-customer)에 대한 비디오와 설명서를 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-124">To help get you started, we have created videos and documentation about [how to set up, purchase, and manage Azure DevOps](/vsts/billing/csp/set-up-csp-customer) in CSP.</span></span>

## <a name="azure-marketplace-items-in-azure-csp"></a><span data-ttu-id="649eb-125">Azure CSP의 Azure Marketplace 항목</span><span class="sxs-lookup"><span data-stu-id="649eb-125">Azure Marketplace items in Azure CSP</span></span>

<span data-ttu-id="649eb-126">일부 Azure Marketplace 항목은 현재 Azure CSP 구독에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-126">Not all Azure Marketplace items are currently available in Azure CSP subscriptions.</span></span>

- <span data-ttu-id="649eb-127">Microsoft 기반 Azure 서비스: 이러한 서비스는 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-127">Microsoft-based Azure services: These services are available.</span></span> <span data-ttu-id="649eb-128">이전 표와 설명을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="649eb-128">Review the previous table and comments.</span></span>

- <span data-ttu-id="649eb-129">BYOL(사용자 라이선스 필요) 항목: 이러한 항목은 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-129">Bring your own license (BYOL) items: These items are available.</span></span> <span data-ttu-id="649eb-130">BYOL 지원 Azure Marketplace 항목의 전체 목록은 [Azure Marketplace BYOL 페이지](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-130">A full list of BYOL-enabled Azure Marketplace items is available on the [Azure Marketplace BYOL page](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).</span></span>

- <span data-ttu-id="649eb-131">타사 Azure Marketplace 종량제 항목: 공급자가 CSP 채널에 게시한 경우에 이러한 항목을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-131">Pay-As-You-Go third-party Azure Marketplace items: These items are available if the provider has published to the CSP channel.</span></span> <span data-ttu-id="649eb-132">자세한 내용은 [Azure Marketplace 제품 구독 판매](csp-commercial-marketplace-overview.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="649eb-132">For more information, see [Sell subscriptions to Azure Marketplace products](csp-commercial-marketplace-overview.md).</span></span>

- <span data-ttu-id="649eb-133">Citrix XenApp Essentials: 파트너는 CSP에서 고객을 대신하여 XenApp Essentials를 구입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-133">Citrix XenApp Essentials: Partners can purchase XenApp Essentials for customers in CSP.</span></span> <span data-ttu-id="649eb-134">자세한 내용은 [이제 Microsoft 클라우드 솔루션 공급자 채널을 통해 사용할 수 있는 XenApp Essentials 배포](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) Citrix 블로그를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="649eb-134">For more information, see the following Citrix blog- [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).</span></span>

## <a name="national-clouds"></a><span data-ttu-id="649eb-135">국가 클라우드</span><span class="sxs-lookup"><span data-stu-id="649eb-135">National clouds</span></span>

<span data-ttu-id="649eb-136">다음 표에는 국가 클라우드에서 CSP에 사용할 수 있는 자사 Azure 제품, 서비스 및 기능이 정기적으로 업데이트된 목록이 나와 있습니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-136">The following table displays a regularly updated list of the available first-party Azure products, services, and features for CSP in national clouds.</span></span>

| <span data-ttu-id="649eb-137">Azure 제품, 서비스 또는 기능</span><span class="sxs-lookup"><span data-stu-id="649eb-137">Azure product, service, or feature</span></span> | <span data-ttu-id="649eb-138">US Government</span><span class="sxs-lookup"><span data-stu-id="649eb-138">US Government</span></span> | <span data-ttu-id="649eb-139">독일</span><span class="sxs-lookup"><span data-stu-id="649eb-139">Germany</span></span> |
| ------ | :-----------: | :-----------: |
|  <span data-ttu-id="649eb-140">**Compute**</span><span class="sxs-lookup"><span data-stu-id="649eb-140">**Compute**</span></span>  |    |    |
|  <span data-ttu-id="649eb-141">Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="649eb-141">Virtual Machines</span></span>  |  <span data-ttu-id="649eb-142">X</span><span class="sxs-lookup"><span data-stu-id="649eb-142">X</span></span>  |  <span data-ttu-id="649eb-143">X</span><span class="sxs-lookup"><span data-stu-id="649eb-143">X</span></span>  |
|  <span data-ttu-id="649eb-144">Cloud Services</span><span class="sxs-lookup"><span data-stu-id="649eb-144">Cloud Services</span></span>  |    |    |
|  <span data-ttu-id="649eb-145">가상 머신 확장 집합</span><span class="sxs-lookup"><span data-stu-id="649eb-145">Virtual machine scale sets</span></span>  |  <span data-ttu-id="649eb-146">X</span><span class="sxs-lookup"><span data-stu-id="649eb-146">X</span></span>  |  <span data-ttu-id="649eb-147">X</span><span class="sxs-lookup"><span data-stu-id="649eb-147">X</span></span>  |
|  <span data-ttu-id="649eb-148">함수</span><span class="sxs-lookup"><span data-stu-id="649eb-148">Functions</span></span>  |    |    |
|  <span data-ttu-id="649eb-149">Azure Container Service</span><span class="sxs-lookup"><span data-stu-id="649eb-149">Azure Container Service</span></span>  |    |    |
|  <span data-ttu-id="649eb-150">**네트워킹**</span><span class="sxs-lookup"><span data-stu-id="649eb-150">**Networking**</span></span>  |    |    |
|  <span data-ttu-id="649eb-151">Azure DNS</span><span class="sxs-lookup"><span data-stu-id="649eb-151">Azure DNS</span></span>  |    |    |
|  <span data-ttu-id="649eb-152">Content Delivery Network</span><span class="sxs-lookup"><span data-stu-id="649eb-152">Content Delivery Network</span></span>  |    |    |
|  <span data-ttu-id="649eb-153">Traffic Manager</span><span class="sxs-lookup"><span data-stu-id="649eb-153">Traffic Manager</span></span>  |    |    |
|  <span data-ttu-id="649eb-154">ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="649eb-154">ExpressRoute</span></span>  |  <span data-ttu-id="649eb-155">X</span><span class="sxs-lookup"><span data-stu-id="649eb-155">X</span></span>  |  <span data-ttu-id="649eb-156">X</span><span class="sxs-lookup"><span data-stu-id="649eb-156">X</span></span>  |
|  <span data-ttu-id="649eb-157">Virtual Network</span><span class="sxs-lookup"><span data-stu-id="649eb-157">Virtual Network</span></span>  |  <span data-ttu-id="649eb-158">X</span><span class="sxs-lookup"><span data-stu-id="649eb-158">X</span></span>  |  <span data-ttu-id="649eb-159">X</span><span class="sxs-lookup"><span data-stu-id="649eb-159">X</span></span>  |
|  <span data-ttu-id="649eb-160">부하 분산 장치</span><span class="sxs-lookup"><span data-stu-id="649eb-160">Load Balancer</span></span>  |  <span data-ttu-id="649eb-161">X</span><span class="sxs-lookup"><span data-stu-id="649eb-161">X</span></span>  |  <span data-ttu-id="649eb-162">X</span><span class="sxs-lookup"><span data-stu-id="649eb-162">X</span></span>  |
|  <span data-ttu-id="649eb-163">VPN Gateway</span><span class="sxs-lookup"><span data-stu-id="649eb-163">VPN Gateway</span></span>  |  <span data-ttu-id="649eb-164">X</span><span class="sxs-lookup"><span data-stu-id="649eb-164">X</span></span>  |  <span data-ttu-id="649eb-165">X</span><span class="sxs-lookup"><span data-stu-id="649eb-165">X</span></span>  |
|  <span data-ttu-id="649eb-166">Application Gateway</span><span class="sxs-lookup"><span data-stu-id="649eb-166">Application Gateway</span></span>  |  <span data-ttu-id="649eb-167">X</span><span class="sxs-lookup"><span data-stu-id="649eb-167">X</span></span>  |  <span data-ttu-id="649eb-168">X</span><span class="sxs-lookup"><span data-stu-id="649eb-168">X</span></span>  |
|  <span data-ttu-id="649eb-169">Network Watcher</span><span class="sxs-lookup"><span data-stu-id="649eb-169">Network Watcher</span></span>  |  <span data-ttu-id="649eb-170">X</span><span class="sxs-lookup"><span data-stu-id="649eb-170">X</span></span>  |  <span data-ttu-id="649eb-171">X</span><span class="sxs-lookup"><span data-stu-id="649eb-171">X</span></span>  |
|  <span data-ttu-id="649eb-172">**스토리지**</span><span class="sxs-lookup"><span data-stu-id="649eb-172">**Storage**</span></span>  |    |    |
|  <span data-ttu-id="649eb-173">스토리지</span><span class="sxs-lookup"><span data-stu-id="649eb-173">Storage</span></span>  |  <span data-ttu-id="649eb-174">X</span><span class="sxs-lookup"><span data-stu-id="649eb-174">X</span></span>  |  <span data-ttu-id="649eb-175">X</span><span class="sxs-lookup"><span data-stu-id="649eb-175">X</span></span>  |
|  <span data-ttu-id="649eb-176">백업</span><span class="sxs-lookup"><span data-stu-id="649eb-176">Backup</span></span>  |  <span data-ttu-id="649eb-177">X</span><span class="sxs-lookup"><span data-stu-id="649eb-177">X</span></span>  |  <span data-ttu-id="649eb-178">X</span><span class="sxs-lookup"><span data-stu-id="649eb-178">X</span></span>  |
|  <span data-ttu-id="649eb-179">StorSimple</span><span class="sxs-lookup"><span data-stu-id="649eb-179">StorSimple</span></span>  |    |  <span data-ttu-id="649eb-180">X</span><span class="sxs-lookup"><span data-stu-id="649eb-180">X</span></span>  |
|  <span data-ttu-id="649eb-181">Site Recovery</span><span class="sxs-lookup"><span data-stu-id="649eb-181">Site Recovery</span></span>  |  <span data-ttu-id="649eb-182">X</span><span class="sxs-lookup"><span data-stu-id="649eb-182">X</span></span>  |  <span data-ttu-id="649eb-183">X</span><span class="sxs-lookup"><span data-stu-id="649eb-183">X</span></span>  |
|  <span data-ttu-id="649eb-184">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="649eb-184">Data Lake Store</span></span>  |    |    |
|  <span data-ttu-id="649eb-185">Managed Disks</span><span class="sxs-lookup"><span data-stu-id="649eb-185">Managed Disks</span></span>  |  <span data-ttu-id="649eb-186">X</span><span class="sxs-lookup"><span data-stu-id="649eb-186">X</span></span>  |  <span data-ttu-id="649eb-187">X</span><span class="sxs-lookup"><span data-stu-id="649eb-187">X</span></span>  |
|  <span data-ttu-id="649eb-188">**웹 + 모바일**</span><span class="sxs-lookup"><span data-stu-id="649eb-188">**Web + Mobile**</span></span>  |    |    |
|  <span data-ttu-id="649eb-189">App Service</span><span class="sxs-lookup"><span data-stu-id="649eb-189">App Service</span></span>  |  <span data-ttu-id="649eb-190">X</span><span class="sxs-lookup"><span data-stu-id="649eb-190">X</span></span>  |  <span data-ttu-id="649eb-191">X</span><span class="sxs-lookup"><span data-stu-id="649eb-191">X</span></span>  |
|  <span data-ttu-id="649eb-192">App Service on Linux</span><span class="sxs-lookup"><span data-stu-id="649eb-192">App Service on Linux</span></span>  |    |  <span data-ttu-id="649eb-193">X</span><span class="sxs-lookup"><span data-stu-id="649eb-193">X</span></span>  |
|  <span data-ttu-id="649eb-194">API Management</span><span class="sxs-lookup"><span data-stu-id="649eb-194">API Management</span></span>  |  <span data-ttu-id="649eb-195">X</span><span class="sxs-lookup"><span data-stu-id="649eb-195">X</span></span>  |    |
|  <span data-ttu-id="649eb-196">Content Delivery Network</span><span class="sxs-lookup"><span data-stu-id="649eb-196">Content Delivery Network</span></span>  |    |    |
|  <span data-ttu-id="649eb-197">Media Services</span><span class="sxs-lookup"><span data-stu-id="649eb-197">Media Services</span></span>  |  <span data-ttu-id="649eb-198">X</span><span class="sxs-lookup"><span data-stu-id="649eb-198">X</span></span>  |  <span data-ttu-id="649eb-199">X</span><span class="sxs-lookup"><span data-stu-id="649eb-199">X</span></span>  |
|  <span data-ttu-id="649eb-200">Notification Hubs</span><span class="sxs-lookup"><span data-stu-id="649eb-200">Notification Hubs</span></span>  |  <span data-ttu-id="649eb-201">X</span><span class="sxs-lookup"><span data-stu-id="649eb-201">X</span></span>  |  <span data-ttu-id="649eb-202">X</span><span class="sxs-lookup"><span data-stu-id="649eb-202">X</span></span>  |
|  <span data-ttu-id="649eb-203">Azure Search</span><span class="sxs-lookup"><span data-stu-id="649eb-203">Azure Search</span></span>  |    |    |
|  <span data-ttu-id="649eb-204">Azure App Service의 Logic Apps 기능</span><span class="sxs-lookup"><span data-stu-id="649eb-204">Logic Apps feature of Azure App Service</span></span>  |    |    |
|  <span data-ttu-id="649eb-205">**컨테이너**</span><span class="sxs-lookup"><span data-stu-id="649eb-205">**Containers**</span></span>  |    |    |
|  <span data-ttu-id="649eb-206">App Service</span><span class="sxs-lookup"><span data-stu-id="649eb-206">App Service</span></span>  |  <span data-ttu-id="649eb-207">X</span><span class="sxs-lookup"><span data-stu-id="649eb-207">X</span></span>  |  <span data-ttu-id="649eb-208">X</span><span class="sxs-lookup"><span data-stu-id="649eb-208">X</span></span>  |
|  <span data-ttu-id="649eb-209">App Service on Linux</span><span class="sxs-lookup"><span data-stu-id="649eb-209">App Service on Linux</span></span>  |    |  <span data-ttu-id="649eb-210">X</span><span class="sxs-lookup"><span data-stu-id="649eb-210">X</span></span>  |
|  <span data-ttu-id="649eb-211">Batch (배치)</span><span class="sxs-lookup"><span data-stu-id="649eb-211">Batch</span></span>  |  <span data-ttu-id="649eb-212">X</span><span class="sxs-lookup"><span data-stu-id="649eb-212">X</span></span>  |  <span data-ttu-id="649eb-213">X</span><span class="sxs-lookup"><span data-stu-id="649eb-213">X</span></span>  |
|  <span data-ttu-id="649eb-214">Container Registry</span><span class="sxs-lookup"><span data-stu-id="649eb-214">Container Registry</span></span>  |    |    |
|  <span data-ttu-id="649eb-215">Container Instances</span><span class="sxs-lookup"><span data-stu-id="649eb-215">Container Instances</span></span>  |    |    |
|  <span data-ttu-id="649eb-216">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="649eb-216">Service Fabric</span></span>  |  <span data-ttu-id="649eb-217">X</span><span class="sxs-lookup"><span data-stu-id="649eb-217">X</span></span>  |  <span data-ttu-id="649eb-218">X</span><span class="sxs-lookup"><span data-stu-id="649eb-218">X</span></span>  |
|  <span data-ttu-id="649eb-219">Container Service</span><span class="sxs-lookup"><span data-stu-id="649eb-219">Container Service</span></span>  |    |    |
|  <span data-ttu-id="649eb-220">**데이터베이스**</span><span class="sxs-lookup"><span data-stu-id="649eb-220">**Databases**</span></span>  |    |    |
|  <span data-ttu-id="649eb-221">SQL Database</span><span class="sxs-lookup"><span data-stu-id="649eb-221">SQL Database</span></span>  |  <span data-ttu-id="649eb-222">X</span><span class="sxs-lookup"><span data-stu-id="649eb-222">X</span></span>  |  <span data-ttu-id="649eb-223">X</span><span class="sxs-lookup"><span data-stu-id="649eb-223">X</span></span>  |
|  <span data-ttu-id="649eb-224">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="649eb-224">Azure Cosmos DB</span></span>  |  <span data-ttu-id="649eb-225">X</span><span class="sxs-lookup"><span data-stu-id="649eb-225">X</span></span>  |  <span data-ttu-id="649eb-226">X</span><span class="sxs-lookup"><span data-stu-id="649eb-226">X</span></span>  |
|  <span data-ttu-id="649eb-227">SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="649eb-227">SQL Data Warehouse</span></span>  |  <span data-ttu-id="649eb-228">X</span><span class="sxs-lookup"><span data-stu-id="649eb-228">X</span></span>  |  <span data-ttu-id="649eb-229">X</span><span class="sxs-lookup"><span data-stu-id="649eb-229">X</span></span>  |
|  <span data-ttu-id="649eb-230">Redis Cache</span><span class="sxs-lookup"><span data-stu-id="649eb-230">Redis Cache</span></span>  |  <span data-ttu-id="649eb-231">X</span><span class="sxs-lookup"><span data-stu-id="649eb-231">X</span></span>  |  <span data-ttu-id="649eb-232">X</span><span class="sxs-lookup"><span data-stu-id="649eb-232">X</span></span>  |
|  <span data-ttu-id="649eb-233">SQL Server Stretch Database</span><span class="sxs-lookup"><span data-stu-id="649eb-233">SQL Server Stretch Database</span></span>  |  <span data-ttu-id="649eb-234">X</span><span class="sxs-lookup"><span data-stu-id="649eb-234">X</span></span>  |  <span data-ttu-id="649eb-235">X</span><span class="sxs-lookup"><span data-stu-id="649eb-235">X</span></span>  |
|  <span data-ttu-id="649eb-236">Azure Database for MySQL</span><span class="sxs-lookup"><span data-stu-id="649eb-236">Azure Database for MySQL</span></span>  |    |    |
|  <span data-ttu-id="649eb-237">Azure Database for PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="649eb-237">Azure Database for PostgreSQL</span></span>  |    |    |
|  <span data-ttu-id="649eb-238">**데이터 + 분석**</span><span class="sxs-lookup"><span data-stu-id="649eb-238">**Data + Analytics**</span></span>  |    |    |
|  <span data-ttu-id="649eb-239">Databricks</span><span class="sxs-lookup"><span data-stu-id="649eb-239">Databricks</span></span>  |    |    |
|  <span data-ttu-id="649eb-240">HDInsight</span><span class="sxs-lookup"><span data-stu-id="649eb-240">HDInsight</span></span>  |  <span data-ttu-id="649eb-241">X</span><span class="sxs-lookup"><span data-stu-id="649eb-241">X</span></span>  |  <span data-ttu-id="649eb-242">X</span><span class="sxs-lookup"><span data-stu-id="649eb-242">X</span></span>  |
|  <span data-ttu-id="649eb-243">Stream Analytics</span><span class="sxs-lookup"><span data-stu-id="649eb-243">Stream Analytics</span></span>  |    |  <span data-ttu-id="649eb-244">X</span><span class="sxs-lookup"><span data-stu-id="649eb-244">X</span></span>  |
|  <span data-ttu-id="649eb-245">Data Factory</span><span class="sxs-lookup"><span data-stu-id="649eb-245">Data Factory</span></span>  |    |    |
|  <span data-ttu-id="649eb-246">Log Analytics</span><span class="sxs-lookup"><span data-stu-id="649eb-246">Log Analytics</span></span>  |  <span data-ttu-id="649eb-247">X</span><span class="sxs-lookup"><span data-stu-id="649eb-247">X</span></span>  |    |
|  <span data-ttu-id="649eb-248">Data Catalog</span><span class="sxs-lookup"><span data-stu-id="649eb-248">Data Catalog</span></span>  |    |    |
|  <span data-ttu-id="649eb-249">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="649eb-249">Data Lake Store</span></span>  |    |    |
|  <span data-ttu-id="649eb-250">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="649eb-250">Data Lake Analytics</span></span>  |    |    |
|  <span data-ttu-id="649eb-251">Azure Analysis Services</span><span class="sxs-lookup"><span data-stu-id="649eb-251">Azure Analysis Services</span></span>  |    |    |
|  <span data-ttu-id="649eb-252">Power BI Embedded</span><span class="sxs-lookup"><span data-stu-id="649eb-252">Power BI Embedded</span></span>  |    |    |
|  <span data-ttu-id="649eb-253">**AI + Cognitive Services**</span><span class="sxs-lookup"><span data-stu-id="649eb-253">**AI + Cognitive Services**</span></span>  |    |    |
|  <span data-ttu-id="649eb-254">Machine Learning</span><span class="sxs-lookup"><span data-stu-id="649eb-254">Machine Learning</span></span>  |    |  <span data-ttu-id="649eb-255">X</span><span class="sxs-lookup"><span data-stu-id="649eb-255">X</span></span>  |
|  <span data-ttu-id="649eb-256">Azure Bot Service</span><span class="sxs-lookup"><span data-stu-id="649eb-256">Azure Bot Service</span></span>  |    |    |
|  <span data-ttu-id="649eb-257">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="649eb-257">Cognitive Services</span></span>  |    |    |
|  <span data-ttu-id="649eb-258">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="649eb-258">Azure Batch AI</span></span>  |    |    |
|  <span data-ttu-id="649eb-259">**사물 인터넷**</span><span class="sxs-lookup"><span data-stu-id="649eb-259">**Internet of Things**</span></span>  |    |    |
|  <span data-ttu-id="649eb-260">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="649eb-260">IoT Hub</span></span>  |  <span data-ttu-id="649eb-261">X</span><span class="sxs-lookup"><span data-stu-id="649eb-261">X</span></span>  |  <span data-ttu-id="649eb-262">X</span><span class="sxs-lookup"><span data-stu-id="649eb-262">X</span></span>  |
|  <span data-ttu-id="649eb-263">IoT Central</span><span class="sxs-lookup"><span data-stu-id="649eb-263">IoT Central</span></span>  |    |    |
|  <span data-ttu-id="649eb-264">Machine Learning</span><span class="sxs-lookup"><span data-stu-id="649eb-264">Machine Learning</span></span>  |    |  <span data-ttu-id="649eb-265">X</span><span class="sxs-lookup"><span data-stu-id="649eb-265">X</span></span>  |
|  <span data-ttu-id="649eb-266">Stream Analytics</span><span class="sxs-lookup"><span data-stu-id="649eb-266">Stream Analytics</span></span>  |    |  <span data-ttu-id="649eb-267">X</span><span class="sxs-lookup"><span data-stu-id="649eb-267">X</span></span>  |
|  <span data-ttu-id="649eb-268">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="649eb-268">Event Hubs</span></span>  |  <span data-ttu-id="649eb-269">X</span><span class="sxs-lookup"><span data-stu-id="649eb-269">X</span></span>  |  <span data-ttu-id="649eb-270">X</span><span class="sxs-lookup"><span data-stu-id="649eb-270">X</span></span>  |
|  <span data-ttu-id="649eb-271">Location-Based Services</span><span class="sxs-lookup"><span data-stu-id="649eb-271">Location-Based Services</span></span>  |    |    |
|  <span data-ttu-id="649eb-272">Notification Hubs</span><span class="sxs-lookup"><span data-stu-id="649eb-272">Notification Hubs</span></span>  |  <span data-ttu-id="649eb-273">X</span><span class="sxs-lookup"><span data-stu-id="649eb-273">X</span></span>  |  <span data-ttu-id="649eb-274">X</span><span class="sxs-lookup"><span data-stu-id="649eb-274">X</span></span>  |
|  <span data-ttu-id="649eb-275">Time Series Insights</span><span class="sxs-lookup"><span data-stu-id="649eb-275">Time Series Insights</span></span>  |    |    |
|  <span data-ttu-id="649eb-276">**엔터프라이즈 통합**</span><span class="sxs-lookup"><span data-stu-id="649eb-276">**Enterprise Integration**</span></span>  |    |    |
|  <span data-ttu-id="649eb-277">StorSimple</span><span class="sxs-lookup"><span data-stu-id="649eb-277">StorSimple</span></span>  |  <span data-ttu-id="649eb-278">X</span><span class="sxs-lookup"><span data-stu-id="649eb-278">X</span></span>  |    |
|  <span data-ttu-id="649eb-279">API Management</span><span class="sxs-lookup"><span data-stu-id="649eb-279">API Management</span></span>  |    |    |
|  <span data-ttu-id="649eb-280">Event Grid</span><span class="sxs-lookup"><span data-stu-id="649eb-280">Event Grid</span></span>  |    |    |
|  <span data-ttu-id="649eb-281">Data Factory</span><span class="sxs-lookup"><span data-stu-id="649eb-281">Data Factory</span></span>  |    |    |
|  <span data-ttu-id="649eb-282">서비스 버스</span><span class="sxs-lookup"><span data-stu-id="649eb-282">Service Bus</span></span>  |  <span data-ttu-id="649eb-283">X</span><span class="sxs-lookup"><span data-stu-id="649eb-283">X</span></span>  |  <span data-ttu-id="649eb-284">X</span><span class="sxs-lookup"><span data-stu-id="649eb-284">X</span></span>  |
|  <span data-ttu-id="649eb-285">Data Catalog</span><span class="sxs-lookup"><span data-stu-id="649eb-285">Data Catalog</span></span>  |    |    |
|  <span data-ttu-id="649eb-286">SQL Server Stretch Database</span><span class="sxs-lookup"><span data-stu-id="649eb-286">SQL Server Stretch Database</span></span>  |    |  <span data-ttu-id="649eb-287">X</span><span class="sxs-lookup"><span data-stu-id="649eb-287">X</span></span>  |
|  <span data-ttu-id="649eb-288">Azure App Service의 Logic Apps 기능</span><span class="sxs-lookup"><span data-stu-id="649eb-288">Logic Apps feature of Azure App Service</span></span>  |    |    |
|  <span data-ttu-id="649eb-289">**보안 + ID**</span><span class="sxs-lookup"><span data-stu-id="649eb-289">**Security + Identity**</span></span>  |    |    |
|  <span data-ttu-id="649eb-290">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="649eb-290">Azure Active Directory</span></span>  |  <span data-ttu-id="649eb-291">X</span><span class="sxs-lookup"><span data-stu-id="649eb-291">X</span></span>  |  <span data-ttu-id="649eb-292">X</span><span class="sxs-lookup"><span data-stu-id="649eb-292">X</span></span>  |
|  <span data-ttu-id="649eb-293">Azure Active Directory B2C</span><span class="sxs-lookup"><span data-stu-id="649eb-293">Azure Active Directory B2C</span></span>  |    |    |
|  <span data-ttu-id="649eb-294">Multi-Factor Authentication</span><span class="sxs-lookup"><span data-stu-id="649eb-294">Multi-Factor Authentication</span></span>  |    |    |
|  <span data-ttu-id="649eb-295">Azure Active Directory Domain Services</span><span class="sxs-lookup"><span data-stu-id="649eb-295">Azure Active Directory Domain Services</span></span>  |    |    |
|  <span data-ttu-id="649eb-296">Key Vault</span><span class="sxs-lookup"><span data-stu-id="649eb-296">Key Vault</span></span>  |  <span data-ttu-id="649eb-297">X</span><span class="sxs-lookup"><span data-stu-id="649eb-297">X</span></span>  |  <span data-ttu-id="649eb-298">X</span><span class="sxs-lookup"><span data-stu-id="649eb-298">X</span></span>  |
|  <span data-ttu-id="649eb-299">Security Center</span><span class="sxs-lookup"><span data-stu-id="649eb-299">Security Center</span></span>  |  <span data-ttu-id="649eb-300">X</span><span class="sxs-lookup"><span data-stu-id="649eb-300">X</span></span>  |  <span data-ttu-id="649eb-301">X</span><span class="sxs-lookup"><span data-stu-id="649eb-301">X</span></span>  |
|  <span data-ttu-id="649eb-302">**개발자 도구**</span><span class="sxs-lookup"><span data-stu-id="649eb-302">**Developer Tools**</span></span>  |    |    |
|  <span data-ttu-id="649eb-303">Visual Studio Team Services</span><span class="sxs-lookup"><span data-stu-id="649eb-303">Visual Studio Team Services</span></span>  |    |    |
|  <span data-ttu-id="649eb-304">Application Insights</span><span class="sxs-lookup"><span data-stu-id="649eb-304">Application Insights</span></span>  |    |    |
|  <span data-ttu-id="649eb-305">DevTest Labs</span><span class="sxs-lookup"><span data-stu-id="649eb-305">DevTest Labs</span></span>  |    |    |
|  <span data-ttu-id="649eb-306">Visual Studio App Center</span><span class="sxs-lookup"><span data-stu-id="649eb-306">Visual Studio App Center</span></span>  |    |    |
|  <span data-ttu-id="649eb-307">Xamarin University</span><span class="sxs-lookup"><span data-stu-id="649eb-307">Xamarin University</span></span>  |    |    |
|  <span data-ttu-id="649eb-308">**모니터링 + 관리**</span><span class="sxs-lookup"><span data-stu-id="649eb-308">**Monitoring + Management**</span></span>  |    |    |
|  <span data-ttu-id="649eb-309">Advisor</span><span class="sxs-lookup"><span data-stu-id="649eb-309">Advisor</span></span>  |    |    |
|  <span data-ttu-id="649eb-310">백업</span><span class="sxs-lookup"><span data-stu-id="649eb-310">Backup</span></span>  |  <span data-ttu-id="649eb-311">X</span><span class="sxs-lookup"><span data-stu-id="649eb-311">X</span></span>  |  <span data-ttu-id="649eb-312">X</span><span class="sxs-lookup"><span data-stu-id="649eb-312">X</span></span>  |
|  <span data-ttu-id="649eb-313">Site Recovery</span><span class="sxs-lookup"><span data-stu-id="649eb-313">Site Recovery</span></span>  |  <span data-ttu-id="649eb-314">X</span><span class="sxs-lookup"><span data-stu-id="649eb-314">X</span></span>  |  <span data-ttu-id="649eb-315">X</span><span class="sxs-lookup"><span data-stu-id="649eb-315">X</span></span>  |
|  <span data-ttu-id="649eb-316">스케줄러</span><span class="sxs-lookup"><span data-stu-id="649eb-316">Scheduler</span></span>  |  <span data-ttu-id="649eb-317">X</span><span class="sxs-lookup"><span data-stu-id="649eb-317">X</span></span>  |  <span data-ttu-id="649eb-318">X</span><span class="sxs-lookup"><span data-stu-id="649eb-318">X</span></span>  |
|  <span data-ttu-id="649eb-319">자동화</span><span class="sxs-lookup"><span data-stu-id="649eb-319">Automation</span></span>  |  <span data-ttu-id="649eb-320">X</span><span class="sxs-lookup"><span data-stu-id="649eb-320">X</span></span>  |  <span data-ttu-id="649eb-321">X</span><span class="sxs-lookup"><span data-stu-id="649eb-321">X</span></span>  |
|  <span data-ttu-id="649eb-322">Log Analytics</span><span class="sxs-lookup"><span data-stu-id="649eb-322">Log Analytics</span></span>  |  <span data-ttu-id="649eb-323">X</span><span class="sxs-lookup"><span data-stu-id="649eb-323">X</span></span>  |    |
|  <span data-ttu-id="649eb-324">Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="649eb-324">Azure Monitor</span></span>  |    |    |
|  <span data-ttu-id="649eb-325">Azure-Managed Applications</span><span class="sxs-lookup"><span data-stu-id="649eb-325">Azure-Managed Applications</span></span>  |    |    |
|  <span data-ttu-id="649eb-326">Azure Migrate</span><span class="sxs-lookup"><span data-stu-id="649eb-326">Azure Migrate</span></span>  |    |    |
|  <span data-ttu-id="649eb-327">관리 그룹</span><span class="sxs-lookup"><span data-stu-id="649eb-327">Management Groups</span></span>  |    |  

## <a name="next-steps"></a><span data-ttu-id="649eb-328">다음 단계</span><span class="sxs-lookup"><span data-stu-id="649eb-328">Next steps</span></span>

- <span data-ttu-id="649eb-329">파트너 센터에서 Azure에 사용할 수 있는 기능에 대해 [알아봅니다](/azure/cloud-solution-provider/overview/partner-center-overview).</span><span class="sxs-lookup"><span data-stu-id="649eb-329">[Learn](/azure/cloud-solution-provider/overview/partner-center-overview) about the available capabilities for Azure in Partner Center.</span></span>

- <span data-ttu-id="649eb-330">Azure CSP에서 첫 번째 고객을 [만들고](/azure/cloud-solution-provider/customer-management/create-new-customer) Azure 서비스를 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="649eb-330">[Create](/azure/cloud-solution-provider/customer-management/create-new-customer) your first customer in Azure CSP, and deploy Azure services.</span></span>
