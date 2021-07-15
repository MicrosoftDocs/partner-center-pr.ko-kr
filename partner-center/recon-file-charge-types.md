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
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989777"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="20a4d-103">파트너 센터 조정 파일의 다양한 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="20a4d-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="20a4d-104">**적용 대상**: 파트너 센터 | Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="20a4d-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="20a4d-105">**적절한 역할**: 관리 에이전트 | 청구 관리자 | 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="20a4d-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="20a4d-106">이 문서에서는 청구서 섹션과 조정 파일에 있을 수 있는 관련 요금 유형 간의 매핑을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="20a4d-107">청구서는 요금 요약을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="20a4d-108">조정 파일은 요금 유형을 포함하여 품목 트랜잭션에 대한 자세한 분석을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="20a4d-109">조정 파일에 대한 자세한 내용은 [조정 파일 사용 방법을 참조하세요.](use-the-reconciliation-files.md)</span><span class="sxs-lookup"><span data-stu-id="20a4d-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="20a4d-110">[사용량 기반 조정 파일과](usage-based-recon-files.md) [라이선스 기반 조정 파일은](license-based-recon-files.md) 모두 사용량 관련 트랜잭션 및 요금(소비 단위 및 관련 요금)만 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="20a4d-111">조정으로 청구서에 표시되는 일회성 크레딧, 할인 또는 **환불은** 조정 파일에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="20a4d-112">요금 유형을 청구서 요금에 매핑</span><span class="sxs-lookup"><span data-stu-id="20a4d-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="20a4d-113">청구서와 조정 파일 간의 요금 금액을 상호 참조하려면 Microsoft Excel 필터 옵션을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="20a4d-114">조정 파일의 요금 유형을 기준으로 필터링하여 청구서 요금을 조정 파일의 요금 분석 세트에 매핑합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="20a4d-115">라이선스 기반 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-115">License-based charges</span></span>

<span data-ttu-id="20a4d-116">이러한 라이선스 기반 요금을 청구서에 매핑하려면 라이선스 기반 파일에서 **Amount** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="20a4d-117">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="20a4d-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="20a4d-118">요금 설명</span><span class="sxs-lookup"><span data-stu-id="20a4d-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="20a4d-119">활성화 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-119">Activation fee</span></span> | <span data-ttu-id="20a4d-120">구매 후 구독을 사용할 때 고객에게 청구되는 금액입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="20a4d-121">취소 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-121">Cancel fee</span></span> | <span data-ttu-id="20a4d-122">관련 라이선스가 변경될 때 고객에게 비례 배분된 요금이 환불됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="20a4d-123">인스턴스 배분 취소</span><span class="sxs-lookup"><span data-stu-id="20a4d-123">Cancel instance prorate</span></span> | <span data-ttu-id="20a4d-124">월간 구독이 있는 고객이 구독을 일시 중단했으며 관련 라이선스가 같은 달 내에 변경되면 비례 배분 요금이 취소됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="20a4d-125">주기 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-125">Cycle fee</span></span> | <span data-ttu-id="20a4d-126">구독에 대한 정기 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="20a4d-127">주기 인스턴스 비례 배분</span><span class="sxs-lookup"><span data-stu-id="20a4d-127">Cycle instance prorate</span></span> | <span data-ttu-id="20a4d-128">관련 라이선스가 변경될 때 고객으로부터 평가된 비례 배분 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="20a4d-129">취소 시 요금이 부과됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-129">Prorate fees when cancel</span></span> | <span data-ttu-id="20a4d-130">취소 시 사용되지 않은 서비스 부분에 대해 비례 배분된 환불입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="20a4d-131">현재 제품에서 전환할 때 요금 부과</span><span class="sxs-lookup"><span data-stu-id="20a4d-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="20a4d-132">현재 월간 구독에서 연간 구독으로 전환한 후 비례 배분된 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="20a4d-133">새 제품으로 변환할 때 요금을 조달합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="20a4d-134">월간 구독을 새 연간 구독으로 변환한 후 비례 배분된 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="20a4d-135">구매 시 비례 배분 방식 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-135">Prorate fees when purchase</span></span> | <span data-ttu-id="20a4d-136">월간 또는 연간 청구를 모두 사용하는 경우 구독에 대한 요금 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="20a4d-137">갱신 시 요금 부과</span><span class="sxs-lookup"><span data-stu-id="20a4d-137">Prorate fee when renew</span></span> | <span data-ttu-id="20a4d-138">구독 갱신 시 비례 배분 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="20a4d-139">요금 갱신</span><span class="sxs-lookup"><span data-stu-id="20a4d-139">Renew fee</span></span> | <span data-ttu-id="20a4d-140">구독 갱신에 대한 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="20a4d-141">활성화 시 요금 조달</span><span class="sxs-lookup"><span data-stu-id="20a4d-141">Prorate fees when activate</span></span> | <span data-ttu-id="20a4d-142">정품 인증부터 청구 기간이 끝날 때까지 비례 배분된 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="20a4d-143">일회성 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-143">One-time charges</span></span>

