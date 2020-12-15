---
title: 사용자 계정 만들기 및 역할 할당
description: 파트너 센터에 액세스하기 전에 모든 직원에게 역할을 할당해야 합니다. 사용자 계정을 만들고, 역할을 할당하고, 사용 권한을 설정하는 방법에 대해 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492537"
---
# <a name="create-user-accounts"></a><span data-ttu-id="0b209-104">사용자 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="0b209-104">Create user accounts</span></span>  

<span data-ttu-id="0b209-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="0b209-105">**Appropriate roles**</span></span>

- <span data-ttu-id="0b209-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="0b209-106">Account admin</span></span>
- <span data-ttu-id="0b209-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="0b209-107">Global admin</span></span>
- <span data-ttu-id="0b209-108">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="0b209-108">User management admin</span></span>

<span data-ttu-id="0b209-109">파트너 센터에 액세스해야 하는 직원의 사용자 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="0b209-110">이러한 작업은 사용자 관리, 계정 관리 또는 글로벌 관리 권한이 있는 관리자가 수행해야 합니다. 이러한 작업을 수행하는 사용자에게는 사용자 관리자 또는 글로벌 관리자의 AAD(Azure Active Directory) 역할도 할당되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="0b209-111">AAD 역할에 대한 자세한 내용은 [Azure Active Directory의 관리자 역할 권한](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0b209-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="0b209-112">새 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="0b209-112">Add a new user</span></span>

1. <span data-ttu-id="0b209-113">파트너 센터 오른쪽 위의 **설정** 아이콘에서 **계정 설정** 을 선택한 다음, **사용자 관리** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="0b209-114">**사용자 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-114">Select **Add user**.</span></span>

3. <span data-ttu-id="0b209-115">사용자의 전체 이름과 고유의 이메일 주소를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="0b209-116">에이전트 유형 및/또는 사용자에게 할당할 관리자 유형을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="0b209-117">파트너 센터 액세스는 역할 기반이므로 사용자가 특정 작업을 완료하는 데 필요한 기능만 표시하도록 사용자의 보기를 사용자 지정하는 권한을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="0b209-118">역할 할당을 원하는 사용자는 **사용자 관리** 로 이동하여 글로벌 관리자에 대한 필터링을 수행하여 연락할 글로벌 관리자를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="0b209-119">**추가** 를 선택하여 사용자 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="0b209-120">다음 페이지에서 사용자의 세부 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="0b209-121">이 페이지에 표시되는 새 사용자의 로그인 정보를 기록해 두세요.</span><span class="sxs-lookup"><span data-stu-id="0b209-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="0b209-122">나중에 이 정보에 다시 액세스할 수 없으므로 이 정보를 복사하여 새 사용자에게 보내야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="0b209-123">사용자는 사용자 이름 및 임시 암호를 사용하여 파트너 센터에 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="0b209-124">사용자가 파트너 센터에 처음으로 로그인하면 암호를 변경하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="0b209-125">사용자 역할 할당</span><span class="sxs-lookup"><span data-stu-id="0b209-125">Assign user roles</span></span>

<span data-ttu-id="0b209-126">파트너 센터에서 작업하려면 할당된 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="0b209-127">현재 역할에는 Azure Active Directory 테넌트 역할, CSP(클라우드 솔루션 공급자) 역할 및 비 AAD 회사 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="0b209-128">개별 회사에 이러한 모든 역할이 필요할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="0b209-129">파트너 센터에 액세스하려면 개별 회사가 테넌트에 나열되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="0b209-130">역할 할당은 추가 액세스 권한을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="0b209-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0b209-131">다음 단계</span><span class="sxs-lookup"><span data-stu-id="0b209-131">Next steps</span></span>

- [<span data-ttu-id="0b209-132">파트너 센터에서 작업해야 하는 직원에 대한 사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="0b209-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
