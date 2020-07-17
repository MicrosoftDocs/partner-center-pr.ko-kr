---
title: Csp에 대 한 Azure Cost Management Cloudyn
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn 웹 앱을 등록 하 고 파트너 센터에서 비밀 키를 사용 하는 방법을 알아보고, 앱을 사용 하 여 고객 Azure 사용량 및 비용을 추적할 수 있습니다.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435912"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="6858a-103">CSP 파트너를 위한 Azure cost management 앱을 사용 하 여 고객 Azure 사용량 및 비용 추적</span><span class="sxs-lookup"><span data-stu-id="6858a-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="6858a-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="6858a-104">**Applies to**</span></span>

- <span data-ttu-id="6858a-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="6858a-105">Partner Center</span></span>
- <span data-ttu-id="6858a-106">클라우드 솔루션 공급자 프로그램 파트너</span><span class="sxs-lookup"><span data-stu-id="6858a-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="6858a-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="6858a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="6858a-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="6858a-108">Global admin</span></span>
- <span data-ttu-id="6858a-109">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="6858a-109">Admin agent</span></span>

[<span data-ttu-id="6858a-110">Azure Cost Management에 대 한 자세한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="6858a-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="6858a-111">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="6858a-111">Before you begin</span></span>
<span data-ttu-id="6858a-112">Azure Cost Management를 사용 하려면 먼저 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="6858a-113">클라우드 솔루션 공급자 프로그램의 파트너입니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="6858a-114">파트너 센터 API 웹 앱을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="6858a-115">개요</span><span class="sxs-lookup"><span data-stu-id="6858a-115">Overview</span></span>

<span data-ttu-id="6858a-116">Cloudyn는 고객이 얼마나 많은 Azure를 사용 하 고 있는지를 추적 하 고 관리 하는 데 사용할 수 있는 웹 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="6858a-117">파트너 센터 API를 통해 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="6858a-118">파트너 센터에 웹 앱 등록</span><span class="sxs-lookup"><span data-stu-id="6858a-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="6858a-119">파트너 센터에 Azure Active Directory 웹 앱을 등록 하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="6858a-120">[전역 관리자 또는 관리 에이전트 계정을](create-user-accounts-and-set-permissions.md)사용 하 여 [파트너 센터](https://partnercenter.microsoft.com/pcv/dashboard/overview) 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="6858a-121">**파트너 센터**에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-121">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="6858a-122">**웹 앱** 섹션에서 **새 웹 앱 추가**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-122">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="6858a-123">**참고**: 이전에 웹 앱을 만든 경우 3 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-123">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="6858a-124">웹 앱에 대 한 **상거래 id** Guid 및 **앱 id** guid를 복사 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="6858a-125">Azure cost management 앱의 30 일 무료 평가판을 사용 하려면 두 Id가 모두 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="6858a-126">앱에 비밀 키 추가</span><span class="sxs-lookup"><span data-stu-id="6858a-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="6858a-127">**키 추가** 단추 옆의 드롭다운에서 기간을 1 또는 2 년으로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="6858a-128">**키 추가**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-128">Click **Add key**.</span></span> 
3. <span data-ttu-id="6858a-129">비밀 키 값을 복사 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-129">Copy and save the secret key value.</span></span> <span data-ttu-id="6858a-130">이는 30 일 무료 평가판에 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="6858a-131">응용 프로그램 비밀 키는 만료 날짜가 긴 암호와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="6858a-132">나중에 사용 하기 위해 키 값을 안전한 위치에 저장 하세요.</span><span class="sxs-lookup"><span data-stu-id="6858a-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6858a-133">다음 단계</span><span class="sxs-lookup"><span data-stu-id="6858a-133">Next steps</span></span>
<span data-ttu-id="6858a-134">[30 일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="6858a-135">평가판을 시작 하려면 다음 정보가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="6858a-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="6858a-136">파트너 센터 로그인 자격 증명</span><span class="sxs-lookup"><span data-stu-id="6858a-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="6858a-137">상거래 ID GUID</span><span class="sxs-lookup"><span data-stu-id="6858a-137">Commerce ID GUID</span></span>
- <span data-ttu-id="6858a-138">앱 ID GUID</span><span class="sxs-lookup"><span data-stu-id="6858a-138">App ID GUID</span></span>
- <span data-ttu-id="6858a-139">응용 프로그램 비밀 키 값</span><span class="sxs-lookup"><span data-stu-id="6858a-139">Application secret key value</span></span>
