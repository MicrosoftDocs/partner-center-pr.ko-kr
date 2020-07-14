---
title: Salesforce CRM 파트너 센터에 대 한 공동 판매 커넥터
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 조회를 Salesforce CRM과 동기화
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 0a22587f5b555281cae6f557acfc2695ba92727e
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302380"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="c8f5b-103">Salesforce CRM용 공동 판매 커넥터 – 개요</span><span class="sxs-lookup"><span data-stu-id="c8f5b-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="c8f5b-104">적절한 역할</span><span class="sxs-lookup"><span data-stu-id="c8f5b-104">Appropriate roles</span></span>

- <span data-ttu-id="c8f5b-105">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="c8f5b-105">Referrals admin</span></span>
- <span data-ttu-id="c8f5b-106">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="c8f5b-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="c8f5b-107">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="c8f5b-108">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="c8f5b-109">공동 판매 커넥터를 사용 하 여 Microsoft 판매자를 참여 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 하는 새 공동 판매 참조를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="c8f5b-110">이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="c8f5b-111">파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안 모든 조회 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="c8f5b-112">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="c8f5b-113">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="c8f5b-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="c8f5b-114">**토픽**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-114">**Topics**</span></span>   |<span data-ttu-id="c8f5b-115">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-115">**Details**</span></span>   |<span data-ttu-id="c8f5b-116">**링크**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="c8f5b-117">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="c8f5b-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="c8f5b-118">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-118">You need a valid MPN ID</span></span>|<span data-ttu-id="c8f5b-119">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="c8f5b-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="c8f5b-120">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="c8f5b-120">Co-sell ready</span></span>|<span data-ttu-id="c8f5b-121">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="c8f5b-122">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="c8f5b-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="c8f5b-123">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="c8f5b-123">Partner Center account</span></span>|<span data-ttu-id="c8f5b-124">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="c8f5b-125">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="c8f5b-126">계정 관리</span><span class="sxs-lookup"><span data-stu-id="c8f5b-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c8f5b-127">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="c8f5b-127">Partner Center user roles</span></span>|<span data-ttu-id="c8f5b-128">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="c8f5b-129">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="c8f5b-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c8f5b-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="c8f5b-130">Salesforce CRM</span></span>|<span data-ttu-id="c8f5b-131">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="c8f5b-132">Salesforce CRM에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="c8f5b-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="c8f5b-133">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="c8f5b-133">Power Automate Flow Account</span></span>|<span data-ttu-id="c8f5b-134">CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정</span><span class="sxs-lookup"><span data-stu-id="c8f5b-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="c8f5b-135">사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="c8f5b-136">Salesforce CRM에 대 한 파트너 센터 조회 동기화 설치</span><span class="sxs-lookup"><span data-stu-id="c8f5b-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="c8f5b-137">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="c8f5b-138">그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="c8f5b-139">오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="c8f5b-140">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="c8f5b-141">상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource 열기":::

5. <span data-ttu-id="c8f5b-143">팝업 화면에서 **Salesforce에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="c8f5b-145">**지금 가져오기** 단추를 클릭 한 다음 **계속**합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="c8f5b-146">그러면 Salesforce CRM 환경을 선택 하 여 응용 프로그램을 설치할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="c8f5b-147">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="사용 가능한 CRMS":::

8. <span data-ttu-id="c8f5b-149">그런 다음 **솔루션 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="c8f5b-150">페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="c8f5b-151">파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="c8f5b-152">설치는 10-15 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="c8f5b-153">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="c8f5b-154">**Salesforce에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="c8f5b-155">**Salesforce에 대 한 파트너 센터 조회 동기화를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="c8f5b-156">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce 흐름":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="c8f5b-158">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="c8f5b-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="c8f5b-159">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="c8f5b-160">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="c8f5b-161">솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="c8f5b-162">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="c8f5b-163">성공할 경우 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="c8f5b-164">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="c8f5b-164">Configure the solution</span></span>

