---
title: 고객 계정에 대한 사용자 관리 작업 | 파트너 센터
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객에 대 한 사용자 계정을 만들고, 사용자 라이선스를 추가 또는 제거 하 고, 사용자 암호를 다시 설정 하거나, 사용자 계정을 삭제 하거나, 복원 하는 방법에 대해 알아봅니다.
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: MaggiePucciEvans
ms.author: evansma
Keywords: 고객 관리, 계정, 계정 만들기, 라이선스, 라이선스 할당, 사용자 관리, 암호, 암호 재설정, 암호 변경
ms.localizationpriority: medium
ms.openlocfilehash: fb2e616a6bf7dbfa5072ff1617dc37ad76831b8c
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253348"
---
# <a name="user-management-tasks-for-customer-accounts"></a><span data-ttu-id="204ee-104">고객 계정에 대한 사용자 관리 작업</span><span class="sxs-lookup"><span data-stu-id="204ee-104">User management tasks for customer accounts</span></span>

<span data-ttu-id="204ee-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="204ee-105">**Applies to**</span></span>

- <span data-ttu-id="204ee-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="204ee-106">Partner Center</span></span>

<span data-ttu-id="204ee-107">고객의 계정에서 새 사용자를 만들고 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-107">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="204ee-108">삭제 후 30 일 이내에 이전에 삭제 한 사용자 계정을 하나 이상 복원할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-108">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="204ee-109">사용자의 이전 구독 할당도 복원됩니다(이전 할당을 사용할 수 있다고 가정).</span><span class="sxs-lookup"><span data-stu-id="204ee-109">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="204ee-110">고객에 대 한 새 구독을 구입 하는 경우 고객은 계정, 해당 사용자 권한 및 각 사용자가 요구 하는 서비스를 필요로 하는 모든 사용자의 목록을 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-110">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="204ee-111">[Excel 호환 .csv 스프레드시트 파일](bulk-license-provisioning-for-multiple-users.md)을 사용하여 한 번에 [여러 사용자에게 구독을 할당](adding-multiple-users-to-a-customer-account.md)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-111">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="204ee-112">고객용 사용자 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="204ee-112">Create user accounts for a customer</span></span>

1. <span data-ttu-id="204ee-113">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-113">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="204ee-114">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-114">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="204ee-115">고객 메뉴에서 **사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-115">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="204ee-116">각 사용자에 대해 **사용자 추가**를 선택한 다음 권한과 라이선스 등의 정보를 작성합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-116">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="204ee-117">변경 사항을 **저장**합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-117">**Save** your changes.</span></span>

5. <span data-ttu-id="204ee-118">사용자 이름 및 사용자에게 보낼 임시 암호를 기록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-118">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="204ee-119">한 번에 하나씩 여러 사용자를 추가하는 경우 **다른 사용자 추가**를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-119">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="204ee-120">[Excel 호환 .csv 스프레드시트 파일을 가져와서](adding-multiple-users-to-a-customer-account.md) 한 번에 여러 사용자를 추가할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-120">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="204ee-121">다른 사용자 추가를 사용하거나 Excel과 호환되는 .csv 스프레드시트 파일로 가져와 한 번에 다수의 사용자를 추가하는 경우 전체 집합을 완료할 때까지 기다려야 확인 화면에서 이러한 이름과 암호를 메일로 보내거나 인쇄할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-121">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="204ee-122">고객용 사용자 라이선스 추가 또는 제거</span><span class="sxs-lookup"><span data-stu-id="204ee-122">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="204ee-123">다음 단계는 Microsoft 제품에 대 한 사용자 라이선스를 추가 하거나 제거 하는 경우에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-123">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="204ee-124">상업적 marketplace에서 라이선스 기반 SaaS 구독의 사용자 라이선스를 추가 하거나 제거 하려면 [SaaS 구독에 대 한 라이선스 추가 또는 제거](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="204ee-124">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="204ee-125">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-125">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="204ee-126">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-126">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="204ee-127">고객 메뉴에서 **사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-127">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="204ee-128">목록에서 한 명 이상의 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-128">Choose one or more users from the list.</span></span> <span data-ttu-id="204ee-129">예를 들어 고객이 새 라이선스를 방금 구매한 후 아직 라이선스가 없는 사람에게 할당하려고 하는 경우 **사용자 필터링 기준...** 옵션을 사용하여 알맞은 그룹을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-129">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="204ee-130">**라이선스 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-130">Select **Manage licenses**.</span></span> <span data-ttu-id="204ee-131">필요한 사항을 변경한 다음 **저장**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-131">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="204ee-132">제품을 게시 한 ISV (독립 소프트웨어 공급 업체)를 통해 라이선스 할당 및 활성화를 관리 하는 [Azure Marketplace 제품](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)입니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-132">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="204ee-133">고객용 사용자 암호 재설정</span><span class="sxs-lookup"><span data-stu-id="204ee-133">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="204ee-134">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-134">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="204ee-135">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-135">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="204ee-136">고객 메뉴에서 **사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-136">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="204ee-137">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-137">Choose the user from the list.</span></span>

4.  <span data-ttu-id="204ee-138">화면 맨 아래에서 **암호 재설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-138">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="204ee-139">사용자에게 새 임시 암호를 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-139">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="204ee-140">고객용 사용자 계정 삭제</span><span class="sxs-lookup"><span data-stu-id="204ee-140">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="204ee-141">**파트너 센터** 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-141">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="204ee-142">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-142">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="204ee-143">고객 메뉴에서 **사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-143">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="204ee-144">목록에서 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-144">Choose the user from the list.</span></span>

3.  <span data-ttu-id="204ee-145">화면 맨 아래에서 **사용자 계정 삭제**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-145">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="204ee-146">이 계정을 30일 이내에 복원해야 할 경우 고객 **사용자 및 라이선스** 목록의 **삭제된 사용자** 탭에서 이 계정을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-146">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="204ee-147">삭제된 사용자는 30일 이내에 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-147">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="204ee-148">삭제된 사용자 계정 복원</span><span class="sxs-lookup"><span data-stu-id="204ee-148">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="204ee-149">**파트너 센터** 메뉴에서 **고객**을 선택한 다음 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-149">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="204ee-150">**사용자 및 라이선스**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-150">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="204ee-151">**삭제된 사용자( )** 탭을 선택합니다. 복원할 수 있는 삭제된 사용자가 있는 경우 **(1)** 이상이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-151">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="204ee-152">하나 이상의 삭제된 사용자의 확인란을 선택한 다음 **복원**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-152">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="204ee-153">선택한 모든 사용자 계정이 **사용자 및 라이선스** 페이지에 다시 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="204ee-153">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="204ee-154">관련 항목</span><span class="sxs-lookup"><span data-stu-id="204ee-154">Related topics</span></span>


[<span data-ttu-id="204ee-155">여러 사용자에게 라이선스 할당 또는 해지</span><span class="sxs-lookup"><span data-stu-id="204ee-155">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="204ee-156">고객 계정에 대 한 여러 사용자 만들기</span><span class="sxs-lookup"><span data-stu-id="204ee-156">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)