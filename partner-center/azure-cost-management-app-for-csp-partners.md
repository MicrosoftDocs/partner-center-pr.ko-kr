---
title: Csp에 대 한 Azure Cost Management Cloudyn
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn 웹 앱을 등록 하 고 파트너 센터에서 비밀 키를 사용 하는 방법을 알아보고, 앱을 사용 하 여 고객 Azure 사용량 및 비용을 추적할 수 있습니다.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure cost management 앱, 비용 관리, 웹 앱
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d88f37e0fe653c679df5729fa283336e4c7e144
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908371"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="cd135-104">CSP 파트너를 위한 Azure cost management 앱을 사용 하 여 고객 Azure 사용량 및 비용 추적</span><span class="sxs-lookup"><span data-stu-id="cd135-104">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="cd135-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="cd135-105">**Applies to**</span></span>

- <span data-ttu-id="cd135-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="cd135-106">Partner Center</span></span>
- <span data-ttu-id="cd135-107">클라우드 솔루션 공급자 프로그램 파트너</span><span class="sxs-lookup"><span data-stu-id="cd135-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="cd135-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="cd135-108">**Appropriate roles**</span></span>

- <span data-ttu-id="cd135-109">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="cd135-109">Global admin</span></span>
- <span data-ttu-id="cd135-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="cd135-110">Admin agent</span></span>

[<span data-ttu-id="cd135-111">Azure Cost Management에 대 한 자세한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="cd135-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="cd135-112">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="cd135-112">Before you begin</span></span>
<span data-ttu-id="cd135-113">Azure Cost Management를 사용 하려면 먼저 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="cd135-114">클라우드 솔루션 공급자 프로그램의 파트너입니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="cd135-115">파트너 센터 API 웹 앱을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="cd135-116">개요</span><span class="sxs-lookup"><span data-stu-id="cd135-116">Overview</span></span>

<span data-ttu-id="cd135-117">Cloudyn는 고객이 얼마나 많은 Azure를 사용 하 고 있는지를 추적 하 고 관리 하는 데 사용할 수 있는 웹 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="cd135-118">파트너 센터 API를 통해 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="cd135-119">파트너 센터에 웹 앱 등록</span><span class="sxs-lookup"><span data-stu-id="cd135-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="cd135-120">파트너 센터에 Azure Active Directory 웹 앱을 등록 하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="cd135-121">[전역 관리자 또는 관리 에이전트 계정을](create-user-accounts-and-set-permissions.md)사용 하 여 [파트너 센터](https://partnercenter.microsoft.com/pcv/dashboard/overview) 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="cd135-122">**파트너 센터**에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="cd135-123">**웹 앱** 섹션에서 **새 웹 앱 추가**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="cd135-124">**참고**: 이전에 웹 앱을 만든 경우 3 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="cd135-125">웹 앱에 대 한 **상거래 id** Guid 및 **앱 id** guid를 복사 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="cd135-126">Azure cost management 앱의 30 일 무료 평가판을 사용 하려면 두 Id가 모두 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="cd135-127">앱에 비밀 키 추가</span><span class="sxs-lookup"><span data-stu-id="cd135-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="cd135-128">**키 추가** 단추 옆의 드롭다운에서 기간을 1 또는 2 년으로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="cd135-129">**키 추가**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="cd135-130">비밀 키 값을 복사 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-130">Copy and save the secret key value.</span></span> <span data-ttu-id="cd135-131">이는 30 일 무료 평가판에 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="cd135-132">응용 프로그램 비밀 키는 만료 날짜가 긴 암호와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="cd135-133">나중에 사용 하기 위해 키 값을 안전한 위치에 저장 하세요.</span><span class="sxs-lookup"><span data-stu-id="cd135-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cd135-134">다음 단계</span><span class="sxs-lookup"><span data-stu-id="cd135-134">Next steps</span></span>
<span data-ttu-id="cd135-135">[30 일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="cd135-136">평가판을 시작 하려면 다음 정보가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd135-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="cd135-137">파트너 센터 로그인 자격 증명</span><span class="sxs-lookup"><span data-stu-id="cd135-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="cd135-138">상거래 ID GUID</span><span class="sxs-lookup"><span data-stu-id="cd135-138">Commerce ID GUID</span></span>
- <span data-ttu-id="cd135-139">앱 ID GUID</span><span class="sxs-lookup"><span data-stu-id="cd135-139">App ID GUID</span></span>
- <span data-ttu-id="cd135-140">응용 프로그램 비밀 키 값</span><span class="sxs-lookup"><span data-stu-id="cd135-140">Application secret key value</span></span>
