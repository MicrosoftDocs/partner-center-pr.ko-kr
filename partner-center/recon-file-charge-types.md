---
title: 조정 파일 요금 유형
ms.topic: article
ms.date: 06/05/2020
description: '파트너 센터 조정 파일의 요금 유형 (예: 라이선스 기반, 사용량 기반 및 일회성), 크레딧 및 할인을 검색 합니다.'
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441602"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="54c8b-103">파트너 센터 조정 파일의 다양 한 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="54c8b-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="54c8b-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="54c8b-104">**Applies to**</span></span>

- <span data-ttu-id="54c8b-105">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="54c8b-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="54c8b-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="54c8b-106">**Appropriate roles**</span></span>

- <span data-ttu-id="54c8b-107">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="54c8b-107">Admin agent</span></span>
- <span data-ttu-id="54c8b-108">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="54c8b-108">Billing admin</span></span>
- <span data-ttu-id="54c8b-109">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="54c8b-109">Global admin</span></span>

<span data-ttu-id="54c8b-110">이 문서에서는 청구서 섹션과 조정 파일에 있을 수 있는 관련 요금 유형 간의 매핑을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="54c8b-111">청구서는 요금 요약을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="54c8b-112">조정 파일은 요금 유형을 포함 하 여 품목 트랜잭션에 대 한 자세한 분석을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="54c8b-113">조정 파일에 대 한 자세한 내용은 [조정 파일을 사용 하는 방법](use-the-reconciliation-files.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="54c8b-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="54c8b-114">[사용 빈도 기반 조정 파일과](usage-based-recon-files.md) [라이선스 기반 조정 파일](license-based-recon-files.md) 은 모두 사용량 관련 트랜잭션과 요금 (사용한 단위 및 관련 요금)만 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="54c8b-115">송장에 표시 되는 일회용 크레딧, 할인 또는 **환불 조정 파일** 에 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="54c8b-116">청구 요금을 청구서 요금에 매핑</span><span class="sxs-lookup"><span data-stu-id="54c8b-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="54c8b-117">청구서와 조정 파일 간 요금을 상호 참조 하려면 Microsoft Excel의 필터 옵션을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="54c8b-118">조정 파일에서 요금을 기준으로 필터링 하 여 청구서 요금을 조정 파일의 요금 분석 집합에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="54c8b-119">라이선스 기반 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-119">License-based charges</span></span>

<span data-ttu-id="54c8b-120">이러한 라이선스 기반 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="54c8b-121">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="54c8b-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="54c8b-122">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="54c8b-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="54c8b-123">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-123">Activation fee</span></span> | <span data-ttu-id="54c8b-124">구매 후 구독을 사용할 때 고객에 게 청구 되는 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="54c8b-125">취소 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-125">Cancel fee</span></span> | <span data-ttu-id="54c8b-126">연결 된 라이선스를 변경 하는 경우 고객에 게 비례 하는 요금이 환불 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="54c8b-127">비례 배분 인스턴스 취소</span><span class="sxs-lookup"><span data-stu-id="54c8b-127">Cancel instance prorate</span></span> | <span data-ttu-id="54c8b-128">월간 구독을 사용 하는 고객에 게 구독이 일시 중단 되 고 연결 된 라이선스가 동일한 월 내에 변경 되 면 비례 청구 요금이 취소 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="54c8b-129">요금 주기</span><span class="sxs-lookup"><span data-stu-id="54c8b-129">Cycle fee</span></span> | <span data-ttu-id="54c8b-130">구독에 대 한 정기 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="54c8b-131">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="54c8b-131">Cycle instance prorate</span></span> | <span data-ttu-id="54c8b-132">연결 된 라이선스를 변경 하는 경우 고객 으로부터 평가 된 비례 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="54c8b-133">취소 시 비례 배분 수수료</span><span class="sxs-lookup"><span data-stu-id="54c8b-133">Prorate fees when cancel</span></span> | <span data-ttu-id="54c8b-134">취소 시 서비스의 사용 되지 않는 부분에 대해 비례 하는 환불</span><span class="sxs-lookup"><span data-stu-id="54c8b-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="54c8b-135">현재 제품에서 다른 곳으로 전환할 때 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="54c8b-136">현재 월간 구독에서 연간 구독으로 전환 된 후에 비례 하는 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="54c8b-137">새 제품으로 변환할 때 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="54c8b-138">월간 구독을 새 연간 구독으로 변환한 후 요금을 지불 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="54c8b-139">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-139">Prorate fees when purchase</span></span> | <span data-ttu-id="54c8b-140">월별 또는 연간 요금 청구를 모두 사용 하는 경우 구독에 대 한 요금 청구 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="54c8b-141">갱신 시 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-141">Prorate fee when renew</span></span> | <span data-ttu-id="54c8b-142">구독 갱신 시 요금을 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="54c8b-143">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-143">Renew fee</span></span> | <span data-ttu-id="54c8b-144">구독 갱신에 대 한 요금 청구</span><span class="sxs-lookup"><span data-stu-id="54c8b-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="54c8b-145">활성화 시 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-145">Prorate fees when activate</span></span> | <span data-ttu-id="54c8b-146">청구 기간이 끝날 때까지 정품 인증에 대 한 비용을 지불 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="54c8b-147">일회성 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-147">One-time charges</span></span>

<span data-ttu-id="54c8b-148">이러한 일회성 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="54c8b-149">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="54c8b-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="54c8b-150">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="54c8b-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="54c8b-151">새로 생성</span><span class="sxs-lookup"><span data-stu-id="54c8b-151">New</span></span> | <span data-ttu-id="54c8b-152">새 구매가 생성 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="54c8b-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="54c8b-153">addQuantity</span></span> | <span data-ttu-id="54c8b-154">원래 구매 환불 및 증가 후의 새로운 수량 모두에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="54c8b-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="54c8b-155">removeQuantity</span></span> | <span data-ttu-id="54c8b-156">원래 구매 환불 및 감소 후의 새 수량 모두에 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="54c8b-157">취소</span><span class="sxs-lookup"><span data-stu-id="54c8b-157">Cancel</span></span> | <span data-ttu-id="54c8b-158">구독이 취소 될 때 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="54c8b-159">변환</span><span class="sxs-lookup"><span data-stu-id="54c8b-159">Convert</span></span> | <span data-ttu-id="54c8b-160">라이선스가 업그레이드 될 때 사용 되지만 라이선스 수는 변경 되지 않은 상태로 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="54c8b-161">사용 요금</span><span class="sxs-lookup"><span data-stu-id="54c8b-161">Usage charges</span></span>

<span data-ttu-id="54c8b-162">이러한 사용 요금을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="54c8b-163">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="54c8b-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="54c8b-164">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="54c8b-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="54c8b-165">취소 시 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="54c8b-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="54c8b-166">현재 청구 기간 동안 미지불된 사용량에 대해 취소 시 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="54c8b-167">현재 주기에 대 한 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="54c8b-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="54c8b-168">현재 청구 기간에 대한 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="54c8b-169">크레딧</span><span class="sxs-lookup"><span data-stu-id="54c8b-169">Credits</span></span>

<span data-ttu-id="54c8b-170">이러한 크레딧을 청구서에 매핑하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="54c8b-171">라이선스 기반 파일에서 **Totalforcustomer** 의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="54c8b-172">사용량 기반 파일에서 **PostTaxTotal** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="54c8b-173">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="54c8b-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="54c8b-174">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="54c8b-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="54c8b-175">줄 항목 오프셋</span><span class="sxs-lookup"><span data-stu-id="54c8b-175">Offset a line item</span></span> | <span data-ttu-id="54c8b-176">세금을 포함하여 품목에 대한 부분 또는 전체 환불액입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="54c8b-177">사용량 기반 할인</span><span class="sxs-lookup"><span data-stu-id="54c8b-177">Usage-based discounts</span></span>

<span data-ttu-id="54c8b-178">이러한 사용량 기반 할인을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="54c8b-179">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="54c8b-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="54c8b-180">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="54c8b-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="54c8b-181">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="54c8b-181">Activation discount</span></span> | <span data-ttu-id="54c8b-182">구독이 활성화 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="54c8b-183">주기 할인</span><span class="sxs-lookup"><span data-stu-id="54c8b-183">Cycle discount</span></span> | <span data-ttu-id="54c8b-184">주기적 요금에 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="54c8b-185">할인 갱신</span><span class="sxs-lookup"><span data-stu-id="54c8b-185">Renew discount</span></span> | <span data-ttu-id="54c8b-186">구독이 갱신 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="54c8b-187">할인 취소</span><span class="sxs-lookup"><span data-stu-id="54c8b-187">Cancel discount</span></span> | <span data-ttu-id="54c8b-188">할인이 취소될 때 적용되는 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="54c8b-189">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="54c8b-189">License-based discounts</span></span>

<span data-ttu-id="54c8b-190">라이선스 기반 할인을 청구서에 매핑하려면 라이선스 기반 파일에서 **TotalOtherDiscount** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="54c8b-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="54c8b-191">*라이선스 기반 할인은 여러 요금 유형에 적용 될 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="54c8b-191">*License-based discounts may be applied to multiple charge types.*</span></span>
