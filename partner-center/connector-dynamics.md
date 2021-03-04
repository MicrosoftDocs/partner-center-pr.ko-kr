---
title: Dynamics 365 CRM 파트너 센터 용 공동 판매 커넥터
ms.topic: how-to
ms.date: 03/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dynamics 365 CRM 용 공동 판매 커넥터와 파트너 센터의 조회를 동기화 합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 10062fd20e3553856d8b595efd3224ff456c2c49
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756800"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="67239-104">Dynamics 365 CRM 용 공동 판매 커넥터-개요</span><span class="sxs-lookup"><span data-stu-id="67239-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="67239-105">적절한 역할</span><span class="sxs-lookup"><span data-stu-id="67239-105">Appropriate roles</span></span>

- <span data-ttu-id="67239-106">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="67239-106">Referrals admin</span></span>
- <span data-ttu-id="67239-107">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="67239-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="67239-108">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-108">Partner Center Co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="67239-109">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="67239-110">공동 판매 커넥터를 사용 하 여 Microsoft 판매자와 연계 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 날짜를 사용 하는 새로운 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="67239-111">이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="67239-112">파트너 센터가 아닌 선택한 CRM의 모든 조회 작업을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-112">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="67239-113">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="67239-114">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="67239-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="67239-115">**토픽**</span><span class="sxs-lookup"><span data-stu-id="67239-115">**Topics**</span></span>   |<span data-ttu-id="67239-116">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="67239-116">**Details**</span></span>   |<span data-ttu-id="67239-117">**연결**</span><span class="sxs-lookup"><span data-stu-id="67239-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="67239-118">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="67239-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="67239-119">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-119">You need a valid MPN ID</span></span>|<span data-ttu-id="67239-120">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="67239-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="67239-121">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="67239-121">Co-sell ready</span></span>|<span data-ttu-id="67239-122">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="67239-123">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="67239-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="67239-124">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="67239-124">Partner Center account</span></span>|<span data-ttu-id="67239-125">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="67239-126">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="67239-127">계정 관리</span><span class="sxs-lookup"><span data-stu-id="67239-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="67239-128">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="67239-128">Partner Center user roles</span></span>|<span data-ttu-id="67239-129">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="67239-130">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="67239-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| 
|<span data-ttu-id="67239-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="67239-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="67239-132">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="67239-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="67239-133">Dynamics 365에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="67239-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="67239-134">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="67239-134">Power Automate Flow Account</span></span>|<span data-ttu-id="67239-135">테스트/준비 및 프로덕션을 위해 데이터베이스를 사용 하 여 새 프로덕션 환경을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-135">Create new production environment with database for test/staging and production.</span></span> <span data-ttu-id="67239-136">데이터베이스를 사용 하는 기존 프로덕션 환경이 있는 경우 다시 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-136">If you have an existing production environment with database it can be re-used.</span></span> <span data-ttu-id="67239-137">커넥터 솔루션을 설치 하려는 사용자는 전원 자동화 라이선스 및이 환경에 대 한 액세스 권한이 있어야 합니다. 솔루션에서 기록 보기를 클릭 하 여 진행률을 모니터링 하 고 설치에 실패 하는 경우 자세한 [정보를 얻을](https://flow.microsoft.com/) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-137">User who is going to install connector solution needs to have Power Automate license and access to this environment.You can monitor the progress and get more details should the installation fail in [Power Automate](https://flow.microsoft.com/) by clicking See history under Solutions.</span></span>|[<span data-ttu-id="67239-138">환경 만들기 또는 관리</span><span class="sxs-lookup"><span data-stu-id="67239-138">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="67239-139">Dynamics 365에 대 한 파트너 센터 조회 동기화 설치 (전원 자동화 솔루션)</span><span class="sxs-lookup"><span data-stu-id="67239-139">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="67239-140">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-140">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="67239-141">이 단계에서는 사용 가능한 CRM 인스턴스를 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="67239-141">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="67239-142">오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-142">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="67239-143">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-143">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="67239-144">상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-144">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. <span data-ttu-id="67239-146">**Dynamics365에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-146">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="67239-147">**지금 가져오기** 단추를 클릭 한 다음 **계속** 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-147">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="67239-148">그러면 응용 프로그램을 설치할 CRM (Dynamics 365) 환경을 선택할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="67239-148">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="67239-149">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-149">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="67239-150">**솔루션** 에서 **기록 보기** 를 클릭 하 여 진행률을 모니터링 하 고 설치에 실패 하는 경우 자세한 정보를 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-150">You can monitor the progress and get more details should the installation fail in Power Automate by clicking **See history** under **Solutions**.</span></span>
 

9. <span data-ttu-id="67239-151">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="67239-152">**Dynamics 365에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="67239-153">**Dynamics 365에 대 한 파트너 센터 조회 동기화를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="67239-154">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="사용 가능한 CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="67239-156">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="67239-156">Best practice: test before you go live</span></span>

<span data-ttu-id="67239-157">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="67239-158">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="67239-159">스테이징 환경에서 Microsoft Power 자동화 솔루션을 구성 하 고 사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-159">Configure and customize the Microsoft Power Automate solution in staging environment.</span></span>
- <span data-ttu-id="67239-160">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="67239-161">성공할 경우 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="67239-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="67239-162">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="67239-162">Configure the solution</span></span>

1. <span data-ttu-id="67239-163">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="67239-164">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="67239-165">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="67239-166">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="67239-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="67239-167">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="67239-167">Partner Center Events</span></span>

   - <span data-ttu-id="67239-168">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="67239-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="67239-169">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="67239-170">**연결 만들기** 를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="연결 만들기":::

      3. <span data-ttu-id="67239-172">오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="67239-173">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="67239-174">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="67239-175">CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
      7. <span data-ttu-id="67239-176">모든 연결을 추가 하면 사용자 환경에 다음 연결이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-176">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="연결":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="67239-178">연결 편집</span><span class="sxs-lookup"><span data-stu-id="67239-178">Edit the connections</span></span>

1. <span data-ttu-id="67239-179">**솔루션** 페이지로 돌아가서 **기본 솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-179">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="67239-180">**모두** 를 클릭 하 여 **연결 참조 (미리 보기)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-180">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/connection-reference-video.gif" alt-text="연결 편집":::

2. <span data-ttu-id="67239-182">세 개의 점 아이콘을 선택 하 여 각 연결을 하나씩 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-182">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="67239-183">관련 연결을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-183">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="연결 나열"::: 

3.  <span data-ttu-id="67239-185">솔루션 페이지로 돌아가서, Dynamics 365에 대 한 파트너 센터 조회 동기화를 선택 하 고, 다음 시퀀스의 각 흐름 옆에 있는 세 개의 점 아이콘을 클릭 하 여 흐름을 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-185">Return to the Solutions page, select Partner Center Referrals Synchronization for Dynamics 365 and turn on the flow by clicking on three dots icon next to each flow in the following sequence.</span></span> <span data-ttu-id="67239-186">흐름을 설정 하는 동안 문제가 발생 하는 경우 [사용자 지정 단계](connector-dynamics.md#customize-synchronization-steps) 및 [문제 해결 단계](connectors-troubleshoot.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="67239-186">If you encounter any issues while turning on the flow refer to [customization steps](connector-dynamics.md#customize-synchronization-steps) and [troubleshooting steps](connectors-troubleshoot.md).</span></span> 

<span data-ttu-id="67239-187">다음 순서로 흐름을 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-187">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="67239-188">파트너 센터 Webhook 등록 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="67239-188">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="67239-189">공동 판매 조회 – Dynamics 365을 파트너 센터 (Insider Preview)에 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-189">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="67239-190">대로 Dynamics 365 flow에서 세부 정보를 만들거나 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="67239-190">[Customize] Create or Get Details from Dynamics 365 flow</span></span> 
- <span data-ttu-id="67239-191">파트너 센터-Dynamics 365-도우미 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="67239-191">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="67239-192">파트너 센터 Microsoft가 Dynamics 365 (Insider Preview)에 대 한 참조 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="67239-192">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="67239-193">파트너 센터에서 Dynamics 365로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="67239-193">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="67239-194">Dynamics 365-파트너 센터 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="67239-194">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="67239-195">Dynamics 365 기회 파트너 센터 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="67239-195">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="67239-196">Dynamics 365 Microsoft Solutions 파트너 센터 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="67239-196">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="67239-197">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="67239-197">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="67239-198">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-198">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="67239-199">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-199">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="67239-200">**파트너 센터에서 Dynamics 365 (Insider preview)을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-200">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

2. <span data-ttu-id="67239-201">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-201">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

3. <span data-ttu-id="67239-202">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-202">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

 :::image type="content" source="images/webhook-video.gif" alt-text="웹 후크를 사용 하 여 리소스 변경 내용 등록":::

4. <span data-ttu-id="67239-204">"파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-204">Select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and then select **Run**.</span></span>

5. <span data-ttu-id="67239-205">오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-205">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

6. <span data-ttu-id="67239-206">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-206">Enter the following details:</span></span>

   - <span data-ttu-id="67239-207">**Http 트리거 끝점**: 이전 단계에서 복사한 URL</span><span class="sxs-lookup"><span data-stu-id="67239-207">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

   - <span data-ttu-id="67239-208">**등록할 이벤트**: 사용 가능한 모든 이벤트 ("조회 생성", "조회-업데이트", "관련-조회 생성", "관련-조회-업데이트 됨")를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-208">**Events to Register**: Select all available events (“referral-created”, “referral-updated”, “related-referral-created”, “related-referral-updated”)</span></span>

   <span data-ttu-id="67239-209">-**기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예를 지정 하면 지정 된 webhook 이벤트에 대해 하나의 URL만 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-209">-**Overwrite existing trigger endpoints if present**: Yes It is important to note that only one URL can be registered for a given webhook event.</span></span> <span data-ttu-id="67239-210">지정 된 webhook 이벤트에 대해 하나의 URL만 등록할 수 있다는 점에 유의 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-210">It is important to note that only one URL can be registered for a given webhook event.</span></span> 

7. <span data-ttu-id="67239-211">**실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="67239-211">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="67239-212">이제 웹 후크를 수신 대기 하 여 이벤트를 만들고 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-212">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="67239-213">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="67239-213">Customize synchronization steps</span></span>

<span data-ttu-id="67239-214">CRM 시스템은 고도로 사용자 지정 되며 CRM 설정에 따라 전원 자동화 솔루션을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-214">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span>  <span data-ttu-id="67239-215">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 [사용자 지정 필드 매핑 가이드](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-215">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="67239-216">필드 매핑 가이드에 따라 필요한 경우 [사용자 지정]에서 적절 하 게 변경 하 여 **Dynamics 365 flow 또는 환경 변수에서 세부 정보를 만들거나 가져옵니다**  .</span><span class="sxs-lookup"><span data-stu-id="67239-216">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow**  or environment variables.</span></span> <span data-ttu-id="67239-217">이후 솔루션 업그레이드에 영향을 줄 수 있으므로 전원 자동화 솔루션에서 다른 흐름을 업데이트 하지 않는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-217">It is recommended not to update any other flows in Power Automate solution as it can impact future solution upgrades.</span></span> 

<span data-ttu-id="67239-218">사용할 수 있는 사용자 지정은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-218">The following are the available customizations:</span></span>

- <span data-ttu-id="67239-219">기회 이름에 표시 확인: 기본적으로 파트너 이름 옆에 확인 표시가 표시 되어 파트너 센터와 Dynamics 365 CRM 간의 동기화가 성공적으로 수행 됨을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-219">Check mark in Opportunity name: By default, a check mark will be displayed next to Opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="67239-220">마찬가지로 동기화가 실패할 경우 십자 표시가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-220">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="67239-221">기회 이름에 check 또는 cross mark를 추가 하지 않으려면 기회 이름 환경 변수에서 확인 표시 표시의 현재 값을 아니요로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-221">To avoid adding check or cross mark in Opportunity name, set the current value of Display check mark in opportunity name environment variable to No.</span></span>

- <span data-ttu-id="67239-222">거래 값: 기본적으로 파트너 센터의 거래 값은 CRM의 **estimatedvalue** 와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-222">Deal value: By default, deal value from Partner Center will be synced to and from **estimatedvalue** in CRM.</span></span> <span data-ttu-id="67239-223">처리할 거래 값에 대 한 다른 필드가 CRM에 있으면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-223">If you have a different field in CRM for deal value to sync from:</span></span>

    <span data-ttu-id="67239-224">a.</span><span class="sxs-lookup"><span data-stu-id="67239-224">a.</span></span>    <span data-ttu-id="67239-225">Dynamics 365 환경 변수의 거래 값 필드 이름을 CRM의 필드 이름으로 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-225">Update Deal value field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="67239-226">필드의 이름을 표시 이름으로 지정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-226">Note that you should provide the field’s name not its display name.</span></span>

    <span data-ttu-id="67239-227">b.</span><span class="sxs-lookup"><span data-stu-id="67239-227">b.</span></span>    <span data-ttu-id="67239-228">**[사용자 지정] 편집 [사용자 지정] Dynamics 365 flow에서 세부 정보를 만들거나** 업데이트 하 고 crm에서 기회 **만들기 또는 업데이트** 로 이동 하 고, crm에서 **DealValue** 값을 올바른 필드에 할당 하 **는** **기존 기회** 작업을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update** opportunity in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign **DealValue** value to correct field in CRM.</span></span> <span data-ttu-id="67239-229">또한 **예상 수익** 필드에서 **DealValue 할당** 을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-229">Also, remove **DealValue assignment** from **Estimated Revenue** field.</span></span>

- <span data-ttu-id="67239-230">고객 계정 국가 코드: 새 조회를 만들 때 두 문자로 된 국가 코드 (ISO 3166)를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-230">Customer Account Country Code: It is mandatory to provide a two-letter country code (ISO 3166) when creating a new referral.</span></span> <span data-ttu-id="67239-231">기본적으로 국가 코드는 CRM의 계정 address1_country 필드와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-231">By default, country code will be synced to and from Account’s address1_country field in CRM.</span></span> <span data-ttu-id="67239-232">CRM에서 동기화 할 국가 코드에 다른 필드가 있는 경우:</span><span class="sxs-lookup"><span data-stu-id="67239-232">If you have a different field in CRM for country code to sync from:</span></span>

   <span data-ttu-id="67239-233">a.</span><span class="sxs-lookup"><span data-stu-id="67239-233">a.</span></span>    <span data-ttu-id="67239-234">두 문자로 된 코드를 포함 하는 계정의 비 조회 국가 코드 필드:</span><span class="sxs-lookup"><span data-stu-id="67239-234">For a non-lookup country code field in Account which contains two-letter code:</span></span>

   - <span data-ttu-id="67239-235">Dynamics 365 환경 변수의 고객 계정 국가 코드 필드 이름을 CRM의 필드 이름으로 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-235">Update Customer account country code field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="67239-236">필드의 이름을 표시 이름으로 지정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-236">Note that you should provide the field’s name not its display name.</span></span>

   - <span data-ttu-id="67239-237">편집 **[사용자 지정] Dynamics 365 flow에서 세부 정보를 만들거나 가져온**  다음 crm에서 고객 계정 만들기 또는 가져오기를 탐색 하 여 crm의 올바른 필드에 국가 값을 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-237">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to Create or get customer account in CRM action to assign Country value to correct field in CRM.</span></span> <span data-ttu-id="67239-238">또한 Address 1: Country/Region 필드에서 Country value 할당을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-238">Also, remove Country value assignment from Address 1: Country/Region field.</span></span>

   <span data-ttu-id="67239-239">b.</span><span class="sxs-lookup"><span data-stu-id="67239-239">b.</span></span>    <span data-ttu-id="67239-240">계정에서 조회 기반 국가 코드 필드:</span><span class="sxs-lookup"><span data-stu-id="67239-240">For a lookup-based country code field in Account:</span></span>

   - <span data-ttu-id="67239-241">계정에 새 사용자 지정 필드를 추가 하 고 조회 기반 필드에서 선택한 값을 기준으로 두 문자 국가 코드 (ISO 3166)로 자동으로 채웁니다.</span><span class="sxs-lookup"><span data-stu-id="67239-241">Add a new custom field in Account and auto-populate it with two-letter country code (ISO 3166) based on the value selected in lookup-based field and vice-versa.</span></span>

   - <span data-ttu-id="67239-242">비 조회 국가 코드 필드에 대해 위의 단계를 수행 하 여 CRM의 새 사용자 지정 필드와 파트너 센터 간에 새 사용자 지정 필드를 동기화 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-242">Follow the steps above for non-lookup country code field to sync new custom field from CRM to and from Partner Center.</span></span>

- <span data-ttu-id="67239-243">기회 필드: [사용자 지정]을 채워야 하는 필수 필드가 필요 합니다. **[사용자 지정]을 사용 하 여 Dynamics 365 flow에서 세부 정보를 만들거나**  업데이트 하 고 CRM에서 **만들기 또는 업데이트 기회** 로 이동 하 여 비즈니스 요구 사항에 따라 필수 필드에 값을 할당 하는 **새 기회 작업을 만듭니다** .</span><span class="sxs-lookup"><span data-stu-id="67239-243">Opportunity fields: If there are mandatory fields in Opportunity that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update opportunity** in CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="67239-244">잠재 고객 필드: 입력 해야 하는 선행의 필수 필드 (편집 [사용자 지정])를 입력 해야 하 고, **Dynamics 365 flow에서 세부 정보를 만들거나**  업데이트 하 고, CRM에서 **잠재 고객** 을 만들거나 업데이트 하는 방법으로 이동 하 여 비즈니스 요구 사항에 따라 필수 필드에 값을 할당 하는 **새 잠재 고객 작업을 만듭니다** .</span><span class="sxs-lookup"><span data-stu-id="67239-244">Lead fields: If there are mandatory fields in Lead that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update lead** in CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="67239-245">고객 계정: 파트너 센터에서 CRM으로 새 조회를 동기화 할 때, Power 자동화 솔루션은 고객 회사 이름 및 우편 번호를 사용 하 여 CRM에서 기존 계정을 검색 하려고 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-245">Customer Account: When a new referral is synced from Partner Center to CRM, Power Automate solution tries to search for an existing account in CRM using customer company name and postal code.</span></span> <span data-ttu-id="67239-246">이를 찾지 못하면 CRM에서 새 고객 계정이 생성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-246">If it does not find one, a new customer account will be created in CRM.</span></span> <span data-ttu-id="67239-247">검색 조건 및 새 계정 만들기 세부 정보를 업데이트 하려면 **[사용자 지정]을 편집 하 여 Dynamics 365 flow에서 세부 정보를 만들거나** 확인 하 고 CRM에서 **고객 계정 만들기 또는 가져오기** 및 **고객 계정 만들기 작업** 으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-247">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and navigate to **Create or get customer account** in CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="67239-248">환경 변수 업데이트</span><span class="sxs-lookup"><span data-stu-id="67239-248">Update environment variable</span></span>

<span data-ttu-id="67239-249">환경 변수 값을 업데이트 하려면:</span><span class="sxs-lookup"><span data-stu-id="67239-249">To update an environment variable value:</span></span>

1. <span data-ttu-id="67239-250">**솔루션** 페이지로 이동 하 여 **기본 솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-250">Go to **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="67239-251">모두를 클릭 하 여 **환경 변수** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-251">Select **Environment Variable** by clicking All.</span></span>

2. <span data-ttu-id="67239-252">업데이트 해야 하는 값에 대 한 환경 변수를 선택 하 고 세 개의 점 아이콘을 사용 하 여 **편집** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-252">Select the environment variable for the value that needs to be updated and click **Edit** using three dots icon.</span></span>

3. <span data-ttu-id="67239-253">**새 값** 옵션을 사용 하 여 **현재 값** (기본값 업데이트 안 함)을 업데이트 하 고 값을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-253">Update **Current Value** (do not update Default Value) using **New value** option and provide the value.</span></span> <span data-ttu-id="67239-254">값은 변수의 데이터 형식과 일치 해야 합니다. 예/아니요 데이터 형식은 예 또는 아니요 값을 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-254">Value must match the Data type of the variable for e.g. Yes/No data type will accept either Yes or No value.</span></span>

:::image type="content" source="images/environment-variables-video.gif" alt-text="환경 변수 업데이트":::

- <span data-ttu-id="67239-256">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="67239-256">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="67239-257">전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하 고 나면 Dynamics 365와 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-257">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="67239-258">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="67239-258">Pre-requisites</span></span>

<span data-ttu-id="67239-259">파트너 센터 및 Dynamics 365 CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 정하는 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-259">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="67239-260">이 id는 판매자 팀이 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-260">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="67239-261">솔루션 설치의 일부로 사용자 지정 필드 및 개체 집합이 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-261">A set of custom fields and objects will get added as part of the solution installation.</span></span> <span data-ttu-id="67239-262">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-262">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="67239-263">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-263">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="67239-264">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부를 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-264">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center.</span></span> <span data-ttu-id="67239-265">기본적으로이 필드의 값은 아니요 이며 판매자가 Microsoft와의 기회를 공유 하도록 명시적으로 예로 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-265">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="67239-266">파트너 센터에서 CRM으로 공유 되는 새 조회는이 필드 값을 예로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-266">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="67239-267">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="67239-267">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="67239-268">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="67239-268">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>
- <span data-ttu-id="67239-269">**Microsoft에서 microsoft에 어떤 도움을 주는 것이 있나요?**: microsoft에서 조회에 대해 도움을 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-269">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="67239-270">공동 판매 조회를 만들려면 Microsoft에서 필요한 적절 한 도움말을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-270">To create a co-sell referral, select appropriate help required from Microsoft.</span></span> <span data-ttu-id="67239-271">고객 연락처를 공동 판매 참조를 만들 수 있는 기회에 연결 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-271">A customer contact must be associated to the Opportunity to create a co-sell referral.</span></span> <span data-ttu-id="67239-272">비 공동 판매 조회를 만들려면이 필드를 선택 취소 된 상태로 둡니다.</span><span class="sxs-lookup"><span data-stu-id="67239-272">To create a non co-sell referral leave this field un-selected.</span></span> <span data-ttu-id="67239-273">비 공동 판매 조회는 적절 한 도움말 필요 옵션을 선택 하 여 언제 든 지 공동 판매 조회로 변환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-273">A non co-sell referral can be converted to a co-sell referral anytime by selecting appropriate help required option.</span></span>

- <span data-ttu-id="67239-274">**Microsoft 파트너 센터 조회 표시 유형**: Microsoft 파트너 센터 조회에 대 한 표시 유형을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-274">**Microsoft Partner Center Referral Visibility**: Select visibility for Microsoft Partner Center Referral.</span></span> <span data-ttu-id="67239-275">Microsoft 판매자에 게 표시 되는 비 공동 판매 조회가 공동 판매로 전환 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-275">By making it visible to Microsoft sellers, a non co-sell referral may get converted to co-sell.</span></span> <span data-ttu-id="67239-276">Microsoft 도움말이 필요한 경우 기본적으로 Microsoft 판매자에 게 조회를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-276">When Microsoft help is required, referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="67239-277">표시로 표시 된 후에는이 필드를 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-277">Once marked as visible this field cannot be reverted.</span></span>

- <span data-ttu-id="67239-278">**MICROSOFT CRM identifier**: 공동 판매 조회가 microsoft에서 만들어지고 수락 되는 경우이 필드는 MICROSOFT의 CRM 식별자로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="67239-278">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft’s CRM identifier.</span></span>

- <span data-ttu-id="67239-279">**제품:** 사용 되지 않음 –이 필드를 사용 하지 않거나 CRM에 추가 하지 마세요. 이전 버전과의 호환성을 위해서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-279">**Products: Obsolete** – do not use this field or add it to CRM section, it is available for backward compatibility only.</span></span> <span data-ttu-id="67239-280">대신 Microsoft 파트너 센터 솔루션을 사용 하세요.</span><span class="sxs-lookup"><span data-stu-id="67239-280">Use Microsoft Partner Center Solutions instead.</span></span>

- <span data-ttu-id="67239-281">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="67239-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

- <span data-ttu-id="67239-282">**Microsoft 파트너 센터 솔루션**: 공동 판매 준비 된 솔루션 또는 Microsoft 솔루션을 기회와 연결 하는 사용자 지정 개체입니다.</span><span class="sxs-lookup"><span data-stu-id="67239-282">**Microsoft Partner Center Solutions**: A custom object to associate Co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="67239-283">하나 이상의 솔루션을 기회에서 추가 및/또는 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-283">One or more solutions can be added and/or removed from the Opportunity.</span></span> <span data-ttu-id="67239-284">Microsoft와 공유 하기 전에 하나 이상의 공동 판매 준비 또는 Microsoft 솔루션을 기회에 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-284">It is mandatory to add at least one Co-sell ready or Microsoft solution to the Opportunity before sharing it with Microsoft.</span></span> <span data-ttu-id="67239-285">이 개체를 기회에 연결 하려면 CRM에서 기회 양식을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-285">To associate this object to Opportunity, update the Opportunity form in CRM:</span></span>

  <span data-ttu-id="67239-286">기회 양식에서 적절 한 탭을 선택 하 고 아래와 같이 하위 그리드를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-286">Select the appropriate tab in Opportunity form and add a sub-grid as shown below:</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="기회 양식":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{대체 텍스트}":::



- <span data-ttu-id="67239-289">Microsoft 솔루션을 추가한 후에 판매자가 추가할 필요가 없도록 공동 판매 준비 된 솔루션 세부 정보를 미리 채울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67239-289">After adding Microsoft Solutions, you can pre-populate Co-sell ready solutions details so that your sellers don’t have to add them.</span></span> <span data-ttu-id="67239-290">새 솔루션 세부 정보를 추가 하려면 CRM의 Microsoft Solution Details 개체로 이동 하 고 **레코드 추가** 를 클릭 하 여 항목을 하나 추가 하거나 **Excel 업로드** 를 사용 하 여 여러 항목을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-290">To add a new solution detail, go to Microsoft Solution Details object in CRM and click on **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

:::image type="content" source="images/dynamic-1a.png" alt-text="솔루션 세부 정보":::

### <a name="scenarios"></a><span data-ttu-id="67239-292">에서는</span><span class="sxs-lookup"><span data-stu-id="67239-292">SCENARIOS:</span></span>

1. <span data-ttu-id="67239-293">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="67239-293">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="67239-294">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 DYNAMICS 365 crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-294">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="67239-295">Dynamics 365 환경에서 "새 기회"를 만들 때 Microsoft 파트너 센터 섹션이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-295">Ensure that the Microsoft Partner Center section  is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   :::image type="content" source="images/dynamic-2a.png" alt-text="새 기회"::: 

   3. <span data-ttu-id="67239-297">파트너 센터와이 기회를 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="67239-298">**Microsoft에서 어떻게 도울 수 있나요?**: 공동 판매 참조를 만들려면 적절 한 도움말 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-298">**How can Microsoft help?**: To create a Co-sell referral select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="카드 보기에서 적절 한 필드를 가져오는 방법":::

      - <span data-ttu-id="67239-300">**고객 연락처**: 공동 판매 조회를 만들려면 기회에 고객 연락처를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-300">**Customer Contact**: To create a Co-sell referral, add a customer contact to Opportunity.</span></span>
      - <span data-ttu-id="67239-301">**파트너 센터와 동기화**: 예</span><span class="sxs-lookup"><span data-stu-id="67239-301">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="67239-302">Microsoft 솔루션: Microsoft와의 조회를 공유 하려면 올바른 공동 판매 준비 또는 Microsoft 솔루션을 기회에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-302">Microsoft Solutions: To share a referral with Microsoft, add a valid Co-sell ready or Microsoft solution to Opportunity.</span></span>
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="솔루션 ID":::

   4. <span data-ttu-id="67239-304">파트너 센터 옵션을 예로 설정 하 여 Dynamics 365에 대 한 기회가 만들어지면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-304">Once the opportunity is created in Dynamics 365 with Sync with Partner Center option set to Yes, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="67239-305">사용자의 조회가 Dynamics 365 및 조회 식별자와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-305">Your referrals will be synchronized with Dynamics 365 and Referral Identifier.</span></span> <span data-ttu-id="67239-306">조회 링크를 채웁니다.</span><span class="sxs-lookup"><span data-stu-id="67239-306">Referral Link will get populated.</span></span> <span data-ttu-id="67239-307">오류가 발생 하는 경우 감사 필드가 오류 정보로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="67239-307">In case of a failure, the audit field will be populated with error information.</span></span>
     
    5. <span data-ttu-id="67239-308">마찬가지로, "파트너 센터와 동기화" 옵션을 "예"로 설정 하는 기회에 대해 Dynamics 365 CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-308">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    6. <span data-ttu-id="67239-309">파트너 센터와 성공적으로 동기화 되는 기회는 Dynamics 365의 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-309">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="67239-310">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Dynamics 365 환경에서 동기화 할 때 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="67239-310">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="67239-311">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-311">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="67239-312">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-312">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="67239-313">**새 거래** 옵션을 선택 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="67239-313">Create a new Co-sell referral from Partner Center by selecting the  **New deal** option.</span></span>

   4. <span data-ttu-id="67239-314">Dynamics 365 CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-314">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="67239-315">**오픈 기회** 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="67239-315">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="67239-316">Microsoft Partner Center에서 만든 조회는 이제 Dynamics 365 CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67239-316">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="67239-317">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="67239-317">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="67239-318">다음 단계</span><span class="sxs-lookup"><span data-stu-id="67239-318">Next steps</span></span>

- [<span data-ttu-id="67239-319">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="67239-319">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="67239-320">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="67239-320">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="67239-321">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="67239-321">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="67239-322">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="67239-322">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
