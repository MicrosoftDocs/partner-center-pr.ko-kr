---
title: 상업적 marketplace 제품에 대 한 청구 | 파트너 센터
ms.topic: article
ms.date: 02/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 내에서 상업적 marketplace의 고객을 위해 구매한 ISV SaaS 제품 또는 구독에 대 한 청구 작동 방식을 알아봅니다.
author: MicheleHope
ms.author: v-mihope
keywords: 구독, 제품, 구매, Marketplace, 제 3 자, ISV, 청구, 송장, 조정, 정찰 파일
ms.localizationpriority: medium
ms.openlocfilehash: 35db6e9e1fbdfe5e455e5b4e73e39b76cad496aa
ms.sourcegitcommit: 717ef04f5c0040611af3ba9e5a324ab67e99ba14
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/03/2020
ms.locfileid: "78240200"
---
# <a name="billing-for-commercial-marketplace-products"></a><span data-ttu-id="231f6-104">상업적 marketplace 제품에 대 한 청구</span><span class="sxs-lookup"><span data-stu-id="231f6-104">Billing for commercial marketplace products</span></span>

<span data-ttu-id="231f6-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="231f6-105">**Applies to**</span></span>

- <span data-ttu-id="231f6-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="231f6-106">Partner Center</span></span>
- <span data-ttu-id="231f6-107">CSP 프로그램의 파트너</span><span class="sxs-lookup"><span data-stu-id="231f6-107">Partners in the CSP program</span></span>

<span data-ttu-id="231f6-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="231f6-108">**Appropriate roles**</span></span>

- <span data-ttu-id="231f6-109">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="231f6-109">Global admin</span></span>
- <span data-ttu-id="231f6-110">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="231f6-110">Billing admin</span></span>

<span data-ttu-id="231f6-111">CSP 프로그램에서 파트너는 파트너 센터를 사용 하 여 상업적 marketplace의 ISV 게시자 로부터 라이선스 기반 SaaS 제품을 구매할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-111">As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace.</span></span> <span data-ttu-id="231f6-112">이렇게 하면 이러한 유형의 구매 청구서에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-112">After you do so, you can access a bill for these types of purchases.</span></span> <span data-ttu-id="231f6-113">청구 기간은 해당 월의 첫 번째 날부터 시작 하 여 월의 마지막 날에 끝납니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-113">The billing period starts on the first day of the calendar month and ends on the last day of the calendar month.</span></span> <span data-ttu-id="231f6-114">청구서는 다음 달의 여덟 번째 날에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-114">Invoices are made available on the 8th day of the following month.</span></span>

