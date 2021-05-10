---
title: 인사이트 데이터 정의
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 문서에는 인사이트 다운로드 보고서 페이지에서 다운로드할 수 있는 다양한 보고서 및 해당 데이터 정의가 나열됩니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686350"
---
# <a name="export--data-definitions"></a>내보내기 – 데이터 정의 

**적절한 역할** 

- 보고서 뷰어
- 임원 보고서 뷰어

## <a name="introduction"></a>소개 

Insights 대시보드에서 보고서 다운로드 허브를 사용하여 원시 데이터 세트를 내보낼 수 있습니다. 

데이터 정의와 함께 다운로드할 수 있는 다양한 보고서가 다음 표에 나열되어 있습니다. 

### <a name="partner-profile-report"></a>**파트너 프로필 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPNId | MPN(Microsoft 파트너 네트워크 식별자) | 
| PartnerName | 파트너의 이름 | 
| PGA_MPNId | 파트너 글로벌 계정 MPN의 식별자 | 
| PGA_PartnerName | 파트너 글로벌 계정 이름 | 
| City | 파트너의 도시 위치 | 
| 국가 | 파트너의 국가 위치 | 
| HierarchyLevel | 전역 MPN ID인지 또는 위치 MPN ID인지를 나타냅니다. | 

### <a name="customer-details-report"></a>**고객 세부 정보 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerName | 고객의 이름 | 
| CustomerTenantId | 고객 테넌트 식별자 | 
| CustomerTpid | 고객 상위 상위의 식별자 | 
| CustomerSegment | 고객 부문 | 
| CustomerMarket | 고객의 지리적 시장 | 
| CustomerStatus | 고객 상태 (활성 또는 비활성) | 
| 제품 | MPN를 통해 고객에 게 판매 되는 제품: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI 또는 Microsoft Azure | 
| SKU | 제품 SKU | 
| 월 | 사용량 및 수익이 보고 되는 월 | 
| MPNId | Microsoft 파트너 네트워크의 식별자 | 
| PartnerName | 파트너의 이름입니다. | 
| 공동 배치 위치 | 파트너의 지리적 위치 | 
| PartnerAttributionType | 파트너의 특성 유형 | 
| SalesChannel | 판매 채널 | 
| 사용자의 좌석 | 사용 가능한 사용자 | 
| RevenueUSD | 미국 달러 수익 | 

### <a name="reseller-performance-report"></a>**Reseller performance report**

> [!Note]
> 수익 및 ACR 데이터는 경영진 보고서 뷰어인 사용자만 사용할 수 있습니다.

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| ResellerMPNid | Reseller Microsoft 파트너 네트워크 식별자 | 
| ResellerName | 재판매인 이름 | 
| ResellerMarket | Reseller country of market | 
| IndirectProviderMPNId | 간접 공급자 Microsoft 파트너 네트워크 식별자 | 
| IndirectProviderName | 간접 공급자 이름 | 
| 월 | 사용량 및 수익이 보고되는 월 | 
| 제품 | 제품 이름 | 
| 구독 ID | 구독 식별자 | 
| Available 사용사용자 | 사용 가능한 시트 수 | 
| AssignedSeats | 할당된 시트 수 | 
| BilledRevenueUSD | 청구된 수익(미국 달러) | 
| CustomerName | 고객의 이름 | 
| CustomerTPid | 고객 상위 상위의 식별자 | 
| CustomerSegment | 고객 부문 | 
| CustomerMarket | 고객의 지리적 시장 | 
| ResellerStatus | 대리점 상태 | 

### <a name="subscription-details-report"></a>**구독 정보 보고서**

>[!Note]
>수익 및 ACR 데이터는 임원 보고서 뷰어 인 사용자만 사용할 수 있습니다.

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| SubscriptionId | 구독의 GUID입니다. | 
| Subscription.subscriptionstartdate | 구독의 시작 날짜 | 
| Subscription.subscriptionenddate | 구독의 종료 날짜 | 
| SubscriptionState | 구독의 상태 (활성 또는 변동) | 
| 월 | 사용량 및 수익이 보고 되는 월 | 
| IsAutoRenew | 구독이 autorenew 여부를 나타냅니다 (예 또는 아니요). | 
| CustomerName | 고객 이름 | 
| CustomerTenantId | 고객의 GUID | 
| CustomerTpid | 고객 상위 부모 식별자 | 
| CustomerSegment | 고객의 시장 세그먼트 | 
| CustomerMarket | 고객의 지리적 시장 | 
| 제품 | 파트너가 고객에게 판매한 제품 | 
| SKU | 제품의 SKU | 
| MPNId | 파트너의 Microsoft 파트너 네트워크 ID | 
| PartnerName | 파트너의 이름 | 
| PartnerLocation | 파트너의 지리적 위치 | 
| PartnerAttributionType | 구독에 대한 특성 유형 | 
| SalesChannel | 판매 채널 - Direct, CSP(클라우드 솔루션 공급자) 등 | 
| Available 사용사용자 | 현재 사용 가능한 시트 | 
| RevenueUSD | 미국 달러의 수익 | 
| 등록 ID | 구독의 등록 ID | 

