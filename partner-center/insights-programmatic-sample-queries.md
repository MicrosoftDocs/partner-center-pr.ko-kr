---
title: 샘플 쿼리 목록
description: 샘플 쿼리를 사용하여 프로그래밍 방식으로 파트너 인사이트 분석 데이터에 액세스합니다.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375851"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="280dd-103">파트너 센터 인사이트 보고서에 대한 샘플 쿼리</span><span class="sxs-lookup"><span data-stu-id="280dd-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="280dd-104">이 문서에서는 파트너 Insights 보고서에 대한 샘플 쿼리를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="280dd-105">보고서 쿼리 만들기 API 엔드포인트를 호출하여 이러한 쿼리를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="280dd-106">필요한 경우 [보고서 쿼리 만들기 API](insights-programmatic-access-paradigm.md#create-report-query-api) 호출을 수정하여 더 많은 열을 추가하고, 계산 기간을 조정하고, 필터 조건을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="280dd-107">열 이름, 특성 및 설명에 대한 자세한 내용은 데이터 정의 를 [참조하세요.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="280dd-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="280dd-108">고객 세부 정보</span><span class="sxs-lookup"><span data-stu-id="280dd-108">Customer details</span></span>

<span data-ttu-id="280dd-109">이러한 샘플 쿼리는 고객 세부 정보 보고서에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="280dd-110">지리별</span><span class="sxs-lookup"><span data-stu-id="280dd-110">By geography</span></span>

<span data-ttu-id="280dd-111">지난 달 특정 지역의 고객 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="280dd-112">SKU 및 청구 수익별</span><span class="sxs-lookup"><span data-stu-id="280dd-112">By SKU and billed revenue</span></span>

<span data-ttu-id="280dd-113">특정 SKU 및 청구된 수익을 사용하는 고객 목록은 지난 6개월 동안 20,000개 이상입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="280dd-114">사용 가능한 시트별</span><span class="sxs-lookup"><span data-stu-id="280dd-114">By available seats</span></span>

<span data-ttu-id="280dd-115">지난 달 사용 가능한 시트를 기반으로 하는 상위 10명의 고객</span><span class="sxs-lookup"><span data-stu-id="280dd-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="280dd-116">파트너 프로필</span><span class="sxs-lookup"><span data-stu-id="280dd-116">Partner Profile</span></span>

<span data-ttu-id="280dd-117">이러한 샘플 쿼리는 파트너 프로필 보고서에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="280dd-118">지리별</span><span class="sxs-lookup"><span data-stu-id="280dd-118">By geography</span></span>

<span data-ttu-id="280dd-119">특정 지리적 위치에서 파트너의 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="280dd-120">MPN 파트너별</span><span class="sxs-lookup"><span data-stu-id="280dd-120">By MPN partner</span></span>

<span data-ttu-id="280dd-121">동일한 PGA MPN 파트너 아래의 파트너 목록</span><span class="sxs-lookup"><span data-stu-id="280dd-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="280dd-122">Reseller Performance</span><span class="sxs-lookup"><span data-stu-id="280dd-122">Reseller Performance</span></span>

<span data-ttu-id="280dd-123">이러한 샘플 쿼리는 대리점 성능 보고서에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="280dd-124">지리별</span><span class="sxs-lookup"><span data-stu-id="280dd-124">By geography</span></span>

<span data-ttu-id="280dd-125">지난 달 특정 지역의 대리점 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="280dd-126">대리점별</span><span class="sxs-lookup"><span data-stu-id="280dd-126">By reseller</span></span>

<span data-ttu-id="280dd-127">고객 수, 구독 수, 사용 가능한 총 사용자, 할당된 총 사용자, 특정 대리점의 총 수익.</span><span class="sxs-lookup"><span data-stu-id="280dd-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="280dd-128">수익별 상위 10개</span><span class="sxs-lookup"><span data-stu-id="280dd-128">Top 10 by revenue</span></span>

<span data-ttu-id="280dd-129">지난 달의 총 수익을 기준으로 상위 10개 대리점.</span><span class="sxs-lookup"><span data-stu-id="280dd-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="280dd-130">구독 세부 정보</span><span class="sxs-lookup"><span data-stu-id="280dd-130">Subscription Details</span></span>

<span data-ttu-id="280dd-131">이러한 샘플 쿼리는 구독 세부 정보 보고서에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="280dd-132">갱신 자격 기준</span><span class="sxs-lookup"><span data-stu-id="280dd-132">By renewal eligibility</span></span>

<span data-ttu-id="280dd-133">지난 달에 자동 갱신할 수 없는 구독 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="280dd-134">구독 상태별</span><span class="sxs-lookup"><span data-stu-id="280dd-134">By subscription state</span></span>

<span data-ttu-id="280dd-135">지난 달의 사용 안 함 상태에 있는 구독 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="280dd-136">6개월의 개수</span><span class="sxs-lookup"><span data-stu-id="280dd-136">Counts for six months</span></span>

<span data-ttu-id="280dd-137">지난 6개월 동안 특정 파트너의 구독 수, 총 판매 사용자 수, 고객 수입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="280dd-138">Azure 사용량</span><span class="sxs-lookup"><span data-stu-id="280dd-138">Azure Usage</span></span>

<span data-ttu-id="280dd-139">이러한 샘플 쿼리는 Azure 사용량 보고서에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="280dd-140">미터 범주별</span><span class="sxs-lookup"><span data-stu-id="280dd-140">By meter category</span></span>

<span data-ttu-id="280dd-141">지난 6개월 동안 특정 미터 범주에 대한 사용 단위 및 ACR을 사용하는 Azure 사용량 구독 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="280dd-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="280dd-142">총 ACR 기준</span><span class="sxs-lookup"><span data-stu-id="280dd-142">By total ACR</span></span>

<span data-ttu-id="280dd-143">지난 6개월 동안 총 ACR이 20,000개를 초과하는 Azure 사용량 구독 목록</span><span class="sxs-lookup"><span data-stu-id="280dd-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="280dd-144">다음 단계</span><span class="sxs-lookup"><span data-stu-id="280dd-144">Next steps</span></span>

- [<span data-ttu-id="280dd-145">파트너 인사이트 분석 데이터에 액세스하기 위한 API</span><span class="sxs-lookup"><span data-stu-id="280dd-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)