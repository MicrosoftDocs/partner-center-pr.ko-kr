---
title: 조정 파일 요금 유형
ms.topic: article
ms.date: 06/05/2020
description: '파트너 센터 조정 파일의 요금 유형 (예: 라이선스 기반, 사용량 기반 및 일회성), 크레딧 및 할인을 검색 합니다.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fdd372ba260254032d0978e6b2f80947d11aa84f
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949304"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="c6396-103">파트너 센터 조정 파일의 다양 한 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="c6396-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="c6396-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="c6396-104">**Applies to**</span></span>

- <span data-ttu-id="c6396-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="c6396-105">Partner Center</span></span>
- <span data-ttu-id="c6396-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="c6396-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="c6396-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="c6396-107">**Appropriate roles**</span></span>

- <span data-ttu-id="c6396-108">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="c6396-108">Admin agent</span></span>
- <span data-ttu-id="c6396-109">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="c6396-109">Billing admin</span></span>
- <span data-ttu-id="c6396-110">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="c6396-110">Global admin</span></span>

<span data-ttu-id="c6396-111">이 항목에서는 청구서 섹션과 조정 파일에 있을 수 있는 관련 요금 유형 간의 매핑에 대해 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="c6396-112">청구서는 요금 요약을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="c6396-113">조정 파일은 요금 유형을 포함 하 여 품목 트랜잭션에 대 한 자세한 분석을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="c6396-114">조정 파일에 대 한 자세한 내용은 [조정 파일을 사용 하는 방법](use-the-reconciliation-files.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c6396-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="c6396-115">[사용 빈도 기반 조정 파일과](usage-based-recon-files.md) [라이선스 기반 조정 파일](license-based-recon-files.md) 은 모두 사용량 관련 트랜잭션과 요금 (사용한 단위 및 관련 요금)만 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="c6396-116">송장에 표시 되는 일회용 크레딧, 할인 또는 **환불 조정 파일** 에 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="c6396-117">청구 요금을 청구서 요금에 매핑</span><span class="sxs-lookup"><span data-stu-id="c6396-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="c6396-118">청구서와 조정 파일 간 요금을 상호 참조 하려면 Microsoft Excel의 필터 옵션을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="c6396-119">조정 파일에서 요금을 기준으로 필터링 하 여 청구서 요금을 조정 파일의 요금 분석 집합에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="c6396-120">라이선스 기반 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-120">License-based charges</span></span>

<span data-ttu-id="c6396-121">이러한 라이선스 기반 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="c6396-122">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="c6396-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c6396-123">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="c6396-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c6396-124">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-124">Activation fee</span></span> | <span data-ttu-id="c6396-125">구매 후 구독을 사용할 때 고객에 게 청구 되는 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="c6396-126">취소 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-126">Cancel fee</span></span> | <span data-ttu-id="c6396-127">연결 된 사용자가 변경 되 면 고객에 게 비례 하는 요금이 환불 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="c6396-128">비례 배분 인스턴스 취소</span><span class="sxs-lookup"><span data-stu-id="c6396-128">Cancel instance prorate</span></span> | <span data-ttu-id="c6396-129">월간 구독을 사용 하는 고객에 게 구독이 일시 중단 되 고 연결 된 사용자가 같은 월 내에 변경 되 면 비례 청구 요금이 취소 됩니다</span><span class="sxs-lookup"><span data-stu-id="c6396-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="c6396-130">요금 주기</span><span class="sxs-lookup"><span data-stu-id="c6396-130">Cycle fee</span></span> | <span data-ttu-id="c6396-131">구독에 대 한 정기 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="c6396-132">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="c6396-132">Cycle instance prorate</span></span> | <span data-ttu-id="c6396-133">관련 된 사용자가 변경 되 면 고객 으로부터 평가 된 비례 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="c6396-134">취소 시 비례 배분 수수료</span><span class="sxs-lookup"><span data-stu-id="c6396-134">Prorate fees when cancel</span></span> | <span data-ttu-id="c6396-135">취소 시 서비스의 사용 되지 않는 부분에 대해 비례 하는 환불</span><span class="sxs-lookup"><span data-stu-id="c6396-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="c6396-136">현재 제품에서 다른 곳으로 전환할 때 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="c6396-137">현재 월간 구독에서 연간 구독으로 전환 된 후에 비례 하는 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="c6396-138">새 제품으로 변환할 때 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="c6396-139">월간 구독을 새 연간 구독으로 변환한 후 요금을 지불 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="c6396-140">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-140">Prorate fees when purchase</span></span> | <span data-ttu-id="c6396-141">연간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="c6396-142">구매 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-142">Purchase fee</span></span> | <span data-ttu-id="c6396-143">월간 청구를 사용 하는 경우 구독에 대 한 요금 청구 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="c6396-144">갱신 시 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-144">Prorate fee when renew</span></span> | <span data-ttu-id="c6396-145">구독 갱신 시 요금을 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="c6396-146">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-146">Renew fee</span></span> | <span data-ttu-id="c6396-147">구독 갱신에 대 한 요금 청구</span><span class="sxs-lookup"><span data-stu-id="c6396-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="c6396-148">활성화 시 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-148">Prorate fees when activate</span></span> | <span data-ttu-id="c6396-149">청구 기간이 끝날 때까지 정품 인증에 대 한 비용을 지불 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-149">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="c6396-150">일회성 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-150">One-time charges</span></span>

<span data-ttu-id="c6396-151">이러한 일회성 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="c6396-152">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="c6396-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c6396-153">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="c6396-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c6396-154">새로 만들기</span><span class="sxs-lookup"><span data-stu-id="c6396-154">New</span></span> | <span data-ttu-id="c6396-155">새 구매가 생성 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="c6396-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="c6396-156">addQuantity</span></span> | <span data-ttu-id="c6396-157">원래 구매 환불 및 증가 후의 새로운 수량 모두에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="c6396-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="c6396-158">removeQuantity</span></span> | <span data-ttu-id="c6396-159">원래 구매 환불 및 감소 후의 새 수량 모두에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="c6396-160">취소</span><span class="sxs-lookup"><span data-stu-id="c6396-160">Cancel</span></span> | <span data-ttu-id="c6396-161">구독이 취소 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-161">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="c6396-162">변환</span><span class="sxs-lookup"><span data-stu-id="c6396-162">Convert</span></span> | <span data-ttu-id="c6396-163">라이선스가 업그레이드 될 때 사용 되지만 사용자의 수는 변경 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="c6396-164">사용 요금</span><span class="sxs-lookup"><span data-stu-id="c6396-164">Usage charges</span></span>

<span data-ttu-id="c6396-165">이러한 사용 요금을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="c6396-166">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="c6396-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c6396-167">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="c6396-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c6396-168">취소 시 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="c6396-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="c6396-169">현재 청구 기간 동안 미지불된 사용량에 대해 취소 시 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="c6396-170">현재 주기에 대 한 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="c6396-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="c6396-171">현재 청구 기간에 대한 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="c6396-172">크레딧</span><span class="sxs-lookup"><span data-stu-id="c6396-172">Credits</span></span>

<span data-ttu-id="c6396-173">이러한 크레딧을 청구서에 매핑하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="c6396-174">라이선스 기반 파일에서 **Totalforcustomer** 의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="c6396-175">사용량 기반 파일에서 **PostTaxTotal** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="c6396-176">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="c6396-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c6396-177">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="c6396-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c6396-178">줄 항목 오프셋</span><span class="sxs-lookup"><span data-stu-id="c6396-178">Offset a line item</span></span> | <span data-ttu-id="c6396-179">세금을 포함하여 품목에 대한 부분 또는 전체 환불액입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="c6396-180">사용량 기반 할인</span><span class="sxs-lookup"><span data-stu-id="c6396-180">Usage-based discounts</span></span>

<span data-ttu-id="c6396-181">이러한 사용량 기반 할인을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="c6396-182">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="c6396-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c6396-183">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="c6396-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c6396-184">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="c6396-184">Activation discount</span></span> | <span data-ttu-id="c6396-185">구독이 활성화 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="c6396-186">주기 할인</span><span class="sxs-lookup"><span data-stu-id="c6396-186">Cycle discount</span></span> | <span data-ttu-id="c6396-187">주기적 요금에 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="c6396-188">할인 갱신</span><span class="sxs-lookup"><span data-stu-id="c6396-188">Renew discount</span></span> | <span data-ttu-id="c6396-189">구독이 갱신 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="c6396-190">할인 취소</span><span class="sxs-lookup"><span data-stu-id="c6396-190">Cancel discount</span></span> | <span data-ttu-id="c6396-191">할인이 취소될 때 적용되는 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-191">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="c6396-192">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="c6396-192">License-based discounts</span></span>

<span data-ttu-id="c6396-193">라이선스 기반 할인을 청구서에 매핑하려면 라이선스 기반 파일에서 **TotalOtherDiscount** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6396-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="c6396-194">*라이선스 기반 할인은 여러 요금 유형에 적용 될 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="c6396-194">*License-based discounts may be applied to multiple charge types.*</span></span>
