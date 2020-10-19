---
title: 파트너 센터에서 지급 및 세금 프로필
ms.topic: how-to
ms.date: 09/11/2020
description: 지급 및 세금 프로필을 만들고 관리 하 여 성과급 작업에 대해 지불할 수 있습니다. 다른 프로필을 만들고, 관리 하 고, 사용 하는 등의 작업이 포함 됩니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ca2ffe992ff92b98546934f4a249779f39179acb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175351"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="bbd17-104">파트너 센터에서 성과급 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="bbd17-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="bbd17-105">**적용 대상:**</span><span class="sxs-lookup"><span data-stu-id="bbd17-105">**Applies to:**</span></span>

- <span data-ttu-id="bbd17-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="bbd17-106">Partner Center</span></span>

<span data-ttu-id="bbd17-107">**적절한 역할:**</span><span class="sxs-lookup"><span data-stu-id="bbd17-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="bbd17-108">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="bbd17-108">Incentives admin</span></span>
- <span data-ttu-id="bbd17-109">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="bbd17-109">Billing admin</span></span>
- <span data-ttu-id="bbd17-110">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="bbd17-110">Global admin</span></span>

<span data-ttu-id="bbd17-111">특정 MPN 위치에 대한 인센티브 프로그램의 지급금을 받으려면 유효한 지급 및 세금 프로필을 프로그램 및 MPN 위치와 연결하여 등록을 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="bbd17-112">Microsoft는이 지급 및 세금 프로필을 사용하여 지급금을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="bbd17-113">인센티브 프로그램의 규칙에 따라 전자 계좌 이체 또는 결제 신용 전표를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="bbd17-114">역할, 통화 및 기타 Microsoft 프로그램</span><span class="sxs-lookup"><span data-stu-id="bbd17-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="bbd17-115">지급 및 세금 프로필을 시작 하기 전에 아래 정보를 이해 하는 것이 중요 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="bbd17-116">역할 및 권한</span><span class="sxs-lookup"><span data-stu-id="bbd17-116">Roles and permissions</span></span>

<span data-ttu-id="bbd17-117">동기 지불액에 대 한 은행 및 세금 정보를 입력 하려면 성과급 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="bbd17-118">MPN/계정 관리자 인 경우 자신 및/또는 동료를 성과급 관리자로 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="bbd17-119">성과급 관리자 권한을 요청 해야 하는 경우 MPN 관리자 또는 전역 관리자에 게 문의 하세요. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인 하 여 회사에서 이러한 역할을 가진 사람을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="bbd17-120">오른쪽 위의 **설정** 아이콘에서 **사용자 관리** 를 선택 하 고 전역 관리자에서 필터링 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="bbd17-121">성과급 사용자는 동기 수입 및 지불 정보 및 보고서를 볼 수 있지만, 은행 및 세금 정보는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="bbd17-122">자금 지출 통화를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-122">Choose your disbursement currency</span></span>

<span data-ttu-id="bbd17-123">기본적으로 각 엔터티의 현지 통화로는 성과급 불입금이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-123">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="bbd17-124">프로필을 설치 하는 동안 다른 통화를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-124">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="bbd17-125">지불은 Microsoft에서 매월 설정한 환율을 사용 하 여 계산 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-125">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="bbd17-126">선택한 통화로 인 한 값의 변경에 대 한 책임이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-126">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="bbd17-127">은행 및 세금 정보 및 기타 프로그램</span><span class="sxs-lookup"><span data-stu-id="bbd17-127">Bank and tax information and other programs</span></span>

