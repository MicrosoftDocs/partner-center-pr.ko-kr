---
title: Azure 플랜 - 구독 및 리소스 관리
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너가 다양한 RBAC(역할 기반 액세스 제어) 옵션을 사용하여 고객의 Azure 리소스에 대한 운영 제어 및 관리를 얻는 방법에 대해 알아봅니다.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534933"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a><span data-ttu-id="35acd-103">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="35acd-103">Manage subscriptions and resources under the Azure plan</span></span>

<span data-ttu-id="35acd-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="35acd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="35acd-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="35acd-105">Admin agent</span></span>


<span data-ttu-id="35acd-106">이 문서에서는 CSP 파트너가 다양한 RBAC(역할 기반 액세스 제어) 옵션을 사용하여 고객의 Azure 리소스를 운영 제어하고 관리하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-106">This article explains how CSP partners can use different role-based access control (RBAC) options to gain operational control and management of a customer's Azure resources.</span></span> <span data-ttu-id="35acd-107">고객을 Azure 플랜으로 전환하면 기본적으로 Azure에서 권한 있는 관리자 권한(대신 관리를 통한 구독 소유자 권한)이 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-107">When you transition a customer to the Azure plan, you are assigned privileged admin rights in Azure (subscription owner rights through admin on behalf of) by default.</span></span>

 > [!NOTE]
 > <span data-ttu-id="35acd-108">Azure 구독에 대한 관리자 권한은 고객이 구독, 리소스 그룹 또는 워크로드 수준에서 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-108">Admin rights to the Azure subscription can be removed by the customer at a subscription, resource group, or workload level.</span></span> 

 <span data-ttu-id="35acd-109">파트너는 RBAC(역할 기반 액세스 제어) 기능을 통해 제공되는 다양한 옵션을 사용하여 CSP에서 고객 Azure 리소스를 연중무휴 제어하고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-109">Partners can gain 24x7 operational control and management of a customer's Azure resources in CSP by using different options provided through the role-based access control feature (RBAC).</span></span> 

- <span data-ttu-id="35acd-110">**AOBO(관리자 위임)** – [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)를 사용하면 파트너 테넌트에서 관리 에이전트 역할이 있는 모든 사용자는 CSP 프로그램을 통해 만드는 Azure 구독에 대한 RBAC 소유자 액세스 권한을 갖게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-110">**Admin on Behalf Of (AOBO)** - With [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), any user with the Admin Agent role in the partner tenant will have RBAC owner access to Azure subscriptions that you create through the CSP program.</span></span>

- <span data-ttu-id="35acd-111">**Azure Lighthouse**: AOBO는 여러 고객을 대상으로 작동하는 별도의 그룹을 만들거나 그룹 또는 사용자에 대해 여러 역할을 사용할 수 있는 유연성을 허용하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-111">**Azure Lighthouse**: AOBO doesn't allow the flexibility to create distinct groups that work with different customers, or to enable different roles for groups or users.</span></span> <span data-ttu-id="35acd-112">Azure Lighthouse를 사용하면 여러 그룹을 여러 고객 또는 역할에 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-112">Using Azure Lighthouse, you can assign different groups to different customers or roles.</span></span> <span data-ttu-id="35acd-113">사용자는 Azure 위임된 리소스 관리를 통해 적절한 수준의 액세스 권한을 갖게 되므로 관리 에이전트 역할이 있는(따라서 전체 AOBO 액세스 권한을 갖는) 사용자 수를 줄일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-113">Because users will have the appropriate level of access through Azure delegated resource management, you can reduce the number of users who have the Admin Agent role (and thus have full AOBO access).</span></span> <span data-ttu-id="35acd-114">이렇게 하면 고객 리소스에 대한 불필요한 액세스를 제한하여 보안을 향상할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-114">This helps improve security by limiting unnecessary access to your customers' resources.</span></span> <span data-ttu-id="35acd-115">또한 유연성이 향상되어 여러 고객을 대규모로 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-115">It also gives you more flexibility to manage multiple customers at scale.</span></span> <span data-ttu-id="35acd-116">자세한 내용은 [Azure Lighthouse 및 클라우드 솔루션 공급자 프로그램](/azure/lighthouse/concepts/cloud-solution-provider)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-116">For more information, read [Azure Lighthouse and the Cloud Solution Provider program](/azure/lighthouse/concepts/cloud-solution-provider).</span></span>

