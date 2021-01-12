---
title: 파트너 센터 계정에 테 넌 트 추가
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 계정에서 여러 Azure AD 테 넌 트를 추가, 통합 또는 관리 하는 방법을 알아봅니다. 또한이 작업을 수행 하는 몇 가지 이유에 대해 알아보세요.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105558"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="a46d6-104">파트너 센터 계정에서 여러 테 넌 트 추가 및 관리</span><span class="sxs-lookup"><span data-stu-id="a46d6-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="a46d6-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="a46d6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a46d6-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="a46d6-106">Global admin</span></span>

<span data-ttu-id="a46d6-107">이 기능을 사용하여 회사의 여러 테넌트를 관리하고 파트너 센터 계정에 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="a46d6-108">파트너 센터 계정에서 여러 Azure AD 테 넌 트를 관리 해야 하는 이유는 여러 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="a46d6-109">예를 들어:</span><span class="sxs-lookup"><span data-stu-id="a46d6-109">For example:</span></span>

- <span data-ttu-id="a46d6-110">회사에서 다른 회사를 구입할 수 있으며, 새 회사 직원 들이 파트너 센터를 사용할 수 있도록 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="a46d6-111">그러나 두 회사를 분리 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="a46d6-112">이 경우 새 회사의 Azure AD 테 넌 트를 파트너의 글로벌 계정 (표준)과 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="a46d6-113">이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="a46d6-114">비즈니스를 실행 하는 데 둘 이상의 테 넌 트가 있는 경우 (예: contoso.com, contoso.uk, contoso.in) 다중 테 넌 트를 사용 하 여 동일한 PC 계정에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="a46d6-115">인수를 합병 하려면 둘 이상의 테 넌 트를 사용 해야 합니다 (예: Contoso가 Fabrikam을 획득 하는 경우 Constoso.com 및 Fabrikam.com 각 테 넌 트를 모두 사용할 수 있어야 함).</span><span class="sxs-lookup"><span data-stu-id="a46d6-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="a46d6-116">테 넌 트의 사용자는 다음을 수행할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="a46d6-117">교육, 디지털 다운로드, MCP 연결을 위한 파트너 센터 액세스</span><span class="sxs-lookup"><span data-stu-id="a46d6-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="a46d6-118">MPN Admin, 성과급 관리자 등과 같은 파트너 센터 역할을 할당 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="a46d6-119">계정에 다른 Azure AD 테 넌 트 추가</span><span class="sxs-lookup"><span data-stu-id="a46d6-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="a46d6-120">전역 관리자 권한으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="a46d6-121">**설정** 아이콘에서 **계정 설정** 을 선택 하 고 **테 넌 트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="테 넌 트 연결"::: 

3. <span data-ttu-id="a46d6-123">**다른 AD 테 넌 트 연결** 을 선택 하 고 연결 하려는 테 넌 트를 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="a46d6-124">전역 관리자 권한으로 연결 하려는 테 넌 트에 로그인 하 고 연결을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="테 넌 트 연결 확인"::: 

5. <span data-ttu-id="a46d6-126">확인 한 후에는 **모든 설정** 된 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="a46d6-127">**테 넌 트 관리로 돌아가기** 를 선택 하면 새로 추가 된 테 넌 트가 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="a46d6-128">다른 파트너 센터 계정에 이미 연결 되어 있는 경우에는 테 넌 트를 계정에 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="a46d6-129">계정에서 테 넌 트 제거</span><span class="sxs-lookup"><span data-stu-id="a46d6-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="a46d6-130">전역 관리자 권한으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="a46d6-131">**설정** 아이콘에서 **계정 설정** -테 넌 트 >를 선택 하 고 **파트너** 탭을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="a46d6-132">분리 하려는 테 넌 트에 대해 **제거** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="a46d6-133">테 넌 트를 분리 해당 테 넌 트의 사용자가 더 이상 파트너 센터 계정에 액세스할 수 없으며,이로 인해 역량에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="a46d6-134">기본 테 넌 트 및 현재 로그인 한 테 넌 트를 제외한 모든 연결 된 테 넌 트에 대해 **제거** 단추를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a46d6-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="제거 단추가 있는 테 넌 트":::
 

## <a name="next-steps"></a><span data-ttu-id="a46d6-136">다음 단계</span><span class="sxs-lookup"><span data-stu-id="a46d6-136">Next steps</span></span>

- [<span data-ttu-id="a46d6-137">사용자 추가</span><span class="sxs-lookup"><span data-stu-id="a46d6-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