<span data-ttu-id="bbd17-128">Microsoft에서 지불에 이미 은행 데이터를 사용 하는 경우에도 아래에 설명 된 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-128">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="bbd17-129">이렇게 하면 프로필을 새 도구로 복사 하면 중요 한 정보가 노출 될 수 있으므로 회사 데이터의 개인 정보 보호 및 보안을 유지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-129">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="bbd17-130">이 프로세스를 진행 하는 것도 데이터가 완전 하 고 정확한 지 확인 하는 좋은 기회입니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-130">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="bbd17-131">Microsoft 프로그램 마다 다른 프로필 사용</span><span class="sxs-lookup"><span data-stu-id="bbd17-131">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="bbd17-132">소매 내에서 5 가지 소매 동기 프로그램 각각에 대 한 결제는 동일한 은행 계좌로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-132">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="bbd17-133">또는 소매 사무실이 다른 은행 계정에 지불 되는 동안 소매 Xbox 지불을 하나의 은행 계좌로 이동 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-133">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="bbd17-134">파트너 센터에서 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="bbd17-134">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="bbd17-135">아래 섹션에서는 파트너 센터에서 결제 및 세금 프로필을 만들고 관리 하는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-135">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="bbd17-136">파트너 센터에서 지불 프로필을 만들거나 관리 하려면 동기 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-136">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="bbd17-137">각 동기 프로그램의 각 MPN 위치에는 동기 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-137">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="bbd17-138">파트너 센터에서 동기 관리자를 추가 하는 방법에 대 한 자세한 내용은 [사용자 계정 만들기](create-user-accounts-and-set-permissions.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="bbd17-138">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="bbd17-139">파트너 센터의 지급 및 세금 섹션 액세스</span><span class="sxs-lookup"><span data-stu-id="bbd17-139">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="bbd17-140">Azure Active Directory (Azure AD) 계정 (회사 계정)을 사용 하 여 [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/) 로그인 하거나, 할당 된 경우 적절 한 전자 메일 주소를 사용 하 여 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="bbd17-141">하나의 Azure AD 계정 내에 여러 도메인을 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-141">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="bbd17-142">전역 관리자에 게 문의 하 여 연결 된 도메인을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-142">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="bbd17-143">도메인을 사용 하 여 로그인 할 수 있는 경우 @onmicrosoft.com 계정 관리자에 게 문의 하 여 AZURE AD 계정에 도메인을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-143">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="bbd17-144">**회사 또는 학교** 계정 또는 **개인 계정을**선택 하 라는 메시지가 표시 되 면 **회사 또는 학교 계정**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-144">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="bbd17-145">기어 아이콘을 선택 하 여 **설정** 메뉴를 열고 **파트너 설정**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-145">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="bbd17-146">**계정 설정** 메뉴에서 **지급 및 세금**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-146">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="bbd17-147">개별 프로그램에 지급 및 세금 프로필 할당</span><span class="sxs-lookup"><span data-stu-id="bbd17-147">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="bbd17-148">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 하 고 기어 아이콘을 선택 하 여 **설정** 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="bbd17-149">**파트너 설정**을 선택 하 고 **지급 및 세금 섹션**을 확장 한 다음 **지급 및 세금 프로필 할당**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-149">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="bbd17-150">프로그램 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-150">A list of your programs will be displayed.</span></span> <span data-ttu-id="bbd17-151">프로그램 옆의 화살표를 선택 하 여 프로필 세부 정보를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-151">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="bbd17-152">**세금 프로필** 드롭다운 메뉴에서 원하는 세금 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-152">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="bbd17-153">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-153">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="bbd17-154">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-154">Select Continue in the pop-up window.</span></span> <span data-ttu-id="bbd17-155">새 세금 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-155">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="bbd17-156">**지불 방법**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-156">Select **Payment method**.</span></span>

   - <span data-ttu-id="bbd17-157">지불 방법으로 **전자 은행 전송** 을 선택한 경우 원하는 지불 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-157">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="bbd17-158">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-158">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="bbd17-159">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-159">Select Continue in the pop-up window.</span></span> <span data-ttu-id="bbd17-160">새 지불 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-160">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="bbd17-161">**신용 정보** 를 지불 방법으로 선택한 경우 확인을 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-161">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="bbd17-162">이렇게 하면 참조 된 SAP 번호가 조직에 속해 있음을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-162">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="bbd17-163">Microsoft 비즈니스 엔터티가 여러 개 있는 경우 각 엔터티에 대해 지불 프로필을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-163">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="bbd17-164">지불 방법의 가용성은 동기 프로그램의 규칙에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-164">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="bbd17-165">**통화**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-165">Select the **Currency**.</span></span>

6. <span data-ttu-id="bbd17-166">지불 필드를 모두 완료 한 후 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-166">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="bbd17-167">은행 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="bbd17-167">Create your bank profile</span></span>

<span data-ttu-id="bbd17-168">은행 프로필은 조직 수준에서 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-168">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="bbd17-169">이를 통해 하나의 은행 프로필을 여러 MPN ID에 할당 하 고 조직 내의 프로그램을 프로 파일링 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-169">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="bbd17-170">서로 다른 은행 및 세금 규칙이 적용 될 수 있으므로 은행 프로필을 다른 국가에 적용 하는 경우 예외가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-170">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="bbd17-171">다음 페이지에서는 별표가 있는 필드가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-171">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="bbd17-172">필드가 무엇 인지 모르는 경우 정보 아이콘을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-172">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="bbd17-173">**세부 정보** 페이지에서 다음 필드를 완료 합니다. **프로필 이름:** 이 지불 프로필을 식별 하는 고유한 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-173">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="bbd17-174">**은행 계좌 위치:** 회사의 은행이 있는 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-174">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="bbd17-175">**지불 방법:** 파트너 센터에 대 한 기본 결제 방법은 전자 은행 전송입니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-175">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="bbd17-176">**다음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-176">Select **Next**.</span></span>

3. <span data-ttu-id="bbd17-177">**은행 계좌** 페이지에서 사용자 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-177">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="bbd17-178">이 페이지에 표시 되는 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-178">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="bbd17-179">**다음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-179">Select **Next**.</span></span>

5. <span data-ttu-id="bbd17-180">**수혜자** 페이지에서 적절 한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-180">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="bbd17-181">수혜자는 회사에서 사용자 계정에 대해 논의 해야 하는 경우 은행에 연락 하는 사람입니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-181">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="bbd17-182">필드가 완료 되 면 **마침**을 선택 하 고 **확인** 을 선택 하 여 은행 프로필을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-182">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="bbd17-183">**지급 및 세금 프로필** 페이지로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-183">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="bbd17-184">새 프로필의 상태는 유효성 검사가 완료 될 때까지 **보류 중인 Microsoft 유효성 검사** 를 반영 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-184">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="bbd17-185">이 프로세스는 최대 48 시간까지 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-185">This process may take up to 48 hours.</span></span> <span data-ttu-id="bbd17-186">유효성 검사가 완료 되 면 프로필 상태가 **승인 됨** 또는 **필수 작업**으로 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-186">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="bbd17-187">**조치가 필요한**경우 위의 단계를 반복 하 여 필요한 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-187">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="bbd17-188">세금 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="bbd17-188">Create your tax profile</span></span>

<span data-ttu-id="bbd17-189">Microsoft에서 조직에 필요한 세금 정보를 제공 하려면 다음 절차를 따르십시오.</span><span class="sxs-lookup"><span data-stu-id="bbd17-189">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="bbd17-190">이 섹션의 페이지는 동적 이며 국가나 지역에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-190">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="bbd17-191">올바른 세금 정보를 식별 하는 데 도움이 필요한 경우 해당 국가의 적절 한 정부 기관에 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="bbd17-191">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="bbd17-192">W8 또는 W9 양식을 완료 하는 방법에 대 한 정보가 필요한 경우에는 미국에 있는 파트너 회사의 경우 다음 주소가 IRS 사이트로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-192">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="bbd17-193">회사에 대 한 세부 정보만 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-193">Enter only details for your company.</span></span> <span data-ttu-id="bbd17-194">개인 정보를 입력 하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="bbd17-194">Never enter personal details.</span></span>

1. <span data-ttu-id="bbd17-195">**비즈니스 프로필** 페이지에서 필수 필드를 입력 하 고 **다음**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-195">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="bbd17-196">**설치** 페이지에서 회사에 적용 되는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-196">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="bbd17-197">회사가 미국에만 통합 되어 있거나 개인에 대 한 프로필 인 경우 왼쪽에 있는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-197">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="bbd17-198">회사를 미국 외 지역에 통합 하는 경우 오른쪽의 옵션을 선택 하 고 목록에서 국가/지역을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-198">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="bbd17-199">**다음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-199">Select **Next**.</span></span> 

4. <span data-ttu-id="bbd17-200">**세금 상태** 페이지에서 필요한 정보를 입력 하 고 **다음**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-200">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="bbd17-201">이 페이지의 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-201">Fields on this page will vary by country.</span></span> <span data-ttu-id="bbd17-202">사용자의 세부 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-202">your details.</span></span> 

5. <span data-ttu-id="bbd17-203">**추가 설명서** 페이지에서 필수 필드를 선택 하 고 **다음**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-203">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="bbd17-204">**찾아보기** 를 선택 하 여 국가 또는 지역에 필요한 문서를 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-204">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="bbd17-205">문서 이름이 표시 되 면 **업로드**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-205">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="bbd17-206">문서를 제거 해야 하는 경우 **제거**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-206">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="bbd17-207">저장 하 고 계속 하려면 **마침**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-207">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="bbd17-208">팝업 메시지에서 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-208">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="bbd17-209">**지급 및 세금 설치** 페이지로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="bbd17-209">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bbd17-210">다음 단계</span><span class="sxs-lookup"><span data-stu-id="bbd17-210">Next steps</span></span>

- [<span data-ttu-id="bbd17-211">인센티브 지급 및 세금 프로필 FAQ</span><span class="sxs-lookup"><span data-stu-id="bbd17-211">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