- <span data-ttu-id="35acd-117">**디렉터리 또는 게스트 사용자 또는 [서비스 사용자](/azure/active-directory/develop/app-objects-and-service-principals)** : 고객 디렉터리에 사용자를 추가하거나 게스트 사용자를 추가하고 특정 RBAC 역할을 할당하여 CSP 구독에 대한 세밀한 액세스 권한을 위임할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-117">**Directory or Guest Users or [Service Principals](/azure/active-directory/develop/app-objects-and-service-principals)**: You can delegate granular access to CSP subscriptions by adding users in the customer directory or adding guest users and assigning specific RBAC roles.</span></span>

<span data-ttu-id="35acd-118">보안을 위해 사용자에게 작업 수행에 필요한 최소한의 권한만 부여하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-118">Microsoft recommends that users have the minimum permissions they need to perform their work as a security practice.</span></span> <span data-ttu-id="35acd-119">[Azure Active Directory 권한 있는 ID 관리 리소스](/azure/active-directory/privileged-identity-management/pim-configure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-119">See [Azure Active Directory Privileged Identity Management resources](/azure/active-directory/privileged-identity-management/pim-configure).</span></span>

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a><span data-ttu-id="35acd-120">고객의 Azure 리소스를 관리할 수 있도록 파트너 ID(MPN ID)를 자격 증명에 연결하세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-120">Link your partner ID (MPN ID)to your credentials for managing customer's Azure resources</span></span>

<span data-ttu-id="35acd-121">다음 표에서는 파트너 ID를 다양한 RBAC 액세스 옵션과 연결하는 데 사용되는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-121">The following table shows the methods used to associate your partner ID with various RBAC access options.</span></span>

