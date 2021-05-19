---
title: Salesforce CRM 파트너 센터 대한 공동 판매 커넥터
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 조회를 Salesforce CRM과 동기화합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148417"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="597e6-104">Salesforce CRM용 공동 판매 커넥터 – 개요</span><span class="sxs-lookup"><span data-stu-id="597e6-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="597e6-105">**적절한 역할:** 조회 관리자 | CRM의 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="597e6-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="597e6-106">파트너 센터 공동 판매 커넥터를 사용하면 판매자가 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="597e6-107">공동 판매 거래를 관리하는 데 파트너 센터 사용하도록 학습할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="597e6-108">공동 판매 커넥터를 사용하여 새 공동 판매 추천을 만들어 Microsoft 판매자에게 참여시키고, Microsoft 판매자로부터 추천을 받고, 추천을 수락/거부하고, 거래 가치와 같은 거래 데이터를 수정하고, 종료 날짜를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="597e6-109">이러한 공동 판매 거래에 대한 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="597e6-110">파트너 센터 대신 선택한 CRM 내에서 작업하는 동안 모든 조회 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="597e6-111">솔루션은 Microsoft Power Automate Solution을 기반으로 하며 파트너 센터 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="597e6-112">설치하기 전에 - 필수 조건</span><span class="sxs-lookup"><span data-stu-id="597e6-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="597e6-113">**토픽**</span><span class="sxs-lookup"><span data-stu-id="597e6-113">**Topics**</span></span>   |<span data-ttu-id="597e6-114">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="597e6-114">**Details**</span></span>   |<span data-ttu-id="597e6-115">**연결**</span><span class="sxs-lookup"><span data-stu-id="597e6-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="597e6-116">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="597e6-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="597e6-117">유효한 MPN ID가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-117">You need a valid MPN ID</span></span>|<span data-ttu-id="597e6-118">[MPN을](https://partner.microsoft.com/) 조인하려면</span><span class="sxs-lookup"><span data-stu-id="597e6-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="597e6-119">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="597e6-119">Co-sell ready</span></span>|<span data-ttu-id="597e6-120">IP/서비스 솔루션은 공동 판매 준비가 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="597e6-121">Microsoft로 판매</span><span class="sxs-lookup"><span data-stu-id="597e6-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="597e6-122">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="597e6-122">Partner Center account</span></span>|<span data-ttu-id="597e6-123">파트너 센터 테넌트와 연결된 MPN ID는 공동 판매 솔루션과 연결된 MPN ID와 동일해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="597e6-124">커넥터를 배포하기 전에 파트너 센터 Portal에서 공동 판매 추천을 볼 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="597e6-125">계정 관리</span><span class="sxs-lookup"><span data-stu-id="597e6-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="597e6-126">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="597e6-126">Partner Center user roles</span></span>|<span data-ttu-id="597e6-127">커넥터를 설치하고 사용할 직원은 조회 관리자여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="597e6-128">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="597e6-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="597e6-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="597e6-129">Salesforce CRM</span></span>|<span data-ttu-id="597e6-130">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="597e6-131">Salesforce CRM에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="597e6-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="597e6-132">Power Automate Flow 계정</span><span class="sxs-lookup"><span data-stu-id="597e6-132">Power Automate Flow Account</span></span>|<span data-ttu-id="597e6-133">CRM 시스템 관리자 또는 시스템 사용자 지정자의 활성 [Power Automate](https://flow.microsoft.com) 계정입니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="597e6-134">해당 사용자는 설치 전에 한 번 이상 [Power Automate](https://flow.microsoft.com) 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="597e6-135">Microsoft 사용자 지정 필드용 Salesforce 패키지 설치</span><span class="sxs-lookup"><span data-stu-id="597e6-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="597e6-136">파트너 센터 및 Salesforce CRM에서 조회를 동기화하려면 Power Automate 솔루션이 Microsoft 특정 조회 필드를 명확하게 식별해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="597e6-137">이 구분은 파트너 판매자 팀이 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있는 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="597e6-138">Salesforce에서 **메모를** 활성화하고 기회 관련 목록에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="597e6-139">참조</span><span class="sxs-lookup"><span data-stu-id="597e6-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="597e6-140">다음 단계에 따라 **기회 팀을** 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="597e6-141">설치 프로그램에서 **빠른 찾기** 상자를 사용하여 기회 팀 설정을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="597e6-142">필요에 따라 설정을 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-142">Define the settings as needed.</span></span>
[<span data-ttu-id="597e6-143">참조</span><span class="sxs-lookup"><span data-stu-id="597e6-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="597e6-144">Salesforce에서 패키지 설치 관리자 를 사용하여 사용자 지정 필드 및 개체를 [설치합니다.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)</span><span class="sxs-lookup"><span data-stu-id="597e6-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="597e6-145">이 방법을 사용하여 모든 회사에 패키지를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="597e6-146">샌드박스에 설치하는 경우 URL의 초기 부분을 로 바꾸어야 합니다. http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="597e6-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="597e6-147">Salesforce에서 **기회** 관련 목록에 Microsoft 솔루션을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="597e6-148">추가되면 **렌치** 아이콘을 선택하고 속성을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="597e6-149">모범 사례: 라이브로 진행하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="597e6-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="597e6-150">프로덕션 환경에서 Power Automate 솔루션을 설치, 구성 및 사용자 지정하기 전에 준비 CRM 인스턴스에서 솔루션을 테스트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="597e6-151">스테이징 환경/CRM 인스턴스에 Microsoft Power Automate 솔루션을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="597e6-152">솔루션의 복사본을 만들고 스테이징 환경에서 구성 및 Power Automate 흐름 사용자 지정을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="597e6-153">스테이징/CRM 인스턴스에서 솔루션을 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="597e6-154">성공하면 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="597e6-155">Salesforce CRM에 대한 파트너 센터 조회 동기화 설치</span><span class="sxs-lookup"><span data-stu-id="597e6-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="597e6-156">[Power Automate](https://flow.microsoft.com) 이동하여 오른쪽 위 모서리에서 **환경을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="597e6-157">그러면 사용 가능한 CRM 인스턴스가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="597e6-158">오른쪽 위 모서리의 드롭다운에서 적절한 CRM 인스턴스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="597e6-159">왼쪽 탐색 모음에서 **솔루션을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="597e6-160">위쪽 메뉴에서 **AppSource 열기** 링크를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. <span data-ttu-id="597e6-162">팝업 화면에서 **salesforce에 대한 파트너 센터 조회 커넥터를** 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="597e6-164">지금 **받기** 단추를 선택한 **다음, 계속을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="597e6-165">그러면 Salesforce CRM 환경을 선택하여 애플리케이션을 설치할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="597e6-166">약관에 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="사용 가능한 CRM":::

8. <span data-ttu-id="597e6-168">그런 다음 솔루션 관리 페이지로 **안내됩니다.**</span><span class="sxs-lookup"><span data-stu-id="597e6-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="597e6-169">페이지 아래쪽의 화살표 단추를 사용하여 "파트너 센터 조회"로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="597e6-170">파트너 센터 조회 솔루션 옆에 **설치가 예약되어** 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="597e6-171">설치하는 데 10-15분이 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="597e6-172">설치가 완료되면 [Power Automate](https://flow.microsoft.com) 다시 이동하고 왼쪽 탐색 영역에서 **솔루션을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="597e6-173">**Salesforce에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="597e6-174">**Salesforce에 대 한 파트너 센터 조회 동기화를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="597e6-175">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce 흐름":::



## <a name="configure-the-solution"></a><span data-ttu-id="597e6-177">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="597e6-177">Configure the solution</span></span>

1. <span data-ttu-id="597e6-178">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="597e6-179">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="597e6-180">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="597e6-181">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="597e6-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="597e6-182">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="597e6-182">Partner Center Events</span></span>
    - <span data-ttu-id="597e6-183">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="597e6-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="597e6-184">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="597e6-185">**연결 만들기** 를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="연결 만들기":::

- <span data-ttu-id="597e6-187">오른쪽 위 모서리의 검색 창에서 파트너 센터 조회 (미리 보기)를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="597e6-188">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="597e6-189">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="597e6-190">CRM 관리자 사용자에 대 한 Salesforce에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="597e6-191">모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="연결 관찰":::

### <a name="edit-the-connections"></a><span data-ttu-id="597e6-193">연결 편집</span><span class="sxs-lookup"><span data-stu-id="597e6-193">Edit the connections</span></span>

1. <span data-ttu-id="597e6-194">솔루션 페이지로 돌아가서 **기본 솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="597e6-195">**모두** 를 클릭 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="커넥터 편집 시작":::

2. <span data-ttu-id="597e6-197">세 개의 점 아이콘을 선택 하 여 각 연결을 개별적으로 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="597e6-198">관련 연결을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="커넥터 편집":::

3. <span data-ttu-id="597e6-200">다음 순서로 흐름을 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="597e6-201">파트너 센터 Webhook 등록 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="597e6-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="597e6-202">공동 판매 참조-Salesforce를 파트너 센터 (Insider Preview)에 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="597e6-203">파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="597e6-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="597e6-204">파트너 센터를 Salesforce로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="597e6-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="597e6-205">Salesforce에서 파트너 센터로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="597e6-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="597e6-206">Salesforce 기회와 파트너 센터 간 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="597e6-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="597e6-207">파트너 센터 (Insider Preview)에 대 한 Salesforce Microsoft 솔루션</span><span class="sxs-lookup"><span data-stu-id="597e6-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="597e6-208">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="597e6-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="597e6-209">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="597e6-210">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="597e6-211">Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="597e6-212">아래 강조 표시 된 대로 조회 관리자 자격 증명 (b.) 파트너 센터 이벤트를 사용 하 여 (a.) 파트너 센터 사용자에 대 한 연결을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="트리거":::

3. <span data-ttu-id="597e6-214">이러한 업데이트를 만들면 다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="597e6-216">변경 내용을 저장 하 고 **켜기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="597e6-217">파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="597e6-218">**Salesforce CRM에 파트너 센터(Insider Preview)** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="597e6-219">**편집** 아이콘을 선택하고 **HTTP 요청을 받은 경우를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="597e6-220">**복사** 아이콘을 선택하여 제공된 HTTP POST URL을 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 복사":::

8. <span data-ttu-id="597e6-222">이제 "파트너 센터 Webhook 등록(Insider Preview)" Power Automate 흐름을 선택하고 **실행을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="597e6-223">오른쪽 창에서 "흐름 실행" 창이 열리는지 확인하고 **계속을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="597e6-224">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-224">Enter the following details:</span></span>

    1. <span data-ttu-id="597e6-225">**Http 트리거 엔드포인트:** 이전 단계에서 복사한 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="597e6-226">**등록할 이벤트:**"조회가 생성됨" 및 "조회 업데이트됨"</span><span class="sxs-lookup"><span data-stu-id="597e6-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="597e6-227">**기존 트리거 엔드포인트(있는 경우)를 덮어씁니다.** 예(기존 엔드포인트를 덮어씁니다.)</span><span class="sxs-lookup"><span data-stu-id="597e6-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="597e6-228">**실행을** 선택한 **다음, 완료를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="597e6-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="597e6-229">이제 webhook는 이벤트를 만들고 업데이트하기 위해 수신 대기할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="597e6-230">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="597e6-230">Customize synchronization steps</span></span>

<span data-ttu-id="597e6-231">파트너 센터 CRM 시스템 간에 공동 판매 조회가 동기화되면 파트너 센터 PC에서 동기화되는 필드가 여기에 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="597e6-232">CRM 시스템은 종종 고도로 사용자 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="597e6-233">Power Automate 흐름을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="597e6-234">필드 매핑 가이드에 따라 필요한 경우 Power Automate 흐름의 단계를 적절하게 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="597e6-235">CRM에 대한 Microsoft 파트너 센터 매핑이 제공되지만 CRM 환경에 따라 필드를 추가로 사용자 지정하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="597e6-236">각 Power Automate 흐름의 여러 단계를 필요에 따라 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="597e6-237">다음은 사용 가능한 사용자 지정의 예입니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="597e6-238">crm 조회 동기화에 대한 파트너 센터 만들기 또는 업데이트 이벤트에 대한 필드를 사용자 지정하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="597e6-239">Salesforce CRM에 파트너 센터 선택합니다(Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="597e6-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="597e6-240">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="597e6-241">선택 **(범위) 잠재 고객 또는 기회를 동기화** 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="597e6-242">이벤트 만들기에 대 한 CRM 필드 매핑을 사용자 지정 하려면 **새 공유 기회 인지 여부** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="597e6-243">**예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기** 를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="597e6-244">필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="597e6-245">업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 "(범위) 리드 또는 기회 동기화" 단계를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="597e6-246">**기회를 업데이트 하는 경우를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="597e6-247">**예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를** 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="597e6-248">**예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="597e6-249">업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:</span><span class="sxs-lookup"><span data-stu-id="597e6-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="597e6-250">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="597e6-251">**기회 동기화를 선택 (범위)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="597e6-252">업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="597e6-253">**예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트** 단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="597e6-254">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="597e6-255">만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면</span><span class="sxs-lookup"><span data-stu-id="597e6-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="597e6-256">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="597e6-257">**조회 동기화를 선택 (범위) 합니다.**</span><span class="sxs-lookup"><span data-stu-id="597e6-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="597e6-258">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="597e6-259">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="597e6-260">엔드투엔드 양방향 공동 판매 조회 동기화</span><span class="sxs-lookup"><span data-stu-id="597e6-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="597e6-261">Power Automate 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간의 공동 판매 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="597e6-262">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="597e6-262">Pre-requisites</span></span>

<span data-ttu-id="597e6-263">파트너 센터 및 Salesforce CRM에서 조회를 동기화하려면 Power Automate 솔루션이 Microsoft 특정 조회 필드를 명확하게 구분해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="597e6-264">이 ID를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유하려는 추천을 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="597e6-265">사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="597e6-266">CRM 관리자 사용자는 **기회** 사용자 지정 필드를 사용하여 별도의 CRM 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="597e6-267">다음 사용자 지정 필드는 CRM 섹션의 일부여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="597e6-268">**파트너 센터 동기화:** 기회를 Microsoft 파트너 센터 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="597e6-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="597e6-269">**조회 식별자:** Microsoft 파트너 센터 조회에 대한 읽기 전용 식별자 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="597e6-270">**조회 링크:** Microsoft 파트너 센터 조회에 대한 읽기 전용 링크입니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="597e6-271">**Microsoft 도움말** 방법: 추천을 위해 Microsoft에서 필요한 도움말</span><span class="sxs-lookup"><span data-stu-id="597e6-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="597e6-272">**제품:** 이 기회와 관련된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="597e6-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="597e6-273">**감사:** 파트너 센터 조회와 동기화하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="597e6-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="597e6-274">시나리오:</span><span class="sxs-lookup"><span data-stu-id="597e6-274">SCENARIOS:</span></span>

1. <span data-ttu-id="597e6-275">CRM에서 조회를 만들거나 업데이트하고 파트너 센터 동기화할 때 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="597e6-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="597e6-276">CRM의 **기회** 섹션에서 가시성이 있는 사용자로 Salesforce CRM 환경에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="597e6-277">Salesforce CRM 환경에서 "새 기회"를 만들 때 다음 섹션이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 환경":::

   3. <span data-ttu-id="597e6-279">이 기회를 Microsoft 파트너 센터 동기화하려면 카드 보기에서 다음 필드를 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="597e6-280">"파트너 센터 동기화": 예</span><span class="sxs-lookup"><span data-stu-id="597e6-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="597e6-281">"Microsoft의 도움을 주는 방법": 다음 옵션 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="597e6-282">제품: 제품의 솔루션 Id</span><span class="sxs-lookup"><span data-stu-id="597e6-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="597e6-283">**파트너 센터와의 동기화 기회 센터** 옵션을 **예** 로 설정 했으면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="597e6-284">조회가 Salesforce CRM과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="597e6-285">"파트너 센터와 동기화" 옵션이 "예"로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="597e6-286">파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="597e6-287">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="597e6-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="597e6-288">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="597e6-289">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="597e6-290">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="597e6-291">Salesforce CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="597e6-292">**오픈 기회** 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="597e6-293">Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 기회 화면":::

    6. <span data-ttu-id="597e6-295">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="597e6-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="597e6-296">다음 단계</span><span class="sxs-lookup"><span data-stu-id="597e6-296">Next steps</span></span>

- [<span data-ttu-id="597e6-297">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="597e6-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="597e6-298">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="597e6-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="597e6-299">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="597e6-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
