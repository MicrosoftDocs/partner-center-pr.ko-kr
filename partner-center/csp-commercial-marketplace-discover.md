---
title: 제품 검색-상업적 marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 파트너가 파트너 센터를 사용 하 여 Isv (독립 소프트웨어 공급 업체)의 SaaS 제품 또는 가격 책정을 보거나 검색 하는 방법에 대해 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f741ef4e44632e1d239285b58e99fbb38a8f37e7
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979603"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="121ea-103">파트너 센터 상업적 marketplace에서 제품 및 가격 책정 검색</span><span class="sxs-lookup"><span data-stu-id="121ea-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="121ea-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="121ea-104">**Appropriate roles**</span></span>

- <span data-ttu-id="121ea-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="121ea-105">Global admin</span></span>
- <span data-ttu-id="121ea-106">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="121ea-106">Admin agent</span></span>

<span data-ttu-id="121ea-107">Isv (독립 소프트웨어 공급 업체)가 상업적 marketplace에서 제품을 게시 하도록 선택할 때 CSP 프로그램에서 제품을 사용할 수 있도록 할지 여부를 결정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-107">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="121ea-108">CSP 프로그램을 통해 제품을 판매 하도록 선택 하는 경우 CSP 파트너는 파트너 센터 마켓플레이스 영역에 제품을 표시 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-108">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="121ea-109">ISV 제품이 파트너 센터에서 기대한 대로 표시 되지 않는 경우 다음 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-109">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="121ea-110">ISV는 CSP 프로그램을 통해 제품을 판매 하지 않기로 결정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-110">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="121ea-111">예를 들어 일부 ISV 제품은 상용 marketplace의 다른 영역 (예: [Microsoft AppSource](https://appsource.microsoft.com/) 및 [Azure Marketplace](https://azuremarketplace.microsoft.com/))에서 사용할 수 있었지만 파트너 센터 marketplace의 CSP 프로그램에서 파트너에 게 표시 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-111">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="121ea-112">ISV는 선택 된 수의 CSP 파트너만이 제품을 독점적으로 만들도록 결정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-112">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="121ea-113">독점적 제공에 대 한 자세한 내용은이 도움말 항목의 뒷부분에 나오는을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="121ea-113">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="121ea-114">제품 유형이 파트너 센터 또는 Azure Portal (예: 컨테이너 또는 일부 사용량 기반 제품)를 통해 불가능 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-114">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="121ea-115">연결 된 고객의 청구 국가는이 ISV 제품에 대해 지원 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-115">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="121ea-116">파트너 센터에서 Marketplace 제품 보기</span><span class="sxs-lookup"><span data-stu-id="121ea-116">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="121ea-117">CSP 프로그램에서 사용 가능한 상용 marketplace 제품을 보려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-117">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="121ea-118">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 한 다음, 왼쪽 탐색 메뉴에서 **CSP** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-118">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="121ea-119">**판매** 를 선택 하 고 **Marketplace** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-119">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="121ea-120">기본적으로 모든 형식 및 범주의 제품이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-120">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="121ea-121">유형 또는 범주별로 필터를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-121">Select a filter by type or category.</span></span> <span data-ttu-id="121ea-122">또한 **검색** 을 사용 하 여 특정 키워드, 제품 이름 또는 ISV 게시자의 이름을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-122">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="121ea-123">목록에서 특정 제품 제품을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-123">Select a specific product offer from the list.</span></span> <span data-ttu-id="121ea-124">제품 개요 탭으로 이동 하 여 제품에 대해 자세히 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-124">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="121ea-125">이 탭에는 다음과 같은 정보가 포함 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-125">Information on this tab might include:</span></span> 

    - <span data-ttu-id="121ea-126">제품 또는 제안에 대 한 설명</span><span class="sxs-lookup"><span data-stu-id="121ea-126">A description of the product or offer</span></span>

    - <span data-ttu-id="121ea-127">ISV 게시자에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="121ea-127">More information about the ISV publisher</span></span>

    - <span data-ttu-id="121ea-128">ISV 게시자가 업로드 한 설명서 또는 마케팅 자료에 대 한 링크</span><span class="sxs-lookup"><span data-stu-id="121ea-128">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="121ea-129">고객 지원, 엔지니어링 또는 CSP 프로그램의 연락처에 대 한 기타 가능한 ISV 연락처</span><span class="sxs-lookup"><span data-stu-id="121ea-129">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="121ea-130">제품의 사용 가능한 요금제, Sku 또는 가격에 대 한 자세한 내용을 보려면 **요금제 + 가격 책정** 탭을 선택 합니다. 이 탭에는 다음이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-130">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="121ea-131">이 제품을 사용할 수 있는 시장</span><span class="sxs-lookup"><span data-stu-id="121ea-131">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="121ea-132">제품에 사용할 수 있는 Sku 또는 요금제 목록</span><span class="sxs-lookup"><span data-stu-id="121ea-132">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="121ea-133">사용 가능한 각 SKU 또는 요금제에 대 한 가격 책정</span><span class="sxs-lookup"><span data-stu-id="121ea-133">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="121ea-134">파트너 센터 Api를 통해 Marketplace 제품 보기</span><span class="sxs-lookup"><span data-stu-id="121ea-134">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="121ea-135">CSP 프로그램 파트너는 Api를 사용 하 여 적격 제안 목록을 반환할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-135">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="121ea-136">적격 제품은 파트너가 파트너 센터 marketplace를 통해 판매할 수 있는 SaaS ISV 제품에만 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-136">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="121ea-137">Api를 사용 하 여 카탈로그에서 제품을 식별 하는 파트너에 대 한 지침을 참조 하 여 [시장에 대 한 제안 목록을 가져옵니다](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span><span class="sxs-lookup"><span data-stu-id="121ea-137">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="121ea-138">파트너 센터에서 최신 마켓플레이스 제공 가격 책정 보기</span><span class="sxs-lookup"><span data-stu-id="121ea-138">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="121ea-139">제품에 연결 된 최신 가격 정보를 보려면 다음 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="121ea-139">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="121ea-140">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 한 다음, 왼쪽 탐색 메뉴에서 **CSP** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-140">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="121ea-141">**판매**, **가격 책정 및 제품** 을 차례로 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-141">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="121ea-142">**Marketplace** 섹션으로 스크롤하고, 위치를 선택 하 고, **marketplace 가격** 을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-142">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="121ea-143">그러면 SaaS, 라이선스 기반 제품 및 ISV 게시자 로부터 제공 되는 요금제에 대 한 최신 가격 책정 데이터가 포함 된 스프레드시트가 생성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-143">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="121ea-144">일부 Azure 응용 프로그램 가격은 여기에 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-144">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="121ea-145">이 정보는 매일 업데이트 되므로 선택 하는 빈도에 따라 현재 가격을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-145">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="121ea-146">ISV 제품에 무료 평가 기간이 포함 되어 있으면 스프레드시트에 해당 제품에 대 한 두 개의 행이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-146">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="121ea-147">한 행은 무료 평가판 가격 (0)을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-147">One row shows the free trial price of zero.</span></span> <span data-ttu-id="121ea-148">즉, 무료 평가판 기간이 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-148">This means a free trial period is available.</span></span>

    - <span data-ttu-id="121ea-149">다른 행에는 무료 평가 기간이 끝난 후에 적용 되는 가격 및 약관이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-149">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="121ea-150">CSP 프로그램 파트너는 특정 상업적 marketplace 제품에 연결 된 다른 성과급을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-150">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="121ea-151">다른 성과급에 대 한 자세한 내용은 [csp 동기 가이드](https://aka.ms/partnerincentives) (csp 로그인 필요)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="121ea-151">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="121ea-152">Marketplace 독점 제품에 대해 알아보기</span><span class="sxs-lookup"><span data-stu-id="121ea-152">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="121ea-153">Isv는 CSP 프로그램의 특정 파트너만 해당 제품을 사용할 수 있도록 하는 옵션을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-153">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="121ea-154">이를 독점적인 제안 이라고 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-154">This is known as an Exclusive offer.</span></span> <span data-ttu-id="121ea-155">CSP 프로그램의 모든 파트너는 독점적으로 표시 된 제품을 비롯 하 여 파트너 센터 상업적 marketplace의 모든 ISV 제품을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-155">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="121ea-156">제품이 단독으로 표시 **되지 않은** 경우 모든 파트너는 해당 제품을 구매할 수 있습니다 (선택한 고객의 청구 국가가 ISV 제품의 국가 가용성과 일치 하는 것으로 가정).</span><span class="sxs-lookup"><span data-stu-id="121ea-156">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="121ea-157">그러나 단독으로 표시 된 모든 제품의 경우 ISV에서 선택한 파트너만 해당 제품을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-157">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="121ea-158">고객에 게 판매할 것으로 표시 된 제품이 독점적으로 표시 되는 경우 ISV에 게 직접 연락 하 여 독점적인 제품을 판매할 수 있는 권한을 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-158">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="121ea-159">독점 제품의 세부 정보를 볼 때 사용자가 선택할 수 있는 **ISV** 링크를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="121ea-159">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="121ea-160">상업적 marketplace의 ISV 환경에 대해 자세히 알아보려면 [클라우드 솔루션 공급자](/azure/marketplace/cloud-solution-providers)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="121ea-160">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="121ea-161">Marketplace의 CSP 환경에 대 한 자세한 내용은 [상용 마켓플레이스 개요](csp-commercial-marketplace-overview.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="121ea-161">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="121ea-162">다음 단계</span><span class="sxs-lookup"><span data-stu-id="121ea-162">Next steps</span></span>

- [<span data-ttu-id="121ea-163">상업적 marketplace 제품 구매</span><span class="sxs-lookup"><span data-stu-id="121ea-163">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)