|<span data-ttu-id="35acd-122">**범주**</span><span class="sxs-lookup"><span data-stu-id="35acd-122">**Category**</span></span>   |<span data-ttu-id="35acd-123">**시나리오**</span><span class="sxs-lookup"><span data-stu-id="35acd-123">**Scenario**</span></span>   |<span data-ttu-id="35acd-124">**MPN ID 연결**</span><span class="sxs-lookup"><span data-stu-id="35acd-124">**MPN ID association**</span></span>|
|-----------------|:------------------------|:------------------|
|<span data-ttu-id="35acd-125">AOBO</span><span class="sxs-lookup"><span data-stu-id="35acd-125">AOBO</span></span>   |<span data-ttu-id="35acd-126">CSP 직접 파트너 또는 간접 공급자는 고객용 구독을 만들고 AOBO를 사용하여 CSP 직접 파트너 또는 간접 공급자를 구독의 기본 소유자로 만듭니다. CSP 직접 파트너 또는 간접 공급자는 AOBO를 사용하여 구독에 대한 간접 재판매인 액세스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-126">CSP direct partner or indirect provider creates the subscription for the customer making the CSP direct partner or indirect provider default owner of the subscription using AOBO.; CSP direct partner or indirect provider give indirect reseller access to the subscription using AOBO.</span></span>|<span data-ttu-id="35acd-127">자동(파트너 작업 필요 없음)</span><span class="sxs-lookup"><span data-stu-id="35acd-127">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="35acd-128">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="35acd-128">Azure Lighthouse</span></span>|<span data-ttu-id="35acd-129">파트너가 [Marketplace에 새 관리형 서비스 제품](/azure/lighthouse/concepts/managed-services-offers)을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-129">Partner creates a new [Managed Services offer in Marketplace](/azure/lighthouse/concepts/managed-services-offers).</span></span> <span data-ttu-id="35acd-130">이 제품은 CSP 구독에서 허용되고 파트너는 CSP 구독에 대한 액세스 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-130">This offer is accepted on the CSP subscription and partner gets access to the CSP subscription.</span></span>|<span data-ttu-id="35acd-131">자동(파트너 작업 필요 없음)</span><span class="sxs-lookup"><span data-stu-id="35acd-131">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="35acd-132">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="35acd-132">Azure Lighthouse</span></span>|<span data-ttu-id="35acd-133">파트너가 Azure 구독에서 [ARM 템플릿](/azure/lighthouse/how-to/onboard-customer)을 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-133">Partner deploys [ARM template](/azure/lighthouse/how-to/onboard-customer) in Azure subscription</span></span>|<span data-ttu-id="35acd-134">파트너는 MPN ID를 파트너 테넌트의 사용자 또는 서비스 사용자에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-134">Partner needs to associate the MPN ID to the user or service principal in the partner tenant.</span></span> <span data-ttu-id="35acd-135">자세한 내용은 [파트너 ID 연결](/azure/billing/billing-partner-admin-link-started)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-135">For more information - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).</span></span>|
|<span data-ttu-id="35acd-136">디렉터리 또는 게스트 사용자</span><span class="sxs-lookup"><span data-stu-id="35acd-136">Directory or guest user</span></span>|<span data-ttu-id="35acd-137">파트너는 고객 디렉터리에 새 사용자 또는 서비스 사용자를 만들고 사용자에게 CSP 구독에 대한 액세스 권한을 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-137">Partner creates a new user or service principal in the customer directory and gives access to the CSP subscription to the user.</span></span> <span data-ttu-id="35acd-138">파트너는 고객 디렉터리에 새 사용자 또는 서비스 사용자를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-138">Partner creates a new user or service principal in the customer directory.</span></span> <span data-ttu-id="35acd-139">파트너는 사용자를 그룹에 추가하고 해당 그룹에 CSP 구독에 대한 액세스 권한을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-139">Partner adds the user to a group and gives access to the CSP subscription to the group.</span></span>|<span data-ttu-id="35acd-140">파트너는 MPN ID를 고객 테넌트의 사용자 또는 서비스 사용자에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-140">Partner needs to associate the MPN ID to the user or service principal in the customer tenant.</span></span> <span data-ttu-id="35acd-141">자세한 내용은 [파트너 ID 연결](/azure/billing/billing-partner-admin-link-started)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-141">For more information - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).</span></span>|

## <a name="confirm-that-you-have-admin-access"></a><span data-ttu-id="35acd-142">관리자 액세스 권한이 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="35acd-142">Confirm that you have admin access</span></span>

<span data-ttu-id="35acd-143">고객이 보유한 서비스와 획득한 크레딧을 관리하려면 관리자 액세스 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-143">You require admin access to manage your customer's services and to received earned credits.</span></span> <span data-ttu-id="35acd-144">획득한 크레딧에 대한 자세한 내용은 [파트너 획득 크레딧](partner-earned-credit.md)을 읽어 보세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-144">Read [Partner earned credits](partner-earned-credit.md) for detailed information on earned credits.</span></span> <span data-ttu-id="35acd-145">관리자 액세스 권한이 있는지 확인하는 두 가지 방법이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-145">You have two ways to make sure you know that you have admin access.</span></span>

- <span data-ttu-id="35acd-146">일별 사용량 파일 검토 - 일일 사용량 파일 내의 단가 및 유효 단가를 검토하고 할인이 적용되는지 확인하여 관리자 액세스 권한이 있는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-146">Review the daily usage file - This can be determined by reviewing the unit price and effective unit price within the daily usage file and confirming if a discount is being applied.</span></span> <span data-ttu-id="35acd-147">할인을 받고 있다면 현재 관리자입니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-147">If you are receiving the discount you are the admin.</span></span>

- <span data-ttu-id="35acd-148">Azure 모니터 경고 만들기 - CSP 구독에서 RBAC 액세스가 제거될 때 알림을 받도록 Azure Monitor 활동 로그 [경고](/azure/azure-monitor/platform/alerts-activity-log)를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-148">Create an Azure monitor alert - You can create an Azure Monitor activity log [alert](/azure/azure-monitor/platform/alerts-activity-log) to be notified of  when your RBAC access is removed from CSP subscription.</span></span>

