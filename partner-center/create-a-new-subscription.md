---
title: 파트너 센터에서 고객 구독 만들기
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft에서 게시 한 제품 및 타사 Isv가 게시 한 SaaS 제품에 고객 구독을 판매 하는 방법에 대해 알아봅니다.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: e72c499cac9b2408e34a0f6fbf2e442f93faef47
ms.sourcegitcommit: 54f823f0e02e0e7add737d78de74d8eba8d9f381
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/22/2020
ms.locfileid: "86875229"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="83a5c-103">고객 구독 만들기, 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="83a5c-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="83a5c-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="83a5c-104">**Applies to**</span></span>

- <span data-ttu-id="83a5c-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="83a5c-105">Partner Center</span></span>
- <span data-ttu-id="83a5c-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="83a5c-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="83a5c-107">CSP 파트너</span><span class="sxs-lookup"><span data-stu-id="83a5c-107">CSP partners</span></span>

<span data-ttu-id="83a5c-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="83a5c-108">**Appropriate roles**</span></span>

- <span data-ttu-id="83a5c-109">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="83a5c-109">Admin agent</span></span>
- <span data-ttu-id="83a5c-110">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="83a5c-110">Billing admin</span></span>
- <span data-ttu-id="83a5c-111">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="83a5c-111">Global admin</span></span>
- <span data-ttu-id="83a5c-112">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="83a5c-112">Helpdesk agent</span></span>
- <span data-ttu-id="83a5c-113">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="83a5c-113">Sales agent</span></span>

