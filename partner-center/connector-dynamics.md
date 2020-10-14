---
title: Dynamics 365 CRM 파트너 센터 용 공동 판매 커넥터
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dynamics 365 CRM 용 공동 판매 커넥터와 파트너 센터의 조회를 동기화 합니다. 그런 다음 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8ea803e675ce7c2d21d680491bbdaedf792e631f
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031336"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="8f5e6-104">Dynamics 365 CRM 용 공동 판매 커넥터-개요</span><span class="sxs-lookup"><span data-stu-id="8f5e6-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="8f5e6-105">적절한 역할</span><span class="sxs-lookup"><span data-stu-id="8f5e6-105">Appropriate roles</span></span>

- <span data-ttu-id="8f5e6-106">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="8f5e6-106">Referrals admin</span></span>
- <span data-ttu-id="8f5e6-107">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="8f5e6-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="8f5e6-108">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="8f5e6-109">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="8f5e6-110">공동 판매 커넥터를 사용 하 여 Microsoft 판매자와 연계 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 날짜를 사용 하는 새로운 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="8f5e6-111">이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="8f5e6-112">파트너 센터가 아닌 선택한 CRM 내에서 모든 조회 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="8f5e6-113">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="8f5e6-114">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="8f5e6-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="8f5e6-115">**토픽**</span><span class="sxs-lookup"><span data-stu-id="8f5e6-115">**Topics**</span></span>   |<span data-ttu-id="8f5e6-116">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="8f5e6-116">**Details**</span></span>   |<span data-ttu-id="8f5e6-117">**연결**</span><span class="sxs-lookup"><span data-stu-id="8f5e6-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="8f5e6-118">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="8f5e6-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="8f5e6-119">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-119">You need a valid MPN ID</span></span>|<span data-ttu-id="8f5e6-120">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="8f5e6-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="8f5e6-121">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="8f5e6-121">Cosell ready</span></span>|<span data-ttu-id="8f5e6-122">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="8f5e6-123">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="8f5e6-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="8f5e6-124">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="8f5e6-124">Partner Center account</span></span>|<span data-ttu-id="8f5e6-125">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="8f5e6-126">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="8f5e6-127">계정 관리</span><span class="sxs-lookup"><span data-stu-id="8f5e6-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="8f5e6-128">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="8f5e6-128">Partner Center user roles</span></span>|<span data-ttu-id="8f5e6-129">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="8f5e6-130">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="8f5e6-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="8f5e6-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="8f5e6-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="8f5e6-132">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="8f5e6-133">Dynamics 365에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="8f5e6-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="8f5e6-134">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="8f5e6-134">Power Automate Flow Account</span></span>|<span data-ttu-id="8f5e6-135">CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정</span><span class="sxs-lookup"><span data-stu-id="8f5e6-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="8f5e6-136">사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="8f5e6-137">Dynamics 365에 대 한 파트너 센터 조회 동기화 설치 (전원 자동화 솔루션)</span><span class="sxs-lookup"><span data-stu-id="8f5e6-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="8f5e6-138">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="8f5e6-139">이 단계에서는 사용 가능한 CRM 인스턴스를 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="8f5e6-140">오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="8f5e6-141">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="8f5e6-142">상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. <span data-ttu-id="8f5e6-144">**Dynamics365에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="8f5e6-145">**지금 가져오기** 단추를 클릭 한 다음 **계속**합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="8f5e6-146">그러면 응용 프로그램을 설치할 CRM (Dynamics 365) 환경을 선택할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="8f5e6-147">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="8f5e6-148">그런 다음 **솔루션 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="8f5e6-149">페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="8f5e6-150">파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="8f5e6-151">설치는 10-15 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="8f5e6-152">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="8f5e6-153">**Dynamics 365에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="8f5e6-154">**Dynamics 365에 대 한 파트너 센터 조회 동기화를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="8f5e6-155">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="AppSource 열기":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="8f5e6-157">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="8f5e6-157">Best practice: test before you go live</span></span>

<span data-ttu-id="8f5e6-158">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="8f5e6-159">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="8f5e6-160">솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="8f5e6-161">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="8f5e6-162">성공할 경우 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="8f5e6-163">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="8f5e6-163">Configure the solution</span></span>

