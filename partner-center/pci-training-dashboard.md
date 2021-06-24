---
title: 인사이트 학습 대시보드
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 학습 대시보드를 탐색합니다. 학습은 PCI(파트너 센터 Insights) 영역에서 사용할 수 있는 보고서 중 하나입니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 37a4f6cdce2b77f194fc91e0490e1c87ee137b43
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565103"
---
# <a name="trainings-dashboard"></a>학습 대시보드

**적절한 역할:** 경영진 보고서 뷰어 | 보고서 뷰어

교육 대시보드는 회사 직원 회사에서 수행된 인증, 평가 및 검사에 대한 인사이트를 제공합니다. 학습 대시보드에는 다음 섹션이 포함되어 있습니다.

- 요약
- 인증, 평가, 시험별로 학습 성능 분할
- 인증, 평가, 시험과 같은 자격 증명별 개인
- 활동 세부 정보

>[!NOTE] 
>이 보고서는 파트너 센터 Insights 허브에서 사용할 수 있습니다. 이 보고서를 보려면 보고서 뷰어 또는 임원 보고서 뷰어의 역할이 할당되어야 합니다. 이 보고서의 몇 가지 섹션은 경영진 보고서 뷰어인 사용자에게만 표시됩니다. Insights 보고서의 액세스 제어에 대한 자세한 내용은 [PCI 역할](pci-roles.md)을 참조하세요.

## <a name="summary"></a>요약

요약 섹션에는 학습과 관련된 다양한 성능 지표의 숫자 스냅샷 보기가 표시됩니다. 다양한 성능 지표는 인증된 개인, 인증, 시험 자격 증명이 있는 개인, 시험 자격 증명, 평가 자격 증명이 있는 개인 및 평가 자격 증명입니다. 이 섹션의 데이터는 선택한 날짜 범위에 따라 새로 고쳐집니다. 이 날짜 범위는 3개월(3M), 6개월(6M), 12개월(1Y) 또는 사용자 지정 데이터 범위(사용자 지정)일 수 있습니다. 

:::image type="content" source="images/pci/td-summary.png" alt-text="요약.":::

- **인증이 있는 개인:** 회사의 인증을 가진 개별 개인의 수를 나타냅니다.
- **인증 수:** 회사의 개인이 가져온 총 인증 수를 나타냅니다.
- **평가가 있는 개인:** 회사의 평가 자격 증명을 가진 개별 개인 수를 나타냅니다. 
- **평가 수:** 회사의 개인이 평가한 총 평가 수를 나타냅니다.
- **검사가 있는 개인:** 회사의 검사 자격 증명을 가진 개별 개인의 수를 나타냅니다. 
- **검사 횟수**: 회사의 개인이 수행 한 총 검사 수를 나타냅니다.

## <a name="training-performance"></a>학습 성능

교육 성과는 월별 개인 수와 회사의 개인이 완료한 교육을 표시합니다. 선택한 날짜 범위에 대한 차트 형식으로 인증, 평가 및 시험으로 분할됩니다. X축은 선택한 날짜 범위의 월을 나타냅니다. Y축은 선택한 학습 유형에 대해 개별 개인 수와 수행된 학습 수를 나타냅니다. 차트 위의 해당 탭을 선택하여 학습 유형별 분석을 확인합니다. 선택한 날짜 범위에 대한 .tsv 형식의 다운로드 아이콘을 통해 차트 데이터를 다운로드할 수 있습니다.

:::image type="content" source="images/pci/td-training-performance.png" alt-text="학습 성능.":::

## <a name="individuals-performance"></a>개인의 성과

개인 성과 섹션에는 선택한 날짜 범위에 대해 회사의 개인이 학습한 세부 정보가 표시됩니다. 섹션의 왼쪽 패널에서 개인의 이름을 검색하여 선택합니다. 선택한 개인에 대한 학습 세부 정보가 섹션의 오른쪽 패널에 표시됩니다.

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="Indiviual Performance.":::

>[!NOTE] 
> 개인 성능 섹션은 임원 보고서 뷰어인 사용자만 사용할 수 있습니다. 

## <a name="next-steps"></a>다음 단계

[파트너 센터 Insights의 보고서](partner-center-insights.md)

>[!NOTE] 
> 인사이트 대시보드의 보고서 다운로드 섹션에서 이 보고서를 구동하는 원시 데이터를 다운로드할 수 있습니다. [자세한 내용](pci-download-reports.md)