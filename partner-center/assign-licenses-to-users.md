---
title: 고객 계정에 대한 사용자 관리
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 고객에 대한 사용자 관리 - 사용자 계정을 만들고, 사용자 라이선스를 추가 또는 제거하고, 암호를 재설정하고, 사용자 계정을 삭제하거나 복원합니다.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149896"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="8350a-103">고객 계정에 대한 사용자 및 사용자 라이선스 관리</span><span class="sxs-lookup"><span data-stu-id="8350a-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="8350a-104">**적절한 역할:** 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="8350a-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="8350a-105">고객의 계정에서 새 사용자를 만들고 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="8350a-106">삭제 후 30일 이내에 이전에 삭제한 사용자 계정을 하나 이상 복원할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="8350a-107">사용자의 이전 구독 할당도 복원됩니다(이전 할당을 사용할 수 있다고 가정).</span><span class="sxs-lookup"><span data-stu-id="8350a-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="8350a-108">고객에 대한 새 구독을 구입하는 경우 고객은 계정이 필요한 모든 사용자 목록, 사용자 권한 및 각 사용자에게 필요한 서비스를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="8350a-109">**고객** 탭의 **사용자 및 라이선스** 섹션에는 다른 CSP 파트너 또는 다른 구매 채널에서 구매한 라이선스가 있는 사용자를 포함하여 특정 고객의 테넌트에서 만든 모든 사용자가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="8350a-110">[Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)를 사용하여 이름을 가져와서 한 번에 여러 사용자에게 [구독을 할당할](bulk-license-provisioning-for-multiple-users.md) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="8350a-111">고객의 사용자 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="8350a-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="8350a-112">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8350a-113">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8350a-114">고객 메뉴에서 사용자 **및 라이선스를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="8350a-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="8350a-115">추가하는 각 사용자에 대해 **구독 추가를** 선택한 다음, 사용 권한 및 라이선스를 포함한 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="8350a-116">변경 내용을 **저장** 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-116">**Save** your changes.</span></span>

5. <span data-ttu-id="8350a-117">사용자에게 보낼 사용자 이름과 임시 암호를 기록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="8350a-118">여러 사용자를 한 번에 하나씩 추가하는 경우 **다른 사용자 추가** 를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="8350a-119">[Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)를 가져와서 한 번에 여러 사용자를 추가할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="8350a-120">확인 화면에서 이름과 암호를 전자 메일로 보내거나 인쇄하기 전에 전체 집합을 완료할 때까지 기다릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="8350a-121">고객에 대한 사용자 라이선스 추가 또는 제거</span><span class="sxs-lookup"><span data-stu-id="8350a-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="8350a-122">다음 단계는 Microsoft 제품에 대한 사용자 라이선스를 추가하거나 제거하는 데 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="8350a-123">상업용 Marketplace에서 라이선스 기반 SaaS 구독에 대한 사용자 라이선스를 추가하거나 제거하려면 [SaaS 구독에 대한 라이선스 추가 또는 제거를](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8350a-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="8350a-124">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8350a-125">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8350a-126">고객 메뉴에서 **사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="8350a-127">목록에서 한 명 이상의 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-127">Choose one or more users from the list.</span></span> <span data-ttu-id="8350a-128">예를 들어 고객이 새 라이선스를 구매 했 고 아직 없는 사용자에 게 해당 라이선스를 할당 하려는 경우 **사용자 필터** ... 옵션을 사용 하 여 올바른 그룹을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="8350a-129">**라이선스 관리** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-129">Select **Manage licenses**.</span></span> <span data-ttu-id="8350a-130">변경한 후 **저장** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="8350a-131">제품을 게시 한 ISV (독립 소프트웨어 공급 업체)를 통해 라이선스 할당 및 활성화를 관리 하는 [Azure Marketplace 제품](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)입니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="8350a-132">고객에 대 한 사용자 암호 재설정</span><span class="sxs-lookup"><span data-stu-id="8350a-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="8350a-133">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8350a-134">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8350a-135">고객 메뉴에서 **사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="8350a-136">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="8350a-137">화면 아래쪽에서 **암호 재설정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="8350a-138">새 임시 암호를 사용자에 게 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="8350a-139">고객에 대 한 사용자 계정 삭제</span><span class="sxs-lookup"><span data-stu-id="8350a-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="8350a-140">**파트너 센터** 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="8350a-141">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="8350a-142">고객 메뉴에서 **사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="8350a-143">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="8350a-144">화면 맨 아래에서 **사용자 계정 삭제** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="8350a-145">이 계정을 복원 해야 하는 경우 고객의 **사용자 및 라이선스** 목록의 **삭제 된 사용자** 탭에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="8350a-146">삭제 된 사용자를 복원 하는 데 30 일이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="8350a-147">삭제 된 사용자 계정 복원</span><span class="sxs-lookup"><span data-stu-id="8350a-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="8350a-148">**파트너 센터** 메뉴에서 **고객** 을 선택한 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="8350a-149">**사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="8350a-150">삭제 된 **사용자 ()** 탭을 선택 합니다. 복원할 수 있는 삭제 된 사용자가 있는 경우에는 **(1)** 이상을 읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="8350a-151">삭제 된 사용자의 확인란을 하나 이상 선택 하 고 **복원** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="8350a-152">선택한 모든 사용자 계정이 **사용자 및 라이선스** 페이지에 다시 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="8350a-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8350a-153">다음 단계</span><span class="sxs-lookup"><span data-stu-id="8350a-153">Next steps</span></span>

- [<span data-ttu-id="8350a-154">여러 사용자에게 라이선스 할당 또는 해지</span><span class="sxs-lookup"><span data-stu-id="8350a-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="8350a-155">고객 계정에 대 한 여러 사용자 만들기</span><span class="sxs-lookup"><span data-stu-id="8350a-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)