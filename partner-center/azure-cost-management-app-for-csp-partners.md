---
title: CSP용 Cloudyn별 Azure Cost Management
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn 웹 앱을 등록 하 고 파트너 센터에서 비밀 키를 사용 하는 방법을 알아보고, 앱을 사용 하 여 고객 Azure 사용량 및 비용을 추적할 수 있습니다.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534994"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="103cf-103">CSP 파트너를 위한 Azure cost management 앱을 사용 하 여 고객 Azure 사용량 및 비용 추적</span><span class="sxs-lookup"><span data-stu-id="103cf-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="103cf-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="103cf-104">**Appropriate roles**</span></span>

- <span data-ttu-id="103cf-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="103cf-105">Global admin</span></span>
- <span data-ttu-id="103cf-106">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="103cf-106">Admin agent</span></span>

[<span data-ttu-id="103cf-107">Azure Cost Management에 대 한 자세한 정보 보기</span><span class="sxs-lookup"><span data-stu-id="103cf-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="103cf-108">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="103cf-108">Before you begin</span></span>
<span data-ttu-id="103cf-109">Azure Cost Management를 사용 하려면 먼저 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="103cf-110">클라우드 솔루션 공급자 프로그램의 파트너입니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="103cf-111">파트너 센터 API 웹 앱을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="103cf-112">개요</span><span class="sxs-lookup"><span data-stu-id="103cf-112">Overview</span></span>

<span data-ttu-id="103cf-113">Cloudyn는 고객이 얼마나 많은 Azure를 사용 하 고 있는지를 추적 하 고 관리 하는 데 사용할 수 있는 웹 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="103cf-114">파트너 센터 API를 통해 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="103cf-115">파트너 센터에 웹 앱 등록</span><span class="sxs-lookup"><span data-stu-id="103cf-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="103cf-116">파트너 센터에 Azure Active Directory 웹 앱을 등록 하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="103cf-117">[전역 관리자 또는 관리 에이전트 계정을](create-user-accounts-and-set-permissions.md)사용 하 여 [파트너 센터](https://partnercenter.microsoft.com/pcv/dashboard/overview) 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="103cf-118">**파트너 센터** 에서 **계정 설정** &gt; **[앱 관리](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="103cf-119">**웹 앱** 섹션에서 **새 웹 앱 추가** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="103cf-120">**참고**: 이전에 웹 앱을 만든 경우 3 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="103cf-121">웹 앱에 대 한 **상거래 id** Guid 및 **앱 id** guid를 복사 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="103cf-122">Azure cost management 앱의 30 일 무료 평가판을 사용 하려면 두 Id가 모두 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="103cf-123">앱에 비밀 키 추가</span><span class="sxs-lookup"><span data-stu-id="103cf-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="103cf-124">**키 추가** 단추 옆의 드롭다운에서 기간을 1 또는 2 년으로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="103cf-125">**키 추가** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="103cf-126">비밀 키 값을 복사 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-126">Copy and save the secret key value.</span></span> <span data-ttu-id="103cf-127">이는 30 일 무료 평가판에 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="103cf-128">응용 프로그램 비밀 키는 만료 날짜가 긴 암호와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="103cf-129">나중에 사용 하기 위해 키 값을 안전한 위치에 저장 하세요.</span><span class="sxs-lookup"><span data-stu-id="103cf-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="103cf-130">다음 단계</span><span class="sxs-lookup"><span data-stu-id="103cf-130">Next steps</span></span>
<span data-ttu-id="103cf-131">[30 일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="103cf-132">평가판을 시작 하려면 다음 정보가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="103cf-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="103cf-133">파트너 센터 로그인 자격 증명</span><span class="sxs-lookup"><span data-stu-id="103cf-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="103cf-134">상거래 ID GUID</span><span class="sxs-lookup"><span data-stu-id="103cf-134">Commerce ID GUID</span></span>
- <span data-ttu-id="103cf-135">앱 ID GUID</span><span class="sxs-lookup"><span data-stu-id="103cf-135">App ID GUID</span></span>
- <span data-ttu-id="103cf-136">응용 프로그램 비밀 키 값</span><span class="sxs-lookup"><span data-stu-id="103cf-136">Application secret key value</span></span>
