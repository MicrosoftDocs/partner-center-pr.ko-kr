---
title: Power BI 파트너 센터 Analytics 사용
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP의 직접 파트너를 위해 Power BI용 파트너 센터 분석 앱 사용하여 비즈니스 데이터를 보는 방법을 알아봅니다.
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855032"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="0f94d-103">Microsoft Power BI 파트너 센터 Analytics 앱을 사용하여 비즈니스 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="0f94d-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="0f94d-104">**적절한 역할:** 전역 관리자 | 사용자 관리 관리자 | 영업 에이전트 | 관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="0f94d-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="0f94d-105">비즈니스 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="0f94d-105">View your business data</span></span>

<span data-ttu-id="0f94d-106">다음을 포함하여 Power BI용 파트너 센터 분석 앱 비즈니스 데이터의 시각적 표현을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="0f94d-107">고객 기반, 구독 및 라이선스 증가</span><span class="sxs-lookup"><span data-stu-id="0f94d-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="0f94d-108">Office 365, Microsoft Dynamics 및 Microsoft Azure 제품 사용</span><span class="sxs-lookup"><span data-stu-id="0f94d-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="0f94d-109">지난 60일 동안 각 Azure 구독의 각 요금제 리소스에 대한 일일 사용 단위</span><span class="sxs-lookup"><span data-stu-id="0f94d-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="0f94d-110">예상 비용(최신 요금 카드 기준)</span><span class="sxs-lookup"><span data-stu-id="0f94d-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="0f94d-111">고객별을 포함하여 데이터 세트를 내보내고 사용자 지정 보고서를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="0f94d-112">파트너 센터 Analytics 앱 미리 보기 릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="0f94d-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="0f94d-113">이 앱은 클라우드 솔루션 공급자 프로그램의 직접 파트너를 위한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="0f94d-114">CSP의 다른 파트너(예: 간접 대리점)는 로그인할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="0f94d-115">예상 비용은 세전 청구/송장 데이터이며 법적 바인딩되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="0f94d-116">예상 비용은 데이터 인사이트에만 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="0f94d-117">고객 정보는 구독을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="0f94d-118">최근에 계정을 만들었지만 아직 구독이 없는 고객은 개수에 포함되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="0f94d-119">예상 비용은 CSP 가격 책정을 기반으로 하는 최신 요금 카드를 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="0f94d-120">일은 달력 일입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="0f94d-121">비즈니스 통찰력 보고서</span><span class="sxs-lookup"><span data-stu-id="0f94d-121">Business Insights report</span></span>

- <span data-ttu-id="0f94d-122">**고객 테 넌 트**: 구독을 구매한 고객의 고유 Azure AD 테 넌 트 수</span><span class="sxs-lookup"><span data-stu-id="0f94d-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="0f94d-123">**신규 (지난 30 일)**: 지난 30 일 동안 하나 이상의 구독을 구매 하는 신규 고객</span><span class="sxs-lookup"><span data-stu-id="0f94d-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="0f94d-124">**변동 (지난 30 일)**: "활성", "유예 기간" 또는 "사용 안 함" 구독이 없는 고객</span><span class="sxs-lookup"><span data-stu-id="0f94d-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="0f94d-125">**신규 (지난 24 시간)**: 지난 24 시간 동안 하나 이상의 구독을 구매 하는 신규 고객</span><span class="sxs-lookup"><span data-stu-id="0f94d-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="0f94d-126">**지난 12 개월 동안의 월별 예상 비용**: 매월 지난 12 개월 동안 매월 집계 된 예상 사전 세금 송장 달러의 추세</span><span class="sxs-lookup"><span data-stu-id="0f94d-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0f94d-127">**지난 12 개월 동안의 제품별 예상 비용**: 지난 12 개월 동안 집계 된 예정 된 세금 청구서 달러 금액을 기준으로 판매 되는 제품입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="0f94d-128">이 상태는 가장 많은 수익을 가져오는 상위 제품을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="0f94d-129">**지난 12 개월 동안의 고객**: 지난 12 개월 동안 매월 집계 된 새 고객 및 변동 고객의 월에 대 한 월간 추세</span><span class="sxs-lookup"><span data-stu-id="0f94d-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0f94d-130">**지난 12 개월 동안의 고객별 예상 비용**: 지난 12 개월 동안 집계 된 예상 사전 세금 청구서 달러 금액을 기준으로 하는 고객입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="0f94d-131">이 상태는 가장 많은 수익을 가져오는 상위 고객을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="0f94d-132">**제품별 고객 수**: 관련 고객과 함께 판매 되는 제품입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="0f94d-133">이 상태는 대부분의 고객에 게 판매 되는 인기 제품을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="0f94d-134">구독 정보 보고서</span><span class="sxs-lookup"><span data-stu-id="0f94d-134">Subscription Insights report</span></span>

