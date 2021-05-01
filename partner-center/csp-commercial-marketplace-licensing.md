---
title: Marketplace 제품의 라이선스 관리
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV 상업적 marketplace 제품에 대 한 라이선스를 설정 하 고 관리 하는 방법을 알아봅니다.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284879"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="de623-103">Marketplace 제품의 라이선스 관리</span><span class="sxs-lookup"><span data-stu-id="de623-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="de623-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="de623-104">**Appropriate roles**</span></span>

- <span data-ttu-id="de623-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="de623-105">Global admin</span></span>
- <span data-ttu-id="de623-106">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="de623-106">Account admin</span></span>

<span data-ttu-id="de623-107">이 문서에서는 파트너 센터에서 제품을 설정 하 고 Microsoft AppSource에서 사용할 수 있도록 한 다음 해당 제품에 대 한 라이선스를 관리 하는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="de623-108">이 문서의 기능은 현재 공개 미리 보기로 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="de623-109">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="de623-109">Before you begin</span></span>

<span data-ttu-id="de623-110">이 프로세스를 시작 하기 전에 아래 정보를 숙지 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="de623-111">Azure Marketplace 설명서 검토</span><span class="sxs-lookup"><span data-stu-id="de623-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="de623-112">다음 문서에는 계속 하기 전에 알아두어야 할 정보가 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="de623-113">Dynamics 365 for Customer Engagement 및 PowerApps 제품 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="de623-114">파트너 센터에서 상용 마켓플레이스 계정 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="de623-115">제안 ID 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-115">Create your Offer ID</span></span>

<span data-ttu-id="de623-116">아래 절차에는 제품 ID를 입력 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="de623-117">이제 다음 사항을 염두에 둔 적절 한 제안 ID를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="de623-118">이 ID는 마켓플레이스 제품 및 Azure Resource Manager 템플릿의 웹 주소에서 고객에게 표시됩니다(해당하는 경우).</span><span class="sxs-lookup"><span data-stu-id="de623-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="de623-119">게시자 ID와 결합 된 제품 ID의 길이는 40 자 미만 이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="de623-120">소문자와 숫자만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="de623-121">제안 ID는 하이픈 및 밑줄을 포함할 수 있지만 공백은 포함할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="de623-122">예를 들어 게시자 ID가 testpublisherid이 고 테스트-1을 입력 하는 경우 제품 웹 주소는가 됩니다 https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="de623-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="de623-123">**만들기** 를 선택한 후에는이 ID를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="de623-124">제품 별칭 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-124">Create your Offer alias</span></span>

<span data-ttu-id="de623-125">제품 별칭은 파트너 센터의 제품에 사용 되는 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="de623-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="de623-126">또한 아래 지침을 따르는 적절 한 제안 별칭이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="de623-127">이 이름은 마켓플레이스에서 사용되지 않으며 고객에게 표시되는 제품 이름 및 기타 값과 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="de623-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="de623-128">만들기를 선택한 후에는이 이름을 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="de623-129">제품 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-129">Create your offer</span></span>

<span data-ttu-id="de623-130">라이선스 프로세스의 첫 번째 단계는 상업적 마켓플레이스 제품을 만드는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="de623-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="de623-131">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="de623-132">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="de623-133">개요 페이지의 맨 위에서 **새 제품** 을 선택 하 고 **고객 Engagement & PowerApps에 대해 Dynamics 365을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="de623-134">이전에 만든 **제품 ID** 및 제품 **별칭** 을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="de623-135">**만들기** 를 선택하여 제품을 생성하고 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="de623-136">라이선스 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="de623-137">제품에 대 한 라이선스 관리를 사용 하도록 설정 하려면 **Microsoft에서 앱 라이선스 관리 사용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="de623-138">이는 일회성 설정 이며 제품이 게시 된 후에는 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="de623-139">고객이 라이선스 없이 앱의 기본 기능을 실행 하도록 설정 하 고, 라이선스를 구매한 후에 프리미엄 기능을 실행할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="de623-140">이렇게 하려면 **라이선스가 할당 되지 않은 경우에도 고객이 앱을 설치할 수 있도록 허용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="de623-141">제품에서 라이선스 관리를 사용 하도록 설정 하지 않으려는 경우 **지금 받기 (무료)**, **무료 평가판** 또는 **문의처** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="de623-142">계획 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-142">Create your plan</span></span>

