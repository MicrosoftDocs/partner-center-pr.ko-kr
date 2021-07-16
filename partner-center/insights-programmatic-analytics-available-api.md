---
title: 파트너 insights 데이터에 액세스 하기 위한 API 목록
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 insights 데이터에 액세스 하기 위한 API 목록입니다.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376077"
---
# <a name="available-apis-for-partner-insights-analytics"></a>파트너 통찰력 분석에 사용할 수 있는 Api

다음은 파트너 insights 분석과 관련 기능에 대 한 Api 목록입니다.

## <a name="dataset-pull-apis"></a>데이터 세트 풀하기 API

***표 1: 데이터 세트 풀하기 API***

| **API** | **기능** |
| --- | --- |
| [모든 데이터 세트 가져오기](insights-programmatic-analytics-api-get-dataset.md) | 사용 가능한 데이터 세트를 모두 가져옵니다. 데이터 세트는 테이블, 열, 메트릭, 시간 범위를 나열합니다. |
|||

## <a name="query-management-apis"></a>쿼리 관리 API

***표 2: 쿼리 관리 API***

| **API** | **기능** |
| --- | --- |
| [보고서 쿼리 만들기](insights-programmatic-access-paradigm.md#create-report-query-api) | 열과 메트릭을 내보내야 하는 데이터 세트를 정의하는 사용자 지정 쿼리를 만듭니다. |
| [보고서 쿼리 가져오기](insights-programmatic-analytics-api-get-report-queries.md) | 보고서에서 사용할 수 있는 모든 쿼리를 가져옵니다. 기본적으로 모든 시스템 및 사용자 정의 쿼리를 가져옵니다. |
| [보고서 쿼리 삭제](insights-programmatic-analytics-api-delete-report-queries.md) | 사용자 정의 쿼리를 삭제합니다. |
|||

## <a name="report-management-apis"></a>보고서 관리 API

***표 3: 보고서 관리 API***

| **API** | **기능** |
| --- | --- |
| [보고서 만들기](insights-programmatic-access-paradigm.md#create-report-api) | 정기적으로 쿼리를 실행하도록 예약합니다. |
| [보고서 쿼리 시도](insights-programmatic-analytics-api-try-report-queries.md) | 보고서 쿼리 문을 실행합니다. 데이터가 예상한 대로인지 확인하는 데 파트너가 사용할 수 있는 10개의 레코드만 반환합니다. |
| [보고서 가져오기](insights-programmatic-analytics-api-get-report.md) | 예약된 모든 보고서를 가져옵니다. |
| [보고서 업데이트](insights-programmatic-analytics-api-update-report.md) | 보고서 매개 변수를 수정합니다. |
| [보고서 삭제](insights-programmatic-analytics-api-delete-report.md) | 모든 보고서 및 보고서 실행 레코드를 삭제합니다. |
| [보고서 실행 일시 중지](insights-programmatic-analytics-api-pause-report-executions.md) | 예약된 보고서 실행을 일시 중지합니다. |
| [보고서 실행 계속](insights-programmatic-analytics-api-resume-report-executions.md) | 일시 중지된 보고서의 예약된 실행을 계속합니다. |
|||

## <a name="report-execution-pull-apis"></a>보고서 실행 풀하기 API

***표 4: 보고서 실행 풀하기 API***

| **API** | **기능** |
| --- | --- |
| [보고서 실행 가져오기](insights-programmatic-access-paradigm.md#get-report-execution-api) | 지정된 보고서에 대해 발생한 모든 실행을 가져옵니다. |
|||

## <a name="next-steps"></a>다음 단계

- [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)을 통해 API를 사용해 볼 수 있습니다.