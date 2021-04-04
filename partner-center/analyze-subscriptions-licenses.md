---
title: 구독 및 라이선스 분석
description: 구독 및 라이선스 분석 페이지에서 메트릭을 사용 하 여 주의가 필요한 성공 및 영역을 확인 하는 방법을 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 03/31/2021
ms.openlocfilehash: 3f84026cc6402bea71837b06a5e330f2c879a06b
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103794"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>비즈니스 결정과 새로운 목표를 추진 하는 데 도움이 되는 구독 및 라이선스 분석

**적절한 역할**

- 글로벌 관리자
- 사용자 관리 담당자
- 관리 에이전트
- 영업 상담원

데이터는 비즈니스 의사 결정을 유도 합니다. **구독 및 라이선스 분석** 페이지의 메트릭을 사용 하 여 주의가 필요한 성공 및 영역을 식별할 수 있습니다. 새 비즈니스 목표를 계획할 때이 정보를 사용 합니다.

**CSP Ttm 수익 (USD)**:이 메트릭은 파트너 위치 계정 및이 CSP 계정이 연결 된 파트너 전역 계정 (표준)에 대 한 마지막 12 개월 (ttm)의 집계 된 CSP 청구 수익 (usd)을 나타냅니다. 다른 사용자가 다른 CSP 계정을 사용 하는 경우 각각에 로그인 하 여 해당 하는 집계 TTM 수익을 확인 해야 합니다.  다운로드 세부 정보 링크를 클릭 하 여 MPN ID 당 TTM 수익 (USD)의 분석을 가져옵니다.

>[!NOTE]
>상용의 현지 통화 가격 (레거시 상거래용 FX)은 미국 달러의 +/-5% 내에서 관리 됩니다. 기존 Commerce exchange rate (FX)는 최신 상거래 환경의 Azure에서 사용 하는 청구 FX 속도와 다릅니다. 최신 상거래 청구 FX 요금은 Microsoft P&L 속도 (국채 피드의 Reuters)를 기반으로 합니다. 레거시 상거래 FX 요금은 Microsoft 기밀입니다.


보고서의 나머지 부분은 다음 제품을 기반으로 피벗할 수 있습니다.

 - **Dynamics 365**: dynamics 365 데이터  
 - **EMS**: 엔터프라이즈 관리 서비스 데이터  
 - **Microsoft 365**: Microsoft 365 데이터  
 - **Office 365**: office 365 데이터  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a>볼 수 있는 구독 및 라이선스 메트릭의 유형

다음 메트릭을 추적 합니다.

**요약**  
 - **판매 된 구독**: 지정 된 기간 동안 생성 된 구독 수  
  
 - **판매 된 라이선스**: 지정 된 기간 동안 판매 된 라이선스 수  
  
 - **30 일 내에 갱신** 되는 구독: 상태는 지정 된 기간 동안 활성 상태이 고 **Autorenew** 가 true 인 구독 수입니다.
 
 - **활성 구독**: 상태가 **활성** 인 구독  
 
 - **일시 중단 된 구독**: 일시 중단 된 구독의 수, 날짜 필터가 없습니다.  

**제품 분석**
  
 - **구독 수**: 판매 된 구독 별로 정렬 된 상위 5 개 제품  
 
 - **라이선스 수**: 정렬 된 라이선스를 기준으로 상위 5 개 제품 판매

**구독 보존**

 - **갱신 된 구독**: 지난 30 일 동안 갱신 된 구독  

**구독 변동**  
 - **새 구독**: 해당 기간의 새 구독 수 (평가판 제공 제외)  
 
 - **프로 비전 해제 구독**: 프로 비전 해제 또는 날짜별로 일시 중단 된 구독 수  

**일시 중단 된 구독** 
 
 - **일시 중단 됨** 상태의 모든 구독 목록 (평가판 제공 제외)  
  
**활성 구독**

 - 모든 활성 구독 목록  

**평가판 구독 변환**  

 - **평가판 변환**: 지정 된 기간 동안 변환에 대 한 평가를 지불한 모든 **활성** 구독 수입니다.  

**30 일 후에 종료 되는 평가판 구독**  

 - 시작 된 평가판 목록 (종료 날짜가 30 일 이내 이며 구독과 관련 된 유료 시작 날짜가 없음)  



## <a name="next-steps"></a>다음 단계

- [간접 대리점의 성능 분석](analyze-indirect-resellers.md)