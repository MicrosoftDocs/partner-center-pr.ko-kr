---
title: 파트너 센터에서 고객 구독 만들기
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft에서 게시 한 제품 및 타사 Isv가 게시 한 SaaS 제품에 고객 구독을 판매 하는 방법에 대해 알아봅니다.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: 구독, 새로 만들기, 구독 추가, 일시 중단, 취소, 일시 중단, 일시 중단, SaaS, 라이선스, ISV, 타사
ms.localizationpriority: medium
ms.openlocfilehash: 7f8b3e6c444f8aeb59a55d6e7feb881eb6f99a5e
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679060"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="67a7e-104">고객 구독 만들기, 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="67a7e-104">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="67a7e-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="67a7e-105">**Applies to**</span></span>

- <span data-ttu-id="67a7e-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="67a7e-106">Partner Center</span></span>
- <span data-ttu-id="67a7e-107">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="67a7e-107">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="67a7e-108">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="67a7e-108">CSP partners</span></span>

<span data-ttu-id="67a7e-109">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="67a7e-109">**Appropriate roles**</span></span>

- <span data-ttu-id="67a7e-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="67a7e-110">Admin agent</span></span>
- <span data-ttu-id="67a7e-111">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="67a7e-111">Billing admin</span></span>
- <span data-ttu-id="67a7e-112">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="67a7e-112">Global admin</span></span>
- <span data-ttu-id="67a7e-113">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="67a7e-113">Helpdesk agent</span></span>
- <span data-ttu-id="67a7e-114">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="67a7e-114">Sales agent</span></span>

