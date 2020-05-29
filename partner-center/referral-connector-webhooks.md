---
title: 웹 후크를 사용 하 여 리소스 변경 이벤트 가져오기
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 웹 후크 Api를 사용 하 여 조회 리소스 변경이 발생 하는 경우를 확인 합니다.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 조회, webhook api, 리소스 변경 이벤트
ms.localizationpriority: medium
ms.openlocfilehash: 4e1eb2e9bd8ceb4f8c4bf43684305504c8594e5c
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145087"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="61b43-104">Webhook Api를 사용 하 여 리소스 변경 이벤트 등록</span><span class="sxs-lookup"><span data-stu-id="61b43-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="61b43-105">적절한 역할</span><span class="sxs-lookup"><span data-stu-id="61b43-105">Appropriate roles</span></span>

- <span data-ttu-id="61b43-106">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="61b43-106">Referrals admin</span></span>
- <span data-ttu-id="61b43-107">Dynamics 365 CRM 또는 Salesforce CRM에 대 한 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="61b43-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="61b43-108">파트너 센터 Webhook Api를 사용 하 여 리소스 변경 이벤트를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="61b43-109">이러한 변경 이벤트는 HTTP 게시로 url에 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="61b43-110">이 항목에서는 Dynamics 365 CRM 및 Salesforce CRM의 Webhook Api에 대해 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="61b43-111">Url을 등록 하려면 **파트너 센터 Webhook 등록 (Insider preview)** 전원 자동화 흐름을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="61b43-112">(A.)에 대 한 연결을 추가 합니다. 조회 관리자 자격 증명이 있는 파트너 센터 사용자 (b.) 아래 강조 표시 된 파트너 센터 이벤트</span><span class="sxs-lookup"><span data-stu-id="61b43-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![트리거](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="61b43-114">이러한 업데이트를 수행 하면 다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-114">When you make these updates, you will see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="61b43-116">변경 내용을 저장 하 고 **켜기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="61b43-117">파트너 센터 웹 후크가 파트너 센터 및 CRM 시스템의 IP 공동 판매/독립적인 조회 개체에서 이벤트 변경 내용을 수신 대기 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="61b43-118">**파트너 센터에서 Dynamics 365 (Insider preview)** 또는 **파트너 센터를 Salesforce (insider preview)** 로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="61b43-119">**편집** 아이콘을 선택 하 고 **HTTP 요청을 받을 때**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="61b43-120">**복사** 아이콘을 선택 하 여 제공 된 HTTP POST URL을 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![URL 복사](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="61b43-122">이제 "파트너 센터 Webhook 등록 (Insider Preview)" 전원 자동화 흐름을 선택 하 고 **실행**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="61b43-123">오른쪽 창에 "흐름 실행" 창이 열려 있는지 확인 하 고 **계속**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="61b43-124">다음 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-124">Enter the following details:</span></span> 

    <span data-ttu-id="61b43-125">a.</span><span class="sxs-lookup"><span data-stu-id="61b43-125">a.</span></span> <span data-ttu-id="61b43-126">**Http 트리거 끝점**: 이전 단계에서 복사한 URL</span><span class="sxs-lookup"><span data-stu-id="61b43-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="61b43-127">b.</span><span class="sxs-lookup"><span data-stu-id="61b43-127">b.</span></span> <span data-ttu-id="61b43-128">**등록할 이벤트**: "조회 생성" 및 "조회-업데이트 됨"</span><span class="sxs-lookup"><span data-stu-id="61b43-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="61b43-129">다.</span><span class="sxs-lookup"><span data-stu-id="61b43-129">c.</span></span> <span data-ttu-id="61b43-130">**기존 트리거 끝점을 덮어씁니다 (있는 경우**). 예 (기존 끝점을 덮어씁니다.)</span><span class="sxs-lookup"><span data-stu-id="61b43-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="61b43-131">이제 webhook에서 변경 내용 (이벤트 만들기 및 업데이트)을 수신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="61b43-132">**실행** 을 선택한 다음 완료를 선택 **합니다.**</span><span class="sxs-lookup"><span data-stu-id="61b43-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="61b43-133">동기화 단계 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="61b43-133">Customize synchronization steps</span></span>

<span data-ttu-id="61b43-134">공동 판매 조회가 파트너 센터와 CRM 시스템 간에 동기화 되 면 파트너 센터 PC에서 동기화 된 필드가 여기에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="61b43-135">CRM 시스템이 매우 사용자 지정 되는 경우가 많습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="61b43-136">전원 자동화 흐름을 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="61b43-137">필드 매핑 가이드의 지시에 따라 필요한 경우 전원 자동화 흐름의 단계를 적절 하 게 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="61b43-138">CRM에 대 한 Microsoft 파트너 센터 매핑을 제공 하지만 CRM 환경을 기반으로 필드를 추가로 사용자 지정 하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="61b43-139">각 전원 자동화 흐름의 여러 단계는 요구 사항에 따라 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="61b43-140">사용 가능한 사용자 지정의 예는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="61b43-141">파트너 센터에서 이벤트 만들기 또는 업데이트에 대 한 필드를 CRM 조회 동기화로 사용자 지정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="61b43-142">a.</span><span class="sxs-lookup"><span data-stu-id="61b43-142">a.</span></span> <span data-ttu-id="61b43-143">파트너 센터에서 Dynamics 365 (Insider Preview) 또는 파트너 센터를 Salesforce (Insider preview)로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="61b43-144">b.</span><span class="sxs-lookup"><span data-stu-id="61b43-144">b.</span></span> <span data-ttu-id="61b43-145">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="61b43-146">다.</span><span class="sxs-lookup"><span data-stu-id="61b43-146">c.</span></span> <span data-ttu-id="61b43-147">선택 **(범위) 잠재 고객 또는 기회를 동기화**합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="61b43-148">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **새 공유 기회 인지 여부**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="61b43-149">**예 인 경우** 하위 단계를 선택한 다음 **CRM에서 새 기회 만들기**를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="61b43-150">필드 매핑 가이드를 사용 하 여이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="61b43-151">d.</span><span class="sxs-lookup"><span data-stu-id="61b43-151">d.</span></span> <span data-ttu-id="61b43-152">업데이트 이벤트의 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 "(범위) 잠재 고객 또는 기회 동기화" 단계를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="61b43-153">e.</span><span class="sxs-lookup"><span data-stu-id="61b43-153">e.</span></span> <span data-ttu-id="61b43-154">**기회를 업데이트 하는 경우를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="61b43-155">**예 인 경우** 하위 단계를 선택 하 고 **파트너 센터와 CRM의 기회 개체 간 차이를**확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="61b43-156">f.</span><span class="sxs-lookup"><span data-stu-id="61b43-156">f.</span></span> <span data-ttu-id="61b43-157">**예** 를 선택 하 고 **기존 기회 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="61b43-158">업데이트 이벤트의 CRM to PC 조회 동기화에 대 한 필드를 사용자 지정 하려면:</span><span class="sxs-lookup"><span data-stu-id="61b43-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="61b43-159">a.</span><span class="sxs-lookup"><span data-stu-id="61b43-159">a.</span></span> <span data-ttu-id="61b43-160">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="61b43-161">b.</span><span class="sxs-lookup"><span data-stu-id="61b43-161">b.</span></span> <span data-ttu-id="61b43-162">**기회 동기화를 선택 (범위)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="61b43-163">다.</span><span class="sxs-lookup"><span data-stu-id="61b43-163">c.</span></span> <span data-ttu-id="61b43-164">업데이트 이벤트에 대해 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **파트너 센터와 CRM의 리드 개체 사이에 차이가 있는 경우**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="61b43-165">d.</span><span class="sxs-lookup"><span data-stu-id="61b43-165">d.</span></span> <span data-ttu-id="61b43-166">**예 인 경우** 하위 단계을 선택 하 고 **기회 데이터를 사용 하 여 조회 업데이트**단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="61b43-167">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="61b43-168">만든 이벤트에 대 한 CRM에서 PC 조회 동기화에 대 한 필드를 사용자 지정 하려면</span><span class="sxs-lookup"><span data-stu-id="61b43-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="61b43-169">a.</span><span class="sxs-lookup"><span data-stu-id="61b43-169">a.</span></span> <span data-ttu-id="61b43-170">**편집** 을 선택 하 여 전원 자동화 흐름을 편집/사용자 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="61b43-171">b.</span><span class="sxs-lookup"><span data-stu-id="61b43-171">b.</span></span> <span data-ttu-id="61b43-172">**조회 동기화를 선택 (범위) 합니다.**</span><span class="sxs-lookup"><span data-stu-id="61b43-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="61b43-173">다.</span><span class="sxs-lookup"><span data-stu-id="61b43-173">c.</span></span> <span data-ttu-id="61b43-174">만든 이벤트에 대 한 CRM 필드 매핑 (필드 매핑 가이드 기반)을 사용자 지정 하려면 **Microsoft 조회 만들기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="61b43-175">필드 매핑 가이드에 따라이 섹션에서 매핑을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="61b43-176">종단 간 양방향 공동 판매 참조 동기화</span><span class="sxs-lookup"><span data-stu-id="61b43-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="61b43-177">전원 자동화 솔루션을 설치, 구성 및 사용자 지정 하 고 나면 Dynamics 365 또는 Salesforce와 파트너 센터 간에 공동 판매 된 조회 동기화를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="61b43-178">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="61b43-178">Pre-requisites</span></span>

<span data-ttu-id="61b43-179">파트너 센터 및 Dynamics 365 CRM에서 또는 파트너 센터와 Salesforce CRM 간에 조회를 동기화 하려면 전원 자동화 솔루션이 Microsoft 전용 조회 필드를 명확 하 게 구분 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="61b43-180">이를 통해 판매자 팀은 공동 판매를 위해 Microsoft와 공유할 조회를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="61b43-181">사용자 지정 필드 집합은 Dynamics 365 솔루션 **기회** 엔터티에 대 한 파트너 센터 조회 동기화의 일부로 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="61b43-182">CRM admin 사용자는 **기회** 사용자 지정 필드를 사용 하 여 별도의 crm 섹션을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="61b43-183">다음 사용자 지정 필드는 CRM 섹션의 일부 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="61b43-184">**파트너 센터와 동기화**: Microsoft 파트너 센터를 사용 하 여 기회를 동기화할지 여부</span><span class="sxs-lookup"><span data-stu-id="61b43-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="61b43-185">**참조 식별자**: Microsoft 파트너 센터 조회에 대 한 읽기 전용 식별자 필드</span><span class="sxs-lookup"><span data-stu-id="61b43-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="61b43-186">**참조 링크**: Microsoft 파트너 센터에서 조회에 대 한 읽기 전용 링크</span><span class="sxs-lookup"><span data-stu-id="61b43-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="61b43-187">**Microsoft에서 microsoft의 도움**을 받아야 하는 방법: microsoft에서 조회에 대 한 도움말</span><span class="sxs-lookup"><span data-stu-id="61b43-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="61b43-188">**제품**:이 기회와 관련 된 제품 목록</span><span class="sxs-lookup"><span data-stu-id="61b43-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="61b43-189">**감사**: 파트너 센터 조회와 동기화 하기 위한 읽기 전용 감사 내역</span><span class="sxs-lookup"><span data-stu-id="61b43-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="61b43-190">에서는</span><span class="sxs-lookup"><span data-stu-id="61b43-190">SCENARIOS:</span></span>

1. <span data-ttu-id="61b43-191">CRM에서 조회를 만들거나 업데이트 하 고 파트너 센터에서 동기화 하는 경우의 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="61b43-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="61b43-192">a.</span><span class="sxs-lookup"><span data-stu-id="61b43-192">a.</span></span> <span data-ttu-id="61b43-193">CRM의 **기회** 섹션에서 볼 수 있는 사용자를 사용 하 여 DYNAMICS 365 crm 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-193">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="61b43-194">b.</span><span class="sxs-lookup"><span data-stu-id="61b43-194">b.</span></span> <span data-ttu-id="61b43-195">Dynamics 365 환경에서 "새 기회"를 만들 때 다음 섹션이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![기회](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="61b43-197">다.</span><span class="sxs-lookup"><span data-stu-id="61b43-197">c.</span></span> <span data-ttu-id="61b43-198">이 기회를 Microsoft 파트너 센터와 동기화 하려면 카드 보기에서 다음 필드를 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="61b43-199">"파트너 센터와 동기화": 예</span><span class="sxs-lookup"><span data-stu-id="61b43-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="61b43-200">"Microsoft의 도움을 주는 방법": 다음 중에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![도움말 선택](images/cosellconnectors/help.png)

    - <span data-ttu-id="61b43-202">제품: 제품의 솔루션 Id</span><span class="sxs-lookup"><span data-stu-id="61b43-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="61b43-203">d.</span><span class="sxs-lookup"><span data-stu-id="61b43-203">d.</span></span> <span data-ttu-id="61b43-204">**파트너 센터** 옵션을 **예**로 설정 하 여 Dynamics 365에서 통합 기회가 만들어지면 10 분 정도 기다렸다가 파트너 센터 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="61b43-205">사용자의 조회가 Dynamics 365와 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="61b43-206">e.</span><span class="sxs-lookup"><span data-stu-id="61b43-206">e.</span></span> <span data-ttu-id="61b43-207">따라서 "파트너 센터와 동기화" 옵션을 "예"로 설정 하는 기회에 대해 Dynamics 365 CRM에서 기회를 업데이트 하면 변경 내용이 파트너 센터 계정에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="61b43-208">f.</span><span class="sxs-lookup"><span data-stu-id="61b43-208">f.</span></span> <span data-ttu-id="61b43-209">파트너 센터와 성공적으로 동기화 되는 기회는 Dynamics 365의 ✔ 아이콘으로 식별 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="61b43-210">Microsoft 파트너 센터에서 조회를 만들거나 업데이트 하 고 Dynamics 365 환경에서 동기화 할 때 조회 동기화:</span><span class="sxs-lookup"><span data-stu-id="61b43-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="61b43-211">a.</span><span class="sxs-lookup"><span data-stu-id="61b43-211">a.</span></span> <span data-ttu-id="61b43-212">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard/home)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="61b43-213">b.</span><span class="sxs-lookup"><span data-stu-id="61b43-213">b.</span></span> <span data-ttu-id="61b43-214">왼쪽 메뉴에서 **조회** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="61b43-215">다.</span><span class="sxs-lookup"><span data-stu-id="61b43-215">c.</span></span> <span data-ttu-id="61b43-216">"새 거래" 옵션을 클릭 하 여 파트너 센터에서 새 공동 판매 참조를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="61b43-217">d.</span><span class="sxs-lookup"><span data-stu-id="61b43-217">d.</span></span> <span data-ttu-id="61b43-218">Dynamics 365 CRM 환경에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="61b43-219">e.</span><span class="sxs-lookup"><span data-stu-id="61b43-219">e.</span></span> <span data-ttu-id="61b43-220">**오픈 기회**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="61b43-221">Microsoft Partner Center에서 만든 조회는 이제 Dynamics 365 CRM에서 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="61b43-222">f.</span><span class="sxs-lookup"><span data-stu-id="61b43-222">f.</span></span> <span data-ttu-id="61b43-223">동기화 된 조회를 선택 하면 카드 보기 정보가 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="61b43-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="61b43-224">다음 단계</span><span class="sxs-lookup"><span data-stu-id="61b43-224">Next steps</span></span>

- [<span data-ttu-id="61b43-225">Microsoft Power 자동화 플랫폼에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="61b43-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="61b43-226">파트너 센터 webhook 이벤트</span><span class="sxs-lookup"><span data-stu-id="61b43-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="61b43-227">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="61b43-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="61b43-228">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="61b43-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
