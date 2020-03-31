---
title: 청구서 읽기 | 파트너 센터
ms.topic: article
ms.date: 11/21/2019
description: 청구서는 현재 월에 대 한 모든 파트너 센터 요금 (프로그램, 제품 및 고객 전반)의 요약입니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: jasonwhowell
ms.author: jasonh
keywords: 구독 청구, 청구, 파트너 센터에서 청구, 파트너 센터 청구, 내 청구 보기, 송장, 파트너 센터 송장, CSP 송장, 내 청구서 위치
ms.localizationpriority: medium
ms.openlocfilehash: 7e5171a44ba8f23955847f6450e59b948f3c7d52
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390712"
---
# <a name="read-your-bill"></a>청구서 읽기

**적용 대상**

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

**적절한 역할**
-   전역 관리자
-   사용자 관리자
-   청구 관리자
-   관리자 에이전트
-   MPN 파트너 관리자

**청구서** 는 **현재 청구 기간**에 대 한 **모든 파트너 센터 요금** (프로그램, 모든 제품 및 모든 고객)에 대 한 요약입니다.

## <a name="invoice-types"></a>송장 유형

라이선스 기반 요금 (예: Office 365) 및 사용량 기반 요금 (예: Azure)에 대해 하나의 송장을 받게 됩니다.

일회성 요금 (예: Azure 예약 VM 인스턴스)에 대 한 별도의 송장을 받게 됩니다.

## <a name="invoice-file-fields"></a>송장 파일 필드

청구서 파일 (일회성 요금에 대 한 필드 포함)의 모든 필드에 대 한 자세한 설명은 [청구서 파일 필드](invoice-file.md)를 참조 하세요.

## <a name="find-your-bill"></a>청구서 찾기

파트너 센터에서 대시보드의 **청구** 페이지에서 송장을 찾을 수 있습니다. 또한이 페이지에서 청구 내역, 지출 추세 및 조정 파일을 찾을 수 있습니다.

1. 파트너 센터에서 대시보드에 로그인 합니다.
2. 왼쪽 메뉴에서 **청구**를 선택 합니다.
3. **청구** 페이지에서 다운로드 하려는 송장을 선택 합니다.
    - **마지막 청구서 날짜의 계정 잔액**에서 페이지 맨 위에 있는 최신 청구서에 대 한 링크를 찾을 수 있습니다.
    - **청구 내역** 섹션에서 이전 송장을 찾을 수 있습니다. 적절 한 연도를 선택 하 고 적절 한 **청구 기간**옆에 있는 드롭다운 화살표를 선택 합니다. **청구서 (.pdf)** 옆의 링크를 선택 하 여 해당 기간의 송장을 다운로드할 수 있습니다.

## <a name="understand-billing-periods"></a>청구 기간 이해

청구서는 **UTC 시간**에 선택한 청구 날짜의 2 **일** 이내에 사용할 수 있습니다.

예를 들어 9 월 12 일의 청구 날짜가 있는 경우:

- 송장 생성 프로세스는 9 월 13 일 오전 12 시에 **시작** 됩니다.
- 송장 생성 프로세스는 9 월 14 일 오전 12 시에 오전 12 시에 **수행** 됩니다.
- 9 월 15 일에 송장이 11:59PM UTC로 표시 되지 않는 경우에는 Service Level Agreement(서비스 수준 약정) (SLA)를 제외 하 고 서비스 요청을 처리 해야 합니다.

### <a name="csp-monthly-billing"></a>CSP 월간 청구

매월 청구 하도록 선택한 CSP (클라우드 솔루션 공급자) 프로그램의 파트너는 고객의 구독 (라이선스 기반 및 사용 기반 구독 모두)에 대해 체납에서 Microsoft 60 일을 청구 합니다.

## <a name="find-itemized-details-for-charges"></a>요금에 대 한 항목별 세부 정보 찾기

조정 파일을 사용 하 여 요금에 대 한 항목별 세부 정보를 이해할 수 있습니다. 조정 파일에는 고객 청구서를 만드는 데 사용할 수 있는 고객 식별자 및 구독 식별자가 포함 됩니다.

자세한 내용은 [조정 파일 사용 방법](use-the-reconciliation-files.md)을 참조하세요.
