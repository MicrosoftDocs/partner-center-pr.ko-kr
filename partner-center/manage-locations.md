---
title: 파트너 계정의 위치 관리
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 새 위치를 추가하는 방법 및 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663901"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="9aa0e-103">MPN 계정 위치 관리 및 새 위치 추가</span><span class="sxs-lookup"><span data-stu-id="9aa0e-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="9aa0e-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="9aa0e-104">**Applies to**</span></span>

- <span data-ttu-id="9aa0e-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="9aa0e-105">Partner Center</span></span>

<span data-ttu-id="9aa0e-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="9aa0e-106">**Appropriate roles**</span></span>

- <span data-ttu-id="9aa0e-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="9aa0e-107">Global admin</span></span>
- <span data-ttu-id="9aa0e-108">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="9aa0e-108">Account admin</span></span>

<span data-ttu-id="9aa0e-109">위치 MPN ID는 회사의 각 특정 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="9aa0e-110">위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스와 기타 비즈니스 트랜잭션을 처리합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="9aa0e-111">글로벌 MPN ID는 지원 요청과 같은 비 트랜잭션 작업에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="9aa0e-112">다음은 일반적인 시나리오입니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-112">The following is a typical scenario:</span></span>

<span data-ttu-id="9aa0e-113">Contoso는 영국에 해당 PGA(파트너 글로벌 계정) 위치를 가지고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="9aa0e-114">이 위치는 등록된 법적 회사이며, 모든 비 트랜잭션 비즈니스를 관리하는 데 사용되는 하나의 MPN ID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="9aa0e-115">또한 Contoso는 영국, 프랑스 및 미국의 다른 위치에 있는 자회사 또는 사업부에 해당하는 PLA(파트너 위치 계정)를 가지고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="9aa0e-116">MPN 계정 구조에서 이러한 PLA는 고유한 위치 MPN ID로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="9aa0e-117">PLA는 CSP 또는 인센티브 프로그램과 같은 트랜잭션 비즈니스에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="9aa0e-118">결제는 특정 위치에 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="9aa0e-119">CSP 테넌트와 MPN 위치 ID 사이에는 일대일 관계가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="MPN 위치 구조":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="9aa0e-121">새 CSP 비즈니스 위치를 추가하기 위한 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="9aa0e-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="9aa0e-122">새 CSP 비즈니스 위치를 추가하려면 다음과 같은 몇 가지 필수 구성 요소가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="9aa0e-123">비즈니스를 수행하려는 국가에 위치 MPN ID가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="9aa0e-124">아직 CSP에 등록되지 않은 비즈니스 지역에 새 Azure AD 테넌트가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="9aa0e-125">이 테넌트는 CSP에 등록할 때 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="9aa0e-126">새 AAD 테넌트를 사용하여 해당 지역의 CSP 프로그램에 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="9aa0e-127">법적 회사 이름, 주소, 기본 연락처 세부 정보를 포함한 법적 회사 세부 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="9aa0e-128">이 계정에는 확인 프로세스가 수행되므로 유효한 정보를 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="9aa0e-129">**새** Azure AD 테넌트에 대한 **새** 자격 증명을 사용하여 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="9aa0e-130">파트너 센터에서 이미 계정이 있는 것으로 인식하므로 기존 자격 증명을 사용하지 마세요.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="9aa0e-131">Microsoft 파트너 계약에 동의하고 계정을 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="9aa0e-132">위치 추가</span><span class="sxs-lookup"><span data-stu-id="9aa0e-132">Add a location</span></span>

1. <span data-ttu-id="9aa0e-133">**설정 아이콘**에서 **파트너 설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="9aa0e-134">**위치**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-134">Select **Locations.**</span></span>

3. <span data-ttu-id="9aa0e-135">**위치 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="9aa0e-136">**위치 추가** 페이지에서 회사에 추가하려는 위치의 주소 정보와 위치의 기본 연락처를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="9aa0e-137">파트너 센터에서 추가한 위치는 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="9aa0e-138">글로벌 파트너 계정 위치 변경</span><span class="sxs-lookup"><span data-stu-id="9aa0e-138">Change Global partner account location</span></span>

1. <span data-ttu-id="9aa0e-139">**위치** 페이지에서 위치 목록을 검사하여 법인으로 사용할 위치가 나열되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="9aa0e-140">그렇지 않은 경우 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN 위치 구조":::

2. <span data-ttu-id="9aa0e-142">**파트너 프로필**, **법적 비즈니스 프로필 업데이트**를 차례로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN 위치 구조":::

3. <span data-ttu-id="9aa0e-144">지역 및 법인을 선택하고 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN 위치 구조":::

## <a name="next-steps"></a><span data-ttu-id="9aa0e-146">다음 단계</span><span class="sxs-lookup"><span data-stu-id="9aa0e-146">Next steps</span></span>

- <span data-ttu-id="9aa0e-147">[확인 프로세스](verification-responses.md)에 대해 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="9aa0e-147">Learn about the [verification process](verification-responses.md).</span></span>