### <a name="azure-usage-report"></a>**Azure 사용량 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| SubscriptionId | 구독의 GUID입니다. | 
| Subscription.subscriptionstartdate | 구독 시작 날짜 | 
| Subscription.subscriptionenddate | 구독의 끝 날짜입니다. | 
| SubscriptionState | 구독의 현재 상태 (열기, 닫힘, 활성 또는 유예 기간) | 
| 월 | 월별로 집계 된 날짜 | 
| ServiceName | Azure 서비스의 이름입니다. | 
| MeterCategory | 미터 범주의 이름 | 
| UsageUnits | 청구 주기 중에 사용 되는 단위 수 | 
| CustomerName | 고객 이름 | 
| CustomerTenantId | 고객의 테 넌 트 ID | 
| CustomerTpid | 상위 상위 고객 ID | 
| CustomerSegment | 고객 세그먼트 | 
| CustomerMarket | 고객의 지리적 시장 | 
| MPNId | 고객의 Microsoft 파트너 네트워크 ID | 
| PartnerName | 파트너의 이름 | 
| PartnerLocation | 파트너의 지리적 국가 위치 | 
| PartnerAttributionType | 파트너의 특성 유형 | 
| SalesChannel | 판매 채널(Direct/CSP, Indirect/CSP, Direct 등) | 
| ACR_USD | ACR(Azure 소비 수익)(미국 달러) | 
| 등록 ID | Azure 구독의 등록 ID | 

### <a name="office-365-license-usage-report"></a>**Office 365 라이선스 사용 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테넌트 ID | 
| CustomerTpid | 고객 상위 부모 ID | 
| WorkloadName | 비즈니스용 Skype, 팀, Exchange Online | 
| 월 | 사용량이 보고 되는 월 | 
| Paid의 해당 단위 | 사용 가능한 유료 단위 수 | 
| MonthlyActiveUsers | 월간 활성 사용자 수 | 
| CustomerName | 고객 이름 | 
| CustomerMarket | 고객 시장의 지리적 국가 위치 | 
| CustomerSegment | 고객 부문 | 
| MPNId | Microsoft 파트너 네트워크의 식별자 | 
| PartnerName | 파트너의 이름입니다. | 
| 공동 배치 위치 | 파트너의 지리적 위치 | 
| PartnerAttributionType | 파트너의 특성 유형 | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility 라이선스 사용 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테 넌 트 ID | 
| CustomerTpid | 고객 상위 부모 ID | 
| WorkloadName | EMS(Enterprise Mobility + Security) 워크로드의 이름 | 
| 월 | 사용량이 보고되는 월 | 
| PayAvailableUnits | 사용 가능한 유료 단위 수 | 
| MonthlyActiveUsers | 월간 활성 사용자 수 | 
| CustomerName | 고객의 이름 | 
| CustomerMarket | 고객 시장의 지리적 국가 위치 | 
| CustomerSegment | 고객 세그먼트 | 
| MPNId | Microsoft 파트너 네트워크 식별자 | 
| PartnerName | 파트너의 이름 | 
| PartnerLocation | 파트너의 지리적 위치 | 
| PartnerAttributionType | 파트너의 특성 유형 | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 라이선스 사용 현황 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| SubscriptionId | 구독의 GUID입니다. | 
| Subscription.subscriptionstartdate | 구독의 시작 날짜 | 
| Subscription.subscriptionenddate | 구독의 종료 날짜 | 
| SubscriptionStatus | 구독의 상태 | 
| 월 | 사용량이 보고 되는 월 | 
| RevSumDivisionName | Rev 합계 나누기의 이름입니다. | 
| RevSumCategoryName | Rev 합계 범주의 이름 | 
| SKU | 제품의 SKU | 
| SKUId | 제품의 SKU ID | 
| FreeVsPaidSKU | 무료 또는 유료 SKU 인지 여부를 나타냅니다. | 
| SalesModel | 구독 판매에 사용 되는 판매 채널 | 
| DetailedSalesModel | 구독에 대한 자세한 판매 모델 | 
| CustomerName | 고객의 이름 | 
| CustomerTenantId | 고객 테넌트 GUID | 
| CustomerTpid | 고객 상위 부모 식별자 | 
| CustomerSegment | 고객의 시장 세그먼트 | 
| CustomerMarket | 고객의 지리적 시장 | 
| MPNId | Microsoft 파트너 네트워크 식별자 | 
| PartnerName | 파트너의 이름 | 
| PartnerLocation | 파트너의 지리적 국가 위치 | 
| PartnerAttachType | 구독에 대한 특성 유형 | 
| Available 사용사용자 | 현재 사용 가능한 시트 | 
| AssignedSeats | 현재 할당 된 사용자 | 
| ActiveSeats | 현재 활성 사용자 | 
| DeploymentOpportunity | 현재 배포 기회 | 
| ActiveUsagePercent | 현재 활성 사용 백분율 | 

### <a name="power-bi-license-usage-report"></a>**라이선스 사용 현황 보고서 Power BI**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| SubscriptionId | 구독의 GUID입니다. | 
| Subscription.subscriptionstartdate | 구독의 시작 날짜 | 
| Subscription.subscriptionenddate | 구독의 종료 날짜 | 
| SubscriptionStatus | 구독의 상태 (활성, 비활성 또는 유예 기간) | 
| 월 | 월별로 집계 된 날짜 | 
| SKU | 제품의 SKU | 
| SKUId | 제품의 SKU ID | 
| FreeVsPaidSKU | 무료 또는 유료 SKU 차이점 | 
| SalesModel | 구독을 판매하는 데 사용되는 판매 모델 | 
| DetailedSalesModel | 구독에 대한 자세한 판매 모델 | 
| CustomerName | 고객의 이름 | 
| CustomerTenantId | 고객 테넌트 GUID | 
| CustomerTpid | 고객 상위 부모의 식별자 | 
| CustomerSegment | 고객의 시장 세그먼트 | 
| CustomerMarket | 고객의 지리적 시장 | 
| MPNId | Microsoft 파트너 네트워크 식별자 | 
| PartnerName | 파트너의 이름 | 
| PartnerLocation | 파트너의 지리적 국가 위치 | 
| PartnerAttachType | 구독에 대한 특성 유형 | 
| Available 사용사용자 | 현재 사용 가능한 사용자 | 
| AssignedSeats | 현재 할당 된 사용자 | 
| ActiveSeats | 현재 활성 사용자 | 
| DeploymentOpportunity | 현재 배포 기회 | 
| ActiveUsagePercent | 현재 활성 사용 백분율 | 

