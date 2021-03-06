---
title: 청구서 & 정찰 파일을 읽는 방법
ms.topic: article
ms.date: 06/05/2020
description: 청구서 & 조정 파일에 대해 알아봅니다. 청구서에는 해당 월간 기간의 프로그램, 제품 및 고객에 대 한 파트너 센터 요금이 표시 됩니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551200"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>청구서 및 조정 파일 이해-파트너 센터에서 해당 파일을 찾는 방법을 알아봅니다.


**적절 한 역할**: 전역 관리자 | 청구 관리자 | 관리 에이전트


**청구서** 는 **모든 파트너 센터 요금** (프로그램, 모든 제품 및 모든 고객)에 대 한 요약입니다. 

## <a name="find-your-bill-and-reconciliation-file"></a>청구서 및 조정 파일 찾기 

파트너 센터에서 대시보드의 청구 페이지에서 송장을 찾을 수 있습니다. 또한이 페이지에서 청구 내역, 지출 추세 및 조정 파일을 찾을 수 있습니다. 

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home)에 로그인합니다. 

2. 왼쪽 메뉴에서 **청구** 를 선택 합니다. 

3. 청구 상태 페이지에서 청구서 또는 조정 파일을 선택하여 자세한 정보를 확인합니다. 

마지막 청구서 날짜의 계정 잔액에서 페이지 맨 위에 있는 최신 청구서에 대 한 링크를 찾을 수 있습니다. 

청구 내역 섹션에서 이전 송장을 찾을 수 있습니다. 적절 한 연도를 선택 하 고 적절 한 청구 기간 옆에 있는 드롭다운 화살표를 선택 합니다. 청구서 (.pdf) 옆의 링크를 선택 하 여 해당 기간의 송장을 다운로드 합니다. 

## <a name="invoice-types"></a>송장 유형

Microsoft는 라이선스 기반 요금 (예: Office 365) 및 사용량 기반 요금 (예: Azure)에 대해 하나의 송장을 발급 하 고, 일회성 요금 (예: Azure RI, Marketplace 또는 Azure 요금제)에 대 한 별도의 송장을 발급 합니다.

예를 들면 다음과 같습니다.  

**시나리오 1 [단일 통화]**: 파트너가 145P 제품 및 Office 365 라이선스를 구입 했습니다.  

- 파트너는 Office 365 및 Azure (145p)의 요금을 포함 하는 하나의 송장 PDF 및 두 개의 조정 파일을 받습니다.  

**시나리오 2 [단일 통화]**: 파트너가 145p 구매와 함께 azure RI, Marketplace 및/또는 azure 요금제에 대 한 구매를 보유 하 고 있습니다.

- 파트너는 Azure (145p)의 요금을 포함 하는 하나의 송장 PDF와 하나의 조정 파일을 받습니다. 

- 파트너는 Azure reserved instance (RI), Marketplace, Azure 요금제에 대 한 요금을 포함 하는 또 다른 청구서 PDF 및 하나의 조정 파일을 받게 됩니다. 

**시나리오 3 [다중 통화]**: 파트너는 eur의 145p 구매와 함께 DKK의 azure RI 및 Eur의 azure 계획에 대 한 구매를 가집니다.

- 파트너는 DKK의 Azure RI에 대 한 요금을 포함 하는 하나의 송장 PDF와 하나의 조정 파일을 받습니다. 

- 파트너는 EUR의 Azure 요금제에 대 한 요금을 포함 하는 하나의 송장 PDF와 하나의 조정 파일을 받습니다. 

- 파트너는 EUR (또는 파트너 청구 통화)의 145p 제품에 대 한 요금을 포함 하는 또 다른 청구서 PDF 및 하나의 조정 파일을 받게 됩니다. 


## <a name="understanding-invoice-pdf"></a>송장 PDF 이해 

**사용량 및 라이선스 기반 요금 청구서**: Office 365 및 Azure와 같은 서비스에 대 한 요금 청구서는 선택한 청구 날짜의 2 일 (UTC) 이내에 사용할 수 있습니다.  

**Onetime 및 반복 요금 청구서**: azure RI, azure 요금제, Marketplace와 같은 서비스에 대 한 요금 청구서는 매월 8 일 이후 사용 가능 합니다.  

다음은 청구서 PDF 문서에 있는 몇 가지 주요 필드입니다.

**청구서 번호**: 각 청구 기간에 대해 생성 된 청구서 문서에 대 한 고유 식별자입니다. 

**청구 기간**: 사용 및 라이선스 기반 서비스를 사용 하는 기간입니다. 

**청구서 날짜**: 청구서가 매월 생성 되는 청구 날짜 또는 기념일입니다. 

**지불 기한**: 지불을 받아야 하는 날짜입니다. 

**요금**: 각 청구 기간에 대 한 청구 통화로 인 한 금액입니다. 

**크레딧**: 크레딧 (예: SLA (서비스 수준 계약)) 또는 구독에 대 한 변경 내용 (예: 라이선스의 늘어나거나 감소)을 조정 합니다. 

**지불 지침**: 지역을 기준으로 청구서를 지불 하는 방법에 대 한 설명입니다. 지불 시 청구서 번호를 반드시 포함 해야 합니다. 

청구서 파일 (일회성 요금에 대 한 필드 포함)의 모든 필드에 대 한 자세한 설명은 [청구서 파일 필드](invoice-file.md)를 참조 하세요. 

## <a name="understand-reconciliation-files"></a>조정 파일 이해

 요금 드릴 다운/항목별 세부 정보를 제공 하는 조정 파일은 청구서 PDF와 함께 다운로드할 수 있습니다. 조정 파일에는 고객 청구서를 만드는 데 사용할 수 있는 고객 식별자 및 구독 식별자가 포함 됩니다. 조정 파일에 대 한 자세한 내용은 [조정 파일을 사용 하는 방법](use-the-reconciliation-files.md)을 참조 하세요. 

## <a name="next-steps"></a>다음 단계

- [조정 파일을 사용 하는 방법](use-the-reconciliation-files.md)