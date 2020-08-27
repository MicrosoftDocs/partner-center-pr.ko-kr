---
title: 사용자 계정 만들기 및 역할 할당
description: 파트너 센터에 액세스하기 전에 모든 직원에게 역할을 할당해야 합니다. 사용자 계정을 만들고, 역할을 할당하고, 사용 권한을 설정하는 방법에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: f71df7df213b2c6410fab37ce323825511a18b6d
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846933"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="da61c-104">사용자 계정 만들기 및 역할과 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="da61c-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="da61c-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="da61c-105">**Appropriate roles**</span></span>

- <span data-ttu-id="da61c-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-106">Account admin</span></span>
- <span data-ttu-id="da61c-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-107">Global admin</span></span>
- <span data-ttu-id="da61c-108">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="da61c-108">User management admin</span></span>

<span data-ttu-id="da61c-109">파트너 센터에 액세스해야 하는 직원의 사용자 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="da61c-110">이러한 작업은 사용자 관리, 계정 관리 또는 글로벌 관리 권한이 있는 관리자가 수행해야 합니다. 이러한 작업을 수행하는 사용자에게는 사용자 관리자 또는 글로벌 관리자의 AAD(Azure Active Directory) 역할도 할당되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="da61c-111">AAD 역할에 대한 자세한 내용은 [Azure Active Directory의 관리자 역할 권한](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="da61c-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="da61c-112">새 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="da61c-112">Add a new user</span></span>

1. <span data-ttu-id="da61c-113">파트너 센터 오른쪽 위의 **설정** 아이콘에서 **사용자 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="da61c-114">**사용자 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-114">Select **Add user**.</span></span>

3. <span data-ttu-id="da61c-115">사용자의 전체 이름과 고유의 이메일 주소를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="da61c-116">에이전트 유형 및/또는 사용자에게 할당할 관리자 유형을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="da61c-117">파트너 센터 액세스는 역할 기반이므로 사용자가 특정 작업을 완료하는 데 필요한 기능만 표시하도록 사용자의 보기를 사용자 지정하는 권한을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="da61c-118">역할 할당을 원하는 사용자는 **사용자 관리**로 이동하여 글로벌 관리자에 대한 필터링을 수행하여 연락할 글로벌 관리자를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="da61c-119">**추가**를 선택하여 사용자 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="da61c-120">다음 페이지에서 사용자의 세부 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="da61c-121">이 페이지에 표시되는 새 사용자의 로그인 정보를 기록해 두세요.</span><span class="sxs-lookup"><span data-stu-id="da61c-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="da61c-122">나중에 이 정보에 다시 액세스할 수 없으므로 이 정보를 복사하여 새 사용자에게 보내야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="da61c-123">사용자는 사용자 이름 및 임시 암호를 사용하여 파트너 센터에 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="da61c-124">사용자가 파트너 센터에 처음으로 로그인하면 암호를 변경하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="da61c-125">할당된 역할 찾기</span><span class="sxs-lookup"><span data-stu-id="da61c-125">Find the role you've been assigned</span></span>

<span data-ttu-id="da61c-126">전역 관리자가 알려주지 않은 경우 다음을 수행하여 파트너 센터에서 어떤 역할을 수행하는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="da61c-127">파트너 센터 [대시보드]https://partner.microsoft.com/dashboard/home) 에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="da61c-128">**계정 설정** 아이콘을 선택한 다음, **내 프로필**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="da61c-129">**역할 및 권한** 탭을 선택합니다. 사용자의 역할 및 권한이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="da61c-130">로그인할 때 프로그램이 표시되지 않으면 일반적으로 해당 프로그램에서 사용할 수 있는 올바른 권한이 없음을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="da61c-131">따라서, 예를 들어 로그인할 때 인센티브 페이지가 표시되지 않는다면 인센티브 권한이 없는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="da61c-132">전역 관리자는 필요한 권한을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="da61c-133">글로벌 관리자 찾기</span><span class="sxs-lookup"><span data-stu-id="da61c-133">Find your global admin</span></span>

<span data-ttu-id="da61c-134">사용자가 역할을 변경해야 하거나 새 사용자가 특정 역할 할당을 원하는 경우가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="da61c-135">역할을 변경하거나 새 사용자에게 역할을 할당할 수 있는 전역 관리자를 찾으려면 파트너 센터의 오른쪽 상단에 있는 **계정 설정 아이콘**에서 **사용자 관리**를 선택하고 전역 관리자에 대해 필터링하거나 **내 프로필**로 이동하여 **역할 및 권한**을 선택하고 권한을 높이는 데 도움을 줄 수 있는 여러 관리자 목록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="da61c-136">새 글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-136">New global admin</span></span>

<span data-ttu-id="da61c-137">글로벌 관리자가 조직을 떠나고 다른 사용자가 이 역할을 수행해야 하는 경우 Azure 또는 Office 365 팀에 티켓을 제출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="da61c-138">이 작업을 수행하는 방법에 대한 자세한 내용을 보려면 아래 옵션 중 하나를 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="da61c-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="da61c-139">Azure의 새 글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="da61c-140">Office 365의 새 글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="da61c-141">사용자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="da61c-141">Assign user roles</span></span>

<span data-ttu-id="da61c-142">파트너 센터에서 작업하려면 할당된 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="da61c-143">현재 역할에는 Azure Active Directory 테넌트 역할, CSP(클라우드 솔루션 공급자) 역할 및 비 AAD 회사 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="da61c-144">개별 회사에 이러한 모든 역할이 필요할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="da61c-145">파트너 센터에 액세스하려면 개별 회사가 테넌트에 나열되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="da61c-146">역할 할당은 추가 액세스 권한을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="da61c-147">**AAD 테넌트 역할에는 다음이 포함됩니다**.</span><span class="sxs-lookup"><span data-stu-id="da61c-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="da61c-148">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-148">Global admin</span></span>
- <span data-ttu-id="da61c-149">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-149">User admin</span></span>

<span data-ttu-id="da61c-150">**CSP 역할에는 다음이 포함됩니다**.</span><span class="sxs-lookup"><span data-stu-id="da61c-150">**CSP roles include**:</span></span>
- <span data-ttu-id="da61c-151">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="da61c-151">Admin agent</span></span>
- <span data-ttu-id="da61c-152">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-152">Billing admin</span></span>
- <span data-ttu-id="da61c-153">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="da61c-153">Sales agent</span></span>
- <span data-ttu-id="da61c-154">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="da61c-154">Helpdesk agent</span></span>

<span data-ttu-id="da61c-155">**MPN 멤버십과 회사를 관리하는 역할(비 AAD)**</span><span class="sxs-lookup"><span data-stu-id="da61c-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="da61c-156">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-156">MPN partner admin</span></span>
- <span data-ttu-id="da61c-157">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-157">Account admin</span></span>
- <span data-ttu-id="da61c-158">추천 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-158">Referral admin</span></span>
- <span data-ttu-id="da61c-159">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-159">Business profile admin</span></span>
- <span data-ttu-id="da61c-160">인센티브 관리자 및 사용자</span><span class="sxs-lookup"><span data-stu-id="da61c-160">Incentives admin and user</span></span>

<span data-ttu-id="da61c-161">**제어판 공급업체는 CSP 및 비 AAD 역할입니다**.</span><span class="sxs-lookup"><span data-stu-id="da61c-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="da61c-162">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="da61c-162">Global admin</span></span>

<span data-ttu-id="da61c-163">**게스트 사용자**은 AAD 테넌트의 일부여야 하며 모든 비 AAD 역할을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="da61c-164">역할과 각 역할이 수행할 수 있는 작업에 대한 자세한 내용은 [사용자 권한 할당](permissions-overview.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="da61c-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="da61c-165">파트너 센터에서 사용자의 Microsoft Learn 계정 연결</span><span class="sxs-lookup"><span data-stu-id="da61c-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="da61c-166">사용자가 역량 달성을 위해 취하고 있는 교육 및 학습 경로를 볼 수 있으려면 해당 MCP ID를 파트너 센터 계정에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="da61c-167">글로벌 관리자로서, 새 사용자를 추가할 때 계정에 MCP ID를 연결하도록 알려 주어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="da61c-168">파트너 센터 계정에 MCP ID를 연결하는 방법</span><span class="sxs-lookup"><span data-stu-id="da61c-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="da61c-169">파트너 센터 대시보드에서, 대시보드 오른쪽 모서리에 있는 **계정** 아이콘을 선택한 다음, **내 프로필**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="da61c-170">**학습** 아래에서 Microsoft Learning 계정을 연결할 수 있으며, 또한 Microsoft 계정을 파트너 대학에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="da61c-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="da61c-171">다음 단계</span><span class="sxs-lookup"><span data-stu-id="da61c-171">Next steps</span></span>

- [<span data-ttu-id="da61c-172">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="da61c-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)