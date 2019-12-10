---
title: 파트너 계정 관리-위치 | 파트너 센터
ms.topic: article
ms.date: 03/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: MPN ID가 동기 프로그램, CSP 비즈니스, 구독 및 기타 트랜잭션에 어떻게 사용 되는지 알아보세요.
author: LauraBrenner
ms.author: labrenne
keywords: 파트너 계정, 위치
ms.localizationpriority: medium
ms.openlocfilehash: fe4e2cca922b479bfdec92feb5b21d8824546e23
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943506"
---
# <a name="manage-your-partner-account-locations"></a><span data-ttu-id="58a07-104">파트너 계정 관리: 위치</span><span class="sxs-lookup"><span data-stu-id="58a07-104">Manage your partner account: Locations</span></span>

<span data-ttu-id="58a07-105">위치 MPN Id는 회사의 각 특정 위치를 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-105">The location MPN IDs identify each specific location of your company.</span></span> <span data-ttu-id="58a07-106">Location MPN ID를 사용 하 여 동기 프로그램에 등록 하 고, transact-sql (Cloud Solution Provider) 비즈니스에 등록 하 고, 새 구독과 기타 비즈니스 트랜잭션을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, to add new subscriptions, and other business transactions.</span></span> <span data-ttu-id="58a07-107">회사 MPN ID는 지원 요청 등의 비트랜잭션 작업에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-107">The company MPN ID is used for non-transactional activities such as support requests.</span></span>

<span data-ttu-id="58a07-108">**일반적인 시나리오는 다음과 같습니다.**</span><span class="sxs-lookup"><span data-stu-id="58a07-108">**The following is a typical scenario:**</span></span> 

<span data-ttu-id="58a07-109">파트너 회사는 CSP 비즈니스 및 게시 비즈니스를 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-109">A partner company can have a CSP business and a publishing business.</span></span> <span data-ttu-id="58a07-110">CSP 비즈니스는 여러 로캘에서 배치 될 수 있으며 해당 pub 비즈니스는 다른 로캘에서 있을 수 있습니다. 등록 된 합법적인 비즈니스에는 사용자 추가 또는 지원 요청 로깅과 같은 비트랜잭션 비즈니스를 모두 관리 하는 데 사용 되는 하나의 MPN ID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-110">Their CSP business can be located in several locales and their pub business may be located in other locales.Their registered legal business has one MPN ID which is used for managing all non-transactional business such as adding users or logging support requests.</span></span> 

<span data-ttu-id="58a07-111">각 위치에는 CSP, 성과급 프로그램 등의 트랜잭션 비즈니스에 사용 되는 MPN ID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-111">Each of their locations has an MPN ID which is used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="58a07-112">지급은 특정 위치에 연결 됩니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-112">Payouts are tied to specific locations.</span></span>

<span data-ttu-id="58a07-113">사용자에 게는 위치를 교차 하는 역할이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-113">Users may have roles that cross locations.</span></span> <span data-ttu-id="58a07-114">예를 들어, 성과급 관리자는 유럽의 모든 위치에 대해 해당 역할을 가질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-114">For example, the incentives admin could have that role for all locations in Europe.</span></span>

<span data-ttu-id="58a07-115">**위치를 추가 하려면**</span><span class="sxs-lookup"><span data-stu-id="58a07-115">**To add a location**</span></span>

1. <span data-ttu-id="58a07-116">**설정 아이콘**에서 **파트너 설정을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-116">From the **Setting icon**, select the **Partner settings**.</span></span> 

2. <span data-ttu-id="58a07-117">**위치를 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="58a07-117">Select **Locations.**</span></span>

3. <span data-ttu-id="58a07-118">**위치 추가를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-118">Select **Add a location**.</span></span>  

4. <span data-ttu-id="58a07-119">**위치 추가** 페이지에서 회사에 추가 하려는 위치의 주소 세부 정보 뿐만 아니라 위치에 대 한 기본 연락처를 삽입 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-119">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

<span data-ttu-id="58a07-120">참고: 파트너 센터에 위치를 추가한 후에는 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-120">Note: Once a location is added in Partner Center, it cannot be removed.</span></span>

<span data-ttu-id="58a07-121">**법률 본사 위치 변경**</span><span class="sxs-lookup"><span data-stu-id="58a07-121">**Change legal headquarters location**</span></span>

1. <span data-ttu-id="58a07-122">**위치 페이지에서** 위치 목록을 확인 하 여 법률 엔터티로 사용할 위치가 나열 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-122">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="58a07-123">그렇지 않은 경우 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-123">If it isn't, add it.</span></span>

![비즈니스 위치 업데이트](images/updatepartnerprofile2.png)

2. <span data-ttu-id="58a07-125">**파트너 프로필** 을 선택한 다음, **법적 비즈니스 프로필 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-125">Select **Partner profile** and then select **Update legal business profile**</span></span>

![비즈니스 위치 업데이트](images/updatepartnerprofile1.png)

3. <span data-ttu-id="58a07-127">지역 및 법률 엔터티를 선택 하 고 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="58a07-127">Select the region and legal entity and **Submit** it.</span></span>

![비즈니스 위치 업데이트](images/updatepartnerprofile3.png)