### <a name="create-an-azure-monitor-alert"></a><span data-ttu-id="35acd-149">Azure 모니터 경고 만들기</span><span class="sxs-lookup"><span data-stu-id="35acd-149">Create an Azure monitor alert</span></span>

1. <span data-ttu-id="35acd-150">경고를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-150">Create alert.</span></span>

   :::image type="content" source="images/azure/azurealert1.png" alt-text="azure 경고":::

2. <span data-ttu-id="35acd-152">경고를 발생시킬 작업 유형을 선택합니다. 예를 들어 이메일을 원하는 것으로 지정하는 경우 역할 할당 삭제가 발생하면 알려주는 이메일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-152">Select the type of action you want the alert to take.For example, if you specify that you want an email, you will receive an email notifying you if any role assignment deletion occurs.</span></span>

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="경고 구성":::

### <a name="aobo-removal"></a><span data-ttu-id="35acd-154">AOBO 제거</span><span class="sxs-lookup"><span data-stu-id="35acd-154">AOBO removal</span></span>

<span data-ttu-id="35acd-155">고객은 Azure Portal에서 **액세스 제어** 로 이동하여 구독에 대한 액세스를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-155">Customers can manage access to their subscriptions by going to **Access Control** on the Azure portal.</span></span> <span data-ttu-id="35acd-156">고객이 **역할 할당** 탭에서 **액세스 제거** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-156">From the **Role assignments** tab, they select **Remove access**.</span></span> <span data-ttu-id="35acd-157">이 경우 다음과 같은 조치를 취할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-157">If this happens, you can:</span></span>

- <span data-ttu-id="35acd-158">고객에게 연락하여 관리자 액세스를 복구할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-158">Talk with your customer to see if admin access can be reinstated.</span></span>

- <span data-ttu-id="35acd-159">[RBAC(역할 기반 액세스 제어)](/azure/role-based-access-control/overview)를 통해 제공되는 액세스 권한을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-159">Use the access provided through [role-based access control (RBAC)](/azure/role-based-access-control/overview).</span></span>

- <span data-ttu-id="35acd-160">[Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/)를 통해 제공되는 액세스 권한을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-160">Use access provided through [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).</span></span>

<span data-ttu-id="35acd-161">역할 기반 액세스는 관리자 액세스와 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-161">Role-based access differs from admin access.</span></span> <span data-ttu-id="35acd-162">역할은 수행할 수 있는 작업과 수행할 수 없는 작업의 범위를 정확하게 구분합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-162">Roles delimit precisely what you can and can't do.</span></span> <span data-ttu-id="35acd-163">관리자 액세스는 좀 더 광범위합니다.</span><span class="sxs-lookup"><span data-stu-id="35acd-163">Admin access is broader.</span></span>

<span data-ttu-id="35acd-164">PEC를 얻을 수 있는 역할에 대해 알아보려면 [파트너 획득 크레딧에 대한 역할 및 권한](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)을 읽어 보세요.</span><span class="sxs-lookup"><span data-stu-id="35acd-164">To see the roles eligible to earn PEC, read [Roles and permissions for the partner earned credit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).</span></span>

## <a name="next-steps"></a><span data-ttu-id="35acd-165">다음 단계</span><span class="sxs-lookup"><span data-stu-id="35acd-165">Next steps</span></span>

- [<span data-ttu-id="35acd-166">Azure CSP 구독에 대한 관리자 권한 철회 및 복구</span><span class="sxs-lookup"><span data-stu-id="35acd-166">Revoking and reinstating admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)

- [<span data-ttu-id="35acd-167">파트너 획득 크레딧 - 개요</span><span class="sxs-lookup"><span data-stu-id="35acd-167">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- [<span data-ttu-id="35acd-168">관리형 서비스에 대한 파트너 획득 크레딧</span><span class="sxs-lookup"><span data-stu-id="35acd-168">Partner earned credit for managed services</span></span>](partner-earned-credit-explanation.md)