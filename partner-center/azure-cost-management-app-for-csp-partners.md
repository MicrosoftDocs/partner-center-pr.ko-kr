---
title: CSP 파트너 | 파트너 센터용 Cloudyn의 Azure 비용 관리
ms.topic: article
ms.date: 10/29/2018
description: Cloudyn의 Azure 비용 관리를 사용하려면 파트너 센터 API에 프로비전된 액세스가 필요합니다.
author: Janet
ms.author: janet
Keywords: Azure 비용 관리 앱에 비용을 관리, 웹 앱
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586086"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="d0f22-104">Azure CSP 파트너용 Azure 비용 관리 앱</span><span class="sxs-lookup"><span data-stu-id="d0f22-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="d0f22-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="d0f22-105">**Applies to**</span></span>

-  <span data-ttu-id="d0f22-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="d0f22-106">Partner Center</span></span>

[<span data-ttu-id="d0f22-107">Azure Cost Management에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="d0f22-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="d0f22-108">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="d0f22-108">Before you begin</span></span>
<span data-ttu-id="d0f22-109">Azure 비용 관리를 사용하려면 먼저 다음 요구 사항을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="d0f22-110">클라우드 솔루션 공급자 프로그램의 파트너여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="d0f22-111">파트너 센터 API 웹 앱을 만들 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="d0f22-112">개요</span><span class="sxs-lookup"><span data-stu-id="d0f22-112">Overview</span></span>

<span data-ttu-id="d0f22-113">Cloudyn의 Azure 비용 관리는 고객이 Azure를 사용하는 정도와 사용 비용을 추적하고 관리할 수 있는 웹 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-113">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="d0f22-114">파트너 센터 API를 통해 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="d0f22-115">파트너 센터에서 웹 앱 등록</span><span class="sxs-lookup"><span data-stu-id="d0f22-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="d0f22-116">파트너 센터에서 Azure Active Directory 웹 앱을 등록하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="d0f22-117">[전역 관리자 또는 관리자 에이전트 계정](create-user-accounts-and-set-permissions.md)을 사용하여 [파트너 센터](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="d0f22-118">**파트너 센터**를 선택 **계정 설정** &gt;  **[앱 관리](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="d0f22-119">**Web App** 섹션에서 **Add new web app**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="d0f22-120">**참고**: 웹 앱을 이전에 만든 경우 3 단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="d0f22-121">웹 앱의 **Commerce ID** GUID 및 **App ID** GUID를 복사하고 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="d0f22-122">30일 무료 평가판 Azure 비용 관리 앱을 사용하려면 두 ID가 모두 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="d0f22-123">앱에 비밀 키를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="d0f22-124">**Add key** 버튼 옆에 있는 드롭다운 목록에서 기간을 1년 또는 2년으로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="d0f22-125">**Add key**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="d0f22-126">비밀 키 값을 복사하고 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-126">Copy and save the secret key value.</span></span> <span data-ttu-id="d0f22-127">30일 무료 평가판을 사용하려면 이 키가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="d0f22-128">응용 프로그램 비밀 키 긴 만료 날짜를 사용 하 여 암호와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="d0f22-129">나중에 사용할 수 있도록 키 값을 안전한 위치에 저장하십시오.</span><span class="sxs-lookup"><span data-stu-id="d0f22-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0f22-130">다음 단계</span><span class="sxs-lookup"><span data-stu-id="d0f22-130">Next steps</span></span>
<span data-ttu-id="d0f22-131">[30일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="d0f22-132">평가판을 시작하려면 다음 세부 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="d0f22-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="d0f22-133">파트너 센터 로그인 자격 증명</span><span class="sxs-lookup"><span data-stu-id="d0f22-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="d0f22-134">Commerce ID GUID</span><span class="sxs-lookup"><span data-stu-id="d0f22-134">Commerce ID GUID</span></span>
- <span data-ttu-id="d0f22-135">App ID GUID</span><span class="sxs-lookup"><span data-stu-id="d0f22-135">App ID GUID</span></span>
- <span data-ttu-id="d0f22-136">응용 프로그램 비밀 키 값</span><span class="sxs-lookup"><span data-stu-id="d0f22-136">Application secret key value</span></span>
