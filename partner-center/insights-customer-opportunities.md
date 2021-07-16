---
title: 파트너 센터 Insights-cloudascent 성향 보고서
description: 파트너 센터의 CloudAscent 성향 보고서에 대해 알아봅니다. Microsoft 제품을 구매 하는 고객의 성향에 대 한 정보를 포함 합니다.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 6916d44e3f028fbfd788d3bee54671dbadd874d1
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376244"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>파트너 센터 대시보드에서 사용할 수 있는 CloudAscent 성향 보고서

**적절 한 역할**: 임원 보고서 뷰어 | 보고서 뷰어

파트너 센터 대시보드는 CloudAscent 프로그램에서 다운로드 가능한 성향 데이터를 제공 합니다. 데이터는 고객의 Microsoft 제품 구매 가능성을 보여 줍니다.  이 문서에서는 이러한 데이터의 분석, 점수 매기기 사용 방법 및 의미에 대해 설명 합니다.

## <a name="summary-definitions"></a>요약 정의

- **SMC 고객**– 성향 다운로드에 있는 고객의 총 수입니다.  고객은 레코드 파트너에 의해 식별 됩니다.
- **계약 만료**– 현재 회계 연도 내에서 만료 되는 계약 수를 제공 하 고 있습니다.
- 열린 **만료 수익**– 미해결 계약에 연결 된 수익입니다.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="고객 기회 요약 대시보드의 스크린샷":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB 조각화

SMB (중소기업) 세그먼트는 세 개의 고유한 하위 세그먼트로 나뉩니다.

1. **상위 관리 되지 않음** 에는 Microsoft에 대 한 기회가 가장 많은 대규모 SMB 고객이 포함 됩니다. 일반적으로 관리 되는 상위 관리 되지 않는 고객은 많은 직원, 대규모 IT 예산 및 지출, Microsoft에 대 한 많은 잠재적 수익을 포함 하 여 관리 되는 계정에 유사한 특성을 공유 합니다.

   다음 두 가지 방법으로 관리 되지 않는 상위 관리를 정의 합니다.

   - **상위 관리 되지 않는 사용자 기반**-300 이상의 직원이 포함 된 계정이 포함 되어 있습니다. User-Based 계정은 처음 구매 하거나 Microsoft 365, Dynamics 365 또는 화면과 같은 사용자 기반 구독 제품을 확장 하는 데 적합 한 대상입니다.
   - **상위 관리 되지 않는 계산 기반** – Azure 잠재력이 $10k 보다 큰 계정을 포함 합니다. 계산 기반 계정에는 기존 Azure가 포함 됩니다. 미래의 연간 잠재력 및 Azure를 아직 구매 했지만 $10k 보다 더 큰 Azure가 있는 계정에 대 한 계정입니다.

2. **중간 규모 비즈니스** 는 기존 고객을 포함 하 고, 25-300 명의 직원이 있는 잠재 고객 계정을 포함 합니다.

3. **중소기업** 은 10-25 직원을 포함 하는 비즈니스를 포함 합니다.

4. **소규모 비즈니스** 는 직원 들이 1-9 인 비즈니스를 포함 합니다.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="SMC 유형별 고객.":::

**상위 관리 되지 않는 상위** 및 **중간 규모 비즈니스** 하위 세그먼트는 microsoft 및 microsoft 파트너에 대 한 ltv (high time value) 고객을 나타냅니다. 이로 인해이 세그먼트의 증가를 추진 하는 데 중점을 두는 부분이 있습니다. 이러한 두 개의 하위 세그먼트에서 Microsoft 365를 사용 하 여 소켓을 획득 하 고 D365/Azure lob (기간 업무) 앱을 추가로 수익 창출 하 고, Microsoft에 대 한 고급 ltv를 실현 하는 것이 더 좋습니다.

현재는 두 가지 주요 영역인 고객은 성장을 추가 합니다. sr-2. Microsoft 365를 사용 하는 클라우드 소켓을 잘 활용 하는 동시에 Dynamics 365 및 Azure에서 많은 기회를 제공 합니다.

다음 스크린샷은 4 개의 SMB 하위 세그먼트를 나타냅니다. CloudAscent는 관리 되지 않는 모든 상위 및 중간 규모 비즈니스 계정의 프로 파일링, 점수 매기기 및 모델링 우선 순위를 지정 합니다.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="SMB subsegments의 스크린샷":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB는 machine learning 기술을 사용 하 여 관리 되지 않는 상위 및 중간 규모 비즈니스 부문에서 판매 및 마케팅 고객 예측을 구동 합니다. 신호가 어떻게 수집 되 고 성향 권장 사항으로 설정 되나요?

- **데이터 수집**: 웹 크롤러는 회사 도메인에 대해 ping을 수행 하 고, 블로그 게시물을 모니터링 하 고, 보도, 소셜 스트림 및 기술 포럼을 통해 수십억 개의 고객 신호를 검색 하 고 수집 합니다.  수집 된 신호 외에도 firmographics 정보는 D&B, Microsoft 내부 구독 및 트랜잭션 데이터와 같은 내부 및 외부 원본에서 수집 됩니다.

