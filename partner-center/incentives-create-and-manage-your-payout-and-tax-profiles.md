---
title: 파트너 센터에서 지급 및 세금 프로필 만들기 및 관리
ms.topic: article
ms.date: 06/29/2020
description: 성과급 작업에 대 한 지불을 받으려면 먼저 지급 및 세금 프로필을 만들어야 합니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: kim-davis
ms.author: kimnich
ms.localizationpriority: medium
ms.openlocfilehash: 02212a09ab18ff5b978107af00ac990aa0c702a3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949682"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="7a2f0-103">파트너 센터의 지급 및 세금 프로필</span><span class="sxs-lookup"><span data-stu-id="7a2f0-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="7a2f0-104">적용 대상:</span><span class="sxs-lookup"><span data-stu-id="7a2f0-104">Applies to:</span></span>

- <span data-ttu-id="7a2f0-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="7a2f0-105">Partner Center</span></span>

<span data-ttu-id="7a2f0-106">특정 MPN 위치에 대한 인센티브 프로그램의 지급금을 받으려면 유효한 지급 및 세금 프로필을 프로그램 및 MPN 위치와 연결하여 등록을 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="7a2f0-107">Microsoft는이 지급 및 세금 프로필을 사용하여 지급금을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="7a2f0-108">인센티브 프로그램의 규칙에 따라 전자 계좌 이체 또는 결제 신용 전표를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="7a2f0-109">적절 한 역할:</span><span class="sxs-lookup"><span data-stu-id="7a2f0-109">Appropriate roles:</span></span>

- <span data-ttu-id="7a2f0-110">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="7a2f0-110">Incentives admin</span></span>
- <span data-ttu-id="7a2f0-111">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="7a2f0-111">Billing admin</span></span>
- <span data-ttu-id="7a2f0-112">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="7a2f0-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="7a2f0-113">파트너 센터에서 지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7a2f0-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="7a2f0-114">아래 섹션에서는 파트너 센터에서 결제 및 세금 프로필을 만들고 관리 하는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="7a2f0-115">파트너 센터에서 지불 프로필을 만들거나 관리 하려면 동기 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="7a2f0-116">각 동기 프로그램의 각 MPN 위치에는 동기 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="7a2f0-117">파트너 센터에서 동기 관리자를 추가 하는 방법에 대 한 자세한 내용은 [파트너 센터에서 동기 사용자 또는 관리자를 추가 하는 방법](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="7a2f0-118">파트너 센터의 지급 및 세금 섹션 액세스</span><span class="sxs-lookup"><span data-stu-id="7a2f0-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="7a2f0-119">AAD 계정 (회사 계정)을 사용 하 여 파트너 센터에 로그인 하거나 할당 된 경우 적절 한 전자 메일 주소를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="7a2f0-120">하나의 AAD 계정 내에 여러 도메인을 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="7a2f0-121">전역 관리자에 게 문의 하 여 연결 된 도메인을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="7a2f0-122">도메인에만 로그인 할 수 있는 경우 **@onmicrosoft.com** 계정 관리자에 게 문의 하 여 AAD 계정에 도메인을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="7a2f0-123">**회사 또는 학교 계정** 또는 **개인 계정을**선택 하 라는 메시지가 표시 되 면 **회사 또는 학교 계정**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="7a2f0-124">기어 아이콘을 선택 하 여 **설정** 메뉴를 열고 **파트너 설정**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="7a2f0-125">**계정 설정** 메뉴에서 **지급 및 세금**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="7a2f0-126">개별 프로그램에 지급 및 세금 프로필 할당</span><span class="sxs-lookup"><span data-stu-id="7a2f0-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="7a2f0-127">파트너 센터에서 기어 아이콘을 선택 하 여 **설정** 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="7a2f0-128">**파트너 설정**을 선택 하 고 **지급 및 세금 섹션**을 확장 한 다음 **지급 및 세금 프로필 할당**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="7a2f0-129">프로그램 목록이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="7a2f0-130">프로그램 옆의 화살표를 선택 하 여 프로필 세부 정보를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="7a2f0-131">**세금 프로필** 드롭다운 메뉴에서 원하는 세금 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="7a2f0-132">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="7a2f0-133">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="7a2f0-134">새 세금 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="7a2f0-135">**지불 방법**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="7a2f0-136">지불 방법으로 **전자 은행 전송** 을 선택한 경우 지불 프로필 드롭다운에서 원하는 지불 프로필을 선택 하거나 새 프로필을 만드는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="7a2f0-137">새 프로필을 만드는 옵션을 선택 하면 적절 하 게 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="7a2f0-138">팝업 창에서 계속을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="7a2f0-139">새 지불 프로필을 만드는 프로세스는 아래에 제공 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="7a2f0-140">**신용 메모** 를 지불 방법으로 선택한 경우 확인을 완료 하 여 참조 된 SAP 번호가 조직에 속해 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="7a2f0-141">Microsoft 비즈니스 엔터티가 여러 개 있는 경우 각 엔터티에 대해 지불 프로필을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="7a2f0-142">지불 방법의 가용성은 동기 프로그램의 규칙에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="7a2f0-143">**통화**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="7a2f0-144">지불 필드를 모두 완료 한 후 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="7a2f0-145">은행 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="7a2f0-145">Create your bank profile</span></span>