1. <span data-ttu-id="8f5e6-164">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="8f5e6-165">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="8f5e6-166">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="8f5e6-167">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="8f5e6-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="8f5e6-168">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="8f5e6-168">Partner Center Events</span></span>

   - <span data-ttu-id="8f5e6-169">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="8f5e6-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="8f5e6-170">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="8f5e6-171">**연결 만들기**를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="AppSource 열기":::

      3. <span data-ttu-id="8f5e6-173">오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="8f5e6-174">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="8f5e6-175">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="8f5e6-176">CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="8f5e6-177">전원 자동화 흐름을 연결과 연결 하려면 각 전원 자동화 흐름을 편집 하 여 Common Data Service 및 파트너 센터 조회에 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-177">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="8f5e6-178">변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-178">Save the changes.</span></span>

5. <span data-ttu-id="8f5e6-179">전원 자동화 흐름을 **켭니다** .</span><span class="sxs-lookup"><span data-stu-id="8f5e6-179">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="8f5e6-180">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="8f5e6-180">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="8f5e6-181">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-181">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="8f5e6-182">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-182">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="8f5e6-183">Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-183">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="8f5e6-184">아래 강조 표시 된 대로 조회 관리자 자격 증명 (b.) 파트너 센터 이벤트를 사용 하 여 (a.) 파트너 센터 사용자에 대 한 연결을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-184">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="AppSource 열기":::

3. <span data-ttu-id="8f5e6-186">이러한 업데이트를 만들면 다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-186">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="AppSource 열기":::

4. <span data-ttu-id="8f5e6-188">변경 내용을 저장 하 고 **켜기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-188">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="8f5e6-189">파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-189">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="8f5e6-190">**파트너 센터에서 Dynamics 365 (Insider preview)을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-190">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="8f5e6-191">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-191">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="8f5e6-192">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-192">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="AppSource 열기":::

8. <span data-ttu-id="8f5e6-194">이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-194">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="8f5e6-195">오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-195">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="8f5e6-196">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-196">Enter the following details:</span></span>

    1. <span data-ttu-id="8f5e6-197">**Http 트리거 끝점**: 이전 단계에서 복사한 URL</span><span class="sxs-lookup"><span data-stu-id="8f5e6-197">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="8f5e6-198">**등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"</span><span class="sxs-lookup"><span data-stu-id="8f5e6-198">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="8f5e6-199">**기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)</span><span class="sxs-lookup"><span data-stu-id="8f5e6-199">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="8f5e6-200">**실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="8f5e6-200">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="8f5e6-201">이제 웹 후크를 수신 대기 하 여 이벤트를 만들고 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-201">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="8f5e6-202">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="8f5e6-202">Customize synchronization steps</span></span>

<span data-ttu-id="8f5e6-203">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-203">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="8f5e6-204">CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-204">Often CRM systems are highly customized.</span></span> <span data-ttu-id="8f5e6-205">전원 자동화 흐름을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-205">You can customize the Power Automate flows.</span></span> <span data-ttu-id="8f5e6-206">필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-206">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="8f5e6-207">CRM에 대 한 Microsoft 파트너 센터 매핑이 제공 되지만 CRM 환경에 따라 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-207">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="8f5e6-208">각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-208">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="8f5e6-209">사용 가능한 사용자 지정의 예는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-209">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="8f5e6-210">파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-210">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="8f5e6-211">a.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-211">a.</span></span> <span data-ttu-id="8f5e6-212">파트너 센터에서 Dynamics 365 (Insider Preview) 또는 파트너 센터를 Salesforce (Insider preview)로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-212">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="8f5e6-213">b.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-213">b.</span></span> <span data-ttu-id="8f5e6-214">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-214">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="8f5e6-215">다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-215">c.</span></span> <span data-ttu-id="8f5e6-216">선택 **(범위) 잠재 고객 또는 기회를 동기화**합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-216">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="8f5e6-217">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **새 공유 기회 인지 여부**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-217">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="8f5e6-218">**예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기**를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-218">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="8f5e6-219">필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-219">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="8f5e6-220">d.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-220">d.</span></span> <span data-ttu-id="8f5e6-221">업데이트 이벤트의 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 "(범위) 잠재 고객 또는 기회 동기화" 단계를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-221">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="8f5e6-222">e.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-222">e.</span></span> <span data-ttu-id="8f5e6-223">**기회를 업데이트 하는 경우를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-223">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="8f5e6-224">**예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를**확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-224">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="8f5e6-225">f.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-225">f.</span></span> <span data-ttu-id="8f5e6-226">**예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-226">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="8f5e6-227">업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:</span><span class="sxs-lookup"><span data-stu-id="8f5e6-227">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="8f5e6-228">a.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-228">a.</span></span> <span data-ttu-id="8f5e6-229">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="8f5e6-230">b.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-230">b.</span></span> <span data-ttu-id="8f5e6-231">**기회 동기화를 선택 (범위)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-231">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="8f5e6-232">다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-232">c.</span></span> <span data-ttu-id="8f5e6-233">업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 **파트너 센터와 crm의 리드 개체 사이에 차이가 있는 경우**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-233">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="8f5e6-234">d.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-234">d.</span></span> <span data-ttu-id="8f5e6-235">**예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트**단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-235">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="8f5e6-236">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-236">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="8f5e6-237">만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면</span><span class="sxs-lookup"><span data-stu-id="8f5e6-237">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="8f5e6-238">a.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-238">a.</span></span> <span data-ttu-id="8f5e6-239">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="8f5e6-240">b.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-240">b.</span></span> <span data-ttu-id="8f5e6-241">**조회 동기화를 선택 (범위) 합니다.**</span><span class="sxs-lookup"><span data-stu-id="8f5e6-241">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="8f5e6-242">다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-242">c.</span></span> <span data-ttu-id="8f5e6-243">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-243">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="8f5e6-244">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="8f5e6-245">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="8f5e6-245">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="8f5e6-246">전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하 고 나면 Dynamics 365와 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-246">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="8f5e6-247">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="8f5e6-247">Pre-requisites</span></span>

