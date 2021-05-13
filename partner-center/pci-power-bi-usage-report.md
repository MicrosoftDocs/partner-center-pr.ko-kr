---
title: 파트너 센터 insights Power BI 사용량 보고서
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 사용자가 수행 하는 작업을 확인 하 고 고객을 위해 판매 하거나 관리 하는 Power BI 구독의 사용과 관련 하 여 개선할 수 있는 위치를 확인 합니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 9626ceda405b54ea2043814fef3d7f5c81bc35af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854591"
---
# <a name="power-bi-usage-report-available-from-the-partner-center-insights-dashboard"></a>파트너 센터 Insights 대시보드에서 사용 가능한 Power BI 사용 보고서

**적절 한 역할**: 전역 관리자 | 관리 에이전트 | 보고서 뷰어 | 임원 보고서 뷰어

Power BI 사용 보고서는 고객이 판매 하거나 관리 하는 Power BI 구독에 대 한 사용 데이터를 제공 합니다. Power BI 사용 보고서에서 다음 섹션을 볼 수 있습니다.

- 요약
- 지리 별 Power BI 사용
- SKU에서 Power BI 사용
- 구독 성능
- Power BI 사용량 분포

 > [!NOTE]
 > 이 보고서는 Insights 대시보드에서 사용할 수 있습니다. 이 보고서를 보려면 전역 관리자, 계정 관리자, 보고서 뷰어 또는 임원 보고서 뷰어와 같은 파트너 센터에서 특정 역할을 할당 받아야 합니다. 자세한 내용은 회사의 전역 관리자를 참조 하세요 .이 보고서의 특정 데이터 형식은 임원 보고서 뷰어 권한이 있는 사용자만 사용할 수 있습니다.

## <a name="summary"></a>요약

요약 섹션에서는 고객을 위해 판매 하거나 관리 하는 Power BI 사용 구독과 관련 된 주요 표시기의 스냅숏 보기를 제공 합니다. 

- 사용 가능한 사용자: 선택한 시간 프레임 동안 판매 된 총 라이선스 수입니다.

   마이크로 차트는 선택한 날짜 범위에 대해 사용 가능한 좌석 수의 월 단위 추세를 제공 합니다.

- 할당 된 사용자: 선택한 시간 프레임 동안 할당 된 총 라이선스 수입니다.

   마이크로 차트는 선택한 날짜 범위 동안 할당 된 사용자 수의 월 단위 추세를 표시 합니다.

- 활성 사용자: 선택한 시간 프레임 동안 사용 된 총 라이선스 수입니다. 

   마이크로 차트는 선택한 기간 동안 월별 활성 좌석의 월 추세를 표시 합니다.

- 활성 사용량 %: 선택한 시간 프레임에 사용 가능한 시트의 백분율로 표현된 활성 시트의 총 수입니다. 

   마이크로 차트는 선택한 기간 동안 활성 사용률의 월별 추세를 표시합니다.

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="Power BI 사용 요약":::

## <a name="power-bi-usage-by-geography"></a>지리별 사용량 Power BI

**지리별 Power BI 사용량은** 고객 국가별 사용 가능한 사용자 및 활성 사용자 분포를 표현합니다. 맵의 밝은 색은 낮은 값을 나타내고 어두운 색은 더 높은 값을 나타냅니다. 확대/축소할 그리드에서 국가를 검색하고 선택할 수 있습니다.

**국가/지역** 수 테이블에는 Azure 사용량 이벤트가 생성되는 총 국가/지역이 표시됩니다.

그리드에서 국가를 검색하고 선택하여 지도의 위치를 확대/축소할 수 있습니다. 맵에서 **홈** 옵션을 선택하여 원래 보기로 되돌려야 합니다.

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="지리별 사용량 Power BI":::

## <a name="power-bi-usage-by-sku"></a>SKU별 Power BI 사용량

SKU별 Power BI 사용량은 사용 가능한 시트, 활성 시트 및 SKU별 할당된 시트의 월별 추세를 표현합니다.

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="SKU별 Power BI 사용량":::

## <a name="subscriptions-performance"></a>구독 성능

구독 성능은 고객 구독당 활성 사용량의 월별 추세를 보여 줍니다. 청구된 수익별 상위 100명의 고객에 대한 데이터가 표에 표시되며, 모든 고객을 검색하거나 원시 데이터를 다운로드하여 모든 구독에 대한 세부 정보를 볼 수 있습니다.

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="구독 성능 Power BI":::

## <a name="power-bi-usage-distribution"></a>Power BI 사용량 분포

Power BI 사용량 분포는 사용 가능한 사용자, 활성 사용자 및 S SKU별 할당된 사용자에 대한 분석을 제공합니다.

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="Power BI 사용량 분포":::

## <a name="next-steps"></a>다음 단계

- 자세한 보고서는 [파트너 센터 정보](partner-center-insights.md)를 참조 하세요.

- Insights 대시보드의 보고서 다운로드 섹션에서 원시 데이터를 다운로드 하 여이 보고서를 켤 수 있습니다. [자세한 내용](pci-download-reports.md) 
