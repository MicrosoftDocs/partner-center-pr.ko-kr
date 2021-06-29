---
title: Salesforce CRM 파트너 센터에 대 한 공동 판매 커넥터
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 조회를 Salesforce CRM과 동기화 합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029127"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="707f6-104">Salesforce CRM용 공동 판매 커넥터 – 개요</span><span class="sxs-lookup"><span data-stu-id="707f6-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="707f6-105">**적절 한 역할**: 조회 관리자 | CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="707f6-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="707f6-106">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="707f6-107">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-107">They won't have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="707f6-108">공동 판매 커넥터를 사용 하 여 Microsoft 판매자를 참여 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 하는 새 공동 판매 참조를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="707f6-109">이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="707f6-110">파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안 모든 조회 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="707f6-111">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="707f6-112">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="707f6-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="707f6-113">**토픽**</span><span class="sxs-lookup"><span data-stu-id="707f6-113">**Topics**</span></span>|<span data-ttu-id="707f6-114">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="707f6-114">**Details**</span></span>|<span data-ttu-id="707f6-115">**연결**</span><span class="sxs-lookup"><span data-stu-id="707f6-115">**Links**</span></span>|
|--------------|--------------------|------|
|<span data-ttu-id="707f6-116">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="707f6-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="707f6-117">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-117">You need a valid MPN ID</span></span>|<span data-ttu-id="707f6-118">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="707f6-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="707f6-119">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="707f6-119">Co-sell ready</span></span>|<span data-ttu-id="707f6-120">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="707f6-121">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="707f6-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="707f6-122">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="707f6-122">Partner Center account</span></span>|<span data-ttu-id="707f6-123">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="707f6-124">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="707f6-125">계정 관리</span><span class="sxs-lookup"><span data-stu-id="707f6-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="707f6-126">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="707f6-126">Partner Center user roles</span></span>|<span data-ttu-id="707f6-127">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="707f6-128">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="707f6-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="707f6-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="707f6-129">Salesforce CRM</span></span>|<span data-ttu-id="707f6-130">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="707f6-131">Salesforce CRM에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="707f6-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="707f6-132">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="707f6-132">Power Automate Flow Account</span></span>|<span data-ttu-id="707f6-133">테스트, 준비 및 프로덕션을 위해 데이터베이스를 사용 하 여 새 프로덕션 환경을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-133">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="707f6-134">데이터베이스를 사용 하는 기존 프로덕션 환경이 있는 경우 다시 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-134">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="707f6-135">커넥터 솔루션을 설치 하려는 사용자에 게는 전원 자동화 라이선스와이 환경에 대 한 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-135">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="707f6-136">설치에 실패 하는 경우 진행 상황을 모니터링 하 고 [전원 자동화](https://flow.microsoft.com/) 에서 자세한 정보를 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-136">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="707f6-137">**솔루션** 에서 **기록 보기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-137">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="707f6-138">환경 만들기 또는 관리</span><span class="sxs-lookup"><span data-stu-id="707f6-138">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="707f6-139">Microsoft 사용자 지정 필드에 대 한 Salesforce 패키지 설치</span><span class="sxs-lookup"><span data-stu-id="707f6-139">Installation of Salesforce Package for Microsoft Custom Fields</span></span>

