---
title: 파트너 센터에서 지급 및 세금 프로필
ms.topic: how-to
ms.date: 02/24/2021
description: 지급 및 세금 프로필을 만들고 관리 하 여 성과급 작업에 대해 지불할 수 있습니다. 다른 프로필을 만들고, 관리 하 고, 사용 하는 등의 작업이 포함 됩니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ba8c1a811d66a5e6233f625c3981283341ea546c
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756592"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="dd05e-104">파트너 센터에서 성과급 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="dd05e-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="dd05e-105">**적절한 역할:**</span><span class="sxs-lookup"><span data-stu-id="dd05e-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="dd05e-106">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="dd05e-106">Incentives admin</span></span>
- <span data-ttu-id="dd05e-107">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="dd05e-107">Account admin</span></span>
- <span data-ttu-id="dd05e-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="dd05e-108">Global admin</span></span>

<span data-ttu-id="dd05e-109">특정 MPN 위치에 대한 인센티브 프로그램의 지급금을 받으려면 유효한 지급 및 세금 프로필을 프로그램 및 MPN 위치와 연결하여 등록을 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="dd05e-110">Microsoft는이 지급 및 세금 프로필을 사용하여 지급금을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="dd05e-111">인센티브 프로그램의 규칙에 따라 전자 계좌 이체 또는 결제 신용 전표를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="dd05e-112">역할, 통화 및 기타 Microsoft 프로그램</span><span class="sxs-lookup"><span data-stu-id="dd05e-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="dd05e-113">지급 및 세금 프로필을 시작 하기 전에 아래 정보를 이해 하는 것이 중요 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="dd05e-114">역할 및 권한</span><span class="sxs-lookup"><span data-stu-id="dd05e-114">Roles and permissions</span></span>

<span data-ttu-id="dd05e-115">동기 지불액에 대 한 은행 및 세금 정보를 입력 하려면 성과급 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="dd05e-116">MPN/계정 관리자 인 경우 자신 및/또는 동료를 성과급 관리자로 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="dd05e-117">성과급 관리자 권한을 요청 해야 하는 경우 MPN 관리자 또는 전역 관리자에 게 문의 하세요. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인 하 여 회사에서 이러한 역할을 가진 사람을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="dd05e-118">오른쪽 위의 **설정** 아이콘에서 **사용자 관리** 를 선택 하 고 전역 관리자에서 필터링 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="dd05e-119">성과급 사용자는 동기 수입 및 지불 정보 및 보고서를 볼 수 있지만, 은행 및 세금 정보는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="dd05e-120">자금 지출 통화를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-120">Choose your disbursement currency</span></span>

