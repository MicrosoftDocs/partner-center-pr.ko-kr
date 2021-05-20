---
title: 테넌트 ID, 도메인 이름, 사용자 개체 ID 찾기
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 조직의 Azure AD 테넌트 ID, 도메인 이름 또는 특정 사용자 개체 ID인 Azure Portal ID를 찾는 방법을 알아봅니다. 일부 작업에는 이 정보가 필요합니다.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150865"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="ab974-104">사용자의 중요한 ID 찾기</span><span class="sxs-lookup"><span data-stu-id="ab974-104">Locate important IDs for a user</span></span>

<span data-ttu-id="ab974-105">**적절한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="ab974-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="ab974-106">이 문서에서는 [Azure Portal](https://portal.azure.com/) 사용하여 사용자에 대한 다음 정보를 찾는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="ab974-107">사용자 조직 또는 회사의 Microsoft Azure Active Directory(Azure AD) 테넌트 ID</span><span class="sxs-lookup"><span data-stu-id="ab974-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="ab974-108">Azure AD 테넌트와 연결된 조직 또는 회사의 주 도메인 이름</span><span class="sxs-lookup"><span data-stu-id="ab974-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="ab974-109">사용자 개체 ID</span><span class="sxs-lookup"><span data-stu-id="ab974-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="ab974-110">Microsoft Azure AD 테넌트 ID 및 주 도메인 이름 찾기</span><span class="sxs-lookup"><span data-stu-id="ab974-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="ab974-111">다음 단계에 따라 Azure Portal 내에서 Azure AD 테넌트 ID 또는 주 도메인 이름을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="ab974-112">(프로그래밍 방식으로 테넌트 ID를 찾으려면 [PowerShell 또는 CLI를 사용하여 테넌트 ID 찾기를](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="ab974-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="ab974-113">테넌트 ID는 서로 다른 애플리케이션 또는 리소스에서 다른 이름을 호출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="ab974-114">예를 들어 테넌트 ID를 디렉터리 ID, azure AD(Azure Active Directory) 테넌트, Microsoft ID 또는 특정 보고서의 경우 *tenantguid라고* 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="ab974-115">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="ab974-116">메뉴에서 **Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="메뉴에서 Azure Active Directory 옵션을 선택하는 Azure Portal 표시합니다.":::

3. <span data-ttu-id="ab974-118">Azure Active Directory **개요** 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="ab974-119">Azure AD 테넌트 ID 또는 주 도메인 이름을 찾으려면 **테넌트 ID** 필드와 **주 도메인** 필드를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="ab974-120">이러한 필드는 테넌트 정보 섹션에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="두 개의 강조 표시된 필드( 테넌트 ID 및 주 도메인 이름)가 있는 개요 페이지를 표시합니다.":::

4. <span data-ttu-id="ab974-122">몇 가지 다른 방법으로 Azure Portal 테넌트 ID를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="ab974-123">메뉴에서 **Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="ab974-124">그런 다음, 메뉴에서 **관리** 섹션을 찾아 **속성을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="ab974-125">속성 페이지에는 사용자의 연결 된 테 넌 트 ID도 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="강조 표시 된 테 넌 트 ID 필드가 있는 속성 페이지를 표시 합니다.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="ab974-127">사용자 개체 ID 찾기</span><span class="sxs-lookup"><span data-stu-id="ab974-127">Find the user object ID</span></span>

<span data-ttu-id="ab974-128">도메인 이름 및 테 넌 트 ID를 찾는 것 만으로는 항상 충분 하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="ab974-129">사용자에 게 할당 된 특정 개체 ID를 찾아야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="ab974-130">Azure Portal에서 사용자의 개체 ID를 찾으려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="ab974-131">[Azure Portal](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="ab974-132">메뉴에서 **Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="ab974-133">메뉴에서 **관리** 섹션을 찾은 다음 **사용자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="강조 표시 된 사용자 옵션을 사용 하 여 Azure Active Directory 메뉴를 표시 합니다.":::

4. <span data-ttu-id="ab974-135">사용자 페이지의 검색 상자에 사용자 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="특정 사용자를 검색 하는 검색 상자가 있는 사용자 페이지를 표시 합니다.":::

5. <span data-ttu-id="ab974-137">목록에 표시 되는 사용자 이름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="검색 된 사용자에 대 한 행을 표시 하는 사용자 페이지를 표시 합니다.":::

6. <span data-ttu-id="ab974-139">사용자의 프로필 페이지에서 Id 섹션을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="ab974-140">개체 ID 필드는 사용자의 고유 개체 ID와 함께 여기에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ab974-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id 섹션이 있는 사용자 프로필 페이지 및 개체 ID에 대해 하나의 강조 표시 된 필드를 표시 합니다.":::

## <a name="next-steps"></a><span data-ttu-id="ab974-142">다음 단계</span><span class="sxs-lookup"><span data-stu-id="ab974-142">Next steps</span></span>

- [<span data-ttu-id="ab974-143">PowerShell 또는 CLI를 사용 하 여 프로그래밍 방식으로 테 넌 트 ID 찾기</span><span class="sxs-lookup"><span data-stu-id="ab974-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="ab974-144">Azure Active Directory의 사용자 프로필에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="ab974-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="ab974-145">파트너가 파트너 센터에서 고객 세부 정보를 보거나 내보내는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="ab974-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

