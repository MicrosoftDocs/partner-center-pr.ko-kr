---
title: 파트너 계정의 위치 관리
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 새 위치를 추가하는 방법 및 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624275"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="a5b29-103">MPN 계정 위치 관리 및 새 위치 추가</span><span class="sxs-lookup"><span data-stu-id="a5b29-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="a5b29-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="a5b29-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a5b29-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="a5b29-105">Global admin</span></span>
- <span data-ttu-id="a5b29-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="a5b29-106">Account admin</span></span>

<span data-ttu-id="a5b29-107">위치 MPN ID는 회사의 각 특정 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="a5b29-108">위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스와 기타 비즈니스 트랜잭션을 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="a5b29-109">글로벌 MPN ID는 지원 요청과 같은 비 트랜잭션 작업에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="a5b29-110">다음은 일반적인 시나리오입니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-110">The following is a typical scenario:</span></span>

<span data-ttu-id="a5b29-111">Contoso는 영국에 PGA(파트너 글로벌 계정)를 가지고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="a5b29-112">이는 이 업체의 등록된 합법적인 사업이며 이 회사의 글로벌 MPN ID는 모든 비 트랜잭션 비즈니스를 관리하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="a5b29-113">또한 Contoso는 영국, 프랑스 및 미국의 다른 위치에 있는 자회사 또는 사업부에 해당하는 PLA(파트너 위치 계정)를 가지고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="a5b29-114">MPN 계정 구조에서 이러한 PLA는 고유한 위치 MPN ID로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="a5b29-115">PLA는 CSP 또는 인센티브 프로그램과 같은 트랜잭션 비즈니스에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="a5b29-116">결제는 특정 위치에 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="a5b29-117">CSP 테넌트와 MPN 위치 ID 사이에는 일대일 관계가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 위치 구조":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="a5b29-119">CSP 비즈니스에 대한 새 위치를 추가하기 위한 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="a5b29-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="a5b29-120">새 CSP 비즈니스 계정을 추가하려면 먼저 사전 요구 사항을 충족했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="a5b29-121">CSP 비즈니스를 수행하려는 국가에 위치 MPN ID가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="a5b29-122">새 MPN 위치를 만들려면 아래의 "MPN 위치 추가"를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a5b29-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="a5b29-123">새 CSP 간접 재판매인 등록을 만들려면 [간접 공급자와 협력](indirect-reseller-tasks-in-partner-center.md#get-started)을 읽어보세요.</span><span class="sxs-lookup"><span data-stu-id="a5b29-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="a5b29-124">**새** CSP 계정에 대해서는 **새** 자격 증명을 사용하여 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="a5b29-125">파트너 센터에서 이미 계정이 있는 것으로 인식하므로 기존 자격 증명을 사용하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="a5b29-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="a5b29-126">Microsoft 파트너 계약에 동의하고 계정을 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="a5b29-127">직접 청구 파트너로 등록하려면 [직접 청구 파트너 요구 사항](direct-partner-new-requirements.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a5b29-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="a5b29-128">MPN 위치 보기</span><span class="sxs-lookup"><span data-stu-id="a5b29-128">View your MPN locations</span></span>

1. <span data-ttu-id="a5b29-129">MPN 계정 자격 증명으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="a5b29-130">(MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="a5b29-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="a5b29-131">**설정** 아이콘에서 **계정 설정** 을 선택한 다음, **조직 프로필**, **법무** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="a5b29-132">**파트너** 탭에서, PMC에서 마이그레이션된 위치를 수정하라는 배너 오류 메시지가 없는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="a5b29-133">있는 경우 지침에 따라 해당 위치를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="a5b29-134">오류 메시지가 없는 경우 **설정** 에서 **계정 설정**, **조직 프로필**, **식별자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="a5b29-135">이 CSP 계정의 국가와 일치하는 "위치" 유형의 MPN ID를 찾아 아래에서 검색하고 연결을 완료하는 데 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="a5b29-136">사용하려는 CSP 계정과 일치하는 위치 MPN ID를 찾을 수 없는 경우 새 위치를 추가하여 새 MPN ID를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="a5b29-137">아래 **MPN 위치 추가** 를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a5b29-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="a5b29-138">MPN 위치 추가</span><span class="sxs-lookup"><span data-stu-id="a5b29-138">Add an MPN location</span></span>

1. <span data-ttu-id="a5b29-139">파트너 센터에서 MPN 계정을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a5b29-140">(MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="a5b29-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a5b29-141">MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="a5b29-142">**설정 아이콘** 에서 **계정 설정** 을 선택한 다음, **조직 프로필** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="a5b29-143">**법무** 를 선택한 다음, **파트너** 탭에서 **비즈니스 위치** 를 선택하고 **위치 추가** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="a5b29-144">회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="a5b29-145">**위치 추가** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-145">Click **Add location**.</span></span> <span data-ttu-id="a5b29-146">그러면 CSP 트랜잭션 및 성과급에 사용할 수 있는 새 위치에 대한 새 MPN ID가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="새로운 법적 비즈니스 추가":::

> [!NOTE]
> <span data-ttu-id="a5b29-148">파트너 센터에서 추가한 위치는 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-148">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="a5b29-149">올바른 MPN ID를 사용하여 로그인한 경우 파트너 센터의 왼쪽 메뉴에 **MPN** 이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="a5b29-150">파트너 전역 계정의 국가 변경</span><span class="sxs-lookup"><span data-stu-id="a5b29-150">Change country of Partner global account</span></span> 

1. <span data-ttu-id="a5b29-151">파트너 센터에서 MPN 계정을 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-151">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a5b29-152">(MPN 자격 증명은 CSP 자격 증명과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="a5b29-152">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a5b29-153">MPN 계정에는 전역 관리자 또는 계정 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-153">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="a5b29-154">**파트너** 탭에서 **비즈니스 위치** 에서 위치 목록을 확인하여 법인으로 원하는 위치가 나열되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-154">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="a5b29-155">위치를 추가하려면 **위치 추가** 를 클릭하고, 플라이 아웃에서 회사에 추가하려는 위치 정보 즉, 회사 이름, 주소 및 연락처 등 필요한 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-155">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="a5b29-156">**국가/지역** 드롭다운 옆에 있는 **국가 변경** 을 선택하고 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-156">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="법적 비즈니스 프로필 데이터 플라이 아웃":::

5. <span data-ttu-id="a5b29-158">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-158">Click **Save**.</span></span>

6. <span data-ttu-id="a5b29-159">MPN 전역 계정 국가는 새로운 법적 국가로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="a5b29-159">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="a5b29-160">다음 단계</span><span class="sxs-lookup"><span data-stu-id="a5b29-160">Next steps</span></span>

- <span data-ttu-id="a5b29-161">[확인 프로세스](verification-responses.md)에 대해 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="a5b29-161">Learn about the [verification process](verification-responses.md).</span></span>