1. <span data-ttu-id="c8f5b-165">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="c8f5b-166">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="c8f5b-167">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="c8f5b-168">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="c8f5b-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="c8f5b-169">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="c8f5b-169">Partner Center Events</span></span>
   - <span data-ttu-id="c8f5b-170">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="c8f5b-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="c8f5b-171">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="c8f5b-172">**연결 만들기**를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="연결 만들기":::

   3. <span data-ttu-id="c8f5b-174">오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="c8f5b-175">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="c8f5b-176">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="c8f5b-177">CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="c8f5b-178">전원 자동화 흐름을 연결과 연결 하려면 각 전원 자동화 흐름을 편집 하 여 Common Data Service 및 파트너 센터 조회에 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="c8f5b-179">변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-179">Save the changes.</span></span>

5. <span data-ttu-id="c8f5b-180">전원 자동화 흐름을 **켭니다** .</span><span class="sxs-lookup"><span data-stu-id="c8f5b-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="c8f5b-181">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="c8f5b-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="c8f5b-182">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="c8f5b-183">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="c8f5b-184">Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="c8f5b-185">(A.)에 대 한 연결을 추가 합니다. 조회 관리자 자격 증명이 있는 파트너 센터 사용자 (b.) 아래 강조 표시 된 파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="c8f5b-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="트리거":::

3. <span data-ttu-id="c8f5b-187">이러한 업데이트를 만들면 다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="c8f5b-189">변경 내용을 저장 하 고 **켜기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="c8f5b-190">파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="c8f5b-191">**파트너 센터에서 SALESFORCE CRM (Insider preview)을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="c8f5b-192">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="c8f5b-193">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL 복사":::

8. <span data-ttu-id="c8f5b-195">이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="c8f5b-196">오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="c8f5b-197">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-197">Enter the following details:</span></span>

    1. <span data-ttu-id="c8f5b-198">**Http 트리거 끝점**: 이전 단계에서 복사한 URL</span><span class="sxs-lookup"><span data-stu-id="c8f5b-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="c8f5b-199">**등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"</span><span class="sxs-lookup"><span data-stu-id="c8f5b-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="c8f5b-200">**기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)</span><span class="sxs-lookup"><span data-stu-id="c8f5b-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="c8f5b-201">**실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="c8f5b-202">이제 웹 후크를 수신 대기 하 여 이벤트를 만들고 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="c8f5b-203">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="c8f5b-203">Customize synchronization steps</span></span>

<span data-ttu-id="c8f5b-204">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="c8f5b-205">CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="c8f5b-206">전원 자동화 흐름을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="c8f5b-207">필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="c8f5b-208">CRM에 대 한 Microsoft 파트너 센터 매핑이 제공 되지만 CRM 환경에 따라 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="c8f5b-209">각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="c8f5b-210">사용 가능한 사용자 지정의 예는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="c8f5b-211">파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="c8f5b-212">파트너 센터에서 Salesforce CRM (Insider Preview)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="c8f5b-213">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="c8f5b-214">선택 **(범위) 잠재 고객 또는 기회를 동기화**합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="c8f5b-215">이벤트 만들기에 대 한 CRM 필드 매핑을 사용자 지정 하려면 **새 공유 기회 인지 여부**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="c8f5b-216">**예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기**를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="c8f5b-217">필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="c8f5b-218">업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 "(범위) 잠재 고객 또는 기회 동기화" 단계를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="c8f5b-219">**기회를 업데이트 하는 경우를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="c8f5b-220">**예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를**확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="c8f5b-221">**예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="c8f5b-222">업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:</span><span class="sxs-lookup"><span data-stu-id="c8f5b-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="c8f5b-223">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="c8f5b-224">**기회 동기화를 선택 (범위)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="c8f5b-225">업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="c8f5b-226">**예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트**단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="c8f5b-227">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="c8f5b-228">만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면</span><span class="sxs-lookup"><span data-stu-id="c8f5b-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="c8f5b-229">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="c8f5b-230">**조회 동기화를 선택 (범위) 합니다.**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="c8f5b-231">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="c8f5b-232">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="c8f5b-233">Salesforce CRM 기회 레이아웃에서 별도의 섹션 만들기</span><span class="sxs-lookup"><span data-stu-id="c8f5b-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="c8f5b-234">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="c8f5b-235">이를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유할 조회를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c8f5b-236">사용자 지정 필드 집합은 Salesforce CRM **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="c8f5b-237">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="c8f5b-238">Salesforce CRM 관리자 사용자는 별도의 CRM 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="c8f5b-239">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="c8f5b-240">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="c8f5b-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="c8f5b-241">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="c8f5b-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="c8f5b-242">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="c8f5b-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="c8f5b-243">**Microsoft에서 어떤 도움을 하나요?**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-243">**How can Microsoft help?**</span></span> <span data-ttu-id="c8f5b-244">Microsoft에서 조회에 필요한 도움말</span><span class="sxs-lookup"><span data-stu-id="c8f5b-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="c8f5b-245">**제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="c8f5b-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="c8f5b-246">**감사**: Microsoft 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역입니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="c8f5b-247">필드 및 관계 설정</span><span class="sxs-lookup"><span data-stu-id="c8f5b-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="c8f5b-248">Salesforce 계정에 로그인 하 고 **기회**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="c8f5b-249">**설정** 및 **개체 편집** 옵션을 클릭 하 여 필요한 필드를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="c8f5b-250">왼쪽 탐색에서 **필드 & 관계** 선택</span><span class="sxs-lookup"><span data-stu-id="c8f5b-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="필드":::

