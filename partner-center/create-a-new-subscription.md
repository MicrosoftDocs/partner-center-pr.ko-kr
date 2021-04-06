---
title: 파트너 센터에서 고객 구독 만들기
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 타사 Isv가 게시 한 SaaS 제품 뿐만 아니라 Microsoft에서 게시 한 제품에 대 한 구독을 고객에 게 판매 하는 방법을 알아봅니다.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502938"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="7160e-103">고객 구독 만들기, 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="7160e-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="7160e-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="7160e-104">**Applies to**</span></span>

- <span data-ttu-id="7160e-105">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="7160e-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7160e-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="7160e-106">**Appropriate roles**</span></span>

- <span data-ttu-id="7160e-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="7160e-107">Admin agent</span></span>
- <span data-ttu-id="7160e-108">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="7160e-108">Billing admin</span></span>
- <span data-ttu-id="7160e-109">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="7160e-109">Global admin</span></span>
- <span data-ttu-id="7160e-110">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="7160e-110">Helpdesk agent</span></span>
- <span data-ttu-id="7160e-111">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="7160e-111">Sales agent</span></span>

<span data-ttu-id="7160e-112">파트너 센터에서 고객 기록을 만들면 카탈로그에서 제품의 구독을 판매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="7160e-113">이러한 제품에는 타사 Isv (독립 소프트웨어 공급 업체)가 [상업적 marketplace](https://azuremarketplace.microsoft.com/marketplace)에 게시 한 Microsoft 및 SaaS (Software As a Service) 제품에서 게시 한 제품이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="7160e-114">일부 제안은 고객 당 하나의 구독으로 제한 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="7160e-115">제한되는 제품 목록을 보려면 파트너 센터 가격 책정 및 제품 페이지를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="7160e-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="7160e-116">CSP 프로그램의 파트너는 파트너 센터 내의 ISV 게시자 로부터 **라이선스 기반** 또는 **요금제** SaaS 구독을 구입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="7160e-117">즉, 사용자가 액세스할 수 있는 [전용 제품](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 을 비롯 하 여 ISV 게시자가 사용 가능 하도록 설정한 모든 **라이선스 기반** 또는 **요금제** SaaS 제품을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="7160e-118">Isv의 다른 상업적 marketplace 제품 (예: Azure 응용 프로그램, 컨테이너 또는 Vm을 포함 하는 사용량 기반 제품)을 구입 하거나 관리 하려면 [Azure Portal](https://portal.azure.com/)으로 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="7160e-119">새 구독 만들기</span><span class="sxs-lookup"><span data-stu-id="7160e-119">Create a new subscription</span></span>

1. <span data-ttu-id="7160e-120">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7160e-121">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="7160e-122">**구독 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-122">Select **Add subscription**.</span></span> <span data-ttu-id="7160e-123">**온라인 서비스** 탭에는 사용 가능한 Marketplace SaaS 제품이 모두 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="7160e-124">특정 유형의 구독만 표시하려면 사용 가능한 필터 중에서 원하는 필터를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="7160e-125">**게시자** **: microsoft를 선택 하** 여 isv가 게시 한 상용 마켓플레이스 **제품을 볼 수 있습니다** .</span><span class="sxs-lookup"><span data-stu-id="7160e-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="7160e-126">**청구 유형**: 사용 하려는 구독 청구 유형 ( **라이선스** 또는 **사용**)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="7160e-127">월별 및 연간 청구 빈도를 결정 하는 데 도움이 되는 정보는 [라이선스 기반 청구](license-based-billing.md) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7160e-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="7160e-128">**범주**: **Enterprise**, **Small business** 또는 **평가판** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="7160e-129">평가판 구독에 대한 자세한 내용은 [고객에게 Microsoft 제품의 평가판 제공](offer-your-customers-trials-of-microsoft-products.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7160e-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="7160e-130">고객을 위해 구매할 제품 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="7160e-131">표시 되는 제품은 고객 부문 유형 (교육, 정부 등) 및 적용 한 필터에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="7160e-132">Marketplace에 표시 된 일부 제안은 특정 고객 또는 특정 CSP 파트너에 게 제공 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="7160e-133">이는 다음과 같은 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-133">This can be because:</span></span>

   - <span data-ttu-id="7160e-134">고객은 이미 해당 제품에 대 한 구독을 보유 하 고 있으며 하나만 허용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="7160e-135">고객의 구독이 일시 중단 되었을 수 있습니다 .이 경우에는 새 구독을 구입 하는 대신 구독을 다시 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="7160e-136">ISV SaaS 제품의 경우 제품을 구매할 수 없는 몇 가지 이유가 있을 수 있습니다. ISV는 고객의 청구 국가 또는 지역을 지원 하지 않을 수 있습니다. ISV는 CSP 프로그램을 통해 제공 서비스를 제공 하지 않도록 선택할 수 있습니다. 또는 ISV는 특정 CSP 파트너 [에게만 제공 되는 제품을 만들](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="7160e-137">ISV 제품은 파트너 센터를 통해 불가능 되지 않을 수도 있습니다 (예: 컨테이너 또는 몇 가지 사용 빈도 기반 제안).</span><span class="sxs-lookup"><span data-stu-id="7160e-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="7160e-138">추가 하려는 각 구독에 대해 라이선스 수 (필요한 경우)를 입력 하 고 **카트에 추가를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="7160e-139">구독 추가가 완료 되 면 **검토** 를 선택 하 고 주문을 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="7160e-140">주문을 검토 하 고 이러한 구독을 구매할 준비가 되 면 **구매** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="7160e-141">고객에 대 한 구독을 구매한 후에는 다음이 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="7160e-142">해당 고객의 **구독** 페이지에서 구독 이름을 선택 하 여 구독을 검토 하거나 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="7160e-143">여기에서 사용 가능한 경우 추가 기능 라이선스를 선택하거나, 라이선스 수를 변경하거나, 구독을 일시 중단할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="7160e-144">**ISV SaaS (라이선스 기반 및 요금제) 구독의 경우:**</span><span class="sxs-lookup"><span data-stu-id="7160e-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="7160e-145">ISV 게시자 사이트에 대 한 링크를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="7160e-146">이 링크를 통해 고객 구독의 배포 또는 계정 설정을 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="7160e-147">이 유형의 ISV 구독에 대 한 계정 설정/프로 비전을 완료 하는 지침이 포함 된 전자 메일은 사용자 또는 고객 모두에 게 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="7160e-148">구독에 30 일 무료 평가판이 제공 되는 경우 무료 평가판 기간이 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="7160e-149">CSP 프로그램의 파트너는 고객을 위해 구매한 제품에 대 한 무료 평가판 기간을 되지 않으며 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="7160e-150">무료 평가판 기간이 종료 되 면 구독 기간이 시작 되 고 구독이 유료 상태로 전환 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="7160e-151">그러면 구독은 동일한 일정에 따라 자동 갱신 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="7160e-152">추가 기능을 사용하여 구독 업데이트</span><span class="sxs-lookup"><span data-stu-id="7160e-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="7160e-153">추가 기능을 구매 하려면 먼저 고객이 활성 기본 구독을 보유 하 고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="7160e-154">카탈로그를 통해 추가 기능을 구매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="7160e-155">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7160e-156">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="7160e-157">관리 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="7160e-158">**상태** 섹션 아래에는 구독에 사용할 수 있는 추가 기능 목록이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="7160e-159">필요한 각 추가 기능에 대 한 라이선스의 수량을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="7160e-160">그런 다음, 변경 내용을 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="7160e-161">파트너 센터를 통해 추가 기능을 구입 하는 기능은 직접 청구 및 간접 공급자만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="7160e-162">기본 요구 사항 및 지역 가용성에 따라 적합 한 추가 기능만 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="7160e-163">가격 책정 및 제품에 대 한 자세한 내용은 Cloud 재판매인 제품 매트릭스를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7160e-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="7160e-164">기본 구독을 일시 중단하면 연결된 추가 기능도 일시 중단됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="7160e-165">추가 기능에 대한 시작 날짜는 기본 구독에 맞춰지며 첫 번째 청구서에서 요금은 청구 시작 날짜와 청구 종료 날짜에 비례한 요금으로 계산됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="7160e-166">자세한 내용은 [라이선스 기반 청구](license-based-billing.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7160e-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="7160e-167">구독 일시 중단 또는 취소</span><span class="sxs-lookup"><span data-stu-id="7160e-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="7160e-168">파트너는 고객이 요청한 경우 또는 지불 이나 사기 행위의 경우 구독을 일시 중단 하거나 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="7160e-169">구독 일시 중단</span><span class="sxs-lookup"><span data-stu-id="7160e-169">Suspend a subscription</span></span>

<span data-ttu-id="7160e-170">구독 상태를 **일시 중지 됨** 으로 변경 하면 사용자가 로그인 하거나 서비스에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="7160e-171">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7160e-172">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="7160e-173">관리 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="7160e-174">**상태** 섹션에서 **일시 중단됨** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="7160e-175">그런 다음, 변경 내용을 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="7160e-176">90일 이내에 또는 90일에 계정이 개설된 시간과 첫 번째 청구 기간 사이의 일 수를 더한 기간(최대 120일) 이내에 구독을 다시 활성화하지 않으면 모든 데이터가 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="7160e-177">구독을 일시 중단할 경우, **일시 중단** 버튼 아래에 표시된 날짜는 구독을 다시 활성화하지 않을 경우 자동으로 구독이 만료되는 시점을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="7160e-178">구독 취소</span><span class="sxs-lookup"><span data-stu-id="7160e-178">Cancel a subscription</span></span>

<span data-ttu-id="7160e-179">파트너 센터 [상업적 marketplace](csp-commercial-marketplace-overview.md)내에서 타사 ISV 게시자의 라이선스 기반 SaaS 구독을 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="7160e-180">취소 기간 내에 취소 하는 동안에는 전체 환불을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="7160e-181">매월 청구 되는 ISV 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="7160e-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="7160e-182">주문을 넣은 후 24 시간 이내에 취소 하면 다음 청구서에 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="7160e-183">주문을 넣은 후 24 시간 이상 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="7160e-184">매년 청구 되는 제품의 경우:</span><span class="sxs-lookup"><span data-stu-id="7160e-184">For offers billed annually:</span></span>

- <span data-ttu-id="7160e-185">주문을 입력 한 후 14 일 이내에 취소 하면 다음 청구서에서 전체 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="7160e-186">주문을 입력 한 후 14 일이 지난 후에 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="7160e-187">이러한 기간이 끝난 후에는 구독을 취소 하는 옵션이 더 이상 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="7160e-188">사용량 기반 및 요금제로, 가상 컴퓨터 또는 컨테이너를 사용 하는 타사 ISV 서비스는 반환 대상이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="7160e-189">사용 빈도 기반 서비스를 취소 메서드로 프로 비전 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="7160e-190">요금 청구는 사용 후 청구 되므로 이러한 서비스는 환불을 받을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="7160e-191">ISV 게시자에서 라이선스 기반 SaaS 구독을 취소하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="7160e-192">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7160e-193">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="7160e-194">취소 하려는 구독을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="7160e-195">**상태** 열에서 **취소** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="7160e-196">그런 다음, 변경 내용을 **제출** 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="7160e-197">대화 상자가 표시 되 면 관련 세부 정보를 입력 한 다음 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="7160e-198">취소를 확인 하려면 **예, 취소** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="7160e-199">Api를 사용 하 여 Azure Marketplace 구독을 취소 하도록 선택할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="7160e-200">이렇게 하려면 [Azure Marketplace 구독 취소](/partner-center/develop/cancel-an-azure-marketplace-subscription)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7160e-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="7160e-201">상업용 마켓플레이스 구독을 자동으로 갱신할지 선택</span><span class="sxs-lookup"><span data-stu-id="7160e-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="7160e-202">기본적으로 활성 구독은 구독 기간이 만료될 때 자동으로 갱신되도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="7160e-203">[상업적 marketplace 제품에](csp-commercial-marketplace-overview.md)대 한 구독의 경우 필요에 따라 구독을 자동으로 갱신 하지 않도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="7160e-204">활성 상업적 marketplace 구독이 자동으로 갱신 되지 않도록 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="7160e-205">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7160e-206">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="7160e-207">**구독** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-207">Select **Subscriptions**.</span></span> <span data-ttu-id="7160e-208">고객에 대해 구매한 라이선스 기반 구독을 나열 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="7160e-209">**구독** 열에서 수정 하려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="7160e-210">구독 정보 페이지에서 **상태** 섹션을 찾고 **자동 갱신** 확인란의 선택을 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="7160e-211">**제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7160e-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7160e-212">다음 단계</span><span class="sxs-lookup"><span data-stu-id="7160e-212">Next steps</span></span>

- [<span data-ttu-id="7160e-213">고객을 위한 상업용 마켓플레이스 제품</span><span class="sxs-lookup"><span data-stu-id="7160e-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="7160e-214">고객을 위한 상업적 마켓플레이스 제품 관리</span><span class="sxs-lookup"><span data-stu-id="7160e-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="7160e-215">상용 마켓플레이스 개요</span><span class="sxs-lookup"><span data-stu-id="7160e-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)