<span data-ttu-id="707f6-140">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 식별 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-140">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="707f6-141">이 경계 파트너 판매자 팀에 게 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-141">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="707f6-142">Salesforce에서 **메모** 를 활성화 하 고 기회 관련 목록에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-142">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> [<span data-ttu-id="707f6-143">참조</span><span class="sxs-lookup"><span data-stu-id="707f6-143">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. <span data-ttu-id="707f6-144">다음 단계를 수행 하 여 **기회 팀** 을 활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-144">Activate **Opportunity teams** by following the steps:</span></span>
    - <span data-ttu-id="707f6-145">설치에서 **빠른 찾기** 상자를 사용 하 여 기회 팀 설정을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-145">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="707f6-146">필요에 따라 설정을 정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-146">Define the settings as needed.</span></span> [<span data-ttu-id="707f6-147">참조</span><span class="sxs-lookup"><span data-stu-id="707f6-147">Reference</span></span>](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. <span data-ttu-id="707f6-148">Salesforce에서 [패키지 설치 관리자](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)를 사용 하 여 사용자 지정 필드 및 개체를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-148">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="707f6-149">이 설치 관리자를 사용 하 여 모든 회사에 패키지를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-149">Use this installer to install the package into any company.</span></span>

    >[!NOTE]
    ><span data-ttu-id="707f6-150">Sandbox에를 설치 하는 경우 URL의 초기 부분을로 바꾸어야 합니다 `http://test.salesforce.com` .</span><span class="sxs-lookup"><span data-stu-id="707f6-150">If you are installing into a sandbox, you must replace the initial portion of the URL with `http://test.salesforce.com`.</span></span>

1. <span data-ttu-id="707f6-151">Salesforce에서 **기회** 관련 목록에 Microsoft 솔루션을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-151">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="707f6-152">추가 되 면 **렌치** 아이콘을 선택 하 고 속성을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-152">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="707f6-153">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="707f6-153">Best Practice: Test before you go live</span></span>

<span data-ttu-id="707f6-154">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-154">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="707f6-155">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-155">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="707f6-156">솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-156">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="707f6-157">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-157">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="707f6-158">성공할 경우 프로덕션 인스턴스에 대 한 관리 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-158">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="707f6-159">Salesforce CRM에 대 한 파트너 센터 조회 동기화 설치</span><span class="sxs-lookup"><span data-stu-id="707f6-159">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="707f6-160">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-160">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="707f6-161">그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-161">This will show you the available CRM instances.</span></span>

1. <span data-ttu-id="707f6-162">오른쪽 위 모서리의 드롭다운 목록에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-162">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="707f6-163">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-163">Select **Solutions** on the left navigation bar.</span></span>

1. <span data-ttu-id="707f6-164">상단 메뉴에서 **AppSource 열기** 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-164">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="AppSource 열기":::

1. <span data-ttu-id="707f6-166">팝업 화면에서 **Salesforce에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-166">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="지금 가져오기의 스크린샷":::

1. <span data-ttu-id="707f6-168">**지금 가져오기** 단추를 선택한 다음 **계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-168">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="707f6-169">다음 페이지에서 Salesforce CRM 환경을 선택 하 여 응용 프로그램을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-169">In the next page, select the Salesforce CRM environment to install the application.</span></span> <span data-ttu-id="707f6-170">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-170">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="707f6-171">그런 다음 **솔루션 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-171">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="707f6-172">페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-172">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="707f6-173">파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-173">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="707f6-174">설치는 10-15 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-174">Installation will take 10-15 minutes.</span></span>

1. <span data-ttu-id="707f6-175">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-175">After the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="707f6-176">이제 솔루션 목록에서 **Salesforce에 대 한 파트너 센터 조회 동기화** 를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-176">Notice that **Partner Center Referrals Synchronization for Salesforce** is now available in the Solutions list.</span></span>

1. <span data-ttu-id="707f6-177">**Salesforce에 대 한 파트너 센터 조회 동기화를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-177">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="707f6-178">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-178">The following Power Automate flows and entities are available:</span></span>

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce 흐름":::

## <a name="configure-the-solution"></a><span data-ttu-id="707f6-180">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="707f6-180">Configure the solution</span></span>

1. <span data-ttu-id="707f6-181">CRM 인스턴스에 솔루션을 설치한 후 다시 [전원 자동화](https://flow.microsoft.com/)로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-181">After you've installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="707f6-182">오른쪽 위 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-182">From the **Environments** drop-down in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="707f6-183">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-183">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="707f6-184">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="707f6-184">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="707f6-185">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="707f6-185">Partner Center Events</span></span>
   - <span data-ttu-id="707f6-186">솔루션의 전원 자동화 흐름을 사용 하는 CRM 관리자</span><span class="sxs-lookup"><span data-stu-id="707f6-186">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="707f6-187">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 **파트너 센터 조회** 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-187">Select **Connections** from the left navigation bar, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="707f6-188">**연결 만들기** 를 선택 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-188">Create a connection by selecting **Create a connection**.</span></span>

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="연결 만들기를 보여 주는 스크린샷":::

   1. <span data-ttu-id="707f6-190">오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-190">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="707f6-191">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-191">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="707f6-192">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-192">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   1. <span data-ttu-id="707f6-193">CRM 관리자 사용자에 대 한 Salesforce에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-193">Create a connection for Salesforce for the CRM administrator user.</span></span>
  
   1. <span data-ttu-id="707f6-194">CRM 관리자 사용자에 대 한 Microsoft Dataverse의 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-194">Create a connection for Microsoft Dataverse for the CRM administrator user.</span></span>

   1. <span data-ttu-id="707f6-195">모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-195">After you've added all the Connections, you should see the following connections in your environment:</span></span>

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="연결을 관찰 하는 방법을 보여 주는 스크린샷":::

### <a name="edit-the-connections"></a><span data-ttu-id="707f6-197">연결 편집</span><span class="sxs-lookup"><span data-stu-id="707f6-197">Edit the connections</span></span>

1. <span data-ttu-id="707f6-198">**솔루션** 페이지로 돌아가서 **기본 솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-198">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="707f6-199">**모두** 를 클릭 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-199">Select **Connection Reference (preview)** by clicking **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="연결 편집을 보여 주는 스크린샷":::

1. <span data-ttu-id="707f6-201">각 연결은 말줄임표 아이콘을 선택하여 개별적으로 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-201">Edit each of the Connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="707f6-202">관련 연결을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-202">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="스크린샷 atht는 커넥터를 편집하는 방법을 보여줍니다.":::

1. <span data-ttu-id="707f6-204">다음 순서로 흐름을 켭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-204">Turn on the flows in the following sequence:</span></span>
   - <span data-ttu-id="707f6-205">파트너 센터 Webhook 등록(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-205">Partner Center Webhook Registration (Insider Preview)</span></span>
   - <span data-ttu-id="707f6-206">[사용자 지정] Salesforce에서 세부 정보 만들기 또는 얻기</span><span class="sxs-lookup"><span data-stu-id="707f6-206">[Customize] Create or Get Details from Salesforce</span></span>
   - <span data-ttu-id="707f6-207">파트너 센터 공동 판매 Referral-Salesforce 만들기(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-207">Create Co-sell Referral-Salesforce to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="707f6-208">Salesforce에 대한 Microsoft 공동 판매 조회 업데이트 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-208">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>  
   - <span data-ttu-id="707f6-209">Salesforce에 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-209">Partner Center to Salesforce (Insider Preview)</span></span>
   - <span data-ttu-id="707f6-210">Salesforce에서 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-210">Salesforce to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="707f6-211">Salesforce 파트너 센터 기회(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-211">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="707f6-212">파트너 센터 Salesforce Microsoft 솔루션(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="707f6-212">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="707f6-213">Webhook API를 사용하여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="707f6-213">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="707f6-214">파트너 센터 webhook API를 사용하여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-214">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="707f6-215">이러한 변경 이벤트는 URL에 HTTP 게시물로 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-215">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="707f6-216">**Salesforce CRM에 파트너 센터(Insider Preview)** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-216">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

1. <span data-ttu-id="707f6-217">편집 **아이콘을** 선택하고 **HTTP 요청을 받은 경우를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-217">Select the **Edit icon** and select **When an HTTP request is received**.</span></span>

1. <span data-ttu-id="707f6-218">**복사** 아이콘을 선택하여 제공된 **HTTP POST URL** 를 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-218">Select the **Copy** icon to copy the provided **HTTP POST URL**.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL을 복사하는 방법을 보여 주는 스크린샷":::

1. <span data-ttu-id="707f6-220">파트너 센터 **Webhook 등록(Insider Preview)** Power Automate 흐름을 선택한 다음, **실행을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-220">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="707f6-221">오른쪽 창에서 **실행 흐름** 창이 열리는지 확인하고 **계속을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-221">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="707f6-222">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-222">Enter the following details:</span></span>

   - <span data-ttu-id="707f6-223">**Http 트리거 엔드포인트:** 이 URL은 이전 단계에서 복사되었습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-223">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="707f6-224">**등록할 이벤트:** 사용 가능한 **이벤트(조회 생성, 조회** **업데이트,** 관련 조회 생성 및 **related-referral-updated)를** Select all. </span><span class="sxs-lookup"><span data-stu-id="707f6-224">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="707f6-225">**있는 경우 기존 트리거 엔드포인트를 덮어쓰시겠습니까?**: 예.</span><span class="sxs-lookup"><span data-stu-id="707f6-225">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="707f6-226">지정된 웹후크 이벤트에 대해 하나의 URL만 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-226">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="707f6-227">**흐름 실행을** 선택한 **다음, 완료를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-227">Select **Run flow**, and then select **Done**.</span></span>

<span data-ttu-id="707f6-228">이제 webhook는 이벤트를 수신 대기, 생성 및 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-228">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="707f6-229">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="707f6-229">Customize synchronization steps</span></span>

<span data-ttu-id="707f6-230">CRM 시스템은 고도로 사용자 지정되며 CRM 설정에 따라 Power Automate 솔루션을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-230">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="707f6-231">파트너 센터 CRM 시스템 간에 공동 판매 조회가 동기화되면 파트너 센터 PC에서 동기화되는 [필드가 사용자 지정 필드 매핑 가이드에](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-231">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="707f6-232">필드 매핑 가이드에 따라 필요한 경우 Salesforce 또는 환경 **변수에서 [사용자 지정] 만들기 또는 세부 정보 얻기를** 적절하게 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-232">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Salesforce** or environment variables.</span></span> <span data-ttu-id="707f6-233">향후 솔루션 업그레이드에 영향을 줄 수 있으므로 Power Automate 솔루션의 다른 흐름을 업데이트하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="707f6-233">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="707f6-234">다음 사용자 지정을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-234">The following customizations are available:</span></span>

- <span data-ttu-id="707f6-235">**영업 기회 이름에 확인 표시** 표시: 기본적으로 영업 기회 이름 옆에 확인 표시가 표시되어 파트너 센터 및 Salesforce CRM 간의 동기화가 성공적으로 수행되고 있음을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-235">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Salesforce CRM is happening successfully.</span></span> <span data-ttu-id="707f6-236">마찬가지로 동기화에 실패하면 교차 표시가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-236">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="707f6-237">기회 이름에 확인 표시 또는 교차 표시를 추가하지 않으려면 기회 이름 환경 **변수에서 표시 확인 표시의** 현재 값을 아니요로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-237">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>

- <span data-ttu-id="707f6-238">**스테이지 이름:**</span><span class="sxs-lookup"><span data-stu-id="707f6-238">**Stage name**:</span></span>

  - <span data-ttu-id="707f6-239">**활성 스테이지 이름:** Salesforce에서 영업 기회의 영업 파이프라인에 있는 단계입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-239">**Active stage name**: This is the stage in an opportunity's sales pipeline in Salesforce.</span></span>  <span data-ttu-id="707f6-240">활성 스테이지를 나타내며 파트너 센터 허용된 상태의 조회와 동일합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-240">It represents an active stage and is equivalent to a referral in accepted state in Partner Center.</span></span> <span data-ttu-id="707f6-241">보류 중 단계 이후 판매 파이프라인의 다음 단계가 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-241">This can be the next stage in the sales pipeline after the on-hold stage.</span></span> <span data-ttu-id="707f6-242">영업 기회의 판매 스테이지를 활성 스테이지에서 활성 스테이지로 이동하면 파트너 센터 조회가 수락되고 변경 내용이 동기화를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-242">Moving Opportunity's sales stage out of the on-hold stage into active stage will accept the referral in Partner Center and changes will start synchronizing.</span></span>

  - <span data-ttu-id="707f6-243">**보류 중 스테이지 이름:** Salesforce에서 영업 기회의 판매 파이프라인에 있는 스테이지의 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-243">**On-hold stage name**: Name of the stage in an opportunity's sales pipeline in Salesforce.</span></span> <span data-ttu-id="707f6-244">보류 중 단계를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-244">It represents an on-hold stage.</span></span> <span data-ttu-id="707f6-245">아직 수락되지 않은 Microsoft에서 공유한 새로운 공동 판매 추천은 Salesforce에서 이 단계로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-245">New co-sell referrals shared from Microsoft that are not yet accepted will be set to this stage in Salesforce.</span></span> <span data-ttu-id="707f6-246">보류 중인 단계에서 기회에서 변경된 내용은 파트너 센터 동기화되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-246">Any changes made in an opportunity while it is on-hold stage will not synchronize to Partner Center.</span></span> <span data-ttu-id="707f6-247">이 보류 중 단계에서 기회의 판매 스테이지를 이동하면 파트너 센터 조회가 수락되고 변경 내용이 동기화를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-247">Moving Opportunity's sales stage out of this on-hold stage will accept the referral in Partner Center and changes will start synchronizing.</span></span>

- <span data-ttu-id="707f6-248">**고객 계정 국가 코드:** 새 조회를 만들 때 두 문자로 된 국가 코드(ISO 3166)를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-248">**Customer Account Country Code**: It is mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="707f6-249">기본적으로 국가 코드는 Salesforce의 계정 **BillingCountry** 필드와 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-249">By default, the country code will be synced to and from the account's **BillingCountry** field in Salesforce.</span></span> <span data-ttu-id="707f6-250">Salesforce에 동기화할 국가 코드에 대한 다른 필드가 있는 경우:</span><span class="sxs-lookup"><span data-stu-id="707f6-250">If you have a different field in Salesforce for the country code to sync from:</span></span>

  - <span data-ttu-id="707f6-251">두 문자로 된 코드가 포함된 계정의 비후크업 국가 코드 필드의 경우:</span><span class="sxs-lookup"><span data-stu-id="707f6-251">For a nonlookup country code field in the account that contains a two-letter code:</span></span>

    - <span data-ttu-id="707f6-252">Salesforce 환경 변수의 **고객 계정 국가 코드** 필드 이름을 CRM의 필드 이름으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-252">Update the **Customer Account Country Code** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="707f6-253">표시 이름이 아닌 필드 이름을 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-253">Make sure that you provide the field's name, not its display name.</span></span>

    - <span data-ttu-id="707f6-254">**[사용자 지정] Salesforce에서 세부 정보 만들기 또는 받기를** 편집하고 **CRM에서 고객 계정 만들기 또는 받기 작업으로 이동하여 CRM의** 올바른 필드에 **국가** 값을 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-254">Edit **[Customize] Create or Get Details from Salesforce**, and go to **Create or get customer account in CRM** action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="707f6-255">또한 BillingCountry 에서 **국가** 값 **할당을 제거합니다.**</span><span class="sxs-lookup"><span data-stu-id="707f6-255">Also, remove the **Country** value assignment from the **BillingCountry**.</span></span>

  - <span data-ttu-id="707f6-256">계정의 조회 기반 국가 코드 필드의 경우:</span><span class="sxs-lookup"><span data-stu-id="707f6-256">For a lookup-based country code field in the account:</span></span>

    - <span data-ttu-id="707f6-257">계정에 새 사용자 지정 필드를 추가하고 조회 기반 필드에서 선택한 값에 따라 두 문자로 된 국가 코드(ISO 3166)로 자동으로 채우며 그 반대의 경우도 마찬가지입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-257">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>

    - <span data-ttu-id="707f6-258">비후크업 국가 코드 필드에 대한 이전 단계에 따라 CRM에서 파트너 센터 새 사용자 지정 필드를 동기화합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-258">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="707f6-259">**거래 값:** 기본적으로 파트너 센터 거래 값은 CRM의 **Amount와** 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-259">**Deal value**: By default, the deal value from Partner Center will be synchronized to and from **Amount** in the CRM.</span></span> <span data-ttu-id="707f6-260">CRM에 동기화할 거래 값에 대한 다른 필드가 있는 경우:</span><span class="sxs-lookup"><span data-stu-id="707f6-260">If you have a different field in the CRM for the deal value to synchronize from:</span></span>

  - <span data-ttu-id="707f6-261">Salesforce 환경 변수의 **Deal 값** 필드 이름을 CRM의 필드 이름으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-261">Update the **Deal value** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="707f6-262">표시 이름이 아닌 필드 이름을 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-262">Make sure that you provide the field's name, not its display name.</span></span>

  - <span data-ttu-id="707f6-263">[사용자 **지정] Salesforce에서 세부 정보 만들기 또는 받기를** 편집하고 CRM에서 **기회 만들기 또는 업데이트로** 이동하고 **새 기회 만들기** 및 **기존 기회** 업데이트 작업을 모두 업데이트하여 **DealValue를** Salesforce의 올바른 필드에 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-263">Edit **[Customize] Create or Get Details from Salesforce** and go to **Create or update opportunity** in CRM and update both **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** to the correct field in Salesforce.</span></span>

- <span data-ttu-id="707f6-264">**거래 값 통화 코드:** Salesforce의 거래 값 통화 코드 필드 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-264">**Deal value currency code**: Name of the deal value currency code field in Salesforce.</span></span> <span data-ttu-id="707f6-265">이 필드 API 이름은 Microsoft 파트너 센터 조회를 만들거나 업데이트할 때 기회의 거래 가치 통화 코드를 얻는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-265">This field API name will be used to get Opportunity's deal value currency code when creating or updating referral in Microsoft Partner Center.</span></span> <span data-ttu-id="707f6-266">거래 값 통화 코드 필드가 기본 필드 **CurrencyIsoCode와** 다른 경우 이 환경 변수의 현재 값을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-266">If deal value currency code field is different than default field **CurrencyIsoCode**, update the current value of this environment variable.</span></span>

  - <span data-ttu-id="707f6-267">Salesforce 환경 변수의 **거래 값 통화** 필드 이름을 CRM의 필드 이름으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-267">Update the **Deal value currency** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="707f6-268">표시 이름이 아닌 필드 이름을 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-268">Make sure that you provide the field's name, not its display name.</span></span>

  - <span data-ttu-id="707f6-269">**[사용자 지정] Salesforce에서 세부 정보 만들기 또는 받기를** 편집하고 CRM에서 **기회 만들기 또는 업데이트로** 이동하고 **새 기회 만들기** 및 **기존 기회** 업데이트 작업을 모두 업데이트하여 **DealValueCurrency를** Salesforce의 올바른 필드에 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-269">Edit **[Customize] Create or Get Details from Salesforce** and go to **Create or update opportunity** in CRM and update both **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValueCurrency** to the correct field in Salesforce.</span></span>

- <span data-ttu-id="707f6-270">**공동 판매 기회 동기화:** **예로** 설정하면 공동 판매 및 파이프라인 공유 기회만 파트너 센터 Salesforce로 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-270">**Sync Co-sell opportunity**: If set to **yes**, only co-sell and pipeline sharing opportunities will be synchronized from Partner Center to Salesforce.</span></span> <span data-ttu-id="707f6-271">**아니요로** 설정하면 잠재 고객, 공동 판매 및 파이프라인 공유 기회가 파트너 센터 Salesforce로 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-271">If set to **no**, leads, co-sell, and pipeline sharing opportunities will be synchronized from Partner Center to Salesforce.</span></span> <span data-ttu-id="707f6-272">이 변수는 Salesforce에서 파트너 센터 동기화되는 기회에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-272">This variable does not have any impact on the opportunities synchronized from Salesforce to Partner Center.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="707f6-273">환경 변수 업데이트</span><span class="sxs-lookup"><span data-stu-id="707f6-273">Update environment variable</span></span>

<span data-ttu-id="707f6-274">환경 변수 값을 업데이트하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-274">To update an environment variable value:</span></span>

1. <span data-ttu-id="707f6-275">**솔루션** 페이지로 이동하여 기본 **솔루션** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-275">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="707f6-276">**모두** 를 선택하여 **환경 변수를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-276">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="707f6-277">업데이트해야 하는 값에 대한 환경 변수를 선택하고, 말줄임표 아이콘을 사용하여 **편집을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-277">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="707f6-278">새 값 옵션을 사용하고 값을 제공하여 **현재** 값을 업데이트합니다(기본값은 업데이트하지 마세요).  </span><span class="sxs-lookup"><span data-stu-id="707f6-278">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="707f6-279">값은 변수의 데이터 형식과 일치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-279">The value must match the data type of the variable.</span></span> <span data-ttu-id="707f6-280">예를 들어 예 또는 아니요 데이터 형식은 예 또는 아니요 값을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-280">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="환경 변수 업데이트를 보여 주는 스크린샷":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="707f6-282">엔드투엔드 양방향 공동 판매 조회 동기화</span><span class="sxs-lookup"><span data-stu-id="707f6-282">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="707f6-283">Power Automate 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간의 공동 판매 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-283">After you've installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="707f6-284">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="707f6-284">Pre-requisites</span></span>

<span data-ttu-id="707f6-285">파트너 센터 및 Salesforce CRM에서 조회를 동기화하려면 Power Automate 솔루션이 Microsoft 특정 조회 필드를 명확하게 구분해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-285">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="707f6-286">이 ID를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-286">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="707f6-287">사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-287">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="707f6-288">CRM 관리자 사용자는 **기회** 사용자 지정 필드를 사용하여 별도의 CRM 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-288">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="707f6-289">다음 사용자 지정 필드는 CRM 섹션의 일부여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-289">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="707f6-290">**파트너 센터 동기화:** 영업 기회를 파트너 센터 동기화할지 여부를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-290">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="707f6-291">기본적으로 이 필드의 값은 아니요이며 판매자가 Microsoft와 기회를 공유하려면 명시적으로 예 로 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-291">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="707f6-292">파트너 센터 CRM으로 공유된 새 조회에는 이 필드 값이 Yes로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-292">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="707f6-293">**조회 식별자:** Microsoft 파트너 센터 조회에 대한 읽기 전용 식별자 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-293">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral.</span></span>

- <span data-ttu-id="707f6-294">**조회 링크:** Microsoft 파트너 센터 조회에 대한 읽기 전용 링크입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-294">**Referral Link**: A read-only link to the referral in Microsoft Partner Center.</span></span>

- <span data-ttu-id="707f6-295">**Microsoft 도움말:** 추천을 위해 Microsoft에서 필요한 도움말입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-295">**How can Microsoft help**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="707f6-296">공동 판매 추천을 만들려면 Microsoft에서 필요한 적절한 도움말을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-296">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="707f6-297">고객 연락처는 공동 판매 추천을 만들 수 있는 기회와 연결되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-297">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="707f6-298">공동 판매가 아닌 추천을 만들려면 이 필드를 선택하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="707f6-298">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="707f6-299">언제든지 적절한 도움말 필수 옵션을 선택하여 공동 판매가 아닌 추천을 공동 판매 추천으로 변환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-299">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>

- <span data-ttu-id="707f6-300">**Microsoft 파트너 센터 조회 표시 유형:** 파트너 센터 조회에 대한 표시 유형 선택</span><span class="sxs-lookup"><span data-stu-id="707f6-300">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="707f6-301">Microsoft 판매자에 게 표시 하면 비 공동 판매 조회가 공동 판매로 전환 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-301">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="707f6-302">Microsoft 도움말이 필요한 경우 기본적으로 Microsoft 판매자에 게 조회를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-302">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="707f6-303">이 필드가 표시 된 것으로 표시 된 후에는 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-303">After this field is marked as visible, it can't be reverted.</span></span>

- <span data-ttu-id="707f6-304">**MICROSOFT CRM identifier**: 공동 판매 조회가 microsoft에서 만들어지고 수락 되는 경우이 필드는 MICROSOFT의 CRM 식별자로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-304">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>

- <span data-ttu-id="707f6-305">**Microsoft 파트너 센터 솔루션**: 공동 판매 준비 된 솔루션 또는 Microsoft 솔루션을 기회와 연결 하는 사용자 지정 개체입니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-305">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="707f6-306">하나 이상의 솔루션을 기회에서 추가 하거나 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-306">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="707f6-307">Microsoft와 공유 하기 전에 하나 이상의 공동 판매 준비 또는 Microsoft 솔루션을 기회에 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-307">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="707f6-308">이 개체를 기회에 연결 하려면 CRM에서 **기회** 양식을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-308">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

- <span data-ttu-id="707f6-309">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="707f6-309">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="707f6-310">에서는</span><span class="sxs-lookup"><span data-stu-id="707f6-310">SCENARIOS</span></span>

1. <span data-ttu-id="707f6-311">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="707f6-311">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="707f6-312">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 Salesforce crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-312">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="707f6-313">**Microsoft Partner Center** 섹션은 Salesforce CRM 환경에서 **새 기회** 를 만들 때 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-313">Ensure that the section, **Microsoft Partner Center** is present when you create a **New Opportunity** in Salesforce CRM environment.</span></span>

   1. <span data-ttu-id="707f6-314">파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔ icon in Salesforce CRM.</span></span>
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce 환경의 스크린샷":::

   1. <span data-ttu-id="707f6-316">이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-316">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="707f6-317">**Microsoft에서 어떻게 도울 수 있나요?**: 공동 판매 조회를 만들려면 적절 한 도움말 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-317">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="카드 보기에서 적절 한 필드를 가져오는 방법을 보여 주는 스크린샷":::

      - <span data-ttu-id="707f6-319">**파트너 센터와 동기화**: 예</span><span class="sxs-lookup"><span data-stu-id="707f6-319">**Sync with Partner Center**: Yes</span></span>
      - <span data-ttu-id="707f6-320">**고객 연락처**: 공동 판매 리퍼럴을 만들려면 기회에 고객 연락처를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-320">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="707f6-321">**Microsoft 솔루션**: microsoft와의 조회를 공유 하려면 올바른 공동 판매 준비 또는 microsoft 솔루션을 기회에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-321">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>

   1. <span data-ttu-id="707f6-322">**파트너 센터와의 동기화 기회 센터** 옵션을 **예** 로 설정한 후 10 분 동안 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-322">After you have set the opportunity **Sync with Partner Center** option to **Yes**, wait for 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="707f6-323">조회가 Salesforce CRM와 동기화 되 고 조회 링크가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-323">Your referrals will be synchronized with Salesforce CRM, and Referral Link will get populated.</span></span> <span data-ttu-id="707f6-324">오류가 있으면 감사 필드가 오류 정보로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-324">If there's a failure, the Audit field will be populated with error information.</span></span>

   1. <span data-ttu-id="707f6-325">마찬가지로, **파트너 센터와 동기화** 옵션이 **예** 로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-325">Similarly, when the **Sync with Partner Center** option is set to **Yes**, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

2. <span data-ttu-id="707f6-326">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="707f6-326">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="707f6-327">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-327">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    1. <span data-ttu-id="707f6-328">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-328">Select **Referrals** from the left-hand menu.</span></span>

    1. <span data-ttu-id="707f6-329">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-329">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    1. <span data-ttu-id="707f6-330">Salesforce CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-330">Sign into your Salesforce CRM environment.</span></span>

    1. <span data-ttu-id="707f6-331">**오픈 기회** 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-331">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="707f6-332">Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-332">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    1. <span data-ttu-id="707f6-333">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-333">When you select a synchronized referral, the card view details are populated.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce 기회 페이지의 스크린샷":::

>[!NOTE]
><span data-ttu-id="707f6-335">**배포에 대 한 도움이 필요 하세요?**</span><span class="sxs-lookup"><span data-stu-id="707f6-335">**Need help with deployment?**</span></span>
><span data-ttu-id="707f6-336">공동 판매 참조 커넥터 배포에 대 한 도움이 필요 하면 파트너 기술 컨설턴트와 협력 하 여</span><span class="sxs-lookup"><span data-stu-id="707f6-336">For assistance with your Co-sell referral connector deployment, you can engage a Partner Technical Consultant.</span></span> <span data-ttu-id="707f6-337">성공적인 구현에 대 한 배포 지원 및 모범 사례를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="707f6-337">They can provide deployment assistance and best practices for a successful implementation.</span></span>
>
><span data-ttu-id="707f6-338">자세한 내용은 [기술 예약 판매 및 배포 서비스 요청을 제출 하는 방법](technical-benefits.md) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="707f6-338">For more information, see [How to Submit a technical presales and deployment services request](technical-benefits.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="707f6-339">다음 단계</span><span class="sxs-lookup"><span data-stu-id="707f6-339">Next steps</span></span>

- [<span data-ttu-id="707f6-340">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="707f6-340">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="707f6-341">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="707f6-341">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="707f6-342">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="707f6-342">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
