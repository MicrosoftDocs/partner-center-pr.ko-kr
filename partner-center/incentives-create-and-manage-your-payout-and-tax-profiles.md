---
title: 파트너 센터에서 지급 및 세금 프로필
ms.topic: how-to
ms.date: 04/15/2021
description: 지급 및 세금 프로필을 만들고 관리 하 여 성과급 작업에 대해 지불할 수 있습니다. 다른 프로필을 만들고, 관리 하 고, 사용 하는 등의 작업이 포함 됩니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684256"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="47d65-104">파트너 센터에서 성과급 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="47d65-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="47d65-105">**적절 한 역할**: 성과급 관리자 | 계정 관리자 | 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="47d65-105">**Appropriate roles**: Incentives admin | Account admin | Global admin</span></span>

<span data-ttu-id="47d65-106">특정 MPN 위치에 대한 인센티브 프로그램의 지급금을 받으려면 유효한 지급 및 세금 프로필을 프로그램 및 MPN 위치와 연결하여 등록을 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="47d65-107">Microsoft는이 지급 및 세금 프로필을 사용하여 지급금을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="47d65-108">인센티브 프로그램의 규칙에 따라 전자 계좌 이체 또는 결제 신용 전표를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a><span data-ttu-id="47d65-109">역할, 통화 및 여러 Microsoft 동기 프로그램</span><span class="sxs-lookup"><span data-stu-id="47d65-109">Roles, currencies, and multiple Microsoft incentive programs</span></span>

<span data-ttu-id="47d65-110">지급 및 세금 프로필을 시작 하기 전에 아래 정보를 이해 하는 것이 중요 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-110">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="47d65-111">역할 및 권한</span><span class="sxs-lookup"><span data-stu-id="47d65-111">Roles and permissions</span></span>

<span data-ttu-id="47d65-112">동기 지불액에 대 한 은행 및 세금 정보를 입력 하려면 성과급 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-112">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="47d65-113">MPN/계정 관리자 인 경우 자신 및/또는 동료를 성과급 관리자로 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-113">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="47d65-114">성과급 관리자 권한을 요청 해야 하는 경우 MPN 관리자 또는 전역 관리자에 게 문의 하세요. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인 하 여 회사에서 이러한 역할을 가진 사람을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-114">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="47d65-115">오른쪽 위의 **설정** 아이콘에서 **사용자 관리** 를 선택 하 고 전역 관리자에서 필터링 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-115">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="47d65-116">성과급 사용자는 동기 수입 및 지불 정보 및 보고서를 볼 수 있지만, 은행 및 세금 정보는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-116">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="47d65-117">자금 지출 통화를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-117">Choose your disbursement currency</span></span>

