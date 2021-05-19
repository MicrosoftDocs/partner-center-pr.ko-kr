---
title: 마켓플레이스 제품의 라이선스 관리
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV 상업용 Marketplace 제안에 대한 라이선스를 설정하고 관리하는 방법을 알아봅니다.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147958"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="f9532-103">마켓플레이스 제품의 라이선스 관리</span><span class="sxs-lookup"><span data-stu-id="f9532-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="f9532-104">**적절한 역할:** 전역 관리자 | 계정 관리자</span><span class="sxs-lookup"><span data-stu-id="f9532-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="f9532-105">이 문서에서는 파트너 센터 제안을 설정하고, Microsoft AppSource 사용할 수 있게 한 다음, 해당 제안에 대한 라이선스를 관리하는 프로세스를 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-105">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="f9532-106">이 문서의 기능은 현재 공개 미리 보기로 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-106">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="f9532-107">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="f9532-107">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="f9532-108">상업용 마켓플레이스 기본 사항</span><span class="sxs-lookup"><span data-stu-id="f9532-108">Commercial marketplace basics</span></span>

<span data-ttu-id="f9532-109">이 프로세스를 시작하기 전에 상업용 Marketplace의 기본 사항들을 숙지해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-109">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="f9532-110">아래 표의 문서는 시작하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-110">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="f9532-111">토픽</span><span class="sxs-lookup"><span data-stu-id="f9532-111">Topic</span></span>  | <span data-ttu-id="f9532-112">아티클</span><span class="sxs-lookup"><span data-stu-id="f9532-112">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="f9532-113">상업용 마켓플레이스 플랜</span><span class="sxs-lookup"><span data-stu-id="f9532-113">Commercial marketplace plans</span></span> | [<span data-ttu-id="f9532-114">상업용 마켓플레이스 제품에 대한 요금제 및 가격 책정</span><span class="sxs-lookup"><span data-stu-id="f9532-114">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="f9532-115">상업용 마켓플레이스 제안</span><span class="sxs-lookup"><span data-stu-id="f9532-115">Commercial marketplace offers</span></span>  | [<span data-ttu-id="f9532-116">목록 유형</span><span class="sxs-lookup"><span data-stu-id="f9532-116">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="f9532-117">상업용 마켓플레이스 계정</span><span class="sxs-lookup"><span data-stu-id="f9532-117">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="f9532-118">파트너 센터에서 상업용 마켓플레이스 계정 관리</span><span class="sxs-lookup"><span data-stu-id="f9532-118">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="f9532-119">제안 ID 확인</span><span class="sxs-lookup"><span data-stu-id="f9532-119">Determine your Offer ID</span></span>

<span data-ttu-id="f9532-120">아래 절차에서는 제안 ID를 입력하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-120">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="f9532-121">이제 다음 사항에 유의하여 적절한 제안 ID를 생각해보십시오.</span><span class="sxs-lookup"><span data-stu-id="f9532-121">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="f9532-122">이 ID는 마켓플레이스 제품 및 Azure Resource Manager 템플릿의 웹 주소에서 고객에게 표시됩니다(해당하는 경우).</span><span class="sxs-lookup"><span data-stu-id="f9532-122">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="f9532-123">게시자 ID와 결합된 제품 ID의 길이는 40자 미만이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-123">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="f9532-124">소문자와 숫자만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-124">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="f9532-125">제안 ID에는 하이픈과 밑줄이 포함될 수 있지만 공백은 포함될 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-125">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="f9532-126">예를 들어 게시자 ID가 `testpublisherid` 이고 를 입력하면 제안 웹 주소는 가 `test-offer-1` `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-126">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="f9532-127">이 ID는 **만들기** 를 선택한 후에는 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-127">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="f9532-128">제안 별칭 확인</span><span class="sxs-lookup"><span data-stu-id="f9532-128">Determine your Offer alias</span></span>

<span data-ttu-id="f9532-129">제안 별칭은 파트너 센터 제안에 사용되는 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-129">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="f9532-130">또한 아래 지침을 따르는 적절한 제안 별칭이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-130">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="f9532-131">이 이름은 마켓플레이스에서 사용되지 않으며 고객에게 표시되는 제품 이름 및 기타 값과 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-131">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="f9532-132">이 이름은 만들기를 선택한 후에는 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-132">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="f9532-133">제품 만들기</span><span class="sxs-lookup"><span data-stu-id="f9532-133">Create your offer</span></span>

<span data-ttu-id="f9532-134">라이선스 프로세스의 첫 번째 단계는 상업용 Marketplace 제안을 만드는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-134">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="f9532-135">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-135">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f9532-136">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-136">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="f9532-137">개요 페이지의 맨 위에서 **새 제품** 을 선택 하 고 **고객 Engagement & PowerApps에 대해 Dynamics 365을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-137">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="f9532-138">이전에 만든 **제품 ID** 및 제품 **별칭** 을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-138">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="f9532-139">**만들기** 를 선택하여 제품을 생성하고 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-139">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="f9532-140">라이선스 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-140">Choose your licensing options.</span></span>

    - <span data-ttu-id="f9532-141">제품에 대 한 라이선스 관리를 사용 하도록 설정 하려면 **Microsoft에서 앱 라이선스 관리 사용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-141">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="f9532-142">이는 일회성 설정 이며 제품이 게시 된 후에는 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-142">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="f9532-143">고객이 라이선스 없이 앱의 기본 기능을 실행 하도록 설정 하 고, 라이선스를 구매한 후에 프리미엄 기능을 실행할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-143">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="f9532-144">이렇게 하려면 **라이선스가 할당 되지 않은 경우에도 고객이 앱을 설치할 수 있도록 허용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-144">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="f9532-145">제품에서 라이선스 관리를 사용 하도록 설정 하지 않으려는 경우 **지금 받기 (무료)**, **무료 평가판** 또는 **문의처** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-145">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="f9532-146">계획 만들기</span><span class="sxs-lookup"><span data-stu-id="f9532-146">Create your plan</span></span>

<span data-ttu-id="f9532-147">이러한 단계에서는 제품에 대해 사용 하도록 설정 하려는 계획을 정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-147">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="f9532-148">왼쪽 탐색 메뉴에서 **계획 개요** 를 선택한 다음 **새 계획 만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-148">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="f9532-149">**계획 ID** 및 **계획 이름을** 입력 하 고 **만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-149">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="f9532-150">**계획 목록** 페이지에서 **계획 설명을** 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-150">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="f9532-151">설명을 저장 하 고 나중에 완료 하려면 **초안 저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-151">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="f9532-152">완료 되 면 **검토 및 게시** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-152">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="f9532-153">이제 계획 정보가 제품 목록 (계획 섹션) 아래 appsource.microsoft.com에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-153">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="f9532-154">이 제품에 대 한 모든 계획을 만든 후에는 각 계획의 서비스 ID를 복사 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-154">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="f9532-155">계획 목록 페이지의 맨 위에서 **계획 개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-155">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="f9532-156">각 계획에 대 한 서비스 ID를 안전한 위치에 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-156">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="f9532-157">솔루션에 서비스 Id 추가</span><span class="sxs-lookup"><span data-stu-id="f9532-157">Add Service IDs to your solution</span></span>

<span data-ttu-id="f9532-158">다음 단계는 방금 복사한 각 계획에 대한 서비스 ID를 추가하여 솔루션을 업데이트하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-158">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="f9532-159">이에 대한 지침은 [솔루션에 대한 AppSource 패키지 만들기를 참조하세요.](/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="f9532-159">For guidance on this, see [Create an AppSource Package for your solution](/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="f9532-160">패키지 업로드 및 제안 게시</span><span class="sxs-lookup"><span data-stu-id="f9532-160">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="f9532-161">왼쪽 탐색 창에서 **상업용 Marketplace** 를 선택한 다음, **기술 구성을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-161">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="f9532-162">**기본 라이선스 모델에서** **사용자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-162">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="f9532-163">**CRM 패키지** 에서 패키지 위치의 URL을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-163">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="f9532-164">왼쪽 탐색 창의 다른 탭을 사용하여 다른 필수 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-164">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="f9532-165">완료되면 **검토 및 게시를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-165">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="f9532-166">제안을 게시한 후에는 정보를 검토하고 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-166">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="f9532-167">이 프로세스에 문제가 있는 경우 알려드리겠습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-167">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="f9532-168">모든 문제가 해결되면 AppSource에서 제안을 사용할 수 있다는 알림이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-168">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="f9532-169">이 시점에서 라이브로 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-169">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="f9532-170">파트너 센터 라이브로 제공</span><span class="sxs-lookup"><span data-stu-id="f9532-170">Make your offer live in Partner Center</span></span>

<span data-ttu-id="f9532-171">아래 절차에서는 AppSource에서 제안을 라이브로 만드는 과정을 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-171">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="f9532-172">이 프로세스에 대한 자세한 내용은 [목록 옵션 소개를 참조하세요.](/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="f9532-172">To learn more about this process, see [Introduction to listing options](/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="f9532-173">제안을 게시하면 라이브로 이동하는 데 4-6시간이 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-173">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="f9532-174">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-174">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f9532-175">왼쪽 탐색 메뉴에서 **상업용 Marketplace/개요를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-175">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="f9532-176">**개요** 페이지에서 찾고 있는 제안을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-176">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="f9532-177">게시할 준비가 된 제안의 상태는 **미리 보기** 입니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-177">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="f9532-178">제안을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-178">Select the offer.</span></span>
4. <span data-ttu-id="f9532-179">**제품 개요** 페이지에서 **라이브 이동** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-179">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="f9532-180">제품은 4-6 시간 이내에 라이브 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-180">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="f9532-181">AppSource에 대 한 제품 목록을 보려면 **제품 개요** 페이지의 맨 아래에 있는 **appsource** 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-181">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="f9532-182">**라이선스가 지원 되는 제품의** 경우: 제품에 라이선스 확인이 필요한 경우 사용자는 연락처를 클릭 하 여 잠재 고객에 **게 연락** 하 여 통신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-182">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="f9532-183">**무료 설치 옵션을 사용 하는 라이선스 사용 제품의** 경우: 제품에 라이선스 확인이 필요 하지 않은 경우 관리자에 **게 연락** 뿐만 아니라 **지금 가져오기** 단추가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-183">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="f9532-184">무료 설치 옵션을 시도 하려는 사용자는 **지금 가져오기** 를 클릭 해야 합니다. 그러면 Power Platform 관리 센터에 제품을 설치 하 게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-184">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="f9532-185">사용자는 궁금한 점이 있거나 유료 요금제로 업그레이드 하려는 경우에도 사용자 **에 게 연락** 하는 것을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-185">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="f9532-186">ISV 연결을 위한 등록 처리 등록</span><span class="sxs-lookup"><span data-stu-id="f9532-186">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="f9532-187">고객에 게 라이선스를 할당 하려면 먼저 각 판매를 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-187">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="f9532-188">이렇게 하려면 [거래 등록](register-deals.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="f9532-188">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="f9532-189">고객 초대</span><span class="sxs-lookup"><span data-stu-id="f9532-189">Invite the customer</span></span>

<span data-ttu-id="f9532-190">다음 절차를 사용 하 여 고객에 게이 거래에 참여할 수 있도록 초대 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-190">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="f9532-191">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-191">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f9532-192">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-192">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="f9532-193">왼쪽 탐색 메뉴에서 **조회** 를 선택 하 고 **거래 등록** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-193">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="f9532-194">**제출** 된 거래에 대해 필터링 하 고 **진행** 중인 탭을 선택한 후 원하는 거래를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-194">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="f9532-195">이 거래의 개요 페이지에서 **라이선스 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-195">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="f9532-196">**라이선스 관리** 창의 **고객 세부 정보** 드롭다운 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-196">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="f9532-197">고객 관계가 아직 없는 경우 **+ 새 고객 초대를 선택 하 여 동의** 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-197">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="f9532-198">표시 되는 링크를 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-198">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="f9532-199">이 링크를 고객의 청구 관리자 또는 전역 관리자에 게 전자 메일로 보내고,이 링크를 사용 하 여 admin.microsoft.com에 액세스 하 고, 사용자가 설정 하는 관계를 승인 하 고 권한을 부여 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-199">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="f9532-200">고객이 이 단계를 수행할 때까지 관계가 설정되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-200">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="f9532-201">라이선스 활성화, 관리 및 제거</span><span class="sxs-lookup"><span data-stu-id="f9532-201">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="f9532-202">고객이 사용자와의 관계에 권한을 부여하면 제안에서 계획을 추가하고 각 플랜에 라이선스를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-202">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="f9532-203">이 계약의 라이선스 관리 창에서 **+계획 추가를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-203">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="f9532-204">이 **솔루션에 대한 계획** 및 **라이선스 수** 필드를 완료한 다음, 라이선스 **업데이트를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="f9532-204">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="f9532-205">고객이 직원을 관리하고 할당할 수 있도록 admin.microsoft.com 라이선스를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9532-205">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="f9532-206">기존 플랜의 라이선스 수를 변경하려면 **라이선스 수** 필드에 새 번호를 입력한 **다음, 라이선스 업데이트를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="f9532-206">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="f9532-207">거래 라이선스를 비활성화하거나 제거하려면 **작업** 필드에서 휴지통 아이콘을 선택한 **다음, 라이선스 업데이트를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="f9532-207">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9532-208">다음 단계</span><span class="sxs-lookup"><span data-stu-id="f9532-208">Next steps</span></span>

[<span data-ttu-id="f9532-209">라이선스 리소스</span><span class="sxs-lookup"><span data-stu-id="f9532-209">Licensing resources</span></span>](support-resources-licensing.md)