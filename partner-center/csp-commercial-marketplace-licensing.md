---
title: Marketplace 제품의 라이선스 관리
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV 상업적 marketplace 제품에 대 한 라이선스를 설정 하 고 관리 하는 방법을 알아봅니다.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328018"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="437bf-103">Marketplace 제품의 라이선스 관리</span><span class="sxs-lookup"><span data-stu-id="437bf-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="437bf-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="437bf-104">**Appropriate roles**</span></span>

- <span data-ttu-id="437bf-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="437bf-105">Global admin</span></span>
- <span data-ttu-id="437bf-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="437bf-106">Account admin</span></span>

<span data-ttu-id="437bf-107">이 문서에서는 파트너 센터에서 제품을 설정 하 고 Microsoft AppSource에서 사용할 수 있도록 한 다음 해당 제품에 대 한 라이선스를 관리 하는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="437bf-108">이 문서의 기능은 현재 공개 미리 보기로 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="437bf-109">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="437bf-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="437bf-110">상업적 marketplace 기본 사항</span><span class="sxs-lookup"><span data-stu-id="437bf-110">Commercial marketplace basics</span></span>

<span data-ttu-id="437bf-111">이 프로세스를 시작 하기 전에 먼저 상용 marketplace의 기본 사항을 숙지 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="437bf-112">아래 표의 문서는 시작 하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="437bf-113">항목</span><span class="sxs-lookup"><span data-stu-id="437bf-113">Topic</span></span>  | <span data-ttu-id="437bf-114">아티클</span><span class="sxs-lookup"><span data-stu-id="437bf-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="437bf-115">상업적 마켓플레이스 요금제</span><span class="sxs-lookup"><span data-stu-id="437bf-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="437bf-116">상업적 marketplace 제품에 대 한 계획 및 가격 책정</span><span class="sxs-lookup"><span data-stu-id="437bf-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="437bf-117">상업적 marketplace 제안</span><span class="sxs-lookup"><span data-stu-id="437bf-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="437bf-118">유형 목록</span><span class="sxs-lookup"><span data-stu-id="437bf-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="437bf-119">상업적 마켓플레이스 계정</span><span class="sxs-lookup"><span data-stu-id="437bf-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="437bf-120">파트너 센터에서 상용 마켓플레이스 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="437bf-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="437bf-121">제안 ID 확인</span><span class="sxs-lookup"><span data-stu-id="437bf-121">Determine your Offer ID</span></span>

<span data-ttu-id="437bf-122">아래 절차에는 제품 ID를 입력 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="437bf-123">이제 다음 사항을 염두에 둔 적절 한 제안 ID를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="437bf-124">이 ID는 마켓플레이스 제품 및 Azure Resource Manager 템플릿의 웹 주소에서 고객에게 표시됩니다(해당하는 경우).</span><span class="sxs-lookup"><span data-stu-id="437bf-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="437bf-125">게시자 ID와 결합 된 제품 ID의 길이는 40 자 미만 이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="437bf-126">소문자와 숫자만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="437bf-127">제안 ID는 하이픈 및 밑줄을 포함할 수 있지만 공백은 포함할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="437bf-128">예를 들어 게시자 ID가이 고을 입력 하는 경우 `testpublisherid` `test-offer-1` 제품 웹 주소는 `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` 입니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="437bf-129">**만들기** 를 선택한 후에는이 ID를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="437bf-130">제품 별칭 결정</span><span class="sxs-lookup"><span data-stu-id="437bf-130">Determine your Offer alias</span></span>

<span data-ttu-id="437bf-131">제품 별칭은 파트너 센터의 제품에 사용 되는 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="437bf-132">또한 아래 지침을 따르는 적절 한 제안 별칭이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="437bf-133">이 이름은 Marketplace에서 사용되지 않으며 고객에게 표시되는 제품 이름 및 기타 값과 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="437bf-134">만들기를 선택한 후에는이 이름을 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="437bf-135">제품 만들기</span><span class="sxs-lookup"><span data-stu-id="437bf-135">Create your offer</span></span>

