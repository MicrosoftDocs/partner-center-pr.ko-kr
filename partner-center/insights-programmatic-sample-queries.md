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
# <a name="sample-queries-for-partner-center-insights-report"></a>파트너 센터 인사이트 보고서에 대한 샘플 쿼리

이 문서에서는 파트너 Insights 보고서에 대한 샘플 쿼리를 제공합니다. 보고서 쿼리 만들기 API 엔드포인트를 호출하여 이러한 쿼리를 사용할 수 있습니다. 필요한 경우 [보고서 쿼리 만들기 API](insights-programmatic-access-paradigm.md#create-report-query-api) 호출을 수정하여 더 많은 열을 추가하고, 계산 기간을 조정하고, 필터 조건을 추가할 수 있습니다.

열 이름, 특성 및 설명에 대한 자세한 내용은 데이터 정의 를 [참조하세요.](insights-data-definitions.md)

## <a name="customer-details"></a>고객 세부 정보

이러한 샘플 쿼리는 고객 세부 정보 보고서에 적용됩니다.

### <a name="by-geography"></a>지리별

지난 달 특정 지역의 고객 목록입니다.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>SKU 및 청구 수익별

특정 SKU 및 청구된 수익을 사용하는 고객 목록은 지난 6개월 동안 20,000개 이상입니다.

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>사용 가능한 시트별

지난 달 사용 가능한 시트를 기반으로 하는 상위 10명의 고객

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>파트너 프로필

이러한 샘플 쿼리는 파트너 프로필 보고서에 적용됩니다.

### <a name="by-geography"></a>지리별

특정 지리적 위치에서 파트너의 목록입니다.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>MPN 파트너별

동일한 PGA MPN 파트너 아래의 파트너 목록

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Reseller Performance

이러한 샘플 쿼리는 대리점 성능 보고서에 적용됩니다.

### <a name="by-geography"></a>지리별

지난 달 특정 지역의 대리점 목록입니다.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>대리점별

고객 수, 구독 수, 사용 가능한 총 사용자, 할당된 총 사용자, 특정 대리점의 총 수익.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>수익별 상위 10개

지난 달의 총 수익을 기준으로 상위 10개 대리점.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>구독 세부 정보

이러한 샘플 쿼리는 구독 세부 정보 보고서에 적용됩니다.

### <a name="by-renewal-eligibility"></a>갱신 자격 기준

지난 달에 자동 갱신할 수 없는 구독 목록입니다.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>구독 상태별

지난 달의 사용 안 함 상태에 있는 구독 목록입니다.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>6개월의 개수

지난 6개월 동안 특정 파트너의 구독 수, 총 판매 사용자 수, 고객 수입니다.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Azure 사용량

이러한 샘플 쿼리는 Azure 사용량 보고서에 적용됩니다.

### <a name="by-meter-category"></a>미터 범주별

지난 6개월 동안 특정 미터 범주에 대한 사용 단위 및 ACR을 사용하는 Azure 사용량 구독 목록입니다.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>총 ACR 기준

지난 6개월 동안 총 ACR이 20,000개를 초과하는 Azure 사용량 구독 목록

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>다음 단계

- [파트너 인사이트 분석 데이터에 액세스하기 위한 API](insights-programmatic-analytics-available-api.md)