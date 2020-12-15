---
title: Insights 데이터 정의
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 문서에서는 Insights 다운로드 보고서 페이지에서 다운로드할 수 있는 다양 한 보고서의 목록 및 각 보고서의 데이터 정의를 제공 합니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501755"
---
# <a name="export--data-definitions"></a>Export – 데이터 정의 

 **적절한 역할** 

- 보고서 뷰어 
- 임원 보고서 뷰어 

## <a name="introduction"></a>소개 

Insights 대시보드의 다운로드 보고서 허브를 사용 하면 원시 데이터 집합을 내보낼 수 있습니다.  

데이터 정의와 함께 다운로드할 수 있는 다양 한 보고서는 다음과 같습니다. 

**파트너 프로필**: 프로필 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다. 


| **열 이름** | **데이터 설명** |
|---------|:---------|
|MPNId|Microsoft 파트너 네트워크 ID|
|PartnerName|파트너의 이름입니다. |
|PGA_MPNId|파트너 전역 계정 MPN ID|
|PGA_PartnerName|파트너 전역 계정 이름|
|구/군/시|파트너의 도시 위치 |
|국가|파트너의 국가 위치 |
|계층 구조 수준|전역 MPN ID 또는 위치 MPN ID 인지를 나타냅니다.|

**고객 세부 정보**: 고객 세부 정보 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CustomerName|고객 이름 |
|CustomerTenantId|고객 테넌트 ID |
|CustomerTpid|고객 상위 부모 식별자 |
|CustomerSegment|고객 부문 |
|CustomerMarket|고객의 지리적 시장  |
|CustomerStatus|고객 상태 (활성/비활성) |
|Product|MPN을 통해 고객에 게 판매 되는 제품입니다. 이 항목은 O365, D365, Enterprise Mobility, Power BI Microsoft Azure 중 하나입니다.|
|SKU|   제품 SKU|
|월| 사용량 및 수익이 보고 되는 월|
|MPNId| Microsoft 파트너 네트워크 ID|
|PartnerName|   파트너의 이름입니다.|
|공동 배치 위치|   파트너의 지리적 위치|
|PartnerAttributionType|    파트너의 특성 유형|
|SalesChannel|  Sales Channel|
|사용자의 좌석|    사용 가능한 사용자| 
|RevenueUSD|    USD의 수익|

**재판매인 성능**: 재판매인 성능 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

> [!Note]
> 수익 및 ACR 데이터는 임원 보고서 뷰어 인 사용자 에게만 사용할 수 있습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|ResellerMpnid|재판매인 Microsoft 파트너 네트워크 식별자| 
|ResellerName|재판매인 이름|
|ResellerMarket|대리점의 시장 국가| 
|IndirectProviderMPNId|간접 공급자 Microsoft 파트너 네트워크 식별자|
|IndirectProviderName|간접 공급자 이름|
|월|사용량 및 수익이 보고 되는 월|
|Product|제품 이름|
|구독 ID|구독 식별자|
|사용자의 좌석|사용 가능한 사용자 수|
|AssignedSeats|할당 된 사용자 수|
|BilledRevenueUSD|청구 되는 수익 ($)|
|CustomerName|고객 이름| 
|CustomerTPid|고객 상위 부모 식별자| 
|CustomerSegment|고객 부문 |
|CustomerMarket|고객의 지리적 시장 |
|ResellerStatus|대리점 상태| 

**구독 세부 정보**: 구독 세부 정보 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

>[!Note]
>수익 및 ACR 데이터는 임원 보고서 뷰어 인 사용자 에게만 사용할 수 있습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|SubscriptionId|    구독의 GUID입니다.|
|Subscription.subscriptionstartdate| 구독의 시작 날짜|
|Subscription.subscriptionenddate|   구독의 종료 날짜|
|SubscriptionState| 구독의 상태 (활성 또는 변동)|
|월| 사용량 및 수익이 보고 되는 월|
|IsAutoRenew|   구독이 자동 갱신 인지 여부를 나타냅니다 (Y/N).|
|CustomerName|  고객 이름| 
|CustomerTenantId|  고객 GUID|
|CustomerTpid|  고객 상위 부모 식별자| 
|CustomerSegment|   고객의 시장 부문| 
|CustomerMarket|    고객의 지리적 시장|
|Product|   파트너가 고객에 게 판매 하는 제품| 
|SKU|   제품의 Sku |
|MPNId| 파트너의 Microsoft 파트너 네트워크 ID입니다. |
|PartnerName|   파트너의 이름입니다. |
|공동 배치 위치|   파트너의 지리적 위치 |
|PartnerAttributionType|    구독에 대 한 특성 유형|
|SalesChannel|  판매 채널 (직접/CSP 등) |
|사용자의 좌석|    현재 사용 가능한 사용자|
|RevenueUSD|    USD의 수익|
|등록 ID| 구독의 등록 ID|

