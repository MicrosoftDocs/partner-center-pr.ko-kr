---
title: 인사이트 데이터 정의
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 문서에는 다양 한 보고서와 해당 데이터 정의가 나열 되어 있으며,이는 Insights 다운로드 보고서 페이지에서 다운로드할 수 있습니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861396"
---
# <a name="export--data-definitions"></a>Export – 데이터 정의 

 **적절한 역할** 

- 보고서 뷰어 
- 임원 보고서 뷰어 

## <a name="introduction"></a>소개 

Insights 대시보드의 다운로드 보고서 허브를 사용 하 여 원시 데이터 집합을 내보낼 수 있습니다. 

데이터 정의와 함께 다운로드할 수 있는 다양 한 보고서는 다음 표에 나와 있습니다. 

### <a name="partner-profile-report"></a>**파트너 프로필 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPNId | Microsoft 파트너 네트워크 식별자 (MPN) | 
| PartnerName | 파트너의 이름입니다. | 
| PGA_MPNId | 파트너 전역 계정 MPN의 식별자 | 
| PGA_PartnerName | 파트너 전역 계정 이름 | 
| 구/군/시 | 파트너의 도시 위치 | 
| 국가 | 파트너의 국가 위치 | 
| 계층 구조 수준 | 전역 MPN ID 또는 위치 MPN ID 인지 여부를 나타냅니다. | 

### <a name="customer-details-report"></a>**고객 세부 정보 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerName | 고객 이름 | 
| CustomerTenantId | 고객 테 넌 트의 식별자 | 
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
| RevenueUSD | 미국 달러의 수익 | 

### <a name="reseller-performance-report"></a>**재판매인 성능 보고서**

> [!Note]
> 수익 및 ACR 데이터는 임원 보고서 뷰어 인 사용자만 사용할 수 있습니다.

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| ResellerMPNid | 재판매인 Microsoft 파트너 네트워크 식별자 | 
| ResellerName | 재판매인 이름 | 
| ResellerMarket | 대리점의 시장 국가 | 
| IndirectProviderMPNId | 간접 공급자 Microsoft 파트너 네트워크의 식별자입니다. | 
| IndirectProviderName | 간접 공급자 이름 | 
| 월 | 사용량 및 수익이 보고 되는 월 | 
| 제품 | 제품 이름 | 
| 구독 ID | 구독의 식별자입니다. | 
| 사용자의 좌석 | 사용 가능한 사용자 수 | 
| AssignedSeats | 할당 된 사용자 수 | 
| BilledRevenueUSD | 미국 달러로 청구 되는 수익 | 
| CustomerName | 고객 이름 | 
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
| CustomerSegment | 고객의 시장 부문 | 
| CustomerMarket | 고객의 지리적 시장 | 
| 제품 | 파트너가 고객에 게 판매 하는 제품 | 
| SKU | 제품의 SKU | 
| MPNId | 파트너의 Microsoft 파트너 네트워크 ID입니다. | 
| PartnerName | 파트너의 이름입니다. | 
| 공동 배치 위치 | 파트너의 지리적 위치 | 
| PartnerAttributionType | 구독에 대 한 특성 유형 | 
| SalesChannel | 판매 다이렉트, CSP (클라우드 솔루션 공급자) 등의 채널 | 
| 사용자의 좌석 | 현재 사용 가능한 사용자 | 
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
| CustomerSegment | 고객의 부문 | 
| CustomerMarket | 고객의 지리적 시장 | 
| MPNId | 고객의 Microsoft 파트너 네트워크 ID | 
| PartnerName | 파트너의 이름입니다. | 
| 공동 배치 위치 | 파트너의 지리적 국가 위치 | 
| PartnerAttributionType | 파트너의 특성 유형 | 
| SalesChannel | 판매 채널 (직접/CSP, 간접/CSP, 직접 등) | 
| ACR_USD | 미국 달러의 Azure 사용 수익 (ACR) | 
| 등록 ID | Azure 구독의 등록 ID | 