<span data-ttu-id="83a5c-114">파트너 센터에서 고객 기록을 만들면 카탈로그에서 제품의 구독을 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="83a5c-115">여기에는 타사 Isv (독립 소프트웨어 공급 업체)가 [상업적 marketplace](https://azuremarketplace.microsoft.com/marketplace)에 게시 한 SaaS (Software As a Service) 제품 뿐만 아니라 Microsoft에서 게시 한 제품이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="83a5c-116">일부 제안은 고객 당 하나의 구독으로 제한 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="83a5c-117">제한되는 제품 목록을 보려면 파트너 센터 가격 책정 및 제품 페이지를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="83a5c-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="83a5c-118">CSP 프로그램의 파트너는 파트너 센터 내에서 ISV 게시자의 **라이선스 기반** SaaS 구독만 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="83a5c-119">즉, 사용자가 액세스할 수 있는 [전용 제품](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 을 비롯 하 여 ISV 게시자가 사용할 수 있도록 설정한 모든 **라이선스 기반** SaaS 제품을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="83a5c-120">Isv (Azure 응용 프로그램, 컨테이너 또는 Vm과 관련 된 **사용량 기반**, 요금제 또는 소비 기반 제품)에서 기타 상업적 marketplace 제품을 구매 하거나 관리 하려면 [azure 관리 포털](https://portal.azure.com/)로 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="83a5c-121">자세한 내용은 [상용 마켓플레이스 제품 구매](csp-commercial-marketplace-purchase.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="83a5c-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="83a5c-122">새 구독 만들기</span><span class="sxs-lookup"><span data-stu-id="83a5c-122">Create a new subscription</span></span>

1. <span data-ttu-id="83a5c-123">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="83a5c-124">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="83a5c-125">**구독 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-125">Select **Add subscription**.</span></span> <span data-ttu-id="83a5c-126">**온라인 서비스** 탭에는 사용 가능한 Marketplace SaaS 제품이 모두 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="83a5c-127">특정 유형의 구독만 표시하려면 사용 가능한 필터 중에서 원하는 필터를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="83a5c-128">**게시자** **: microsoft를 선택 하** 여 isv가 게시 한 상용 마켓플레이스 **제품을 볼 수 있습니다** .</span><span class="sxs-lookup"><span data-stu-id="83a5c-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="83a5c-129">**청구 유형**: 사용 하려는 구독 청구 유형 ( **라이선스** 또는 **사용**)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="83a5c-130">월간 청구 주기와 연간 청구 주기 중 어떤 것을 선택할지 결정할 때 도움이 되는 정보는 [새 청구 기능에 대한 FAQ](faq-about-new-billing-features.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83a5c-130">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="83a5c-131">**범주**: **Enterprise**, **Small business**또는 **평가판**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="83a5c-132">평가판 구독에 대한 자세한 내용은 [고객에게 Microsoft 제품의 평가판 제공](offer-your-customers-trials-of-microsoft-products.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="83a5c-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="83a5c-133">고객을 위해 구매할 제품 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="83a5c-134">표시 되는 제품은 고객 부문 유형 (교육, 정부 등) 및 적용 한 필터에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="83a5c-135">Marketplace에 표시 된 일부 제안은 특정 고객 또는 특정 CSP 파트너에 게 제공 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="83a5c-136">이는 다음과 같은 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-136">This can be because:</span></span>

   - <span data-ttu-id="83a5c-137">고객은 이미 해당 제품에 대 한 구독을 보유 하 고 있으며 하나만 허용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="83a5c-138">고객의 구독이 일시 중단 되었을 수 있습니다 .이 경우에는 새 구독을 구입 하는 대신 구독을 다시 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="83a5c-139">ISV SaaS 제품의 경우 제품을 구매할 수 없는 몇 가지 이유가 있을 수 있습니다. ISV는 고객의 청구 국가 또는 지역을 지원 하지 않을 수 있습니다. ISV는 CSP 프로그램을 통해 제공 서비스를 제공 하지 않도록 선택할 수 있습니다. 또는 ISV는 특정 CSP 파트너 [에게만 제공 되는 제품을 만들](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="83a5c-140">ISV 제품은 파트너 센터를 통해 불가능 되지 않을 수도 있습니다 (예: 컨테이너 또는 몇 가지 사용 빈도 기반 제안).</span><span class="sxs-lookup"><span data-stu-id="83a5c-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="83a5c-141">추가 하려는 각 구독에 대해 라이선스 수 (필요한 경우)를 입력 하 고 **카트에 추가를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="83a5c-142">구독 추가가 완료 되 면 **검토** 를 선택 하 고 주문을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="83a5c-143">주문을 검토 하 고 이러한 구독을 구매할 준비가 되 면 **구매**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="83a5c-144">고객에 대 한 구독을 구매한 후에는 다음이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="83a5c-145">해당 고객의 **구독** 페이지에서 구독 이름을 선택 하 여 구독을 검토 하거나 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="83a5c-146">여기에서 사용 가능한 경우 추가 기능 라이선스를 선택하거나, 라이선스 수를 변경하거나, 구독을 일시 중단할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="83a5c-147">**ISV SaaS (라이선스 기반) 구독의 경우:**</span><span class="sxs-lookup"><span data-stu-id="83a5c-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="83a5c-148">ISV 게시자 사이트에 대 한 링크를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="83a5c-149">이 링크를 통해 고객 구독의 배포 또는 계정 설정을 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="83a5c-150">이 유형의 ISV 구독에 대 한 계정 설정/프로 비전을 완료 하는 지침이 포함 된 전자 메일은 사용자 또는 고객 모두에 게 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="83a5c-151">구독에 30 일 무료 평가판이 제공 되는 경우 무료 평가판 기간이 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="83a5c-152">CSP 프로그램의 파트너는 고객을 위해 구매한 제품에 대 한 무료 평가판 기간을 되지 않으며 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="83a5c-153">무료 평가판 기간이 종료 되 면 구독 기간이 시작 되 고 구독이 유료 상태로 전환 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="83a5c-154">그러면 구독은 동일한 일정에 따라 autorenew 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-154">The subscription will then autorenew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="83a5c-155">추가 기능을 사용 하 여 구독 업데이트</span><span class="sxs-lookup"><span data-stu-id="83a5c-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="83a5c-156">추가 기능을 구입 하려면 고객에 게 먼저 활성 기본 구독이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="83a5c-157">카탈로그를 통해 추가 기능을 구매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="83a5c-158">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="83a5c-159">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-159">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="83a5c-160">관리 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="83a5c-161">**상태** 섹션 아래에는 구독에 사용할 수 있는 추가 기능 목록이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="83a5c-162">필요한 각 추가 기능에 대 한 라이선스의 수량을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="83a5c-163">그런 다음, 변경 내용을 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="83a5c-164">파트너 센터를 통해 추가 기능을 구입 하는 기능은 CSP 파트너만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-164">The ability to purchase add-ons through Partner Center is only available to CSP partners.</span></span>
<span data-ttu-id="83a5c-165">기본 요구 사항 및 지역 가용성에 따라 적합 한 추가 기능만 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="83a5c-166">가격 책정 및 제안에 대 한 자세한 내용은 Cloud 재판매인 제품 매트릭스를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="83a5c-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="83a5c-167">기본 구독을 일시 중단 하면 연결 된 추가 기능도 일시 중단 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="83a5c-168">추가 기능에 대 한 시작 날짜는 기본 구독에 맞춰 청구 되 고 요금은 청구 시작 날짜와 청구 종료 날짜부터 첫 번째 청구서의 pro-rata 요금으로 계산 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> 


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="83a5c-169">구독 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="83a5c-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="83a5c-170">파트너는 고객이 요청한 경우 또는 지불 이나 사기 행위의 경우 구독을 일시 중단 하거나 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="83a5c-171">구독 일시 중단</span><span class="sxs-lookup"><span data-stu-id="83a5c-171">Suspend a subscription</span></span>

<span data-ttu-id="83a5c-172">구독 상태를 **일시 중지 됨**으로 변경 하면 사용자가 로그인 하거나 서비스에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="83a5c-173">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="83a5c-174">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="83a5c-175">관리 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="83a5c-176">**상태** 섹션에서 **일시 중단됨**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="83a5c-177">그런 다음, 변경 내용을 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="83a5c-178">90일 이내에 또는 90일에 계정이 개설된 시간과 첫 번째 청구 기간 사이의 일 수를 더한 기간(최대 120일) 이내에 구독을 다시 활성화하지 않으면 모든 데이터가 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="83a5c-179">구독을 일시 중단할 경우, **일시 중단** 버튼 아래에 표시된 날짜는 구독을 다시 활성화하지 않을 경우 자동으로 구독이 만료되는 시점을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="83a5c-180">구독 취소</span><span class="sxs-lookup"><span data-stu-id="83a5c-180">Cancel a subscription</span></span>

<span data-ttu-id="83a5c-181">파트너 센터 [상업적 marketplace](csp-commercial-marketplace-overview.md)내에서 타사 ISV 게시자의 라이선스 기반 SaaS 구독을 취소 하는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="83a5c-182">취소 기간 내에 취소 하는 동안에는 전체 환불을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="83a5c-183">매월 청구 되는 ISV 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="83a5c-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="83a5c-184">주문을 넣은 후 24 시간 이내에 취소 하면 다음 청구서에 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="83a5c-185">주문을 넣은 후 24 시간 이상 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="83a5c-186">매년 청구 되는 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="83a5c-186">For offers billed annually:</span></span>

- <span data-ttu-id="83a5c-187">주문을 입력 한 후 14 일 이내에 취소 하면 다음 청구서에서 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="83a5c-188">주문을 입력 한 후 14 일이 지난 후에 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="83a5c-189">이러한 기간이 끝난 후에는 구독을 취소 하는 옵션이 더 이상 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="83a5c-190">사용량 기반 및 요금제로, 가상 컴퓨터 또는 컨테이너를 사용 하는 타사 ISV 서비스는 반환 대상이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="83a5c-191">사용 빈도 기반 서비스를 취소 메서드로 프로 비전 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="83a5c-192">요금 청구는 사용 후 청구 되므로 이러한 서비스는 환불을 받을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="83a5c-193">ISV 게시자에서 라이선스 기반 SaaS 구독을 취소하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="83a5c-194">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="83a5c-195">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="83a5c-196">취소 하려는 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="83a5c-197">**상태** 열에서 **취소**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="83a5c-198">그런 다음, 변경 내용을 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="83a5c-199">대화 상자가 표시 되 면 관련 세부 정보를 입력 한 다음 **제출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="83a5c-200">취소를 확인 하려면 **예, 취소**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="83a5c-201">Api를 사용 하 여 Azure Marketplace 구독을 취소 하도록 선택할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="83a5c-202">이렇게 하려면 [Azure Marketplace 구독 취소](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="83a5c-202">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="83a5c-203">상업용 마켓플레이스 구독을 자동으로 갱신할지 선택</span><span class="sxs-lookup"><span data-stu-id="83a5c-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="83a5c-204">기본적으로 활성 구독은 구독 기간이 만료될 때 자동으로 갱신되도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="83a5c-205">[상업적 marketplace 제품에](csp-commercial-marketplace-overview.md)대 한 구독의 경우 필요에 따라 구독을 자동으로 갱신 하지 않도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="83a5c-206">활성 상업적 marketplace 구독이 자동으로 갱신 되지 않도록 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="83a5c-207">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="83a5c-208">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="83a5c-209">**구독**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-209">Select **Subscriptions**.</span></span> <span data-ttu-id="83a5c-210">고객에 대해 구매한 라이선스 기반 구독을 나열 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="83a5c-211">**구독** 열에서 수정 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="83a5c-212">구독 정보 페이지에서 **상태** 섹션을 찾고 **자동 갱신** 확인란의 선택을 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="83a5c-213">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="83a5c-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="83a5c-214">다음 단계</span><span class="sxs-lookup"><span data-stu-id="83a5c-214">Next steps</span></span>

- [<span data-ttu-id="83a5c-215">고객을 위한 상업용 마켓플레이스 제품</span><span class="sxs-lookup"><span data-stu-id="83a5c-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="83a5c-216">고객을 위한 상업적 마켓플레이스 제품 관리</span><span class="sxs-lookup"><span data-stu-id="83a5c-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="83a5c-217">상용 마켓플레이스 개요</span><span class="sxs-lookup"><span data-stu-id="83a5c-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
