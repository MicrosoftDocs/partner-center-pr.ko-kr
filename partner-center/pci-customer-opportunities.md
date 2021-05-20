---
title: 파트너 센터 Insights - CloudAscent Propensity 보고서
description: 파트너 센터 CloudAscent Propensity 보고서에 대해 알아봅니다. Microsoft 제품을 구매하는 고객의 전파에 대한 정보를 포함합니다.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153041"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>파트너 센터 대시보드에서 사용할 수 있는 CloudAscent Propensity 보고서

**적절한 역할:** 경영진 보고서 뷰어 | 보고서 뷰어

파트너 센터 대시보드는 CloudAscent 프로그램에서 다운로드 가능한 전파 데이터를 제공합니다. 데이터는 고객이 Microsoft 제품을 구매할 가능성을 보여줍니다.  이 문서에서는 이 데이터의 분석, 점수 매기기 사용 방법 및 그 의미에 대해 설명합니다.

## <a name="summary-definitions"></a>요약 정의

- **SMC 고객**– 전파 다운로드의 총 고객 수입니다.  고객은 레코드 파트너에 의해 식별됩니다.
- **계약 만료**– 현재 회계 연도 내에 만료 계약 수를 제공합니다.
- **만료 수익 열기**– 미해결 만료 계약과 관련된 수익입니다.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="고객 기회 요약 대시보드의 스크린샷.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB 구분

SMB(중소기업) 세그먼트는 세 개의 고유한 하위 세그먼트로 나뉩니다.

1. **관리되지 않는 상위에는** Microsoft에 가장 많은 기회를 가진 가장 큰 SMB 고객이 포함됩니다. 일반적인 상위 관리되지 않는 고객은 직원 수, 대규모 IT 예산 및 지출, Microsoft의 잠재적 수익이 많은 관리형 계정과 비슷한 특징을 공유합니다.

   다음과 같은 두 가지 방법으로 관리되지 않는 상위를 정의합니다.

   - **상위 관리되지 않는 사용자 기반**– 300명 이상의 직원이 있는 계정을 포함합니다. User-Based 계정은 처음 구매 하거나 Microsoft 365, Dynamics 365 또는 화면과 같은 사용자 기반 구독 제품을 확장 하는 데 적합 한 대상입니다.
   - **상위 관리 되지 않는 계산 기반** – Azure 잠재력이 $10k 보다 큰 계정을 포함 합니다. 계산 기반 계정에는 기존 Azure가 포함 됩니다. 미래의 연간 잠재력 및 Azure를 아직 구매 했지만 $10k 보다 더 큰 Azure가 있는 계정에 대 한 계정입니다.

2. **중간 규모 비즈니스** 는 기존 고객을 포함 하 고, 25-300 명의 직원이 있는 잠재 고객 계정을 포함 합니다.

3. **중소기업** 은 10-25 직원을 포함 하는 비즈니스를 포함 합니다.

4. **소규모 비즈니스** 는 직원 들이 1-9 인 비즈니스를 포함 합니다.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC 유형별 고객.":::

**상위 관리 되지 않는 상위** 및 **중간 규모 비즈니스** 하위 세그먼트는 microsoft 및 microsoft 파트너에 대 한 ltv (high time value) 고객을 나타냅니다. 이로 인해이 세그먼트의 증가를 추진 하는 데 중점을 두는 부분이 있습니다. 이러한 두 개의 하위 세그먼트에서 Microsoft 365를 사용 하 여 소켓을 획득 하 고 D365/Azure LOB (기간 업무) 앱을 추가로 수익 창출 하 고, Microsoft에 대 한 고급 LTV를 실현 하는 것이 더 좋습니다.

현재는 두 가지 주요 영역인 고객은 성장을 추가 합니다. sr-2. Microsoft 365를 사용 하는 클라우드 소켓을 잘 활용 하는 동시에 Dynamics 365 및 Azure에서 많은 기회를 제공 합니다.

다음 스크린샷은 4 개의 SMB 하위 세그먼트를 나타냅니다. CloudAscent는 관리 되지 않는 모든 상위 및 중간 규모 비즈니스 계정의 프로 파일링, 점수 매기기 및 모델링 우선 순위를 지정 합니다.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB subsegments의 스크린샷":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB는 machine learning 기술을 사용 하 여 관리 되지 않는 상위 및 중간 규모 비즈니스 부문에서 판매 및 마케팅 고객 예측을 구동 합니다. 신호가 어떻게 수집 되 고 성향 권장 사항으로 설정 되나요?

- **데이터 수집:** 웹 크롤러가 회사 도메인을 ping하고 블로그 게시물, 릴리스, 소셜 스트림 및 기술 포럼을 모니터링하여 수십억 개의 고객 신호를 검색하고 수집합니다.  수집된 신호 외에도 D&B, Microsoft 내부 구독 및 트랜잭션 데이터와 같은 내부 및 외부 원본 모두에서 firmographics 정보가 수집됩니다.