### <a name="office-365-license-usage-report"></a>**Office 365 라이선스 사용 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테 넌 트 ID | 
| CustomerTpid | 상위 상위 고객 ID | 
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
| CustomerTpid | 상위 상위 고객 ID | 
| WorkloadName | EMS (Enterprise Mobility + Security) 작업의 이름 | 
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
| DetailedSalesModel | 구독에 대 한 세부 판매 모델 | 
| CustomerName | 고객 이름 | 
| CustomerTenantId | 고객 테 넌 트의 GUID | 
| CustomerTpid | 고객 상위 부모 식별자 | 
| CustomerSegment | 고객의 시장 부문 | 
| CustomerMarket | 고객의 지리적 시장 | 
| MPNId | Microsoft 파트너 네트워크의 식별자 | 
| PartnerName | 파트너의 이름입니다. | 
| 공동 배치 위치 | 파트너의 지리적 국가 위치 | 
| PartnerAttachType | 구독에 대 한 특성 유형 | 
| 사용자의 좌석 | 현재 사용 가능한 사용자 | 
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
| SalesModel | 구독을 판매 하는 데 사용 되는 판매 모델 | 
| DetailedSalesModel | 구독에 대 한 세부 판매 모델 | 
| CustomerName | 고객 이름 | 
| CustomerTenantId | 고객 테 넌 트의 GUID | 
| CustomerTpid | 고객 상위 상위의 식별자 | 
| CustomerSegment | 고객의 시장 부문 | 
| CustomerMarket | 고객의 지리적 시장 | 
| MPNId | Microsoft 파트너 네트워크의 식별자 | 
| PartnerName | 파트너의 이름입니다. | 
| 공동 배치 위치 | 파트너의 지리적 국가 위치 | 
| PartnerAttachType | 구독에 대 한 특성 유형 | 
| 사용자의 좌석 | 현재 사용 가능한 사용자 | 
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

### <a name="teams-monthly-usage-report"></a>**팀 월간 사용량 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테 넌 트 ID | 
| CustomerTpid | 고객 상위 상위의 식별자 | 
| 월 | 사용량이 보고 되는 월 | 
| 하위 워크 로드 | 사용량이 보고 되는 하위 작업 (회의, 호출 또는 전화 시스템) | 
| 데스크톱 사용자 | 데스크톱에서 팀을 사용 하는 사용자 수 | 
| 모바일 사용자 | 모바일에서 팀을 사용 하는 사용자 수 | 
| 웹 사용자 | 웹에서 팀을 사용 하는 사용자 수 | 
| AllUpParticipants | 매월 팀의 고유 사용자 수 | 

### <a name="teams-usage-3p-apps-report"></a>**팀 사용 3P 앱 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| CustomerTenantId | 고객의 테 넌 트 ID | 
| CustomerTpid | 상위 상위 고객 ID | 
| 월 | 사용량이 보고 되는 월 | 
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
| IcMCP | 사용자가 Microsoft 인증 전문가 (MCP) 인지 여부를 나타냅니다. | 
| MCPID | 사용자의 MCP ID | 
| MPNId | Microsoft 파트너 네트워크의 식별자 | 
| PartnerName | 파트너의 이름입니다. | 
| PartnerCityLocation | 파트너의 지리적 도시 위치 | 
| PartnerCountryLocation | 파트너의 지리적 국가 위치 | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| 사용자 이름 | 사용자의 이름 | 
| UserId | 사용자의 GUID입니다. | 
| TrainingName | 교육의 이름 | 
| TrainingType | 학습 유형 (모듈 또는 학습 경로) | 
| 제품 | 학습 모듈을 적용할 수 있는 제품 | 
| 역할 | 해당 교육의 적용 가능한 역할 | 
| 만료 날짜 | 학습 완료 날짜 | 
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
| CompetencyAttainmentOptionName | 역량 attainment 옵션의 이름입니다. | 
| 월 | 메트릭이 보고 되는 월 | 
| MetricName | 역량에 해당 하는 메트릭의 이름입니다. | 
| MetricMonthlyContribution | 메트릭의 월간 기여 | 
| TTMAggregate | 후행 12 개월 동안의 집계 메트릭 | 
| AnniversaryYearAggregate | 현재 기념일 연도에 대 한 집계 메트릭 | 
| GoldThreshold | 골드 역량을 충족 하기 위한 성능 요구 사항 | 
| SilverThreshold | 실버 역량을 충족 하기 위한 성능 요구 사항 | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**클라우드 어센더-Microsoft 365 성향 보고서**

