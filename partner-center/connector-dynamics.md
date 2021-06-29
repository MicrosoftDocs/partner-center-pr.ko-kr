---
title: Dynamics 365 CRM 파트너 센터 공동 판매 커넥터
description: 파트너 센터 조회를 Dynamics 365 CRM용 공동 판매 커넥터와 동기화합니다. 그런 다음 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 87083c8124762f0952b0c98cbc209164151dcb0c
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029195"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a><span data-ttu-id="fc08b-104">Dynamics 365 CRM용 공동 판매 커넥터 개요</span><span class="sxs-lookup"><span data-stu-id="fc08b-104">Co-sell connector for Dynamics 365 CRM overview</span></span>

<span data-ttu-id="fc08b-105">**적절한 역할:** 조회 관리자 | CRM의 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="fc08b-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="fc08b-106">파트너 센터 공동 판매 커넥터를 사용하면 판매자가 CRM 시스템 내에서 Microsoft와 공동 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-106">Partner Center co-sell connectors enable your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="fc08b-107">공동 판매 거래를 관리하는 데 파트너 센터 사용하도록 학습할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-107">They won't have to be trained to use Partner Center to manage co-sell deals.</span></span> <span data-ttu-id="fc08b-108">공동 판매 커넥터를 사용하여 새 공동 판매 추천을 만들어 Microsoft 판매자에게 참여시키고, Microsoft 판매자로부터 추천을 받고, 추천을 수락 또는 거부하고, 거래 가치 및 마감 날짜와 같은 거래 데이터를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-108">Use the co-sell connectors to create a new co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept or decline referrals, and modify deal data such as deal value and closing date.</span></span> <span data-ttu-id="fc08b-109">이러한 공동 판매 거래에 대한 Microsoft 판매자의 업데이트를 받을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-109">You can also receive any updates from the Microsoft sellers on these co-sell deals.</span></span> <span data-ttu-id="fc08b-110">모든 조회 작업은 파트너 센터 대신 선택한 CRM에서 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-110">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="fc08b-111">솔루션은 Power Automate 기반으로 하며 파트너 센터 API를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-111">The solution is based on Power Automate and uses Partner Center APIs.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc08b-112">필수 조건</span><span class="sxs-lookup"><span data-stu-id="fc08b-112">Prerequisites</span></span>

<span data-ttu-id="fc08b-113">솔루션을 설치하기 전에 다음 필수 구성을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-113">Before you install the solution, make sure to meet the following prerequisites.</span></span>

