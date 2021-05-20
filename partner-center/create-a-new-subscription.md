---
title: 파트너 센터 고객 구독 만들기
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 타사 ISV에서 게시한 SaaS 제품뿐만 아니라 Microsoft에서 게시한 제품에 대한 구독을 고객에게 판매하는 방법을 알아봅니다.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201411"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="1ad28-103">고객 구독 만들기, 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="1ad28-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="1ad28-104">**적용된 내용:** 파트너 센터 | Microsoft Cloud for US Government 대한 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="1ad28-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="1ad28-105">**적절한 역할:** 관리 에이전트 | 청구 관리자 | 전역 관리자 | Helpdesk 에이전트 | 판매 에이전트</span><span class="sxs-lookup"><span data-stu-id="1ad28-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="1ad28-106">파트너 센터에서 고객 기록을 만들면 카탈로그에서 제품의 구독을 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="1ad28-107">여기에는 Microsoft 및 SaaS(Software as a Service) 제품이 타사 ISV(Independent Software Vendor)에서 [상업용 Marketplace에](https://azuremarketplace.microsoft.com/marketplace)게시한 제품이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="1ad28-108">일부 제안은 고객당 하나의 구독으로 제한됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="1ad28-109">제한되는 제품 목록을 보려면 파트너 센터 가격 책정 및 제품 페이지를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="1ad28-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="1ad28-110">CSP 프로그램의 파트너는 파트너 센터 내에서 ISV 게시자로부터 **라이선스 기반** 또는 **요금제** SaaS 구독을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="1ad28-111">즉, 액세스 권한이 있는 단독 제안을 포함하여 ISV 게시자가 제공하는 **라이선스 기반** 또는 **요금제** SaaS [제안을](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="1ad28-112">ISV에서 다른 상업용 Marketplace 제안(예: Azure 애플리케이션, 컨테이너 또는 VM과 관련된 사용량 기반 제안)을 구매하거나 관리하려면 [Azure Portal](https://portal.azure.com/)이동해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="1ad28-113">파트너 센터 모든 날짜와 시간은 UTC(협정 세계시) 표준에 지정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="1ad28-114">현지 시간과 최대 24시간이 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="1ad28-115">새 구독 만들기</span><span class="sxs-lookup"><span data-stu-id="1ad28-115">Create a new subscription</span></span>

1. <span data-ttu-id="1ad28-116">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1ad28-117">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1ad28-118">**구독 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-118">Select **Add subscription**.</span></span> <span data-ttu-id="1ad28-119">**온라인 서비스** 탭에는 사용 가능한 모든 Marketplace SaaS 제안이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="1ad28-120">특정 유형의 구독만 표시하려면 사용 가능한 필터 중에서 원하는 필터를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="1ad28-121">**게시자:** **Microsoft** 또는 **파트너의** 제품만 보려면 Microsoft를 선택하고 ISV에서 게시한 상업용 Marketplace 제품을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="1ad28-122">**청구 유형:** 사용하려는 구독 청구 **유형(라이선스** 또는 **사용량)을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="1ad28-123">월별 [청구 빈도와](license-based-billing.md) 연간 청구 빈도를 결정하는 데 도움이 되는 정보는 라이선스 기반 청구를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1ad28-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="1ad28-124">**범주:** **엔터프라이즈,** **중소기업** 또는 **평가판을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="1ad28-125">평가판 구독에 대한 자세한 내용은 [고객에게 Microsoft 제품의 평가판 제공](offer-your-customers-trials-of-microsoft-products.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1ad28-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="1ad28-126">고객을 위해 구매할 제품 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="1ad28-127">표시 되는 제품은 고객 부문 유형 (교육, 정부 등) 및 적용 한 필터에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="1ad28-128">Marketplace에 표시 된 일부 제안은 특정 고객 또는 특정 CSP 파트너에 게 제공 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="1ad28-129">이는 다음과 같은 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-129">This can be because:</span></span>

   - <span data-ttu-id="1ad28-130">고객은 이미 해당 제품에 대 한 구독을 보유 하 고 있으며 하나만 허용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="1ad28-131">고객의 구독이 일시 중단 되었을 수 있습니다 .이 경우에는 새 구독을 구입 하는 대신 구독을 다시 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="1ad28-132">ISV SaaS 제품의 경우 제품을 구매할 수 없는 몇 가지 이유가 있을 수 있습니다. ISV는 고객의 청구 국가 또는 지역을 지원 하지 않을 수 있습니다. ISV는 CSP 프로그램을 통해 제공 서비스를 제공 하지 않도록 선택할 수 있습니다. 또는 ISV는 특정 CSP 파트너 [에게만 제공 되는 제품을 만들](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="1ad28-133">ISV 제품은 파트너 센터를 통해 불가능 되지 않을 수도 있습니다 (예: 컨테이너 또는 몇 가지 사용 빈도 기반 제안).</span><span class="sxs-lookup"><span data-stu-id="1ad28-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="1ad28-134">추가 하려는 각 구독에 대해 라이선스 수 (필요한 경우)를 입력 하 고 **카트에 추가를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="1ad28-135">구독 추가가 완료 되 면 **검토** 를 선택 하 고 주문을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="1ad28-136">주문을 검토 하 고 이러한 구독을 구매할 준비가 되 면 **구매** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="1ad28-137">고객에 대 한 구독을 구매한 후에는 다음이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="1ad28-138">해당 고객의 **구독** 페이지에서 구독 이름을 선택 하 여 구독을 검토 하거나 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="1ad28-139">여기에서 사용 가능한 경우 추가 기능 라이선스를 선택하거나, 라이선스 수를 변경하거나, 구독을 일시 중단할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="1ad28-140">**ISV SaaS (라이선스 기반 및 요금제) 구독의 경우:**</span><span class="sxs-lookup"><span data-stu-id="1ad28-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="1ad28-141">ISV 게시자 사이트에 대 한 링크를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="1ad28-142">이 링크를 통해 고객 구독의 배포 또는 계정 설정을 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="1ad28-143">이 유형의 ISV 구독에 대 한 계정 설정/프로 비전을 완료 하는 지침이 포함 된 전자 메일은 사용자 또는 고객 모두에 게 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="1ad28-144">구독에 30 일 무료 평가판이 제공 되는 경우 무료 평가판 기간이 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="1ad28-145">CSP 프로그램의 파트너는 고객을 위해 구매한 제품에 대 한 무료 평가판 기간을 되지 않으며 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="1ad28-146">평가판 기간이 종료되면 구독 기간이 시작되고 구독이 유료 상태로 전환됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="1ad28-147">그러면 구독이 동일한 일정에 따라 자동 갱신됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="1ad28-148">추가 기능을 사용하여 구독 업데이트</span><span class="sxs-lookup"><span data-stu-id="1ad28-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="1ad28-149">추가 기능 구매를 위해 고객은 먼저 활성 기본 구독이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="1ad28-150">카탈로그를 통해 추가 기능을 구매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="1ad28-151">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1ad28-152">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1ad28-153">관리하려는 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="1ad28-154">**상태** 섹션 아래에는 구독에 사용 가능한 추가 기능 목록이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="1ad28-155">필요한 각 추가 기능의 라이선스 수량을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="1ad28-156">그런 다음, 변경 내용을 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="1ad28-157">파트너 센터 통해 추가 기능을 구매하는 기능은 직접 청구 및 간접 공급자에게만 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="1ad28-158">기본 요구 사항 및 지역별 가용성에 따라 적격 추가 기능만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="1ad28-159">가격 책정 및 제안에 대한 자세한 내용은 Cloud Reseller 제품 매트릭스를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1ad28-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="1ad28-160">기본 구독을 일시 중단하면 연결된 추가 기능도 일시 중단됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="1ad28-161">추가 기능에 대한 시작 날짜는 기본 구독에 맞춰지며 첫 번째 청구서에서 요금은 청구 시작 날짜와 청구 종료 날짜에 비례한 요금으로 계산됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="1ad28-162">자세한 내용은 [라이선스 기반 청구를 참조하세요.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="1ad28-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="1ad28-163">구독 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="1ad28-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="1ad28-164">파트너는 고객이 요청한 경우 또는 미지불 또는 사기의 경우 구독을 일시 중단하거나 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="1ad28-165">구독 일시 중단</span><span class="sxs-lookup"><span data-stu-id="1ad28-165">Suspend a subscription</span></span>

<span data-ttu-id="1ad28-166">구독 상태를 **일시 중단으로** 변경하면 사용자가 로그인하거나 서비스에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="1ad28-167">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1ad28-168">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1ad28-169">관리하려는 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="1ad28-170">**상태** 섹션에서 **일시 중단됨** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="1ad28-171">그런 다음, 변경 내용을 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="1ad28-172">90일 이내에 또는 90일에 계정이 개설된 시간과 첫 번째 청구 기간 사이의 일 수를 더한 기간(최대 120일) 이내에 구독을 다시 활성화하지 않으면 모든 데이터가 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="1ad28-173">구독을 일시 중단할 경우, **일시 중단** 버튼 아래에 표시된 날짜는 구독을 다시 활성화하지 않을 경우 자동으로 구독이 만료되는 시점을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="1ad28-174">CSP 구독에는 만료된 기간(웹 직접 구독의 방식)이 없으며 서비스가 계속 작동하지만 구독에서 청구 요금이 생성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="1ad28-175">CSP 구독은 활성 또는 일시 중단되거나 완전히 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="1ad28-176">구독 취소</span><span class="sxs-lookup"><span data-stu-id="1ad28-176">Cancel a subscription</span></span>

<span data-ttu-id="1ad28-177">파트너 센터 상업용 Marketplace 내의 타사 ISV 게시자에서 라이선스 기반 SaaS 구독을 취소할 수 [있습니다.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="1ad28-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="1ad28-178">취소 기간 내에 취소하는 한 전체 환불을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="1ad28-179">ISV의 경우 매월 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="1ad28-180">주문을 한 후 24시간 이내에 취소하면 다음 청구서에서 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="1ad28-181">주문을 한 후 24시간 후에 취소하는 경우 갱신 시 취소가 발생하도록 예약됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="1ad28-182">매년 청구 되는 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="1ad28-182">For offers billed annually:</span></span>

- <span data-ttu-id="1ad28-183">주문을 입력 한 후 14 일 이내에 취소 하면 다음 청구서에서 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="1ad28-184">주문을 입력 한 후 14 일이 지난 후에 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="1ad28-185">이러한 기간이 끝난 후에는 구독을 취소 하는 옵션이 더 이상 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="1ad28-186">사용량 기반 및 요금제로, 가상 컴퓨터 또는 컨테이너를 사용 하는 타사 ISV 서비스는 반환 대상이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="1ad28-187">사용 빈도 기반 서비스를 취소 메서드로 프로 비전 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="1ad28-188">요금 청구는 사용 후 청구 되므로 이러한 서비스는 환불을 받을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="1ad28-189">ISV 게시자에서 라이선스 기반 SaaS 구독을 취소하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="1ad28-190">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1ad28-191">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1ad28-192">취소 하려는 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="1ad28-193">**상태** 열에서 **취소** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="1ad28-194">그런 다음, 변경 내용을 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="1ad28-195">대화 상자가 표시 되 면 관련 세부 정보를 입력 한 다음 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="1ad28-196">취소를 확인 하려면 **예, 취소** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="1ad28-197">Api를 사용 하 여 Azure Marketplace 구독을 취소 하도록 선택할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="1ad28-198">이렇게 하려면 [Azure Marketplace 구독 취소](/partner-center/develop/cancel-an-azure-marketplace-subscription)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="1ad28-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="1ad28-199">상업용 마켓플레이스 구독을 자동으로 갱신할지 선택</span><span class="sxs-lookup"><span data-stu-id="1ad28-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="1ad28-200">기본적으로 활성 구독은 구독 기간이 만료될 때 자동으로 갱신되도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="1ad28-201">[상업적 marketplace 제품에](csp-commercial-marketplace-overview.md)대 한 구독의 경우 필요에 따라 구독을 자동으로 갱신 하지 않도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="1ad28-202">활성 상업적 marketplace 구독이 자동으로 갱신 되지 않도록 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="1ad28-203">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1ad28-204">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1ad28-205">**구독** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-205">Select **Subscriptions**.</span></span> <span data-ttu-id="1ad28-206">고객에 대해 구매한 라이선스 기반 구독을 나열 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="1ad28-207">**구독** 열에서 수정 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="1ad28-208">구독 정보 페이지에서 **상태** 섹션을 찾고 **자동 갱신** 확인란의 선택을 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="1ad28-209">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1ad28-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1ad28-210">다음 단계</span><span class="sxs-lookup"><span data-stu-id="1ad28-210">Next steps</span></span>

- [<span data-ttu-id="1ad28-211">고객을 위한 상업용 마켓플레이스 제품</span><span class="sxs-lookup"><span data-stu-id="1ad28-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="1ad28-212">고객을 위한 상업적 마켓플레이스 제품 관리</span><span class="sxs-lookup"><span data-stu-id="1ad28-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="1ad28-213">상용 마켓플레이스 개요</span><span class="sxs-lookup"><span data-stu-id="1ad28-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)