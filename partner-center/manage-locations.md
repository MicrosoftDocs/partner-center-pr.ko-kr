---
title: 파트너 계정의 위치 관리
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 새로운 위치를 추가하는 방법과 인센티브 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에서 위치 MPN ID를 사용하는 방법을 알아봅니다.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f13676c8a4343feb5a099053b32b7444bbdfba45
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436872"
---
# <a name="manage-your-partner-account-locations-in-partner-center-and-add-a-new-location"></a><span data-ttu-id="0f91f-103">파트너 센터에서 파트너 계정 위치 관리 및 새 위치 추가</span><span class="sxs-lookup"><span data-stu-id="0f91f-103">Manage your partner account locations in Partner Center and add a new location</span></span>

<span data-ttu-id="0f91f-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="0f91f-104">**Appropriate roles**</span></span>
- <span data-ttu-id="0f91f-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="0f91f-105">Global admin</span></span>
- <span data-ttu-id="0f91f-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="0f91f-106">User admin</span></span>
- <span data-ttu-id="0f91f-107">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="0f91f-107">Billing admin</span></span>
- <span data-ttu-id="0f91f-108">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="0f91f-108">Admin agent</span></span>
- <span data-ttu-id="0f91f-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="0f91f-109">Sales agent</span></span>

<span data-ttu-id="0f91f-110">위치 MPN ID는 각 회사의 위치를 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-110">The location MPN IDs identify each specific location of your company.</span></span> <span data-ttu-id="0f91f-111">위치 MPN ID를 사용하여 인센티브 프로그램에 등록하고, CSP(클라우드 솔루션 공급자) 비즈니스를 거래하고, 새 구독 및 기타 비즈니스 트랜잭션을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-111">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, to add new subscriptions, and other business transactions.</span></span> <span data-ttu-id="0f91f-112">회사 MPN ID는 지원 요청 등의 비트랜잭션 작업에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-112">The company MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="0f91f-113">다음은 일반적인 시나리오입니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-113">The following is a typical scenario:</span></span>

<span data-ttu-id="0f91f-114">파트너가 산하에 CSP 회사와 퍼블리싱 회사를 각각 하나씩 거느리고 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-114">A partner company can have a CSP business and a publishing business.</span></span> <span data-ttu-id="0f91f-115">파트너의 CSP 회사가 여러 위치에 분산되어 있고 퍼블리싱 비즈니스는 다른 위치에 있을 수 있습니다. 파트너의 등록된 합법적인 회사는 사용자 추가 또는 지원 요청 로깅과 같은 모든 비트랜잭션 비즈니스를 관리하는 데 사용되는 하나의 MPN ID를 갖고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-115">Their CSP business can be located in several locales and their pub business may be located in other locales.Their registered legal business has one MPN ID used for managing all non-transactional business such as adding users or logging support requests.</span></span>


<span data-ttu-id="0f91f-116">각 위치에는 CSP 또는 인센티브 프로그램 같은 트랜잭션 비즈니스에 사용되는 MPN ID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-116">Each of their locations has an MPN ID used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="0f91f-117">결제는 특정 위치에 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-117">Payouts are tied to specific locations.</span></span>

<span data-ttu-id="0f91f-118">사용자에게는 위치를 넘나드는 역할이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-118">Users may have roles that cross locations.</span></span> <span data-ttu-id="0f91f-119">예를 들어 인센티브 관리자는 유럽의 모든 위치에 대해 해당 역할을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-119">For example, the incentives admin could have that role for all locations in Europe.</span></span>

## <a name="to-add-a-location"></a><span data-ttu-id="0f91f-120">위치를 추가하려면</span><span class="sxs-lookup"><span data-stu-id="0f91f-120">To add a location</span></span>

1. <span data-ttu-id="0f91f-121">**설정 아이콘**에서 **파트너 설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-121">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="0f91f-122">**위치**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-122">Select **Locations.**</span></span>

3. <span data-ttu-id="0f91f-123">**위치 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-123">Select **Add a location**.</span></span>  

4. <span data-ttu-id="0f91f-124">**위치 추가** 페이지에서 회사에 추가하려는 위치의 주소 정보와 위치의 기본 연락처를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-124">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="0f91f-125">파트너 센터에서 추가한 위치는 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-125">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-legal-headquarters-location"></a><span data-ttu-id="0f91f-126">법률적 본사 위치 변경</span><span class="sxs-lookup"><span data-stu-id="0f91f-126">Change legal headquarters location</span></span>

1. <span data-ttu-id="0f91f-127">**위치** 페이지에서 위치 목록을 검사하여 법인으로 사용할 위치가 나열되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-127">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="0f91f-128">그렇지 않은 경우 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-128">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="현재 모든 위치의 목록이 포함된 파트너 센터 계정 위치 페이지의 스크린샷":::

2. <span data-ttu-id="0f91f-130">**파트너 프로필**, **법적 비즈니스 프로필 업데이트**를 차례로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-130">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="선택 가능한 업데이트 옵션을 사용하여 파트너 센터 계정 파트너 프로필 정보를 보여주는 스크린샷":::

3. <span data-ttu-id="0f91f-132">지역 및 법인을 선택하고 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f91f-132">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="파트너의 법적 비즈니스 프로필을 업데이트하는 스크린샷에는 국가 또는 지역과 법인을 업데이트하는 드롭다운 목록이 표시됩니다.":::
