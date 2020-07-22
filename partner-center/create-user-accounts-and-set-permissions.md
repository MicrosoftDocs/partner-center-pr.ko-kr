---
title: 사용자 계정 만들기 및 역할 할당
description: 파트너 센터에 액세스하기 전에 모든 직원에게 역할을 할당해야 합니다. 사용자 계정을 만들고, 역할을 할당하고, 사용 권한을 설정하는 방법에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: c7d04307be7a81cf3501e1b50e278cf1a012afcd
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435192"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="86be7-104">사용자 계정 만들기 및 역할과 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="86be7-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="86be7-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="86be7-105">**Appropriate roles**</span></span>

- <span data-ttu-id="86be7-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-106">Account admin</span></span>
- <span data-ttu-id="86be7-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-107">Global admin</span></span>
- <span data-ttu-id="86be7-108">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="86be7-108">User management admin</span></span>

<span data-ttu-id="86be7-109">파트너 센터에 액세스해야 하는 직원의 사용자 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="86be7-110">이러한 작업은 사용자 관리, 계정 관리 또는 글로벌 관리 권한이 있는 관리자가 수행해야 합니다. 이러한 작업을 수행하는 사용자에게는 사용자 관리자 또는 글로벌 관리자의 AAD(Azure Active Directory) 역할도 할당되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="86be7-111">AAD 역할에 대한 자세한 내용은 [Azure Active Directory의 관리자 역할 권한](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="86be7-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="86be7-112">새 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="86be7-112">Add a new user</span></span>

1. <span data-ttu-id="86be7-113">파트너 센터 오른쪽 위의 **설정** 아이콘에서 **사용자 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="86be7-114">**사용자 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-114">Select **Add user**.</span></span>

3. <span data-ttu-id="86be7-115">사용자의 전체 이름과 고유의 이메일 주소를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="86be7-116">에이전트 유형 및/또는 사용자에게 할당할 관리자 유형을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="86be7-117">파트너 센터 액세스는 역할 기반이므로 사용자가 특정 작업을 완료하는 데 필요한 기능만 표시하도록 사용자의 보기를 사용자 지정하는 권한을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="86be7-118">역할 할당을 원하는 사용자는 **사용자 관리**로 이동하여 글로벌 관리자에 대한 필터링을 수행하여 연락할 글로벌 관리자를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="86be7-119">**추가**를 선택하여 사용자 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="86be7-120">다음 페이지에서 사용자의 세부 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="86be7-121">이 페이지에 표시되는 새 사용자의 로그인 정보를 기록해 두세요.</span><span class="sxs-lookup"><span data-stu-id="86be7-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="86be7-122">나중에 이 정보에 다시 액세스할 수 없으므로 이 정보를 복사하여 새 사용자에게 보내야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="86be7-123">사용자는 사용자 이름 및 임시 암호를 사용하여 파트너 센터에 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="86be7-124">사용자가 파트너 센터에 처음으로 로그인하면 암호를 변경하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="86be7-125">글로벌 관리자 찾기</span><span class="sxs-lookup"><span data-stu-id="86be7-125">Find your global admin</span></span>

<span data-ttu-id="86be7-126">사용자가 역할을 변경해야 하거나 새 사용자가 특정 역할 할당을 원하는 경우가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-126">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="86be7-127">역할을 변경하거나 새 사용자에게 역할을 할당할 수 있는 글로벌 관리자를 찾으려면 파트너 센터의 오른쪽 위에 있는 **설정 아이콘**에서 **사용자 관리**를 선택하고 글로벌 관리자를 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-127">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="86be7-128">새 글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-128">New global admin</span></span>

<span data-ttu-id="86be7-129">글로벌 관리자가 조직을 떠나고 다른 사용자가 이 역할을 수행해야 하는 경우 Azure 또는 Office 365 팀에 티켓을 제출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-129">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="86be7-130">이 작업을 수행하는 방법에 대한 자세한 내용을 보려면 아래 옵션 중 하나를 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="86be7-130">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="86be7-131">Azure의 새 글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-131">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="86be7-132">Office 365의 새 글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-132">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="86be7-133">사용자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="86be7-133">Assign user roles</span></span>

<span data-ttu-id="86be7-134">파트너 센터에서 작업하려면 할당된 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-134">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="86be7-135">현재 역할에는 Azure Active Directory 테넌트 역할, CSP(클라우드 솔루션 공급자) 역할 및 비 AAD 회사 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-135">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="86be7-136">개별 회사에 이러한 모든 역할이 필요할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-136">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="86be7-137">파트너 센터에 액세스하려면 개별 회사가 테넌트에 나열되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-137">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="86be7-138">역할 할당은 추가 액세스 권한을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-138">Role assignments provide additional access.</span></span>


<span data-ttu-id="86be7-139">**AAD 테넌트 역할에는 다음이 포함됩니다**.</span><span class="sxs-lookup"><span data-stu-id="86be7-139">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="86be7-140">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-140">Global admin</span></span>
- <span data-ttu-id="86be7-141">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-141">User admin</span></span>

<span data-ttu-id="86be7-142">**CSP 역할에는 다음이 포함됩니다**.</span><span class="sxs-lookup"><span data-stu-id="86be7-142">**CSP roles include**:</span></span>
- <span data-ttu-id="86be7-143">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="86be7-143">Admin agent</span></span>
- <span data-ttu-id="86be7-144">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-144">Billing admin</span></span>
- <span data-ttu-id="86be7-145">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="86be7-145">Sales agent</span></span>
- <span data-ttu-id="86be7-146">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="86be7-146">Helpdesk agent</span></span>

<span data-ttu-id="86be7-147">**MPN 멤버십과 회사를 관리하는 역할(비 AAD)**</span><span class="sxs-lookup"><span data-stu-id="86be7-147">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="86be7-148">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-148">MPN partner admin</span></span>
- <span data-ttu-id="86be7-149">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-149">Account admin</span></span>
- <span data-ttu-id="86be7-150">추천 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-150">Referral admin</span></span>
- <span data-ttu-id="86be7-151">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-151">Business profile admin</span></span>
- <span data-ttu-id="86be7-152">인센티브 관리자 및 사용자</span><span class="sxs-lookup"><span data-stu-id="86be7-152">Incentives admin and user</span></span>

<span data-ttu-id="86be7-153">**제어판 공급업체는 CSP 및 비 AAD 역할입니다**.</span><span class="sxs-lookup"><span data-stu-id="86be7-153">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="86be7-154">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="86be7-154">Global admin</span></span>

<span data-ttu-id="86be7-155">**게스트 사용자**은 AAD 테넌트의 일부여야 하며 모든 비 AAD 역할을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-155">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="86be7-156">역할과 각 역할이 수행할 수 있는 작업에 대한 자세한 내용은 [사용자 권한 할당](permissions-overview.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="86be7-156">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="86be7-157">파트너 센터에서 사용자의 Microsoft Learn 계정 연결</span><span class="sxs-lookup"><span data-stu-id="86be7-157">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="86be7-158">사용자가 역량 달성을 위해 취하고 있는 교육 및 학습 경로를 볼 수 있으려면 해당 MCP ID를 파트너 센터 계정에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-158">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="86be7-159">글로벌 관리자로서, 새 사용자를 추가할 때 계정에 MCP ID를 연결하도록 알려 주어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-159">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="86be7-160">파트너 센터 계정에 MCP ID를 연결하는 방법</span><span class="sxs-lookup"><span data-stu-id="86be7-160">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="86be7-161">파트너 센터 대시보드에서, 대시보드 오른쪽 모서리에 있는 **계정** 아이콘을 선택한 다음, **내 프로필**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-161">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="86be7-162">**학습** 아래에서 Microsoft Learning 계정을 연결할 수 있으며, 또한 Microsoft 계정을 파트너 대학에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="86be7-162">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
