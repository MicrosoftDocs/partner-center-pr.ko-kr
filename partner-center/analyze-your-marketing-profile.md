---
title: 잠재 고객 분석
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 잠재 고객 정보 페이지를 사용 하 여 대상 고객의 주의를 캡처하고 조회를 생성 하는 방법을 확인 하는 방법을 알아봅니다.
author: vikrambmsft
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 6ddb9544e0c6f6a29540fe30d03d307318ddfdf8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150219"
---
# <a name="analyze-your-leads---see-how-well-you-attract-target-customers-and-potential-referrals"></a>잠재 고객 분석 - 대상 고객과 잠재적 추천을 얼마나 잘 끌어올 수 있는지 확인
<!-- 
https://go.microsoft.com/fwlink/?linkid=849120
-->

**적절 한 역할**: 조회 관리자

조회의 **분석** 섹션 아래에 있는 **리드** 페이지를 통해 조회를 수행 하는 방법을 확인할 수 있습니다. 이러한 메트릭을 정기적으로 검토하여 주의가 필요한 추세 또는 영역을 파악하고, 비즈니스 목표를 달성하세요.

잠재 고객 insights 데이터를 보려면 파트너 센터 메뉴에서 조회로 이동 하 여 **> 잠재 고객 > 분석** 합니다.

## <a name="apply-filters"></a>필터 적용

**잠재 고객** 페이지의 맨 위 근처에서 데이터를 표시할 기간을 선택할 수 있습니다. 기본적으로 **3M**(3개월)이 선택되지만, 6개월 또는 1년의 데이터를 표시하도록 선택할 수 있습니다. **사용자 지정** 을 선택하여 특정 기간의 모든 추천에 대한 데이터를 볼 수도 있습니다.

[필터] 단추를 클릭하여 이 페이지의 모든 데이터를 고객 이름, 국가, 거래 유형, 거래 방향, 솔루션 이름 및 상태별로 필터링할 수 있는 패널을 열 수 있습니다. 다음은 세 가지 필터의 세부 정보입니다.

- **고객 이름**: 기본값은 **모두** 이지만, 하나 이상의 고객을 선택하여 데이터 범위를 제한할 수 있습니다.
- **국가**: 기본값은 **모두** 이지만, 하나 이상의 고객 국가를 선택하여 데이터 범위를 제한할 수 있습니다.
- **조회 프로그램**: 기본값은 **모두** 이지만 특정 조회 프로그램으로 데이터를 제한할 수 있습니다. 이 필터는 조직이 조회 프로그램에 등록 된 경우에만 표시 됩니다.
- **상태**: 기본값은 **모두** 이지만, 데이터 범위를 수락, 거부됨, 만료됨, 손실됨, 선택할 수 없음 등의 추천 상태 유형을 하나 이상 포함하고 있는 추천으로 제한할 수 있습니다.
- **정규화 유형**: 기본값은 **모두** 이지만 marketplace 리드 또는 우량 리더 인 조회로 데이터를 제한 하도록 선택할 수 있습니다.

아래에 나열된 모든 차트의 정보는 아래에 설명된 예외를 제외하고 선택한 날짜 범위와 모든 필터를 반영합니다. 일부 섹션에서는 특정 솔루션으로 필터링하는 것처럼 추가 필터를 적용할 수 있습니다.

## <a name="referrals-summary"></a>조회 요약

이 카드는 잠재 고객이 수행 하는 방법에 대 한 개요를 보여 줍니다.

이 차트는 총 페이지 방문 횟수, 작업 단추에 대 한 호출 수 (연락처 파트너) 클릭, 작업에 대 한 호출을 클릭 한 후 고객이 생성 한 잠재 고객 수, 선택한 기간에 대해 성공한 총 잠재 고객 수를 표시 합니다.

백분율 변경 메트릭(화살표 표시기가 있고 빨간색 또는 녹색으로 표시됨)은 **선택한 날짜 범위의 마지막 전체 월** 과 **해당 범위의 첫 번째 전체 월** 간의 차이를 나타냅니다. 예를 들어 현재 날짜가 6월 15일이고 지난 3개월의 데이터를 표시하도록 **3M** 필터를 선택했다고 가정합시다. 이 경우 이 메트릭은 5월(선택한 기간의 마지막 전체 월)과 3월(선택한 기간의 첫 번째 전체 월) 간의 차이를 보여줍니다. 선택한 날짜 범위가 지난 **3M** 이므로 5월과 3월의 데이터를 비교합니다.

:::image type="content" source="images/referrals/leadsanalyticssummary.png" alt-text="리드 분석의 요약 카드를 표시 하는 이미지입니다.":::

## <a name="conversion-funnel"></a>전환 유입 경로

이 섹션에서는 거래가 수명 주기 동안 한 상태에서 다른 상태로 어떻게 전환되는지 알려주는 시각적 표시기를 보여줍니다. 이 섹션의 기본 피벗을 기반으로 거래 볼륨 및 거래 금액(USD)에 따라 전체 수명 주기를 볼 수 있습니다. 첫 번째 섹션에는 형식에 따라 볼륨 또는 값의 시각적 표시기를 제공 하는 거래의 유형이 표시 됩니다. 또한 **과거** 에는 섹션을 수락/거절 하거나 보고서에 대해 선택한 기간에 성공/손실로 표시 하는 작업을 수행 하는 거래를 나타내는 데 사용 되는 섹션도 있습니다. 필터를 적용하여 거래의 다양한 수명 주기 동안 거래의 진행 상황을 볼 수 있습니다.