- **Machine Learning:** 신호는 클라우드 제품 및 클러스터별로 각 고객에 대한 영업 및 마케팅 예측의 구조적 데이터 집합을 출력하는 기계 학습 모델에 공급됩니다.  각 고객은 고객의 적합을 결정하는 Microsoft의 상위 SMB와 유사해 보이는 모델을 사용하여 점수를 매기고, 고객의 온라인 동작을 통합하는 기계 학습 알고리즘은 의도로 정의됩니다. 점수 매기기는 Microsoft Cloud Products 구매에 대한 고객의 성향을 보여 주는 클러스터로 병합됩니다.

- **최적화:** Machine Learning 시스템은 매월 트랜잭션 데이터와 구독 데이터를 분기별로 소비하여 모델을 최적화합니다.  승/손실 데이터를 사용하여 Machine Learning 알고리즘을 조정하고 클러스터 권장 사항을 MSX에서 작동하는 기회와 비교하여 모델이 예상대로 작동하는지 확인합니다.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 기계 학습의 스크린샷.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

전파 권장 사항은 어떻게 생성하나요?

웹 크롤러 및 다양한 원본에서 제공된 데이터를 통해 수집된 신호를 사용하여 펌그래픽 데이터와 고객의 소셜 미디어 신호를 통합합니다.  채점은 의도에 적합하고 점수 매기기 모델을 위해 비교 모델에서 이러한 신호와 데이터를 사용합니다.

1. 고객 계정 맞춤

   - 펌그래픽을 정의하는 내부 및 외부 데이터 포인트입니다.

   - 점수 매기기 맞춤은 가장 적합한 SMB에 유사 모델을 사용하여 고객을 비교하고 고객이 Microsoft 클라우드 제품에 적합한지 확인합니다.

   - 맞춤 점수 매기기는 분기별로 업데이트됩니다.

2. 고객 계정 의도

   - 소셜 미디어 및 고객의 온라인 동작과 관련된 신호는 의도를 정의합니다.

   - 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다.

   - 의도 점수 매기기는 매월 업데이트 됩니다.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 예측 모델":::

3. Clustering

   적합성 및 의도에 대 한 신호는 클러스터링 점수에 통합 됩니다. CloudAscent에는 네 개의 클러스터가 있습니다.

      - 현재 작업-판매 준비 고객
      - 마케팅 준비 고객 평가
      - 키우십시오-드라이브 인식 캠페인
      - 교육-의도에 대 한 교육 및 모니터링

   클러스터링을 사용 하면 사용자가 부문 요인을 기반으로 하는 특정 고객을 대상으로 지정할 수 있습니다. 예를 들어 제품, 지역, 산업 및 수직입니다.

   CloudAscent 통합 문서에서 **성향 모델** 탭은 성향 및 예상 공백 수익을 공유 합니다. 적합성 및 의도의 클러스터링을 정의 하기 위해 다음 단계를 진행 합니다.

      1. ML 모델을 사용 하 여 먼저 100의 등급에 따라 고객 맞춤 점수와 의도 점수를 계산 합니다.  정확한 점수는 ML 모델에 따라 달라 집니다.  아래 예제 점수:

         |**분류**|**점수**|
         |---------|:---------|
         |높음|75-100|
         |중간|55-74|
         |낮음|30 - 54|
         |매우 낮음|0 - 29|

      2. 위의 규칙을 사용하여 고객 적합성 및 의도 신호 모두에서 회사를 높음, 중간, 낮음 및 매우 낮음으로 분류합니다.

      3. 고객 맞춤 및 의도 신호를 2D 행렬에 그리고 각 교집합이 전파를 나타냅니다. 예를 들어 가장 높은 전파를 나타내는 High Fit + High Intent = A1입니다.

      4. 마지막으로 이러한 세그먼트는 클러스터를 구성하도록 그룹화됩니다.  예를 들어 A1, A2, A3, A4는 지금 작동 클러스터를 형성합니다.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent 모델.":::

   이러한 고객의 경우 지금 행동 및 고객 평가 대상을 지정하는 것이 좋습니다.

## <a name="cloudascent-products--models"></a>CloudAscent 제품 & 모델

다음 그래픽은 CloudAscent 내의 각 전파 모델에 대한 보기를 제공합니다.

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent propensity 모델.":::

공백 모델은 제품이 없거나 순 신규 잠재 고객인 기존 Microsoft 고객에 대한 예측으로 구성됩니다.

업셀 모델은 트랜잭션 데이터를 사용하여 Azure 및 Microsoft 365 S CPU에서 업셀 가능성을 예측합니다.

이러한 고객은 이미 Azure 또는 Microsoft 365 있으며, upsell 모델에서는 기존 SKU를 더 많이 구매할 가능성이 있음을 보여줍니다.

EOS는 Win 7, Office 2010, SQL Server 및 Windows Server에 대한 EOS(서비스 종료) 고객을 공유합니다. EOS 데이터는 MS Sales에서 가져와서 사용 가능한 경우 CloudAscent propensity 모델링으로 오버레이됩니다. EOS 데이터는 Modern Work에 있으며 Azure Sales는 재생됩니다.
