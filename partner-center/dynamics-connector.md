---
title: Dynamics 365 CRM 파트너 센터 용 공동 판매 커넥터
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dynamics 365 커넥터를 사용 하 여 Microsoft에서 조회를 가져옵니다.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: bddd29e9136d998ef8a25616d2058d1380b36665
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825690"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="3a81d-103">Dynamics 365 CRM 용 공동 판매 커넥터-개요</span><span class="sxs-lookup"><span data-stu-id="3a81d-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="3a81d-104">적절한 역할</span><span class="sxs-lookup"><span data-stu-id="3a81d-104">Appropriate roles</span></span>

- <span data-ttu-id="3a81d-105">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="3a81d-105">Referrals admin</span></span>
- <span data-ttu-id="3a81d-106">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="3a81d-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="3a81d-107">파트너 센터 공동 판매 커넥터를 통해 판매자는 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="3a81d-108">파트너 센터를 사용 하 여 공동 판매 거래를 관리 하도록 교육을 받을 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="3a81d-109">공동 판매 커넥터를 사용 하 여 microsoft 판매자와 협력 하 고, Microsoft 판매자 로부터 조회를 받고, 조회를 수락/거부 하 고, 거래 가치, 마감 날짜 등의 거래 데이터를 수정 하 고, 이러한 공동 판매 거래에 대 한 Microsoft 판매자의 업데이트를 받을 수 있는 새로운 공동 판매 참조를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="3a81d-110">파트너 센터가 아닌 선택한 CRM 내에서 작업 하는 동안이 모든 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="3a81d-111">이 솔루션은 Microsoft Power 자동화 솔루션을 기반으로 하며 Microsoft 파트너 센터 Api를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="3a81d-112">설치 전-필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="3a81d-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="3a81d-113">**토픽**</span><span class="sxs-lookup"><span data-stu-id="3a81d-113">**Topics**</span></span>   |<span data-ttu-id="3a81d-114">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="3a81d-114">**Details**</span></span>   |<span data-ttu-id="3a81d-115">**링크**</span><span class="sxs-lookup"><span data-stu-id="3a81d-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="3a81d-116">Microsoft 파트너 네트워크 ID</span><span class="sxs-lookup"><span data-stu-id="3a81d-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="3a81d-117">유효한 MPN ID가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-117">You need a valid MPN ID</span></span>|<span data-ttu-id="3a81d-118">[MPN](https://partner.microsoft.com/) 에 조인 하려면</span><span class="sxs-lookup"><span data-stu-id="3a81d-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="3a81d-119">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="3a81d-119">Co-sell ready</span></span>|<span data-ttu-id="3a81d-120">I p/서비스 솔루션은 공동 판매 준비를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="3a81d-121">Microsoft와 판매</span><span class="sxs-lookup"><span data-stu-id="3a81d-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="3a81d-122">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="3a81d-122">Partner Center account</span></span>|<span data-ttu-id="3a81d-123">파트너 센터 테 넌 트와 연결 된 MPN ID는 공동 판매 솔루션과 연결 된 MPN ID와 동일 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="3a81d-124">커넥터를 배포 하기 전에 파트너 센터 포털에서 공동 판매 조회를 확인할 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="3a81d-125">계정 관리</span><span class="sxs-lookup"><span data-stu-id="3a81d-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="3a81d-126">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="3a81d-126">Partner Center user roles</span></span>|<span data-ttu-id="3a81d-127">커넥터를 설치 하 고 사용 하는 직원은 조회 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="3a81d-128">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="3a81d-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="3a81d-129">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="3a81d-129">Dynamics 365 CRM</span></span>|<span data-ttu-id="3a81d-130">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="3a81d-131">Dynamics 365에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="3a81d-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="3a81d-132">전원 자동화 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="3a81d-132">Power Automate Flow Account</span></span>|<span data-ttu-id="3a81d-133">CRM 시스템 관리자 또는 시스템 사용자 지정자에 대 한 활성 [전원 자동화](https://flow.microsoft.com) 계정</span><span class="sxs-lookup"><span data-stu-id="3a81d-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="3a81d-134">사용자가 설치 하기 전에 최소 한 번 이상 [전원](https://flow.microsoft.com) 에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="3a81d-135">Dynamics 365에 대 한 파트너 센터 조회 동기화 설치 (전원 자동화 솔루션)</span><span class="sxs-lookup"><span data-stu-id="3a81d-135">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span> 

1. <span data-ttu-id="3a81d-136">[전원 자동화](https://flow.microsoft.com) 로 이동 하 고 오른쪽 상단 모서리에서 **환경** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="3a81d-137">그러면 사용 가능한 CRM 인스턴스가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="3a81d-138">오른쪽 상단 모서리의 드롭다운에서 적절 한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="3a81d-139">왼쪽 탐색 모음에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="3a81d-140">상단 메뉴에서 **AppSource 열기** 링크를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-140">Click on the **Open AppSource** link on the top menu.</span></span>

![AppSource 열기](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="3a81d-142">**Dynamics365에 대 한 파트너 센터 조회 커넥터** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-142">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="3a81d-143">**지금 가져오기** 단추를 클릭 한 다음 **계속**합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="3a81d-144">그러면 응용 프로그램을 설치할 CRM (Dynamics 365) 환경을 선택할 수 있는 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="3a81d-145">사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="3a81d-146">그런 다음 **솔루션 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="3a81d-147">페이지 아래쪽에 있는 화살표 단추를 사용 하 여 "파트너 센터 조회"로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="3a81d-148">파트너 센터 조회 솔루션 옆에 **설치 예정** 됨이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="3a81d-149">설치는 10-15 분 정도 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="3a81d-150">설치가 완료 되 면 [전원 자동화](https://flow.microsoft.com) 로 다시 이동 하 여 왼쪽 탐색 영역에서 **솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="3a81d-151">**Dynamics 365에 대 한 파트너 센터 조회 동기화** 는 솔루션 목록에서 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-151">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="3a81d-152">**Dynamics 365에 대 한 파트너 센터 조회 동기화를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="3a81d-153">다음과 같은 전원 자동화 흐름과 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-153">The following Power Automate flows and entities are available:</span></span>

![사용 가능한 CRMS](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="3a81d-155">모범 사례: 라이브 상태로 전환 하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="3a81d-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="3a81d-156">프로덕션 환경에서 전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하기 전에 스테이징 CRM 인스턴스에서 솔루션을 테스트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="3a81d-157">스테이징 환경/a p i 인스턴스에 Microsoft Power 자동화 솔루션을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="3a81d-158">솔루션의 복사본을 만들고, 스테이징 환경에서 구성 및 파워 자동화 흐름 사용자 지정을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="3a81d-159">스테이징/CRM 인스턴스에서 솔루션을 테스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="3a81d-160">성공할 경우 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="3a81d-161">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="3a81d-161">Configure the solution</span></span>

1. <span data-ttu-id="3a81d-162">CRM 인스턴스에 솔루션을 설치한 후에는 [전원 자동화](https://flow.microsoft.com/)로 다시 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="3a81d-163">오른쪽 상단 모서리의 **환경** 드롭다운에서 전원 자동화 솔루션을 설치한 CRM 인스턴스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="3a81d-164">세 가지 사용자 계정을 연결 하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="3a81d-165">조회 관리자 자격 증명이 있는 파트너 센터 사용자</span><span class="sxs-lookup"><span data-stu-id="3a81d-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="3a81d-166">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="3a81d-166">Partner Center Events</span></span>
- <span data-ttu-id="3a81d-167">솔루션에서 흐름을 자동화 하는 CRM admin</span><span class="sxs-lookup"><span data-stu-id="3a81d-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="3a81d-168">a.</span><span class="sxs-lookup"><span data-stu-id="3a81d-168">a.</span></span> <span data-ttu-id="3a81d-169">왼쪽 탐색 모음에서 **연결** 을 선택 하 고 목록에서 "파트너 센터 조회" 솔루션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="3a81d-170">b.</span><span class="sxs-lookup"><span data-stu-id="3a81d-170">b.</span></span> <span data-ttu-id="3a81d-171">**연결 만들기**를 클릭 하 여 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![연결 만들기](images/cosellconnectors/createconnection.png)
    
    <span data-ttu-id="3a81d-173">c.</span><span class="sxs-lookup"><span data-stu-id="3a81d-173">c.</span></span> <span data-ttu-id="3a81d-174">오른쪽 위 모서리의 검색 창에서 **파트너 센터 조회 (미리 보기)** 를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="3a81d-175">d.</span><span class="sxs-lookup"><span data-stu-id="3a81d-175">d.</span></span> <span data-ttu-id="3a81d-176">조회 관리자의 자격 증명 역할을 사용 하 여 파트너 센터 사용자에 대 한 연결을 만듭니다. 우표.</span><span class="sxs-lookup"><span data-stu-id="3a81d-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="3a81d-177">다음으로, 조회 관리자의 자격 증명을 사용 하 여 파트너 센터 사용자에 대 한 파트너 센터 이벤트 연결을 만듭니다. 350.</span><span class="sxs-lookup"><span data-stu-id="3a81d-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="3a81d-178">CRM 관리자 사용자에 대 한 Common Data Service (현재 환경)에 대 한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="3a81d-179">전원 자동화 흐름을 연결과 연결 하려면 각 전원 자동화 흐름을 편집 하 여 Common Data Service 및 파트너 센터 조회에 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="3a81d-180">변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="3a81d-180">Save the changes.</span></span>

5. <span data-ttu-id="3a81d-181">전원 자동화 흐름을 **켭니다** .</span><span class="sxs-lookup"><span data-stu-id="3a81d-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3a81d-182">다음 단계</span><span class="sxs-lookup"><span data-stu-id="3a81d-182">Next steps</span></span>

- [<span data-ttu-id="3a81d-183">웹 후크를 사용 하 여 리소스 변경 이벤트 가져오기</span><span class="sxs-lookup"><span data-stu-id="3a81d-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="3a81d-184">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="3a81d-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="3a81d-185">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="3a81d-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="3a81d-186">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="3a81d-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