<span data-ttu-id="de623-143">이러한 단계에서는 제품에 대해 사용 하도록 설정 하려는 계획을 정의 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="de623-144">왼쪽 탐색 메뉴에서 **계획 개요** 를 선택한 다음 **새 계획 만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="de623-145">**계획 ID** 및 **계획 이름을** 입력 하 고 **만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="de623-146">**계획 목록** 페이지에서 **계획 설명을** 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="de623-147">설명을 저장 하 고 나중에 완료 하려면 **초안 저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="de623-148">완료 되 면 **검토 및 게시** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="de623-149">이제 계획 정보가 제품 목록 (계획 섹션) 아래 appsource.microsoft.com에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="de623-150">이 제품에 대 한 모든 계획을 만든 후에는 각 계획의 서비스 ID를 복사 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="de623-151">계획 목록 페이지의 맨 위에서 **계획 개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="de623-152">각 계획에 대 한 서비스 ID를 안전한 위치에 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="de623-153">솔루션에 서비스 Id 추가</span><span class="sxs-lookup"><span data-stu-id="de623-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="de623-154">다음 단계는 방금 복사한 각 계획에 대 한 서비스 Id를 추가 하 여 솔루션을 업데이트 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="de623-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="de623-155">이에 대 한 지침은 [솔루션에 대 한 AppSource 패키지 만들기](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="de623-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="de623-156">패키지 업로드 및 제품 게시</span><span class="sxs-lookup"><span data-stu-id="de623-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="de623-157">왼쪽 탐색 창에서 **상업용 마켓플레이스** 를 선택 하 고 **기술 구성** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="de623-158">**기본 라이선스 모델** 아래에서 **사용자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="de623-159">**CRM 패키지** 에서 패키지 위치의 URL을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="de623-160">왼쪽 탐색 창의 다른 탭을 사용 하 여 기타 필요한 정보를 입력할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="de623-161">완료 되 면 **검토 및 게시** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="de623-162">제품을 게시 한 후에는 정보를 검토 하 고 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="de623-163">이 프로세스에 문제가 있는 경우 사용자에 게 알려 드리겠습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="de623-164">모든 문제가 해결 되 면 제품이 AppSource에서 사용 가능 하다는 알림을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="de623-165">이 시점에서 라이브로 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="de623-166">파트너 센터에서 제품을 라이브 상태로 만들기</span><span class="sxs-lookup"><span data-stu-id="de623-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="de623-167">아래 절차는 AppSource에서 제품을 라이브 상태로 만드는 과정을 안내 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="de623-168">이 프로세스에 대해 자세히 알아보려면 [목록 옵션 소개](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="de623-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="de623-169">제품을 게시 한 후에는 사용 시간이 4-6 시간이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="de623-170">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="de623-171">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="de623-172">**개요** 페이지에서 원하는 제품을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="de623-173">게시할 준비가 된 제품은 **미리 보기** 상태를 갖습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="de623-174">제품을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-174">Select the offer.</span></span>
4. <span data-ttu-id="de623-175">**제품 개요** 페이지에서 **라이브 이동** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="de623-176">제품은 4-6 시간 이내에 라이브 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="de623-177">AppSource에 대 한 제품 목록을 보려면 **제품 개요** 페이지의 맨 아래에 있는 **appsource** 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="de623-178">**라이선스가 지원 되는 제품의** 경우: 제품에 라이선스 확인이 필요한 경우 사용자는 연락처를 클릭 하 여 잠재 고객에 **게 연락** 하 여 통신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="de623-179">**무료 설치 옵션을 사용 하는 라이선스 사용 제품의** 경우: 제품에 라이선스 확인이 필요 하지 않은 경우 관리자에 **게 연락** 뿐만 아니라 **지금 가져오기** 단추가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="de623-180">무료 설치 옵션을 시도 하려는 사용자는 **지금 가져오기** 를 클릭 해야 합니다. 그러면 Power Platform 관리 센터에 제품을 설치 하 게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="de623-181">사용자는 궁금한 점이 있거나 유료 요금제로 업그레이드 하려는 경우에도 사용자 **에 게 연락** 하는 것을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="de623-182">DealReg의 ISV Connect 거래 등록</span><span class="sxs-lookup"><span data-stu-id="de623-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="de623-183">다음 단계는 거래를 등록 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="de623-183">The next step is to register your deal.</span></span> <span data-ttu-id="de623-184">이렇게 하려면 [거래 등록](https://docs.microsoft.com/partner-center/register-deals)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="de623-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="de623-185">고객 초대</span><span class="sxs-lookup"><span data-stu-id="de623-185">Invite the customer</span></span>

<span data-ttu-id="de623-186">다음 절차를 사용 하 여 고객에 게이 거래에 참여할 수 있도록 초대 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="de623-187">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="de623-188">왼쪽 탐색 메뉴에서 **상업용 마켓플레이스/개요** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="de623-189">**제출** 된 거래에 대해 필터링 하 고 **진행** 중인 탭을 선택한 후 원하는 거래를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="de623-190">이 거래의 개요 페이지에서 **라이선스 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="de623-191">**라이선스 관리** 창의 **고객 세부 정보** 드롭다운 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="de623-192">고객 관계가 아직 없는 경우 **+ 새 고객 초대를 선택 하 여 동의** 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="de623-193">표시 되는 링크를 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="de623-194">이 링크를 고객의 청구 관리자 또는 전역 관리자에 게 전자 메일로 보내고,이 링크를 사용 하 여 admin.microsoft.com에 액세스 하 고, 사용자가 설정 하는 관계를 승인 하 고 권한을 부여 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="de623-195">관계는 고객이이 단계를 수행할 때까지 설정 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="de623-196">라이선스 활성화, 관리 및 제거</span><span class="sxs-lookup"><span data-stu-id="de623-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="de623-197">고객이 설정 되 면 제품에서 요금제를 추가 하 고 각 계획에 라이선스를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="de623-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="de623-198">이 거래에 대 한 라이선스 관리 창에서 **+ 계획 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="de623-199">**이 솔루션에 대 한 계획** 및 **라이선스 수** 필드를 완료 한 후 **라이선스 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="de623-200">라이선스는 고객이 관리 하 고 직원에 게 할당할 수 있는 admin.microsoft.com에서 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="de623-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="de623-201">기존 계획의 라이선스 수를 변경 하려면 **라이선스 수** 필드에 새 숫자를 입력 한 다음 **라이선스 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="de623-202">거래의 라이선스를 비활성화 하거나 제거 하려면 **작업** 필드에서 휴지통 아이콘을 선택 하 고 **라이선스 업데이트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="de623-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>