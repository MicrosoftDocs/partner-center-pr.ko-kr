---
title: 파트너 센터 계정에 테 넌 트 추가
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 계정에서 여러 Azure AD 테 넌 트를 추가, 통합 또는 관리 하는 방법 및이를 수행 하는 이유를 알아봅니다.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151205"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="cf1a9-103">파트너 센터 계정에서 여러 테 넌 트 추가 및 관리</span><span class="sxs-lookup"><span data-stu-id="cf1a9-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="cf1a9-104">**적절 한 역할**: 전역 관리자 | 계정 관리자</span><span class="sxs-lookup"><span data-stu-id="cf1a9-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="cf1a9-105">이 문서에서는 회사에 대해 여러 Azure Active Directory (Azure AD) 테 넌 트를 통합 한 다음 파트너 센터 계정에서 추가 하 고 관리 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="cf1a9-106">이 작업을 수행 하는 데는 여러 가지 이유가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-106">There are many reasons to do so.</span></span> <span data-ttu-id="cf1a9-107">예를 들면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-107">For example:</span></span>

- <span data-ttu-id="cf1a9-108">Contoso가 다른 회사인 Fabrikam을 획득 했다고 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="cf1a9-109">두 회사를 분리 하 여 새 직원이 파트너 센터를 사용할 수 있도록 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="cf1a9-110">이 경우 새 회사의 Azure AD 테 넌 트를 파트너 전역 계정 (표준)과 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="cf1a9-111">이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="cf1a9-112">둘 이상의 테 넌 트 (예: *contoso.com*, *contoso.uk* 및 *contoso.in*)를 사용 하 여 비즈니스를 실행 하는 경우 배포할지에를 사용 하 여 동일한 PC 계정으로 그룹화 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="cf1a9-113">인수 및 합병 지침이 두 회사의 테 넌 트로 작업 해야 하는 경우 *constoso.com* 및 *fabrikam.com* 테 넌 트를 모두 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="cf1a9-114">테 넌 트의 사용자는 다음을 수행할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="cf1a9-115">교육, 디지털 다운로드 또는 Microsoft 공인 전문가 (MCP) 연결을 위한 파트너 센터에 액세스 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="cf1a9-116">Microsoft 파트너 네트워크 (MPN) 관리자 또는 성과급 관리자와 같은 파트너 센터 역할을 할당 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="cf1a9-117">계정에 Azure AD 테 넌 트 추가</span><span class="sxs-lookup"><span data-stu-id="cf1a9-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="cf1a9-118">[Microsoft 파트너 센터](https://partner.microsoft.com/dashboard)에 전역 관리자 권한으로 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="cf1a9-119">오른쪽 위에서 **설정** 을 선택 하 고 **계정 설정** 을 선택한 다음 **테 넌 트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD 프로필 창에 있는 연결 단추의 스크린샷"::: 

1. <span data-ttu-id="cf1a9-121">**연결** 을 선택한 다음 연결 하려는 테 넌 트를 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="cf1a9-122">프롬프트에서 연결하려는 테넌트에서 전역 관리자로 로그인한 다음, **확인을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="새 Azure AD 연결 확인 창의 확인 단추 스크린샷."::: 

   <span data-ttu-id="cf1a9-124">연결을 확인하면 **모든 집합** 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="cf1a9-125">새로 추가된 테넌트 를 보려면 **테넌트 관리로 돌아가기를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="cf1a9-126">테넌트는 이미 다른 파트너 센터 계정에 연결된 경우 계정과 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="cf1a9-127">계정에서 테넌트 제거</span><span class="sxs-lookup"><span data-stu-id="cf1a9-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="cf1a9-128">[Microsoft 파트너 센터](https://partner.microsoft.com/dashboard)전역 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="cf1a9-129">오른쪽 위에서 **설정** 아이콘을 선택한 다음, **계정 설정 을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="cf1a9-130">왼쪽 창에서 **테넌트 를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="cf1a9-131">**Azure AD 테넌트 관리에서** **파트너** 탭을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="cf1a9-132">**연결을 제거하려는** 테넌트 옆에 있는 제거를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="현재 테넌트 연결 및 해당 제거 링크의 스크린샷.":::

   <span data-ttu-id="cf1a9-134">앞의 스크린샷에 표시된 것처럼 주 테넌트 및 현재 로그인한 테넌트만 제외하고 연결된 모든 테넌트에서 **제거** 링크를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="cf1a9-135">테넌트를 제거하면 해당 테넌트의 사용자는 더 이상 파트너 센터 계정에 액세스할 수 없으며 제거는 역량에 영향을 미칠 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf1a9-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="cf1a9-136">다음 단계</span><span class="sxs-lookup"><span data-stu-id="cf1a9-136">Next steps</span></span>

- [<span data-ttu-id="cf1a9-137">사용자 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="cf1a9-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