4. <span data-ttu-id="c8f5b-252">**필드 & 관계** 테이블에 다음 필드를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="c8f5b-253">**필드 레이블**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-253">**Field label**</span></span>   |<span data-ttu-id="c8f5b-254">**필드 이름**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-254">**Field name**</span></span>|<span data-ttu-id="c8f5b-255">**데이터 형식**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-255">**Data type**</span></span>|<span data-ttu-id="c8f5b-256">**인덱싱**</span><span class="sxs-lookup"><span data-stu-id="c8f5b-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="c8f5b-257">감사</span><span class="sxs-lookup"><span data-stu-id="c8f5b-257">Audit</span></span>| <span data-ttu-id="c8f5b-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="c8f5b-258">Audit__c</span></span>|<span data-ttu-id="c8f5b-259">긴 텍스트 영역 (100000) (표시 되는 줄 4)</span><span class="sxs-lookup"><span data-stu-id="c8f5b-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="c8f5b-260">Microsoft에서 어떤 도움을 하나요?</span><span class="sxs-lookup"><span data-stu-id="c8f5b-260">How can Microsoft help?</span></span>|<span data-ttu-id="c8f5b-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="c8f5b-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="c8f5b-262">선택 목록</span><span class="sxs-lookup"><span data-stu-id="c8f5b-262">Picklist\*</span></span>|
   |<span data-ttu-id="c8f5b-263">제품</span><span class="sxs-lookup"><span data-stu-id="c8f5b-263">Products</span></span>|<span data-ttu-id="c8f5b-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="c8f5b-264">Products_c</span></span>|<span data-ttu-id="c8f5b-265">텍스트 (255)</span><span class="sxs-lookup"><span data-stu-id="c8f5b-265">text (255)</span></span>||
   |<span data-ttu-id="c8f5b-266">조회</span><span class="sxs-lookup"><span data-stu-id="c8f5b-266">Referral</span></span> | <span data-ttu-id="c8f5b-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="c8f5b-267">Referral_Identfier_c</span></span>|<span data-ttu-id="c8f5b-268">텍스트 (100) (외부 ID)</span><span class="sxs-lookup"><span data-stu-id="c8f5b-268">Text(100)(External ID)</span></span>|<span data-ttu-id="c8f5b-269">예</span><span class="sxs-lookup"><span data-stu-id="c8f5b-269">yes</span></span>|
   |<span data-ttu-id="c8f5b-270">조회 링크</span><span class="sxs-lookup"><span data-stu-id="c8f5b-270">Referral Link</span></span>| <span data-ttu-id="c8f5b-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="c8f5b-271">Referral_Link_c_</span></span>|<span data-ttu-id="c8f5b-272">URL (255)</span><span class="sxs-lookup"><span data-stu-id="c8f5b-272">URL(255)</span></span>||
   |<span data-ttu-id="c8f5b-273">파트너 센터와 동기화</span><span class="sxs-lookup"><span data-stu-id="c8f5b-273">Sync with Partner Center</span></span>|<span data-ttu-id="c8f5b-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="c8f5b-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="c8f5b-275">Checkbox (기본값 선택 하지 않음)</span><span class="sxs-lookup"><span data-stu-id="c8f5b-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="c8f5b-276">\* 선택 목록 값:</span><span class="sxs-lookup"><span data-stu-id="c8f5b-276">\*Picklist values:</span></span>

   - <span data-ttu-id="c8f5b-277">작업 관련 값 제안</span><span class="sxs-lookup"><span data-stu-id="c8f5b-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="c8f5b-278">고객 기술 아키텍처</span><span class="sxs-lookup"><span data-stu-id="c8f5b-278">Customer technical architecture</span></span>
   - <span data-ttu-id="c8f5b-279">개념 증명 또는 데모</span><span class="sxs-lookup"><span data-stu-id="c8f5b-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="c8f5b-280">견적 또는 라이선스</span><span class="sxs-lookup"><span data-stu-id="c8f5b-280">Quotes or licensing</span></span>
   - <span data-ttu-id="c8f5b-281">판매 고객 성공 후</span><span class="sxs-lookup"><span data-stu-id="c8f5b-281">Post sales customer success</span></span>
   - <span data-ttu-id="c8f5b-282">일반 또는 기타</span><span class="sxs-lookup"><span data-stu-id="c8f5b-282">General or other</span></span>

