---
title: CSP 파트너 | 파트너 센터용 Cloudyn의 Azure 비용 관리
ms.topic: article
ms.date: 10/29/2018
description: Cloudyn의 Azure 비용 관리를 사용하려면 파트너 센터 API에 프로비전된 액세스가 필요합니다.
author: Janet
ms.author: janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995797"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="94cf5-103">Azure CSP 파트너용 Azure 비용 관리 앱</span><span class="sxs-lookup"><span data-stu-id="94cf5-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="94cf5-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="94cf5-104">Applies to</span></span>**

-  <span data-ttu-id="94cf5-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="94cf5-105">Partner Center</span></span>

[<span data-ttu-id="94cf5-106">Azure 비용 관리에 대한 자세한 정보 얻기</span><span class="sxs-lookup"><span data-stu-id="94cf5-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="94cf5-107">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="94cf5-107">Before you begin</span></span>
<span data-ttu-id="94cf5-108">Azure 비용 관리를 사용하려면 먼저 다음 요구 사항을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="94cf5-109">클라우드 솔루션 공급자 프로그램의 파트너여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="94cf5-110">파트너 센터 API 웹 앱을 만들 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="94cf5-111">개요</span><span class="sxs-lookup"><span data-stu-id="94cf5-111">Overview</span></span>

<span data-ttu-id="94cf5-112">Cloudyn의 Azure 비용 관리는 고객이 Azure를 사용하는 정도와 사용 비용을 추적하고 관리할 수 있는 웹 앱입니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="94cf5-113">파트너 센터 API를 통해 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="94cf5-114">파트너 센터에서 웹 앱 등록</span><span class="sxs-lookup"><span data-stu-id="94cf5-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="94cf5-115">파트너 센터에서 Azure Active Directory 웹 앱을 등록하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="94cf5-116">[전역 관리자 또는 관리자 에이전트 계정](create-user-accounts-and-set-permissions.md)을 사용하여 [파트너 센터](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="94cf5-117">**파트너 센터**에서 **계정 설정** 선택 &gt; **[앱 관리](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** 합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-117">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="94cf5-118">**Web App** 섹션에서 **Add new web app**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="94cf5-119">**참고**: 이전에 웹 앱을 만든 경우 3단계를 건너뛸 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="94cf5-120">웹 앱의 **Commerce ID** GUID 및 **App ID** GUID를 복사하고 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="94cf5-121">30일 무료 평가판 Azure 비용 관리 앱을 사용하려면 두 ID가 모두 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="94cf5-122">앱에 비밀 키를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-122">Add a secret key to your app</span></span>
1. <span data-ttu-id="94cf5-123">**Add key** 버튼 옆에 있는 드롭다운 목록에서 기간을 1년 또는 2년으로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="94cf5-124">**Add key**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-124">Click **Add key**.</span></span> 
3. <span data-ttu-id="94cf5-125">비밀 키 값을 복사하고 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-125">Copy and save the secret key value.</span></span> <span data-ttu-id="94cf5-126">30일 무료 평가판을 사용하려면 이 키가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-126">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="94cf5-127">응용 프로그램 비밀 키는 만료 날짜가 더 긴 암호와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-127">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="94cf5-128">나중에 사용할 수 있도록 키 값을 안전한 위치에 저장하십시오.</span><span class="sxs-lookup"><span data-stu-id="94cf5-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="94cf5-129">다음 단계</span><span class="sxs-lookup"><span data-stu-id="94cf5-129">Next steps</span></span>
<span data-ttu-id="94cf5-130">[30일 무료 평가판](https://go.microsoft.com/fwlink/?linkid=857895)을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="94cf5-131">평가판을 시작하려면 다음 세부 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="94cf5-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="94cf5-132">파트너 센터 로그인 자격 증명</span><span class="sxs-lookup"><span data-stu-id="94cf5-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="94cf5-133">Commerce ID GUID</span><span class="sxs-lookup"><span data-stu-id="94cf5-133">Commerce ID GUID</span></span>
- <span data-ttu-id="94cf5-134">App ID GUID</span><span class="sxs-lookup"><span data-stu-id="94cf5-134">App ID GUID</span></span>
- <span data-ttu-id="94cf5-135">응용 프로그램 비밀 키 값</span><span class="sxs-lookup"><span data-stu-id="94cf5-135">Application secret key value</span></span>