<span data-ttu-id="7a2f0-146">은행 프로필은 조직 수준에서 만들어지며,이를 통해 동일한 은행 프로필을 여러 MPN ID에 할당 하 고 조직 내의 프로그램을 프로 파일링 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="7a2f0-147">서로 다른 은행 및 세금 규칙이 적용 될 수 있으므로 은행 프로필을 다른 국가에 적용 하는 경우 예외가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="7a2f0-148">다음 페이지에서는 별표가 있는 필드가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="7a2f0-149">필드가 무엇 인지 모르는 경우 정보 아이콘을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="7a2f0-150">**세부 정보** 페이지에서 다음 필드를 완료 합니다. **프로필 이름:** 이 지불 프로필을 식별 하는 고유한 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="7a2f0-151">**은행 계좌 위치:** 회사의 은행이 있는 국가입니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="7a2f0-152">**지불 방법:** 선호 하는 지불 방법은 파트너 센터에서 전자 은행 전송입니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="7a2f0-153">**새로 만들기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-153">Select **Next**.</span></span>

3. <span data-ttu-id="7a2f0-154">**은행 계좌** 페이지에서 사용자 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="7a2f0-155">이 페이지에 표시 되는 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="7a2f0-156">**새로 만들기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-156">Select **Next**.</span></span>

5. <span data-ttu-id="7a2f0-157">**수혜자** 페이지에서 적절 한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="7a2f0-158">수혜자는 회사에서 사용자 계정에 대해 논의 해야 하는 경우 은행에 연락 하는 사람입니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="7a2f0-159">필드가 완료 되 면 **마침**을 선택 하 고 **확인** 을 선택 하 여 은행 프로필을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="7a2f0-160">**지급 및 세금 프로필** 페이지로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="7a2f0-161">새 프로필의 상태는 유효성 검사가 완료 될 때까지 **보류 중인 Microsoft 유효성 검사** 를 반영 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="7a2f0-162">이 작업에는 최대 48 시간이 소요 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-162">This may take up to 48 hours.</span></span> <span data-ttu-id="7a2f0-163">유효성 검사가 완료 되 면 프로필 상태가 **승인 됨** 또는 **필수 작업**으로 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="7a2f0-164">**조치가 필요한**경우 위의 단계를 반복 하 여 필요한 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="7a2f0-165">세금 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="7a2f0-165">Create your tax profile</span></span>

<span data-ttu-id="7a2f0-166">Microsoft에서 조직에 필요한 세금 정보를 제공 하려면 다음 절차를 따르십시오.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="7a2f0-167">이 섹션의 페이지는 동적 이며 국가나 지역에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="7a2f0-168">올바른 세금 정보를 식별 하는 데 도움이 필요한 경우 해당 국가의 적절 한 정부 기관에 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="7a2f0-169">W8 또는 W9 양식을 완료 하는 방법에 대 한 정보가 필요한 경우에는 미국에 있는 파트너 회사의 경우 다음 주소가 IRS 사이트로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="7a2f0-170">회사에 대 한 세부 정보만 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-170">Enter only details for your company.</span></span> <span data-ttu-id="7a2f0-171">개인 정보를 입력 하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-171">Never enter personal details.</span></span>

1. <span data-ttu-id="7a2f0-172">**비즈니스 프로필** 페이지에서 필수 필드를 입력 하 고 **다음**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="7a2f0-173">**설치** 페이지에서 회사에 적용 되는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="7a2f0-174">회사가 미국에만 통합 되어 있거나 개인에 대 한 프로필 인 경우 왼쪽에 있는 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="7a2f0-175">회사를 미국 외 지역에 통합 하는 경우 오른쪽의 옵션을 선택 하 고 목록에서 국가/지역을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="7a2f0-176">**새로 만들기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-176">Select **Next**.</span></span> 

4. <span data-ttu-id="7a2f0-177">**세금 상태** 페이지에서 필요한 정보를 입력 하 고 **다음**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="7a2f0-178">이 페이지의 필드는 국가별로 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="7a2f0-179">사용자의 세부 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-179">your details.</span></span> 

