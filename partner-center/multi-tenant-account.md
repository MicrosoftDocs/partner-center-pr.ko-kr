---
title: 파트너 센터 계정에 테 넌 트 추가
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 계정에서 여러 Azure AD 테 넌 트를 추가, 통합 또는 관리 하는 방법을 알아봅니다. 또한이 작업을 수행 하는 몇 가지 이유에 대해 알아보세요.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175165"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="67d5a-104">파트너 센터 계정에서 여러 테 넌 트 추가 및 관리</span><span class="sxs-lookup"><span data-stu-id="67d5a-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="67d5a-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="67d5a-105">**Applies to**</span></span>

- <span data-ttu-id="67d5a-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="67d5a-106">Partner Center</span></span>

<span data-ttu-id="67d5a-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="67d5a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="67d5a-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="67d5a-108">Global admin</span></span>

<span data-ttu-id="67d5a-109">이 기능을 사용하여 회사의 여러 테넌트를 관리하고 파트너 센터 계정에 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="67d5a-110">파트너 센터 계정에서 여러 Azure AD 테 넌 트를 관리 해야 하는 이유는 여러 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="67d5a-111">예를 들면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-111">For example:</span></span>

- <span data-ttu-id="67d5a-112">회사에서 다른 회사를 구입할 수 있으며, 새 회사 직원 들이 파트너 센터를 사용할 수 있도록 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="67d5a-113">그러나 두 회사를 분리 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="67d5a-114">이 경우 새 회사의 Azure AD 테 넌 트를 파트너의 글로벌 계정 (표준)과 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="67d5a-115">이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="67d5a-116">비즈니스를 실행 하는 데 둘 이상의 테 넌 트가 있는 경우 (예: contoso.com, contoso.uk, contoso.in) 다중 테 넌 트를 사용 하 여 동일한 PC 계정에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="67d5a-117">인수를 합병 하려면 둘 이상의 테 넌 트를 사용 해야 합니다 (예: Contoso가 Fabrikam을 획득 하는 경우 Constoso.com 및 Fabrikam.com 각 테 넌 트를 모두 사용할 수 있어야 함).</span><span class="sxs-lookup"><span data-stu-id="67d5a-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="67d5a-118">테 넌 트의 사용자는 다음을 수행할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="67d5a-119">교육, 디지털 다운로드, MCP 연결을 위한 파트너 센터 액세스</span><span class="sxs-lookup"><span data-stu-id="67d5a-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="67d5a-120">MPN Admin, 성과급 관리자 등과 같은 파트너 센터 역할을 할당 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="67d5a-121">계정에 다른 Azure AD 테 넌 트 추가</span><span class="sxs-lookup"><span data-stu-id="67d5a-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="67d5a-122">전역 관리자 권한으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="67d5a-123">**설정** 아이콘에서 **계정 설정** 을 선택 하 고 **테 넌 트**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-123">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="테 넌 트 연결"::: 

3. <span data-ttu-id="67d5a-125">**다른 AD 테 넌 트 연결** 을 선택 하 고 연결 하려는 테 넌 트를 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="67d5a-126">전역 관리자 권한으로 연결 하려는 테 넌 트에 로그인 하 고 연결을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="테 넌 트 연결"::: 

5. <span data-ttu-id="67d5a-128">확인 한 후에는 **모든 설정** 된 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="67d5a-129">**테 넌 트 관리로 돌아가기** 를 선택 하면 새로 추가 된 테 넌 트가 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="67d5a-130">다른 파트너 센터 계정에 이미 연결 되어 있는 경우에는 테 넌 트를 계정에 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="67d5a-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="67d5a-131">다음 단계</span><span class="sxs-lookup"><span data-stu-id="67d5a-131">Next steps</span></span>

- [<span data-ttu-id="67d5a-132">사용자 추가</span><span class="sxs-lookup"><span data-stu-id="67d5a-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
