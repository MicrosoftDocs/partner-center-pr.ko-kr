---
title: 유효 단가 계산
ms.topic: how-to
ms.date: 04/02/2021
description: 유효 단가 및 계산 방법에 대해 알아봅니다. 이 문서에는 샘플 계산도 포함되어 있습니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147125"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="78315-104">Azure 플랜 사용량에 대한 유효 단가 계산</span><span class="sxs-lookup"><span data-stu-id="78315-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="78315-105">**적절한 역할:** 청구 관리자</span><span class="sxs-lookup"><span data-stu-id="78315-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="78315-106">유효 단가</span><span class="sxs-lookup"><span data-stu-id="78315-106">The effective unit price</span></span>

<span data-ttu-id="78315-107">유효 단가는 리소스 수준과 달리 미터 수준에서 계산되며 측정기 사용량에 따라 매일 조정됩니다.</span><span class="sxs-lookup"><span data-stu-id="78315-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="78315-108">다음 세 가지 요소를 사용하여 유효 단가를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="78315-109">사용량- 청구 주기 전체에서 매일 모니터링됩니다.</span><span class="sxs-lookup"><span data-stu-id="78315-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="78315-110">미터에 대한 청구 가능 비용</span><span class="sxs-lookup"><span data-stu-id="78315-110">Billable cost for the meter</span></span>
- <span data-ttu-id="78315-111">계층화(해당하는 경우)</span><span class="sxs-lookup"><span data-stu-id="78315-111">Tiering (if applicable)</span></span>

<span data-ttu-id="78315-112">청구 주기 동안 매일 사용량을 모니터링하기 때문에 유효 단가가 변동됩니다.</span><span class="sxs-lookup"><span data-stu-id="78315-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="78315-113">사용량 계산을 중지하고 청구 기간을 닫으면 지정된 청구 주기에 대한 최종 가격을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78315-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="78315-114">네 번째 또는 다섯 번째 소수점 이하의 사용량에 대부분의 변경 내용이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="78315-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="78315-115">미터에서 계층형 가격 책정을 사용하는지 확인</span><span class="sxs-lookup"><span data-stu-id="78315-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="78315-116">측정기에서 계층형 가격 책정을 사용하는지 여부를 모르는 경우 아래 절차를 사용하여 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="78315-117">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="78315-118">**판매를** 선택하고 **가격 책정 및 제안을** 선택한 **다음, Azure 플랜 가격 책정을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="78315-119">ID로 미터를 찾은 다음 가격 책정 데이터를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="78315-120">샘플 계산</span><span class="sxs-lookup"><span data-stu-id="78315-120">Sample calculation</span></span>

<span data-ttu-id="78315-121">아래 표에서는 오픈 기간 동안 유효 단가를 계산하는 방법의 예를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="78315-122">표에서 다음 값이 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="78315-123">**UP** = 리소스의 단가 = 0.868</span><span class="sxs-lookup"><span data-stu-id="78315-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="78315-124">**Bcu** = 청구 가능한 소비 단위 (측정기)</span><span class="sxs-lookup"><span data-stu-id="78315-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="78315-125">**BC** = 측정기 = BCU \* UP \* 0.85에 대 한 청구 가능 비용입니다.</span><span class="sxs-lookup"><span data-stu-id="78315-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="78315-126">이는 15%의 PEC 할인에 대 한 조정을 반영 합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="78315-127">그런 다음 최소 금액을 청구 하기 위해 함수의 하한값을 사용 하 여 소수점이 하 두 자리로 값을 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="78315-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="78315-128">**유효 단가** = bcu/BC</span><span class="sxs-lookup"><span data-stu-id="78315-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="78315-129">참고:이 예제의 미터에는 가격 책정 또는 기타 할인이 포함 되지 않습니다. 할인 백분율 및 기타 조정의 유효 단가 요소가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78315-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="78315-130">Date</span><span class="sxs-lookup"><span data-stu-id="78315-130">Date</span></span> | <span data-ttu-id="78315-131">BCU (청구 가능한 소비 단위)</span><span class="sxs-lookup"><span data-stu-id="78315-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="78315-132">BC (청구 가능 비용)</span><span class="sxs-lookup"><span data-stu-id="78315-132">BC (Billable cost)</span></span> | <span data-ttu-id="78315-133">유효 단가</span><span class="sxs-lookup"><span data-stu-id="78315-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="78315-134">3-8 월</span><span class="sxs-lookup"><span data-stu-id="78315-134">3-Aug</span></span> | <span data-ttu-id="78315-135">29</span><span class="sxs-lookup"><span data-stu-id="78315-135">29</span></span> | <span data-ttu-id="78315-136">21.39</span><span class="sxs-lookup"><span data-stu-id="78315-136">21.39</span></span> | <span data-ttu-id="78315-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="78315-137">0.737586206896552</span></span> |
| <span data-ttu-id="78315-138">10-8 월</span><span class="sxs-lookup"><span data-stu-id="78315-138">10-Aug</span></span> | <span data-ttu-id="78315-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="78315-139">210.950039</span></span> | <span data-ttu-id="78315-140">155.63</span><span class="sxs-lookup"><span data-stu-id="78315-140">155.63</span></span> | <span data-ttu-id="78315-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="78315-141">0.737757626107858</span></span> |
| <span data-ttu-id="78315-142">25-8 월</span><span class="sxs-lookup"><span data-stu-id="78315-142">25-Aug</span></span> | <span data-ttu-id="78315-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="78315-143">555.950039</span></span> | <span data-ttu-id="78315-144">410.17</span><span class="sxs-lookup"><span data-stu-id="78315-144">410.17</span></span> | <span data-ttu-id="78315-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="78315-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="78315-146">다음 단계</span><span class="sxs-lookup"><span data-stu-id="78315-146">Next steps</span></span>

- [<span data-ttu-id="78315-147">청구 및 세금</span><span class="sxs-lookup"><span data-stu-id="78315-147">Billing and taxes</span></span>](billing.md)
