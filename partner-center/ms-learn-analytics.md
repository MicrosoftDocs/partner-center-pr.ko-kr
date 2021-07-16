---
title: 파트너 센터 Insights Microsoft Learn 분석
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 개별 교육, 완료된 모듈, 완료된 학습 경로 등에 대한 데이터를 활용하여 회사의 학습자를 추적합니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d9f9ce631fe667030638e1a9167809e3dae69830
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373872"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Microsoft Learn 분석 보고서 사용

**적절한 역할:** 전역 관리자 | MPN 파트너 관리자

[Microsoft Learn](/learn/) 보고서는 완료한 모듈 및 학습 경로를 포함하여 회사의 학습자에 대한 정보를 제공합니다. 보고서는 각 개별 학습자의 상태를 표시합니다. 회사의 전역 관리자 및 MPN 관리자는 데이터를 볼 수 있습니다.

## <a name="how-to-read-the-report"></a>보고서를 읽는 방법

### <a name="summary-charts"></a>요약 차트

이러한 차트에는 학습된 개인, 모듈 완성 및 학습 경로에 대한 개수 및 월별 누적 추세가 요약되어 있습니다.

**학습된 개인 수:** 선택한 날짜 범위 동안 하나 이상의 모듈을 완료한 모든 고유 학습자의 수입니다. 

**학습된 개인 추세 미니 차트:** 월별 활성 학습자 누적 수 

**모듈 완성 횟수:** 선택한 날짜 범위 동안 파트너 회사의 학습자가 완료한 모듈 수입니다.
예를 들어 15명의 개인이 "모듈 1"을 완료하고 동일한 15명의 개인이 "모듈 2"를 완료한 경우 모듈 완성 횟수는 30입니다. 모듈 완료 날짜는 선택한 날짜 범위에 속해야 합니다.

**모듈 완성 추세 미니 차트:** 월별 모듈 완성 누적 횟수 

**Learning 경로 완성 횟수:** 선택한 날짜 범위 동안 파트너 회사의 학습자가 Learning 경로 완성 횟수입니다.
예를 들어 Learning 경로 "경로 1"이 20명으로 완료되고 동일한 20명의 개인이 Learning 경로 "경로 2"를 완료한 경우 Learning 경로 완료 횟수는 40입니다. Learning 경로 완료 날짜는 선택한 날짜 범위 내에 있어야 합니다.

**Learning 경로 완성 추세 미니 차트:** 월별 학습 경로 완성 누적 횟수 

### <a name="trained-individuals-monthly-trend"></a>학습된 개인의 월간 추세

이 데이터는 해당 월에 처음으로 모듈을 완료한 회사 사용자의 추세입니다. 

**X축은** 선택한 시간 필터의 월입니다. 

**Y축은** 해당 월 동안 등록(모듈의 첫 번째 완료)한 활성 학습자의 수입니다. 이는 누적되지 않습니다.

### <a name="module-completions-monthly-trend"></a>모듈 완성 월별 추세

이 데이터는 해당 월 동안 모든 회사 사용자가 완료한 모듈의 추세입니다. (누적되지 않음) 

**X축은** 선택한 시간 필터의 월입니다. 

**Y축은** 해당 월 동안의 모듈 완성 횟수입니다. 이는 누적되지 않습니다.

### <a name="learning-path-completions-monthly-trend"></a>Learning 경로 완료 월별 추세

이 데이터는 해당 월 동안 회사 사용자가 완료한 학습 경로의 추세입니다. (누적되지 않음) 

**X축은** 선택한 시간 필터의 월입니다. 

**Y축은** 해당 월의 모듈 완성 횟수입니다. 이는 누적되지 않습니다.

### <a name="learning-path-completion-tabs"></a>Learning 경로 완성 탭

#### <a name="module-tab"></a>모듈 탭

이 탭에는 상위 5개 모듈 이름으로 회사에서 완료된 모듈에 대한 분석이 포함됩니다. 모듈이 연결된 제품입니다. 및 사용자 역할은 모듈과 관련이 있습니다.  

- 모듈 완성 도넛형 차트: 모듈 이름별 모듈 완성(요약 섹션에 표시된 개수)의 분석입니다.

차트의 가운데에 표시되는 숫자는 완료된 총 모듈입니다.

- 역할별 완료: 모듈 역할별 모듈 완성 분석입니다. 모듈이 여러 역할에 연결된 경우 각 역할이 모듈 완성 횟수에 추가됩니다.

차트의 가운데에 표시되는 숫자는 모듈 완성에 대한 고유 역할의 수입니다. 

