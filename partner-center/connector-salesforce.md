---
title: Salesforce CRM 파트너 센터에 대 한 공동 판매 커넥터
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 조회를 Salesforce CRM과 동기화
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145107"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="02b8d-103">Salesforce CRM 용 공동 판매 커넥터-개요</span><span class="sxs-lookup"><span data-stu-id="02b8d-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="02b8d-104">적절한 역할</span><span class="sxs-lookup"><span data-stu-id="02b8d-104">Appropriate roles</span></span>

- <span data-ttu-id="02b8d-105">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="02b8d-105">Referrals admin</span></span>
- <span data-ttu-id="02b8d-106">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="02b8d-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="02b8d-107">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="02b8d-108">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="02b8d-109">공동 판매 커넥터를 사용 하 여 Microsoft 판매자를 참여 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 값과 같은 데이터를 수정 하 고, 종료 하는 새 공동 판매 참조를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="02b8d-110">이러한 공동 판매 거래에서 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="02b8d-111">파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안 모든 조회 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="02b8d-112">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="02b8d-113">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="02b8d-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="02b8d-114">**토픽**</span><span class="sxs-lookup"><span data-stu-id="02b8d-114">**Topics**</span></span>   |<span data-ttu-id="02b8d-115">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="02b8d-115">**Details**</span></span>   |<span data-ttu-id="02b8d-116">**링크**</span><span class="sxs-lookup"><span data-stu-id="02b8d-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="02b8d-117">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="02b8d-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="02b8d-118">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-118">You need a valid MPN ID</span></span>|<span data-ttu-id="02b8d-119">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="02b8d-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="02b8d-120">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="02b8d-120">Co-sell ready</span></span>|<span data-ttu-id="02b8d-121">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="02b8d-122">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="02b8d-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="02b8d-123">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="02b8d-123">Partner Center account</span></span>|<span data-ttu-id="02b8d-124">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="02b8d-125">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="02b8d-126">계정 관리</span><span class="sxs-lookup"><span data-stu-id="02b8d-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="02b8d-127">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="02b8d-127">Partner Center user roles</span></span>|<span data-ttu-id="02b8d-128">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="02b8d-129">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="02b8d-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="02b8d-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="02b8d-130">Salesforce CRM</span></span>|<span data-ttu-id="02b8d-131">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="02b8d-132">Salesforce CRM에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="02b8d-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="02b8d-133">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="02b8d-133">Power Automate Flow Account</span></span>|<span data-ttu-id="02b8d-134">CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정</span><span class="sxs-lookup"><span data-stu-id="02b8d-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="02b8d-135">사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="02b8d-136">Salesforce CRM에 대 한 파트너 센터 조회 동기화 설치</span><span class="sxs-lookup"><span data-stu-id="02b8d-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="02b8d-137">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="02b8d-138">그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="02b8d-139">오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="02b8d-140">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="02b8d-141">상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-141">Click on the **Open AppSource** link on the top menu.</span></span>