| 열 이름 | 데이터 설명 | 
| :--------- | :--------- | 
| MPN ID | Microsoft 파트너 네트워크 ID | 
| 파트너 이름 | 파트너의 이름입니다. | 
| 고객 ID | 고객의 식별자 번호 | 
| DUNS 번호 | 성향에 대해 점수가 매겨진 고객의 Dun & Bradstreet (D&B) 번호 | 
| 계정 이름 | 계정 이름 | 
| 도메인 | 계정의 도메인 | 
| 조직 크기 | 조직의 규모 | 
| 업종 | 조직이 속한 업계 | 
| Vertical | Microsoft, D&B 및 기타 산업 표준에 의해 식별 되는 성향에 대해 점수가 매겨진 고객의 세로 | 
| 영역 | 위치의 지리적 영역 | 
| 자회사 | 성향에 대해 점수가 매겨진 고객의 자회사 | 
| Sales Territory | 성향에 대해 점수가 매겨진 고객의 판매 지역 | 
| 구/군/시 | 조직의 지리적 도시 위치 | 
| 시스템 상태 | 조직의 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 조직의 지리적 국가 위치 | 
| Segment | 시장 부문 | 
| 하위 세그먼트 | 시장 subsegment | 
| SMC 유형 요약 | SMC 유형 | 
| 상위 관리 되지 않는 계산 기준 | 상위 관리 되지 않는 고객-계산 | 
| 상위 관리 되지 않는 사용자 기반 | 상위 관리 되지 않는 고객 – 사용자 | 
| IsNonProfit | 조직이 비영리 인지 여부를 나타냅니다 (예 또는 아니요). | 
| 원격 작업 사용-대상 Exchange Online | 상향 판매에 대 한 활성 Exchange Online 구독이 있는 고객은 Microsoft 365 | 
| 클라우드 어센더 성향-+ 10 라이선스를 사용 하 여 원격 작업-온-프레미스 획득 (현재 버전) 사용 | 현재 온-프레미스 Office 또는 Windows 클라이언트를 보유 하는 고객입니다. 즉, 클라이언트 버전이 EOL (기간 종료) 버전 보다 이후입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 점수가 성향 고객입니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향를 사용 하 여 원격 작업-온-프레미스 획득 (현재 버전) 사용-<10 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 이후 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 점수가 성향 고객입니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향 없이 원격 작업-온-프레미스 획득 (현재 버전) 사용-+ 10 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 이후 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향을 사용 하지 않고 원격 작업-온-프레미스 취득 (현재 버전) 사용-<10 개 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 이후 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향-+ 10 라이선스를 사용 하 여 원격 작업-온-프레미스 획득 (EOL 버전) 사용 | EOL 온-프레미스 Office 또는 Windows 클라이언트 (즉, EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향를 사용 하 여 원격 작업-온-프레미스 획득 (EOL 버전) 사용-<10 라이선스 | EOL 온-프레미스 Office 또는 Windows 클라이언트 (즉, EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 클라우드 어센더 성향 없이 원격 작업-온-프레미스 획득 (EOL 버전) 사용-+ 10 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| Cloud 성향를 사용 하지 않고 원격 작업-온-프레미스 취득 (EOL 버전)을 사용 하도록 설정-<10 라이선스 | 현재 온-프레미스 Office 또는 Windows 클라이언트 (EOL 버전 또는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Microsoft 365 변환할 대상으로 지정 해야 합니다. | 
| 원격 작업 사용-Microsoft 365에 대 한 높은 성향 잠재 고객 (Act NowithEvaluate) | Microsoft 365에 대 한 높은 성향 고객이 있는 잠재 고객 | 
| 원격 작업 사용-Microsoft 365를 사용 하 여 경합 (확대/축소) | 확대/축소 및 Microsoft 365 있는 고객, 팀으로의 변환 대상 | 
| 원격 작업 사용-Microsoft 365 하지 않고 경합 (확대/축소) | 확대/축소, 팀으로의 변환을 위한 대상 고객 | 
| Microsoft 365 E5를 대상으로 하는 비용 및 관리-Microsoft 365 E3 대상 절감 | Microsoft 365 E3, 대상 Microsoft 365 E5 인 기존 고객 | 
| 비용 및 관리-Microsoft 365 Business 프리미엄을 대상으로 하는 Microsoft 365 Business Basic 및 Business Standard 고객 절감 | 기존 Microsoft 365 Business Basic 및 Business Standard customers, Microsoft 365 Business Premium의 대상 | 
| 조직 생산성 변화-Surface 성향 | 고객에 게 화면에 대 한 성향 표시 | 
| M365Cluster | Microsoft 365를 구매 하는 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 현재 작업을 수행한 후에도 여전히 용량이 있는 경우에만 키우십시오를 대상으로 지정 하 고 고객을 대상으로 평가 합니다. | 
| M365Fit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 가장 작은 Smb (중소기업)로 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적 적합성 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| M365Intent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| SurfaceCluster | 맞춤 및 의도 권장 사항을 클러스터로 통합 하 여 Surface를 구매할 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 현재 작업을 수행한 후에도 여전히 용량이 있는 경우에만 키우십시오를 대상으로 지정 하 고 고객을 대상으로 평가 합니다. | 
| SurfaceFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| SurfaceIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| O365Cluster | Office 365를 구매 하는 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 현재 작업을 수행한 후에도 여전히 용량이 있는 경우에만 키우십시오를 대상으로 지정 하 고 고객을 대상으로 평가 합니다. | 
| O365Fit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| O365Intent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| M365UpsellCustomer | 고객이 상향 판매 성향을 표시 하는지 여부를 식별 Microsoft 365 | 
| Google 포함 | 고객이 소유 하 고 있는 Google 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| AWS | 고객이 AWS (소유 Amazon Web Services) 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
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
| 구/군/시 | 지리적 위치 | 
| 시스템 상태 | 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 지리적 국가 위치 | 
| Segment | 시장 부문 | 
| 하위 세그먼트 | 시장 subsegment | 
| SMC 유형 요약 | 고객 분류: 상위 관리 되지 않는 사용자 기반 고객은 300 명 이상의 직원을가지고 있으며, 상위 관리 되지 않는 계산 기지는 고객에 게 서 USD10, 000 년의 잠재력, 중소기업은 25 명 이상의 고객으로, 중소기업은 25 명 미만의 고객입니다. | 
| 상위 관리 되지 않는 계산 기준 | 상위 관리 되지 않는 고객-계산 | 
| 상위 관리 되지 않는 사용자 기반 | 상위 관리 되지 않는 고객 – 사용자 | 
| IsNonProfit | 조직이 비영리 인지 여부를 나타냅니다 (예 또는 아니요). | 
| 디지털 판매-Microsoft 365 사용자 크기 >= 25 명 (SalesPro 성향 model)을 활성화 합니다. | Dynamics 365이 없는 고객. 좌석 크기: 25 +. 파트너는 Dynamics 365 SalesPro의 교차 판매를 대상으로 해야 합니다. | 
| 디지털 판매-Dynamics 365 SalesPro 성향 (Act 또는 Evaluate) 활성화 | Dynamics 365이 없는 상위 성향 고객. 파트너는 Dynamics 365 SalesPro을 대상으로 해야 합니다. | 
| Navision에 대 한 금융 & 위험 관리-Dynamics 온-프레미스 설치 기본-(Business Central 성향 model) | 온-프레미스 Navision를 사용 하는 기존 고객. 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| 금융 위험 관리 & 사기 행위 온-프레미스 설치 기본-Dynamics AX (Dynamics 365 재무 + Operations 성향 model) | 온-프레미스 AX를 사용 하는 기존 고객 파트너는 Dynamics 365 재무 + 작업을 대상으로 해야 합니다. | 
| 사기 행위 & 사기 행위 관리-Dynamics 온-프레미스 설치 기본-뛰어난 Plains (Business Central 성향 모델) | 온-프레미스에서 좋은 Plains 있는 기존 고객. 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| 사기 행위 & 사기 행위 관리-Dynamics 온-프레미스 설치 기반-솔로몬 (Business Central 성향 모델) | 온-프레미스를 사용 하는 기존 고객 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| & 사기 행위 관리-Dynamics 온-프레미스 설치 기본-기타 (Business Central 성향 model) | 이전에 나열 되지 않은 다른 온-프레미스 솔루션을 사용 하는 기존 고객 파트너는 Dynamics 365 비즈니스 중부를 대상으로 해야 합니다. | 
| Agile 비즈니스 프로세스 빌드-Dynamics 온-프레미스 설치 base-AX/GP/SL/NAV/Other (Dynamics 365 성향 model) | Agile 비즈니스 프로세스 빌드-Dynamics 온-프레미스 설치 base-AX/GP/SL/NAV/Other (Dynamics 365 성향 model) | 
| Agile 비즈니스 프로세스 빌드-Dynamics 경합 베이스-Mendix/OutSystems/Salesforce (Dynamics 365 성향 model) | Agile 비즈니스 프로세스 빌드-Dynamics 경합 베이스-Mendix/OutSystems/Salesforce (Dynamics 365 성향 model) | 
| Agile 비즈니스 프로세스 빌드-Dynamics 365 재무 + 작업 설치 기준 | 기존 Dynamics 365 재무 + 운영 고객. Power Apps를 대상으로 하는 파트너입니다. | 
| Agile 비즈니스 프로세스 빌드-Dynamics 365 Business Central 설치 기반 | 기존 Dynamics 365 비즈니스 중부 고객. Power Apps를 대상으로 하는 파트너입니다. | 
| Agile 비즈니스 프로세스 빌드-Dynamics 365 Customer Engagement 설치 기준 | 기존 Dynamics 365 고객 참여 고객 Power Apps를 대상으로 하는 파트너입니다. | 
| 복원 력 있는 공급망을 빌드하고, 비 Oracle 또는 SAP ERP (엔터프라이즈 리소스 계획) 고객을 사용 하 여 Dynamics 365 공급망 관리로 첫 Dynamics 365 워크 로드를 활성화 합니다. | Dynamics 365 공급망 관리를 위한 대상 고객 | 
| 복원 력 있는 공급망 빌드-기존 Dynamics 365 고객 Engagement 고객에 게 상호 판매 Dynamics 365 공급망 관리 및/또는 소매 또는 상거래 | 기존 Dynamics 365 고객 Engagement 고객이 교차 판매 Dynamics 365 공급망 관리를 대상으로 합니다. | 
| 복원 력 있는 공급망 빌드-dynamics 365 고객 참여 및 Oracle 또는 SAP에 대 한 Dynamics 365 공급망 관리 및/또는 소매 또는 상거래를 교차 판매 합니다. | Dynamics 365 공급망 관리를 대상으로 하는 기존 Dynamics 365 고객 Engagement 고객이 Oracle 또는 SAP를 대상으로 합니다. | 
| D365BCCluster | Dynamics 365 비즈니스 중부를 구매 하는 고객의 성향을 식별 합니다. 성향 for Business Central을 표시 하는 고객은 중간 및 작은 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365BCFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| D365BCIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| D365FOCluster | Dynamics 365 재무 및 운영을 구매 하는 고객의 성향을 식별 합니다. 재무 + 작업에 대해 성향를 표시 하는 고객은 관리 되지 않는 상위 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365FOFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| D365FOIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| D365CECluster | Dynamics 365 고객 참여를 구매 하는 고객의 성향을 식별 합니다. 고객 Engagement에 대 한 성향를 표시 하는 고객은 중간 및 작은 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365CEFit | Dynamics 365 고객 Engagement에 맞게 맞춤을 나타냅니다. | 
| D365CEIntent | Dynamics 365 고객 Engagement의 용도를 나타냅니다. | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | 고객이 Dynamics 온-프레미스 AX 또는 CRM에 대 한 오픈 갱신을 보유 하는지 여부를 식별 합니다. | 
| M365UpsellCustomer | 고객이 상향 판매 성향을 표시 하는지 여부를 식별 Microsoft 365 | 
| Google 포함 | 고객이 소유 하 고 있는 Google 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| AWS | 고객이 소유 하는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| EA 있음 | 갱신이 EA 또는 EA 구독 인지 여부를 식별 합니다. | 
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
| 구/군/시 | 지리적 위치 | 
| 시스템 상태 | 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 지리적 국가 위치 | 
| Segment | 시장 부문 | 
| 하위 세그먼트 | 시장 subsegment | 
| SMC 유형 요약 | SMC 유형 | 
| 상위 관리 되지 않는 계산 기준 | 상위 관리 되지 않는 고객-계산 | 
| 상위 관리 되지 않는 사용자 기반 | 상위 관리 되지 않는 고객 – 사용자 | 
| IsNonProfit | 조직이 비영리 인지 여부를 나타냅니다 (예 또는 아니요). | 
| 마이그레이션-EOL Windows Server IB 클라우드 어센더 성향-5 + 라이선스를 사용 하는 EOL Windows Server | EOL 온-프레미스 Windows Server (즉, EOL 버전 또는 그 이전 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 점수가 성향 고객입니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL Windows Server IB-클라우드 <성향를 사용 하는 EOL Windows Server 5 개 라이선스 | EOL 온-프레미스 Windows Server (즉, EOL 버전 또는 그 이전 버전)가 있는 고객입니다. 고객이 라이선스를 5 개 미만으로 보유 합니다. 점수가 성향 고객입니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL Windows Server-클라우드 어센더 성향 없이 IB Windows Server + 라이선스 | EOL 온-프레미스 Windows Server (즉, EOL 버전 또는 그 이전 버전)가 있는 고객입니다. 고객이 라이선스를 5 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL Windows Server IB 클라우드 <성향이 없는 Windows Server 5 개 라이선스 | EOL 온-프레미스 Windows Server (즉, EOL 버전 또는 그 이전 버전)가 있는 고객입니다. 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL SQL-EOL SQL Server IB 클라우드 어센더 성향-5 + 라이선스 | EOL 온-프레미스 SQL Server (즉, EOL 버전 또는 이전 버전)을 보유 하 고 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| IB 클라우드 <성향를 사용 하 여 마이그레이션-EOL SQL-EOL SQL Server 5 개 라이선스 | EOL 온-프레미스 SQL Server (즉, EOL 버전 또는 이전 버전)을 보유 하 고 있는 고객입니다. 라이선스가 5 개 미만입니다. 점수가 성향 고객입니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-EOL SQL-EOL SQL Server IB 성향 (Cloud 어센더) | EOL 온-프레미스 SQL Server (즉, EOL 버전 또는 이전 버전)을 보유 하 고 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| IB 성향 <를 사용 하지 않고 클라우드 어센더를 사용 하지 않는 마이그레이션-eol SQL Server 5 개 라이선스 | EOL 온-프레미스 SQL Server (즉, EOL 버전 또는 이전 버전)을 보유 하 고 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-온-프레미스 Windows Server 마이그레이션-현재 Windows Server IB 및 클라우드 어센더 성향-5 + 라이선스 | 현재 온-프레미스 Windows Server가 있는 고객 (EOL 이후의 버전)입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-온-프레미스 Windows Server 마이그레이션-IB 성향를 사용 하 여 현재 Windows Server 클라우드 어센더 사용 <-5 개 라이선스 | 현재 온-프레미스 Windows Server가 있는 고객 (EOL 이후의 버전)입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게는 Azure에 대 한 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-온-프레미스 Windows Server 마이그레이션-클라우드 어센더 성향 없는 현재 Windows Server IB + 라이선스 | 현재 온-프레미스 Windows Server가 있는 고객 (EOL 이후의 버전)입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-온-프레미스 Windows Server 마이그레이션-클라우드 성향 없이 현재 Windows Server IB-<5 개 라이선스 | 현재 온-프레미스 Windows Server가 있는 고객 (EOL 이후의 버전)입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Azure SQL 또는 SQL Vm (가상 머신)으로 마이그레이션-성향 IB 이상 라이선스를 사용 하 여 현재 SQL Server | 현재 온-프레미스 SQL Server (즉, EOL 이후 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-Cloud 성향를 사용 하 여 현재 SQL Server IB-<5 개 라이선스 | 현재 온-프레미스 SQL Server (즉, EOL 이후 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게는 성향 점수가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-클라우드 어센더 성향 IB 이상 라이선스 없이 현재 SQL Server | 현재 온-프레미스 SQL Server (즉, EOL 이후 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-Cloud 성향를 <사용 하지 않는 현재 SQL Server IB 5 개 라이선스 | 현재 온-프레미스 SQL Server (즉, EOL 이후 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-OSS-오픈 소스 셰익스피어 (OSS) DB로 마이그레이션 | 기존 고객에 게는 PostgreSQL, MySQL, MariaDB 등의 경쟁 제품 중 하나가 있습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-OSS-Azure의 Linux | Linux를 사용 하는 기존 고객 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-SAP-Azure의 SAP | 기존 고객이 SAP를 사용 합니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Windows 가상 데스크톱-원격 데스크톱 서비스 IB | 활성 Windows 원격 데스크톱 서비스 고객을 식별 합니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Windows 가상 데스크톱-최신 작업을 Azure/WVD로 교차 판매 | Microsoft 365 있는 고객을 식별 하 고 Azure를 사용 하지 않습니다. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-VMware IB | 제품이 있는 기존 고객: VMware. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 마이그레이션-Citrix IB | 제품을 포함 하는 기존 고객: Citrix Systems. 파트너는 Azure로 마이그레이션하기 위해이 고객을 대상으로 해야 합니다. | 
| 혁신적인 분석-Azure 성향를 사용 하는 Power BI IB | 및 활성 Power BI 구독을 포함 하는 고객: Power BI 독립 실행형 Pro, Power BI-Azure 제품군, Power BI Office 제품군, Power BI 제품군-Microsoft 365 | 
| GitHub를 사용 하 여 DevOps 사용-Visual Studio/MSDN IB | 활성 Visual Studio 버전을 사용 하는 고객 식별 | 
| Windows Server Standard 버전 | 고객의 Windows Server Standard 구매 버전을 표시 합니다. | 
| Windows Server Standard 라이선스 | 고객의 Windows Server Standard 구매 라이선스 유형을 표시 합니다. | 
| Windows Server Data Center 버전 | 고객의 Windows 데이터 센터 구매 버전을 표시 합니다. | 
| Windows Server 데이터 센터 라이선스 | 고객의 Windows 데이터 센터 구매 라이선스 유형을 표시 합니다. | 
| AzureFit | Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 점수 매기기는 lookalike 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 적합성 인지 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다. | 
| AzureIntent | 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하는 데 적합 합니다. 의도 점수 매기기는 매월 업데이트 됩니다. | 
| AzureCluster | 클러스터에 적합 한 권장 사항을 통합 하 여 Azure를 구매 하는 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| WindowsServerDataCenter_HasOpenRenewal | 고객이 Windows Server Datacenter에 대해 오픈 갱신을 보유 하는지 여부를 식별 합니다. | 
| WindowsServerStandard_HasOpenRenewal | 고객이 Windows Server Standard에 대 한 오픈 갱신을 보유 하는지 여부를 식별 합니다. | 
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
| Vertical | Microsoft, D&B 및 기타 산업 표준에 의해 식별 되는 성향에 대해 점수가 매겨진 고객의 세로 | 
| 영역 | 위치의 지리적 영역 | 
| 자회사 | 성향에 대해 점수가 매겨진 고객의 자회사 | 
| Sales Territory | 성향에 대해 점수가 매겨진 고객의 판매 지역 | 
| 구/군/시 | 지리적 위치 | 
| 시스템 상태 | 지리적 상태 위치 | 
| 우편 번호 | 조직의 우편 번호 | 
| 국가 | 지리적 국가 위치 | 
| Segment | 시장 부문 | 
| 하위 세그먼트 | 시장 subsegment | 
| SMC 유형 요약 | SMC 유형 | 
| 상위 관리 되지 않는 계산 기준 | 상위 관리 되지 않는 고객-계산 | 
| 상위 관리 되지 않는 사용자 기반 | 상위 관리 되지 않는 고객 – 사용자 | 
| IsNonProfit | 조직이 비영리 인지 여부를 나타냅니다 (예 또는 아니요). | 
| Google 포함 | 고객이 소유 하는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| AWS | 고객이 소유 하는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다. | 
| Azure 클러스터 | Azure를 구매 하는 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365 재무 + 운영 클러스터 | Dynamics 365 재무 및 운영을 구매 하는 고객의 성향을 식별 합니다. 재무 + 작업에 대해 성향를 표시 하는 고객은 관리 되지 않는 상위 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365 CE 클러스터 | Dynamics 365 고객 참여를 구매 하는 고객의 성향을 식별 합니다. 고객 Engagement에 대 한 성향를 표시 하는 고객은 중간 및 작은 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| D365 BC 클러스터 | Dynamics 365 비즈니스 중부를 구매 하는 고객의 성향을 식별 합니다. 성향 for Business Central을 표시 하는 고객은 중간 및 작은 범주에 있습니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| Microsoft 365 클러스터 | Microsoft 365를 구매 하는 고객의 성향을 식별 합니다. 지금 작업을 대상으로 하 고 더 높은 수익률을 생성 하기 때문에 클러스터를 평가 합니다. 키우십시오를 대상으로 하 고, 현재 작업을 대상으로 하 고 고객을 평가한 후에도 여전히 용량이 있는 경우 고객을 교육 합니다. | 
| 라이선스 프로그램 | 갱신에 대 한 라이선스 프로그램 유형을 식별 합니다. | 
| 규약 ID | 규약의 식별자 | 
| 계약 종료 날짜 | 규약의 종료 날짜 | 
| 만료 유형 | 만료 유형 | 
| 만료 되는 수익 | 구독 만료와 관련 된 수익 | 
| EA 있음 | 갱신이 EA 또는 EA 구독 인지 여부를 식별 합니다. | 
| 열림 | 갱신이 오픈 또는 오픈 값 계약 인지 여부를 식별 합니다. | 
| Azure 상향 판매 고객 | 고객이 Azure에 대 한 상향 판매 성향를 표시 하는지 여부를 식별 합니다. | 
| Microsoft 365 상향 판매 고객 | 고객이 상향 판매 성향을 표시 하는지 여부를 식별 Microsoft 365 | 
| RevSumDivisionName | 갱신을 위한 제품을 식별 합니다. | 

## <a name="next-steps"></a>다음 단계

자세한 내용은 [보고서 다운로드](pci-download-reports.md)를 참조 하세요.
