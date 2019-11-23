---
title: Use your reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Use your reconciliation files to understand detailed line-item views of Partner Center charges.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384800"
---
# <a name="use-your-reconciliation-files"></a><span data-ttu-id="99386-103">Use your reconciliation files</span><span class="sxs-lookup"><span data-stu-id="99386-103">Use your reconciliation files</span></span>

<span data-ttu-id="99386-104">적용 대상:</span><span class="sxs-lookup"><span data-stu-id="99386-104">Applies to:</span></span>

- <span data-ttu-id="99386-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="99386-105">Partner Center</span></span>
- <span data-ttu-id="99386-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="99386-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="99386-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span><span class="sxs-lookup"><span data-stu-id="99386-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="99386-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span><span class="sxs-lookup"><span data-stu-id="99386-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="99386-109">Appropriate roles:</span><span class="sxs-lookup"><span data-stu-id="99386-109">Appropriate roles:</span></span>

- <span data-ttu-id="99386-110">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="99386-110">Billing admin</span></span>
- <span data-ttu-id="99386-111">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="99386-111">Global admin</span></span>

<span data-ttu-id="99386-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="99386-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="99386-113">Understand reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="99386-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="99386-114">License-based reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="99386-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="99386-115">Usage-based reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="99386-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="99386-116">One-time and recurring reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="99386-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="99386-117">Daily-rated usage reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="99386-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="99386-118">Understand charge types in reconciliation files</span><span class="sxs-lookup"><span data-stu-id="99386-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="99386-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="99386-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="99386-120">Fix formatting issues</span><span class="sxs-lookup"><span data-stu-id="99386-120">Fix formatting issues</span></span>

<span data-ttu-id="99386-121">Occasionally, a reconciliation file might contain formatting issues.</span><span class="sxs-lookup"><span data-stu-id="99386-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="99386-122">For example, this issue might occur if the en-US locale is not used.</span><span class="sxs-lookup"><span data-stu-id="99386-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="99386-123">Follow these steps for fix any formatting issues in your reconciliation files:</span><span class="sxs-lookup"><span data-stu-id="99386-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="99386-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="99386-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="99386-125">Select the first column in the file.</span><span class="sxs-lookup"><span data-stu-id="99386-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="99386-126">Open the **Convert Text to Columns Wizard**.</span><span class="sxs-lookup"><span data-stu-id="99386-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="99386-127">On the ribbon, select **Data**, then select **Text to Columns**.</span><span class="sxs-lookup"><span data-stu-id="99386-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="99386-128">In the wizard, select **Delimited file type**.</span><span class="sxs-lookup"><span data-stu-id="99386-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="99386-129">Then, select **Next**.</span><span class="sxs-lookup"><span data-stu-id="99386-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="99386-130">In the **Delimiters** field, select **Comma**.</span><span class="sxs-lookup"><span data-stu-id="99386-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="99386-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span><span class="sxs-lookup"><span data-stu-id="99386-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="99386-132">In the **Column data format** field, select **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="99386-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="99386-133">Then, select **Next**.</span><span class="sxs-lookup"><span data-stu-id="99386-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="99386-134">In the **Column data format** field, select **Text** for all amount columns.</span><span class="sxs-lookup"><span data-stu-id="99386-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="99386-135">Then, select **Finish**.</span><span class="sxs-lookup"><span data-stu-id="99386-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="99386-136">Download reconciliation files programmatically</span><span class="sxs-lookup"><span data-stu-id="99386-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="99386-137">Reconciliation files can be very large and are sometimes difficult to download.</span><span class="sxs-lookup"><span data-stu-id="99386-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="99386-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="99386-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="99386-139">Map taxes or VAT</span><span class="sxs-lookup"><span data-stu-id="99386-139">Map taxes or VAT</span></span>

<span data-ttu-id="99386-140">To map Taxes or value-added tax (VAT) to your invoice:</span><span class="sxs-lookup"><span data-stu-id="99386-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="99386-141">Sum the **Tax** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="99386-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="99386-142">Sum the **TaxAmount** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="99386-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="99386-143">Itemize reconciliation files by partner</span><span class="sxs-lookup"><span data-stu-id="99386-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="99386-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span><span class="sxs-lookup"><span data-stu-id="99386-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="99386-145">MPN ID</span><span class="sxs-lookup"><span data-stu-id="99386-145">MPN ID</span></span> | <span data-ttu-id="99386-146">설명</span><span class="sxs-lookup"><span data-stu-id="99386-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="99386-147">MPN ID</span><span class="sxs-lookup"><span data-stu-id="99386-147">MPN ID</span></span> | <span data-ttu-id="99386-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span><span class="sxs-lookup"><span data-stu-id="99386-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="99386-149">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="99386-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="99386-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="99386-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="99386-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="99386-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="99386-152">간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="99386-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="99386-153">재판매인 MPN ID</span><span class="sxs-lookup"><span data-stu-id="99386-153">Reseller MPN ID</span></span>

<span data-ttu-id="99386-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span><span class="sxs-lookup"><span data-stu-id="99386-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="99386-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span><span class="sxs-lookup"><span data-stu-id="99386-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="99386-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span><span class="sxs-lookup"><span data-stu-id="99386-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="99386-157">To view or update the **Reseller MPN ID**:</span><span class="sxs-lookup"><span data-stu-id="99386-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="99386-158">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="99386-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="99386-159">파트너 센터 메뉴에서 **고객**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="99386-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="99386-160">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="99386-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="99386-161">In the customer menu, select **Subscriptions**.</span><span class="sxs-lookup"><span data-stu-id="99386-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="99386-162">Choose the subscription from the list.</span><span class="sxs-lookup"><span data-stu-id="99386-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="99386-163">**업데이트**를 선택하여 **재판매인(MPN ID)** 을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="99386-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
