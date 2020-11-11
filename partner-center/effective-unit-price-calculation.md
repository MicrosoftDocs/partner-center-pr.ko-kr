---
title: 유효 단위 가격 계산
ms.topic: how-to
ms.date: 11/10/2020
description: 유효 가격 단위 및 계산 방법에 대해 알아봅니다. 에는 샘플 계산이 포함 되어 있습니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498581"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="65b57-104">Azure 계획 소비에 대 한 유효 단위 가격 계산</span><span class="sxs-lookup"><span data-stu-id="65b57-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="65b57-105">유효 단가</span><span class="sxs-lookup"><span data-stu-id="65b57-105">The effective unit price</span></span>

<span data-ttu-id="65b57-106">유효 단가는 리소스 수준과 달리 미터 수준에서 계산 되며 미터 사용에 따라 매일 조정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="65b57-107">다음 세 가지 요소를 사용 하 여 유효 단가를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="65b57-108">사용량-청구 주기 전체에 걸쳐 매일 모니터링 됩니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="65b57-109">측정기에 대 한 청구 가능 비용</span><span class="sxs-lookup"><span data-stu-id="65b57-109">Billable cost for the meter</span></span>
- <span data-ttu-id="65b57-110">계층화 (해당 하는 경우)</span><span class="sxs-lookup"><span data-stu-id="65b57-110">Tiering (if applicable)</span></span>

<span data-ttu-id="65b57-111">청구 주기 동안 매일 사용량을 모니터링 하므로 유효 단가가 변동 됩니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="65b57-112">지정 된 청구 주기에 대 한 최종 가격은 소비 계산을 중지 하 고 청구 기간을 종결 한 후에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="65b57-113">네 번째 또는 다섯 번째 소수 자릿수 뒤의 소비에 대 한 대부분의 변경 내용이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="65b57-114">측정기에서 계층화 된 가격 책정을 사용 하는지 확인</span><span class="sxs-lookup"><span data-stu-id="65b57-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="65b57-115">측정기에서 계층화 된 가격 책정을 사용 하는지 여부를 모르는 경우 아래 절차를 사용 하 여 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="65b57-116">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="65b57-117">**판매** 를 선택 하 고 **가격 책정 및 제품** 을 선택한 후 **Azure 계획 가격 책정** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="65b57-118">ID로 측정기를 찾은 후 가격 데이터를 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="65b57-119">샘플 계산</span><span class="sxs-lookup"><span data-stu-id="65b57-119">Sample calculation</span></span>

<span data-ttu-id="65b57-120">아래 표에서는 여는 기간 동안 유효 단가를 계산 하는 방법의 예를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="65b57-121">테이블에서 다음 값이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="65b57-122">**UP** = 리소스의 단가 = 0.868</span><span class="sxs-lookup"><span data-stu-id="65b57-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="65b57-123">**Bcu** = 청구 가능한 소비 단위 (측정기)</span><span class="sxs-lookup"><span data-stu-id="65b57-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="65b57-124">**BC** = 측정기 = BCU \* UP \* 0.85에 대 한 청구 가능 비용입니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="65b57-125">이는 15%의 PEC 할인에 대 한 조정을 반영 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="65b57-126">그런 다음 최소 금액을 청구 하기 위해 함수의 하한값을 사용 하 여 소수점이 하 두 자리로 값을 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="65b57-127">**유효 단가** = bcu/BC</span><span class="sxs-lookup"><span data-stu-id="65b57-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="65b57-128">참고:이 예제의 미터는 가격 책정의 계층을 포함 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="65b57-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="65b57-129">날짜</span><span class="sxs-lookup"><span data-stu-id="65b57-129">Date</span></span> | <span data-ttu-id="65b57-130">BCU (청구 가능한 소비 단위)</span><span class="sxs-lookup"><span data-stu-id="65b57-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="65b57-131">BC (청구 가능 비용)</span><span class="sxs-lookup"><span data-stu-id="65b57-131">BC (Billable cost)</span></span> | <span data-ttu-id="65b57-132">유효 단가</span><span class="sxs-lookup"><span data-stu-id="65b57-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="65b57-133">3-8 월</span><span class="sxs-lookup"><span data-stu-id="65b57-133">3-Aug</span></span> | <span data-ttu-id="65b57-134">29</span><span class="sxs-lookup"><span data-stu-id="65b57-134">29</span></span> | <span data-ttu-id="65b57-135">21.39</span><span class="sxs-lookup"><span data-stu-id="65b57-135">21.39</span></span> | <span data-ttu-id="65b57-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="65b57-136">0.737586206896552</span></span> |
| <span data-ttu-id="65b57-137">10-8 월</span><span class="sxs-lookup"><span data-stu-id="65b57-137">10-Aug</span></span> | <span data-ttu-id="65b57-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="65b57-138">210.950039</span></span> | <span data-ttu-id="65b57-139">155.63</span><span class="sxs-lookup"><span data-stu-id="65b57-139">155.63</span></span> | <span data-ttu-id="65b57-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="65b57-140">0.737757626107858</span></span> |
| <span data-ttu-id="65b57-141">25-8 월</span><span class="sxs-lookup"><span data-stu-id="65b57-141">25-Aug</span></span> | <span data-ttu-id="65b57-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="65b57-142">555.950039</span></span> | <span data-ttu-id="65b57-143">410.17</span><span class="sxs-lookup"><span data-stu-id="65b57-143">410.17</span></span> | <span data-ttu-id="65b57-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="65b57-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="65b57-145">다음 단계</span><span class="sxs-lookup"><span data-stu-id="65b57-145">Next steps</span></span>

- [<span data-ttu-id="65b57-146">청구 및 세금</span><span class="sxs-lookup"><span data-stu-id="65b57-146">Billing and taxes</span></span>](billing.md)
