---
title: Customer insights에 대 한 분석 사용
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 분석을 사용 하 여 비즈니스와 고객이 구매한 라이선스를 사용 하는 방법을 더 잘 이해 하는 방법을 알아보세요.
author: LauraBrenner
ms.author: labrenne
keywords: 데이터, 분석, 데이터 분석, power bi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3232a8c5b2f3e0bb4458dffdc577cbd561064dae
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795207"
---
# <a name="use-analytics-to-learn-more-about-customer-license-use-and-how-you-can-help-meet-their-needs"></a><span data-ttu-id="2dac7-104">분석을 사용 하 여 고객 라이선스 사용에 대 한 자세한 내용 및 고객의 요구를 충족 하는 데 도움이 되는 방법</span><span class="sxs-lookup"><span data-stu-id="2dac7-104">Use analytics to learn more about customer license use and how you can help meet their needs</span></span>

<span data-ttu-id="2dac7-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="2dac7-105">**Applies to**</span></span>

- <span data-ttu-id="2dac7-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="2dac7-106">Partner Center</span></span>
- <span data-ttu-id="2dac7-107">MPN 파트너</span><span class="sxs-lookup"><span data-stu-id="2dac7-107">MPN partners</span></span>
- <span data-ttu-id="2dac7-108">CSP 프로그램의 파트너</span><span class="sxs-lookup"><span data-stu-id="2dac7-108">Partners in the CSP program</span></span>

<span data-ttu-id="2dac7-109">**적절 한 역할**</span><span class="sxs-lookup"><span data-stu-id="2dac7-109">**Appropriate role**</span></span>

- <span data-ttu-id="2dac7-110">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="2dac7-110">MPN Partner admin</span></span>

<span data-ttu-id="2dac7-111">CSP 비즈니스 개발 계획을 작성하려면 고객이 Microsoft 제품을 어떻게 사용하는지 이해해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-111">Planning ways to develop your CSP business includes understanding how your customers use their Microsoft products.</span></span> <span data-ttu-id="2dac7-112">파트너 센터에서 데이터를 수집 하기 위한 몇 가지 옵션이 있으며, 비즈니스와 고객이 구매한 라이선스를 사용 하 고 있는 경우에는 데이터를 수집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-112">You have several options for gathering data in Partner Center, and you can gather data on both your business and on if and how your customers are using the licenses they've purchased.</span></span> <span data-ttu-id="2dac7-113">CSP 직접 모델을 사용 하는 경우 추가 데이터를 수집 하기 위해 Power BI 위해 파트너 센터 분석 앱을 설치 하 고 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-113">If you are in the CSP direct model, you have the opportunity to install and use the Partner Center Analytics app for Power BI to gather additional data.</span></span>

## <a name="access-to-user-analytics"></a><span data-ttu-id="2dac7-114">사용자 분석에 대 한 액세스</span><span class="sxs-lookup"><span data-stu-id="2dac7-114">Access to user analytics</span></span>

<span data-ttu-id="2dac7-115">파트너 센터에서는 MPN 파트너 관리자만 사용자 분석에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-115">In Partner Center, only the MPN partner admin has access to user analytics.</span></span> <span data-ttu-id="2dac7-116">회사의 누군가가이 액세스를 요구 하는 경우 (예: 대금 청구 관리자) 해당 사용자를 MPN Partner Admin 역할에 할당 하 여 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-116">If someone in your company needs this access (for example, a billing admin), you can grant it by assigning that person the MPN Partner Admin role.</span></span>

>[!NOTE] 
><span data-ttu-id="2dac7-117">액세스 권한을 부여 하려면 MPN 파트너 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-117">To grant access, you must be an MPN partner admin.</span></span>

<span data-ttu-id="2dac7-118">**파트너 센터에서 사용자 분석에 대 한 액세스 권한 부여**</span><span class="sxs-lookup"><span data-stu-id="2dac7-118">**Grant access to user analytics in Partner Center**</span></span> 

