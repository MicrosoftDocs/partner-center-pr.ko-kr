---
title: 조정 파일 요금 유형
ms.topic: article
ms.date: 06/05/2020
description: '파트너 센터 조정 파일에서 요금 유형(예: 라이선스 기반, 사용량 기반 및 일회성), 크레딧 및 할인을 검색합니다.'
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855882"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="caddd-103">파트너 센터 조정 파일의 다양한 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="caddd-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="caddd-104">**적용된 내용:** 파트너 센터 | Microsoft Cloud for US Government 대한 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="caddd-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="caddd-105">**적절한 역할:** 관리 에이전트 | 청구 관리자 | 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="caddd-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="caddd-106">이 문서에서는 청구서 섹션과 조정 파일에 있을 수 있는 관련 요금 유형 간의 매핑을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="caddd-107">청구서는 요금 요약을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="caddd-108">조정 파일은 요금 유형을 포함하여 품목 트랜잭션에 대한 자세한 분석을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="caddd-109">조정 파일에 대한 자세한 내용은 [조정 파일 사용 방법을 참조하세요.](use-the-reconciliation-files.md)</span><span class="sxs-lookup"><span data-stu-id="caddd-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="caddd-110">[사용량 기반 조정 파일과](usage-based-recon-files.md) [라이선스 기반 조정 파일은](license-based-recon-files.md) 모두 사용량 관련 트랜잭션 및 요금(소비 단위 및 관련 요금)만 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="caddd-111">조정으로 청구서에 표시되는 일회성 크레딧, 할인 또는 **환불은** 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="caddd-112">요금 유형을 청구서 요금에 매핑</span><span class="sxs-lookup"><span data-stu-id="caddd-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="caddd-113">청구서와 조정 파일 간의 요금 금액을 상호 참조하려면 Microsoft Excel의 필터 옵션을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="caddd-114">조정 파일의 요금 유형을 기준으로 필터링하여 청구서 요금을 조정 파일의 요금 분석 세트에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="caddd-115">라이선스 기반 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-115">License-based charges</span></span>

<span data-ttu-id="caddd-116">이러한 라이선스 기반 요금을 청구서에 매핑하려면 라이선스 기반 파일에서 **Amount** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="caddd-117">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="caddd-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="caddd-118">요금 설명</span><span class="sxs-lookup"><span data-stu-id="caddd-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="caddd-119">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-119">Activation fee</span></span> | <span data-ttu-id="caddd-120">구매 후 구독을 사용할 때 고객에게 청구되는 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="caddd-121">취소 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-121">Cancel fee</span></span> | <span data-ttu-id="caddd-122">관련 라이선스가 변경될 때 고객에게 비례 배분된 요금이 환불됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="caddd-123">인스턴스 배분 취소</span><span class="sxs-lookup"><span data-stu-id="caddd-123">Cancel instance prorate</span></span> | <span data-ttu-id="caddd-124">월간 구독을 사용 하는 고객에 게 구독이 일시 중단 되 고 연결 된 라이선스가 동일한 월 내에 변경 되 면 비례 청구 요금이 취소 됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="caddd-125">요금 주기</span><span class="sxs-lookup"><span data-stu-id="caddd-125">Cycle fee</span></span> | <span data-ttu-id="caddd-126">구독에 대 한 정기 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="caddd-127">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="caddd-127">Cycle instance prorate</span></span> | <span data-ttu-id="caddd-128">연결 된 라이선스를 변경 하는 경우 고객 으로부터 평가 된 비례 청구 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="caddd-129">취소 시 비례 배분 수수료</span><span class="sxs-lookup"><span data-stu-id="caddd-129">Prorate fees when cancel</span></span> | <span data-ttu-id="caddd-130">취소 시 서비스의 사용 되지 않는 부분에 대해 비례 하는 환불</span><span class="sxs-lookup"><span data-stu-id="caddd-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="caddd-131">현재 제품에서 다른 곳으로 전환할 때 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="caddd-132">현재 월간 구독에서 연간 구독으로 전환 된 후에 비례 하는 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="caddd-133">새 제품으로 변환할 때 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="caddd-134">월간 구독을 새 연간 구독으로 변환한 후 요금을 지불 합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="caddd-135">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-135">Prorate fees when purchase</span></span> | <span data-ttu-id="caddd-136">월별 또는 연간 요금 청구를 모두 사용 하는 경우 구독에 대 한 요금 청구 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="caddd-137">갱신 시 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-137">Prorate fee when renew</span></span> | <span data-ttu-id="caddd-138">구독 갱신 시 요금을 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="caddd-139">갱신 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-139">Renew fee</span></span> | <span data-ttu-id="caddd-140">구독 갱신에 대 한 요금 청구</span><span class="sxs-lookup"><span data-stu-id="caddd-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="caddd-141">활성화 시 비례 배분 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-141">Prorate fees when activate</span></span> | <span data-ttu-id="caddd-142">청구 기간이 끝날 때까지 정품 인증에 대 한 비용을 지불 합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="caddd-143">일회성 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-143">One-time charges</span></span>

