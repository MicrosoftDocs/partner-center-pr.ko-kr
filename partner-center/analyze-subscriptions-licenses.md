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
ms.openlocfilehash: 45a0ebb70f6e139b1e130c3cfc1d24eb79b41a0d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150151"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>비즈니스 결정과 새로운 목표를 추진 하는 데 도움이 되는 구독 및 라이선스 분석

**적절 한 역할**: 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트 | 판매 에이전트

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
 - **판매된 구독:** 지정된 기간 동안 생성된 구독 수  
  
 - **판매된 라이선스:** 지정된 기간 동안 판매된 라이선스 수  
  
 - **30일 이내에 갱신되는 구독:** 지정된 기간 동안 상태가 활성 상태이고 **Autorenew가** true인 구독 수
 
 - **활성 구독:** 상태가 **활성인** 구독  
 
 - **일시 중단된 구독:** 일시 중단된 구독 수, 날짜 필터가 없습니다.  

**제품 분석**
  
 - **구독 수:** 판매된 구독별로 정렬된 상위 5개 제품  
 
 - **라이선스 수:** 판매된 정렬된 라이선스별 상위 5개 제품

**구독 보존**

 - **갱신된 구독:** 지난 30일 동안 갱신된 구독  

**구독 변동**  
 - **새 구독:** 기간 동안 새 구독 수(평가판 제품 제외)  
 
 - **프로비전 해제된 구독:** 날짜별로 프로비전 해제되거나 일시 중단된 구독 수  

**일시 중단된 구독** 
 
 - 평가판 제안을 제외하고 상태가 **일시 중단된** 모든 구독 목록  
  
**활성 구독**

 - 모든 활성 구독 목록  

**평가판 구독 변환**  

 - **평가판 변환:** 지정된 기간 동안 전환에 대한 평가판이 발생한 모든 **활성** 구독 수  

**평가판 구독이 30일 후에 종료됩니다.**  

 - 시작 된 평가판 목록 (종료 날짜가 30 일 이내 이며 구독과 관련 된 유료 시작 날짜가 없음)  



## <a name="next-steps"></a>다음 단계

- [간접 대리점의 성능 분석](analyze-indirect-resellers.md)