**Azure 사용**: azure 사용 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|SubscriptionId|    구독의 GUID입니다.|
|Subscription.subscriptionstartdate| 구독 시작 날짜입니다.|
|Subscription.subscriptionenddate|   구독이 종료 되는 날짜입니다.|
|SubscriptionState| 구독의 현재 상태 (열림/닫힘/활성/InGrace 기간)|
|월| 월별로 집계 된 날짜 |
|ServiceName|   Azure 서비스의 이름입니다.|
|MeterCategory| 미터 범주의 이름|
|UsageUnits|    청구 주기 동안 사용 된 단위 수 |
|CustomerName|  고객 이름 |
|CustomerTenantId|  고객의 테 넌 트 ID |
|CustomerTpid|  상위 상위 고객 ID |
|CustomerSegment|   고객의 부문 |
|CustomerMarket|    고객의 지리적 시장 |
|MPNId  |고객의 Microsoft 파트너 네트워크 ID |
|PartnerName|   파트너의 이름입니다. |
|공동 배치 위치    |파트너의 지리적 국가 위치 |
|PartnerAttributionType |파트너의 특성 유형|
|SalesChannel|  판매 채널 (직접/CSP 간접/CSP 직접 등) |
|ACR_USD|   USD의 Azure 사용 수익|
|등록 ID| Azure 구독의 등록 ID|

**Office 365-라이선스 사용**: Office 365 라이선스 사용 현황 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CustomerTenantId|  고객의 테 넌 트 ID| 
|CustomerTpid|  상위 상위 고객 ID |
|WorkloadName|  Sfb, 팀, EXO |
|월| 사용량이 보고 되는 월|
|Paid의 해당 단위|    사용 가능한 유료 단위 수|
|MonthlyActiveUsers|    월간 활성 사용자 수|
|CustomerName|  고객 이름|
|CustomerMarket|    고객 시장의 지리적 국가 위치 |
|CustomerSegment|   고객 부문 |
|MPNId| Microsoft 파트너 네트워크 ID|
|PartnerName|   파트너의 이름입니다.|
|공동 배치 위치|   파트너의 지리적 위치|
|PartnerAttributionType|    파트너의 특성 유형|

**Enterprise Mobility – 라이선스 사용**: EMS – 라이선스 사용 현황 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CustomerTenantId|  고객의 테 넌 트 ID| 
|CustomerTpid|  상위 상위 고객 ID |
|WorkloadName|  EMS 작업의 이름 |
|월| 사용량이 보고 되는 월|
|Paid의 해당 단위|    사용 가능한 유료 단위 수|
|MonthlyActiveUsers|    월간 활성 사용자 수|
|CustomerName|  고객 이름|
|CustomerMarket|고객 시장의 지리적 국가 위치 |
|CustomerSegment|   고객 부문 |
|MPNId| Microsoft 파트너 네트워크 ID|
|PartnerName|   파트너의 이름입니다.|
|공동 배치 위치|   파트너의 지리적 위치|
|PartnerAttributionType|    파트너의 특성 유형|

**Dynamics 365 – 라이선스 사용**: dynamics 365 – 라이선스 사용 현황 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|SubscriptionId|구독의 GUID입니다.|
|Subscription.subscriptionstartdate| 구독의 시작 날짜|
|Subscription.subscriptionenddate|   구독의 종료 날짜|
|SubscriptionStatus|    구독의 상태 |
|월| 사용량이 보고 되는 월|
|RevSumDivisionName|    Rev 합계 나누기의 이름입니다.|
|RevSumCategoryName|    Rev 합계 범주의 이름|
|SKU|   제품의 Sku |
|SKUId| 제품의 Sku ID |
|FreeVsPaidSKU| 무료 또는 유료 SKU 인지 여부를 나타냅니다. |
|SalesModel|    구독 판매에 사용 되는 판매 채널|
|DetailedSalesModel|    구독에 대 한 세부 판매 모델|
|CustomerName|  고객 이름 |
|CustomerTenantId|  고객 테 넌 트 GUID |
|CustomerTpid|  고객 상위 부모 식별자 |
|CustomerSegment|   고객의 시장 부문 |
|CustomerMarket|    고객의 지리적 시장 |
|MPNId| Microsoft 파트너 네트워크 ID |
|PartnerName|   파트너의 이름입니다. |
|공동 배치 위치|   파트너의 지리적 국가 위치 |
|PartnerAttachType| 구독에 대 한 특성 유형|
|사용자의 좌석|    현재 사용 가능한 사용자|
|AssignedSeats| 현재 할당 된 사용자 |
|ActiveSeats|   현재 활성 사용자 |
|DeploymentOpportunity| 현재 배포 기회|
|ActiveUsagePercent|    현재 활성 사용 백분율|
 