<span data-ttu-id="20a4d-144">이러한 일회성 요금을 청구서에 매핑하려면 라이선스 기반 파일에서 **Amount** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="20a4d-145">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="20a4d-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="20a4d-146">요금 설명</span><span class="sxs-lookup"><span data-stu-id="20a4d-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="20a4d-147">new</span><span class="sxs-lookup"><span data-stu-id="20a4d-147">new</span></span> | <span data-ttu-id="20a4d-148">새 구매를 만들 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="20a4d-149">갱신</span><span class="sxs-lookup"><span data-stu-id="20a4d-149">renew</span></span> | <span data-ttu-id="20a4d-150">기간이 끝난 후 구독이 갱신될 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-150">Used when a subscription is renewed after the end of the term.</span></span> |
| <span data-ttu-id="20a4d-151">addQuantity</span><span class="sxs-lookup"><span data-stu-id="20a4d-151">addQuantity</span></span> | <span data-ttu-id="20a4d-152">원래 구매의 환불과 증가 후 새 수량 모두에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-152">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="20a4d-153">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="20a4d-153">removeQuantity</span></span> | <span data-ttu-id="20a4d-154">감소 후 원래 구매의 환불과 새 수량 모두에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-154">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="20a4d-155">cancelImmediate</span><span class="sxs-lookup"><span data-stu-id="20a4d-155">cancelImmediate</span></span> | <span data-ttu-id="20a4d-156">구독이 취소될 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-156">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="20a4d-157">변환</span><span class="sxs-lookup"><span data-stu-id="20a4d-157">convert</span></span> | <span data-ttu-id="20a4d-158">라이선스를 업그레이드할 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-158">Used when a license is upgraded.</span></span> |
| <span data-ttu-id="20a4d-159">customerCredit</span><span class="sxs-lookup"><span data-stu-id="20a4d-159">customerCredit</span></span> | <span data-ttu-id="20a4d-160">트랜잭션에 대해 크레딧(예: Azure, SLA 등)을 부여할 때 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-160">Used when credits (e.g., Azure, SLA, etc.) are given against a transaction.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="20a4d-161">사용 요금</span><span class="sxs-lookup"><span data-stu-id="20a4d-161">Usage charges</span></span>

<span data-ttu-id="20a4d-162">이러한 사용 요금을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="20a4d-163">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="20a4d-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="20a4d-164">요금 설명</span><span class="sxs-lookup"><span data-stu-id="20a4d-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="20a4d-165">취소 시 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="20a4d-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="20a4d-166">현재 청구 기간 동안 미지불된 사용량에 대해 취소 시 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="20a4d-167">현재 주기에 대한 사용 요금 평가</span><span class="sxs-lookup"><span data-stu-id="20a4d-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="20a4d-168">현재 청구 기간에 대한 사용 요금에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="20a4d-169">크레딧</span><span class="sxs-lookup"><span data-stu-id="20a4d-169">Credits</span></span>

<span data-ttu-id="20a4d-170">이러한 크레딧을 청구서에 매핑하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="20a4d-171">라이선스 기반 파일에서 **TotalForCustomer의** 합계를 구합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="20a4d-172">사용량 기반 파일에서 **PostTaxTotal** 열의 합계를 구합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="20a4d-173">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="20a4d-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="20a4d-174">요금 설명</span><span class="sxs-lookup"><span data-stu-id="20a4d-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="20a4d-175">줄 항목 오프셋</span><span class="sxs-lookup"><span data-stu-id="20a4d-175">Offset a line item</span></span> | <span data-ttu-id="20a4d-176">세금을 포함하여 품목에 대한 부분 또는 전체 환불액입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="20a4d-177">사용량 기반 할인</span><span class="sxs-lookup"><span data-stu-id="20a4d-177">Usage-based discounts</span></span>

<span data-ttu-id="20a4d-178">이러한 사용량 기반 할인을 청구서에 매핑하려면 사용량 기반 파일에서 **PretaxCharges** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="20a4d-179">요금 설명(조정 파일의 ChargeType 열)</span><span class="sxs-lookup"><span data-stu-id="20a4d-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="20a4d-180">요금 설명</span><span class="sxs-lookup"><span data-stu-id="20a4d-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="20a4d-181">정품 인증 할인</span><span class="sxs-lookup"><span data-stu-id="20a4d-181">Activation discount</span></span> | <span data-ttu-id="20a4d-182">구독이 활성화될 때 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="20a4d-183">주기 할인</span><span class="sxs-lookup"><span data-stu-id="20a4d-183">Cycle discount</span></span> | <span data-ttu-id="20a4d-184">주기적 요금에 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="20a4d-185">할인 갱신</span><span class="sxs-lookup"><span data-stu-id="20a4d-185">Renew discount</span></span> | <span data-ttu-id="20a4d-186">구독이 갱신될 때 적용되는 할인입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="20a4d-187">할인 취소</span><span class="sxs-lookup"><span data-stu-id="20a4d-187">Cancel discount</span></span> | <span data-ttu-id="20a4d-188">할인이 취소될 때 적용되는 요금입니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="20a4d-189">라이선스 기반 할인</span><span class="sxs-lookup"><span data-stu-id="20a4d-189">License-based discounts</span></span>

<span data-ttu-id="20a4d-190">라이선스 기반 할인을 청구서에 매핑하려면 라이선스 기반 파일에서 **TotalOtherDiscount** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="20a4d-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="20a4d-191">*라이선스 기반 할인은 여러 요금 유형에 적용될 수 있습니다.*</span><span class="sxs-lookup"><span data-stu-id="20a4d-191">*License-based discounts may be applied to multiple charge types.*</span></span>