<span data-ttu-id="8f5e6-248">파트너 센터 및 Dynamics 365 CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 정하는 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-248">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="8f5e6-249">이 id는 판매자 팀이 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-249">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="8f5e6-250">사용자 지정 필드 집합은 **기회** 엔터티의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-250">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="8f5e6-251">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-251">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="8f5e6-252">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-252">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="8f5e6-253">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="8f5e6-253">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="8f5e6-254">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="8f5e6-254">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="8f5e6-255">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="8f5e6-255">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="8f5e6-256">**Microsoft에서 microsoft의 도움**을 받아야 하는 방법: microsoft에서 조회에 대 한 도움말</span><span class="sxs-lookup"><span data-stu-id="8f5e6-256">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="8f5e6-257">**제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="8f5e6-257">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="8f5e6-258">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="8f5e6-258">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="8f5e6-259">에서는</span><span class="sxs-lookup"><span data-stu-id="8f5e6-259">SCENARIOS:</span></span>

1. <span data-ttu-id="8f5e6-260">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="8f5e6-260">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="8f5e6-261">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 DYNAMICS 365 crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-261">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="8f5e6-262">Dynamics 365 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-262">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="AppSource 열기":::

   3. <span data-ttu-id="8f5e6-264">이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-264">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="8f5e6-265">**파트너 센터와 동기화**: 예</span><span class="sxs-lookup"><span data-stu-id="8f5e6-265">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="8f5e6-266">**Microsoft에서 도움을 주는 방법**: 다음 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-266">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="AppSource 열기":::

      - <span data-ttu-id="8f5e6-268">**제품**: 제품의 솔루션 id</span><span class="sxs-lookup"><span data-stu-id="8f5e6-268">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="8f5e6-269">**파트너 센터** 옵션을 **예**로 설정 하 여 Dynamics 365에 대 한 기회가 만들어지면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-269">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="8f5e6-270">사용자의 조회가 Dynamics 365와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-270">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="8f5e6-271">마찬가지로, "파트너 센터와 동기화" 옵션을 "예"로 설정 하는 기회에 대해 Dynamics 365 CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-271">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="8f5e6-272">파트너 센터와 성공적으로 동기화 되는 기회는 Dynamics 365의 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-272">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="8f5e6-273">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Dynamics 365 환경에서 동기화 할 때 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="8f5e6-273">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="8f5e6-274">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-274">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="8f5e6-275">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-275">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="8f5e6-276">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-276">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="8f5e6-277">Dynamics 365 CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-277">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="8f5e6-278">**오픈 기회**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-278">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="8f5e6-279">Microsoft Partner Center에서 만든 조회는 이제 Dynamics 365 CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-279">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="8f5e6-280">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="8f5e6-280">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8f5e6-281">다음 단계</span><span class="sxs-lookup"><span data-stu-id="8f5e6-281">Next steps</span></span>

- [<span data-ttu-id="8f5e6-282">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="8f5e6-282">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="8f5e6-283">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="8f5e6-283">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="8f5e6-284">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="8f5e6-284">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="8f5e6-285">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="8f5e6-285">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)