1. <span data-ttu-id="2dac7-119">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2dac7-120">파트너 센터 메뉴의 파트너 센터 **사용자 관리** 페이지에서 검색 상자를 사용 하 여 액세스 해야 하는 사용자를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-120">From the Partner Center menu, On the Partner Center **User management** page, use the Search box to find the person who needs access.</span></span>
2.  <span data-ttu-id="2dac7-121">검색 결과에서 사용자의 이름을 선택 하 여 **사용자 세부 정보** 페이지를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-121">In the search results, select the person's name to open the **User details** page.</span></span>
3.  <span data-ttu-id="2dac7-122">**역할 및 권한**에서 **MPN partner admin** 을 선택 하 고 **업데이트**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2dac7-122">Under **Roles and permissions**, select **MPN partner admin** and then select **Update**.</span></span>

 
## <a name="access-data-in-partner-center"></a><span data-ttu-id="2dac7-123">파트너 센터에서 데이터 액세스</span><span class="sxs-lookup"><span data-stu-id="2dac7-123">Access data in Partner Center</span></span>

|<span data-ttu-id="2dac7-124">**데이터를 가져오려면**</span><span class="sxs-lookup"><span data-stu-id="2dac7-124">**To get data on**</span></span>   |<span data-ttu-id="2dac7-125">**다운로드**</span><span class="sxs-lookup"><span data-stu-id="2dac7-125">**Download this**</span></span>   |<span data-ttu-id="2dac7-126">**이 글 읽기**</span><span class="sxs-lookup"><span data-stu-id="2dac7-126">**Read this**</span></span>   | <span data-ttu-id="2dac7-127">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="2dac7-127">**Applies to**</span></span>    |
|---------------------|:-----------------------|:---------------|:--------------|
|<span data-ttu-id="2dac7-128">고객이 구매한 라이선스를 사용 하는 방법</span><span class="sxs-lookup"><span data-stu-id="2dac7-128">How your customers are using the licenses they purchased</span></span>   |<span data-ttu-id="2dac7-129">파트너 센터 => 제품 분석의 배포 및 사용 현황 데이터</span><span class="sxs-lookup"><span data-stu-id="2dac7-129">Deployment and usage data from Partner Center => Product analytics</span></span>   |[<span data-ttu-id="2dac7-130">채택률 및 만족도 높이기</span><span class="sxs-lookup"><span data-stu-id="2dac7-130">Increase adoption and satisfaction</span></span>](increasing-adoption-and-satisfaction.md)|<span data-ttu-id="2dac7-131">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="2dac7-131">CSP partners</span></span>|
|<span data-ttu-id="2dac7-132">구독과 관련 된 고객 활동</span><span class="sxs-lookup"><span data-stu-id="2dac7-132">Customer activity regarding subscriptions</span></span>   |<span data-ttu-id="2dac7-133">활동 로그</span><span class="sxs-lookup"><span data-stu-id="2dac7-133">Activity logs</span></span>   |[<span data-ttu-id="2dac7-134">고객 활동 로그 보기</span><span class="sxs-lookup"><span data-stu-id="2dac7-134">View customer activity logs</span></span>](activity-logs.md)|<span data-ttu-id="2dac7-135">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="2dac7-135">CSP partners</span></span>   |
|<span data-ttu-id="2dac7-136">고객 기준, 사용량, Azure 소비 등의 성장</span><span class="sxs-lookup"><span data-stu-id="2dac7-136">Growth of customer base, usage, Azure consumption and more</span></span>   |<span data-ttu-id="2dac7-137">Power BI에 대 한 파트너 센터 앱</span><span class="sxs-lookup"><span data-stu-id="2dac7-137">Partner Center app for Power BI</span></span>   |[<span data-ttu-id="2dac7-138">Power BI용 파트너 센터 Analytics 앱(CSP의 직접 파트너)</span><span class="sxs-lookup"><span data-stu-id="2dac7-138">Partner Center Analytics app for Power BI (direct partners in CSP)</span></span>](power-bi-app-for-direct-partners.md)|<span data-ttu-id="2dac7-139">CSP 직접 파트너</span><span class="sxs-lookup"><span data-stu-id="2dac7-139">CSP direct partners</span></span>|






