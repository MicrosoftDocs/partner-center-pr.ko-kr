---
title: 고객 계정에 대 한 사용자 및 사용자 라이선스 관리
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 사용자 계정을 만들고, 사용자 라이선스를 추가 또는 제거 하 고, 사용자 암호를 다시 설정 하 고, 사용자 계정을 삭제 하거나 복원 하는 등 파트너 센터에서 고객의 사용자를 관리 하는 방법에 대해 알아봅니다.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474073"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="00d97-103">고객 계정에 대 한 사용자 및 사용자 라이선스 관리</span><span class="sxs-lookup"><span data-stu-id="00d97-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="00d97-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="00d97-104">**Appropriate roles**</span></span>

- <span data-ttu-id="00d97-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="00d97-105">Global admin</span></span>
- <span data-ttu-id="00d97-106">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="00d97-106">User management admin</span></span>
- <span data-ttu-id="00d97-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="00d97-107">Admin agent</span></span>


<span data-ttu-id="00d97-108">고객의 계정에서 새 사용자를 만들고 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="00d97-109">삭제 후 30 일 이내에 이전에 삭제 한 사용자 계정을 하나 이상 복원할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="00d97-110">사용자의 이전 구독 할당도 복원 됩니다 (이전 할당을 사용할 수 있는 것으로 가정).</span><span class="sxs-lookup"><span data-stu-id="00d97-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="00d97-111">고객에 대 한 새 구독을 구입 하는 경우 고객은 계정, 해당 사용자 권한 및 각 사용자가 요구 하는 서비스를 필요로 하는 모든 사용자의 목록을 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="00d97-112">[Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)을 사용 하 여 [여러 사용자에 게 한 번에 여러 사용자에 게 구독을 할당할](bulk-license-provisioning-for-multiple-users.md) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-112">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="00d97-113">고객의 사용자 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="00d97-113">Create user accounts for a customer</span></span>

1. <span data-ttu-id="00d97-114">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-114">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="00d97-115">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="00d97-116">고객 메뉴에서 **사용자 및 라이선스** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-116">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="00d97-117">추가 하는 각 사용자에 대해 **구독 추가** 를 선택 하 고 사용 권한 및 라이선스를 포함 한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-117">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="00d97-118">변경 내용을 **저장** 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-118">**Save** your changes.</span></span>

5. <span data-ttu-id="00d97-119">사용자에 게 보낼 사용자 이름 및 임시 암호를 기록해 두어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-119">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="00d97-120">한 번에 여러 사용자를 추가 하는 경우 **다른 사용자 추가** 를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-120">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="00d97-121">[Excel 호환 .csv 스프레드시트 파일을 가져오면](adding-multiple-users-to-a-customer-account.md)여러 사용자를 한 번에 추가할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-121">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="00d97-122">전자 메일을 보내거나 확인 화면에서 이름 및 암호를 인쇄 하기 전에 전체 설정이 완료 될 때까지 기다릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-122">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="00d97-123">고객에 대 한 사용자 라이선스 추가 또는 제거</span><span class="sxs-lookup"><span data-stu-id="00d97-123">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="00d97-124">다음 단계는 Microsoft 제품에 대 한 사용자 라이선스를 추가 하거나 제거 하는 경우에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-124">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="00d97-125">상업적 marketplace에서 라이선스 기반 SaaS 구독의 사용자 라이선스를 추가 하거나 제거 하려면 [SaaS 구독에 대 한 라이선스 추가 또는 제거](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00d97-125">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="00d97-126">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-126">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="00d97-127">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-127">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="00d97-128">고객 메뉴에서 **사용자 및 라이선스** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-128">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="00d97-129">목록에서 하나 이상의 사용자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-129">Choose one or more users from the list.</span></span> <span data-ttu-id="00d97-130">예를 들어 고객이 새 라이선스를 구매 했 고 아직 없는 사용자에 게 해당 라이선스를 할당 하려는 경우 **사용자 필터** ... 옵션을 사용 하 여 올바른 그룹을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-130">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="00d97-131">**라이선스 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-131">Select **Manage licenses**.</span></span> <span data-ttu-id="00d97-132">변경한 후 **저장** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-132">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="00d97-133">제품을 게시 한 ISV (독립 소프트웨어 공급 업체)를 통해 라이선스 할당 및 활성화를 관리 하는 [Azure Marketplace 제품](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)입니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-133">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="00d97-134">고객에 대 한 사용자 암호 재설정</span><span class="sxs-lookup"><span data-stu-id="00d97-134">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="00d97-135">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-135">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="00d97-136">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-136">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="00d97-137">고객 메뉴에서 **사용자 및 라이선스** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-137">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="00d97-138">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-138">Choose the user from the list.</span></span>

4.  <span data-ttu-id="00d97-139">화면 아래쪽에서 **암호 재설정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-139">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="00d97-140">새 임시 암호를 사용자에 게 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-140">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="00d97-141">고객에 대 한 사용자 계정 삭제</span><span class="sxs-lookup"><span data-stu-id="00d97-141">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="00d97-142">**파트너 센터** 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-142">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="00d97-143">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-143">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="00d97-144">고객 메뉴에서 **사용자 및 라이선스** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-144">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="00d97-145">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-145">Choose the user from the list.</span></span>

3.  <span data-ttu-id="00d97-146">화면 맨 아래에서 **사용자 계정 삭제** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-146">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="00d97-147">이 계정을 복원 해야 하는 경우 고객의 **사용자 및 라이선스** 목록의 **삭제 된 사용자** 탭에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-147">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="00d97-148">삭제 된 사용자를 복원 하는 데 30 일이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-148">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="00d97-149">삭제 된 사용자 계정 복원</span><span class="sxs-lookup"><span data-stu-id="00d97-149">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="00d97-150">**파트너 센터** 메뉴에서 **고객** 을 선택한 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-150">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="00d97-151">**사용자 및 라이선스** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-151">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="00d97-152">삭제 된 **사용자 ()** 탭을 선택 합니다. 복원할 수 있는 삭제 된 사용자가 있는 경우에는 **(1)** 이상을 읽어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-152">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="00d97-153">삭제 된 사용자의 확인란을 하나 이상 선택 하 고 **복원** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-153">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="00d97-154">선택한 모든 사용자 계정이 **사용자 및 라이선스** 페이지에 다시 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="00d97-154">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="00d97-155">관련 항목</span><span class="sxs-lookup"><span data-stu-id="00d97-155">Related topics</span></span>


[<span data-ttu-id="00d97-156">여러 사용자에게 라이선스 할당 또는 해지</span><span class="sxs-lookup"><span data-stu-id="00d97-156">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="00d97-157">고객 계정에 대 한 여러 사용자 만들기</span><span class="sxs-lookup"><span data-stu-id="00d97-157">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)