<span data-ttu-id="47d65-118">지불 프로필을 설정할 때 선택한 통화로 지불 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-118">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="47d65-119">지불은 Microsoft에서 매월 설정한 환율을 사용 하 여 계산 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-119">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="47d65-120">선택한 통화로 인 한 값의 변경에 대 한 책임이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-120">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="47d65-121">Microsoft 프로그램 마다 다른 프로필 사용</span><span class="sxs-lookup"><span data-stu-id="47d65-121">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="47d65-122">회사에서 여러 개의 동기 프로그램을 등록 한 경우에는 모든 사용자에 대해 동일한 결제 계정을 사용 하거나 다른 프로그램에 다른 지불 계정을 사용 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-122">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="47d65-123">파트너 센터에서 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="47d65-123">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="47d65-124">아래 섹션에서는 파트너 센터에서 결제 및 세금 프로필을 만들고 관리 하는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-124">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="47d65-125">파트너 센터에서 결제 및 세금 프로필을 만들거나 관리 하려면 동기 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-125">You must be an Incentive admin to create or manage payment and tax profiles in Partner Center.</span></span> <span data-ttu-id="47d65-126">각 동기 프로그램의 각 MPN 위치에는 동기 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-126">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="47d65-127">파트너 센터에서 동기 관리자를 추가 하는 방법에 대 한 자세한 내용은 [사용자 계정 만들기](create-user-accounts-and-set-permissions.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="47d65-127">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="47d65-128">파트너 센터의 지급 및 세금 섹션 액세스</span><span class="sxs-lookup"><span data-stu-id="47d65-128">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="47d65-129">Azure Active Directory (Azure AD) 계정 (회사 계정)을 사용 하 여 [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/) 로그인 하거나, 할당 된 경우 적절 한 전자 메일 주소를 사용 하 여 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-129">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="47d65-130">하나의 Azure AD 계정 내에 여러 도메인을 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-130">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="47d65-131">전역 관리자에 게 문의 하 여 연결 된 도메인을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-131">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="47d65-132">도메인에만 로그인 할 수 @onmicrosoft.com 있고 추가 도메인이 필요한 경우 계정 관리자에 게 문의 하 여 AZURE AD 계정에 도메인을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-132">If you're only able to sign in with the @onmicrosoft.com domain and you need additional domains, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="47d65-133">**회사 또는 학교** 계정 또는 **개인 계정을** 선택 하 라는 메시지가 표시 되 면 **회사 또는 학교 계정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-133">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="47d65-134">기어 아이콘을 선택 하 여 **설정** 메뉴를 열고 **계정 설정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-134">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="47d65-135">**계정 설정** 메뉴에서 **지급 및 세금** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-135">In the **Account settings** menu, select **Payout and tax**.</span></span>

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="47d65-136">개별 프로그램에 지급 및 세금 프로필 할당</span><span class="sxs-lookup"><span data-stu-id="47d65-136">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="47d65-137">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 하 고 기어 아이콘을 선택 하 여 **설정** 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="47d65-138">**계정 설정** 을 선택 하 고 **지급 및 세금 섹션** 을 확장 한 다음 **지급 및 세금 프로필 할당** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-138">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="47d65-139">프로그램 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-139">A list of your programs will be displayed.</span></span> <span data-ttu-id="47d65-140">프로그램 옆의 화살표를 선택 하 여 프로필 세부 정보를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-140">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="47d65-141">**세금 프로필** 드롭다운 메뉴에서 원하는 세금 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-141">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="47d65-142">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-142">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="47d65-143">팝업 창에서 **계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-143">Select **Continue** in the pop-up window.</span></span> <span data-ttu-id="47d65-144">새 세금 프로필을 만드는 프로세스는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-144">The process for creating a new tax profile is provided below.</span></span>

