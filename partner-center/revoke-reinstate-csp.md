---
title: Azure CSP에 대한 관리자 권한 복구
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너가 고객의 Azure CSP 구독을 관리할 수 있도록 고객이 파트너의 관리자 권한을 복구하도록 돕는 방법에 대해 알아봅니다.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855423"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="35007-103">고객의 Azure CSP 구독에 대한 관리자 권한 복구</span><span class="sxs-lookup"><span data-stu-id="35007-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="35007-104">**적절한 역할**: 전역 관리자 | 관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="35007-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="35007-105">CSP 파트너로서 고객은 Azure 사용량과 해당 시스템을 관리할 것으로 기대하는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="35007-106">이렇게 하려면 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="35007-107">고객과의 재판매인 관계가 설정되면 일부 권한이 부여됩니다.</span><span class="sxs-lookup"><span data-stu-id="35007-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="35007-108">다른 권한은 고객이 사용자에게 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="35007-109">CSP의 Azure에 대한 관리자 권한</span><span class="sxs-lookup"><span data-stu-id="35007-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="35007-110">CSP에는 Azure에 대한 다음 두 가지 수준의 관리자 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="35007-111">**테넌트 수준 관리자 권한**(**위임된 관리자 권한**) – CSP 파트너는 고객과의 CSP 재판매인 관계를 설정하면서 이러한 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="35007-112">위임된 관리자 권한을 통해 CSP 파트너는 고객의 테넌트에 액세스할 수 있으므로 사용자 추가/관리, 암호 재설정 및 사용자 라이선스 관리와 같은 관리 기능을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="35007-113">**구독 수준 관리자 권한** – CSP 파트너는 고객에 대한 Azure CSP 구독을 만들면서 이러한 권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="35007-114">이러한 권한이 있으면 CSP 파트너는 이러한 구독에 완전하게 액세스할 수 있으므로 Azure 리소스를 프로비저닝하고 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="35007-115">CSP 파트너의 관리자 권한 복구</span><span class="sxs-lookup"><span data-stu-id="35007-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="35007-116">고객에게 AdminAgents 그룹의 개체 ID를 제공하는 한 고객은 CSP 역할 할당을 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="35007-117">위임된 관리자 권한을 다시 얻으려면 고객과 협력해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="35007-118">파트너 센터 대시보드에 로그인하고, 파트너 센터 메뉴에서 **고객** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="35007-119">협력하는 고객을 선택하고, **재판매인 관계를 요청** 합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="35007-120">이 작업은 테넌트 관리자 권한이 있는 고객에 대한 링크를 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="35007-121">해당 고객은 링크를 선택하고, 재판매인 관계 요청을 승인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="재판매인 관계 만들기의 이메일 예제":::

4. <span data-ttu-id="35007-123">파트너는 AdminAgents 그룹의 개체 ID를 가져오기 위해 파트너 테넌트에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="35007-124">**소유자 또는 사용자 액세스 관리자** 역할을 하며 구독 수준에서 역할 할당을 만들 수 있는 권한이 있는 고객은 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="35007-125">CSP 구독이 있는 테넌트에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="35007-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="35007-126">구독에 연결합니다(사용자에게 테넌트의 여러 구독에 대한 역할 할당 권한이 있는 경우에만 적용 가능).</span><span class="sxs-lookup"><span data-stu-id="35007-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="35007-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="35007-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="35007-128">역할 할당 만들기</span><span class="sxs-lookup"><span data-stu-id="35007-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="35007-129">구독 범위 대신 리소스 그룹 수준 또는 리소스 수준에서 소유자 역할 권한을 부여하려는 경우 다음 명령을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="35007-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="35007-130">다음 단계</span><span class="sxs-lookup"><span data-stu-id="35007-130">Next steps</span></span>

- [<span data-ttu-id="35007-131">Azure 플랜 하에서 구독 및 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="35007-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