<span data-ttu-id="437bf-136">라이선스 프로세스의 첫 번째 단계는 상업적 마켓플레이스 제품을 만드는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="437bf-137">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="437bf-138">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="437bf-139">개요 페이지의 맨 위에서 **새 제품** 을 선택 하 고 **고객 Engagement & PowerApps에 대해 Dynamics 365을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="437bf-140">이전에 만든 **제품 ID** 및 제품 **별칭** 을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="437bf-141">**만들기** 를 선택하여 제품을 생성하고 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="437bf-142">라이선스 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="437bf-143">제품에 대 한 라이선스 관리를 사용 하도록 설정 하려면 **Microsoft에서 앱 라이선스 관리 사용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="437bf-144">이는 일회성 설정 이며 제품이 게시 된 후에는 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="437bf-145">고객이 라이선스 없이 앱의 기본 기능을 실행 하도록 설정 하 고, 라이선스를 구매한 후에 프리미엄 기능을 실행할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="437bf-146">이렇게 하려면 **라이선스가 할당 되지 않은 경우에도 고객이 앱을 설치할 수 있도록 허용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="437bf-147">제품에서 라이선스 관리를 사용 하도록 설정 하지 않으려는 경우 **지금 받기 (무료)**, **무료 평가판** 또는 **문의처** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="437bf-148">계획 만들기</span><span class="sxs-lookup"><span data-stu-id="437bf-148">Create your plan</span></span>