- <span data-ttu-id="0f94d-135">**구독 상태**:</span><span class="sxs-lookup"><span data-stu-id="0f94d-135">**Subscription status**:</span></span>

- <span data-ttu-id="0f94d-136">활성: "활성" 또는 "유예" 상태에 속하는 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="0f94d-137">일시 중단 됨: "사용 안 함" 상태로 속한 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="0f94d-138">프로 비전 해제: "프로 비전 되지 않음" 또는 "만료 됨" 상태에 속하는 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="0f94d-139">**만료 상태**:</span><span class="sxs-lookup"><span data-stu-id="0f94d-139">**Expiry status**:</span></span>

  - <span data-ttu-id="0f94d-140">만료 됨: 이미 만료 된 구독 (구독 종료 날짜가 지났습니다.)</span><span class="sxs-lookup"><span data-stu-id="0f94d-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="0f94d-141">30일 후 만료: 30일 후에 만료되는 구독(구독 종료 날짜는 다음 30일 이후)</span><span class="sxs-lookup"><span data-stu-id="0f94d-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="0f94d-142">30일 이내에 만료: 다음 30일 내에 만료되는 구독(구독 종료 날짜는 오늘과 다음 30일 사이)</span><span class="sxs-lookup"><span data-stu-id="0f94d-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="0f94d-143">**총 구독:**"활성", "유예 중" 또는 "사용 안 함" 상태의 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="0f94d-144">**신규(지난 30일)**: 지난 30일 이내에 고객이 구매한 새 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="0f94d-145">**신규(지난 24시간)**: 지난 24시간 이내에 고객이 구매한 새 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="0f94d-146">**30일 이내에 만료: 다음 30일** 이내에 만료되는 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="0f94d-147">**변동(지난 30일)**: 지난 30일 이내에 프로비저닝이 해제되었거나 일시 중단(비활성화)된 구독</span><span class="sxs-lookup"><span data-stu-id="0f94d-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="0f94d-148">**구독 유형별 배포:** 라이선스 기반 및 사용량 기반 구독 유형별 총 구독의 % 분포</span><span class="sxs-lookup"><span data-stu-id="0f94d-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="0f94d-149">**제품별 활성 구독 수:** 활성 구독 수별로 정렬된 판매 제품</span><span class="sxs-lookup"><span data-stu-id="0f94d-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="0f94d-150">**지난 12개월 동안의 구독: 지난 12개월** 동안 매월 집계된 새 구독 및 변동 구독의 월별 추세</span><span class="sxs-lookup"><span data-stu-id="0f94d-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0f94d-151">**고객 구독 세부 정보:** 고객, 구독 및 제안에 대한 자세한 보기</span><span class="sxs-lookup"><span data-stu-id="0f94d-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="0f94d-152">라이선스 인사이트 보고서:</span><span class="sxs-lookup"><span data-stu-id="0f94d-152">License Insights report:</span></span>

- <span data-ttu-id="0f94d-153">**총 라이선스:** 모든 라이선스 기반 구독에서 집계된 총 라이선스 수</span><span class="sxs-lookup"><span data-stu-id="0f94d-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="0f94d-154">**신규(지난 30일)**: 지난 30일 이내에 라이선스 추가</span><span class="sxs-lookup"><span data-stu-id="0f94d-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="0f94d-155">**변동(지난 30일)**: 지난 30일 이내에 라이선스 감소</span><span class="sxs-lookup"><span data-stu-id="0f94d-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="0f94d-156">**신규(지난 24시간)**: 지난 24시간 이내에 라이선스 추가</span><span class="sxs-lookup"><span data-stu-id="0f94d-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="0f94d-157">**지난 90일 동안의 라이선스: 지난 90일** 동안 월별로 집계된 라이선스 추가 및 감소의 월별 추세</span><span class="sxs-lookup"><span data-stu-id="0f94d-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="0f94d-158">**제품별 활성 라이선스 수:** 판매된 제품이 활성 라이선스 수에 따라 정렬됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="0f94d-159">**고객별 활성 라이선스 수:** 활성 라이선스 수별로 정렬된 고객</span><span class="sxs-lookup"><span data-stu-id="0f94d-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="0f94d-160">**지난 90일 동안의 고객 라이선스 이벤트 세부 정보:** 이벤트 날짜, 이벤트 이름, 수량 및 수량 변경을 포함하여 고객, 구독 및 구독 이벤트에 대한 자세한 보기입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="0f94d-161">라이선스 사용량 보고서:</span><span class="sxs-lookup"><span data-stu-id="0f94d-161">Licenses Usage report:</span></span>

