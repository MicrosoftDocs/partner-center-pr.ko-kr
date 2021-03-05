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
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124808"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="bf369-103">파트너 센터 계정에서 여러 테 넌 트 추가 및 관리</span><span class="sxs-lookup"><span data-stu-id="bf369-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="bf369-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="bf369-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bf369-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="bf369-105">Global admin</span></span>
- <span data-ttu-id="bf369-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="bf369-106">Account admin</span></span>

<span data-ttu-id="bf369-107">이 문서에서는 회사에 대해 여러 Azure Active Directory (Azure AD) 테 넌 트를 통합 한 다음 파트너 센터 계정에서 추가 하 고 관리 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="bf369-108">이 작업을 수행 하는 데는 여러 가지 이유가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-108">There are many reasons to do so.</span></span> <span data-ttu-id="bf369-109">예를 들면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-109">For example:</span></span>

- <span data-ttu-id="bf369-110">Contoso가 다른 회사인 Fabrikam을 획득 했다고 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="bf369-111">두 회사를 분리 하 여 새 직원이 파트너 센터를 사용할 수 있도록 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="bf369-112">이 경우 새 회사의 Azure AD 테 넌 트를 파트너 전역 계정 (표준)과 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="bf369-113">이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="bf369-114">둘 이상의 테 넌 트 (예: *contoso.com*, *contoso.uk* 및 *contoso.in*)를 사용 하 여 비즈니스를 실행 하는 경우 배포할지에를 사용 하 여 동일한 PC 계정으로 그룹화 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="bf369-115">인수 및 합병 지침이 두 회사의 테 넌 트로 작업 해야 하는 경우 *constoso.com* 및 *fabrikam.com* 테 넌 트를 모두 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="bf369-116">테 넌 트의 사용자는 다음을 수행할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="bf369-117">교육, 디지털 다운로드 또는 Microsoft 공인 전문가 (MCP) 연결을 위한 파트너 센터에 액세스 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="bf369-118">Microsoft 파트너 네트워크 (MPN) 관리자 또는 성과급 관리자와 같은 파트너 센터 역할을 할당 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="bf369-119">계정에 Azure AD 테 넌 트 추가</span><span class="sxs-lookup"><span data-stu-id="bf369-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="bf369-120">[Microsoft 파트너 센터](https://partner.microsoft.com/dashboard)에 전역 관리자 권한으로 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="bf369-121">오른쪽 위에서 **설정** 을 선택 하 고 **계정 설정** 을 선택한 다음 **테 넌 트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD 프로필 창에 있는 연결 단추의 스크린샷"::: 

1. <span data-ttu-id="bf369-123">**연결** 을 선택한 다음 연결 하려는 테 넌 트를 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="bf369-124">프롬프트에서 연결할 테 넌 트에 대 한 전역 관리자로 로그인 한 다음 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="새 Azure AD 연결 확인 창에 있는 확인 단추의 스크린샷"::: 

   <span data-ttu-id="bf369-126">연결을 확인 한 후에는 **모든 설정** 된 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="bf369-127">새로 추가 된 테 넌 트를 보려면 **테 넌 트 관리로 돌아가기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="bf369-128">다른 파트너 센터 계정에 이미 연결 되어 있는 경우에는 계정과 테 넌 트를 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="bf369-129">계정에서 테 넌 트 제거</span><span class="sxs-lookup"><span data-stu-id="bf369-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="bf369-130">[Microsoft 파트너 센터](https://partner.microsoft.com/dashboard)에 전역 관리자 권한으로 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="bf369-131">오른쪽 위에서 **설정** 아이콘을 선택 하 고 **계정 설정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="bf369-132">왼쪽 창에서 **테 넌 트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="bf369-133">**AZURE AD 테 넌 트 관리** 에서 **파트너** 탭을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="bf369-134">연결을 제거 하려는 테 넌 트 옆에 있는 **제거** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="현재 테 넌 트 연결 및 제거 링크의 스크린샷":::

   <span data-ttu-id="bf369-136">앞의 스크린샷에 표시 된 것 처럼, 현재 로그인 한 기본 테 넌 트 및 테 넌 트를 제외 하 고 모든 연결 된 테 넌 트에 대해 **제거** 링크를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="bf369-137">테 넌 트를 제거 하는 경우 해당 테 넌 트의 사용자는 더 이상 파트너 센터 계정에 액세스할 수 없으며 제거는 역량에 영향을 미칠 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf369-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bf369-138">다음 단계</span><span class="sxs-lookup"><span data-stu-id="bf369-138">Next steps</span></span>

- [<span data-ttu-id="bf369-139">사용자 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="bf369-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