<span data-ttu-id="67a7e-115">파트너 센터에서 고객 기록을 만들면 카탈로그에서 제품의 구독을 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-115">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="67a7e-116">여기에는 타사 Isv (독립 소프트웨어 공급 업체)가 [상업적 marketplace](https://azuremarketplace.microsoft.com/marketplace)에 게시 한 SaaS (Software As a Service) 제품 뿐만 아니라 Microsoft에서 게시 한 제품이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-116">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="67a7e-117">일부 제안은 고객 당 하나의 구독으로 제한 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-117">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="67a7e-118">제한되는 제품 목록을 보려면 파트너 센터 가격 책정 및 제품 페이지를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="67a7e-118">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="67a7e-119">CSP 프로그램의 파트너는 파트너 센터 내에서 ISV 게시자의 **라이선스 기반** SaaS 구독만 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-119">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="67a7e-120">즉, 사용자가 액세스할 수 있는 [전용 제품](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 을 비롯 하 여 ISV 게시자가 사용할 수 있도록 설정한 모든 **라이선스 기반** SaaS 제품을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-120">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="67a7e-121">Isv (Azure 응용 프로그램, 컨테이너 또는 Vm과 관련 된 **사용량 기반**, 요금제 또는 소비 기반 제품)에서 기타 상업적 marketplace 제품을 구매 하거나 관리 하려면 [azure 관리 포털](https://portal.azure.com/)로 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-121">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="67a7e-122">자세한 내용은 [상용 마켓플레이스 제품 구매](csp-commercial-marketplace-purchase.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="67a7e-122">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="67a7e-123">새 구독 만들기</span><span class="sxs-lookup"><span data-stu-id="67a7e-123">Create a new subscription</span></span>

1. <span data-ttu-id="67a7e-124">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-124">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="67a7e-125">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="67a7e-126">**구독 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-126">Select **Add subscription**.</span></span> <span data-ttu-id="67a7e-127">**온라인 서비스** 탭에는 사용 가능한 Marketplace SaaS 제품이 모두 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-127">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="67a7e-128">특정 유형의 구독만 표시하려면 사용 가능한 필터 중에서 원하는 필터를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-128">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="67a7e-129">**게시자** **: microsoft를 선택 하** 여 isv가 게시 한 상용 마켓플레이스 **제품을 볼 수 있습니다** .</span><span class="sxs-lookup"><span data-stu-id="67a7e-129">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="67a7e-130">**청구 유형**: 사용 하려는 구독 청구 유형 ( **라이선스** 또는 **사용**)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-130">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="67a7e-131">월간 청구 주기와 연간 청구 주기 중 어떤 것을 선택할지 결정할 때 도움이 되는 정보는 [새 청구 기능에 대한 FAQ](faq-about-new-billing-features.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="67a7e-131">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="67a7e-132">**범주**: **Enterprise**, **Small business**또는 **평가판**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-132">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="67a7e-133">평가판 구독에 대한 자세한 내용은 [고객에게 Microsoft 제품의 평가판 제공](offer-your-customers-trials-of-microsoft-products.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="67a7e-133">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="67a7e-134">고객을 위해 구매할 제품 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-134">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="67a7e-135">표시 되는 제품은 고객 부문 유형 (교육, 정부 등) 및 적용 한 필터에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-135">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="67a7e-136">Marketplace에 표시 된 일부 제안은 특정 고객 또는 특정 CSP 파트너에 게 제공 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-136">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="67a7e-137">이는 다음과 같은 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-137">This can be because:</span></span>

   - <span data-ttu-id="67a7e-138">고객은 이미 해당 제품에 대 한 구독을 보유 하 고 있으며 하나만 허용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-138">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="67a7e-139">고객의 구독이 일시 중단 되었을 수 있습니다 .이 경우에는 새 구독을 구입 하는 대신 구독을 다시 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-139">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="67a7e-140">ISV SaaS 제품의 경우 제품을 구매할 수 없는 몇 가지 이유가 있을 수 있습니다. ISV는 고객의 청구 국가 또는 지역을 지원 하지 않을 수 있습니다. ISV는 CSP 프로그램을 통해 제공 서비스를 제공 하지 않도록 선택할 수 있습니다. 또는 ISV는 특정 CSP 파트너 [에게만 제공 되는 제품을 만들](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-140">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="67a7e-141">ISV 제품은 파트너 센터를 통해 불가능 되지 않을 수도 있습니다 (예: 컨테이너 또는 몇 가지 사용 빈도 기반 제안).</span><span class="sxs-lookup"><span data-stu-id="67a7e-141">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="67a7e-142">추가 하려는 각 구독에 대해 라이선스 수 (필요한 경우)를 입력 하 고 **카트에 추가를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-142">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="67a7e-143">구독 추가가 완료 되 면 **검토** 를 선택 하 고 주문을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-143">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="67a7e-144">주문을 검토 하 고 이러한 구독을 구매할 준비가 되 면 **구매**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-144">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="67a7e-145">고객에 대 한 구독을 구매한 후에는 다음이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-145">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="67a7e-146">해당 고객의 **구독** 페이지에서 구독 이름을 선택 하 여 구독을 검토 하거나 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-146">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="67a7e-147">여기에서 사용 가능한 경우 추가 기능 라이선스를 선택하거나, 라이선스 수를 변경하거나, 구독을 일시 중단할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-147">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="67a7e-148">**ISV SaaS (라이선스 기반) 구독의 경우:**</span><span class="sxs-lookup"><span data-stu-id="67a7e-148">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="67a7e-149">ISV 게시자 사이트에 대 한 링크를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-149">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="67a7e-150">이 링크를 통해 고객 구독의 배포 또는 계정 설정을 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-150">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="67a7e-151">이 유형의 ISV 구독에 대 한 계정 설정/프로 비전을 완료 하는 지침이 포함 된 전자 메일은 사용자 또는 고객 모두에 게 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-151">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="67a7e-152">구독에 30 일 무료 평가판이 제공 되는 경우 무료 평가판 기간이 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-152">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="67a7e-153">CSP 프로그램의 파트너는 고객을 위해 구매한 제품에 대 한 무료 평가판 기간을 되지 않으며 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-153">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="67a7e-154">무료 평가판 기간이 종료 되 면 구독 기간이 시작 되 고 구독이 유료 상태로 전환 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-154">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="67a7e-155">그러면 구독은 동일한 일정에 따라 autorenew 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-155">The subscription will then autorenew according to the same schedule.</span></span>

## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="67a7e-156">구독 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="67a7e-156">Suspend or cancel a subscription</span></span>

<span data-ttu-id="67a7e-157">파트너는 고객이 요청한 경우 또는 지불 이나 사기 행위의 경우 구독을 일시 중단 하거나 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-157">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="67a7e-158">구독 일시 중단</span><span class="sxs-lookup"><span data-stu-id="67a7e-158">Suspend a subscription</span></span>

<span data-ttu-id="67a7e-159">구독 상태를 **일시 중지 됨**으로 변경 하면 사용자가 로그인 하거나 서비스에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-159">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="67a7e-160">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-160">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="67a7e-161">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-161">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="67a7e-162">관리 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-162">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="67a7e-163">**상태** 섹션에서 **일시 중단됨**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-163">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="67a7e-164">그런 다음, 변경 내용을 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-164">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="67a7e-165">90일 이내에 또는 90일에 계정이 개설된 시간과 첫 번째 청구 기간 사이의 일 수를 더한 기간(최대 120일) 이내에 구독을 다시 활성화하지 않으면 모든 데이터가 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-165">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="67a7e-166">구독을 일시 중단할 경우, **일시 중단** 버튼 아래에 표시된 날짜는 구독을 다시 활성화하지 않을 경우 자동으로 구독이 만료되는 시점을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-166">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> <span data-ttu-id="67a7e-167">자세한 내용은 [새로운 청구 기능에 대 한 FAQ](faq-about-new-billing-features.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="67a7e-167">For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="67a7e-168">구독 취소</span><span class="sxs-lookup"><span data-stu-id="67a7e-168">Cancel a subscription</span></span>

<span data-ttu-id="67a7e-169">파트너 센터 [상업적 marketplace](csp-commercial-marketplace-overview.md)내에서 타사 ISV 게시자의 라이선스 기반 SaaS 구독을 취소 하는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-169">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="67a7e-170">취소 기간 내에 취소 하는 동안에는 전체 환불을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-170">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="67a7e-171">매월 청구 되는 ISV 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="67a7e-171">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="67a7e-172">주문을 넣은 후 24 시간 이내에 취소 하면 다음 청구서에 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-172">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="67a7e-173">주문을 넣은 후 24 시간 이상 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-173">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="67a7e-174">매년 청구 되는 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="67a7e-174">For offers billed annually:</span></span>

- <span data-ttu-id="67a7e-175">주문을 입력 한 후 14 일 이내에 취소 하면 다음 청구서에서 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-175">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="67a7e-176">주문을 입력 한 후 14 일이 지난 후에 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-176">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="67a7e-177">이러한 기간이 끝난 후에는 구독을 취소 하는 옵션이 더 이상 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-177">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="67a7e-178">사용량 기반 및 요금제로, 가상 컴퓨터 또는 컨테이너를 사용 하는 타사 ISV 서비스는 반환 대상이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-178">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="67a7e-179">사용 빈도 기반 서비스를 취소 메서드로 프로 비전 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-179">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="67a7e-180">요금 청구는 사용 후 청구 되므로 이러한 서비스는 환불을 받을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-180">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="67a7e-181">ISV 게시자에서 라이선스 기반 SaaS 구독을 취소하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-181">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="67a7e-182">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-182">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="67a7e-183">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-183">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="67a7e-184">취소 하려는 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-184">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="67a7e-185">**상태** 열에서 **취소**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-185">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="67a7e-186">그런 다음, 변경 내용을 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-186">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="67a7e-187">대화 상자가 표시 되 면 관련 세부 정보를 입력 한 다음 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-187">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="67a7e-188">취소를 확인 하려면 **예, 취소**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-188">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="67a7e-189">Api를 사용 하 여 Azure Marketplace 구독을 취소 하도록 선택할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-189">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="67a7e-190">이렇게 하려면 [Azure Marketplace 구독 취소](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="67a7e-190">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="67a7e-191">상업용 마켓플레이스 구독을 자동으로 갱신할지 선택</span><span class="sxs-lookup"><span data-stu-id="67a7e-191">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="67a7e-192">기본적으로 활성 구독은 구독 기간이 만료되면 자동으로 갱신되도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-192">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="67a7e-193">[상업용 마켓플레이스 제품 구독](csp-commercial-marketplace-overview.md)의 경우 필요에 따라 구독을 자동으로 갱신하지 않도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-193">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="67a7e-194">활성 상업적 marketplace 구독이 자동으로 갱신 되지 않도록 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-194">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="67a7e-195">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="67a7e-196">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="67a7e-197">**구독**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-197">Select **Subscriptions**.</span></span> <span data-ttu-id="67a7e-198">고객에 대해 구매한 라이선스 기반 구독을 나열 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-198">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="67a7e-199">**구독** 열에서 수정 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-199">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="67a7e-200">구독 정보 페이지에서 **상태** 섹션을 찾고 **자동 갱신** 확인란의 선택을 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-200">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="67a7e-201">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="67a7e-201">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="67a7e-202">다음 단계</span><span class="sxs-lookup"><span data-stu-id="67a7e-202">Next steps</span></span>

- [<span data-ttu-id="67a7e-203">고객을 위한 상업용 마켓플레이스 제품</span><span class="sxs-lookup"><span data-stu-id="67a7e-203">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="67a7e-204">고객을 위한 상업적 마켓플레이스 제품 관리</span><span class="sxs-lookup"><span data-stu-id="67a7e-204">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="67a7e-205">상업용 Marketplace 개요</span><span class="sxs-lookup"><span data-stu-id="67a7e-205">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