|<span data-ttu-id="fc08b-114">**토픽**</span><span class="sxs-lookup"><span data-stu-id="fc08b-114">**Topics**</span></span>   |<span data-ttu-id="fc08b-115">**세부 정보**</span><span class="sxs-lookup"><span data-stu-id="fc08b-115">**Details**</span></span>   |<span data-ttu-id="fc08b-116">**연결**</span><span class="sxs-lookup"><span data-stu-id="fc08b-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="fc08b-117">MPN(Microsoft 파트너 네트워크) ID</span><span class="sxs-lookup"><span data-stu-id="fc08b-117">Microsoft Partner Network (MPN) ID</span></span> |<span data-ttu-id="fc08b-118">유효한 MPN ID가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-118">You need a valid MPN ID.</span></span>|[<span data-ttu-id="fc08b-119">파트너 네트워크 가입</span><span class="sxs-lookup"><span data-stu-id="fc08b-119">Join the Partner Network</span></span>](https://partner.microsoft.com/)|
|<span data-ttu-id="fc08b-120">공동 판매 준비</span><span class="sxs-lookup"><span data-stu-id="fc08b-120">Co-sell ready</span></span>|<span data-ttu-id="fc08b-121">IP/서비스 솔루션은 공동 판매 준비가 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="fc08b-122">Microsoft로 판매</span><span class="sxs-lookup"><span data-stu-id="fc08b-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="fc08b-123">파트너 센터 계정</span><span class="sxs-lookup"><span data-stu-id="fc08b-123">Partner Center account</span></span>|<span data-ttu-id="fc08b-124">파트너 센터 테넌트와 연결된 MPN ID는 공동 판매 솔루션과 연결된 MPN ID와 동일해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your co-sell solution.</span></span> <span data-ttu-id="fc08b-125">커넥터를 배포하기 전에 파트너 센터 포털에서 공동 판매 추천을 볼 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-125">Verify that you can see your co-sell referrals in the Partner Center portal before you deploy the connectors.</span></span>|[<span data-ttu-id="fc08b-126">계정 관리</span><span class="sxs-lookup"><span data-stu-id="fc08b-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="fc08b-127">파트너 센터 사용자 역할</span><span class="sxs-lookup"><span data-stu-id="fc08b-127">Partner Center user roles</span></span>|<span data-ttu-id="fc08b-128">커넥터를 설치하고 사용할 직원은 조회 관리자여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-128">The employee who will install and use the connectors must be a Referrals admin.</span></span>|[<span data-ttu-id="fc08b-129">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="fc08b-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="fc08b-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="fc08b-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="fc08b-131">CRM 사용자 역할은 시스템 관리자 또는 시스템 사용자 지정자입니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-131">The CRM user role is System admin or System customizer.</span></span>|[<span data-ttu-id="fc08b-132">Dynamics 365에서 역할 할당</span><span class="sxs-lookup"><span data-stu-id="fc08b-132">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="fc08b-133">Power Automate 흐름 계정</span><span class="sxs-lookup"><span data-stu-id="fc08b-133">Power Automate flow account</span></span>|<span data-ttu-id="fc08b-134">테스트, 스테이징 및 프로덕션을 위한 데이터베이스를 사용하여 새 프로덕션 환경을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-134">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="fc08b-135">데이터베이스가 있는 기존 프로덕션 환경이 있는 경우 다시 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-135">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="fc08b-136">커넥터 솔루션을 설치하려는 사용자에게는 Power Automate 라이선스와 이 환경에 대한 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-136">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="fc08b-137">설치가 실패하면 진행 상황을 모니터링하고 [Power Automate](https://flow.microsoft.com/) 자세한 정보를 얻을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-137">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="fc08b-138">솔루션 에서 **기록 보기를** **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="fc08b-138">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="fc08b-139">환경 만들기 또는 관리</span><span class="sxs-lookup"><span data-stu-id="fc08b-139">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="fc08b-140">dynamics 365용 파트너 센터 조회 동기화 설치(Power Automate 솔루션)</span><span class="sxs-lookup"><span data-stu-id="fc08b-140">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate solution)</span></span>

1. <span data-ttu-id="fc08b-141">[Power Automate](https://flow.microsoft.com)로 이동하고 오른쪽 위 모서리에서 **환경을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-141">Go to [Power Automate](https://flow.microsoft.com), and select **Environments** in the upper-right corner.</span></span> <span data-ttu-id="fc08b-142">이 단계에서는 사용 가능한 CRM 인스턴스를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-142">This step will show you the available CRM instances.</span></span>

1. <span data-ttu-id="fc08b-143">오른쪽 위 모서리의 드롭다운 목록에서 적절한 CRM 인스턴스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-143">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="fc08b-144">왼쪽에서 **솔루션을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-144">Select **Solutions** on the left.</span></span>

1. <span data-ttu-id="fc08b-145">위쪽 메뉴에서 **AppSource 열기** 링크를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-145">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="AppSource 열기를 보여 주는 스크린샷":::

1. <span data-ttu-id="fc08b-147">팝업 화면에서 **dynamics 365용 파트너 센터 조회 커넥터를** 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-147">Search for **Partner Center Referrals Connectors for Dynamics 365** in the pop-up screen.</span></span>  

1. <span data-ttu-id="fc08b-148">지금 **받기** 단추를 선택한 다음, **계속을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-148">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="fc08b-149">CRM(Dynamics 365) 환경을 선택하여 애플리케이션을 설치할 수 있는 페이지가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-149">A page appears where you can select the CRM (Dynamics 365) environment to install the application.</span></span> <span data-ttu-id="fc08b-150">약관에 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-150">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="fc08b-151">진행 상황을 모니터링할 수 있으며 설치에 실패하는 경우 솔루션 아래에서 기록 **보기를** 선택하여 Power Automate 자세한 내용을 확인할 수 **있습니다.**</span><span class="sxs-lookup"><span data-stu-id="fc08b-151">You can monitor the progress and, if the installation fails, you can get more details in Power Automate by selecting **See history** under **Solutions**.</span></span>

1. <span data-ttu-id="fc08b-152">설치가 완료되면 [Power Automate](https://flow.microsoft.com) 돌아가서 왼쪽에서 **솔루션을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-152">After the installation is complete, go back to [Power Automate](https://flow.microsoft.com) and select **Solutions** on the left.</span></span> <span data-ttu-id="fc08b-153">이제 솔루션 목록에서 **Dynamics 365에 대한 파트너 센터 조회 동기화를** 사용할 수 **있습니다.**</span><span class="sxs-lookup"><span data-stu-id="fc08b-153">**Partner Center Referrals Synchronization for Dynamics 365** is now available in the **Solutions** list.</span></span>

1. <span data-ttu-id="fc08b-154">**Dynamics 365에 대한 파트너 센터 조회 동기화를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="fc08b-155">다음 Power Automate 흐름 및 엔터티를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-155">The following Power Automate flows and entities are available.</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="사용 가능한 CRM을 보여 주는 스크린샷":::

## <a name="test-before-you-go-live"></a><span data-ttu-id="fc08b-157">라이브로 진행하기 전에 테스트</span><span class="sxs-lookup"><span data-stu-id="fc08b-157">Test before you go live</span></span>

<span data-ttu-id="fc08b-158">프로덕션 환경에서 Power Automate 솔루션을 설치, 구성 및 사용자 지정하기 전에 준비 CRM 인스턴스에서 솔루션을 테스트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span> <span data-ttu-id="fc08b-159">다음 작업이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-159">You'll need to:</span></span>

- <span data-ttu-id="fc08b-160">스테이징 환경 CRM 인스턴스에 Power Automate 솔루션을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-160">Install the Power Automate solution on a staging environment CRM instance.</span></span>
- <span data-ttu-id="fc08b-161">스테이징 환경에서 Power Automate 솔루션을 구성하고 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-161">Configure and customize the Power Automate solution in a staging environment.</span></span>
- <span data-ttu-id="fc08b-162">스테이징 CRM 인스턴스에서 솔루션을 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-162">Test the solution on a staging CRM instance.</span></span>
- <span data-ttu-id="fc08b-163">테스트가 성공하면 프로덕션 인스턴스에 관리형 솔루션으로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-163">After a successful test, import as a managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="fc08b-164">솔루션 구성</span><span class="sxs-lookup"><span data-stu-id="fc08b-164">Configure the solution</span></span>

1. <span data-ttu-id="fc08b-165">CRM 인스턴스에 솔루션을 설치한 후 [Power Automate](https://flow.microsoft.com/)으로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-165">After you've installed the solution in your CRM instance, go back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="fc08b-166">오른쪽 위 모서리의 **환경** 드롭다운 목록에서 Power Automate 솔루션을 설치한 CRM 인스턴스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-166">From the **Environments** drop-down list in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="fc08b-167">세 개의 사용자 계정을 연결하는 연결을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-167">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="fc08b-168">조회 관리자 자격 증명을 사용하여 사용자 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="fc08b-168">Partner Center user with Referrals admin credentials</span></span>
   - <span data-ttu-id="fc08b-169">파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="fc08b-169">Partner Center Events</span></span>
   - <span data-ttu-id="fc08b-170">솔루션에서 Power Automate 흐름을 가진 CRM 관리자</span><span class="sxs-lookup"><span data-stu-id="fc08b-170">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="fc08b-171">왼쪽에서 **연결을** 선택하고 목록에서 **파트너 센터 조회** 솔루션을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-171">Select **Connections** on the left, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="fc08b-172">연결 만들기를 선택하여 **연결을 만듭니다.**</span><span class="sxs-lookup"><span data-stu-id="fc08b-172">Create a connection by selecting **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="연결 만들기를 보여 주는 스크린샷.":::

   1. <span data-ttu-id="fc08b-174">오른쪽 위 모서리의 검색 표시줄에서 **파트너 센터 조회(미리 보기)를** 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-174">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="fc08b-175">조회 관리자의 자격 증명 역할을 사용하여 파트너 센터 사용자에 대한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="fc08b-176">다음으로, 조회 관리자 자격 증명을 사용하여 파트너 센터 사용자에 대한 파트너 센터 이벤트 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-176">Next, create a Partner Center Events connection for your Partner Center user with the Referrals admin credentials.</span></span>

   1. <span data-ttu-id="fc08b-177">CRM 관리자 사용자에 대한 Common Data Service(현재 환경)에 대한 연결을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
   1. <span data-ttu-id="fc08b-178">모든 연결을 추가한 후에는 사용자 환경에서 다음 연결이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-178">After you've added all the connections, you should see the following connections in your environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="연결을 보여 주는 스크린샷":::

## <a name="edit-the-connections"></a><span data-ttu-id="fc08b-180">연결 편집</span><span class="sxs-lookup"><span data-stu-id="fc08b-180">Edit the connections</span></span>

1. <span data-ttu-id="fc08b-181">**솔루션** 페이지로 돌아가서 **기본 솔루션** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-181">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="fc08b-182">**모든** 를 선택하여 **연결 참조(미리 보기)를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-182">Select **Connection Reference (preview)** by selecting **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="연결 편집을 보여 주는 스크린샷":::

1. <span data-ttu-id="fc08b-184">말줄임표 아이콘을 선택하여 각 연결을 개별적으로 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-184">Edit each of the connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="fc08b-185">관련 연결을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-185">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="나열된 연결을 보여 주는 스크린샷.":::

1. <span data-ttu-id="fc08b-187">**솔루션** 페이지로 돌아가서 **dynamics 365에 대한 파트너 센터 조회 동기화를** 선택하고 다음 시퀀스의 각 흐름 옆에 있는 말줄임표 아이콘을 선택하여 흐름을 켭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-187">Return to the **Solutions** page, select **Partner Center Referrals Synchronization for Dynamics 365**, and turn on the flow by selecting the ellipsis icon next to each flow in the following sequence.</span></span> <span data-ttu-id="fc08b-188">흐름을 설정하는 동안 문제가 발생하는 경우 [사용자 지정 단계](connector-dynamics.md#customize-synchronization-steps) 및 문제 해결 단계를 [참조하세요.](connectors-troubleshoot.md)</span><span class="sxs-lookup"><span data-stu-id="fc08b-188">If you encounter any issues while you turn on the flow, see [Customization steps](connector-dynamics.md#customize-synchronization-steps) and [Troubleshooting steps](connectors-troubleshoot.md).</span></span>

<span data-ttu-id="fc08b-189">다음 순서로 흐름을 켭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-189">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="fc08b-190">파트너 센터 Webhook 등록(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-190">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-191">공동 판매 조회 만들기 – Dynamics 365 to 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-191">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-192">[사용자 지정] Dynamics 365 흐름에서 세부 정보 만들기 또는 얻기</span><span class="sxs-lookup"><span data-stu-id="fc08b-192">[Customize] Create or Get Details from Dynamics 365 flow</span></span>
- <span data-ttu-id="fc08b-193">Dynamics 365 - Helper에 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-193">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-194">Dynamics 365에 대한 Microsoft 공동 판매 조회 업데이트 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-194">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-195">Dynamics 365로 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-195">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-196">Dynamics 365 to 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-196">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-197">Dynamics 365 파트너 센터 기회(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-197">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="fc08b-198">Dynamics 365 Microsoft Solutions to 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="fc08b-198">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="fc08b-199">webhook API를 사용하여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="fc08b-199">Use webhook APIs to register for resource change events</span></span>

<span data-ttu-id="fc08b-200">파트너 센터 webhook API를 사용하여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-200">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="fc08b-201">이러한 변경 이벤트는 HTTP 게시로 URL에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-201">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="fc08b-202">**파트너 센터에서 Dynamics 365 (Insider preview)을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-202">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

1. <span data-ttu-id="fc08b-203">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-203">Select the **Edit** icon, and select **When a HTTP request is received**.</span></span>

1. <span data-ttu-id="fc08b-204">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-204">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/webhook-video.gif" alt-text="웹 후크를 사용 하 여 리소스 변경 내용을 등록 하는 방법을 보여 주는 스크린샷":::

1. <span data-ttu-id="fc08b-206">**파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 하 고 **실행** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-206">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="fc08b-207">오른쪽 창에서 **흐름 실행** 창이 열려 있는지 확인 하 고 **계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-207">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="fc08b-208">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-208">Enter the following details:</span></span>

   - <span data-ttu-id="fc08b-209">**Http 트리거 끝점**:이 URL은 이전 단계에서 복사 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-209">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="fc08b-210">**등록할 이벤트**: 사용 가능한 모든 이벤트 (**조회 생성**, **조회-업데이트**, **관련-조회 생성** 및 **관련 조회-업데이트 됨**)를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-210">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="fc08b-211">**기존 트리거 끝점이 있으면 덮어쓰시겠습니까?**: 예.</span><span class="sxs-lookup"><span data-stu-id="fc08b-211">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="fc08b-212">지정 된 webhook 이벤트에 대해 하나의 URL만 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-212">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="fc08b-213">**흐름 실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="fc08b-213">Select **Run flow**, and then select **Done.**</span></span>

<span data-ttu-id="fc08b-214">이제 웹 후크는 이벤트를 수신 하 고, 만들고, 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-214">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="fc08b-215">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="fc08b-215">Customize synchronization steps</span></span>

<span data-ttu-id="fc08b-216">CRM 시스템은 고도로 사용자 지정 되며 CRM 설정에 따라 전원 자동화 솔루션을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-216">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="fc08b-217">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 [사용자 지정 필드 매핑 가이드](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-217">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="fc08b-218">필드 매핑 가이드에 따라 필요한 경우 [사용자 지정]에서 적절 하 게 변경 하 여 **Dynamics 365 flow 또는 환경 변수에서 세부 정보를 만들거나 가져옵니다** .</span><span class="sxs-lookup"><span data-stu-id="fc08b-218">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow** or environment variables.</span></span> <span data-ttu-id="fc08b-219">이후 솔루션 업그레이드에 영향을 줄 수 있으므로 전원 자동화 솔루션에서 다른 흐름을 업데이트 하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="fc08b-219">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="fc08b-220">다음 사용자 지정을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-220">The following customizations are available:</span></span>

- <span data-ttu-id="fc08b-221">**기회 이름에 확인 표시 표시**: 기본적으로 파트너 센터와 DYNAMICS 365 CRM 간의 동기화가 성공적으로 수행 되 고 있음을 나타내기 위해 기회 이름 옆에 확인 표시가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-221">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="fc08b-222">마찬가지로 동기화가 실패할 경우 십자 표시가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-222">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="fc08b-223">기회 이름에 check 또는 cross mark를 추가 하지 않으려면 **기회 이름 환경 변수에서 표시 확인 표시** 의 현재 값을 아니요로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-223">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>
- <span data-ttu-id="fc08b-224">**거래 값**: 기본적으로 파트너 센터의 거래 값은 CRM의 **estimatedvalue** 와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-224">**Deal value**: By default, the deal value from Partner Center will be synced to and from **estimatedvalue** in the CRM.</span></span> <span data-ttu-id="fc08b-225">CRM에서 동기화 할 거래 값에 다른 필드가 있는 경우:</span><span class="sxs-lookup"><span data-stu-id="fc08b-225">If you have a different field in the CRM for the deal value to sync from:</span></span>

  - <span data-ttu-id="fc08b-226">Dynamics 365 환경 변수의 **거래 값** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-226">Update the **Deal value** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="fc08b-227">표시 이름이 아니라 필드 이름을 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-227">Make sure that you provide the field's name, not its display name.</span></span>
  - <span data-ttu-id="fc08b-228">**[사용자 지정] 편집 [사용자 지정] Dynamics 365 flow에서 세부 정보를 만들거나** 업데이트 하 고, Crm에서 **만들기 또는 업데이트 기회** 로 이동 하 고, **새 기회 만들기** 및 업데이트 **기존 기회** 작업을 업데이트 하 여 **DealValue** 값을 crm의 올바른 필드에 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or update opportunity** in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** value to the correct field in the CRM.</span></span> <span data-ttu-id="fc08b-229">또한 **예상 수익** 필드에서 **DealValue** 할당을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-229">Also, remove the **DealValue** assignment from the **Estimated Revenue** field.</span></span>

- <span data-ttu-id="fc08b-230">**고객 계정 국가 코드**: 새 조회를 만들 때 두 문자로 된 국가 코드 (ISO 3166)를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-230">**Customer Account Country Code**: It's mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="fc08b-231">기본적으로 국가 코드는 CRM의 계정 **address1_country** 필드와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-231">By default, the country code will be synced to and from the account's **address1_country** field in the CRM.</span></span> <span data-ttu-id="fc08b-232">CRM에서 동기화 할 국가 코드에 대 한 다른 필드가 있는 경우:</span><span class="sxs-lookup"><span data-stu-id="fc08b-232">If you have a different field in the CRM for the country code to sync from:</span></span>

  - <span data-ttu-id="fc08b-233">두 문자로 된 코드를 포함 하는 계정에 있는 비 조회 국가 코드 필드:</span><span class="sxs-lookup"><span data-stu-id="fc08b-233">For a nonlookup country code field in the account that contains a two-letter code:</span></span>
    - <span data-ttu-id="fc08b-234">Dynamics 365 환경 변수의 **고객 계정 국가 코드** 필드 이름을 CRM의 필드 이름으로 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-234">Update the **Customer Account Country Code** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="fc08b-235">표시 이름이 아니라 필드 이름을 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-235">Make sure that you provide the field's name, not its display name.</span></span>
    - <span data-ttu-id="fc08b-236">편집 **[사용자 지정] Dynamics 365 flow에서 세부 정보를 만들거나 가져온** 다음 crm 작업에서 **고객 계정 만들기 또는 가져오기** 로 이동 하 여 crm의 올바른 필드에 **국가** 값을 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-236">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or get customer account** in the CRM action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="fc08b-237">또한 **Address 1: country/region** 필드에서 **country** value 할당을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-237">Also, remove the **Country** value assignment from the **Address 1: Country/Region** field.</span></span>

  - <span data-ttu-id="fc08b-238">계정에서 조회 기반 국가 코드 필드:</span><span class="sxs-lookup"><span data-stu-id="fc08b-238">For a lookup-based country code field in the account:</span></span>
    - <span data-ttu-id="fc08b-239">계정에 새 사용자 지정 필드를 추가 하 고 조회 기반 필드에서 선택한 값을 기준으로 두 자로 된 국가 코드 (ISO 3166)로 자동으로 채우거 나 그 반대의 경우도 마찬가지입니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-239">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>
    - <span data-ttu-id="fc08b-240">비 조회 국가 코드 필드에 대해 앞의 단계를 수행 하 여 CRM과 파트너 센터 간에 새 사용자 지정 필드를 동기화 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-240">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="fc08b-241">**기회 필드**: 채워야 하는 **기회** 에 필수 필드가 있는 경우 **[사용자 지정]을 편집 하 여 Dynamics 365 Flow에서 세부 정보를 만들거나** 확인 하 고 CRM에서 **만들기 또는 업데이트 기회** 로 이동 및 업데이트 비즈니스 요구 사항에 따라 필수 필드에 값을 할당 하는 **새 기회 작업을 만듭니다** .</span><span class="sxs-lookup"><span data-stu-id="fc08b-241">**Opportunity fields**: If there are mandatory fields in **Opportunity** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update opportunity** in the CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="fc08b-242">**잠재 고객 필드**: 채워야 하는 **선행** 의 필수 필드가 있는 경우 [사용자 지정]을 편집 하 여 **Dynamics 365 Flow에서 세부 정보를 만들거나** 업데이트 하 고, CRM에서 **잠재 고객을 만들거나** 업데이트 하 고, 비즈니스 요구 사항에 따라 필수 필드에 값을 할당 하는 **새 잠재 고객 작업을 만듭니다** .</span><span class="sxs-lookup"><span data-stu-id="fc08b-242">**Lead fields**: If there are mandatory fields in **Lead** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update lead** in the CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="fc08b-243">**고객 계정**: 파트너 센터에서 crm으로 새 조회를 동기화 할 경우, 전원 자동화 솔루션은 고객 회사 이름 및 우편 번호를 사용 하 여 CRM에서 기존 계정을 검색 하려고 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-243">**Customer account**: When a new referral is synced from Partner Center to the CRM, the Power Automate solution tries to search for an existing account in the CRM by using the customer company name and postal code.</span></span> <span data-ttu-id="fc08b-244">하나를 찾지 못하면 CRM에 새 고객 계정이 생성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-244">If it doesn't find one, a new customer account will be created in the CRM.</span></span> <span data-ttu-id="fc08b-245">검색 조건 및 새 계정 만들기 정보를 업데이트 하려면 **[사용자 지정]을 편집 하 여 Dynamics 365 flow에서 세부 정보를 만들거나 가져온** 다음 CRM에서 고객 **계정 만들기 또는 가져오기** 및 **고객 계정 만들기 작업** 으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-245">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or get customer account** in the CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="fc08b-246">환경 변수 업데이트</span><span class="sxs-lookup"><span data-stu-id="fc08b-246">Update environment variable</span></span>

<span data-ttu-id="fc08b-247">환경 변수 값을 업데이트 하려면:</span><span class="sxs-lookup"><span data-stu-id="fc08b-247">To update an environment variable value:</span></span>

1. <span data-ttu-id="fc08b-248">**솔루션** 페이지로 이동 하 여 **기본 솔루션** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-248">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="fc08b-249">**모두** 를 선택 하 여 **환경 변수** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-249">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="fc08b-250">업데이트 해야 하는 값에 대 한 환경 변수를 선택 하 고 줄임표 아이콘을 사용 하 여 **편집** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-250">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="fc08b-251">**새 값** 옵션을 사용 하 고 값을 제공 하 여 **현재 값** 을 업데이트 합니다 ( **기본값** 업데이트 안 함).</span><span class="sxs-lookup"><span data-stu-id="fc08b-251">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="fc08b-252">값은 변수의 데이터 형식과 일치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-252">The value must match the data type of the variable.</span></span> <span data-ttu-id="fc08b-253">예를 들어 예 또는 아니요 데이터 형식은 예 또는 아니요 값을 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-253">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="환경 변수 업데이트를 보여 주는 스크린샷":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a><span data-ttu-id="fc08b-255">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="fc08b-255">End-to-end bidirectional co-sell referral synchronization</span></span>

<span data-ttu-id="fc08b-256">전원 자동화 솔루션을 설치, 구성 및 사용자 지정한 후 Dynamics 365 및 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-256">After you've installed, configured, and customized the Power Automate solution, you can test for co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="fc08b-257">필수 조건</span><span class="sxs-lookup"><span data-stu-id="fc08b-257">Prerequisites</span></span>

<span data-ttu-id="fc08b-258">파트너 센터 및 Dynamics 365 CRM에서 조회를 동기화 하기 위해 전원 자동화 솔루션은 Microsoft 전용 조회 필드를 명확 하 게 정하는 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-258">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="fc08b-259">이 id는 판매자 팀이 공동 판매를 위해 Microsoft와 공유할 조회를 결정 하는 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-259">This identification gives your seller teams the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="fc08b-260">솔루션 설치의 일부로 사용자 지정 필드 및 개체 집합이 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-260">A set of custom fields and objects will be added as part of the solution installation.</span></span> <span data-ttu-id="fc08b-261">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-261">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="fc08b-262">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-262">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="fc08b-263">**파트너 센터와 동기화**: 파트너 센터와 기회를 동기화할지 여부를 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-263">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="fc08b-264">기본적으로이 필드의 값은 아니요 이며 판매자가 Microsoft와의 기회를 공유 하도록 명시적으로 예로 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-264">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="fc08b-265">파트너 센터에서 CRM으로 공유 되는 새 조회는이 필드 값을 예로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-265">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>
- <span data-ttu-id="fc08b-266">**조회 식별자**: 파트너 센터 조회에 대 한 읽기 전용 식별자 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-266">**Referral Identifier**: A read-only identifier field for the Partner Center referral.</span></span>
- <span data-ttu-id="fc08b-267">**조회 링크**: 파트너 센터에서 조회에 대 한 읽기 전용 링크입니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-267">**Referral Link**: A read-only link to the referral in Partner Center.</span></span>
- <span data-ttu-id="fc08b-268">**Microsoft에서 microsoft에 어떤 도움을 주는 것이 있나요?**: microsoft에서 조회에 대해 도움을 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-268">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="fc08b-269">공동 판매 조회를 만들려면 Microsoft에서 필요한 적절 한 도움말을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-269">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="fc08b-270">고객 연락처를 공동 판매 참조를 만들 수 있는 기회에 연결 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-270">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="fc08b-271">비 공동 판매 조회를 만들려면이 필드를 선택 하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="fc08b-271">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="fc08b-272">비 공동 판매 조회는 적절 한 도움말-필수 옵션을 선택 하 여 언제 든 지 공동 판매 조회로 변환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-272">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>
- <span data-ttu-id="fc08b-273">**Microsoft 파트너 센터 조회 표시 유형**: 파트너 센터 조회에 대 한 표시 유형을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-273">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="fc08b-274">Microsoft 판매자에 게 표시 하면 비 공동 판매 조회가 공동 판매로 전환 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-274">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="fc08b-275">Microsoft 도움말이 필요한 경우 기본적으로 Microsoft 판매자에 게 조회를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-275">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="fc08b-276">이 필드가 표시 된 것으로 표시 된 후에는 되돌릴 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-276">After this field is marked as visible, it can't be reverted.</span></span>
- <span data-ttu-id="fc08b-277">**MICROSOFT CRM identifier**: 공동 판매 조회가 microsoft에서 만들어지고 수락 되는 경우이 필드는 MICROSOFT의 CRM 식별자로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-277">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>
- <span data-ttu-id="fc08b-278">**제품: 사용 되지** 않음:이 필드를 사용 하지 않거나 CRM 섹션에 추가 하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="fc08b-278">**Products: Obsolete**: Don't use this field or add it to the CRM section.</span></span> <span data-ttu-id="fc08b-279">이전 버전과의 호환성을 위해서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-279">It's available for backward compatibility only.</span></span> <span data-ttu-id="fc08b-280">파트너 센터 솔루션을 대신 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-280">Use Partner Center solutions instead.</span></span>
- <span data-ttu-id="fc08b-281">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역입니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals.</span></span>
- <span data-ttu-id="fc08b-282">**Microsoft 파트너 센터 솔루션**: 공동 판매 준비 된 솔루션 또는 Microsoft 솔루션을 기회와 연결 하는 사용자 지정 개체입니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-282">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="fc08b-283">하나 이상의 솔루션을 기회에서 추가 하거나 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-283">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="fc08b-284">Microsoft와 공유 하기 전에 하나 이상의 공동 판매 준비 또는 Microsoft 솔루션을 기회에 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-284">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="fc08b-285">이 개체를 기회에 연결 하려면 CRM에서 **기회** 양식을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-285">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

  <span data-ttu-id="fc08b-286">**기회** 양식에서 적절 한 탭을 선택 하 고 여기에 표시 된 대로 subgrid를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-286">Select the appropriate tab on the **Opportunity** form, and add a subgrid as shown here.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="기회 양식을 보여 주는 스크린샷":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft 솔루션을 보여 주는 스크린샷":::

- <span data-ttu-id="fc08b-289">Microsoft 솔루션을 추가한 후에 판매자가 추가할 필요가 없도록 공동 판매 준비 솔루션 세부 정보를 미리 채울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-289">After you add Microsoft solutions, you can prepopulate co-sell ready solution details so that your sellers don't have to add them.</span></span> <span data-ttu-id="fc08b-290">새 솔루션 세부 정보를 추가 하려면 CRM의 Microsoft Solution Details 개체로 이동 하 고 **레코드 추가** 를 선택 하 여 항목을 하나 추가 하거나 **Excel 업로드** 를 사용 하 여 여러 항목을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-290">To add a new solution detail, go to the Microsoft Solution Details object in the CRM and select **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="새로운 Microsoft 솔루션 세부 정보를 보여 주는 스크린샷":::

### <a name="scenarios"></a><span data-ttu-id="fc08b-292">시나리오</span><span class="sxs-lookup"><span data-stu-id="fc08b-292">Scenarios</span></span>

1. <span data-ttu-id="fc08b-293">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="fc08b-293">Referral synchronization when referral is created or updated in the CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="fc08b-294">CRM의 **기회** 섹션에 표시 되는 사용자를 사용 하 여 DYNAMICS 365 CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-294">Sign in to your Dynamics 365 CRM environment with the user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="fc08b-295">Dynamics 365 환경에서 새로운 기회를 만들 때 **Microsoft 파트너 센터** 섹션이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-295">Ensure that the **Microsoft Partner Center** section is present when you create a new opportunity in the Dynamics 365 environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="새 기회를 보여 주는 스크린샷":::

   1. <span data-ttu-id="fc08b-297">파트너 센터와이 기회를 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="fc08b-298">**Microsoft에서 어떻게 도울 수 있나요?**: 공동 판매 조회를 만들려면 적절 한 도움말 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-298">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="카드 보기에서 적절 한 필드를 가져오는 방법을 보여 주는 스크린샷":::

      - <span data-ttu-id="fc08b-300">**고객 연락처**: 공동 판매 리퍼럴을 만들려면 기회에 고객 연락처를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-300">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="fc08b-301">**파트너 센터와 동기화**: 예.</span><span class="sxs-lookup"><span data-stu-id="fc08b-301">**Sync With Partner Center**: Yes.</span></span>
      - <span data-ttu-id="fc08b-302">**Microsoft 솔루션**: microsoft와의 조회를 공유 하려면 올바른 공동 판매 준비 또는 microsoft 솔루션을 기회에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-302">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="솔루션 ID를 보여 주는 스크린샷":::

   1. <span data-ttu-id="fc08b-304">**파트너 센터에 동기화** 옵션을 예로 설정 하 여 Dynamics 365에서 기회가 생성 된 후 10 분 정도 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-304">After the opportunity is created in Dynamics 365 with the **Sync With Partner Center** option set to Yes, wait 10 minutes.</span></span> <span data-ttu-id="fc08b-305">파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-305">Then sign in to your Partner Center account.</span></span> <span data-ttu-id="fc08b-306">사용자의 조회가 Dynamics 365 및 **조회 식별자** 와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-306">Your referrals will be synchronized with Dynamics 365 and **Referral Identifier**.</span></span> <span data-ttu-id="fc08b-307">**조회 링크** 를 채웁니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-307">**Referral Link** will get populated.</span></span> <span data-ttu-id="fc08b-308">오류가 있으면 **감사** 필드가 오류 정보로 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-308">If there's a failure, the **Audit** field will be populated with error information.</span></span>

      1. <span data-ttu-id="fc08b-309">마찬가지로, **파트너 센터와 동기화** 옵션을 예로 설정 하는 기회에 대해 DYNAMICS 365 CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-309">Likewise, for an opportunity that had the **Sync With Partner Center** option set to Yes, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

      1. <span data-ttu-id="fc08b-310">파트너 센터와 성공적으로 동기화 되는 기회는 Dynamics 365의 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-310">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

1. <span data-ttu-id="fc08b-311">조회가 파트너 센터에서 만들어지거나 업데이트 된 후 Dynamics 365 환경에서 동기화 되는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="fc08b-311">Referral synchronization when the referral is created or updated in Partner Center and synchronized in the Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="fc08b-312">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-312">Sign in to your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   1. <span data-ttu-id="fc08b-313">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-313">Select **Referrals** from the left menu.</span></span>

   1. <span data-ttu-id="fc08b-314">**새 거래** 옵션을 선택 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-314">Create a new co-sell referral from Partner Center by selecting the **New deal** option.</span></span>

   1. <span data-ttu-id="fc08b-315">Dynamics 365 CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-315">Sign in to your Dynamics 365 CRM environment.</span></span>

   1. <span data-ttu-id="fc08b-316">**오픈 기회** 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-316">Go to **Open Opportunities**.</span></span> <span data-ttu-id="fc08b-317">이제 파트너 센터에서 만든 조회가 Dynamics 365 CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-317">The referral created in Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   1. <span data-ttu-id="fc08b-318">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="fc08b-318">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fc08b-319">다음 단계</span><span class="sxs-lookup"><span data-stu-id="fc08b-319">Next steps</span></span>

- [<span data-ttu-id="fc08b-320">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="fc08b-320">Manage leads</span></span>](manage-leads.md)
- [<span data-ttu-id="fc08b-321">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="fc08b-321">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
- [<span data-ttu-id="fc08b-322">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="fc08b-322">More about Microsoft Power Automate platform</span></span>](/power-automate/)
- [<span data-ttu-id="fc08b-323">파트너 센터 웹후크</span><span class="sxs-lookup"><span data-stu-id="fc08b-323">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