- **Machine Learning**: 신호는 클라우드 제품 및 클러스터에서 각 고객에 대 한 판매 및 마케팅 예측의 구조화 된 데이터 집합을 출력 하는 기계 학습 모델에 공급 됩니다.  각 고객은 고객의 적합도를 결정 하는 Microsoft의 최고 SMB에 대 한 유사 모델을 사용 하 여 점수가 매겨진 것 이며, 고객의 온라인 동작을 통합 하는 기계 학습 알고리즘이 의도 한 대로 정의 됩니다. 점수 매기기는 Microsoft 클라우드 제품을 구매 하는 고객의 성향을 보여 주는 클러스터로 병합 됩니다.

- **최적화**: Machine Learning 시스템은 매월 트랜잭션 데이터를 사용 하 고 구독 데이터를 분기별로 사용 하 여 모델을 최적화 합니다.  Machine Learning은 win/손실 데이터를 사용 하 여 알고리즘을 조정 하 고 클러스터 권장 사항을 MSX에서 수행 되는 기회와 비교 하 여 모델이 예상 대로 작동 하는지 확인 합니다.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="SMB machine learning의 스크린샷":::

## <a name="cloudascent-propensity"></a>CloudAscent 성향

성향 권장 사항은 어떻게 만들 수 있나요?

웹 크롤러 및 다양 한 소스에서 제공 된 데이터를 통해 수집 된 신호를 사용 하 여 firmographics 데이터 및 고객의 소셜 미디어 신호를 통합 합니다.  점수 매기기는 이러한 신호와 데이터를 비교 모델에서 사용 하 여 의도에 맞게 모델에 맞게 조정 합니다.

1. 고객 계정 맞춤

   - Firmographics를 정의 하는 내부 및 외부 데이터 요소입니다.

   - 맞춤 점수 매기기는 비슷한 모델을 사용 하 여 고객을 비교 하 고 Microsoft 클라우드 제품에 대 한 잠재적인 일치 여부를 확인 합니다.

   - 점수 매기기는 분기별로 업데이트 됩니다.

2. 고객 계정 의도

   - 소셜 미디어와 관련 된 신호 및 고객의 온라인 동작이 의도를 정의 합니다.

   - 의도 점수 매기기는 클러스터를 정의 하기 위해 적합 한 것 위에 중첩 됩니다.

   - 의도 점수 매기기는 매월 업데이트 됩니다.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB 예측 모델":::

3. 클러스터링

   적합성 및 의도에 대 한 신호는 클러스터링 점수에 통합 됩니다. CloudAscent에는 네 개의 클러스터가 있습니다.

      - 현재 작업-판매 준비 고객
      - 마케팅 준비 고객 평가
      - 키우십시오-드라이브 인식 캠페인
      - 교육-의도에 대 한 교육 및 모니터링

   클러스터링을 사용 하면 사용자가 부문 요인을 기반으로 하는 특정 고객을 대상으로 지정할 수 있습니다. 예를 들어 제품, 지역, 산업 및 수직입니다.

   CloudAscent 통합 문서에서 **성향 모델** 탭은 성향 및 예상 공백 수익을 공유 합니다. 적합성 및 의도의 클러스터링을 정의 하기 위해 다음 단계를 진행 합니다.

      1. ML 모델을 사용 하 여 먼저 100 규모의 고객 맞춤 점수와 의도 점수를 계산 합니다.  정확한 점수는 ML 모델에 따라 달라 집니다.  아래 예제 점수:

         |**분류**|**점수**|
         |---------|:---------|
         |높음|75-100|
         |중간|55-74|
         |낮음|30 - 54|
         |매우 낮음|0 - 29|

      2. 위의 규칙을 사용 하 여 회사를 높음, 중간, 낮음으로 분류 하 고 고객에 게 적합 한 신호를 제공 합니다.

      3. 성향를 나타내는 각 교차 영역에 대 한 고객 맞춤 및 의도 신호를 2D 행렬에 표시 합니다. 예를 들어, 최고 성향을 나타내는 높은 맞춤 + 높은 의도 = A1이 있습니다.

      4. 마지막으로 이러한 세그먼트는 클러스터를 형성 하는 그룹입니다.  예를 들어 A1, A2, A3, A4는 이제 Act 클러스터를 형성 합니다.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent 모델.":::

   이러한 고객의 경우 이제 Act를 대상으로 지정 하 고 고객을 평가 하는 것이 좋습니다.

## <a name="cloudascent-products--models"></a>CloudAscent 제품 & 모델

다음 그림은 CloudAscent 내의 각 성향 모델에 대 한 보기를 제공 합니다.

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent 성향 모델입니다.":::

공백 모델은 제품이 없는 기존 Microsoft 고객에 대 한 예측으로 구성 되 고, 그렇지 않은 경우에는 네트워크를 통해 새로운 고객을 대상으로 합니다.

상향 판매 모델은 트랜잭션 데이터를 사용 하 여 Azure 및 Microsoft 365 sku에서 상향 판매의 가능성을 예측 합니다.

이러한 고객에 게는 이미 Azure 또는 Microsoft 365이 모두 있고 상향 판매 모델에서 기존 SKU를 추가로 구매할 가능성이 있음을 보여 줍니다.

eos는 Win 7, Office 2010, SQL Server 및 Windows Server에 대 한 eos (서비스 종료) 고객을 공유 합니다. EOS 데이터는 MS Sales에서 끌어오고, 사용 가능한 경우 CloudAscent 성향 모델링에 중첩 됩니다. EOS 데이터는 최신 작업 및 Azure Sales가 재생 됩니다.
