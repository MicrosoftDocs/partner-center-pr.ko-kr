---
title: Salesforce CRM 파트너 센터에 대 한 공동 판매 커넥터
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 조회를 Salesforce CRM과 동기화 합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284386"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="b3e95-104">Salesforce CRM용 공동 판매 커넥터 – 개요</span><span class="sxs-lookup"><span data-stu-id="b3e95-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="b3e95-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="b3e95-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b3e95-106">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="b3e95-106">Referrals admin</span></span>
- <span data-ttu-id="b3e95-107">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="b3e95-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b3e95-108">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b3e95-109">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b3e95-110">공동 판매 커넥터를 사용 하 여 Microsoft 판매자를 참여 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 하는 새 공동 판매 참조를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="b3e95-111">이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b3e95-112">파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안 모든 조회 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b3e95-113">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b3e95-114">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="b3e95-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b3e95-115">**토픽**</span><span class="sxs-lookup"><span data-stu-id="b3e95-115">**Topics**</span></span>   |<span data-ttu-id="b3e95-116">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="b3e95-116">**Details**</span></span>   |<span data-ttu-id="b3e95-117">**연결**</span><span class="sxs-lookup"><span data-stu-id="b3e95-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b3e95-118">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="b3e95-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b3e95-119">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-119">You need a valid MPN ID</span></span>|<span data-ttu-id="b3e95-120">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="b3e95-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b3e95-121">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="b3e95-121">Co-sell ready</span></span>|<span data-ttu-id="b3e95-122">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b3e95-123">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="b3e95-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b3e95-124">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="b3e95-124">Partner Center account</span></span>|<span data-ttu-id="b3e95-125">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b3e95-126">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b3e95-127">계정 관리</span><span class="sxs-lookup"><span data-stu-id="b3e95-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b3e95-128">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="b3e95-128">Partner Center user roles</span></span>|<span data-ttu-id="b3e95-129">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b3e95-130">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="b3e95-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b3e95-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b3e95-131">Salesforce CRM</span></span>|<span data-ttu-id="b3e95-132">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b3e95-133">Salesforce CRM에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="b3e95-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="b3e95-134">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="b3e95-134">Power Automate Flow Account</span></span>|<span data-ttu-id="b3e95-135">CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정</span><span class="sxs-lookup"><span data-stu-id="b3e95-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="b3e95-136">사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="b3e95-137">Microsoft 사용자 지정 필드에 대 한 Salesforce 패키지 설치</span><span class="sxs-lookup"><span data-stu-id="b3e95-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="b3e95-138">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 식별 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="b3e95-139">이 경계 파트너 판매자 팀에 게 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="b3e95-140">Salesforce에서 **메모** 를 활성화 하 고 기회 관련 목록에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="b3e95-141">참조</span><span class="sxs-lookup"><span data-stu-id="b3e95-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="b3e95-142">다음 단계를 수행 하 여 **기회 팀** 을 활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="b3e95-143">설치에서 **빠른 찾기** 상자를 사용 하 여 기회 팀 설정을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="b3e95-144">필요에 따라 설정을 정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-144">Define the settings as needed.</span></span>
[<span data-ttu-id="b3e95-145">참조</span><span class="sxs-lookup"><span data-stu-id="b3e95-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="b3e95-146">Salesforce에서 [패키지 설치 관리자](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)를 사용 하 여 사용자 지정 필드 및 개체를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="b3e95-147">이를 사용 하 여 모든 회사에 패키지를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="b3e95-148">Sandbox에를 설치 하는 경우 URL의 초기 부분을 다음으로 바꾸어야 합니다. http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="b3e95-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="b3e95-149">Salesforce에서 **기회** 관련 목록에 Microsoft 솔루션을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="b3e95-150">추가 되 면 **렌치** 아이콘을 선택 하 고 속성을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b3e95-151">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="b3e95-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="b3e95-152">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b3e95-153">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="b3e95-154">솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="b3e95-155">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="b3e95-156">성공할 경우 프로덕션 인스턴스에 대 한 관리 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="b3e95-157">Salesforce CRM에 대 한 파트너 센터 조회 동기화 설치</span><span class="sxs-lookup"><span data-stu-id="b3e95-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="b3e95-158">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b3e95-159">그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b3e95-160">오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="b3e95-161">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b3e95-162">상단 메뉴에서 **AppSource 열기** 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. <span data-ttu-id="b3e95-164">팝업 화면에서 **Salesforce에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="b3e95-166">**지금 가져오기** 단추를 선택 하 고 **계속** 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="b3e95-167">그러면 Salesforce CRM 환경을 선택 하 여 응용 프로그램을 설치할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="b3e95-168">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="사용 가능한 CRMS":::

8. <span data-ttu-id="b3e95-170">그런 다음 **솔루션 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="b3e95-171">페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="b3e95-172">파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="b3e95-173">설치는 10-15 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="b3e95-174">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b3e95-175">**Salesforce에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b3e95-176">**Salesforce에 대 한 파트너 센터 조회 동기화를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="b3e95-177">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 흐름":::



## <a name="configure-the-solution"></a><span data-ttu-id="b3e95-179">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="b3e95-179">Configure the solution</span></span>

1. <span data-ttu-id="b3e95-180">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="b3e95-181">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="b3e95-182">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="b3e95-183">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="b3e95-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="b3e95-184">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="b3e95-184">Partner Center Events</span></span>
    - <span data-ttu-id="b3e95-185">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="b3e95-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="b3e95-186">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="b3e95-187">**연결 만들기** 를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="연결 만들기":::

- <span data-ttu-id="b3e95-189">오른쪽 위 모서리의 검색 창에서 파트너 센터 조회 (미리 보기)를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="b3e95-190">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="b3e95-191">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="b3e95-192">CRM 관리자 사용자에 대 한 Salesforce에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="b3e95-193">모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="연결 관찰":::

### <a name="edit-the-connections"></a><span data-ttu-id="b3e95-195">연결 편집</span><span class="sxs-lookup"><span data-stu-id="b3e95-195">Edit the connections</span></span>

1. <span data-ttu-id="b3e95-196">솔루션 페이지로 돌아가서 **기본 솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="b3e95-197">**모두** 를 클릭 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="커넥터 편집 시작":::

2. <span data-ttu-id="b3e95-199">세 개의 점 아이콘을 선택 하 여 각 연결을 개별적으로 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="b3e95-200">관련 연결을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="커넥터 편집":::

3. <span data-ttu-id="b3e95-202">다음 순서로 흐름을 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="b3e95-203">파트너 센터 Webhook 등록 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b3e95-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="b3e95-204">공동 판매 참조-Salesforce를 파트너 센터 (Insider Preview)에 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b3e95-205">파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="b3e95-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b3e95-206">파트너 센터를 Salesforce로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b3e95-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b3e95-207">Salesforce에서 파트너 센터로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b3e95-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b3e95-208">Salesforce 기회와 파트너 센터 간 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b3e95-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b3e95-209">파트너 센터 (Insider Preview)에 대 한 Salesforce Microsoft 솔루션</span><span class="sxs-lookup"><span data-stu-id="b3e95-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b3e95-210">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="b3e95-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b3e95-211">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b3e95-212">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b3e95-213">Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b3e95-214">아래 강조 표시 된 대로 조회 관리자 자격 증명 (b.) 파트너 센터 이벤트를 사용 하 여 (a.) 파트너 센터 사용자에 대 한 연결을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="트리거":::

3. <span data-ttu-id="b3e95-216">이러한 업데이트를 만들면 다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="b3e95-218">변경 내용을 저장 하 고 **켜기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="b3e95-219">파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="b3e95-220">**파트너 센터에서 SALESFORCE CRM (Insider preview)을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="b3e95-221">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b3e95-222">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 복사":::

8. <span data-ttu-id="b3e95-224">이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b3e95-225">오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="b3e95-226">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-226">Enter the following details:</span></span>

    1. <span data-ttu-id="b3e95-227">**Http 트리거 끝점**: 이전 단계에서 복사한 URL</span><span class="sxs-lookup"><span data-stu-id="b3e95-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="b3e95-228">**등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"</span><span class="sxs-lookup"><span data-stu-id="b3e95-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="b3e95-229">**기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)</span><span class="sxs-lookup"><span data-stu-id="b3e95-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="b3e95-230">**실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="b3e95-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b3e95-231">이제 웹 후크를 수신 대기 하 여 이벤트를 만들고 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b3e95-232">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="b3e95-232">Customize synchronization steps</span></span>

<span data-ttu-id="b3e95-233">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b3e95-234">CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b3e95-235">전원 자동화 흐름을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b3e95-236">필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b3e95-237">CRM에 대 한 Microsoft 파트너 센터 매핑이 제공 되지만 CRM 환경에 따라 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b3e95-238">각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b3e95-239">사용 가능한 사용자 지정의 예는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b3e95-240">파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="b3e95-241">파트너 센터에서 Salesforce CRM (Insider Preview)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="b3e95-242">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="b3e95-243">선택 **(범위) 잠재 고객 또는 기회를 동기화** 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b3e95-244">이벤트 만들기에 대 한 CRM 필드 매핑을 사용자 지정 하려면 **새 공유 기회 인지 여부** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b3e95-245">**예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기** 를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b3e95-246">필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="b3e95-247">업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 "(범위) 리드 또는 기회 동기화" 단계를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="b3e95-248">**기회를 업데이트 하는 경우를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b3e95-249">**예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를** 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="b3e95-250">**예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="b3e95-251">업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:</span><span class="sxs-lookup"><span data-stu-id="b3e95-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="b3e95-252">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b3e95-253">**기회 동기화를 선택 (범위)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="b3e95-254">업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="b3e95-255">**예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트** 단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="b3e95-256">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b3e95-257">만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면</span><span class="sxs-lookup"><span data-stu-id="b3e95-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="b3e95-258">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b3e95-259">**조회 동기화를 선택 (범위) 합니다.**</span><span class="sxs-lookup"><span data-stu-id="b3e95-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="b3e95-260">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="b3e95-261">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b3e95-262">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="b3e95-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b3e95-263">전원 자동화 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b3e95-264">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="b3e95-264">Pre-requisites</span></span>

<span data-ttu-id="b3e95-265">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b3e95-266">이 id는 판매자 팀에 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b3e95-267">사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="b3e95-268">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b3e95-269">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b3e95-270">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="b3e95-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b3e95-271">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="b3e95-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b3e95-272">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="b3e95-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b3e95-273">Microsoft의 도움을 주는 **방법**: microsoft에서 조회에 필요한 도움말</span><span class="sxs-lookup"><span data-stu-id="b3e95-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b3e95-274">**제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="b3e95-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b3e95-275">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="b3e95-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="b3e95-276">에서는</span><span class="sxs-lookup"><span data-stu-id="b3e95-276">SCENARIOS:</span></span>

1. <span data-ttu-id="b3e95-277">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="b3e95-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="b3e95-278">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 Salesforce crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="b3e95-279">Salesforce CRM 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 환경":::

   3. <span data-ttu-id="b3e95-281">이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="b3e95-282">"파트너 센터와 동기화": 예</span><span class="sxs-lookup"><span data-stu-id="b3e95-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="b3e95-283">"Microsoft의 도움을 주는 방법": 다음 옵션 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="b3e95-284">제품: 제품의 솔루션 Id</span><span class="sxs-lookup"><span data-stu-id="b3e95-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="b3e95-285">**파트너 센터와의 동기화 기회 센터** 옵션을 **예** 로 설정 했으면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b3e95-286">조회가 Salesforce CRM과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="b3e95-287">"파트너 센터와 동기화" 옵션이 "예"로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="b3e95-288">파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="b3e95-289">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="b3e95-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="b3e95-290">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="b3e95-291">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="b3e95-292">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="b3e95-293">Salesforce CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="b3e95-294">**오픈 기회** 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b3e95-295">Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 기회 화면":::

    6. <span data-ttu-id="b3e95-297">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="b3e95-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b3e95-298">다음 단계</span><span class="sxs-lookup"><span data-stu-id="b3e95-298">Next steps</span></span>

- [<span data-ttu-id="b3e95-299">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="b3e95-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b3e95-300">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="b3e95-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b3e95-301">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="b3e95-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