### <a name="teams-meetings-and-calls-report"></a>**팀 모임 및 호출 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테 넌 트 ID | 
| CustomerTpid | 고객 상위 상위의 식별자 | 
| 월 | 사용량이 보고 되는 월 | 
| 하위 워크 로드 | 사용량이 보고 되는 하위 작업 (회의, 호출 또는 전화 시스템) | 
| 모임 수 | 모임 수 | 
| 모임 기간 | 총 모임 기간 (시) | 

### <a name="teams-monthly-usage-report"></a>**Teams 월별 사용 현황 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테넌트 ID | 
| CustomerTpid | 고객 상위 부모의 식별자 | 
| 월 | 사용량이 보고되는 월 | 
| 하위 워크로드 | 사용량이 보고되는 하위 워크로드(회의, 통화 또는 전화 시스템) | 
| 데스크톱 사용자 | 데스크톱에서 Teams를 사용하는 사용자 수 | 
| 모바일 사용자 | 모바일에서 Teams를 사용하는 사용자 수 | 
| 웹 사용자 | 웹에서 Teams를 사용하는 사용자 수 | 
| AllUpParticipants | 해당 월의 Teams 고유 사용자 수 | 

### <a name="teams-usage-3p-apps-report"></a>**Teams 사용량 3P 앱 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테넌트 ID | 
| CustomerTpid | 고객 상위 부모 ID | 
| 월 | 사용량이 보고되는 월 | 
| 3P 앱 이름 | 팀 앱 이름 | 
| 사용자 수 | 앱에 대 한 사용자 수 | 


### <a name="training-details-report"></a>**학습 세부 정보 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| TrainingActivityId | 교육의 식별자 | 
| TrainingTitle | 학습 제목 | 
| TrainingType | 교육 유형 (인증 또는 시험) | 
| IndividualFirstName | 고객의 이름 | 
| IndividualLastName | 고객의 성 | 
| 메일 | 고객의 개인 전자 메일 ID | 
| CorpEmail | 고객의 Office 전자 메일 ID | 
| TrainingCompletionDate | 학습 완료 날짜 | 
| 월 | 데이터가 보고 되는 월 | 
| IcMCP | 사용자가 MCP(Microsoft Certified Professional)인지 여부를 나타냅니다. | 
| MCPID | 사용자의 MCP ID | 
| MPNId | Microsoft 파트너 네트워크 식별자 | 
| PartnerName | 파트너의 이름 | 
| PartnerCityLocation | 파트너의 지리적 도시 위치 | 
| PartnerCountryLocation | 파트너의 지리적 국가 위치 | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| UserName | 사용자의 이름 | 
| UserId | 사용자의 GUID | 
| TrainingName | 학습 이름 | 
| TrainingType | 학습 유형(모듈 또는 학습 경로) | 
| 제품 | 학습 모듈을 적용할 수 있는 제품 | 
| 역할 | 교육의 적용 가능한 역할 | 
| CompletionDate | 학습 완료 날짜 | 
| MPNId | Microsoft 파트너 네트워크의 식별자 | 
| PartnerName | 파트너의 이름입니다. | 
| 국가 | 파트너의 지리적 국가 위치 | 

### <a name="competency-summary-and-history-report"></a>**역량 요약 및 기록 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CompetencyName | 역량의 이름 | 
| CompetencyLevel | 역량 수준 (골드 또는 실버) | 
| CompetencyStatus | 역량의 현재 상태 (활성, 비활성 또는 유예 기간) | 
| CompetencyStartDate | 역량의 시작 날짜 | 
| CompetencyEndDate | 역량의 종료 날짜 | 