<span data-ttu-id="caddd-144">이러한 일회성 요금을 청구서에 매핑하려면 라이선스 기반 파일의 **Amount** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="caddd-145">요금 설명 (조정 파일의 Chargetcharcolumn)</span><span class="sxs-lookup"><span data-stu-id="caddd-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="caddd-146">요금 설명</span><span class="sxs-lookup"><span data-stu-id="caddd-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="caddd-147">신규</span><span class="sxs-lookup"><span data-stu-id="caddd-147">New</span></span> | <span data-ttu-id="caddd-148">새 구매를 만들 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="caddd-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="caddd-149">addQuantity</span></span> | <span data-ttu-id="caddd-150">원래 구매의 환불과 증가 후 새 수량 모두에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="caddd-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="caddd-151">removeQuantity</span></span> | <span data-ttu-id="caddd-152">원래 구매의 환불과 감소 후 새 수량 모두에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="caddd-153">취소</span><span class="sxs-lookup"><span data-stu-id="caddd-153">Cancel</span></span> | <span data-ttu-id="caddd-154">구독이 취소될 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="caddd-155">변환</span><span class="sxs-lookup"><span data-stu-id="caddd-155">Convert</span></span> | <span data-ttu-id="caddd-156">라이선스가 업그레이드되었지만 라이선스 수가 변경되지 않은 상태로 유지되는 경우 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="caddd-157">사용 요금</span><span class="sxs-lookup"><span data-stu-id="caddd-157">Usage charges</span></span>

<span data-ttu-id="caddd-158">이러한 사용 요금을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="caddd-159">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="caddd-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="caddd-160">요금 설명</span><span class="sxs-lookup"><span data-stu-id="caddd-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="caddd-161">취소 시 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="caddd-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="caddd-162">현재 청구 기간 동안 미지불된 사용량에 대해 취소 시 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="caddd-163">현재 주기에 대한 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="caddd-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="caddd-164">현재 청구 기간에 대한 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="caddd-165">크레딧</span><span class="sxs-lookup"><span data-stu-id="caddd-165">Credits</span></span>

<span data-ttu-id="caddd-166">이러한 크레딧을 청구서에 매핑하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="caddd-167">라이선스 기반 파일에서 **TotalForCustomer의** 합계를 구합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="caddd-168">사용량 기반 파일에서 **PostTaxTotal** 열의 합계를 구합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="caddd-169">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="caddd-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="caddd-170">요금 설명</span><span class="sxs-lookup"><span data-stu-id="caddd-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="caddd-171">줄 항목 오프셋</span><span class="sxs-lookup"><span data-stu-id="caddd-171">Offset a line item</span></span> | <span data-ttu-id="caddd-172">세금을 포함하여 품목에 대한 부분 또는 전체 환불액입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="caddd-173">사용량 기반 할인</span><span class="sxs-lookup"><span data-stu-id="caddd-173">Usage-based discounts</span></span>

<span data-ttu-id="caddd-174">이러한 사용량 기반 할인을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="caddd-175">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="caddd-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="caddd-176">요금 청구 설명</span><span class="sxs-lookup"><span data-stu-id="caddd-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="caddd-177">활성화 할인</span><span class="sxs-lookup"><span data-stu-id="caddd-177">Activation discount</span></span> | <span data-ttu-id="caddd-178">구독이 활성화 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="caddd-179">주기 할인</span><span class="sxs-lookup"><span data-stu-id="caddd-179">Cycle discount</span></span> | <span data-ttu-id="caddd-180">주기적 요금에 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="caddd-181">할인 갱신</span><span class="sxs-lookup"><span data-stu-id="caddd-181">Renew discount</span></span> | <span data-ttu-id="caddd-182">구독이 갱신 될 때 적용 되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="caddd-183">할인 취소</span><span class="sxs-lookup"><span data-stu-id="caddd-183">Cancel discount</span></span> | <span data-ttu-id="caddd-184">할인이 취소될 때 적용되는 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="caddd-185">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="caddd-185">License-based discounts</span></span>

<span data-ttu-id="caddd-186">라이선스 기반 할인을 청구서에 매핑하려면 라이선스 기반 파일에서 **TotalOtherDiscount** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="caddd-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="caddd-187">*라이선스 기반 할인은 여러 요금 유형에 적용 될 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="caddd-187">*License-based discounts may be applied to multiple charge types.*</span></span>
