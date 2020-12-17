---
title: Azure CSP에 대한 관리자 권한 복구
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너가 고객의 Azure CSP 구독을 관리할 수 있도록 고객이 파트너의 관리자 권한을 복구하도록 돕는 방법에 대해 알아봅니다.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011505"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="1af99-103">고객의 Azure CSP 구독에 대한 관리자 권한 복구</span><span class="sxs-lookup"><span data-stu-id="1af99-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="1af99-104">**적용 가능한 역할**</span><span class="sxs-lookup"><span data-stu-id="1af99-104">**Applicable roles**</span></span>

- <span data-ttu-id="1af99-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="1af99-105">Global admin</span></span>
- <span data-ttu-id="1af99-106">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="1af99-106">Admin agent</span></span>

<span data-ttu-id="1af99-107">CSP 파트너로서 고객은 Azure 사용량과 해당 시스템을 관리할 것으로 기대하는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="1af99-108">이렇게 하려면 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="1af99-109">고객과의 재판매인 관계가 설정되면 일부 권한이 부여됩니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="1af99-110">다른 권한은 고객이 사용자에게 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="1af99-111">CSP의 Azure에 대한 관리자 권한</span><span class="sxs-lookup"><span data-stu-id="1af99-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="1af99-112">CSP에는 Azure에 대한 다음 두 가지 수준의 관리자 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="1af99-113">**테넌트 수준 관리자 권한**(**위임된 관리자 권한**) – CSP 파트너는 고객과의 CSP 재판매인 관계를 설정하면서 이러한 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="1af99-114">이를 통해 CSP 파트너는 고객의 테넌트에 액세스할 수 있으므로 사용자 추가/관리, 암호 재설정 및 사용자 라이선스 관리와 같은 관리 기능을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="1af99-115">**구독 수준 관리자 권한** – CSP 파트너는 고객에 대한 Azure CSP 구독을 만들면서 이러한 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="1af99-116">이러한 권한이 있으면 CSP 파트너는 이러한 구독에 완전하게 액세스할 수 있으므로 Azure 리소스를 프로비저닝하고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="1af99-117">CSP 파트너의 관리자 권한 복구</span><span class="sxs-lookup"><span data-stu-id="1af99-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="1af99-118">위임된 관리자 권한을 다시 얻으려면 고객과 협력해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="1af99-119">파트너 센터 대시보드에 로그인하고, 파트너 센터 메뉴에서 **고객** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="1af99-120">협력하는 고객을 선택하고, **재판매인 관계를 요청** 합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="1af99-121">그러면 테넌트 관리자 권한이 있는 고객에 대한 링크가 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="1af99-122">해당 사용자는 링크를 선택하고, 재판매인 관계 요청을 승인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="재판매인 관계":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="1af99-124">관리 에이전트 그룹을 Azure CSP 구독 소유자로 추가</span><span class="sxs-lookup"><span data-stu-id="1af99-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="1af99-125">고객은 관리 에이전트 그룹을 Azure CSP 구독, 리소스 그룹 또는 리소스의 소유자로 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-125">Your customer will need to add your admin agent group as the owner of a Azure CSP subscription, a Resource group or a resource.</span></span> 

1. <span data-ttu-id="1af99-126">PowerShell 콘솔 또는 PowerShell ISE(통합 스크립팅 환경)를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="1af99-127">AzureAD 모듈이 설치되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="1af99-128">Azure AD 테넌트에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="1af99-129">관리 에이전트 그룹의 ObjectId를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="1af99-130">다음 단계는 Azure CSP 구독에 대한 소유자 액세스 권한이 있는 고객 회사의 사용자가 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="1af99-131">Azure CSP 구독에 대한 소유자 액세스 권한이 있는 사용자는 자신의 자격 증명을 사용하여 Azure에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzureRmAccount
   ```

5. <span data-ttu-id="1af99-132">그런 다음, 범위 매개 변수에 적절한 리소스 Uri를 적용하여 관리 에이전트 그룹을 CSP Azure 구독, 리소스 그룹 또는 리소스에 소유자로 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1af99-132">She can then add your admin agent group as owner to the CSP Azure subscription, Resource group or Resource by applying a proper Resource Uri in Scope parameter.</span></span> 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a><span data-ttu-id="1af99-133">다음 단계</span><span class="sxs-lookup"><span data-stu-id="1af99-133">Next steps</span></span>

[<span data-ttu-id="1af99-134">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="1af99-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