5. <span data-ttu-id="c8f5b-283">필드는 **관계 & 필드** 에 생성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="만든 필드":::

6. <span data-ttu-id="c8f5b-285">기회 레이아웃에서 위에 나열 된 필드를 사용 하 여 별도의 섹션을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="c8f5b-286">이 섹션은 기회 레이아웃의 판매자에 게 제공 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="파트너 센터 필드 레이아웃":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="c8f5b-288">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="c8f5b-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="c8f5b-289">전원 자동화 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="c8f5b-290">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="c8f5b-290">Pre-requisites</span></span>

<span data-ttu-id="c8f5b-291">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="c8f5b-292">이 id는 판매자 팀에 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c8f5b-293">사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="c8f5b-294">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="c8f5b-295">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="c8f5b-296">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="c8f5b-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="c8f5b-297">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="c8f5b-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="c8f5b-298">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="c8f5b-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="c8f5b-299">Microsoft의 도움을 주는 **방법**: microsoft에서 조회에 필요한 도움말</span><span class="sxs-lookup"><span data-stu-id="c8f5b-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="c8f5b-300">**제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="c8f5b-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="c8f5b-301">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="c8f5b-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="c8f5b-302">에서는</span><span class="sxs-lookup"><span data-stu-id="c8f5b-302">SCENARIOS:</span></span>

1. <span data-ttu-id="c8f5b-303">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="c8f5b-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="c8f5b-304">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 Salesforce crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="c8f5b-305">Salesforce CRM 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 환경":::

   3. <span data-ttu-id="c8f5b-307">이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="c8f5b-308">"파트너 센터와 동기화": 예</span><span class="sxs-lookup"><span data-stu-id="c8f5b-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="c8f5b-309">"Microsoft의 도움을 주는 방법": 다음 옵션 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="c8f5b-310">제품: 제품의 솔루션 Id</span><span class="sxs-lookup"><span data-stu-id="c8f5b-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="c8f5b-311">**파트너 센터와의 동기화 기회 센터** 옵션을 **예**로 설정 했으면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="c8f5b-312">조회가 Salesforce CRM과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="c8f5b-313">"파트너 센터와 동기화" 옵션이 "예"로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="c8f5b-314">파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="c8f5b-315">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="c8f5b-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="c8f5b-316">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="c8f5b-317">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="c8f5b-318">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="c8f5b-319">Salesforce CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="c8f5b-320">**오픈 기회**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="c8f5b-321">Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 기회 화면":::

    6. <span data-ttu-id="c8f5b-323">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="c8f5b-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c8f5b-324">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c8f5b-324">Next steps</span></span>

- [<span data-ttu-id="c8f5b-325">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="c8f5b-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="c8f5b-326">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="c8f5b-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="c8f5b-327">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="c8f5b-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="c8f5b-328">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="c8f5b-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)