<span data-ttu-id="231f6-115">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/) 또는 [파트너 센터 api](https://docs.microsoft.com/partner-center/develop/)를 사용 하 여 청구서에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-115">You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="231f6-116">CSP 프로그램의 파트너는 파트너 센터 또는 Azure Portal (고객의 이전 CSP 구매한 Azure 테 넌 트를 사용 하 여)에서 해당 제품을 구매할 때 고객이 구매한 ISV 상용 marketplace 솔루션에 대 한 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-116">Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).</span></span>

>[!NOTE]
><span data-ttu-id="231f6-117">고객이 자신의 Azure AD 테 넌 트를 사용 하는 경우 (CSP 프로그램에서 파트너 로부터 구매한 것이 아닌 경우), 고객은 ([Microsoft AppSource](https://appsource.microsoft.com/) 또는 [Azure Marketplace](https://azuremarketplace.microsoft.com/))에서 직접 자체 ISV SaaS 솔루션을 구매할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-117">If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)).</span></span> <span data-ttu-id="231f6-118">이러한 작업을 수행 하는 경우 Microsoft에서 직접 자신의 청구서를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-118">If they do so, they will receive their own bill directly from Microsoft.</span></span> <span data-ttu-id="231f6-119">마찬가지로, CSP 프로그램의 파트너가 Azure 구독 또는 새 Azure 계획을 고객에 게 판매 하 고 해당 테 넌 트에 대해 고객 (또는 간접 재판매인)의 [역할 기반 액세스](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) 권한을 부여 하는 경우 (또는 간접 **재판매인)는**csp 파트너에 게 사전 승인 또는 알림 없이 상업적 마켓플레이스 제품을 구매할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-119">Likewise, if a partner in the CSP program sells an Azure subscription or the new Azure plan to the customer and grants the customer (or indirect reseller) [role-based access](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer (or indirect reseller) can also purchase commercial marketplace offers without prior approval or notification to the CSP partner.</span></span> <span data-ttu-id="231f6-120">이러한 경우 Microsoft는 CSP 프로그램에서 고객의 구매에 대 한 파트너에 게 직접 알리지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-120">In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers.</span></span> <span data-ttu-id="231f6-121">그러나 Microsoft는 Azure 구독에 대 한 작업에 대 한 알림 또는 알림을 설정 하는 데 사용할 수 있는 선택적 [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) 메커니즘을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-121">However, Microsoft does offer an optional [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.</span></span>

## <a name="access-billing-information-for-commercial-marketplace-products"></a><span data-ttu-id="231f6-122">상용 marketplace 제품에 대 한 청구 정보 액세스</span><span class="sxs-lookup"><span data-stu-id="231f6-122">Access billing information for commercial marketplace products</span></span>

<span data-ttu-id="231f6-123">청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-123">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> <span data-ttu-id="231f6-124">상용 marketplace 제품 구매를 위한 최신 청구서 및 조정 파일에 액세스 하려면:</span><span class="sxs-lookup"><span data-stu-id="231f6-124">To access the latest invoice and reconciliation file for commercial marketplace product purchases:</span></span>

1. <span data-ttu-id="231f6-125">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-125">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="231f6-126">파트너 센터 메뉴에서 **청구**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-126">From the Partner Center menu, select **Billing**.</span></span> 

    <span data-ttu-id="231f6-127">청구 페이지의 맨 위에 **되풀이** 및 **되풀이 및 일회성 구매**라는 두 개의 탭이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-127">You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**.</span></span> <span data-ttu-id="231f6-128">각 탭에서 여러 marketplace 제품에 대 한 정찰 (청구서 및 조정) 파일에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-128">Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:</span></span>

    - <span data-ttu-id="231f6-129">**되풀이** 탭: Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro 및 Microsoft Azure와 관련 된 구독의 청구서 및 조정 파일을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-129">**Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro, and Microsoft Azure.</span></span>

    - <span data-ttu-id="231f6-130">**되풀이 및 일회성 구매** 탭: azure 요금제, azure 예약, 소프트웨어 및 상업적 marketplace 제품에 대 한 송장 및 조정 파일이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-130">**Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.</span></span>
  
3. <span data-ttu-id="231f6-131">**되풀이 및 일회성 구매** 탭을 선택 합니다. 다른 통화로 고객에 대 한 구독을 구매한 경우 각 통화에 대 한 탭이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-131">Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency.</span></span> <span data-ttu-id="231f6-132">이 페이지에서는 다음과 같은 몇 가지 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-132">You can do a few things fr:om this page:</span></span>

    - <span data-ttu-id="231f6-133">최신 청구서 및 조정 파일을 보려면 **청구서** 또는 **조정 파일**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-133">To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**.</span></span> <span data-ttu-id="231f6-134">원할 경우 [파트너 센터 api](https://docs.microsoft.com/partner-center/develop/)를 사용 하 여 최신 청구서 및 정찰 파일 데이터에 액세스할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-134">(If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

    - <span data-ttu-id="231f6-135">이전 청구서 및 정찰 파일을 보려면 아래 **청구 기록** 행을 확장 하십시오.</span><span class="sxs-lookup"><span data-stu-id="231f6-135">To see earlier invoices and recon files, expand the **Billing history** row below.</span></span>

    - <span data-ttu-id="231f6-136">최근 계정 작업을 기준으로 언제 든 지 예상 계정 잔액 또는 청구서를 확인 하려면 **견적** 제목에서 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-136">To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.</span></span>  

    >[!NOTE]
    > <span data-ttu-id="231f6-137">해당 월의 여덟 번째 날에 청구서를 게시할 때 세금 및 기타 적용 가능한 모든 요금 및 크레딧이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-137">When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits.</span></span> <span data-ttu-id="231f6-138">즉, 최종 금액이 청구 기간 중에 표시 되는 것과 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-138">This means the final amount due might differ from what you see during the billing period.</span></span>

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a><span data-ttu-id="231f6-139">상업적 marketplace 제품에 대 한 청구서 및 정찰 파일에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="231f6-139">More about invoices and recon files for commercial marketplace products</span></span>

<span data-ttu-id="231f6-140">이 섹션에서는 타사 ISV 게시자의 고객을 위해 구매한 상용 marketplace SaaS 구독의 청구서 및 조정 파일에 대해 자세히 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-140">This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.</span></span>

<span data-ttu-id="231f6-141">파트너 센터 메뉴의 **청구** 옵션에서 **되풀이 및 일회성 구매** 를 선택 하는 경우 Microsoft (자사) 및 ISV (타사) 구매와 관련 된 요금에 대 한 청구서 및 조정 파일에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-141">When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases.</span></span> <span data-ttu-id="231f6-142">이러한 구매는 다음에 연결 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-142">These purchases may be associated with:</span></span>

- <span data-ttu-id="231f6-143">SaaS 구독 (Microsoft 또는 ISV 게시자)</span><span class="sxs-lookup"><span data-stu-id="231f6-143">SaaS subscriptions (from either Microsoft or ISV publishers)</span></span>

- <span data-ttu-id="231f6-144">Azure 플랜</span><span class="sxs-lookup"><span data-stu-id="231f6-144">Azure plan</span></span>

- <span data-ttu-id="231f6-145">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="231f6-145">Azure reservations</span></span>

- <span data-ttu-id="231f6-146">기타 구독 기반 소프트웨어 (Microsoft 또는 ISV 게시자)</span><span class="sxs-lookup"><span data-stu-id="231f6-146">Other subscription-based software (from either Microsoft or ISV publishers)</span></span>

<span data-ttu-id="231f6-147">이러한 구매의 예로는 SUSE Linux software (소프트웨어 구독) 또는 Azure ISV SaaS 제품 구독이 포함 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-147">Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.</span></span>

>[!NOTE]
> <span data-ttu-id="231f6-148">청구서 및 정찰 파일을 읽는 방법에 대 한 자세한 내용은 [청구 개요](billing.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="231f6-148">For more information about how to read invoice and recon files, see also [Billing overview](billing.md).</span></span>

### <a name="tips-on-reading-your-invoice"></a><span data-ttu-id="231f6-149">청구서 읽기 팁</span><span class="sxs-lookup"><span data-stu-id="231f6-149">Tips on reading your invoice</span></span>

<span data-ttu-id="231f6-150">타사 ISV 게시자 로부터 라이선스 기반 SaaS 제품을 구매 하는 경우 청구서에 대 한 라이선스 요금에 대 한 요금이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-150">When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice.</span></span> <span data-ttu-id="231f6-151">ISV의 SaaS 제품이 기본 Azure 인프라 리소스를 사용 하거나 소비 하는 경우에도 마찬가지입니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-151">This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources.</span></span> <span data-ttu-id="231f6-152">ISV의 SaaS 제품에 대 한 고객의 Azure 인프라 사용 요금은 ISV에 직접 청구 되기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-152">That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV.</span></span> <span data-ttu-id="231f6-153">Isv는 자신의 Azure 사용량이 매일 등급 청구 조정 파일에 연결 된 Azure 사용량 요금을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-153">(ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)</span></span>

<span data-ttu-id="231f6-154">청구서에는 다음과 같은 여러 페이지가 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-154">Your invoice will contain several pages:</span></span>

- <span data-ttu-id="231f6-155">**청구서의 1 페이지:** CSP 프로그램 파트너의 청구 정보에 대 한 요약 개요를 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-155">**Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details.</span></span> <span data-ttu-id="231f6-156">여기에는 청구 기간에 대 한 요금, 청구서 번호, 지불 약관 (순 60 일) 및 요금 청구 지불 방법에 대 한 요약 (통신 또는 확인)이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-156">This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.</span></span>

- <span data-ttu-id="231f6-157">**청구서의 2 페이지 (및 모든 후속 페이지):** 상업적 marketplace의 자사 Microsoft 구매 및 타사 ISV (라이선스 기반) 구매에 대 한 요금을 청구 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-157">**Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace.</span></span> <span data-ttu-id="231f6-158">각 제품 이름 아래의 **게시자** 줄에서 ISV 라이선스 기반 구매를 식별할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-158">You can identify ISV license-based purchases by the **Publisher** line beneath each product name.</span></span> <span data-ttu-id="231f6-159">관련 조정 파일은 특정 송장 요금에 대 한 더 많은 청구 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-159">The associated reconciliation file offers more billing details for specific invoice charges.</span></span>

- <span data-ttu-id="231f6-160">**청구서의 마지막 페이지:** ISV의 라이선스 기반 marketplace 제품에 대 한 요금이 청구 되는 경우이 마지막 페이지에 ISV 게시자 이름 및 주소에 대 한 자세한 정보가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-160">**Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.</span></span>

### <a name="tips-on-reading-your-reconciliation-file"></a><span data-ttu-id="231f6-161">조정 파일을 읽는 방법에 대 한 팁</span><span class="sxs-lookup"><span data-stu-id="231f6-161">Tips on reading your reconciliation file</span></span>

<span data-ttu-id="231f6-162">**되풀이 및 일회성 구매** 조정 파일에는 청구서의 요금에 매핑되는 추가 세부 정보를 포함 하는 여러 열이 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-162">The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice.</span></span> <span data-ttu-id="231f6-163">가 나 **ername** 열은 Microsoft 또는 타사 ISV 게시자의 구매 여부를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-163">The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.</span></span>

<span data-ttu-id="231f6-164">조정 파일의 일부 요금은 비용은 $0로 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-164">Some charges in your reconciliation file may appear with a cost of $0.</span></span> <span data-ttu-id="231f6-165">ISV "무료 평가판" 제안 (일반적으로 30 또는 60 일) 또는 사용자 라이선스 제품을 제공 하기 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-165">This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.</span></span>

<span data-ttu-id="231f6-166">무료 평가판 ISV의 경우 다음을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-166">In the case of free trial ISV offers:</span></span>

- <span data-ttu-id="231f6-167">무료 평가판 기간은 해당 시간 동안 ISV의 라이선스 기반 SaaS 제품 비용을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-167">The free trial period covers the cost of the ISV's license-based SaaS product during that time.</span></span> <span data-ttu-id="231f6-168">또한 해당 SaaS 제품의 관련 Azure 인프라 사용에 대 한 요금이 청구 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-168">You will also not be charged for associated Azure infrastructure use of that SaaS product.</span></span>  <span data-ttu-id="231f6-169">그러나 사용량 기반 ISV 제품을 사용 하는 경우 무료 평가판에는 기본 Azure 인프라 사용량의 비용이 포함 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-169">If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage.</span></span> <span data-ttu-id="231f6-170">이 경우 Azure 인프라 사용 요금은 별도의 Azure 조정 파일에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-170">In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.</span></span>

- <span data-ttu-id="231f6-171">고객을 위해 ISV의 무료 평가판 적격 제품을 구매 하 여 배포할 경우 ISV 게시자는 평가판에 자동으로 등록 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-171">When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher.</span></span> <span data-ttu-id="231f6-172">ISV 게시자가 정의한 기간 후에는 무료 평가판 기간이 자동으로 종료 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-172">The free trial period ends automatically after the period defined by the ISV publisher.</span></span> <span data-ttu-id="231f6-173">기간이 종료 되 면 고객에 게 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-173">After the period ends, the customer will be charged.</span></span> <span data-ttu-id="231f6-174">즉, 조정 파일은 평가 기간을 추적 하는 제품 및 유료 제품을 추적 하는 제품 (평가 기간이 종료 될 때까지 $0 비용을 표시 함)에 대 한 2 개의 행을 표시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-174">This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends).</span></span> <span data-ttu-id="231f6-175">평가판이 종료 되 면 유료 제품을 표시 하는 행이 요금을 표시 하기 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="231f6-175">Once the trial ends, the row showing the paid offer will start to show charges.</span></span> 

<span data-ttu-id="231f6-176">각 열이 나타내는 내용에 대 한 자세한 내용은 [조정 파일 사용](use-the-reconciliation-files.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="231f6-176">For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md).</span></span> <span data-ttu-id="231f6-177">[파트너 센터에서 청구 유형](billing-different-types.md) 도 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="231f6-177">See also [Types of billing in Partner Center](billing-different-types.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="231f6-178">다음 단계</span><span class="sxs-lookup"><span data-stu-id="231f6-178">Next Steps</span></span>

- [<span data-ttu-id="231f6-179">고객을 위한 상용 마켓플레이스 제품 관리</span><span class="sxs-lookup"><span data-stu-id="231f6-179">Manage commercial marketplace products for customers</span></span>](csp-commercial-marketplace-manage.md)
- [<span data-ttu-id="231f6-180">상용 마켓플레이스 제품 지원에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="231f6-180">Learn about support for commercial marketplace products</span></span>](csp-commercial-marketplace-support.md)