### <a name="competency-performance-report"></a>**역량 성능 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CompetencyName | 역량의 이름 | 
| CompetencyAttainmentOptionName | 역량 획득 옵션의 이름 | 
| 월 | 메트릭이 보고되는 월 | 
| MetricName | 역량과 관련된 메트릭의 이름 | 
| MetricMonthlyContribution | 메트릭의 월간 기여도 | 
| TTMAggregate | 후행 12개월에 대한 집계 메트릭 | 
| AnniversaryYearAggregate | 현재 1주년 집계 메트릭 | 
| GoldThreshold | 골드 역량을 충족하기 위한 성능 요구 사항 | 
| SilverThreshold | 실버 역량을 충족하기 위한 성능 요구 사항 | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**클라우드 상승 - Microsoft 365 전파 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 파트너 네트워크 ID | 
| 파트너 이름 | 파트너의 이름 | 
| 고객 ID | 고객의 식별자 번호 | 
| 2018년 3월 1 | Propensity에 대한 점수가 매겨진 고객의 & Bradstreet(D&B) 번호 | 
| 계정 이름 | 계정 이름 | 
| 도메인 | 계정의 도메인 | 
| 조직 크기 | 조직의 규모 | 
| 업종 | 조직이 속한 업계 | 
| Vertical | Microsoft, D&B 및 기타 산업 표준에 의해 식별 되는 성향에 대해 점수가 매겨진 고객의 세로 | 
| 영역 | 위치의 지리적 영역 | 
| 자회사 | 성향에 대해 점수가 매겨진 고객의 자회사 | 
| Sales Territory | 성향에 대해 점수가 매겨진 고객의 판매 지역 | 
| City | 조직의 지리적 도시 위치 | 
| 시스템 상태 | 조직의 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 조직의 지리적 국가 위치 | 
| Segment | 시장 부문 | 
| 하위 세그먼트 | 시장 subsegment | 
| SMC 유형 요약 | SMC 유형 | 
| 상위 관리 되지 않는 계산 기준 | 상위 관리 되지 않는 고객-계산 | 
| 상위 관리 되지 않는 사용자 기반 | 관리되지 않는 상위 고객 - 사용자 | 
| IsNonProfit | 조직이 비영리 조직인지 여부를 나타냅니다(예 또는 아니요). | 
| 원격 작업 사용 - 대상 Exchange Online | 활성 Exchange Online 구독이 있는 고객, Microsoft 365 | 
| 원격 작업 사용 - 클라우드 Ascent propensity를 사용하여 온-프레미스 취득(현재 버전) - +10개 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트가 있는 고객입니다. 즉, 클라이언트 버전은 EOL(수명 종료) 버전보다 늦습니다. 고객에게 10개 이상의 라이선스가 있습니다. 전파 점수가 있는 고객입니다. 파트너는 Microsoft 365 변환을 대상으로 해야 합니다. | 
| 클라우드 Ascent propensity를 사용하여 원격 작업 - 온-프레미스 취득(현재 버전) 사용 - <10개 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트(즉, EOL 이후 버전)가 있는 고객입니다. 고객에게 10개 미만의 라이선스가 있습니다. 전파 점수가 있는 고객입니다. 파트너는 Microsoft 365 변환을 대상으로 해야 합니다. | 
| 원격 작업 사용 - 클라우드 Ascent propensity 없이 온-프레미스 취득(현재 버전) - +10개의 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트(즉, EOL 이후 버전)가 있는 고객입니다. 고객에게 10개 이상의 라이선스가 있습니다. 고객에게는 전파 점수가 없습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향을 사용 하지 않고 원격 작업-온-프레미스 취득 (현재 버전) 사용-<10 개 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 이후 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향-+ 10 라이선스를 사용 하 여 원격 작업-온-프레미스 획득 (EOL 버전) 사용 | EOL 온-프레미스 Office 또는 Windows 클라이언트 (즉, EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향를 사용 하 여 원격 작업-온-프레미스 획득 (EOL 버전) 사용-<10 라이선스 | EOL 온-프레미스 Office 또는 Windows 클라이언트 (즉, EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향 없이 원격 작업-온-프레미스 획득 (EOL 버전) 사용-+ 10 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Microsoft 365 변환을 대상으로 해야 합니다. | 
| 클라우드 Ascent propensity 없이 원격 작업 - 온-프레미스 취득(EOL 버전) 사용 - <10개의 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트(즉, EOL 버전 이하)가 있는 고객입니다. 고객에게 10개 미만의 라이선스가 있습니다. 고객에게는 전파 점수가 없습니다. 파트너는 Microsoft 365 변환을 대상으로 해야 합니다. | 
| 원격 작업 사용 - Microsoft 365 대한 높은 전파 가능성(Act NowithEvaluate) | Microsoft 365 대한 높은 전파를 가진 잠재 고객 | 
| 원격 작업 사용 - Microsoft 365 사용하여 경쟁(확대/축소) | Zoom 및 Microsoft 365 있는 고객, Teams로의 전환 대상 | 
| 원격 작업 사용 - Microsoft 365 없이 경쟁(확대/축소) | Zoom이 있는 고객, Teams로 변환 대상 | 
| 비용 절감 및 관리 - Microsoft 365 E5를 대상으로 하는 E3 Microsoft 365 | Microsoft 365 E3의 기존 고객, Microsoft 365 E5 대상 | 
| 비용 절감 및 관리 - Microsoft 365 Business Premium을 대상으로 하는 Business Basic 및 Business Standard 고객 Microsoft 365 | Microsoft 365 Business Premium을 대상으로 하는 기존 Microsoft 365 Business Basic 및 Business Standard 고객 | 
| 조직 생산성 변환 - 표면적 전파 | 고객에게 Surface에 대한 전파를 표시합니다. | 
| M365Cluster | 구매 Microsoft 365 대한 고객의 성향을 식별합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 현재 작업을 수행한 후에도 여전히 용량이 있는 경우에만 키우십시오를 대상으로 지정 하 고 고객을 대상으로 평가 합니다. | 
| M365Fit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 가장 작은 Smb (중소기업)로 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적 적합성 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| M365Intent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| SurfaceCluster | 맞춤 및 의도 권장 사항을 클러스터로 통합 하 여 Surface를 구매할 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 현재 작업을 수행한 후에도 여전히 용량이 있는 경우에만 키우십시오를 대상으로 지정 하 고 고객을 대상으로 평가 합니다. | 
| SurfaceFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| SurfaceIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 채점은 맞춤에 오버레이되어 클러스터를 정의합니다. 의도 점수 매기기는 매월 업데이트됩니다. | 
| O365Cluster | Office 365 구매에 대한 고객의 성향을 식별합니다. 더 높은 수율을 생성하므로 지금 작동 및 평가 클러스터를 대상으로 지정합니다. 지금 행동 및 고객 평가가 대상으로 지정된 후에 용량이 아직 있는 경우에만 고객에 대한 대상을 지정하고 고객을 교육합니다. | 
| O365Fit | 펌그래픽을 정의하는 내부 및 외부 데이터 포인트입니다. 점수 매기기 맞춤은 최상의 SMB에 유사 모델을 사용하여 고객을 비교하고 고객이 Microsoft 클라우드 제품에 적합한지 여부를 확인합니다. 맞춤 점수 매기기는 분기별로 업데이트됩니다. | 
| O365Intent | 소셜 미디어 및 고객의 온라인 동작과 관련된 신호는 의도를 정의합니다. 의도 채점은 클러스터를 정의하기 위해 Fit에 오버레이됩니다. 의도 점수 매기기는 매월 업데이트됩니다. | 
| M365UpsellCustomer | 고객이 Microsoft 365 대한 업셀 전파를 표시하는지 여부를 식별합니다. | 
| Google이 있습니다. | 고객이 Google 제품을 소유하기 위한 경쟁 신호를 표시하는지 여부를 식별합니다. | 
| AWS가 있습니다. | 고객이 AWS(Amazon Web Services) 제품을 소유하기 위한 경쟁 신호를 표시하는지 여부를 식별합니다. | 
| EA 있음 | 갱신이 EA (기업 계약) 인지 EA 구독 인지를 식별 합니다. | 
| 열림 | 갱신이 오픈 또는 오픈 값 계약 인지 여부를 식별 합니다. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**클라우드 어센더-Dynamics 365 성향 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 파트너 네트워크 ID | 
| 파트너 이름 | 파트너의 이름입니다. | 
| 고객 ID | 고객 식별자 번호 | 
| DUNS 번호 | 성향에 대해 점수가 매겨진 고객의 & Bradstreet 수 | 
| 계정 이름 | 계정 이름 | 
| 도메인 | 계정의 도메인 | 
| 조직 크기 | 조직의 규모 | 
| 업종 | 조직이 속한 업계 | 
| Vertical | Microsoft, D&B 및 기타 산업 표준에 의해 식별 되는 성향에 대해 점수가 매겨진 고객의 세로
| 영역 | 위치의 지리적 영역 | 
| 자회사 | 성향에 대해 점수가 매겨진 고객의 자회사 | 
| Sales Territory | 성향에 대해 점수가 매겨진 고객의 판매 지역 | 
| City | 지리적 위치 | 
| 시스템 상태 | 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 지리적 국가 위치 | 
| Segment | 시장 세그먼트 | 
| 하위 세그먼트 | 시장 하위 | 
| SMC 유형 요약 | 고객 분류: 상위 관리되지 않는 사용자 기반은 직원 수가 300명 이상인 고객이고, 관리되지 않는 상위 컴퓨팅 기반은 Azure 3년 잠재 고객이 USD10,000이고, 중간 규모 기업은 직원 수가 25명 이상인 고객이고, 중소기업은 직원 수가 25명 미만인 고객입니다. | 
| Top Unmanaged - Compute Base | 관리되지 않는 상위 고객 - 컴퓨팅 | 
| 상위 관리되지 않는 - 사용자 기반 | 관리되지 않는 상위 고객 - 사용자 | 
| IsNonProfit | 조직이 비영리 조직인지 여부를 나타냅니다(예 또는 아니요). | 
| 디지털 판매 활성화 - Microsoft 365 - 시트 크기 >= 25명(SalesPro propensity 모델) | Dynamics 365가 없는 고객 시트 크기: 25 이상. 파트너는 Dynamics 365 SalesPro의 교차 판매를 대상으로 해야 합니다. | 
| 디지털 판매 활성화 - Dynamics 365 SalesPro propensity(지금 작동 또는 평가) | Dynamics 365가 없는 고가용성 고객. 파트너는 Dynamics 365 SalesPro을 대상으로 해야 합니다. | 
| Navision에 대 한 금융 & 위험 관리-Dynamics 온-프레미스 설치 기본-(Business Central 성향 model) | 온-프레미스 Navision를 사용 하는 기존 고객. 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| 금융 위험 관리 & 사기 행위 온-프레미스 설치 기본-Dynamics AX (Dynamics 365 재무 + Operations 성향 model) | 온-프레미스 AX를 사용 하는 기존 고객 파트너는 Dynamics 365 재무 + 작업을 대상으로 해야 합니다. | 
| 사기 행위 & 사기 행위 관리-Dynamics 온-프레미스 설치 기본-뛰어난 Plains (Business Central 성향 모델) | 온-프레미스에서 좋은 Plains 있는 기존 고객. 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| 사기 행위 & 사기 행위 관리-Dynamics 온-프레미스 설치 기반-솔로몬 (Business Central 성향 모델) | 온-프레미스를 사용 하는 기존 고객 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| & 사기 행위 관리-Dynamics 온-프레미스 설치 기본-기타 (Business Central 성향 model) | 이전에 나열 되지 않은 다른 온-프레미스 솔루션을 사용 하는 기존 고객 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| Agile 비즈니스 프로세스 빌드-Dynamics 온-프레미스 설치 base-AX/GP/SL/NAV/Other (Dynamics 365 성향 model) | Agile 비즈니스 프로세스 빌드-Dynamics 온-프레미스 설치 base-AX/GP/SL/NAV/Other (Dynamics 365 성향 model) | 
| Agile 비즈니스 프로세스 빌드-Dynamics 경합 베이스-Mendix/OutSystems/Salesforce (Dynamics 365 성향 model) | Agile 비즈니스 프로세스 빌드-Dynamics 경합 베이스-Mendix/OutSystems/Salesforce (Dynamics 365 성향 model) | 
| Agile 비즈니스 프로세스 빌드 - Dynamics 365 Finance + Operations install base | 기존 Dynamics 365 Finance + Operations 고객. Power Apps 대상으로 지정할 파트너입니다. | 
| Agile 비즈니스 프로세스 빌드 - Dynamics 365 Business Central 설치 기준 | 기존 Dynamics 365 Business Central 고객. Power Apps 대상으로 지정할 파트너입니다. | 
| Agile 비즈니스 프로세스 빌드 - Dynamics 365 Customer Engagement 설치 기준 | 기존 Dynamics 365 Customer Engagement 고객. Power Apps 대상으로 지정할 파트너입니다. | 
| 복원력 있는 공급망 빌드 - Windows 및 비 Oracle 또는 SAP ERP(엔터프라이즈 리소스 계획) 고객을 통해 Dynamics 365 Supply Chain Management로 첫 번째 Dynamics 365 워크로드 활성화 | Dynamics 365 Supply Chain Management를 위한 대상 고객 | 
| 복원력 있는 공급망 빌드 - Dynamics 365 Supply Chain Management 및/또는 소매 또는 상거래를 기존 Dynamics 365 Customer Engagement 고객에게 교차 판매 | 교차 판매 Dynamics 365 Supply Chain Management를 대상으로 하는 기존 Dynamics 365 Customer Engagement 고객 | 
| 복원력 있는 공급망 빌드 - Dynamics 365 Supply Chain Management 및/또는 소매 또는 상거래를 Dynamics 365 Customer Engagement 및 Oracle 또는 SAP에 교차 판매 | Dynamics 365 Supply Chain Management를 대상으로 하는 Oracle 또는 SAP를 보유한 기존 Dynamics 365 Customer Engagement 고객 | 
| D365BCCluster | Dynamics 365 Business Central 구매에 대한 고객의 성향을 식별합니다. Business Central에 대한 선호도를 표시하는 고객은 중소형 범주에 있습니다. 지금 작동을 대상으로 지정하고 클러스터를 평가합니다. 더 높은 수율을 생성하기 때문입니다. 지금 행동 및 고객 평가 대상을 지정한 후에도 용량이 여전히 있는 경우에만 고객에 대한 대상을 지정하고 고객을 교육합니다. | 
| D365BCFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| D365BCIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| D365FOCluster | Dynamics 365 재무 및 운영을 구매 하는 고객의 성향을 식별 합니다. 재무 + 작업에 대해 성향를 표시 하는 고객은 관리 되지 않는 상위 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365FOFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| D365FOIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트됩니다. | 
| D365CECluster | Dynamics 365 Customer Engagement 구매에 대한 고객의 성향을 식별합니다. 고객 참여에 대한 선호도를 표시하는 고객은 중소형 범주에 있습니다. 지금 작동을 대상으로 지정하고 클러스터를 평가합니다. 더 높은 수율을 생성하기 때문입니다. 지금 행동 및 고객 평가 대상을 지정한 후에도 용량이 여전히 있는 경우에만 고객에 대한 대상을 지정하고 고객을 교육합니다. | 
| D365CEFit | Dynamics 365 Customer Engagement에 적합함을 나타냅니다. | 
| D365CEIntent | Dynamics 365 Customer Engagement에 대한 의도를 나타냅니다. | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | 고객에게 Dynamics 온-프레미스 AX 또는 CRM에 대한 개방형 갱신이 있는지 여부를 식별합니다. | 
| M365UpsellCustomer | 고객이 Microsoft 365 대한 업셀 전파를 표시하는지 여부를 식별합니다. | 
| Google이 있습니다. | 고객이 Google 제품을 소유하기 위한 경쟁 신호를 표시하는지 여부를 식별합니다. | 
| AWS가 있습니다. | 고객이 AWS 제품을 소유하기 위한 경쟁 신호를 표시하는지 여부를 식별합니다. | 
| EA가 있습니다. | 갱신이 EA 또는 EA 구독인지 여부를 식별합니다. | 
| 열림 | 갱신이 오픈 또는 오픈 값 계약 인지 여부를 식별 합니다. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**클라우드 어센더-Azure 성향 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 파트너 네트워크 ID | 
| 파트너 이름 | 파트너의 이름입니다. | 
| 고객 ID | 고객 식별자 번호 | 
| DUNS 번호 | 성향에 대해 점수가 매겨진 고객의 & Bradstreet 수 | 
| 계정 이름 | 계정 이름 | 
| 도메인 | 계정의 도메인 | 
| 조직 크기 | 조직의 규모 | 
| 업종 | 업종 | 
| Vertical | Microsoft, D&B 및 기타 산업 표준에 의해 식별 되는 성향에 대해 점수가 매겨진 고객의 세로 | 
| 영역 | 위치의 지리적 영역 | 
| 자회사 | 성향에 대해 점수가 매겨진 고객의 자회사 | 
| Sales Territory | 성향에 대해 점수가 매겨진 고객의 판매 지역 | 
| City | 지리적 위치 | 
| 시스템 상태 | 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 지리적 국가 위치 | 
| Segment | 시장 세그먼트 | 
| 하위 세그먼트 | 시장 하위 | 
| SMC 유형 요약 | SMC 유형 | 
| Top Unmanaged - Compute Base | 관리되지 않는 상위 고객 - 컴퓨팅 | 
| 상위 관리되지 않는 - 사용자 기반 | 관리되지 않는 상위 고객 - 사용자 | 
| IsNonProfit | 조직이 비영리 조직인지 여부를 나타냅니다(예 또는 아니요). | 
| 마이그레이션 - EOL Windows Server - 클라우드 Ascent propensity를 사용하는 EOL Windows Server IB - 5개 이상의 라이선스 | EOL 온-프레미스 Windows Server(즉, EOL 버전 이하)가 있는 고객입니다. 고객에게 5개 이상의 라이선스가 있습니다. 전파 점수가 있는 고객입니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - EOL Windows Server - 클라우드 Ascent propensity를 사용하는 EOL Windows Server IB - <5개 라이선스 | EOL 온-프레미스 Windows Server(즉, EOL 버전 이하)가 있는 고객입니다. 고객에게 5개 미만의 라이선스가 있습니다. 전파 점수가 있는 고객입니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL Windows Server-클라우드 어센더 성향 없이 IB Windows Server + 라이선스 | EOL 온-프레미스 Windows Server (즉, EOL 버전 또는 그 이전 버전)가 있는 고객입니다. 고객이 라이선스를 5 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL Windows Server IB 클라우드 <성향이 없는 Windows Server 5 개 라이선스 | EOL 온-프레미스 Windows Server (즉, EOL 버전 또는 그 이전 버전)가 있는 고객입니다. 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL SQL-EOL SQL Server IB 클라우드 어센더 성향-5 + 라이선스 | EOL 온-프레미스 SQL Server (즉, EOL 버전 또는 이전 버전)을 보유 하 고 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| IB 클라우드 <성향를 사용 하 여 마이그레이션-EOL SQL-EOL SQL Server 5 개 라이선스 | EOL 온-프레미스 SQL Server (즉, EOL 버전 또는 이전 버전)을 보유 하 고 있는 고객입니다. 라이선스가 5 개 미만입니다. 점수가 성향 고객입니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - EOL SQL - 클라우드 상승 전파가 없는 EOL SQL Server IB - 5개 이상의 라이선스 | EOL 온-프레미스 SQL Server(즉, EOL 버전 이하)가 있는 고객입니다. 고객에게 5개 이상의 라이선스가 있습니다. 고객에게는 전파 점수가 없습니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - EOL SQL - Cloud Ascent propensity가 없는 EOL SQL Server IB - <5개 라이선스 | EOL 온-프레미스 SQL Server(즉, EOL 버전 이하)가 있는 고객입니다. 고객에게 5개 미만의 라이선스가 있습니다. 고객에게는 전파 점수가 없습니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - 온-프레미스 Windows Server 마이그레이션 - 클라우드 Ascent propensity를 사용하는 현재 Windows Server IB - 5개 이상의 라이선스 | 현재 온-프레미스 Windows Server(즉, EOL 이후 버전)가 있는 고객입니다. 고객에게 5개 이상의 라이선스가 있습니다. 고객에게는 전파 점수가 있습니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - 온-프레미스 Windows Server 마이그레이션 - 클라우드 Ascent propensity를 사용하여 현재 Windows Server IB - <5개 라이선스 | 현재 온-프레미스 Windows Server(즉, EOL 이후 버전)가 있는 고객입니다. 고객에게 5개 미만의 라이선스가 있습니다. 고객에게 Azure에 대한 전파 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-온-프레미스 Windows Server 마이그레이션-클라우드 어센더 성향 없는 현재 Windows Server IB + 라이선스 | 현재 온-프레미스 Windows Server가 있는 고객 (EOL 이후의 버전)입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-온-프레미스 Windows Server 마이그레이션-클라우드 성향 없이 현재 Windows Server IB-<5 개 라이선스 | 현재 온-프레미스 Windows Server가 있는 고객 (EOL 이후의 버전)입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Azure SQL 또는 SQL Vm (가상 머신)으로 마이그레이션-성향 IB 이상 라이선스를 사용 하 여 현재 SQL Server | 현재 온-프레미스 SQL Server (즉, EOL 이후 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-Cloud 성향를 사용 하 여 현재 SQL Server IB-<5 개 라이선스 | 현재 온-프레미스 SQL Server (즉, EOL 이후 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게는 성향 점수가 있습니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - Azure SQL 또는 SQL VM으로 마이그레이션 - Cloud Ascent propensity 없이 현재 SQL Server IB - 5개 이상의 라이선스 | 현재 온-프레미스 SQL Server 있는 고객(즉, EOL 이후 버전). 고객에게 5개 이상의 라이선스가 있습니다. 고객에게는 전파 점수가 없습니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - Azure SQL 또는 SQL VM으로 마이그레이션 - Cloud Ascent propensity 없이 현재 SQL Server IB - <5개의 라이선스 | 현재 온-프레미스 SQL Server 있는 고객(즉, EOL 이후 버전). 고객에게 5개 미만의 라이선스가 있습니다. 고객에게는 전파 점수가 없습니다. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - OSS - OSS(오픈 소스 익스피리소스) DB로 마이그레이션 | 다음 경쟁 제품 중 하나를 가진 기존 고객: PostgreSQL, MySQL, MariaDB. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - OSS - Azure의 Linux | Linux를 이용한 기존 고객. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션 - SAP - Azure의 SAP | SAP를 이용한 기존 고객. 파트너는 이 고객을 대상으로 Azure로 마이그레이션해야 합니다. | 
| 마이그레이션-Windows 가상 데스크톱-원격 데스크톱 서비스 IB | 활성 Windows 원격 데스크톱 서비스 고객을 식별 합니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Windows 가상 데스크톱-최신 작업을 Azure/WVD로 교차 판매 | Microsoft 365 있는 고객을 식별 하 고 Azure를 사용 하지 않습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-VMware IB | 제품이 있는 기존 고객: VMware. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Citrix IB | 제품을 포함 하는 기존 고객: Citrix Systems. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 혁신적인 분석-Azure 성향를 사용 하는 Power BI IB | 및 활성 Power BI 구독을 포함 하는 고객: Power BI 독립 실행형 Pro, Power BI-Azure 제품군, Power BI Office 제품군, Power BI 제품군-Microsoft 365 | 
| GitHub를 사용 하 여 DevOps 사용-Visual Studio/MSDN IB | 활성 Visual Studio 버전을 사용 하는 고객 식별 | 
| Windows Server Standard 버전 | 고객의 Windows Server Standard 구매 버전을 표시 합니다. | 
| Windows Server Standard 라이선스 | 고객의 Windows Server Standard 구매 라이선스 유형을 표시 합니다. | 
| Windows Server Data Center 버전 | 고객이 구매한 Windows Data Center 버전을 표시합니다. | 
| Windows Server Data Center 라이선스 | 고객이 구매한 Windows Data Center의 라이선스 유형을 표시합니다. | 
| AzureFit | 펌그래픽을 정의하는 내부 및 외부 데이터 포인트입니다. 점수 매기기 맞춤은 가장 적합한 SMB에 유사 모델을 사용하여 고객을 비교하고 고객이 Microsoft 클라우드 제품에 적합한지 여부를 확인합니다. 맞춤 점수 매기기는 분기별로 업데이트됩니다. | 
| AzureIntent | 소셜 미디어 및 고객의 온라인 동작과 관련된 신호는 의도를 정의합니다. 의도 채점은 맞춤에 오버레이되어 클러스터를 정의합니다. 의도 점수 매기기는 매월 업데이트됩니다. | 
| AzureCluster | 맞춤 및 의도 권장 사항을 클러스터에 통합하여 Azure를 구매하는 고객의 성향을 식별합니다. 지금 작동을 대상으로 지정하고 클러스터를 평가합니다. 더 높은 수율을 생성하기 때문입니다. 지금 행동 및 고객 평가 대상을 지정한 후에도 용량이 여전히 있는 경우에만 고객에 대한 대상을 지정하고 고객을 교육합니다. | 
| WindowsServerDataCenter_HasOpenRenewal | 고객에게 Windows Server Datacenter에 대한 공개 갱신이 있는지 여부를 식별합니다. | 
| WindowsServerStandard_HasOpenRenewal | 고객에게 Windows Server Standard에 대한 공개 갱신이 있는지 여부를 식별합니다. | 
| AzureUpsellCustomer | 고객이 Azure에 대 한 상향 판매 성향를 표시 하는지 여부를 식별 합니다. | 
| Google 포함 | 고객이 소유 하 고 있는 Google 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| AWS | 고객이 소유 하는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| EA 있음 | 갱신이 EA 또는 EA 구독 인지 여부를 식별 합니다. | 
| 열림 | 갱신이 오픈 또는 오픈 값 계약 인지 여부를 식별 합니다. | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**클라우드 어센더-규약 갱신 성향 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 파트너 네트워크 ID | 
| 파트너 이름 | 파트너의 이름입니다. | 
| 고객 ID | 고객 식별자 번호 | 
| DUNS 번호 | 성향에 대해 점수가 매겨진 고객의 & Bradstreet 수 | 
| 계정 이름 | 계정 이름 | 
| 도메인 | 계정의 도메인 | 
| 조직 크기 | 조직의 규모 | 
| 업종 | 업종 | 
| Vertical | Microsoft, D&B 및 기타 산업 표준으로 식별된 대로 전파 점수가 매여지는 고객의 수직 | 
| 영역 | 위치의 지리적 영역 | 
| 자회사 | 전파 점수가 매여지는 고객의 자회사 | 
| Sales Territory | 전파 점수가 매해지는 고객의 판매 지역 | 
| City | 지리적 도시 위치 | 
| 시스템 상태 | 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 지리적 국가 위치 | 
| Segment | 시장 세그먼트 | 
| 하위 세그먼트 | 시장 하위 | 
| SMC 유형 요약 | SMC 유형 | 
| Top Unmanaged - Compute Base | 관리되지 않는 상위 고객 - 컴퓨팅 | 
| 상위 관리되지 않는 - 사용자 기반 | 관리되지 않는 상위 고객 - 사용자 | 
| IsNonProfit | 조직이 비영리 조직인지 여부를 나타냅니다(예 또는 아니요). | 
| Google이 있습니다. | 고객이 소유 하는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| AWS | 고객이 소유 하는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| Azure 클러스터 | Azure를 구매 하는 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365 재무 + 운영 클러스터 | Dynamics 365 재무 및 운영을 구매 하는 고객의 성향을 식별 합니다. 재무 + 작업에 대해 성향를 표시 하는 고객은 관리 되지 않는 상위 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365 CE 클러스터 | Dynamics 365 고객 참여를 구매 하는 고객의 성향을 식별 합니다. 고객 Engagement에 대 한 성향를 표시 하는 고객은 중간 및 작은 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365 BC 클러스터 | Dynamics 365 비즈니스 중부를 구매 하는 고객의 성향을 식별 합니다. 성향 for Business Central을 표시 하는 고객은 중간 및 작은 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 지금 행동 및 고객 평가 대상을 지정한 후에도 용량이 여전히 있는 경우에만 고객에 대한 대상을 지정하고 고객을 교육합니다. | 
| Microsoft 365 클러스터 | 구매 Microsoft 365 고객의 전파를 식별합니다. 지금 작동을 대상으로 지정하고 클러스터를 평가합니다. 더 높은 수율을 생성하기 때문입니다. 지금 행동 및 고객 평가 대상을 지정한 후에도 용량이 여전히 있는 경우에만 고객에 대한 대상을 지정하고 고객을 교육합니다. | 
| 라이선스 프로그램 | 갱신에 대한 라이선스 프로그램 유형을 식별합니다. | 
| 규약 ID | 규약의 식별자 | 
| 계약 종료 날짜 | 계약의 종료 날짜 | 
| 만료 유형 | 만료 유형 | 
| 만료 수익 | 만료 구독과 관련된 수익 | 
| EA가 있습니다. | 갱신이 EA 또는 EA 구독인지 여부를 식별합니다. | 
| 열려 있습니다. | 갱신이 Open 또는 Open Value 계약인지 여부를 식별합니다. | 
| Azure Upsell 고객 | 고객이 Azure에 대한 업셀 전파를 표시하는지 여부를 식별합니다. | 
| upsell 고객 Microsoft 365 | 고객이 상향 판매 성향을 표시 하는지 여부를 식별 Microsoft 365 | 
| RevSumDivisionName | 갱신을 위한 제품을 식별 합니다. | 

## <a name="next-steps"></a>다음 단계

자세한 내용은 [보고서 다운로드](pci-download-reports.md)를 참조 하세요.