<span data-ttu-id="dd05e-121">지불 프로필을 설정할 때 선택한 통화로 지불 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="dd05e-122">지불은 Microsoft에서 매월 설정한 환율을 사용 하 여 계산 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="dd05e-123">선택한 통화로 인 한 값의 변경에 대 한 책임이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="dd05e-124">Microsoft 프로그램 마다 다른 프로필 사용</span><span class="sxs-lookup"><span data-stu-id="dd05e-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="dd05e-125">회사에서 여러 개의 동기 프로그램을 등록 한 경우에는 모든 사용자에 대해 동일한 결제 계정을 사용 하거나 다른 프로그램에 다른 지불 계정을 사용 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="dd05e-126">파트너 센터에서 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="dd05e-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="dd05e-127">아래 섹션에서는 파트너 센터에서 결제 및 세금 프로필을 만들고 관리 하는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="dd05e-128">파트너 센터에서 지불 프로필을 만들거나 관리 하려면 동기 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="dd05e-129">각 동기 프로그램의 각 MPN 위치에는 동기 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="dd05e-130">파트너 센터에서 동기 관리자를 추가 하는 방법에 대 한 자세한 내용은 [사용자 계정 만들기](create-user-accounts-and-set-permissions.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="dd05e-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="dd05e-131">파트너 센터의 지급 및 세금 섹션 액세스</span><span class="sxs-lookup"><span data-stu-id="dd05e-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="dd05e-132">Azure Active Directory (Azure AD) 계정 (회사 계정)을 사용 하 여 [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/) 로그인 하거나, 할당 된 경우 적절 한 전자 메일 주소를 사용 하 여 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="dd05e-133">하나의 Azure AD 계정 내에 여러 도메인을 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="dd05e-134">전역 관리자에 게 문의 하 여 연결 된 도메인을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="dd05e-135">도메인을 사용 하 여 로그인 할 수 있는 경우 @onmicrosoft.com 계정 관리자에 게 문의 하 여 AZURE AD 계정에 도메인을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="dd05e-136">**회사 또는 학교** 계정 또는 **개인 계정을** 선택 하 라는 메시지가 표시 되 면 **회사 또는 학교 계정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="dd05e-137">기어 아이콘을 선택 하 여 **설정** 메뉴를 열고 **계정 설정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="dd05e-138">**계정 설정** 메뉴에서 **지급 및 세금** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="dd05e-139">개별 프로그램에 지급 및 세금 프로필 할당</span><span class="sxs-lookup"><span data-stu-id="dd05e-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="dd05e-140">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 하 고 기어 아이콘을 선택 하 여 **설정** 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="dd05e-141">**계정 설정** 을 선택 하 고 **지급 및 세금 섹션** 을 확장 한 다음 **지급 및 세금 프로필 할당** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="dd05e-142">프로그램 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="dd05e-143">프로그램 옆의 화살표를 선택 하 여 프로필 세부 정보를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="dd05e-144">**세금 프로필** 드롭다운 메뉴에서 원하는 세금 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="dd05e-145">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="dd05e-146">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="dd05e-147">새 세금 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="dd05e-148">**지불 방법** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="dd05e-149">지불 방법으로 **전자 은행 전송** 을 선택한 경우 원하는 지불 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="dd05e-150">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="dd05e-151">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="dd05e-152">새 지불 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="dd05e-153">**신용 정보** 를 지불 방법으로 선택한 경우 확인을 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="dd05e-154">이렇게 하면 참조 된 SAP 번호가 조직에 속해 있음을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="dd05e-155">Microsoft 비즈니스 엔터티가 여러 개 있는 경우 각 엔터티에 대해 지불 프로필을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="dd05e-156">지불 방법의 가용성은 동기 프로그램의 규칙에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-156">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="dd05e-157">특정 동기 프로그램에 대해 로컬 Microsoft 자회사에서 location MPN ID를 지불 하 고 LRD (제한 된 위험 배포자) 신용 메모를 지불 방법으로 허용 하는 경우 지불 프로필은 LRD 신용 메모 지불 방법으로 미리 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-157">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="dd05e-158">각 동기 프로그램 및 위치 MPN ID에 대 한 LRD 신용 메모 지불 방법 행에서 지불 프로필 섹션의 상태로 **확인 또는** **확인 필요** 가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-158">On the LRD credit note payment method row for the respective incentive program and location MPN ID you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="dd05e-159">신용 메모 지불을 받으려면 location MPN and 결제 방법과 연결 된 CSP 테 넌 트 ID 세부 정보를 확인 하 고 확인 하는 데 **필요한 확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-159">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="dd05e-160">**신용 메모 세부 정보** 대화 상자에서 제공 된 CSP 테 넌 트 ID 및 세부 정보가 올바른지 확인 하 고 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-160">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="dd05e-161">둘 이상의 테 넌 트 ID가 표시 되는 경우 지불액을 받으려는 CSP 테 넌 트 ID를 신중 하 게 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-161">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="dd05e-162">그런 다음, **확인** 을 선택 하 여 회사 세부 정보가 올바른지 확인 하 고, 선택한 CSP 테 넌 트 ID에 대해 동기를 지불 해야 한다는 것을 승인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-162">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="dd05e-163">상태가 **확인** 됨으로 표시 되 면 CSP 테 넌 트 ID의 할당이 완료 된 것 이며 추가 작업이 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-163">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="dd05e-164">확인을 선택 하 여 할당에 대 한 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-164">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="dd05e-165">파트너에 게 세금 면제 적용을 명시적으로 요청 하는 것을 요청 하는 국가에서는 동기 프로그램 및 위치 MPN의 세금 프로필 섹션에서 세금 프로필 옆에 세금 면제를 적용 하는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-165">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="dd05e-166">이 확인란을 선택 하면 사용자의 동기 크레딧 메모에 세금 면제 혜택이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-166">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="dd05e-167">현재이 결제 방법은 Microsoft 상거래 동기 프로그램을 위한 오스트레일리아, 뉴질랜드 및 캐나다 파트너 에게만 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-167">Currently, this payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="dd05e-168">MCI 프로그램에 대해 등록 된이 세 국가에서 직접 청구 파트너 또는 간접 공급자 인 경우 사용 가능한 지불 방법으로 LRD 크레딧 정보를 표시 하지 않으려면 테 넌 트 ID가 관련 파트너 MPN 위치 계정과 연결 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-168">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="dd05e-169">이에 대 한 자세한 내용은 [조직 프로필을 업데이트 하는 방법을](update-your-partner-profile.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="dd05e-169">For more information on this read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="dd05e-170">**통화** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-170">Select the **Currency**.</span></span>

6. <span data-ttu-id="dd05e-171">지불 필드를 모두 완료 한 후 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-171">When you’ve completed all of the payment fields, select **Submit**.</span></span>


## <a name="create-your-bank-profile"></a><span data-ttu-id="dd05e-172">은행 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="dd05e-172">Create your bank profile</span></span>

<span data-ttu-id="dd05e-173">은행 프로필은 조직 수준에서 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-173">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="dd05e-174">이를 통해 하나의 은행 프로필을 여러 MPN ID에 할당 하 고 조직 내의 프로그램을 프로 파일링 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-174">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="dd05e-175">서로 다른 은행 및 세금 규칙이 적용 될 수 있으므로 은행 프로필을 다른 국가에 적용 하는 경우 예외가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-175">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="dd05e-176">다음 페이지에서는 별표가 있는 필드가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-176">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="dd05e-177">필드가 무엇 인지 모르는 경우 정보 아이콘을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-177">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="dd05e-178">**세부 정보** 페이지에서 다음 필드를 완료 합니다. **프로필 이름:** 이 지불 프로필을 식별 하는 고유한 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-178">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="dd05e-179">**은행 계좌 위치:** 회사의 은행이 있는 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-179">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="dd05e-180">**지불 방법:** 파트너 센터에 대 한 기본 결제 방법은 전자 은행 전송입니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-180">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="dd05e-181">**다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-181">Select **Next**.</span></span>

3. <span data-ttu-id="dd05e-182">**은행 계좌** 페이지에서 사용자 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-182">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="dd05e-183">이 페이지에 표시 되는 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-183">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="dd05e-184">**다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-184">Select **Next**.</span></span>

5. <span data-ttu-id="dd05e-185">**수혜자** 페이지에서 적절 한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-185">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="dd05e-186">수혜자는 회사에서 사용자 계정에 대해 논의 해야 하는 경우 은행에 연락 하는 사람입니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-186">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="dd05e-187">필드가 완료 되 면 **마침** 을 선택 하 고 **확인** 을 선택 하 여 은행 프로필을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-187">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="dd05e-188">**지급 및 세금 프로필** 페이지로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-188">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="dd05e-189">새 프로필의 상태는 유효성 검사가 완료 될 때까지 **보류 중인 Microsoft 유효성 검사** 를 반영 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-189">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="dd05e-190">이 프로세스는 최대 48 시간까지 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-190">This process may take up to 48 hours.</span></span> <span data-ttu-id="dd05e-191">유효성 검사가 완료 되 면 프로필 상태가 **승인 됨** 또는 **필수 작업** 으로 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-191">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="dd05e-192">**조치가 필요한** 경우 위의 단계를 반복 하 여 필요한 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-192">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="dd05e-193">세금 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="dd05e-193">Create your tax profile</span></span>

<span data-ttu-id="dd05e-194">Microsoft에서 조직에 필요한 세금 정보를 제공 하려면 다음 절차를 따르십시오.</span><span class="sxs-lookup"><span data-stu-id="dd05e-194">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="dd05e-195">이 섹션의 페이지는 동적 이며 국가나 지역에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-195">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="dd05e-196">올바른 세금 정보를 식별 하는 데 도움이 필요한 경우 해당 국가의 적절 한 정부 기관에 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="dd05e-196">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="dd05e-197">W8 또는 W9 양식을 완료 하는 방법에 대 한 정보가 필요한 경우에는 미국에 있는 파트너 회사의 경우 다음 주소가 IRS 사이트로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-197">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="dd05e-198">회사에 대 한 세부 정보만 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-198">Enter only details for your company.</span></span> <span data-ttu-id="dd05e-199">개인 정보를 입력 하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="dd05e-199">Never enter personal details.</span></span>

1. <span data-ttu-id="dd05e-200">**비즈니스 프로필** 페이지에서 필수 필드를 입력 하 고 **다음** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-200">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="dd05e-201">**설치** 페이지에서 회사에 적용 되는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-201">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="dd05e-202">회사가 미국에만 통합 되어 있거나 개인에 대 한 프로필 인 경우 왼쪽에 있는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-202">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="dd05e-203">회사를 미국 외 지역에 통합 하는 경우 오른쪽의 옵션을 선택 하 고 목록에서 국가/지역을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-203">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="dd05e-204">**다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-204">Select **Next**.</span></span> 

4. <span data-ttu-id="dd05e-205">**세금 상태** 페이지에서 필요한 정보를 입력 하 고 **다음** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-205">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="dd05e-206">이 페이지의 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-206">Fields on this page will vary by country.</span></span> <span data-ttu-id="dd05e-207">사용자의 세부 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-207">your details.</span></span> 

5. <span data-ttu-id="dd05e-208">**추가 설명서** 페이지에서 필수 필드를 선택 하 고 **다음** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-208">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="dd05e-209">**찾아보기** 를 선택 하 여 국가 또는 지역에 필요한 문서를 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-209">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="dd05e-210">문서 이름이 표시 되 면 **업로드** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-210">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="dd05e-211">문서를 제거 해야 하는 경우 **제거** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-211">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="dd05e-212">저장 하 고 계속 하려면 **마침** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-212">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="dd05e-213">팝업 메시지에서 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-213">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="dd05e-214">**지급 및 세금 설치** 페이지로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="dd05e-214">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dd05e-215">다음 단계</span><span class="sxs-lookup"><span data-stu-id="dd05e-215">Next steps</span></span>

- [<span data-ttu-id="dd05e-216">지급 및 세금에 대 한 일반적인 질문</span><span class="sxs-lookup"><span data-stu-id="dd05e-216">Common questions about payouts and taxes</span></span>](payout-faq.md)
