---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389811"
---
# <a name="understand-charge-types"></a><span data-ttu-id="b4a47-103">Understand charge types</span><span class="sxs-lookup"><span data-stu-id="b4a47-103">Understand charge types</span></span>

<span data-ttu-id="b4a47-104">적용 대상:</span><span class="sxs-lookup"><span data-stu-id="b4a47-104">Applies to:</span></span>

- <span data-ttu-id="b4a47-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b4a47-105">Partner Center</span></span>
- <span data-ttu-id="b4a47-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b4a47-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b4a47-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="b4a47-108">Your invoice provides a summary of charges.</span><span class="sxs-lookup"><span data-stu-id="b4a47-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="b4a47-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="b4a47-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="b4a47-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="b4a47-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="b4a47-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span><span class="sxs-lookup"><span data-stu-id="b4a47-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="b4a47-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="b4a47-113">Map charge types to invoice charges</span><span class="sxs-lookup"><span data-stu-id="b4a47-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="b4a47-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="b4a47-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="b4a47-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="b4a47-116">라이선스 기반 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-116">License-based charges</span></span>

<span data-ttu-id="b4a47-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b4a47-118">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="b4a47-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b4a47-119">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="b4a47-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b4a47-120">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-120">Activation fee</span></span> | <span data-ttu-id="b4a47-121">The amount charged to the customer when they use the subscription after purchase.</span><span class="sxs-lookup"><span data-stu-id="b4a47-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="b4a47-122">취소 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-122">Cancel fee</span></span> | <span data-ttu-id="b4a47-123">Prorated charges refunded to the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="b4a47-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="b4a47-124">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="b4a47-124">Cycle fee</span></span> | <span data-ttu-id="b4a47-125">Periodic charges for a subscription.</span><span class="sxs-lookup"><span data-stu-id="b4a47-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="b4a47-126">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="b4a47-126">Cycle instance prorate</span></span> | <span data-ttu-id="b4a47-127">Prorated charges assessed from the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="b4a47-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="b4a47-128">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-128">Prorate fees when cancel</span></span> | <span data-ttu-id="b4a47-129">Prorated refund for unused portion of service upon cancellation.</span><span class="sxs-lookup"><span data-stu-id="b4a47-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="b4a47-130">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-130">Prorate fees when purchase</span></span> | <span data-ttu-id="b4a47-131">The charge type for a subscription when using annual billing.</span><span class="sxs-lookup"><span data-stu-id="b4a47-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="b4a47-132">구매 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-132">Purchase fee</span></span> | <span data-ttu-id="b4a47-133">The charge type for a subscription when using monthly billing.</span><span class="sxs-lookup"><span data-stu-id="b4a47-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="b4a47-134">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-134">Prorate fee when renew</span></span> | <span data-ttu-id="b4a47-135">Prorated fees upon subscription renewal.</span><span class="sxs-lookup"><span data-stu-id="b4a47-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="b4a47-136">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-136">Renew fee</span></span> | <span data-ttu-id="b4a47-137">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="b4a47-138">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-138">Prorate fees when activate</span></span> | <span data-ttu-id="b4a47-139">>Prorated fees from activation until end of billing period.</span><span class="sxs-lookup"><span data-stu-id="b4a47-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="b4a47-140">One-time charges</span><span class="sxs-lookup"><span data-stu-id="b4a47-140">One-time charges</span></span>

<span data-ttu-id="b4a47-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b4a47-142">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="b4a47-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b4a47-143">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="b4a47-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b4a47-144">신규 항목</span><span class="sxs-lookup"><span data-stu-id="b4a47-144">New</span></span> | <span data-ttu-id="b4a47-145">Used when a new purchase is created.</span><span class="sxs-lookup"><span data-stu-id="b4a47-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="b4a47-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b4a47-146">addQuantity</span></span> | <span data-ttu-id="b4a47-147">Used in both the refund of the original purchase and the new quantity after an increase.</span><span class="sxs-lookup"><span data-stu-id="b4a47-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="b4a47-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b4a47-148">removeQuantity</span></span> | <span data-ttu-id="b4a47-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span><span class="sxs-lookup"><span data-stu-id="b4a47-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="b4a47-150">취소</span><span class="sxs-lookup"><span data-stu-id="b4a47-150">Cancel</span></span> | <span data-ttu-id="b4a47-151">Used when a subscription is cancelled.</span><span class="sxs-lookup"><span data-stu-id="b4a47-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="b4a47-152">변환</span><span class="sxs-lookup"><span data-stu-id="b4a47-152">Convert</span></span> | <span data-ttu-id="b4a47-153">Used when a license is upgraded but the number of seats remains unchanged.</span><span class="sxs-lookup"><span data-stu-id="b4a47-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="b4a47-154">사용 요금</span><span class="sxs-lookup"><span data-stu-id="b4a47-154">Usage charges</span></span>

<span data-ttu-id="b4a47-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b4a47-156">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="b4a47-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b4a47-157">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="b4a47-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b4a47-158">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="b4a47-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="b4a47-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span><span class="sxs-lookup"><span data-stu-id="b4a47-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="b4a47-160">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="b4a47-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="b4a47-161">Access usage fee for the current billing period.</span><span class="sxs-lookup"><span data-stu-id="b4a47-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="b4a47-162">크레딧</span><span class="sxs-lookup"><span data-stu-id="b4a47-162">Credits</span></span>

<span data-ttu-id="b4a47-163">To map these credits to your invoice:</span><span class="sxs-lookup"><span data-stu-id="b4a47-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="b4a47-164">Sum the **TotalForCustomer** from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="b4a47-165">Sum the **PostTaxTotal** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="b4a47-166">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="b4a47-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b4a47-167">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="b4a47-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b4a47-168">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="b4a47-168">Offset a line item</span></span> | <span data-ttu-id="b4a47-169">Partial or whole refund to a line item, including taxes.</span><span class="sxs-lookup"><span data-stu-id="b4a47-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="b4a47-170">사용량 기반 할인</span><span class="sxs-lookup"><span data-stu-id="b4a47-170">Usage-based discounts</span></span>

<span data-ttu-id="b4a47-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b4a47-172">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="b4a47-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b4a47-173">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="b4a47-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b4a47-174">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="b4a47-174">Activation discount</span></span> | <span data-ttu-id="b4a47-175">Discount applied when subscription activated.</span><span class="sxs-lookup"><span data-stu-id="b4a47-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="b4a47-176">주기 할인</span><span class="sxs-lookup"><span data-stu-id="b4a47-176">Cycle discount</span></span> | <span data-ttu-id="b4a47-177">Discount applied on periodic charges.</span><span class="sxs-lookup"><span data-stu-id="b4a47-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="b4a47-178">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="b4a47-178">Renew discount</span></span> | <span data-ttu-id="b4a47-179">Discount applied when subscription renewed.</span><span class="sxs-lookup"><span data-stu-id="b4a47-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="b4a47-180">취소 할인</span><span class="sxs-lookup"><span data-stu-id="b4a47-180">Cancel discount</span></span> | <span data-ttu-id="b4a47-181">Charges applied when discounts cancelled.</span><span class="sxs-lookup"><span data-stu-id="b4a47-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="b4a47-182">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="b4a47-182">License-based discounts</span></span>

<span data-ttu-id="b4a47-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="b4a47-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="b4a47-184">*License-based discounts may be applied to multiple charge types.*</span><span class="sxs-lookup"><span data-stu-id="b4a47-184">*License-based discounts may be applied to multiple charge types.*</span></span>
