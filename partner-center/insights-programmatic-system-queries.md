---
title: 파트너 insights 프로그래밍 방식의 액세스를 위한 시스템 쿼리 목록
description: 파트너 insights 분석 데이터에 액세스 하는 데 사용할 수 있는 시스템 쿼리에 대해 자세히 알아보세요.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 4b0bd5411d02463b015cf812cde78e34ef853814
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375832"
---
# <a name="list-of-system-queries-for-partner-insights-programmatic-access"></a><span data-ttu-id="1c85a-103">파트너 insights 프로그래밍 방식의 액세스를 위한 시스템 쿼리 목록</span><span class="sxs-lookup"><span data-stu-id="1c85a-103">List of system queries for partner insights programmatic access</span></span>

<span data-ttu-id="1c85a-104">QueryId를 사용 하 여 [보고서 만들기 API](insights-programmatic-access-paradigm.md#create-report-api) 에서 직접 다음 시스템 쿼리를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c85a-104">The following system queries can be used in the [Create Report API](insights-programmatic-access-paradigm.md#create-report-api) directly with a QueryId.</span></span> <span data-ttu-id="1c85a-105">시스템 쿼리는 6 개월 (6M) 계산 기간 동안 파트너 센터의 보고서 내보내기와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1c85a-105">The system queries are like the export reports in Partner Center for a six-month (6M) computation period.</span></span>

<span data-ttu-id="1c85a-106">열 이름, 특성 및 설명에 대 한 자세한 내용은 [데이터 정의](insights-data-definitions.md) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="1c85a-106">For more details on the column names, attributes, and description, please refer to the [Data Definitions](insights-data-definitions.md)</span></span>

<span data-ttu-id="1c85a-107">다음 섹션에서는 다양한 보고서에 대한 보고서 쿼리를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="1c85a-107">The following sections provide report queries for various reports.</span></span>

## <a name="customers"></a><span data-ttu-id="1c85a-108">고객</span><span class="sxs-lookup"><span data-stu-id="1c85a-108">Customers</span></span>

<span data-ttu-id="1c85a-109">지난 6 개월 동안 고객에 게 보고</span><span class="sxs-lookup"><span data-stu-id="1c85a-109">The Customers report for the last six months</span></span>

<span data-ttu-id="1c85a-110">쿼리 ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span><span class="sxs-lookup"><span data-stu-id="1c85a-110">Query ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-111">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-111">Report query</span></span>
```sql
SELECT PGAMpnId,MpnId,PartnerName,CustomerName,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,
CustomerMarket,CustomerStatus,CustomerTenantId,CustomerTenantName,CustomerTenantCountry,TenantDomainName,
Product,RawProductName,ProductPartNumber,SKU,Month,PartnerLocation,PartnerAttributionType,SalesChannel,
IsDuplicateRowForPGA,AvailableSeats,BilledRevenueUSD,AzureConsumedRevenueUSD 
FROM CustomersAndTenants TIMESPAN LAST_6_MONTHS
```

## <a name="seats-subscriptions-and-revenue"></a><span data-ttu-id="1c85a-112">좌석 구독 및 수익</span><span class="sxs-lookup"><span data-stu-id="1c85a-112">Seats Subscriptions and Revenue</span></span>

<span data-ttu-id="1c85a-113">지난 6 개월 동안의 좌석, 구독 및 수익 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-113">Seats, subscriptions, and revenue report for the last six months</span></span>

<span data-ttu-id="1c85a-114">쿼리 ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span><span class="sxs-lookup"><span data-stu-id="1c85a-114">Query ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-115">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-115">Report query</span></span>

```sql
SELECT PGAMpnId,MpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionState,month,
IsAutoRenew,CustomerName,CustomerTenantId,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,CustomerMarket,
ProductFamily,ReportingProductName,Product,RawProductName,ProductPartNumber,SKU,RevSumDivisionName,PartnerName,
SolutionArea,PartnerLocation,PartnerAttributionType,SalesChannel,PricingLevel,EnrollmentNumber,
IsDuplicateRowForPGA,SubscriptionStartMonth,TotalSoldSeats,TotalAssignedSeats,BilledRevenueUSD,
AzureConsumedRevenueUSD FROM SeatsSubscriptionsAndRevenue TIMESPAN LAST_6_MONTHS
```

## <a name="partner-profile"></a><span data-ttu-id="1c85a-116">파트너 프로필</span><span class="sxs-lookup"><span data-stu-id="1c85a-116">Partner Profile</span></span>

<span data-ttu-id="1c85a-117">데이터 프로파일링</span><span class="sxs-lookup"><span data-stu-id="1c85a-117">Profile data</span></span>

<span data-ttu-id="1c85a-118">쿼리 ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span><span class="sxs-lookup"><span data-stu-id="1c85a-118">Query ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-119">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-119">Report query</span></span>

```sql
SELECT MPNId,PartnerName,PGA_MPNId,PGA_PartnerName,City,Country,HierarchyLevel 
FROM Profile
```

## <a name="azure-usage"></a><span data-ttu-id="1c85a-120">Azure 사용량</span><span class="sxs-lookup"><span data-stu-id="1c85a-120">Azure Usage</span></span>

<span data-ttu-id="1c85a-121">지난 6 개월 동안의 AzureUsage 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-121">AzureUsage report for the last six months</span></span>

<span data-ttu-id="1c85a-122">쿼리 ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span><span class="sxs-lookup"><span data-stu-id="1c85a-122">Query ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-123">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-123">Report query</span></span>

```sql
SELECT PGAMpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,FirstUseDate,SubscriptionState,Month,
ServiceName,MeterCategory,UsageUnits,UsageQuantity,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MpnId,PartnerName,PartnerLocation,PartnerAttributionType,SalesChannel,EnrollmentNumber,
IsACRDuplicateAtPGALevel,ResellerID,ResellerName,MonthlySubscriptionLevelACR,TotalACR 
FROM AzureUsage TIMESPAN LAST_6_MONTHS
```

## <a name="office-usage"></a><span data-ttu-id="1c85a-124">Office 보려면</span><span class="sxs-lookup"><span data-stu-id="1c85a-124">Office Usage</span></span>

<span data-ttu-id="1c85a-125">지난 6 개월 동안 사용 현황 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-125">OfficeUsage report for the last six months</span></span>

<span data-ttu-id="1c85a-126">쿼리 ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span><span class="sxs-lookup"><span data-stu-id="1c85a-126">Query ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-127">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-127">Report query</span></span>

```sql
SELECT CustomerTenantId,CustomerTpid,WorkloadName,Month,PaidAvailableUnits,MonthlyActiveUsers,CustomerName,
CustomerMarket,CustomerSegment,MPNId,PartnerName,PartnerLocation,PartnerAttributionType,IsDuplicateRowForPGA
FROM OfficeUsage TIMESPAN LAST_6_MONTHS
```

## <a name="dynamics-usage"></a><span data-ttu-id="1c85a-128">Dynamics 사용</span><span class="sxs-lookup"><span data-stu-id="1c85a-128">Dynamics Usage</span></span>

<span data-ttu-id="1c85a-129">6 개월 동안 DynamicsUsage 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-129">DynamicsUsage report for six months</span></span>

<span data-ttu-id="1c85a-130">쿼리 ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span><span class="sxs-lookup"><span data-stu-id="1c85a-130">Query ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-131">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-131">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,RevSumDivisionName,
RevSumCategoryName,SKU,SKUId,FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,
CustomerTpid,CustomerSegment,CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM DynamicsUsage TIMESPAN LAST_6_MONTHS
```

## <a name="power-bi-usage"></a><span data-ttu-id="1c85a-132">Power BI 사용량</span><span class="sxs-lookup"><span data-stu-id="1c85a-132">Power BI usage</span></span>

<span data-ttu-id="1c85a-133">6 개월 동안 PowerBIUsage 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-133">PowerBIUsage report for six months</span></span>

<span data-ttu-id="1c85a-134">쿼리 ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span><span class="sxs-lookup"><span data-stu-id="1c85a-134">Query ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-135">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-135">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM PowerBIUsage TIMESPAN LAST_6_MONTHS
```

## <a name="ems-usage"></a><span data-ttu-id="1c85a-136">EMS 사용</span><span class="sxs-lookup"><span data-stu-id="1c85a-136">EMS Usage</span></span>

<span data-ttu-id="1c85a-137">6 개월 동안 EMSUsage 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-137">EMSUsage report for six months</span></span>

<span data-ttu-id="1c85a-138">쿼리 ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span><span class="sxs-lookup"><span data-stu-id="1c85a-138">Query ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-139">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-139">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,PaidAvailableUnits,
MonthlyActiveUsers,AADPPaidAvailableUnits,IntunePaidAvailableUnits,AzipPaidAvailableUnits,
AADPMonthlyActiveUsers,IntuneMonthlyActiveUsers,AzipMonthlyActiveUsers FROM EMSUsage TIMESPAN LAST_6_MONTHS
```

## <a name="competency-performance-requirement-report"></a><span data-ttu-id="1c85a-140">역량 성능 요구 사항 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-140">Competency Performance requirement report</span></span>

<span data-ttu-id="1c85a-141">6 개월 동안 CompetencyPeformanceRequirement 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-141">CompetencyPeformanceRequirement report for six months</span></span>

<span data-ttu-id="1c85a-142">쿼리 ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span><span class="sxs-lookup"><span data-stu-id="1c85a-142">Query ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-143">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-143">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyAttainmentOptionName,Month,MetricName,MetricMonthlyContribution,TTMAggregate,
AnniversaryYearAggregate,GoldThreshold,SilverThreshold 
FROM CompetencyPeformanceRequirement 
TIMESPAN LAST_6_MONTHS
```

## <a name="cloud-products-reseller-performance"></a><span data-ttu-id="1c85a-144">클라우드 제품 재판매인 성능</span><span class="sxs-lookup"><span data-stu-id="1c85a-144">Cloud products reseller performance</span></span>

### <a name="report-description"></a><span data-ttu-id="1c85a-145">보고서 설명</span><span class="sxs-lookup"><span data-stu-id="1c85a-145">Report description</span></span>

<span data-ttu-id="1c85a-146">6 개월 동안 CloudProductsResellerPerformance 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-146">CloudProductsResellerPerformance report for six months</span></span>

<span data-ttu-id="1c85a-147">쿼리 ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span><span class="sxs-lookup"><span data-stu-id="1c85a-147">Query ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-148">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-148">Report query</span></span>

```sql
SELECT ResellerMpnid,ResellerName,ResellerMarket,IndirectProviderMPNId,IndirectProviderName,Month,Product,
SubscriptionID,AvailableSeats,AssignedSeats,BilledRevenueUSD,CustomerName,CustomerTPid,CustomerSegment,
CustomerMarket,ResellerStatus 
FROM CloudProductsResellerPerformance TIMESPAN LAST_6_MONTHS
```

## <a name="clas-agreement-renewal-propensity"></a><span data-ttu-id="1c85a-149">CLAS 규약 갱신 성향</span><span class="sxs-lookup"><span data-stu-id="1c85a-149">CLAS Agreement Renewal propensity</span></span>

<span data-ttu-id="1c85a-150">6 개월 동안 CLASAgreementRenewalsPropensity 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-150">CLASAgreementRenewalsPropensity report for six months</span></span>

<span data-ttu-id="1c85a-151">쿼리 ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span><span class="sxs-lookup"><span data-stu-id="1c85a-151">Query ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-152">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-152">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,HasGoogle,HasAWS,AzureCluster,D365FOCluster,D365CECluster,D365BCCluster,
M365Cluster,LicenseProgram,AgreementID,AgreementEndDate,ExpirationType,ExpiringRevenue,HasEA,HasOpen,
AzureUpsellCustomer,M365UpsellCustomer,RevSumDivisionName 
FROM CLASAgreementRenewalsPropensity
```

## <a name="clas-azure-propensity"></a><span data-ttu-id="1c85a-153">CLAS Azure 성향</span><span class="sxs-lookup"><span data-stu-id="1c85a-153">CLAS Azure propensity</span></span>

<span data-ttu-id="1c85a-154">6 개월 동안 CLASAzurePropensity 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-154">CLASAzurePropensity report for six months</span></span>

<span data-ttu-id="1c85a-155">쿼리 ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span><span class="sxs-lookup"><span data-stu-id="1c85a-155">Query ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-156">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-156">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,MigrateEOSWinServerWithCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithCLASPropensityBelow5Licenses,
MigrateEOSWinServerWithoutCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithoutCLASPropensityBelow5Licenses,MigrateEOSSQLWithCLASPropensityAbove5Licenses,
MigrateEOSSQLWithCLASPropensityBelow5Licenses,MigrateEOSSQLWithoutCLASPropensityAbove5Licenses,
MigrateEOSSQLWithoutCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithoutCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerIBWithoutCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityBelow5Licenses,MigrateOSSMigrateToOSSDB,
MigrateOSSLinuxOnAzure,MigrateSAPOnAzure,MigrateWVDRDSIB,MigrateWVDCrossSellModernWorkToAzureWVD,
MigrateVMWareIB,MigrateCitrixIB,InnovateAnalyticsPowerBIIBWithHighAzurepropensity,
EnableDevOpsWithGitHubVisualStudioMSDNIB,WinServerStandardVersion,WinServerStandardLicense,
WinServerDataCenterVersion,WinServerDataCenterLicense,AzureFit,AzureIntent,AzureCluster,
WindowsServerDataCenter_HasOpenRenewal,WindowsServerStandard_HasOpenRenewal,AzureUpsellCustomer,HasGoogle,
HasAWS,HasEA,HasOpen 
FROM CLASAzurePropensity
```

## <a name="clas-d365-propensity"></a><span data-ttu-id="1c85a-157">CLAS D365 성향</span><span class="sxs-lookup"><span data-stu-id="1c85a-157">CLAS D365 propensity</span></span>

<span data-ttu-id="1c85a-158">6 개월 동안 CLASD365Propensity 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-158">CLASD365Propensity report for six months</span></span>

<span data-ttu-id="1c85a-159">쿼리 ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span><span class="sxs-lookup"><span data-stu-id="1c85a-159">Query ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-160">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-160">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,ActivateDigitalSellingM365SeatSizeAbove25SeatsSalesProPropensityModel,
ActivateDigitalSellingD365SalesProPropensityActNowOrEvaluate,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseNavisionBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseAXFAndOPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseGreatPlainsBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseSolomonBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseOthersBCPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionFAndOPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionBCPropensityModel,
BuildAgileBusinessProcessesDynamicsOnPremInstallBaseAXGPSLNAVOtherD365PropensityModel,
BuildAgileBusinessProcessesDynamicsCompeteBaseMendixOutsystemsSalesforceD365PropensityModel,
BuildAgileBusinessProcessesD365FAndOInstallBase,BuildAgileBusinessProcessesD365BCInstallBase,
BuildAgileBusinessProcessesD365CEInstallBase,
BuildaResilientSupplyChainWinandActivateFirstD365WorkloadasD365SupplyChainwithNonOracleSAPERPCustomers,
BuildaResilientSupplyChainCrossSellD365SupplyChainANDORRetailCommercetoExistingD365CECustomers,
BuildaResilientSupplyChainCrossSellD365SupChainANDORRetailCommercetoD365CEANDOracleORSAP,D365BCCluster,
D365BCFit,D365BCIntent,D365FOCluster,D365FOFit,D365FOIntent,D365CECluster,D365CEFit,D365CEIntent,
DynamicsOnPremAXorCRM_HasOpenRenewal,M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASD365Propensity
```

## <a name="clas-m365-propensity"></a><span data-ttu-id="1c85a-161">CLAS M365 성향</span><span class="sxs-lookup"><span data-stu-id="1c85a-161">CLAS M365 propensity</span></span>

<span data-ttu-id="1c85a-162">6 개월 동안 CLASM365Propensity 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-162">CLASM365Propensity report for six months</span></span>

<span data-ttu-id="1c85a-163">쿼리 ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span><span class="sxs-lookup"><span data-stu-id="1c85a-163">Query ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-164">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-164">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,EnableRemoteWorkTargetExchangeOnline,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkHighPropensityProspectforM365ActNowEvaluate,EnableRemoteWorkCompeteZoomwithM365,
EnableRemoteWorkCompeteZoomwithoutM365,ReduceCostandManageM365E3targetedforM365E5,
ReduceCostandManageM365BBandBScustomerstargetedforM365BP,TransformOrganizationalProductivitySurfacePropensity,
M365Cluster,M365Fit,M365Intent,SurfaceCluster,SurfaceFit,SurfaceIntent,O365Cluster,O365Fit,O365Intent,
M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASM365Propensity
```

## <a name="teams-usage-3p-apps"></a><span data-ttu-id="1c85a-165">Teams 사용 3P 앱</span><span class="sxs-lookup"><span data-stu-id="1c85a-165">Teams Usage 3P Apps</span></span>

<span data-ttu-id="1c85a-166">6 개월 동안 TeamsUsage3PApps 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-166">TeamsUsage3PApps report for six months</span></span>

<span data-ttu-id="1c85a-167">쿼리 ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span><span class="sxs-lookup"><span data-stu-id="1c85a-167">Query ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-168">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-168">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,CustomerName,CustomerCountry,DateKey,AppName,UserCount 
FROM TeamsUsage3PApps TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-workload"></a><span data-ttu-id="1c85a-169">Teams 사용 작업</span><span class="sxs-lookup"><span data-stu-id="1c85a-169">Teams usage workload</span></span>

<span data-ttu-id="1c85a-170">6 개월 동안 TeamsUsageWorkload 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-170">TeamsUsageWorkload report for six months</span></span>

<span data-ttu-id="1c85a-171">쿼리 ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span><span class="sxs-lookup"><span data-stu-id="1c85a-171">Query ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-172">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-172">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,MonthKey,SubWorkload,DesktopUsers,WebUsers,MobileUsers,AllUpPartiticipants
FROM TeamsUsageWorkload TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-meetings-and-calls"></a><span data-ttu-id="1c85a-173">Teams 사용 회의 및 호출</span><span class="sxs-lookup"><span data-stu-id="1c85a-173">Teams usage meetings and calls</span></span>

<span data-ttu-id="1c85a-174">6 개월 동안 TeamsUsageMeetingsAndCalls 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-174">TeamsUsageMeetingsAndCalls report for six months</span></span>

<span data-ttu-id="1c85a-175">쿼리 ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span><span class="sxs-lookup"><span data-stu-id="1c85a-175">Query ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-176">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-176">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,DateKey,SubWorkload,MeetingCount,MeetingDuration 
FROM TeamsUsageMeetingsAndCalls TIMESPAN LAST_6_MONTHS
```

## <a name="competency-summary-history"></a><span data-ttu-id="1c85a-177">역량 요약 기록</span><span class="sxs-lookup"><span data-stu-id="1c85a-177">Competency summary history</span></span>

<span data-ttu-id="1c85a-178">6 개월 동안 CompetencySummaryHistory 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-178">CompetencySummaryHistory report for six months</span></span>

<span data-ttu-id="1c85a-179">쿼리 ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span><span class="sxs-lookup"><span data-stu-id="1c85a-179">Query ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-180">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-180">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyLevel,CompetencyStatus,CompetencyStartDate,CompetencyEndDate 
FROM CompetencySummaryHistory TIMESPAN LAST_6_MONTHS
```

## <a name="training-completion"></a><span data-ttu-id="1c85a-181">학습 완료</span><span class="sxs-lookup"><span data-stu-id="1c85a-181">Training completion</span></span>

<span data-ttu-id="1c85a-182">6 개월 동안의 학습 완료 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-182">Training Completions report for six months</span></span>

<span data-ttu-id="1c85a-183">쿼리 ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span><span class="sxs-lookup"><span data-stu-id="1c85a-183">Query ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-184">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-184">Report query</span></span>

```sql
SELECT TrainingActivityId,TrainingTitle,TrainingType,AADUserId,TrainingCompletionDate,Month,IcMCP,MCPID,MPNId,
PartnerName,PartnerCityLocation,PartnerCountryLocation 
FROM TrainingCompletions TIMESPAN LAST_6_MONTHS
```

## <a name="microsoft-learn"></a><span data-ttu-id="1c85a-185">Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="1c85a-185">Microsoft Learn</span></span>

<span data-ttu-id="1c85a-186">지난 6 개월 동안 Microsoft Learn 보고서</span><span class="sxs-lookup"><span data-stu-id="1c85a-186">Microsoft Learn report for the last six months</span></span>

<span data-ttu-id="1c85a-187">쿼리 ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span><span class="sxs-lookup"><span data-stu-id="1c85a-187">Query ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span></span>

### <a name="report-query"></a><span data-ttu-id="1c85a-188">보고서 쿼리</span><span class="sxs-lookup"><span data-stu-id="1c85a-188">Report query</span></span>

```sql
SELECT UserName,UserId,TrainingName,TrainingType,Products,Roles,CompletionDate,MPNId,PartnerName,CustomerMarket 
FROM MSLearn TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="1c85a-189">다음 단계</span><span class="sxs-lookup"><span data-stu-id="1c85a-189">Next steps</span></span>

- [<span data-ttu-id="1c85a-190">파트너 insights 분석 데이터에 액세스 하기 위한 Api</span><span class="sxs-lookup"><span data-stu-id="1c85a-190">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
- [<span data-ttu-id="1c85a-191">파트너 insights 분석 데이터에 액세스 하기 위한 샘플 응용 프로그램</span><span class="sxs-lookup"><span data-stu-id="1c85a-191">Sample application for accessing partner insights analytics data</span></span>](insights-programmatic-sample-application.md)