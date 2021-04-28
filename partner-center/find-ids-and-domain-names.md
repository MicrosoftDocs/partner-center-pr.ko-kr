---
title: 테 넌 트 ID, 도메인 이름, 사용자 개체 ID 찾기
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Portal에서 Id를 찾는 방법에 대해 알아봅니다. 조직의 Azure AD 테 넌 트 ID, 도메인 이름 또는 특정 사용자 개체 ID입니다. 일부 작업에는이 정보가 필요 합니다.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172254"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="c9194-104">사용자에 대 한 중요 한 Id 찾기</span><span class="sxs-lookup"><span data-stu-id="c9194-104">Locate important IDs for a user</span></span>

<span data-ttu-id="c9194-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="c9194-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c9194-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="c9194-106">Global admin</span></span>

<span data-ttu-id="c9194-107">이 문서에서는 [Azure Portal](https://portal.azure.com/) 를 사용 하 여 사용자에 대 한 다음 정보를 찾는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="c9194-108">사용자의 조직 또는 회사의 Microsoft Azure Active Directory (Azure AD) 테 넌 트 ID</span><span class="sxs-lookup"><span data-stu-id="c9194-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="c9194-109">Azure AD 테 넌 트와 연결 된 조직 또는 회사의 주 도메인 이름</span><span class="sxs-lookup"><span data-stu-id="c9194-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="c9194-110">사용자 개체 ID</span><span class="sxs-lookup"><span data-stu-id="c9194-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="c9194-111">Microsoft Azure AD 테 넌 트 ID 및 주 도메인 이름 찾기</span><span class="sxs-lookup"><span data-stu-id="c9194-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="c9194-112">Azure Portal 내에서 Azure AD 테 넌 트 ID 또는 주 도메인 이름을 찾으려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="c9194-113">(테 넌 트 ID를 프로그래밍 방식으로 찾으려면 [PowerShell 또는 CLI를 사용 하 여 테 넌 트 Id 찾기](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)를 참조 하세요.)</span><span class="sxs-lookup"><span data-stu-id="c9194-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="c9194-114">테 넌 트 ID는 다른 응용 프로그램 또는 리소스에서 다른 이름으로 호출 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="c9194-115">예를 들어 테 넌 트 ID를 디렉터리 ID, Azure Active Directory (Azure AD) 테 넌 트, Microsoft ID 또는 *tenantguid* 를 비롯 한 특정 보고서에 대해 참조할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="c9194-116">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="c9194-117">메뉴에서 **Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="메뉴에서 Azure Active Directory 옵션을 선택 하 Azure Portal 표시 합니다.":::

3. <span data-ttu-id="c9194-119">Azure Active Directory **개요** 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="c9194-120">Azure AD 테 넌 트 ID 또는 주 도메인 이름을 찾으려면 **테 넌 트 id** 필드 및 **주 도메인** 필드를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="c9194-121">이러한 필드는 테 넌 트 정보 섹션에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="두 개의 강조 표시 된 필드, 테 넌 트 ID 및 주 도메인 이름이 있는 개요 페이지를 표시 합니다.":::

4. <span data-ttu-id="c9194-123">Azure Portal에서 테 넌 트 ID는 몇 가지 다른 방법으로 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="c9194-124">메뉴에서 **Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="c9194-125">그런 다음 메뉴에서 **관리** 섹션을 찾아 **속성** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="c9194-126">속성 페이지에는 사용자의 연결 된 테 넌 트 ID도 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="강조 표시 된 테 넌 트 ID 필드가 있는 속성 페이지를 표시 합니다.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="c9194-128">사용자 개체 ID 찾기</span><span class="sxs-lookup"><span data-stu-id="c9194-128">Find the user object ID</span></span>

<span data-ttu-id="c9194-129">도메인 이름 및 테 넌 트 ID를 찾는 것 만으로는 항상 충분 하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="c9194-130">사용자에 게 할당 된 특정 개체 ID를 찾아야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="c9194-131">Azure Portal에서 사용자의 개체 ID를 찾으려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="c9194-132">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="c9194-133">메뉴에서 **Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="c9194-134">메뉴에서 **관리** 섹션을 찾은 다음 **사용자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="강조 표시 된 사용자 옵션을 사용 하 여 Azure Active Directory 메뉴를 표시 합니다.":::

4. <span data-ttu-id="c9194-136">사용자 페이지의 검색 상자에 사용자 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="특정 사용자를 검색 하는 검색 상자가 있는 사용자 페이지를 표시 합니다.":::

5. <span data-ttu-id="c9194-138">목록에 표시 되는 사용자 이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="검색 된 사용자에 대 한 행을 표시 하는 사용자 페이지를 표시 합니다.":::

6. <span data-ttu-id="c9194-140">사용자의 프로필 페이지에서 Id 섹션을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="c9194-141">개체 ID 필드는 사용자의 고유 개체 ID와 함께 여기에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c9194-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id 섹션이 있는 사용자 프로필 페이지 및 개체 ID에 대해 하나의 강조 표시 된 필드를 표시 합니다.":::

## <a name="next-steps"></a><span data-ttu-id="c9194-143">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c9194-143">Next steps</span></span>

- [<span data-ttu-id="c9194-144">PowerShell 또는 CLI를 사용 하 여 프로그래밍 방식으로 테 넌 트 ID 찾기</span><span class="sxs-lookup"><span data-stu-id="c9194-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="c9194-145">Azure Active Directory의 사용자 프로필에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="c9194-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="c9194-146">파트너가 파트너 센터에서 고객 세부 정보를 보거나 내보내는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="c9194-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