<span data-ttu-id="437bf-149">이러한 단계에서는 제품에 대해 사용 하도록 설정 하려는 계획을 정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="437bf-150">왼쪽 탐색 메뉴에서 **계획 개요** 를 선택한 다음 **새 계획 만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="437bf-151">**계획 ID** 및 **계획 이름을** 입력 하 고 **만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="437bf-152">**계획 목록** 페이지에서 **계획 설명을** 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="437bf-153">설명을 저장 하 고 나중에 완료 하려면 **초안 저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="437bf-154">완료 되 면 **검토 및 게시** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="437bf-155">이제 계획 정보가 제품 목록 (계획 섹션) 아래 appsource.microsoft.com에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="437bf-156">이 제품에 대 한 모든 계획을 만든 후에는 각 계획의 서비스 ID를 복사 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="437bf-157">계획 목록 페이지의 맨 위에서 **계획 개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="437bf-158">각 계획에 대 한 서비스 ID를 안전한 위치에 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="437bf-159">솔루션에 서비스 Id 추가</span><span class="sxs-lookup"><span data-stu-id="437bf-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="437bf-160">다음 단계는 방금 복사한 각 계획에 대 한 서비스 Id를 추가 하 여 솔루션을 업데이트 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="437bf-161">이에 대 한 지침은 [솔루션에 대 한 AppSource 패키지 만들기](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="437bf-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="437bf-162">패키지 업로드 및 제품 게시</span><span class="sxs-lookup"><span data-stu-id="437bf-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="437bf-163">왼쪽 탐색 창에서 **상업용 마켓플레이스** 를 선택 하 고 **기술 구성** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="437bf-164">**기본 라이선스 모델** 아래에서 **사용자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="437bf-165">**CRM 패키지** 에서 패키지 위치의 URL을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="437bf-166">왼쪽 탐색 창의 다른 탭을 사용 하 여 기타 필요한 정보를 입력할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="437bf-167">완료 되 면 **검토 및 게시** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="437bf-168">제품을 게시 한 후에는 정보를 검토 하 고 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="437bf-169">이 프로세스에 문제가 있는 경우 사용자에 게 알려 드리겠습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="437bf-170">모든 문제가 해결 되 면 제품이 AppSource에서 사용 가능 하다는 알림을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="437bf-171">이 시점에서 라이브로 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="437bf-172">파트너 센터에서 제품을 라이브 상태로 만들기</span><span class="sxs-lookup"><span data-stu-id="437bf-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="437bf-173">아래 절차는 AppSource에서 제품을 라이브 상태로 만드는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="437bf-174">이 프로세스에 대해 자세히 알아보려면 [목록 옵션 소개](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="437bf-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="437bf-175">제품을 게시 한 후에는 사용 시간이 4-6 시간이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="437bf-176">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="437bf-177">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="437bf-178">**개요** 페이지에서 원하는 제품을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="437bf-179">게시할 준비가 된 제품은 **미리 보기** 상태를 갖습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="437bf-180">제품을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-180">Select the offer.</span></span>
4. <span data-ttu-id="437bf-181">**제품 개요** 페이지에서 **라이브 이동** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="437bf-182">제품은 4-6 시간 이내에 라이브 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="437bf-183">AppSource에 대 한 제품 목록을 보려면 **제품 개요** 페이지의 맨 아래에 있는 **appsource** 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="437bf-184">**라이선스가 지원 되는 제품의** 경우: 제품에 라이선스 확인이 필요한 경우 사용자는 연락처를 클릭 하 여 잠재 고객에 **게 연락** 하 여 통신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="437bf-185">**무료 설치 옵션을 사용 하는 라이선스 사용 제품의** 경우: 제품에 라이선스 확인이 필요 하지 않은 경우 관리자에 **게 연락** 뿐만 아니라 **지금 가져오기** 단추가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="437bf-186">무료 설치 옵션을 시도 하려는 사용자는 **지금 가져오기** 를 클릭 해야 합니다. 그러면 Power Platform 관리 센터에 제품을 설치 하 게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="437bf-187">사용자는 궁금한 점이 있거나 유료 요금제로 업그레이드 하려는 경우에도 사용자 **에 게 연락** 하는 것을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="437bf-188">ISV 연결을 위한 등록 처리 등록</span><span class="sxs-lookup"><span data-stu-id="437bf-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="437bf-189">고객에 게 라이선스를 할당 하려면 먼저 각 판매를 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="437bf-190">이렇게 하려면 [거래 등록](register-deals.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="437bf-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="437bf-191">고객 초대</span><span class="sxs-lookup"><span data-stu-id="437bf-191">Invite the customer</span></span>

<span data-ttu-id="437bf-192">다음 절차를 사용 하 여 고객에 게이 거래에 참여할 수 있도록 초대 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="437bf-193">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="437bf-194">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="437bf-195">왼쪽 탐색 메뉴에서 **조회** 를 선택 하 고 **거래 등록** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="437bf-196">**제출** 된 거래에 대해 필터링 하 고 **진행** 중인 탭을 선택한 후 원하는 거래를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="437bf-197">이 거래의 개요 페이지에서 **라이선스 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="437bf-198">**라이선스 관리** 창의 **고객 세부 정보** 드롭다운 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="437bf-199">고객 관계가 아직 없는 경우 **+ 새 고객 초대를 선택 하 여 동의** 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="437bf-200">표시 되는 링크를 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="437bf-201">이 링크를 고객의 청구 관리자 또는 전역 관리자에 게 전자 메일로 보내고,이 링크를 사용 하 여 admin.microsoft.com에 액세스 하 고, 사용자가 설정 하는 관계를 승인 하 고 권한을 부여 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="437bf-202">관계는 고객이이 단계를 수행할 때까지 설정 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="437bf-203">라이선스 활성화, 관리 및 제거</span><span class="sxs-lookup"><span data-stu-id="437bf-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="437bf-204">고객의 관계에 대 한 권한이 부여 되 면 제품에서 요금제를 추가 하 고 각 계획에 라이선스를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="437bf-205">이 거래에 대 한 라이선스 관리 창에서 **+ 계획 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="437bf-206">**이 솔루션에 대 한 계획** 및 **라이선스 수** 필드를 완료 한 후 **라이선스 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="437bf-207">라이선스는 고객이 관리 하 고 직원에 게 할당할 수 있는 admin.microsoft.com에서 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="437bf-208">기존 계획의 라이선스 수를 변경 하려면 **라이선스 수** 필드에 새 숫자를 입력 한 다음 **라이선스 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="437bf-209">거래의 라이선스를 비활성화 하거나 제거 하려면 **작업** 필드에서 휴지통 아이콘을 선택 하 고 **라이선스 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="437bf-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="437bf-210">다음 단계</span><span class="sxs-lookup"><span data-stu-id="437bf-210">Next steps</span></span>

[<span data-ttu-id="437bf-211">라이선스 리소스</span><span class="sxs-lookup"><span data-stu-id="437bf-211">Licensing resources</span></span>](support-resources-licensing.md)
