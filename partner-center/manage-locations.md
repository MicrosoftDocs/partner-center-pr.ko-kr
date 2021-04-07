---
title: 파트너 계정의 위치 관리
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 새 위치를 추가하는 방법 및 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441333"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="0cdf2-103">MPN 계정 위치 관리 및 새 위치 추가(삭제)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="0cdf2-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="0cdf2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0cdf2-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="0cdf2-105">Global admin</span></span>
- <span data-ttu-id="0cdf2-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="0cdf2-106">Account admin</span></span>

<span data-ttu-id="0cdf2-107">위치 MPN ID는 회사의 각 특정 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="0cdf2-108">위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스와 기타 비즈니스 트랜잭션을 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="0cdf2-109">글로벌 MPN ID는 지원 요청과 같은 비 트랜잭션 작업에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="0cdf2-110">다음 시나리오가 일반적입니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-110">The following scenario is typical:</span></span>

<span data-ttu-id="0cdf2-111">Contoso는 영국에 PGA(파트너 글로벌 계정)를 가지고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="0cdf2-112">PGA는 등록된 합법적인 사업이며 이 회사의 글로벌 MPN ID는 모든 비 트랜잭션 비즈니스를 관리하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="0cdf2-113">또한 Contoso는 영국, 프랑스 및 미국의 다른 위치에 있는 자회사 또는 사업부에 해당하는 PLA(파트너 위치 계정)를 가지고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="0cdf2-114">MPN 계정 구조에서 이러한 PLA는 고유한 위치 MPN ID로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="0cdf2-115">PLA는 CSP 또는 인센티브 프로그램과 같은 트랜잭션 비즈니스에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="0cdf2-116">결제는 특정 위치에 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="0cdf2-117">CSP 테넌트와 MPN 위치 ID 사이에는 일대일 관계가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 위치 구조":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="0cdf2-119">CSP 비즈니스에 대한 새 위치를 추가하기 위한 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="0cdf2-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="0cdf2-120">새 CSP 비즈니스 계정을 추가하려면 먼저 사전 요구 사항을 충족했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="0cdf2-121">CSP 비즈니스를 수행하려는 국가에 위치 MPN ID가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="0cdf2-122">새 MPN 위치를 만들려면 아래의 "MPN 위치 추가"를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="0cdf2-123">새 CSP 간접 재판매인 등록을 만들려면 [간접 공급자와 협력](indirect-reseller-tasks-in-partner-center.md#get-started)을 읽어보세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="0cdf2-124">**새** CSP 계정에 대해서는 **새** 자격 증명을 사용하여 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="0cdf2-125">파트너 센터에서 이미 계정이 있는 것으로 인식하므로 기존 자격 증명을 사용하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="0cdf2-126">Microsoft 파트너 계약에 동의하고 계정을 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="0cdf2-127">직접 청구 파트너로 등록하려면 [직접 청구 파트너 요구 사항](direct-partner-new-requirements.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="0cdf2-128">MPN 위치 보기</span><span class="sxs-lookup"><span data-stu-id="0cdf2-128">View your MPN locations</span></span>

1. <span data-ttu-id="0cdf2-129">MPN 계정 자격 증명으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="0cdf2-130">(MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="0cdf2-131">**설정** 아이콘에서 **계정 설정** 을 선택한 다음, **조직 프로필**, **법무** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="0cdf2-132">**파트너** 탭에서, PMC에서 마이그레이션된 위치를 수정하라는 배너 오류 메시지가 없는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="0cdf2-133">PMC에서 위치가 올바르게 설정되지 않았거나 PC로 아직 전환되지 않은 경우 해당 위치를 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap은 위치를 업데이트하는 방법을 보여줍니다.":::
 
4.  <span data-ttu-id="0cdf2-135">**PMC 위치 검토** 화면에서 **업데이트** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="0cdf2-136">다음 필드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-136">Update the following fields:</span></span>

- <span data-ttu-id="0cdf2-137">**이름 필드**: 회사 위치 이름이 올바른지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="0cdf2-138">중복 오류가 표시되는 경우, 예를 들어 Contoso에서 Contoso, Inc.로 변경해 보세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="0cdf2-139">**법인 필드**: 위치가 연결된 법인을 선택했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="0cdf2-140">**주소란 1 및 2** : 주소가 정확한지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="0cdf2-141">**시 및 주/도 필드**: 시와 주/도의 조합이 올바른지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="0cdf2-142">주/도를 선택하는 드롭다운 메뉴가 표시되는 국가가 있고 필드를 수동으로 입력해야 하는 국가도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="0cdf2-143">**우편 번호 필드**: 우편 번호 필드가 표시된 국가, 지역, 시 또는 주소와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="0cdf2-144">**기본 연락처 정보 필드**: 이름과 성 필드가 채워져 있고 표시된 이메일 주소가 개인 이메일이 아닌 업무용 이메일 주소(예: @outlook.com, @live.com 등)인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="0cdf2-145">**전화 번호 필드**: 전화 번호에 특수 문자, 공백 또는 국가 코드가 포함되어 있지 않은지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="0cdf2-146">전화 번호 필드에 입력할 수 있는 값은 항상 최대 10자입니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="0cdf2-147">오류 메시지가 없는 경우 **설정** 에서 **계정 설정**, **조직 프로필**, **식별자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="0cdf2-148">이 CSP 계정의 국가와 일치하는 "위치" 유형의 MPN ID를 찾아 연결을 완료하는 데 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="0cdf2-149">사용하려는 CSP 계정과 일치하는 위치 MPN ID를 찾을 수 없는 경우 새 위치를 추가하여 새 MPN ID를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="0cdf2-150">아래 **MPN 위치 추가** 를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="0cdf2-151">MPN 위치 추가</span><span class="sxs-lookup"><span data-stu-id="0cdf2-151">Add an MPN location</span></span>

1. <span data-ttu-id="0cdf2-152">파트너 센터에서 MPN 계정을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="0cdf2-153">(MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="0cdf2-154">MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="0cdf2-155">**설정 아이콘** 에서 **계정 설정** 을 선택한 다음, **조직 프로필** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="0cdf2-156">**법무** 를 선택한 다음, **파트너** 탭에서 **비즈니스 위치** 를 선택하고 **위치 추가** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="0cdf2-157">회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="0cdf2-158">**위치 추가** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-158">Click **Add location**.</span></span> <span data-ttu-id="0cdf2-159">그러면 CSP 트랜잭션 및 성과급에 사용할 수 있는 새 위치에 대한 새 MPN ID가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="새로운 법적 비즈니스 추가":::

> [!NOTE]
> <span data-ttu-id="0cdf2-161">파트너 센터에서 추가한 위치는 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="0cdf2-162">올바른 MPN ID를 사용하여 로그인한 경우 파트너 센터의 왼쪽 메뉴에 **MPN** 이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="0cdf2-163">위치 삭제</span><span class="sxs-lookup"><span data-stu-id="0cdf2-163">Delete a location</span></span>

<span data-ttu-id="0cdf2-164">계정에서 위치를 삭제하려면 [파트너 지원](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)에 문의해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="0cdf2-165">이 작업이 미치는 영향을 이해했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="0cdf2-166">삭제된 위치는 검색할 수 없으며 특정 MPN ID에 연결된 모든 항목은 더 이상 인식되지 않거나 회사에 대해 활성화되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="0cdf2-167">파트너 전역 계정의 국가 변경</span><span class="sxs-lookup"><span data-stu-id="0cdf2-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="0cdf2-168">파트너 센터에서 MPN 계정을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="0cdf2-169">(MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="0cdf2-170">MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="0cdf2-171">**파트너** 탭에서 **비즈니스 위치** 에서 위치 목록을 확인하여 법인으로 원하는 위치가 나열되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="0cdf2-172">위치를 추가하려면 **위치 추가** 를 클릭하고, 플라이 아웃에서 회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="0cdf2-173">**국가/지역** 드롭다운 옆에 있는 **국가 변경** 을 선택하고 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="법적 비즈니스 프로필 데이터 플라이 아웃":::

5. <span data-ttu-id="0cdf2-175">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-175">Click **Save**.</span></span>

6. <span data-ttu-id="0cdf2-176">MPN 전역 계정 국가는 새로운 법적 국가로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="0cdf2-177">다음 단계</span><span class="sxs-lookup"><span data-stu-id="0cdf2-177">Next steps</span></span>

- <span data-ttu-id="0cdf2-178">[확인 프로세스](verification-responses.md)에 대해 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-178">Learn about the [verification process](verification-responses.md).</span></span>