**라이선스 사용 Power BI**: Power BI-라이선스 사용 보고서의 다양 한 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|SubscriptionId|    구독의 GUID입니다.|
|Subscription.subscriptionstartdate| 구독의 시작 날짜|
|Subscription.subscriptionenddate|   구독의 종료 날짜|
|SubscriptionStatus|    구독의 상태 (활성 또는 In-Active 또는 유예 기간)|
|월| 월별로 집계 된 날짜 |
|SKU|   제품의 Sku |
|SKUId| 제품의 Sku ID |
|FreeVsPaidSKU| 무료 또는 유료 Sku 차이점 |
|SalesModel|    구독 판매에 사용 되는 판매 모델|
|DetailedSalesModel|    구독에 대 한 세부 판매 모델|
|CustomerName|  고객 이름 |
|CustomerTenantId|  고객 테 넌 트 GUID |
|CustomerTpid|  고객 상위 부모 식별자| 
|CustomerSegment|   고객의 시장 부문 |
|CustomerMarket|    고객의 지리적 시장 |
|MPNId| Microsoft 파트너 네트워크 ID |
|PartnerName|   파트너의 이름입니다. |
|공동 배치 위치|   파트너의 지리적 국가 위치 |
|PartnerAttachType| 구독에 대 한 특성 유형|
|사용자의 좌석|    현재 사용 가능한 사용자|
|AssignedSeats| 현재 할당 된 사용자|
|ActiveSeats|   현재 활성 사용자|
|DeploymentOpportunity| 현재 배포 기회|
|ActiveUsagePercent|    현재 활성 사용 백분율|

**팀 사용량 – 회의 및 호출**: 다양 한 필드의 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CustomerTenantId|  고객의 테 넌 트 ID |
|CustomerTpid|  상위 상위 고객 ID |
|월| 사용량이 보고 되는 월|
|하위 워크 로드|   사용량이 보고 되는 하위 작업 (회의, 통화, 전화 시스템)|
|모임 수| 모임 수|
|모임 기간|  총 모임 기간 (시)|

**팀-월간 사용량 세부 정보**: 다양 한 필드의 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CustomerTenantId|  고객의 테 넌 트 ID |
|CustomerTpid|  상위 상위 고객 ID |
|월| 사용량이 보고 되는 월|
|하위 워크 로드|   사용량이 보고 되는 하위 작업 (회의, 통화, 전화 시스템)|
|데스크톱 사용자| 데스크톱에서 팀을 사용 하는 사용자 수|
|모바일 사용자|  모바일에서 팀을 사용 하는 사용자 수|
|웹 사용자| 웹에서 팀을 사용 하는 사용자 수|
|AllUpParticipants| 매월 팀의 고유 사용자 수|

**팀 사용량 – 3P 앱**: 다양 한 필드의 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CustomerTenantId|  고객의 테 넌 트 ID| 
|CustomerTpid|  상위 상위 고객 ID |
|월| 사용량이 보고 되는 월|
|3P 앱 이름|   팀 앱 이름|
|사용자 수|    앱에 대 한 사용자 수|


**학습 세부 정보**: 학습 정보 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|TrainingActivityId|    교육의 식별자 |
|TrainingTitle| 학습 제목 |
|TrainingType|  교육 유형 (인증/시험)|
|IndividualFirstName|   고객의 이름| 
|IndividualLastName|    고객의 성| 
|메일| 고객의 개인 전자 메일 ID|
|CorpEmail| 고객의 Office 전자 메일 ID|
|TrainingCompletionDate|    학습 완료 날짜 |
|월| 데이터가 보고 되는 월|
|IcMCP| 사용자가 Microsoft 인증 전문가 인지 여부를 나타냅니다.|
|MCPID| 사용자의 MCP ID|
|MPNId| Microsoft 파트너 네트워크 ID |
|PartnerName|   파트너의 이름입니다. |
|PartnerCityLocation|   파트너의 지리적 도시 위치 |
|PartnerCountryLocation|    파트너의 지리적 국가 위치 |

**Microsoft Learn**: Microsoft Learn 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|사용자 이름|사용자의 이름| 
|UserId|사용자 GUID |
|TrainingName|교육의 이름 |
|TrainingType|학습 유형 (모듈/학습 경로)|
|제품|학습 모듈을 적용할 수 있는 제품|
|역할|해당 교육의 적용 가능한 역할 |
|만료 날짜|교육이 완료 된 날짜 |
|MPNId|Microsoft 파트너 네트워크 ID |
|PartnerName|파트너의 이름입니다. |
|국가|파트너의 지리적 국가 위치 |

**역량 요약 및 기록**: 역량 요약 및 기록 보고서의 다양 한 필드의 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CompetencyName|역량의 이름 |
|CompetencyLevel|역량 수준 (골드/Silver)|
|CompetencyStatus|역량의 현재 상태 (활성/비활성/유예 기간)|
|CompetencyStartDate|지정 된 역량의 시작 날짜| 
|CompetencyEndDate|지정 된 역량의 종료 날짜 |

**역량 성능**: 역량 성능 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|CompetencyName|    역량의 이름 |
|CompetencyAttainmentOptionName|    역량 attainment 옵션의 이름입니다.|
|월| 메트릭이 보고 되는 월|
|MetricName|    역량에 관련 된 메트릭의 이름입니다.|
|MetricMonthlyContribution| 메트릭의 월간 기여|
|TTMAggregate|  후행 12 개월 동안의 집계 메트릭|
|AnniversaryYearAggregate|  현재 기념일 연도에 대 한 집계 메트릭|
|GoldThreshold| 골드 역량을 충족 하기 위한 성능 요구 사항|
|SilverThreshold|   실버 역량을 충족 하기 위한 성능 요구 사항|