5. <span data-ttu-id="7a2f0-180">**추가 설명서** 페이지에서 필수 필드를 선택 하 고 **다음**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="7a2f0-181">**찾아보기** 를 선택 하 여 국가 또는 지역에 필요한 문서를 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="7a2f0-182">문서 이름이 표시 되 면 **업로드**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="7a2f0-183">문서를 제거 해야 하는 경우 **제거**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="7a2f0-184">저장 하 고 계속 하려면 **마침**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="7a2f0-185">팝업 메시지에서 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="7a2f0-186">**지급 및 세금 설치** 페이지로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="7a2f0-187">지급 및 세금 프로필 Faq</span><span class="sxs-lookup"><span data-stu-id="7a2f0-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="7a2f0-188">내 지급 및/또는 세금 세부 정보를 제공 해야 하는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="7a2f0-189">Microsoft 동기 프로그램에 대 한 지급을 받으려면 유효한 지급 및 세금 정보를 제공 하 여 등록을 완료 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="7a2f0-190">등록은 Microsoft에서 제공 하는 지급 및 세금 프로필의 유효성을 검사 하는 경우에만 완료 된 것으로 간주 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="7a2f0-191">지급 및/또는 세금 세부 정보를 제공/업데이트 해야 한다는 것을 알고 싶으세요? 어떻게 할까요?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="7a2f0-192">새 동기 프로그램에서 등록 하는 모든 파트너는 등록을 완료 하는 데 유효한 지급 및 세금 정보를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="7a2f0-193">동기 프로그램에 대 한 규칙이 변경 되거나 프로필의 측면이 만료 되었거나 만료 된 경우 업데이트 된 정보를 제공 해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="7a2f0-194">이 경우 개요 페이지에 **작업 필요 – 은행 및/또는 세금 프로필 업데이트**상태가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="7a2f0-195">지급 및/또는 세금 세부 정보를 제공/업데이트하려면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="7a2f0-196">파트너 센터에서 지불 및 세금 정보를 업데이트 하는 방법에 대 한 자세한 내용은 [파트너 센터에서 은행 및 세금 프로필을 만들고 관리 하는 방법](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="7a2f0-197">지급 및 세금 프로필 할당으로 이동할 때 내 등록이 표시되지 않는 이유는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="7a2f0-198">MPN 위치에 대한 인센티브 관리자만 지급 및 세금 프로필을 만들거나 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="7a2f0-199">적절한 권한이 없거나 이러한 권한이 없는 계정으로 로그인했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="7a2f0-200">은행 및 세금에 대한 권한을 관리하려면 조직 관리자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="7a2f0-201">내 조직에 사용할 수 있는 지급 및 세금 프로필은 어디에서 볼 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="7a2f0-202">지급 및 세금 프로필을 보려면 다음 절차를 따르십시오.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="7a2f0-203">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="7a2f0-204">기어 아이콘을 선택하여 **설정** 메뉴를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="7a2f0-205">**파트너 설정**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="7a2f0-206">**계정 설정**에서 **지급 및 세금**을 선택한 다음, **지급 및 세금 프로필**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="7a2f0-207">모든 기존 지급 및 세금 프로필과 상태 및 편집 기능을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="7a2f0-208">조직에서 여러 동기 프로그램에 참여 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="7a2f0-209">지불 및 세금 프로필을 여러 번 제공 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="7a2f0-210">지급 프로필은 일반적으로 사용자가 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="7a2f0-211">지급 프로필은 조직 수준에서 만들어지며, 조직 내 여러 MPN ID 및 인센티브 프로그램에 동일한 은행 프로필을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="7a2f0-212">대부분의 경우 기존 프로필을 다시 사용 하거나 새 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="7a2f0-213">그러나 은행 프로필을 다른 국가 또는 지역에 적용하는 경우에는 현지 은행이나 세금 규칙이 적용될 수 있으므로 예외가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="7a2f0-214">MPN 위치에 대해 만들어진 세금 프로필은 재사용되며 동일한 MPN 위치가 다른 인센티브 프로그램에 참여하는 경우 자동으로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="7a2f0-215">하지만 예외도 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-215">But there can be exceptions.</span></span> <span data-ttu-id="7a2f0-216">예를 들어 새 인센티브 프로그램의 지급 규칙에 세금 프로필에 대한 추가 정보가 필요할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="7a2f0-217">내 도메인에만 로그인 할 수 있습니다 @onmicrosoft.com .</span><span class="sxs-lookup"><span data-stu-id="7a2f0-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="7a2f0-218">  어떻게 해야 합니까?</span><span class="sxs-lookup"><span data-stu-id="7a2f0-218">What should I do?</span></span>

<span data-ttu-id="7a2f0-219">계정 관리자에게 문의하여 AAD 계정에 도메인을 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="7a2f0-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
