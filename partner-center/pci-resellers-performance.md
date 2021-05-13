---
title: 파트너 센터 Insights Resellers Performance 대시보드
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 Insights의 대리점 성능 대시보드는 CSP Indirect Provider 다양한 간접 대리점의 성능에 대한 개요를 제공합니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a2a5697f19baadb5af956a745c032ce1711574d3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855236"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>파트너 센터 Insights의 Reseller Performance 대시보드

**적절한 역할:** 전역 관리자 | 관리 에이전트 | 보고서 뷰어 | 임원 보고서 뷰어

파트너 센터 Insights의 대리점 성능 대시보드는 CSP Indirect Provider 다양한 간접 대리점의 성능에 대한 개요를 제공합니다. 대시보드는 활성 상태인 대리점에 대한 데이터, 창출되는 수익 및 수익을 창출하고 있는 제품을 제공합니다. 간접 공급자는 이름으로 특정 대리점을 검색하고 대리점 성능 대시보드에서 대리점에 대한 세부 정보를 조회할 수 있습니다.

Reseller Performance 대시보드에서 다음 섹션을 볼 수 있습니다.

- 요약
- 대리점의 지리적 분산
- Resellers 추가/변동 
- Resellers 수익 추세 
- 제품별 대리점 성능
- 파트너 위치별 활성 대리점
- 수익 지역 분포 추세
- 고객 세그먼트별 대리점 성과
- Reseller MPA 서명 상태

 > [!NOTE]
 > 이 보고서는 Insights 대시보드에서 사용할 수 있습니다. 이 보고서를 보려면 전역 관리자, 계정 관리자, 보고서 뷰어 또는 임원 보고서 뷰어와 같은 파트너 센터 특정 역할이 할당되어야 합니다. 자세한 내용은 회사의 전역 관리자를 참조하세요. 이 보고서의 특정 데이터 형식은 경영진 보고서 뷰어 권한이 있는 사용자만 사용할 수 있습니다.

## <a name="summary"></a>요약

요약 섹션에서는 CSP Indirect Provider 관련된 KPI(핵심 성과 지표)의 스냅샷 보기를 제공합니다.

- 활성 대리점: 해당 월에 활성 구독이 하나 이상 있는 대리점의 수입니다.

마이크로 차트는 선택한 날짜 범위 동안 활성화 된 고유 대리점의 월 단위 추세를 표시 합니다.

- 거래 재판매인: 해당 월에 하나 이상의 구독을 판매 하는 대리점의 수입니다. 

마이크로 차트는 선택한 날짜 범위에 대해 등록 된 대리점의 월-월 추세를 표시 합니다.

- 새 대리점: 해당 월에 간접 공급자와 거래을 시작한 대리점의 수입니다. 

마이크로 차트는 선택한 날짜 범위 동안 새 대리점 총 수의 월 단위 추세를 표시 합니다.

- 청구 된 수익 USD: 해당 월 동안 대리점에서 구동 하는 USD의 수익입니다. 

마이크로 차트는 선택한 날짜 범위 동안 월-월의 수익 추세를 표시 합니다.

- 제품 별 청구 된 수익 섹션에는 판매 된 제품을 기준으로 하는 USD의 청구 된 수익에 대 한 월이 제공 됩니다. 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="대리점 성능 요약":::

## <a name="geographical-spread-of-resellers"></a>대리점의 지리적 확산

* * 지리 별 대리점 보기는 대리점의 지리적 분포를 제공 합니다. 파트너는이 위젯을 사용 하 여 다양 한 지역으로 분할 된 총 **대리점**, **새 대리점** 및 **청구 된 수익 (USD)** 을 볼 수 있습니다.

표에서 국가를 검색 하 고 선택 하 여 지도의 위치를 확대할 수 있습니다. 맵의 **홈** 옵션을 눌러 원래 뷰로 되돌립니다. 지도 위에 마우스를 가져가면 국가별로 **청구 된 수익 (USD)** 을 볼 수 있습니다. 표에서 청구 되는 필드 (USD)를 정렬할 수 있습니다.

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="지리 별 대리점 ":::

## <a name="resellers-addchurns"></a>대리점 추가/변동

이 보기는 **새 대리점**, **변동 대리점** 및 **기존 대리점** 의 수를 월 단위로 분할 하 여 제공 합니다. 

- 새 재판매인: 선택한 날짜 범위 동안 간접 공급자에 새로 등록된 재판매인 수입니다.
- 변동된 대리점: 이번 달을 제외한 지난 6개월 동안 트랜잭션이 없는 대리점 수입니다.
- 기존 대리점: 이전 달에 거래한 대리점 수입니다.

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="Resellers 추가/변동":::

## <a name="resellers-revenue-trend"></a>Resellers 수익 추세 

이 보기는 O365, D365, EMS, Power BI 및 Azure 제품별로 분할된 USD(청구 수익)의 월별 추세를 제공합니다. 전체 메트릭은 매월 다양한 제품에 대해 집계됩니다. 파트너는 이름으로 특정 대리점을 검색하고 해당 특정 대리점에 대한 데이터를 조회할 수 있습니다. 표의 청구 수익(USD) 필드는 정렬할 수 있습니다.

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="Resellers 수익 추세":::

## <a name="reseller-performance-by-products"></a>제품별 대리점 성능

이 보기는 월별로 다양한 제품의 청구 수익, 구독 수 및 라이선스 수와 같은 주요 메트릭의 분할을 제공합니다. 오른쪽의 원형 차트는 다양한 제품별 메트릭의 전체 분할을 나타내므로 파트너가 대리점에서 판매하는 다양한 제품별 분할을 빠르게 파악할 수 있습니다.

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="제품별 대리점 성능":::

## <a name="active-resellers-by-partner-locations"></a>파트너 위치별 활성 대리점

이 보기는 파트너 지리별로 활성 대리점의 분할을 제공합니다. 상위 5개 지역은 범례에 표시되고 나머지 지역은 '기타'로 분류됩니다.

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="파트너 위치별 활성 대리점":::

## <a name="revenue-geo-distribution-trend"></a>수익 지역 분포 추세

이 보기는 상위 5개 지리적으로 분할된 청구 수익(USD)의 월별 추세를 제공합니다.  나머지 수익은 ' 기타 '로 분류 됩니다.

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="수익 지역 분포 추세":::

## <a name="reseller-performance-by-customer-segment"></a>고객 부문의 재판매인 성능

이 보기를 통해 파트너는 다양 한 고객 세그먼트로 분할 된 수익 USD의 월별 추세, 구독 및 라이선스 수를 이해할 수 있습니다. 상위 5 개 고객 세그먼트가 차트에 표시 되 고 나머지는 ' 기타 '로 분류 됩니다.

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="고객 부문의 재판매인 성능":::

## <a name="reseller-mpa-signing-status"></a>대리점 MPA 서명 상태

이 보기는 MPN 심사 status, PMC to PC Migration status 등의 추가 메타 데이터와 함께 대리점의 MPA 서명 상태를 제공 합니다.

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="대리점 MPA 서명 상태":::

## <a name="next-steps"></a>다음 단계

- 자세한 보고서는 [파트너 센터 정보](partner-center-insights.md)를 참조 하세요.

>[!NOTE] 
> Insights 대시보드의 보고서 다운로드 섹션에서 원시 데이터를 다운로드 하 여이 보고서를 켤 수 있습니다. [자세한 내용](pci-download-reports.md) 
