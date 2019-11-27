---
title: 조정 파일 요금 유형 | 파트너 센터
ms.topic: article
ms.date: 08/26/2019
description: 파트너 센터 조정 파일의 요금 유형 (라이선스 기반, 사용량 기반 및 일회성), 크레딧 및 할인.
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
# <a name="understand-charge-types"></a><span data-ttu-id="81b1e-103">요금 청구 유형 이해</span><span class="sxs-lookup"><span data-stu-id="81b1e-103">Understand charge types</span></span>

<span data-ttu-id="81b1e-104">적용 대상:</span><span class="sxs-lookup"><span data-stu-id="81b1e-104">Applies to:</span></span>

- <span data-ttu-id="81b1e-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="81b1e-105">Partner Center</span></span>
- <span data-ttu-id="81b1e-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="81b1e-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="81b1e-107">이 항목에서는 청구서 섹션과 조정 파일에 있을 수 있는 관련 요금 유형 간의 매핑에 대해 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="81b1e-108">청구서는 요금 요약을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="81b1e-109">조정 파일은 요금 유형을 포함 하 여 품목 트랜잭션에 대 한 자세한 분석을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="81b1e-110">조정 파일에 대 한 자세한 내용은 [조정 파일을 사용 하는 방법](use-the-reconciliation-files.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="81b1e-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="81b1e-111">[사용 빈도 기반 조정 파일과](usage-based-recon-files.md) [라이선스 기반 조정 파일](license-based-recon-files.md) 은 모두 사용량 관련 트랜잭션과 요금 (사용한 단위 및 관련 요금)만 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="81b1e-112">송장에 표시 되는 일회용 크레딧, 할인 또는 **환불 조정 파일** 에 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="81b1e-113">청구 요금을 청구서 요금에 매핑</span><span class="sxs-lookup"><span data-stu-id="81b1e-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="81b1e-114">청구서와 조정 파일 간 요금을 상호 참조 하려면 Microsoft Excel의 필터 옵션을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="81b1e-115">조정 파일에서 요금을 기준으로 필터링 하 여 청구서 요금을 조정 파일의 요금 분석 집합에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="81b1e-116">라이선스 기반 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-116">License-based charges</span></span>

<span data-ttu-id="81b1e-117">이러한 라이선스 기반 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="81b1e-118">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="81b1e-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="81b1e-119">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="81b1e-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="81b1e-120">활성화 수수료</span><span class="sxs-lookup"><span data-stu-id="81b1e-120">Activation fee</span></span> | <span data-ttu-id="81b1e-121">구매 후 구독을 사용할 때 고객에 게 청구 되는 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="81b1e-122">취소 수수료</span><span class="sxs-lookup"><span data-stu-id="81b1e-122">Cancel fee</span></span> | <span data-ttu-id="81b1e-123">연결 된 사용자가 변경 되 면 고객에 게 비례 하는 요금이 환불 됩니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="81b1e-124">주기 수수료</span><span class="sxs-lookup"><span data-stu-id="81b1e-124">Cycle fee</span></span> | <span data-ttu-id="81b1e-125">구독에 대 한 정기 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="81b1e-126">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="81b1e-126">Cycle instance prorate</span></span> | <span data-ttu-id="81b1e-127">관련 된 사용자가 변경 되 면 고객 으로부터 평가 된 비례 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="81b1e-128">취소 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-128">Prorate fees when cancel</span></span> | <span data-ttu-id="81b1e-129">취소 시 서비스의 사용 되지 않는 부분에 대해 비례 하는 환불</span><span class="sxs-lookup"><span data-stu-id="81b1e-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="81b1e-130">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-130">Prorate fees when purchase</span></span> | <span data-ttu-id="81b1e-131">연간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="81b1e-132">구매 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-132">Purchase fee</span></span> | <span data-ttu-id="81b1e-133">월간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="81b1e-134">갱신 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-134">Prorate fee when renew</span></span> | <span data-ttu-id="81b1e-135">구독 갱신 시 요금을 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="81b1e-136">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-136">Renew fee</span></span> | <span data-ttu-id="81b1e-137">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="81b1e-138">활성화 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-138">Prorate fees when activate</span></span> | <span data-ttu-id="81b1e-139">청구 기간이 끝날 때까지 정품 인증에 대 한 > 비례 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="81b1e-140">일회성 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-140">One-time charges</span></span>

<span data-ttu-id="81b1e-141">이러한 일회성 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="81b1e-142">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="81b1e-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="81b1e-143">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="81b1e-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="81b1e-144">단추를 사용하여 새</span><span class="sxs-lookup"><span data-stu-id="81b1e-144">New</span></span> | <span data-ttu-id="81b1e-145">새 구매가 생성 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="81b1e-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="81b1e-146">addQuantity</span></span> | <span data-ttu-id="81b1e-147">원래 구매 환불 및 증가 후의 새로운 수량 모두에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="81b1e-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="81b1e-148">removeQuantity</span></span> | <span data-ttu-id="81b1e-149">원래 구매 환불 및 감소 후의 새 수량 모두에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="81b1e-150">취소</span><span class="sxs-lookup"><span data-stu-id="81b1e-150">Cancel</span></span> | <span data-ttu-id="81b1e-151">구독이 취소 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="81b1e-152">변환</span><span class="sxs-lookup"><span data-stu-id="81b1e-152">Convert</span></span> | <span data-ttu-id="81b1e-153">라이선스가 업그레이드 될 때 사용 되지만 사용자의 수는 변경 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="81b1e-154">사용 요금</span><span class="sxs-lookup"><span data-stu-id="81b1e-154">Usage charges</span></span>

<span data-ttu-id="81b1e-155">이러한 사용 요금을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="81b1e-156">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="81b1e-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="81b1e-157">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="81b1e-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="81b1e-158">취소 시 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="81b1e-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="81b1e-159">현재 청구 기간 동안 미지불 사용 취소 시 사용 요금에 액세스 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="81b1e-160">현재 주기의 사용 요금 계산</span><span class="sxs-lookup"><span data-stu-id="81b1e-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="81b1e-161">현재 청구 기간에 대 한 사용 요금에 액세스 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="81b1e-162">크레딧</span><span class="sxs-lookup"><span data-stu-id="81b1e-162">Credits</span></span>

<span data-ttu-id="81b1e-163">이러한 크레딧을 청구서에 매핑하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="81b1e-164">라이선스 기반 파일에서 **Totalforcustomer** 의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="81b1e-165">사용량 기반 파일에서 **PostTaxTotal** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="81b1e-166">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="81b1e-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="81b1e-167">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="81b1e-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="81b1e-168">품목 오프셋</span><span class="sxs-lookup"><span data-stu-id="81b1e-168">Offset a line item</span></span> | <span data-ttu-id="81b1e-169">세금을 포함 하 여 품목을 부분적으로 또는 전체적으로 환불 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="81b1e-170">사용량 기반 할인</span><span class="sxs-lookup"><span data-stu-id="81b1e-170">Usage-based discounts</span></span>

<span data-ttu-id="81b1e-171">이러한 사용량 기반 할인을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="81b1e-172">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="81b1e-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="81b1e-173">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="81b1e-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="81b1e-174">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="81b1e-174">Activation discount</span></span> | <span data-ttu-id="81b1e-175">구독이 활성화 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="81b1e-176">주기 할인</span><span class="sxs-lookup"><span data-stu-id="81b1e-176">Cycle discount</span></span> | <span data-ttu-id="81b1e-177">정기 요금에 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="81b1e-178">갱신 할인</span><span class="sxs-lookup"><span data-stu-id="81b1e-178">Renew discount</span></span> | <span data-ttu-id="81b1e-179">구독이 갱신 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="81b1e-180">취소 할인</span><span class="sxs-lookup"><span data-stu-id="81b1e-180">Cancel discount</span></span> | <span data-ttu-id="81b1e-181">할인이 취소 된 경우 적용 되는 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="81b1e-182">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="81b1e-182">License-based discounts</span></span>

<span data-ttu-id="81b1e-183">라이선스 기반 할인을 청구서에 매핑하려면 라이선스 기반 파일에서 **TotalOtherDiscount** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="81b1e-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="81b1e-184">*라이선스 기반 할인은 여러 요금 유형에 적용 될 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="81b1e-184">*License-based discounts may be applied to multiple charge types.*</span></span>
