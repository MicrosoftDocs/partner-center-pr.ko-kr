---
title: CSP 파트너 | 파트너 센터용 Cloudyn의 Azure 비용 관리
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn 웹 앱을 등록 하 고 파트너 센터에서 비밀 키를 사용 하는 방법을 알아보고, 앱을 사용 하 여 고객 Azure 사용량 및 비용을 추적할 수 있습니다.
author: Janet
ms.author: janet
Keywords: Azure cost management 앱, 비용 관리, 웹 앱
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253303"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="243e2-104">Azure CSP 파트너용 Azure 비용 관리 앱</span><span class="sxs-lookup"><span data-stu-id="243e2-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="243e2-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="243e2-105">**Applies to**</span></span>

- <span data-ttu-id="243e2-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="243e2-106">Partner Center</span></span>
- <span data-ttu-id="243e2-107">클라우드 솔루션 공급자 프로그램 파트너</span><span class="sxs-lookup"><span data-stu-id="243e2-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="243e2-108">**적절 한 역할**</span><span class="sxs-lookup"><span data-stu-id="243e2-108">**Appropriate roles**</span></span>

- <span data-ttu-id="243e2-109">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="243e2-109">Global admin</span></span>
- <span data-ttu-id="243e2-110">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="243e2-110">Admin agent</span></span>

[<span data-ttu-id="243e2-111">Azure Cost Management에 대 한 자세한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="243e2-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="243e2-112">시작하기 전 주의 사항</span><span class="sxs-lookup"><span data-stu-id="243e2-112">Before you begin</span></span>
<span data-ttu-id="243e2-113">Azure 비용 관리를 사용하려면 먼저 다음 요구 사항을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="243e2-114">클라우드 솔루션 공급자 프로그램의 파트너여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="243e2-115">파트너 센터 API 웹 앱을 만들 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="243e2-116">개요</span><span class="sxs-lookup"><span data-stu-id="243e2-116">Overview</span></span>

<span data-ttu-id="243e2-117">Cloudyn는 고객이 얼마나 많은 Azure를 사용 하 고 있는지를 추적 하 고 관리 하는 데 사용할 수 있는 웹 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="243e2-118">파트너 센터 API를 통해 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="243e2-119">파트너 센터에서 웹 앱 등록</span><span class="sxs-lookup"><span data-stu-id="243e2-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="243e2-120">파트너 센터에서 Azure Active Directory 웹 앱을 등록하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="243e2-121">[전역 관리자 또는 관리자 에이전트 계정](https://partnercenter.microsoft.com/pcv/dashboard/overview)을 사용하여 [파트너 센터](create-user-accounts-and-set-permissions.md)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="243e2-122">**파트너 센터**에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="243e2-123">**Web App** 섹션에서 **Add new web app**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="243e2-124">**참고**: 이전에 웹 앱을 만든 경우 3단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="243e2-125">웹 앱의 **Commerce ID** GUID 및 **App ID** GUID를 복사하고 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="243e2-126">30일 무료 평가판 Azure 비용 관리 앱을 사용하려면 두 ID가 모두 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="243e2-127">앱에 비밀 키를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="243e2-128">**Add key** 버튼 옆에 있는 드롭다운 목록에서 기간을 1년 또는 2년으로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="243e2-129">**Add key**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="243e2-130">비밀 키 값을 복사하고 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-130">Copy and save the secret key value.</span></span> <span data-ttu-id="243e2-131">30일 무료 평가판을 사용하려면 이 키가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="243e2-132">응용 프로그램 비밀 키는 만료 날짜가 긴 암호와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="243e2-133">나중에 사용할 수 있도록 키 값을 안전한 위치에 저장하십시오.</span><span class="sxs-lookup"><span data-stu-id="243e2-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="243e2-134">다음 단계</span><span class="sxs-lookup"><span data-stu-id="243e2-134">Next steps</span></span>
<span data-ttu-id="243e2-135">[30일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="243e2-136">평가판을 시작하려면 다음 세부 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="243e2-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="243e2-137">파트너 센터 로그인 자격 증명</span><span class="sxs-lookup"><span data-stu-id="243e2-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="243e2-138">Commerce ID GUID</span><span class="sxs-lookup"><span data-stu-id="243e2-138">Commerce ID GUID</span></span>
- <span data-ttu-id="243e2-139">App ID GUID</span><span class="sxs-lookup"><span data-stu-id="243e2-139">App ID GUID</span></span>
- <span data-ttu-id="243e2-140">응용 프로그램 비밀 키 값</span><span class="sxs-lookup"><span data-stu-id="243e2-140">Application secret key value</span></span>