- <span data-ttu-id="0f94d-162">**제품별로 할당된 라이선스:** 판매된 제품이 라이선스 할당 횟수별로 정렬됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="0f94d-163">**제품에서 사용 중 라이선스:** 판매된 제품이 라이선스 사용 횟수별로 정렬되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="0f94d-164">**할당된 라이선스의 고객 배포:** 라이선스 할당 %에 따라 20% 범위의 버킷에서 손상되는 총 고객의 % 배포</span><span class="sxs-lookup"><span data-stu-id="0f94d-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="0f94d-165">**사용 중 라이선스의 고객 배포:** 라이선스 사용량 %에 따라 20% 범위의 버킷에서 손상되는 총 고객의 % 배포</span><span class="sxs-lookup"><span data-stu-id="0f94d-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="0f94d-166">**고객이 할당한 라이선스:** 판매된 라이선스 및 고객 및 제품에서 할당한 라이선스에 대한 자세한 보기</span><span class="sxs-lookup"><span data-stu-id="0f94d-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="0f94d-167">**고객이 사용 중 라이선스: 판매된** 라이선스 및 고객 및 제품에서 사용 중 라이선스에 대한 자세한 보기</span><span class="sxs-lookup"><span data-stu-id="0f94d-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="0f94d-168">Azure Insights 보고서:</span><span class="sxs-lookup"><span data-stu-id="0f94d-168">Azure Insights report:</span></span>

- <span data-ttu-id="0f94d-169">**지난 12개월 동안의 사용량 기반 고객: 지난 12개월** 동안 매월 집계된 신규 사용량 기반 고객 및 변동된 사용량 기반 고객의 월별 추세</span><span class="sxs-lookup"><span data-stu-id="0f94d-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0f94d-170">**지난 12개월 동안의 사용량 기반 구독: 지난 12개월** 동안 매월 집계된 새 사용량 기반 구독 및 변동된 사용량 기반 구독의 월별 추세</span><span class="sxs-lookup"><span data-stu-id="0f94d-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0f94d-171">**지난 60일 동안 고객별 예상 사용량 비용: 지난 60일** 동안 집계된 예상 세전 송장 달러 금액을 기준으로 정렬된 사용량 기반 고객입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="0f94d-172">이 상태는 가장 많은 수익을 가져오는 상위 사용량 기반 고객을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="0f94d-173">**지난 60일 동안 범주별 예상 사용량 비용: 지난 60일** 동안 집계된 예상 세전 송장 달러 금액을 기준으로 정렬된 사용량 기반 구독의 미터 범주입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="0f94d-174">**지난 60일 동안 구독별 예상 사용량 비용: 지난 60일** 동안 집계된 예상 세전 송장 달러 금액별 사용량 기반 구독입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="0f94d-175">**예산 지출 별 고객 예상 사용량 비용**: 고객의 현재 사용 지출 예산 백분율 (100%)을 기준으로 정렬 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="0f94d-176">Azure 리소스 사용 보고서:</span><span class="sxs-lookup"><span data-stu-id="0f94d-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="0f94d-177">**선택한 기간 동안 날짜별로 Azure 리소스 사용**: 지난 60 일 이내에 선택한 기간에 대 한 각 사용량 기반 구독에서 각 요금제 리소스의 일별 소비 단위입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="0f94d-178">**선택한 기간에 대 한 Azure 리소스의 예상 사용량 비용**: 지난 60 일 이내에 선택한 기간에 대 한 각 사용량 기반 구독에서 각 요금제 리소스에 대 한 최신 요금 카드를 기준으로 하는 예상 비용입니다.</span><span class="sxs-lookup"><span data-stu-id="0f94d-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0f94d-179">다음 단계</span><span class="sxs-lookup"><span data-stu-id="0f94d-179">Next steps</span></span>

- [<span data-ttu-id="0f94d-180">Power BI 앱에 대 한 파트너 센터 분석 개요</span><span class="sxs-lookup"><span data-stu-id="0f94d-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="0f94d-181">Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기</span><span class="sxs-lookup"><span data-stu-id="0f94d-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