4. <span data-ttu-id="47d65-145">**지불 방법** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-145">Select **Payment method**.</span></span>

   - <span data-ttu-id="47d65-146">지불 방법으로 **전자 은행 전송** 을 선택한 경우 원하는 지불 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-146">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="47d65-147">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="47d65-148">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="47d65-149">새 지불 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-149">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="47d65-150">**신용 정보** 를 지불 방법으로 선택한 경우 확인을 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-150">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="47d65-151">이렇게 하면 참조 된 SAP 번호가 조직에 속해 있음을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-151">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="47d65-152">Microsoft 비즈니스 엔터티가 여러 개 있는 경우 각 엔터티에 대해 지불 프로필을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-152">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="47d65-153">지불 방법의 가용성은 동기 프로그램의 규칙에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-153">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="47d65-154">특정 동기 프로그램에 대해 로컬 Microsoft 자회사에서 location MPN ID를 지불 하 고 LRD (제한 된 위험 배포자) 신용 메모를 지불 방법으로 허용 하는 경우 지불 프로필은 LRD 신용 메모 지불 방법으로 미리 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-154">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="47d65-155">각 동기 프로그램 및 위치 MPN ID에 대 한 LRD 신용 메모 지불 방법 행에서 지불 프로필 섹션의 **상태로 확인 또는** **확인 필요** 가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-155">On the LRD credit note payment method row for the respective incentive program and location MPN ID, you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="47d65-156">신용 메모 지불을 받으려면 location MPN and 결제 방법과 연결 된 CSP 테 넌 트 ID 세부 정보를 확인 하 고 확인 하는 데 **필요한 확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-156">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="47d65-157">**신용 메모 세부 정보** 대화 상자에서 제공 된 CSP 테 넌 트 ID 및 세부 정보가 올바른지 확인 하 고 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-157">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="47d65-158">둘 이상의 테 넌 트 ID가 표시 되는 경우 지불액을 받으려는 CSP 테 넌 트 ID를 신중 하 게 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-158">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="47d65-159">그런 다음, **확인** 을 선택 하 여 회사 세부 정보가 올바른지 확인 하 고, 선택한 CSP 테 넌 트 ID에 대해 동기를 지불 해야 한다는 것을 승인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-159">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="47d65-160">상태가 **확인** 됨으로 표시 되 면 CSP 테 넌 트 ID의 할당이 완료 된 것 이며 추가 작업이 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-160">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="47d65-161">확인을 선택 하 여 할당에 대 한 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-161">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="47d65-162">파트너에 게 세금 면제 적용을 명시적으로 요청 하는 것을 요청 하는 국가에서는 동기 프로그램 및 위치 MPN의 세금 프로필 섹션에서 세금 프로필 옆에 세금 면제를 적용 하는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-162">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="47d65-163">이 확인란을 선택 하면 사용자의 동기 크레딧 메모에 세금 면제 혜택이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-163">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="47d65-164">현재 LRD 신용 메모 지불 방법은 Microsoft 상거래 동기 프로그램을 위한 오스트레일리아, 뉴질랜드 및 캐나다 파트너 에게만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-164">Currently, the LRD Credit Note payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="47d65-165">MCI 프로그램에 대해 등록 된이 세 국가에서 직접 청구 파트너 또는 간접 공급자 인 경우 사용 가능한 지불 방법으로 LRD 크레딧 정보를 표시 하지 않으려면 테 넌 트 ID가 관련 파트너 MPN 위치 계정과 연결 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-165">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="47d65-166">이에 대 한 자세한 내용은 [조직 프로필을 업데이트 하는 방법](update-your-partner-profile.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="47d65-166">For more information on this, read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="47d65-167">**통화** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-167">Select the **Currency**.</span></span>

6. <span data-ttu-id="47d65-168">지불 필드를 모두 완료 한 후 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-168">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="set-up-a-default-bank-profile"></a><span data-ttu-id="47d65-169">기본 은행 프로필 설정</span><span class="sxs-lookup"><span data-stu-id="47d65-169">Set up a default bank profile</span></span>

<span data-ttu-id="47d65-170">기본 은행 프로필을 설정하고 MPN 위치에 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-170">You can set up default bank profiles and assign them to MPN locations.</span></span> <span data-ttu-id="47d65-171">이러한 기본 프로필은 해당 MPN 위치에 대한 후속 등록을 위해 Microsoft에서 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-171">These defaults profiles will be used by Microsoft for subsequent enrollments for that MPN location.</span></span> 

1. <span data-ttu-id="47d65-172">[파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 하 고 기어 아이콘을 선택 하 여 설정 메뉴를 엽니다 \*\*\*\*   .</span><span class="sxs-lookup"><span data-stu-id="47d65-172">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/),  and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="47d65-173"> *\*계정 설정** 을 선택 하 고 *\*지급 및 세금** 섹션을 확장 한 다음 *\*지급 및 세금 프로필** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-173">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profiles**.</span></span> 

3. <span data-ttu-id="47d65-174">**지불 프로필** 섹션에서 **기본 프로필 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-174">Select **Manage default profiles** under the **Payment profiles** section.</span></span> 

4. <span data-ttu-id="47d65-175">기본 은행 프로필을 만들려면 **기본 은행 프로필 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-175">To create a default bank profile, select **Add a default bank profile**.</span></span> 

5. <span data-ttu-id="47d65-176">회사의 사용 가능한 은행 프로필 목록에서 은행 프로필을 선택 하 고,이 은행 프로필에 사용할 통화를 선택한 다음,이 기본 프로필을 적용할 MPN 위치 목록을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-176">Select a bank profile from the list of available bank profiles of your company, select the currency to be used with this bank profile, and then select the list of MPN locations for which you want this default profile to apply.</span></span>

6. <span data-ttu-id="47d65-177">선택 항목을 완료 한 후에 **완료** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-177">Select **Done** once you have completed the selections.</span></span> <span data-ttu-id="47d65-178">모든 필수 필드가 완료 될 때까지 완료 단추를 클릭할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-178">The Done button will not be clickable until all required fields have been completed.</span></span> 

>[!NOTE]
><span data-ttu-id="47d65-179">동일한 은행 및 통화 페어링은 여러 위치에 적용 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-179">The same bank and currency pairing can be applied to multiple locations.</span></span> <span data-ttu-id="47d65-180">MPN 위치에 기본 프로필과 통화 조합이 한 번 할당 된 경우 나중에 기본 프로필 할당을 위해 위치 드롭다운에서 더 이상 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-180">If the location MPN has been assigned a default profile and currency combination once, it will no longer appear in the location dropdown for future default profile assignments.</span></span> <span data-ttu-id="47d65-181">기본 선택 항목이 삭제 되 면 이후 기본 프로필 할당을 위해 MPN 위치가 다시 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-181">If the default selection is deleted, the location MPN will reappear for future default profile assignments.</span></span> <span data-ttu-id="47d65-182">각 은행 프로필 및 통화 조합은 편집 가능한 고유 행으로 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-182">Each bank profile and currency combination is added as an unique, editable row.</span></span>

7. <span data-ttu-id="47d65-183">필요한 변경 내용이 모두 추가 되 면 **저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-183">Once all the required changes have been added, select **Save**.</span></span>  

## <a name="create-your-bank-profile"></a><span data-ttu-id="47d65-184">은행 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="47d65-184">Create your bank profile</span></span>

<span data-ttu-id="47d65-185">은행 프로필은 회사 수준에서 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-185">Bank profiles are created at a company level.</span></span> <span data-ttu-id="47d65-186">이를 통해 하나의 은행 프로필을 여러 MPN ID에 할당 하 고 회사 내의 프로그램을 프로 파일링 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-186">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within a company.</span></span> <span data-ttu-id="47d65-187">서로 다른 은행 및 세금 규칙이 적용 될 수 있으므로 은행 프로필을 다른 국가에 적용 하는 경우 예외가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-187">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="47d65-188">다음 페이지에서는 별표가 있는 필드가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-188">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="47d65-189">필드가 무엇 인지 모르는 경우 정보 아이콘을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-189">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="47d65-190">**세부 정보** 페이지에서 다음 필드를 완료 합니다. **프로필 이름:** 이 지불 프로필을 식별 하는 고유한 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-190">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="47d65-191">**은행 계좌 위치:** 회사의 은행이 있는 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-191">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="47d65-192">**지불 방법:** 파트너 센터에 대 한 기본 결제 방법은 전자 은행 전송입니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-192">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="47d65-193">**다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-193">Select **Next**.</span></span>

3. <span data-ttu-id="47d65-194">**은행 계좌** 페이지에서 사용자 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-194">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="47d65-195">이 페이지에 표시 되는 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-195">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="47d65-196">**다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-196">Select **Next**.</span></span>

5. <span data-ttu-id="47d65-197">**수혜자** 페이지에서 적절 한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-197">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="47d65-198">수혜자는 회사에서 사용자 계정에 대해 논의 해야 하는 경우 은행에 연락 하는 사람입니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-198">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="47d65-199">필드가 완료 되 면 **마침** 을 선택 하 고 **확인** 을 선택 하 여 은행 프로필을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-199">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="47d65-200">**지급 및 세금 프로필** 페이지로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-200">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="47d65-201">유효성 검사가 완료될 때까지 새 프로필의 상태는 **보류 중인 Microsoft 유효성** 검사를 반영합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-201">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="47d65-202">이 프로세스는 최대 48시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-202">This process may take up to 48 hours.</span></span> <span data-ttu-id="47d65-203">유효성 검사가 완료되면 프로필 상태에 승인 또는 **작업 필요** **가** 반영됩니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-203">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="47d65-204">**작업이 필요한** 경우 위의 단계를 반복하여 필요한 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-204">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="47d65-205">세금 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="47d65-205">Create your tax profile</span></span>

<span data-ttu-id="47d65-206">다음 절차에 따라 조직에 필요한 세금 정보를 Microsoft에 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-206">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="47d65-207">이 섹션의 페이지는 동적이며 국가 또는 지역에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-207">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="47d65-208">올바른 세금 정보를 식별하는 데 도움이 필요한 경우 해당 국가의 적절한 정부 출처에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="47d65-208">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="47d65-209">미국 내 파트너 회사의 경우 W8 또는 W9 양식을 작성하기 위한 정보가 필요한 경우 다음 주소를 통해 IRS 사이트로 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-209">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="47d65-210">회사에 대한 세부 정보만 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-210">Enter only details for your company.</span></span> <span data-ttu-id="47d65-211">개인 정보를 입력하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-211">Never enter personal details.</span></span>

1. <span data-ttu-id="47d65-212">비즈니스 **프로필** 페이지에서 필수 필드를 완료한 후 **다음을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-212">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="47d65-213">**설치** 페이지에서 회사에 적용되는 옵션을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-213">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="47d65-214">회사가 미국만 통합된 경우 또는 개인용 프로필인 경우 왼쪽의 옵션을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-214">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="47d65-215">회사가 미국 외부에 통합된 경우 오른쪽의 옵션을 선택한 다음, 목록에서 해당 국가/지역을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-215">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="47d65-216">**다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-216">Select **Next**.</span></span> 

4. <span data-ttu-id="47d65-217">세금 **상태** 페이지에서 필요한 정보를 입력한 후 **다음을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-217">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="47d65-218">이 페이지의 필드는 국가별로 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-218">Fields on this page will vary by country.</span></span> <span data-ttu-id="47d65-219">세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-219">your details.</span></span> 

5. <span data-ttu-id="47d65-220">추가 **설명서** 페이지에서 필수 필드를 선택하고 **다음을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-220">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="47d65-221">**찾아보기를** 선택하여 해당 국가 또는 지역에 필요한 문서를 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-221">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="47d65-222">문서 이름이 표시되면 **업로드** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-222">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="47d65-223">문서를 제거해야 하는 경우 **제거를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-223">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="47d65-224">저장하고 계속하려면 **마침을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-224">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="47d65-225">팝업 메시지에서 **확인을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-225">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="47d65-226">**지급 및 세금 설정** 페이지로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-226">You’ll be taken back to the **Payout and tax setup** page.</span></span>
 
## <a name="update-expired-tax-profiles"></a><span data-ttu-id="47d65-227">만료된 세금 프로필 업데이트</span><span class="sxs-lookup"><span data-stu-id="47d65-227">Update expired tax profiles</span></span>

1. <span data-ttu-id="47d65-228">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인한 다음 기어 아이콘을 선택하여 **설정** 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-228">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span>

1. <span data-ttu-id="47d65-229">**계정 설정을** 선택하고 **지급 및 세금** 섹션을 확장한 다음 지급 및 세금 **프로필을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-229">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profile**.</span></span>

1. <span data-ttu-id="47d65-230">**세금 프로필** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-230">Select **Tax profile**.</span></span>

1. <span data-ttu-id="47d65-231">**만료 날짜** 열을 확인하고 만료되거나 만료될 세금 프로필로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-231">Check the column **Expiration Date** and navigate to the tax profile that is expired or about to expire.</span></span>

1. <span data-ttu-id="47d65-232">**편집** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-232">Select **Edit**.</span></span>

1. <span data-ttu-id="47d65-233">세금 양식 섹션에서 새 세부 정보를 제공하여 세금 양식을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="47d65-233">In the tax form section, update the tax forms by providing the new details.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="47d65-234">다음 단계</span><span class="sxs-lookup"><span data-stu-id="47d65-234">Next steps</span></span>

- [<span data-ttu-id="47d65-235">지급 및 세금에 대한 일반적인 질문</span><span class="sxs-lookup"><span data-stu-id="47d65-235">Common questions about payouts and taxes</span></span>](payout-faq.yml)