- 제품별 완성: 모듈이 매핑된 제품에 의한 모듈 완성 분석입니다. 모듈이 여러 제품과 연결된 경우 각 제품이 모듈 완성 횟수에 추가됩니다.    

차트의 가운데에 표시되는 숫자는 모듈 완성을 위한 고유 제품의 수입니다.  

#### <a name="learning-path-tab"></a>Learning 경로 탭

이 탭에는 상위 5개 모듈 이름으로 회사에서 완료된 학습 경로에 대한 분석이 포함됩니다. 학습 경로가 매핑되는 제품입니다. 및 역할은 이 학습 경로와 관련이 있습니다.  

- Learning 경로 완성 도넛형 차트: 이름으로 Learning 경로 완성(요약 섹션에 표시된 개수)의 분석입니다.

- 역할별 완료: 역할별 학습 경로 완성 분석입니다. 모듈이 여러 역할에 연결된 경우 각 역할은 모듈 완료 횟수에 추가됩니다.

- 제품별 완성: 학습 경로가 매핑되는 제품별 학습 경로 완성에 대한 분석입니다. 모듈이 여러 제품과 연결된 경우 각 제품이 모듈 완성 횟수에 추가됩니다.

### <a name="completions-by-learning-individuals"></a>개인 학습을 통해 완성

여기에는 회사의 학습된 사용자와 완료된 모듈 및 학습 경로에 대한 세부 정보가 나열됩니다.

Microsoft Learn 사용자 개체 ID를 가진 학습자를 식별합니다. **모듈 탭** 아래에서 모든 학습자는 완료된 모듈을 따라 정렬됩니다. Microsoft Learn 사용자 이름, 개체 ID 및 모듈 수와 함께 표시됩니다. 사용자 이름을 사용하여 검색할 수 있습니다. 

Learning 경로 탭 아래에 학습 **경로별로** 정렬된 모든 학습자가 학습자 표시 이름, 개체 ID 및 모듈 수와 함께 표시됩니다.

사용자 개체 ID를 사용하여 학습자의 세부 정보를 얻으려면 다음을 수행합니다. 

1. [Graph 탐색기에 로그인합니다.](https://developer.microsoft.com/graph/graph-explorer ) (귀하는 회사의 Azure AD 테넌트의 전역 관리자여야 합니다.)

2. 사용자 개체 ID를 Graph 탐색기에 [강조 표시된 영역에](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) 복사합니다. 

## <a name="frequently-asked-questions-faq"></a>질문과 대답(FAQ)

1. 회사의 Learn 세부 정보를 볼 수 없습니다.

   이 보고서는 파트너 센터 계정이 있는 파트너가 사용할 수 있습니다. 아직 Partner Membership Center 이 보고서를 볼 수 없습니다.

2. 회사의 Who 이 보고서를 볼 수 있나요? 

   전역 관리자와 MPN 관리자는 보고서를 볼 수 있습니다.

3. 모든 사용자가 자신의 Microsoft Learn 계정을 파트너 센터 계정과 연결해야 합니까?

   *전역 관리자가 새 사용자를 추가한 후* 해당 사용자는 [Microsoft Learn](/learn/) 이동하여 AD(Azure Active Directory) 회사 계정 또는 회사 계정을 Learn 계정과 연결해야 합니다. 이렇게 하면 Insights Learning 탭에 올바른 과정과 기술이 표시됩니다.
   
   사용자는 다음을 수행해야 합니다.
   
   1. [Microsoft Learn](/learn/)로그인합니다.
   2. 프로필 사진을 선택한 다음, **내 프로필** 선택합니다.
   3. **설정** 을 선택합니다.
   4. **계정 관리** 에서 연결된 계정 아래에 해당 작업 **계정을 추가합니다.**

4. 이 보고서에서 MSA 계정으로 Microsoft Learn 로그인하는 모든 회사 사용자를 볼 수 있나요?

   현재 이 작업을 수행하는 가장 좋은 방법은 이러한 사용자를 Azure AD 테넌트에 추가한 다음 파트너 센터 추가하여 파트너 센터 내 프로필 **통해** Microsoft Learn 계정을 연결할 수 있도록 하는 것입니다. 

   MSA 계정을 학습에만 사용하는 사용자의 경우 가까운 시일 안에 Microsoft Learn 팀에서 업무용 메일을 Microsoft Learn 프로필에 연결할 수 있습니다. 

## <a name="next-steps"></a>다음 단계

자세한 보고서는 [파트너 센터 Insights](partner-center-insights.md)참조하세요.

>[!NOTE] 
> 이 보고서를 구동하는 원시 데이터는 Insights 대시보드의 보고서 다운로드 섹션에서 다운로드할 수 있습니다. [자세한 내용](insights-download-reports.md) 
