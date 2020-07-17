---
title: 청구서 & 정찰 파일을 읽는 방법
ms.topic: article
ms.date: 06/05/2020
description: 청구서 & 조정 파일에 대해 알아봅니다. 청구서에는 해당 월간 기간의 프로그램, 제품 및 고객에 대 한 파트너 센터 요금이 표시 됩니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4b91b2f9580d9c369e7a267c2b413db8a4a6300d
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436632"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a><span data-ttu-id="4babe-104">청구서 및 조정 파일 이해-파트너 센터에서 해당 파일을 찾는 방법을 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-104">Understand your bill and reconciliation file - learn how to find them in Partner Center</span></span>

<span data-ttu-id="4babe-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="4babe-105">**Applies to**</span></span>

- <span data-ttu-id="4babe-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4babe-106">Partner Center</span></span>
- <span data-ttu-id="4babe-107">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4babe-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="4babe-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="4babe-108">**Appropriate roles**</span></span>

- <span data-ttu-id="4babe-109">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="4babe-109">Global admin</span></span>
- <span data-ttu-id="4babe-110">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="4babe-110">Billing admin</span></span>
- <span data-ttu-id="4babe-111">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="4babe-111">Admin agent</span></span>


<span data-ttu-id="4babe-112">**청구서** 는 **모든 파트너 센터 요금** (프로그램, 모든 제품 및 모든 고객)에 대 한 요약입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-112">Your **invoice** is a **summary of all your Partner Center charges** (across the program, all products, and all customers).</span></span> 

## <a name="invoice-types"></a><span data-ttu-id="4babe-113">송장 유형</span><span class="sxs-lookup"><span data-stu-id="4babe-113">Invoice types</span></span>

<span data-ttu-id="4babe-114">Microsoft는 라이선스 기반 요금 (예: Office 365) 및 사용량 기반 요금 (예: Azure)에 대해 하나의 송장을 발급 하 고, 일회성 요금 (예: Azure RI, Marketplace 또는 Azure 요금제)에 대 한 별도의 송장을 발급 합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-114">Microsoft will issue one invoice for any license-based charges (such as Office 365) and usage-based charges (such as Azure) and a separate invoice for one-time charges (such as Azure RI, Marketplace, or Azure plan).</span></span>

<span data-ttu-id="4babe-115">예를 들면 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-115">For example,</span></span>  

<span data-ttu-id="4babe-116">**시나리오 1 [단일 통화]**: 파트너가 145P 제품 및 O365 라이선스를 구입 했습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-116">**Scenario 1 [Single Currency]**: Partner has purchases for 145P offer and O365 licenses,</span></span>  

- <span data-ttu-id="4babe-117">파트너는 O365 및 Azure (145p) 모두에 대 한 요금을 포함 하는 하나의 송장 PDF 및 2 조정 파일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-117">Partner will get one invoice PDF and 2 reconciliation files covering the charges for both O365 and Azure (145p).</span></span>  

<span data-ttu-id="4babe-118">**시나리오 2 [단일 통화]**: 파트너가 145p 구매와 함께 azure RI, Marketplace 및/또는 azure 요금제에 대 한 구매를 보유 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-118">**Scenario 2 [Single Currency]**: Partner has purchases for Azure RI, Marketplace and/or Azure plan along with 145p purchases.</span></span>

- <span data-ttu-id="4babe-119">파트너는 Azure (145p)의 요금을 포함 하는 하나의 송장 PDF 및 조정 파일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-119">Partner will get one invoice PDF and a reconciliation file covering the charges for Azure (145p).</span></span> 

- <span data-ttu-id="4babe-120">파트너는 Azure RI, Marketplace, Azure 요금제에 대 한 요금을 포함 하는 또 다른 청구서 PDF 및 조정 파일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-120">Partner will receive another invoice PDF and a reconciliation file covering their charges for Azure RI, Marketplace, Azure plan.</span></span> 

<span data-ttu-id="4babe-121">**시나리오 3 [다중 통화]**: 파트너는 eur의 145p 구매와 함께 DKK의 azure RI 및 Eur의 azure 계획에 대 한 구매를 가집니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-121">**Scenario 3 [Multi-Currency]**: Partner has purchases for Azure RI in DKK and Azure plan in EUR along with 145p purchases in EUR.</span></span>

- <span data-ttu-id="4babe-122">파트너는 DKK의 Azure RI에 대 한 요금을 포함 하는 하나의 송장 PDF 및 조정 파일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-122">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure RI in DKK.</span></span> 

- <span data-ttu-id="4babe-123">파트너는 EUR의 Azure 요금제에 대 한 요금을 포함 하는 하나의 송장 PDF 및 조정 파일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-123">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure plan in EUR.</span></span> 

- <span data-ttu-id="4babe-124">파트너는 EUR (또는 파트너 청구 통화)의 145p 제품에 대 한 요금을 포함 하는 또 다른 청구서 PDF 및 조정 파일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-124">Partner will receive another invoice PDF and a reconciliation file covering their charges for 145p offer in EUR (or partner billing currency).</span></span> 

## <a name="find-your-bill"></a><span data-ttu-id="4babe-125">청구서 찾기</span><span class="sxs-lookup"><span data-stu-id="4babe-125">Find your bill</span></span> 

<span data-ttu-id="4babe-126">파트너 센터에서 대시보드의 청구 페이지에서 송장을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-126">You can find your invoice on the Billing page of the dashboard in Partner Center.</span></span> <span data-ttu-id="4babe-127">또한이 페이지에서 청구 내역, 지출 추세 및 조정 파일을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-127">You can also find your billing history, spending trends, and reconciliation files on this page.</span></span> 

1. <span data-ttu-id="4babe-128">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-128">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span> 