**클라우드 어센더-M365 성향**: 클라우드 어센더-M365 성향 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|MPN ID|    Microsoft 파트너 네트워크 ID|
|파트너 이름|  파트너의 이름입니다.|
|고객 ID|   고객 식별자 번호 |
|DUNS 번호|   성향에 대해 점수가 매겨진 고객의 Dun & Bradstreet 번호|
|계정 이름|  계정 이름 |
|도메인|    계정의 도메인|
|조직 크기|  조직의 규모|
|업종|  업종  |
|Vertical|  Microsoft 및 기타 업계 표준 (D&B)으로 식별 된 성향 점수가 매겨진 고객의 세로|
|영역|  위치의 지리적 영역|
|자회사|    성향에 대해 점수가 매겨진 고객의 자회사|
|Sales Territory|   성향에 대해 점수가 매겨진 고객의 판매 지역|
|구/군/시|  지리적 위치 |
|주| 지리적 상태 위치|
|우편 번호|   우편 번호|
|국가|   지리적 국가 위치 |
|Segment|   시장 부문 |
|하위 세그먼트|   시장 서브 부문 |
|SMC 유형 요약|  SMC 유형 |
|상위 관리 되지 않는 계산 기준|  상위 관리 되지 않는 고객-계산|
|상위 관리 되지 않는 사용자 기반| 상위 관리 되지 않는 고객 – 사용자|
|IsNonProfit|   비영리 또는 수익이 있는지 여부 (예/아니요)|
|원격 작업 사용-대상 Exchange Online|   활성 exchange online 구독이 있는 고객, 상향 판매 M365|
|CLAS 성향-+ 10 라이선스를 사용 하 여 원격 작업 프레미스 획득 (현재 버전) 사용|현재 온-프레미스 Office 또는 Win Client (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 점수가 성향 고객입니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|CLAS 성향 <10 라이선스를 사용 하 여 원격 작업-온-프레미스 획득 (현재 버전) 사용|현재 온-프레미스 Office 또는 Win Client (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 점수가 성향 고객입니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|CLAS 성향 (현재 버전)를 사용 하지 않고 원격 작업 (프레미스)을 사용 하도록 설정-+ 10 라이선스| 현재 온-프레미스 Office 또는 Win Client (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|성향 <10 라이선스를 사용 하지 않고 원격 작업-온-프레미스 획득 (현재 버전) 사용| 현재 온-프레미스 Office 또는 Win Client (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게 성향 점수가 없습니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|CLAS 성향-+ 10 라이선스로 원격 작업 (프레미스)을 사용 하도록 설정 합니다.|EOS (프레미스) Office 또는 Win Client가 있는 고객 (즉, EOS 제품 이전 및 포함)입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게는 성향 점수가 있습니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|CLAS 성향 <10 라이선스를 사용 하 여 원격 작업 인 EOS (프레미스 취득) 사용|EOS (프레미스) Office 또는 Win Client가 있는 고객 (즉, EOS 제품 이전 및 포함)입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게는 성향 점수가 있습니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|CLAS 성향 없이 원격 작업 (프레미스)을 사용 하도록 설정-+ 10 라이선스| 현재 온-프레미스 Office 또는 Win Client (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|성향 <10 라이선스를 사용 하지 않고 원격 작업 인 EOS (프레미스) 사용| 현재 온-프레미스 Office 또는 Win Client (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 고객이 라이선스를 10 개 미만으로 보유 합니다. 고객에 게 성향 점수가 없습니다. M365로의 변환을 위해 파트너는 대상으로 지정 해야 합니다.|
|원격 작업 사용-M365에 대 한 High 성향 잠재 고객 (현재 작업/평가)| M365에 대 한 high 성향가 있는 잠재 고객입니다.|
|원격 작업 사용-M365를 사용 하 여 경합 (확대/축소)| 확대/축소 및 M365이 있는 고객, 팀으로의 변환을 위한 대상|
|원격 작업 사용-M365 없이 경합 (확대/축소)|  확대/축소를 사용 하는 고객 (팀으로 변환)|
|M365 E5의 비용 및 관리-M365 E3 대상 절감| M365 E3이 있는 기존 고객, M365 E5의 대상|
|M365 BP를 대상으로 하는 비용 및 관리-M365 BB 및 BS 고객 절감|    기존 M365 BB 및 BS 고객, M365 BP를 대상으로 합니다.|
|조직 생산성 변화-Surface 성향|    고객이 Surface에 대 한 성향을 표시 합니다.|
|M365Cluster|M365를 구매 하는 고객의 성향을 식별 합니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|M365Fit|   Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다.|
|M365Intent|    소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다. 의도 점수 매기기는 매월 업데이트 됩니다.|
|SurfaceCluster|    이는 클러스터에 맞춤 및 의도 권장 사항을 통합 하 여 고객의 구매 성향을 식별 합니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|SurfaceFit|    Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다.|
|SurfaceIntent| 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다. 의도 점수 매기기는 매월 업데이트 됩니다.|
|O365Cluster|   이는 고객의 성향에서 O365 구매를 식별 합니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|O365Fit|   Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다.|
|O365Intent|    소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다. 의도 점수 매기기는 매월 업데이트 됩니다.|
|M365UpsellCustomer|    고객이 상향 판매 성향 for M365를 표시 하는지 여부를 식별 합니다.|
|Google 포함|    이 플래그는 고객이 소유 하 고 있는 Google 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|AWS|   이 플래그는 고객이 소유 하 고 있는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|EA 있음|    이는 갱신이 EA (기업 계약) 인지 EA 구독 인지를 식별 합니다.|
|열림|  이는 갱신이 오픈 값 계약 인지 여부를 식별 합니다.|

**클라우드 어센더-D365 성향**: 클라우드 어센더-D365 성향 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

| **열 이름** | **데이터 설명** |
|---------|:---------|
|MPN ID|    Microsoft 파트너 네트워크 ID|
|파트너 이름|  파트너의 이름입니다.|
|고객 ID|   고객 식별자 번호 |
|DUNS 번호|   성향에 대해 점수가 매겨진 고객의 Dun & Bradstreet 번호|
|계정 이름|  계정 이름 |
|도메인|    계정의 도메인|
|조직 크기|  조직의 규모|
|업종|  업종  |
|Vertical|  Microsoft 및 기타 업계 표준 (D&B)으로 식별 된 성향 점수가 매겨진 고객의 세로
|영역|  위치의 지리적 영역|
|자회사|    성향에 대해 점수가 매겨진 고객의 자회사|
|Sales Territory|   Sales Territory|
|구/군/시|  지리적 위치 |
|주| 지리적 상태 위치|
|우편 번호|   우편 번호|
|국가|   지리적 국가 위치 |
|Segment|   시장 부문 |
|하위 세그먼트|   시장 서브 부문 |
|SMC 유형 요약|  고객 분류: 상위 관리 되지 않는 사용자 기본은 300 개 이상의 직원이 있는 고객입니다. 상위 관리 되지 않는 계산 기반 고객은 Azure 3 년간 $10k를 사용 하 고 있으며, 중간 규모 비즈니스는 직원 수가 25 명 미만인 고객입니다.|
|상위 관리 되지 않는 계산 기준   |상위 관리 되지 않는 고객-계산|
|상위 관리 되지 않는 사용자 기반| 상위 관리 되지 않는 고객 – 사용자|
|IsNonProfit|   비영리 또는 수익이 있는지 여부 (예/아니요)|
|디지털 판매-M365 크기 >= 25 명 (SalesPro 성향 Model)을 활성화 합니다.|   D365 없는 고객. 좌석 크기: 25 +. 파트너는 D365 Salespro의 교차 판매를 대상으로 해야 합니다.|
|디지털 판매 활성화-D365 SalesPro 성향 (Act Now/Evaluate) |D365 없는 High 성향 고객.  파트너는 D365 SalesPro를 대상으로 해야 합니다.|
|프레미스 설치 Navision (BC 성향 Model) & 금융 위험 관리|온-프레미스 Navision를 사용 하는 기존 고객.  파트너는 D365 BC를 대상으로 해야 합니다.|
|프레미스 설치 기본-AX (F&O 성향 Model) & 금융 위험 관리    |온-프레미스 AX를 사용 하는 기존 고객.  파트너는 D365 F&O를 대상으로 해야 합니다.|
|금융 위험 관리 & 사기 프레미스 설치 기본-뛰어난 Plains (BC 성향 Model)|  온-프레미스 훌륭한 Plains가 있는 기존 고객.  파트너는 D365 BC를 대상으로 해야 합니다.|
|프레미스 설치 기본-솔로몬 (BC 성향 Model) & 금융 위험 관리|온-프레미스 솔로몬를 사용 하는 기존 고객.  파트너는 D365 BC를 대상으로 해야 합니다.|
|프레미스 설치 기본-기타 (BC 성향 Model) & 금융 위험 관리 |위에 나열 되지 않은 다른 온-프레미스 솔루션을 사용 하는 기존 고객  파트너는 D365 BC를 대상으로 해야 합니다.|
|Agile 비즈니스 프로세스 빌드-Dynamics 온-프레미스 Install Base-AX/GP/SL/NAV/Other (D365 성향 Model)|   Agile 비즈니스 프로세스 빌드-Dynamics 온-프레미스 Install Base-AX/GP/SL/NAV/Other (D365 성향 Model)|
|Agile 비즈니스 프로세스 빌드-Dynamics 경합 베이스-Mendix/Outsystems/Salesforce (D365 성향 Model)| Agile 비즈니스 프로세스 빌드-Dynamics 경합 베이스-Mendix/Outsystems/Salesforce (D365 성향 Model)|
|Agile 비즈니스 프로세스 빌드-D365 F&O 설치 기반 |기존 D365 F&O 고객.  Power Apps를 대상으로 하는 파트너입니다.|
|Agile 비즈니스 프로세스 빌드-D365 BC 설치 기반| 기존 D365 BC 고객. Power Apps를 대상으로 하는 파트너입니다.|
|Agile 비즈니스 프로세스 빌드-D365 CE 설치 기반| 기존 D365 CE 고객. Power Apps를 대상으로 하는 파트너입니다.|
|복원 력 있는 공급망 빌드-Win and Activate First D365 워크 로드를 비 Oracle/SAP ERP 고객과 함께 D365 공급망으로 활성화|  D365 공급망에 대 한 대상 고객입니다.|
|복원 력 있는 공급망 빌드-기존 D365 CE 고객에 대 한 교차 판매 D365 공급망 및/또는 소매/상거래 |기존 D365 CE 고객이 교차 판매 D365 공급망을 대상으로 합니다.|
|복원 력 있는 공급망을 빌드합니다. D365 Sup를 교차 판매 합니다. D365 CE 및 (Oracle 또는 SAP)로의 체인 및/또는 소매/상거래| D365 공급망을 대상으로 하는 Oracle 또는 SAP를 대상으로 하는 기존 D365 CE 고객|
|D365BCCluster| 이는 고객의 성향 D365 Business Central 구매를 식별 합니다.  BC for BC를 표시 하는 고객은 중간 및 작은 범주에 성향.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|D365BCFit| Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다.|
|D365BCIntent|  소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다. 의도 점수 매기기는 매월 업데이트 됩니다.|
|D365FOCluster| 이는 고객의 성향 D365 재무 및 운영 구매를 식별 합니다.  F&O에 대 한 성향를 표시 하는 고객은 관리 되지 않는 상위 범주에 있습니다. 이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|D365FOFit| Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다.|
|D365FOIntent|  소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다. 의도 점수 매기기는 매월 업데이트 됩니다.|
|D365CECluster| 고객이 D365 고객 참여를 구매 하는 고객의 성향을 식별 합니다.  CE 용 성향을 표시 하는 고객은 중간 및 작은 범주에 있습니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|D365CEFit| D365 CE에 맞게|
|D365CEIntent|  D365 CE의 의도|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  고객이 Dynamics 온-프레미스 AX 또는 CRM에 대 한 오픈 갱신을 보유 하 고 있는지 여부를 식별 합니다.|
|M365UpsellCustomer|    고객이 상향 판매 성향 for M365를 표시 하는지 여부를 식별 합니다.|
|Google 포함|    이 플래그는 고객이 소유 하 고 있는 Google 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|AWS|   이 플래그는 고객이 소유 하 고 있는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|EA 있음 |이는 갱신이 EA (기업 계약) 인지 EA 구독 인지를 식별 합니다.|
|열림|  이는 갱신이 오픈 값 계약 인지 여부를 식별 합니다.|

**Cloud Ascent-Azure 성향**: Cloud Ascent-Azure 성향 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

|**열 이름** |**데이터 설명** |
|---------|:---------|
|MPN ID|    Microsoft 파트너 네트워크 ID|
|파트너 이름|  파트너의 이름입니다.|
|고객 ID|   고객 식별자 번호 |
|DUNS 번호|   성향에 대해 점수가 매겨진 고객의 Dun & Bradstreet 번호|
|계정 이름|  계정 이름 |
|도메인|    계정의 도메인|
|조직 크기|  조직의 규모|
|업종|  업종  |
|Vertical|  Microsoft 및 기타 업계 표준 (D&B)으로 식별 된 성향 점수가 매겨진 고객의 세로|
|영역|  위치의 지리적 영역|
|자회사|    성향에 대해 점수가 매겨진 고객의 자회사|
|Sales Territory|   Sales Territory|
|구/군/시|  지리적 위치 |
|주| 지리적 상태 위치|
|우편 번호|   우편 번호|
|국가|   지리적 국가 위치 |
|Segment|   시장 부문 |
|하위 세그먼트|   시장 서브 부문 |
|SMC 유형 요약|  SMC 유형 |
|상위 관리 되지 않는 계산 기준|  상위 관리 되지 않는 고객-계산|
|상위 관리 되지 않는 사용자 기반| 상위 관리 되지 않는 고객 – 사용자|
|IsNonProfit|   비영리 또는 수익이 있는지 여부 (예/아니요)|
|IB-성향 + 라이선스를 사용 하 여 Windows Server를 사용 하는 Windows Server 마이그레이션-EOS Win Server|   EOS (프레미스 Win Server 이전 버전 및 포함 하는 이전 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 점수가 성향 고객입니다.  파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|IB <성향를 사용 하 여 Windows Server를 사용 하 여 Windows Server-EOS Win Server 마이그레이션|   EOS (서비스 종료) 온-프레미스 Win Server (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 고객이 라이선스를 5 개 미만으로 보유 합니다. 점수가 성향 고객입니다.  파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|IB 성향 + 라이선스를 사용 하지 않고 Windows Server를 사용 하 여 Windows Server를 마이그레이션합니다. |EOS (프레미스 Win Server 이전 버전 및 포함 하는 이전 버전)가 있는 고객입니다. 고객이 라이선스를 5 개 이상 보유 합니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|IB 성향 <5 라이선스를 사용 하지 않고 Windows Server를 사용 하 여 Windows Server를 마이그레이션합니다.|    EOS (프레미스 Win Server 이전 버전 및 포함 하는 이전 버전)가 있는 고객입니다. 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|IB-성향 + 라이선스를 사용 하 여를 사용 하는 eos SQL-EOS SQL Server|  EOS 온-프레미스 SQL Server (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다.  파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|IB 성향를 사용 하 여를 사용 하는 SQL Server EOS ()-<5 라이선스 마이그레이션|  EOS 온-프레미스 SQL Server (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 라이선스가 5 개 미만입니다. 점수가 성향 고객입니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|IB 성향 + 라이선스를 사용 하지 않고를 사용 하 여 eos (SQL Server EOS)를 마이그레이션합니다.|   EOS 온-프레미스 SQL Server (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|성향-<5 라이선스를 사용 하지 않고 IB를 SQL Server 사용 하 여을 마이그레이션합니다.|   EOS 온-프레미스 SQL Server (즉, 이전 버전 및 EOS 제품을 포함 하는 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-프레미스 Win Server 마이그레이션-현재 Windows Server IB (CLAS 성향 + 라이선스 포함)|   현재 온-프레미스 Win Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-프레미스 Win Server 마이그레이션-현재 Windows Server IB 및 CLAS 성향-<5 라이선스|   현재 온-프레미스 Win Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게는 Azure에 대 한 성향 점수가 있습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-프레미스 Win Server 마이그레이션-현재 Windows Server IB (CLAS 성향 이상 라이선스 제외)|    현재 온-프레미스 Win Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-프레미스 Win Server 마이그레이션-현재 Windows Server IB (CLAS 성향-<5 라이선스 제외) |현재 온-프레미스 Win Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-CLAS 성향 + 라이선스를 사용 하 여 현재 SQL Server IB|  현재 온-프레미스 SQL Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게는 성향 점수가 있습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-CLAS 성향-<5 라이선스로 IB를 사용 하 여 현재 SQL Server|  현재 온-프레미스 SQL Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게는 성향 점수가 있습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-성향를 사용 하지 않고 현재 SQL Server IB + 라이선스|   현재 온-프레미스 SQL Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객에 게 5 개 이상의 라이선스가 있습니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-Azure SQL 또는 SQL Vm으로 마이그레이션-성향를 사용 하지 않고 IB를 사용 하 여 현재 SQL Server <5 개 라이선스|   현재 온-프레미스 SQL Server (즉, EOS 제품 이후의 버전)가 있는 고객입니다. 고객의 라이선스가 5 개 미만입니다. 고객에 게 성향 점수가 없습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-OSS-OSS DB로 마이그레이션| 기존 고객에 게는 PostgreSQL, MySQL, MariaDB 등의 경쟁 제품 중 하나가 있습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-OSS-Azure의 Linux |제품을 포함 하는 기존 고객: Linux. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-SAP-Azure의 SAP|  제품을 포함 하는 기존 고객: SAP. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-WVD-RDS IB |활성 Windows 원격 데스크톱 서비스 고객을 식별 합니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-WVD-최신 작업을 Azure/WVD로 교차 판매 합니다.|   M365를 사용 하는 고객을 식별 하 고 Azure를 포함 하지 않습니다. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-VMware IB|   제품이 있는 기존 고객: VMware. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|마이그레이션-Citrix IB|   제품을 포함 하는 기존 고객: Citrix Systems. 파트너는 이러한 고객을 대상으로 하 여 Azure로 마이그레이션해야 합니다.|
|혁신-분석-Power BI IB w/high Azure 성향|   및 활성 Power BI 구독을 포함 하는 고객: Power BI 독립 실행형 Pro, Power BI-Azure 제품군, Power BI Office 제품군, Power BI 제품군-M365|
|GitHub-VisualStudio/MSDN IB를 사용 하 여 DevOps 사용|    활성 visual 스튜디오를 사용 하는 식별 된 고객|
|Win Server Standard 버전|   고객의 Windows Server Standard 구매 버전을 보여 줍니다.|
|Win Server Standard 라이선스|   고객의 Windows Server Standard 구매 라이선스 유형을 표시 합니다.|
|Win Server Data Center 버전|    고객의 Windows 데이터 센터 구매 버전이 표시 됩니다.|
|Win Server 데이터 센터 라이선스| 고객의 Windows 데이터 센터 구매 라이선스 유형을 표시 합니다.|
|AzureFit|  Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다. 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다. 점수 매기기는 분기별로 업데이트 됩니다.|
|AzureIntent|   소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다. 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다. 의도 점수 매기기는 매월 업데이트 됩니다.|
|AzureCluster|  이는 클러스터에 맞춤 및 의도 권장 사항을 통합 하 여 Azure를 구매 하는 고객의 성향을 식별 합니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|WindowsServerDataCenter_HasOpenRenewal|    고객이 windows server 데이터 센터에 대 한 오픈 갱신을 보유 하 고 있는지 여부를 식별 합니다.|
|WindowsServerStandard_HasOpenRenewal|  이는 고객에 게 windows server standard에 대 한 오픈 갱신이 있는지를 식별 합니다.|
|AzureUpsellCustomer|   고객이 Azure 용 상향 판매 성향을 표시 하는지 여부를 식별 합니다.|
|Google 포함|    이 플래그는 고객이 소유 하 고 있는 Google 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|AWS|   이 플래그는 고객이 소유 하 고 있는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|EA 있음 |이는 갱신이 EA (기업 계약) 인지 EA 구독 인지를 식별 합니다.|
|열림|  이는 갱신이 오픈 값 계약 인지 여부를 식별 합니다.|

**클라우드 Ascent-Agreement 갱신 성향**: 클라우드 어센더-규약 갱신 성향 보고서의 여러 필드에 대 한 데이터 정의는 다음과 같습니다.

|**열 이름** |**데이터 설명** |
|---------|:---------|
|MPN ID|    Microsoft 파트너 네트워크 ID|
|파트너 이름|  파트너의 이름입니다.|
|고객 ID|   고객 식별자 번호 |
|DUNS 번호|   성향에 대해 점수가 매겨진 고객의 Dun & Bradstreet 번호|
|계정 이름|  계정 이름 |
|도메인|    계정의 도메인|
|조직 크기|  조직의 규모|
|업종|  업종  |
|Vertical|  Microsoft 및 기타 업계 표준 (D&B)으로 식별 된 성향 점수가 매겨진 고객의 세로|
|영역|  위치의 지리적 영역|
|자회사|    성향에 대해 점수가 매겨진 고객의 자회사|
|Sales Territory|   Sales Territory|
|구/군/시|  지리적 위치 |
|주| 지리적 상태 위치|
|우편 번호|   우편 번호|
|국가|   지리적 국가 위치 |
|Segment|   시장 부문 |
|하위 세그먼트|   시장 서브 부문 |
|SMC 유형 요약|  SMC 유형 |
|상위 관리 되지 않는 계산 기준|  상위 관리 되지 않는 고객-계산|
|상위 관리 되지 않는 사용자 기반| 상위 관리 되지 않는 고객 – 사용자|
|IsNonProfit|비영리 또는 수익이 있는지 여부 (예/아니요)|
|Google 포함|이 플래그는 고객이 소유 하 고 있는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|AWS|이 플래그는 고객이 소유 하 고 있는 AWS 제품에 대 한 경쟁 신호를 표시 하는지 여부를 식별 합니다.|
|Azure 클러스터|이는 고객의 성향을 식별 하 여 Azure를 구매 합니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|D365 F&O 클러스터|  이는 고객의 성향 D365 재무 및 운영 구매를 식별 합니다.  F&O에 대 한 성향를 표시 하는 고객은 관리 되지 않는 상위 범주에 있습니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|D365 CE 클러스터|   고객이 D365 고객 참여를 구매 하는 고객의 성향을 식별 합니다.  CE 용 성향을 표시 하는 고객은 중간 및 작은 범주에 있습니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|D365 BC 클러스터|   이는 고객의 성향 D365 Business Central 구매를 식별 합니다.  BC for BC를 표시 하는 고객은 중간 및 작은 범주에 성향.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|M365 클러스터|  이는 고객의 성향 M365 구매를 식별 합니다.  이제 클러스터를 작동 하 고 평가를 대상으로 지정 하 여 더 높은 수익률을 생성 해야 합니다.  키우십시오 및 교육 고객은 현재 Act를 대상으로 하 고 고객을 평가 하는 경우에도 여전히 용량이 있는 경우 대상으로 지정 해야 합니다.|
|라이선스 프로그램|   갱신에 대 한 라이선스 프로그램 유형을 식별 합니다.|
|규약 ID|  규약 식별자|
|계약 종료 날짜|    계약 종료 날짜 |
|만료 유형|   만료 유형|
|만료 되는 수익|  구독 만료와 관련 된 수익|
|EA 있음|    이는 갱신이 EA (기업 계약) 인지 EA 구독 인지를 식별 합니다.|
|열림|  이는 갱신이 오픈 값 계약 인지 여부를 식별 합니다.|
|Azure 상향 판매 고객| 고객이 Azure 용 상향 판매 성향을 표시 하는지 여부를 식별 합니다.|
|M365 상향 판매 고객|  고객이 상향 판매 성향 for M365를 표시 하는지 여부를 식별 합니다.|
|RevSumDivisionName|    갱신에 대 한 제품을 식별 합니다.|

## <a name="next-steps"></a>다음 단계

보고서는 [보고서 다운로드](pci-download-reports.md)를 참조 하세요.