![AppSource 열기](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="02b8d-143">팝업 화면에서 **Salesforce에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

![Salesforce](images/salesforce/salesforce1.png)

6. <span data-ttu-id="02b8d-145">**지금 가져오기** 단추를 클릭 한 다음 **계속**합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-145">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="02b8d-146">그러면 Salesforce CRM 환경을 선택 하 여 응용 프로그램을 설치할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="02b8d-147">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-147">Agree to terms and conditions.</span></span>

![사용 가능한 CRMS](images/salesforce/available-crm.png)

8. <span data-ttu-id="02b8d-149">그런 다음 **솔루션 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="02b8d-150">페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="02b8d-151">파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="02b8d-152">설치는 10-15 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-152">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="02b8d-153">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="02b8d-154">**Salesforce에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="02b8d-155">**Salesforce에 대 한 파트너 센터 조회 동기화를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="02b8d-156">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-156">The following Power Automate flows and entities are available:</span></span>

![Salesforce 흐름](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="02b8d-158">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="02b8d-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="02b8d-159">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="02b8d-160">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="02b8d-161">솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="02b8d-162">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="02b8d-163">성공할 경우 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-163">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="02b8d-164">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="02b8d-164">Configure the solution</span></span>

1. <span data-ttu-id="02b8d-165">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="02b8d-166">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="02b8d-167">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-167">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="02b8d-168">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="02b8d-168">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="02b8d-169">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="02b8d-169">Partner Center Events</span></span>
- <span data-ttu-id="02b8d-170">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="02b8d-170">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="02b8d-171">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-171">a.</span></span> <span data-ttu-id="02b8d-172">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-172">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="02b8d-173">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-173">b.</span></span> <span data-ttu-id="02b8d-174">**연결 만들기**를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-174">Create a connection by clicking **Create a connection**.</span></span> 

    ![연결 만들기](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="02b8d-176">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-176">c.</span></span> <span data-ttu-id="02b8d-177">오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-177">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

    <span data-ttu-id="02b8d-178">d.</span><span class="sxs-lookup"><span data-stu-id="02b8d-178">d.</span></span> <span data-ttu-id="02b8d-179">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-179">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="02b8d-180">e.</span><span class="sxs-lookup"><span data-stu-id="02b8d-180">e.</span></span> <span data-ttu-id="02b8d-181">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-181">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>
    
    <span data-ttu-id="02b8d-182">f.</span><span class="sxs-lookup"><span data-stu-id="02b8d-182">f.</span></span> <span data-ttu-id="02b8d-183">CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-183">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="02b8d-184">전원 자동화 흐름을 연결과 연결 하려면 각 전원 자동화 흐름을 편집 하 여 Common Data Service 및 파트너 센터 조회에 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-184">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="02b8d-185">변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-185">Save the changes.</span></span>

5. <span data-ttu-id="02b8d-186">전원 자동화 흐름을 **켭니다** .</span><span class="sxs-lookup"><span data-stu-id="02b8d-186">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="02b8d-187">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="02b8d-187">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="02b8d-188">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-188">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="02b8d-189">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-189">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="02b8d-190">Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-190">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="02b8d-191">(A.)에 대 한 연결을 추가 합니다. 조회 관리자 자격 증명이 있는 파트너 센터 사용자 (b.) 아래 강조 표시 된 파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="02b8d-191">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![트리거](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="02b8d-193">이러한 업데이트를 만들면 다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-193">When you make these updates, you'll see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="02b8d-195">변경 내용을 저장 하 고 **켜기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-195">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="02b8d-196">파트너 센터 웹 후크가 이벤트 변경 내용을 수신 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-196">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="02b8d-197">**파트너 센터에서 SALESFORCE CRM (Insider preview)을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-197">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="02b8d-198">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-198">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="02b8d-199">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-199">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![URL 복사](images/salesforce/copy-url.png)

8. <span data-ttu-id="02b8d-201">이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-201">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="02b8d-202">오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-202">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="02b8d-203">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-203">Enter the following details:</span></span> 

    <span data-ttu-id="02b8d-204">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-204">a.</span></span> <span data-ttu-id="02b8d-205">**Http 트리거 끝점**: 이전 단계에서 복사한 URL</span><span class="sxs-lookup"><span data-stu-id="02b8d-205">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="02b8d-206">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-206">b.</span></span> <span data-ttu-id="02b8d-207">**등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"</span><span class="sxs-lookup"><span data-stu-id="02b8d-207">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="02b8d-208">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-208">c.</span></span> <span data-ttu-id="02b8d-209">**기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)</span><span class="sxs-lookup"><span data-stu-id="02b8d-209">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="02b8d-210">**실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="02b8d-210">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="02b8d-211">이제 웹 후크를 수신 대기 하 여 이벤트를 만들고 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-211">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="02b8d-212">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="02b8d-212">Customize synchronization steps</span></span>

<span data-ttu-id="02b8d-213">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-213">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="02b8d-214">CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-214">Often CRM systems are highly customized.</span></span> <span data-ttu-id="02b8d-215">전원 자동화 흐름을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-215">You can customize the Power Automate flows.</span></span> <span data-ttu-id="02b8d-216">필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-216">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="02b8d-217">CRM에 대 한 Microsoft 파트너 센터 매핑이 제공 되지만 CRM 환경에 따라 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-217">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="02b8d-218">각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-218">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="02b8d-219">사용 가능한 사용자 지정의 예는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-219">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="02b8d-220">파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-220">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="02b8d-221">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-221">a.</span></span> <span data-ttu-id="02b8d-222">파트너 센터에서 Salesforce CRM (Insider Preview)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-222">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

    <span data-ttu-id="02b8d-223">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-223">b.</span></span> <span data-ttu-id="02b8d-224">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-224">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="02b8d-225">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-225">c.</span></span> <span data-ttu-id="02b8d-226">선택 **(범위) 잠재 고객 또는 기회를 동기화**합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-226">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="02b8d-227">이벤트 만들기에 대 한 CRM 필드 매핑을 사용자 지정 하려면 **새 공유 기회 인지 여부**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-227">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="02b8d-228">**예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기**를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-228">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="02b8d-229">필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-229">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="02b8d-230">d.</span><span class="sxs-lookup"><span data-stu-id="02b8d-230">d.</span></span> <span data-ttu-id="02b8d-231">업데이트 이벤트에 대해 CRM 필드 매핑을 사용자 지정 하려면 "(범위) 잠재 고객 또는 기회 동기화" 단계를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-231">To customize CRM field mappings for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="02b8d-232">e.</span><span class="sxs-lookup"><span data-stu-id="02b8d-232">e.</span></span> <span data-ttu-id="02b8d-233">**기회를 업데이트 하는 경우를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-233">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="02b8d-234">**예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를**확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-234">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="02b8d-235">f.</span><span class="sxs-lookup"><span data-stu-id="02b8d-235">f.</span></span> <span data-ttu-id="02b8d-236">**예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-236">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="02b8d-237">업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:</span><span class="sxs-lookup"><span data-stu-id="02b8d-237">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="02b8d-238">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-238">a.</span></span> <span data-ttu-id="02b8d-239">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="02b8d-240">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-240">b.</span></span> <span data-ttu-id="02b8d-241">**기회 동기화를 선택 (범위)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-241">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="02b8d-242">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-242">c.</span></span> <span data-ttu-id="02b8d-243">업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-243">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="02b8d-244">d.</span><span class="sxs-lookup"><span data-stu-id="02b8d-244">d.</span></span> <span data-ttu-id="02b8d-245">**예 인 경우** 하위 단계를 선택 하 고 **기회 데이터가 포함 된 조회 업데이트**단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-245">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="02b8d-246">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-246">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="02b8d-247">만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면</span><span class="sxs-lookup"><span data-stu-id="02b8d-247">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="02b8d-248">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-248">a.</span></span> <span data-ttu-id="02b8d-249">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-249">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="02b8d-250">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-250">b.</span></span> <span data-ttu-id="02b8d-251">**조회 동기화를 선택 (범위) 합니다.**</span><span class="sxs-lookup"><span data-stu-id="02b8d-251">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="02b8d-252">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-252">c.</span></span> <span data-ttu-id="02b8d-253">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-253">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="02b8d-254">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="02b8d-255">Salesforce CRM 기회 레이아웃에서 별도의 섹션 만들기</span><span class="sxs-lookup"><span data-stu-id="02b8d-255">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="02b8d-256">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-256">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="02b8d-257">이를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유할 조회를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-257">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="02b8d-258">사용자 지정 필드 집합은 Salesforce CRM **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-258">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="02b8d-259">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="02b8d-260">Salesforce CRM 관리자 사용자는 별도의 CRM 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-260">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="02b8d-261">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-261">The following custom fields should be part of the CRM section:</span></span>

<span data-ttu-id="02b8d-262">• **파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="02b8d-262">• **Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

<span data-ttu-id="02b8d-263">• **조회 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="02b8d-263">• **Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

<span data-ttu-id="02b8d-264">• **조회 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="02b8d-264">• **Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

<span data-ttu-id="02b8d-265">• **Microsoft가 어떤 도움을 하나요?**</span><span class="sxs-lookup"><span data-stu-id="02b8d-265">• **How can Microsoft help?**</span></span> <span data-ttu-id="02b8d-266">Microsoft에서 조회에 필요한 도움말</span><span class="sxs-lookup"><span data-stu-id="02b8d-266">Help required from Microsoft for the referral</span></span>

<span data-ttu-id="02b8d-267">• **제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="02b8d-267">• **Products**: List of products associated with this opportunity</span></span>

<span data-ttu-id="02b8d-268">• **감사**: Microsoft 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="02b8d-268">• **Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="02b8d-269">필드 및 관계 설정</span><span class="sxs-lookup"><span data-stu-id="02b8d-269">Set up fields and relationships</span></span>

1. <span data-ttu-id="02b8d-270">Salesforce 계정에 로그인 하 고 **기회**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-270">Sign into your Salesforce account and go to **Opportunity**.</span></span> 

2. <span data-ttu-id="02b8d-271">**설정** 및 **개체 편집** 옵션을 클릭 하 여 필요한 필드를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-271">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>


3. <span data-ttu-id="02b8d-272">왼쪽 탐색에서 **필드 & 관계** 선택</span><span class="sxs-lookup"><span data-stu-id="02b8d-272">Select **Fields & Relationships** from the left navigation</span></span>

![필드](images/salesforce/fields1.png)

4. <span data-ttu-id="02b8d-274">"필드 & 관계" 테이블에 다음 필드를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-274">Add the following fields in the “Fields & Relationship” table:</span></span>

|<span data-ttu-id="02b8d-275">**필드 레이블**</span><span class="sxs-lookup"><span data-stu-id="02b8d-275">**Field label**</span></span>   |<span data-ttu-id="02b8d-276">**필드 이름**</span><span class="sxs-lookup"><span data-stu-id="02b8d-276">**Field name**</span></span>|<span data-ttu-id="02b8d-277">**데이터 형식**</span><span class="sxs-lookup"><span data-stu-id="02b8d-277">**Data type**</span></span>|<span data-ttu-id="02b8d-278">**인덱싱**</span><span class="sxs-lookup"><span data-stu-id="02b8d-278">**Indexed**</span></span>|
|---------------------|:-------------------|:--------------|:----------------|
|<span data-ttu-id="02b8d-279">파트너 센터와 동기화</span><span class="sxs-lookup"><span data-stu-id="02b8d-279">Sync with Partner Center</span></span>|<span data-ttu-id="02b8d-280">동기화-파트너 센터-c</span><span class="sxs-lookup"><span data-stu-id="02b8d-280">sync-with-partner-center-c</span></span>|<span data-ttu-id="02b8d-281">Checkbox (기본값 선택 하지 않음)</span><span class="sxs-lookup"><span data-stu-id="02b8d-281">Checkbox (default unchecked)</span></span>||
|<span data-ttu-id="02b8d-282">제품</span><span class="sxs-lookup"><span data-stu-id="02b8d-282">Products</span></span>|<span data-ttu-id="02b8d-283">제품-c</span><span class="sxs-lookup"><span data-stu-id="02b8d-283">Products-c</span></span>|<span data-ttu-id="02b8d-284">텍스트 (255)</span><span class="sxs-lookup"><span data-stu-id="02b8d-284">text (255)</span></span>||
|<span data-ttu-id="02b8d-285">조회</span><span class="sxs-lookup"><span data-stu-id="02b8d-285">Referral</span></span> | <span data-ttu-id="02b8d-286">Referral_Identifier__c</span><span class="sxs-lookup"><span data-stu-id="02b8d-286">Referral_Identifier__c</span></span>|<span data-ttu-id="02b8d-287">텍스트 (100) (외부 ID)</span><span class="sxs-lookup"><span data-stu-id="02b8d-287">Text(100)(External ID)</span></span>|<span data-ttu-id="02b8d-288">예</span><span class="sxs-lookup"><span data-stu-id="02b8d-288">yes</span></span>|
|<span data-ttu-id="02b8d-289">조회 링크</span><span class="sxs-lookup"><span data-stu-id="02b8d-289">Referral Link</span></span>| <span data-ttu-id="02b8d-290">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="02b8d-290">Referral_Link__c_</span></span>|<span data-ttu-id="02b8d-291">URL (255)</span><span class="sxs-lookup"><span data-stu-id="02b8d-291">URL(255)</span></span>||
|<span data-ttu-id="02b8d-292">감사</span><span class="sxs-lookup"><span data-stu-id="02b8d-292">Audit</span></span>| <span data-ttu-id="02b8d-293">Audit__c</span><span class="sxs-lookup"><span data-stu-id="02b8d-293">Audit__c</span></span>|<span data-ttu-id="02b8d-294">긴 텍스트 영역 (100000) (표시 되는 줄 4)</span><span class="sxs-lookup"><span data-stu-id="02b8d-294">Long Text Area(100000)(visible line 4)</span></span>||
|<span data-ttu-id="02b8d-295">Microsoft에서 어떤 도움을 하나요?</span><span class="sxs-lookup"><span data-stu-id="02b8d-295">How can Microsoft help?</span></span>|<span data-ttu-id="02b8d-296">How_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="02b8d-296">How_can_Microsoft_help__c</span></span>|<span data-ttu-id="02b8d-297">선택 목록</span><span class="sxs-lookup"><span data-stu-id="02b8d-297">Picklist\*</span></span>|

<span data-ttu-id="02b8d-298">\* 선택 목록 값:</span><span class="sxs-lookup"><span data-stu-id="02b8d-298">\*Picklist values:</span></span>

<span data-ttu-id="02b8d-299">• 워크 로드 별 가치 제안</span><span class="sxs-lookup"><span data-stu-id="02b8d-299">• Workload specific value proposition</span></span>

<span data-ttu-id="02b8d-300">• 고객 기술 아키텍처</span><span class="sxs-lookup"><span data-stu-id="02b8d-300">• Customer technical architecture</span></span>

<span data-ttu-id="02b8d-301">• 개념 증명 또는 데모</span><span class="sxs-lookup"><span data-stu-id="02b8d-301">• Proof of concept or demo</span></span>

<span data-ttu-id="02b8d-302">• 따옴표 또는 라이선스</span><span class="sxs-lookup"><span data-stu-id="02b8d-302">• Quotes or licensing</span></span>

<span data-ttu-id="02b8d-303">• 판매 고객 성공 후 성공</span><span class="sxs-lookup"><span data-stu-id="02b8d-303">• Post sales customer success</span></span>

<span data-ttu-id="02b8d-304">• 일반 또는 기타</span><span class="sxs-lookup"><span data-stu-id="02b8d-304">• General or other</span></span>

<span data-ttu-id="02b8d-305">5. "필드 & 관계"에서 필드가 생성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-305">5.The fields would get created under “Fields & Relationships”</span></span>

![만든 필드](images/salesforce/fields2.png)

6. <span data-ttu-id="02b8d-307">기회 레이아웃에서 위에 나열 된 필드를 사용 하 여 별도의 섹션을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-307">In the Opportunity layout, create a separate section with the fields as listed above.</span></span> 

    <span data-ttu-id="02b8d-308">•이 섹션은 기회 레이아웃의 판매자에 게 제공 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-308">• This section should be available for the sellers in the Opportunity layout</span></span>


![파트너 센터 필드 레이아웃](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="02b8d-310">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="02b8d-310">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="02b8d-311">전원 자동화 솔루션을 설치, 구성 및 사용자 지정한 후에는 Salesforce CRM과 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-311">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="02b8d-312">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="02b8d-312">Pre-requisites</span></span>

<span data-ttu-id="02b8d-313">파트너 센터 및 Salesforce CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-313">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="02b8d-314">이 id는 판매자 팀에 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-314">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="02b8d-315">사용자 지정 필드 집합은 Salesforce CRM 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-315">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="02b8d-316">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-316">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="02b8d-317">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-317">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="02b8d-318">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="02b8d-318">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="02b8d-319">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="02b8d-319">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="02b8d-320">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="02b8d-320">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="02b8d-321">Microsoft의 도움을 주는 **방법**: microsoft에서 조회에 필요한 도움말</span><span class="sxs-lookup"><span data-stu-id="02b8d-321">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="02b8d-322">**제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="02b8d-322">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="02b8d-323">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="02b8d-323">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="02b8d-324">에서는</span><span class="sxs-lookup"><span data-stu-id="02b8d-324">SCENARIOS:</span></span>

1. <span data-ttu-id="02b8d-325">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="02b8d-325">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="02b8d-326">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-326">a.</span></span> <span data-ttu-id="02b8d-327">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 Salesforce crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-327">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="02b8d-328">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-328">b.</span></span> <span data-ttu-id="02b8d-329">Salesforce CRM 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-329">Ensure that the following section is present when you create a “New Opportunity” in Salesforce CRM environment</span></span>

    ![Salesforce 환경](images/salesforce/salesforce-scenario-1.png)

   

    <span data-ttu-id="02b8d-331">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-331">c.</span></span> <span data-ttu-id="02b8d-332">이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-332">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="02b8d-333">"파트너 센터와 동기화": 예</span><span class="sxs-lookup"><span data-stu-id="02b8d-333">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="02b8d-334">"Microsoft의 도움을 주는 방법": 다음 옵션 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-334">"How can Microsoft help?”: Select from the following options:</span></span>

   

    - <span data-ttu-id="02b8d-335">제품: 제품의 솔루션 Id</span><span class="sxs-lookup"><span data-stu-id="02b8d-335">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="02b8d-336">d.</span><span class="sxs-lookup"><span data-stu-id="02b8d-336">d.</span></span> <span data-ttu-id="02b8d-337">**파트너 센터와의 동기화 기회 센터** 옵션을 **예**로 설정 했으면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-337">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="02b8d-338">조회가 Salesforce CRM과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-338">Your referrals will be synchronized with Salesforce CRM.</span></span>

    <span data-ttu-id="02b8d-339">e.</span><span class="sxs-lookup"><span data-stu-id="02b8d-339">e.</span></span> <span data-ttu-id="02b8d-340">"파트너 센터와 동기화" 옵션이 "예"로 설정 된 경우 Salesforce CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정과 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-340">When the “Sync with Partner Center” option is set to “Yes”, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

    <span data-ttu-id="02b8d-341">f.</span><span class="sxs-lookup"><span data-stu-id="02b8d-341">f.</span></span> <span data-ttu-id="02b8d-342">파트너 센터와 동기화 되는 기회는 Salesforce CRM에서 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-342">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="02b8d-343">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Salesforce CRM 환경에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="02b8d-343">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span> 

    <span data-ttu-id="02b8d-344">a.</span><span class="sxs-lookup"><span data-stu-id="02b8d-344">a.</span></span> <span data-ttu-id="02b8d-345">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-345">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="02b8d-346">b.</span><span class="sxs-lookup"><span data-stu-id="02b8d-346">b.</span></span> <span data-ttu-id="02b8d-347">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-347">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="02b8d-348">다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-348">c.</span></span> <span data-ttu-id="02b8d-349">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-349">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="02b8d-350">d.</span><span class="sxs-lookup"><span data-stu-id="02b8d-350">d.</span></span> <span data-ttu-id="02b8d-351">Salesforce CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-351">Sign into your Salesforce CRM environment.</span></span> 

    <span data-ttu-id="02b8d-352">e.</span><span class="sxs-lookup"><span data-stu-id="02b8d-352">e.</span></span> <span data-ttu-id="02b8d-353">**오픈 기회**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-353">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="02b8d-354">Microsoft Partner Center에서 만든 조회가 이제 Salesforce CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-354">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    ![Salesforce 기회 화면](images/salesforce/salesforce-casino-e.png)

    <span data-ttu-id="02b8d-356">f.</span><span class="sxs-lookup"><span data-stu-id="02b8d-356">f.</span></span> <span data-ttu-id="02b8d-357">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="02b8d-357">When you select a synchronized referral, the card view details are populated.</span></span>





## <a name="next-steps"></a><span data-ttu-id="02b8d-358">다음 단계</span><span class="sxs-lookup"><span data-stu-id="02b8d-358">Next steps</span></span>

- [<span data-ttu-id="02b8d-359">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="02b8d-359">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="02b8d-360">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="02b8d-360">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="02b8d-361">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="02b8d-361">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="02b8d-362">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="02b8d-362">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)