2. <span data-ttu-id="4babe-129">왼쪽 메뉴에서 **청구**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-129">In the left-hand menu, select **Billing**.</span></span> 

3. <span data-ttu-id="4babe-130">청구 페이지에서 다운로드 하려는 송장을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-130">On the Billing page, select the invoice you want to download.</span></span> 

<span data-ttu-id="4babe-131">마지막 청구서 날짜의 계정 잔액에서 페이지 맨 위에 있는 최신 청구서에 대 한 링크를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-131">You can find a link to your latest invoice at the top of the page under Account balance as of last invoice date.</span></span> 

<span data-ttu-id="4babe-132">청구 내역 섹션에서 이전 송장을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-132">You can find previous invoices in the Billing history section.</span></span> <span data-ttu-id="4babe-133">적절 한 연도를 선택 하 고 적절 한 청구 기간 옆에 있는 드롭다운 화살표를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-133">Choose the appropriate year, then select the drop-down arrow next to the appropriate Billing period.</span></span> <span data-ttu-id="4babe-134">청구서 (.pdf) 옆의 링크를 선택 하 여 해당 기간의 송장을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-134">Select the link next to Invoices (.pdf) to download that period's invoice.</span></span> 

## <a name="understanding-invoice-pdf"></a><span data-ttu-id="4babe-135">송장 PDF 이해</span><span class="sxs-lookup"><span data-stu-id="4babe-135">Understanding invoice PDF</span></span> 

<span data-ttu-id="4babe-136">**사용량 및 라이선스 기반 요금 청구서**: Office 365 및 Azure와 같은 서비스에 대 한 요금 청구서는 선택한 청구 날짜의 2 일 (UTC) 이내에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-136">**Invoices for Usage and license-based charges**: Invoices for charges for services such as Office 365 and Azure will be available within two (2) days of your selected billing date [UTC].</span></span>  

<span data-ttu-id="4babe-137">**Onetime 및 반복 요금 청구서**: azure RI, azure 요금제, Marketplace와 같은 서비스에 대 한 요금 청구서는 매월 8 일 이후에는 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-137">**Invoices for onetime and recurring charges**: Invoices for charges for services such as Azure RI, Azure plan, Marketplace will be available not later than 8th of every month.</span></span>  

<span data-ttu-id="4babe-138">다음은 청구서 PDF 문서에 있는 몇 가지 주요 필드입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-138">Below are some of the key fields on the Invoice PDF document –</span></span>

<span data-ttu-id="4babe-139">**청구서 번호**: 각 청구 기간에 대해 생성 된 청구서 문서에 대 한 고유 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-139">**Invoice number**: Unique identifier for the invoice document generated for the respective billing period.</span></span> 

<span data-ttu-id="4babe-140">**청구 기간**: 사용 및 라이선스 기반 서비스를 사용 하는 기간입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-140">**Billing period**: This is the period during which you have usages and license-based services.</span></span> 

<span data-ttu-id="4babe-141">**청구서 날짜**: 청구서가 매월 생성 되는 청구 날짜 또는 기념일입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-141">**Invoice date**: The billing date or anniversary date on which your invoice is generated each month.</span></span> 

<span data-ttu-id="4babe-142">**지불 기한**: 지불을 받아야 하는 날짜입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-142">**Payment due date**: The date by which your payment must be received.</span></span> 

<span data-ttu-id="4babe-143">**요금**: 각 청구 기간에 대 한 청구 통화로 인 한 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-143">**Charges**: The amount due in your billing currency for the respective billing period.</span></span> 

<span data-ttu-id="4babe-144">**크레딧**: 크레딧 (예: SLA) 또는 구독에 대 한 변경 내용 조정 (예: 사용자의 늘어나거나 감소).</span><span class="sxs-lookup"><span data-stu-id="4babe-144">**Credits**: Credits (such as SLA) or adjustments for changes made to subscriptions (for example, seat increases or decreases).</span></span> 

<span data-ttu-id="4babe-145">**지불 지침**: 지역을 기준으로 청구서를 지불 하는 방법에 대 한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-145">**Payment instructions**: Description of how to pay your invoice, based on your region.</span></span> <span data-ttu-id="4babe-146">지불 시 청구서 번호를 반드시 포함 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-146">Always be sure to include your invoice number when making a payment.</span></span> 

<span data-ttu-id="4babe-147">청구서 파일 (일회성 요금에 대 한 필드 포함)의 모든 필드에 대 한 자세한 설명은 [청구서 파일 필드](invoice-file.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="4babe-147">For a detailed description of all the fields in your invoice file (including fields for one-time charges), see [Invoice file fields](invoice-file.md).</span></span> 

## <a name="understand-reconciliation-files"></a><span data-ttu-id="4babe-148">조정 파일 이해</span><span class="sxs-lookup"><span data-stu-id="4babe-148">Understand reconciliation files</span></span>

 <span data-ttu-id="4babe-149">요금 드릴 다운/항목별 세부 정보를 제공 하는 조정 파일은 청구서 PDF와 함께 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-149">Reconciliation files, which provides a drill down/itemized details of your charges, are available to download along with the Invoice PDF.</span></span> <span data-ttu-id="4babe-150">조정 파일에는 고객 청구서를 만드는 데 사용할 수 있는 고객 식별자 및 구독 식별자가 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4babe-150">The reconciliation files include customer identifiers and subscription identifiers that you can use to create customer invoices.</span></span> <span data-ttu-id="4babe-151">정찰 파일에 대 한 자세한 내용을 보려면  [조정 파일을 사용 하는 방법](use-the-reconciliation-files.md) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="4babe-151">Please refer to  [How to use the reconciliation files](use-the-reconciliation-files.md) to get more details on the recon files.</span></span> 