:::image type="content" source="images/referrals/leadsanalyticsfunnel.png" alt-text="추천에 대한 전환 유입 경로를 보여주는 이미지":::

## <a name="leads-by-geography"></a>지리 별 잠재 고객

이 섹션에서는 각 국가/지역에 대한 세부 정보와 함께 거래가 시작된 국가/지역이 표시됩니다. 각 국가의 거래 세부 정보에 대한 테이블 보기와 모든 국가의 지도 보기가 제공됩니다. 테이블에서 특정 국가를 클릭하거나 지도 보기를 클릭하여 특정 국가를 확대/축소할 수 있습니다.

:::image type="content" source="images/referrals/leadsanalyticsgeodistribution.png" alt-text="추천의 지리적 분포를 보여주는 이미지":::

## <a name="leads-by-program"></a>프로그램별 잠재 고객

이 테이블 및 차트 조합을 사용 하면 조회 프로그램 리더가 가장 많은 조회와 가장 높은 가치를 구동 하는 것을 확인할 수 있습니다.
테이블에는 총 잠재 고객, SLA에서 수락된 잠재 고객(24시간)(백분율 및 절대 조건 모두), 만료된 잠재 고객 및 획득 상태로 들어간 잠재 고객 및 총 잠재 고객 값(USD 통화)이 있습니다. 테이블 오른쪽에는 선택한 프로그램에 따라 총 거래 수와 거래 금액이 USD 통화로 표시되는 잠재 고객 추세 그래프도 있습니다. 기본적으로 모든 솔루션이 선택됩니다.

:::image type="content" source="images/referrals/leadsanalyticsreferralsprogram.png" alt-text="적격 조회 프로그램이 성능을 선도하는 것을 보여주는 이미지.":::

## <a name="declined--lost-reasons"></a>거절 및 실패 이유

이 섹션에서는 잠재 고객을 회사에서 **거부** 또는 **손실로** 표시하는 이유를 분석하는 데 도움이 됩니다. 이러한 표현의 옵션은 잠재 고객 닫는 동안 판매자가 거부 또는 손실로 선택한 것과 동일한 이유입니다.

:::image type="content" source="images/referrals/leadsanalyticsreasons.png" alt-text="잠재 고객 거부 또는 손실로 만들 때 파트너가 선택한 이유를 보여주는 이미지.":::

## <a name="comparison-charts"></a>비교 차트

비교 섹션은 볼륨의 여러 차원과 USD 피벗의 잠재 고객 획득 값을 기반으로 잠재 고객 관련 데이터를 비교하는 데 도움이 됩니다.
데이터를 비교할 때 선택할 수 있는 세 가지 요소는 다음과 같습니다.

- 한정 유형
- 시장
- 조회 프로그램

자격 유형을 선택하면 의 추천 성과를 마켓플레이스 잠재 고객 및 적격 잠재 고객과 비교할 수 있습니다. 시장 및 추천 프로그램 모두에 대해 성능을 비교하기 위해 최대 세 가지 옵션을 선택할 수 있습니다. 가로 막대형 차트인 첫 번째 그래프에는 주 피벗(볼륨 또는 거래 금액)을 기준으로 전달 대비 추세를 보여주는 데이터가 포함됩니다. 가로 막대형 차트의 오른쪽에는 동일한 데이터의 백분율로 분포를 표시하는 원형 차트도 있습니다.

:::image type="content" source="images/referrals/leadsanalyticscompare.png" alt-text="비교 섹션을 보여주는 이미지":::

## <a name="raw-data-table"></a>원시 데이터 테이블

잠재 고객과 관련된 모든 원시 데이터가 있는 아래 표는 수행하려는 세부 또는 사용자 지정 분석을 위해 데이터를 신속하게 **내보내는** 데 도움이 됩니다.

:::image type="content" source="images/referrals/leadsanalyticsrawdata.png" alt-text="잠재 고객에 대한 원시 데이터 테이블을 보여주는 이미지":::

## <a name="no-data"></a>데이터 없음

아래 설명된 대로 잠재 고객 분석에 액세스할 때 아래와 같은 빈 차트를 얻는 데는 여러 가지 이유가 있을 수 있습니다.

- 이 계정에 대한 데이터가 없습니다. 거래를 만들어서 이 보고서를 채워 보세요.
- 네트워크 연결 문제가 있습니다. 인터넷 연결을 확인하고 다시 시도하세요.
- 적용한 필터와 일치하는 레코드가 없습니다. 필터를 다시 설정해 보세요.
- 잠재 고객 상태 변경과 분석 보고서에서 동일한 내용이 업데이트되는 사이에 지연이 있습니다. 24시간 후에 보고서를 확인하세요.

:::image type="content" source="images/referrals/nodata.png" alt-text="잠재 고객에 대한 데이터 시각화를 표시하지 않는 이미지":::

> [!TIP]
> 공동 판매 기회가 어떻게 수행되는지 확인하려면 [공동 판매 기회 인사이트 페이지를 검토하세요.](referral-insights.md)

## <a name="next-steps"></a>다음 단계

- [잠재 고객 관리](manage-leads.md)
