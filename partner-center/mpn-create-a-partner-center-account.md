---
title: 파트너 센터 계정 만들기
ms.topic: article
ms.date: 08/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft 파트너 네트워크 구성원이 파트너 센터 계정을 만들어 네트워크 혜택 및 역량을 관리하는 방법에 대해 알아봅니다.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f94b11c4feb9cd1bedd97bebc537a504f9c4d127
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999357"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="1bb7a-103">파트너 센터 계정을 만들어 네트워크 혜택 및 역량 관리</span><span class="sxs-lookup"><span data-stu-id="1bb7a-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="1bb7a-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="1bb7a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1bb7a-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="1bb7a-105">Global admin</span></span>
- <span data-ttu-id="1bb7a-106">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="1bb7a-106">Admin agent</span></span>

<span data-ttu-id="1bb7a-107">파트너 센터에서 계정을 만들거나 파트너 프로그램에 등록하려면 귀사가 Microsoft 파트너 네트워크의 구성원이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="1bb7a-108">네트워크 구성원이 아닌 경우 [지금 가입](https://partner.microsoft.com/commercial#)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="1bb7a-109">파트너 센터 계정을 만든 후 [대시보드 검색](https://vimeo.com/290338211)이라는 짧은 비디오를 시청하세요.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1bb7a-110">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="1bb7a-110">Before you begin</span></span>

<span data-ttu-id="1bb7a-111">파트너 센터에서 계정을 만들고 Microsoft 파트너 네트워크 멤버십을 갱신하려면 다음 정보를 준비해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-111">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="1bb7a-112">시작하기 전에 다음 항목을 수집하는 데 몇 분 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-112">You may want to take a few minutes to gather these items before you get started:</span></span>

-   <span data-ttu-id="1bb7a-113">전역 관리자는 이메일로 작업합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-113">Global administrator work email.</span></span>

-   <span data-ttu-id="1bb7a-114">회사 계정이 무엇인지 여부가 확실하지 않은 경우 [귀사의 회사 계정 테넌트 및 파트너 센터](azure-active-directory-tenants-and-partner-center.md)를 참조하세요. 회사 계정이 아직 없는 경우 계정 생성 과정에서 회사 계정을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-114">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

-   <span data-ttu-id="1bb7a-115">회사의 법적 회사 이름 및 주소.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-115">Your company's legal business name and address.</span></span>  

-   <span data-ttu-id="1bb7a-116">법적 계약서에 서명할 권한.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-116">Authority to sign legal agreements.</span></span> <span data-ttu-id="1bb7a-117">등록 과정에서 법적 계약서에 서명하는 과정이 나오므로 조직을 대신하여 법적 계약서에 서명할 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-117">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

-   <span data-ttu-id="1bb7a-118">기본 연락처 담당자의 이름 및 회사 이메일.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-118">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="1bb7a-119">귀사의 보안 및 개인 정보 보호를 보장하기 위해 기본 연락처로 이메일을 보내 (1) 기본 연락처 담당자가 파트너 센터 계정에 가입했는지, (2) 이 이메일 주소가 귀사의 이메일 주소가 맞는지 확인할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-119">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="1bb7a-120">기본 연락처 담당자가 자신의 이메일 주소를 확인하면 귀하가 제공한 정보 검토가 계속 진행됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-120">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="1bb7a-121">계정을 만드는 과정에서 이 정보를 확인할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-121">We'll verify this information during the account creation process.</span></span> 
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="1bb7a-122">파트너 센터 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="1bb7a-122">Create a Partner Center account</span></span>

1.  <span data-ttu-id="1bb7a-123">**시작** 페이지의 정보를 검토한 후 **다음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-123">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="1bb7a-124">회사의 회사 계정에 전역 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-124">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="1bb7a-125">회사 계정이 무엇인지 여부가 확실하지 않은 경우 [귀사의 회사 계정 테넌트 및 파트너 센터](azure-active-directory-tenants-and-partner-center.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-125">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="1bb7a-126">조직에 회사 이메일 계정이 있으면 **로그인**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-126">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="1bb7a-127">다음 페이지에서 회사 계정의 전역 관리자 자격 증명을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-127">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="1bb7a-128">조직에 회사 계정이 없으면 **계정 만들기**를 선택하여 회사 계정을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-128">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="1bb7a-129">회사 계정을 만든 후 방금 만든 회사 계정에 글로벌 관리자 자격 증명을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-129">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="1bb7a-130">조직의 법적 회사 프로필 및 기본 연락처 정보를 제공하거나 업데이트한 후 **지금 등록**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-130">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="1bb7a-131">기본 연락처는 애플리케이션과 관련하여 Microsoft 쪽에서 연락을 취할 수 있는 조직 내 사람이어야 합니다(귀하 또는 조직 내 다른 사람도 가능).</span><span class="sxs-lookup"><span data-stu-id="1bb7a-131">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="1bb7a-132">또한 이 정보는 이 사람이 귀하의 조직에서 일하고 있으며 파트너 센터 계정에 등록되었는지 여부를 확인하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-132">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="1bb7a-133">귀사의 보안 및 개인 정보 보호를 보장하기 위해 기본 연락처로 이메일을 보내 (1) 기본 연락처 담당자가 파트너 센터 계정에 가입했는지, (2) 이 이메일 주소가 귀사의 이메일 주소가 맞는지 확인할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-133">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="1bb7a-134">기본 연락처 담당자가 자신의 이메일 주소를 확인하면 귀하가 제공한 정보 검토가 계속 진행됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-134">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="1bb7a-135">Microsoft 파트너 네트워크 계약의 약관을 읽고 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-135">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="1bb7a-136">귀하가 관리 담당자 그룹에 추가되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-136">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="1bb7a-137">다른 사용자 추가를 포함하여 계정 설정을 완료하려면 관리 담당자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-137">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="1bb7a-138">다음 단계에 따라 권한을 보거나 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-138">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="1bb7a-139">a.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-139">a.</span></span> <span data-ttu-id="1bb7a-140">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home**)에서 **설정** 아이콘을 선택한 다음, **사용자 관리**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-140">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="1bb7a-141">b.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-141">b.</span></span> <span data-ttu-id="1bb7a-142">사용자 목록에서 이름을 선택한 다음, 관리 담당자가 선택되지 않았으면 **관리 담당자**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-142">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="1bb7a-143">**업데이트**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-143">Select **Update**.</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="1bb7a-144">MPN 계정 정보 보기</span><span class="sxs-lookup"><span data-stu-id="1bb7a-144">View MPN account details</span></span>

<span data-ttu-id="1bb7a-145">파트너 센터 계정을 만든 후에는 파트너 센터로 돌아와서 다양한 계정 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-145">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="1bb7a-146">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)의 **파트너 프로필** 페이지에 여러 가지 계정 정보가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-146">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="1bb7a-147">이러한 계정 정보는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-147">Such details include:</span></span>

- <span data-ttu-id="1bb7a-148">회사의 법적 비즈니스 프로필</span><span class="sxs-lookup"><span data-stu-id="1bb7a-148">Your company's legal business profile</span></span>

- <span data-ttu-id="1bb7a-149">MPN ID 정보</span><span class="sxs-lookup"><span data-stu-id="1bb7a-149">Information about your MPN ID</span></span>

- <span data-ttu-id="1bb7a-150">등록된 Microsoft 프로그램과 관련된 현재 계약의 링크</span><span class="sxs-lookup"><span data-stu-id="1bb7a-150">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="1bb7a-151">예를 들어 MPN 프로그램에 등록된 경우 현재 Microsoft 파트너 네트워크 계약의 링크가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-151">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="1bb7a-152">CSP(클라우드 솔루션 공급자) 프로그램과 같은 다른 파트너 프로그램에 등록된 경우 Microsoft 파트너 계약과 같은 다른 계약의 링크도 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-152">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="1bb7a-153">이러한 링크는 계약을 검토, 액세스 또는 다운로드하거나 서명된 날짜를 확인하려는 경우에 유용하게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-153">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="1bb7a-154">계정 정보를 보거나 MPN 계약을 살펴보고 다운로드하는 방법</span><span class="sxs-lookup"><span data-stu-id="1bb7a-154">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="1bb7a-155">다음 단계에 따라 계정 정보를 보거나 MPN 계약을 살펴보고 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-155">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="1bb7a-156">회사 계정 사용자 이름 및 암호를 사용하여 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-156">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1bb7a-157">[개요] 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-157">An Overview page appears.</span></span> <span data-ttu-id="1bb7a-158">([개요] 페이지가 표시되지 않는 경우 왼쪽 탐색 메뉴에서 **개요**를 선택합니다.)</span><span class="sxs-lookup"><span data-stu-id="1bb7a-158">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="1bb7a-159">대시보드의 오른쪽 위 모서리에서 기어 아이콘을 선택한 다음, **파트너 설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-159">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings**.</span></span> <span data-ttu-id="1bb7a-160">그러면 [파트너 프로필] 페이지로 이동됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-160">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="1bb7a-161">[파트너 프로필] 페이지에서 여러 영역을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-161">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="1bb7a-162">여기에는 **법적 비즈니스 프로필** 영역과 **프로그램 정보** 영역이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-162">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="1bb7a-163">**프로그램 정보**에서 **MPN 프로그램 상태** 필드를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-163">Under **Program info**, locate the **MPN program status** field.</span></span> <span data-ttu-id="1bb7a-164">그러면 Microsoft 파트너 네트워크 계약의 링크가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-164">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="1bb7a-165">프로그램의 현재 상태에 대한 설명도 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-165">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="파트너 프로필 페이지의 [프로그램 정보] 영역을 보여주는 이미지. 빨간색 상자는 이 영역의 [MPN 프로그램 상태] 필드 및 Microsoft 파트너 네트워크 계약과 관련된 링크를 강조 표시합니다.":::

6. <span data-ttu-id="1bb7a-167">이 계약을 살펴보거나 다운로드하려면 **Microsoft 파트너 네트워크 계약**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-167">To view or download this agreement, select **Microsoft Partner Network agreement**.</span></span>  

> [!NOTE]
> <span data-ttu-id="1bb7a-168">CSP(클라우드 솔루션 공급자) 프로그램에 등록된 경우 위의 단계에 따라 Microsoft 파트너 계약과 같은 등록된 다른 프로그램에 대한 계약을 살펴보거나 다운로드할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bb7a-168">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1bb7a-169">다음 단계</span><span class="sxs-lookup"><span data-stu-id="1bb7a-169">Next steps</span></span>

-   [<span data-ttu-id="1bb7a-170">사용자 추가 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="1bb7a-170">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="1bb7a-171">Microsoft Action Pack 구독 구매 또는 갱신</span><span class="sxs-lookup"><span data-stu-id="1bb7a-171">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="1bb7a-172">Microsoft 파트너 네트워크 멤버십 혜택 관리</span><span class="sxs-lookup"><span data-stu-id="1bb7a-172">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="1bb7a-173">골드 및 실버 멤버십을 위한 역량 요구 사항에 대해 알아보기</span><span class="sxs-lookup"><span data-stu-id="1bb7a-173">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="1bb7a-174">비즈니스 프로필을 만들어 Microsoft에서 잠재 고객 받기</span><span class="sxs-lookup"><span data-stu-id="1bb7a-174">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="1bb7a-175">Microsoft에서 잠재 고객 가져오기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1bb7a-175">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
