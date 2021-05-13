---
title: 청구 & 재구성 파일을 읽는 방법
ms.topic: article
ms.date: 06/05/2020
description: 청구서 & 조정 파일에 대해 알아봅니다. 청구서에는 해당 월별 기간의 프로그램, 제품 및 고객에 대한 파트너 센터 요금이 표시됩니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f16b619aba838da1d1da0c5eb13648ebb107c802
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855916"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>청구서 및 조정 파일 이해 - 파트너 센터 찾는 방법 알아보기


**적절한 역할:** 전역 관리자 | 청구 관리자 | 관리 에이전트


**청구서는** 모든 파트너 센터 요금(프로그램, 모든 제품 및 모든 고객)에 대한 **요약입니다.** 

## <a name="find-your-bill-and-reconciliation-file"></a>청구서 및 조정 파일 찾기 

파트너 센터 대시보드의 청구 페이지에서 청구서를 찾을 수 있습니다. 이 페이지에서 청구 기록, 지출 추세 및 조정 파일을 찾을 수도 있습니다. 

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/home)에 로그인합니다. 

2. 왼쪽 메뉴에서 **청구를** 선택합니다. 

3. 청구 상태 페이지에서 청구서 또는 조정 파일을 선택하여 자세한 정보를 확인합니다. 

마지막 청구서 날짜를 기준으로 계정 잔액 아래의 페이지 맨 위에서 최신 청구서에 대한 링크를 찾을 수 있습니다. 

이전 청구서는 청구 기록 섹션에서 찾을 수 있습니다. 적절한 연도를 선택한 다음, 적절한 청구 기간 옆에 있는 드롭다운 화살표를 선택합니다. 청구서(.pdf) 옆에 있는 링크를 선택하여 해당 기간의 청구서를 다운로드합니다. 

## <a name="invoice-types"></a>청구서 유형

Microsoft는 라이선스 기반 요금(예: Office 365) 및 사용량 기반 요금(예: Azure)에 대해 하나의 청구서와 일회성 요금(예: Azure RI, Marketplace 또는 Azure 플랜)에 대한 별도의 청구서를 발급합니다.

예를 들면 다음과 같습니다.  

**시나리오 1 [단일 통화]**: 파트너가 145P 제안 및 O365 라이선스를 구매했습니다.  

- 파트너는 O365 및 Azure(145p) 모두에 대한 요금을 포함하는 청구서 PDF 1개와 조정 파일 2개를 받게 됩니다.  

**시나리오 2 [단일 통화]**: 파트너가 145p 구매와 함께 Azure RI, Marketplace 및/또는 Azure 플랜을 구매했습니다.

- 파트너는 Azure에 대한 요금(145p)을 포함하는 하나의 청구서 PDF 및 조정 파일을 받게 됩니다. 

- 파트너는 Azure RI, Marketplace, Azure 요금제에 대 한 요금을 포함 하는 또 다른 청구서 PDF 및 조정 파일을 받게 됩니다. 

**시나리오 3 [다중 통화]**: 파트너는 eur의 145p 구매와 함께 DKK의 azure RI 및 Eur의 azure 계획에 대 한 구매를 가집니다.

- 파트너는 DKK의 Azure RI에 대 한 요금을 포함 하는 하나의 송장 PDF 및 조정 파일을 받습니다. 

- 파트너는 EUR의 Azure 요금제에 대 한 요금을 포함 하는 하나의 송장 PDF 및 조정 파일을 받게 됩니다. 

- 파트너는 EUR (또는 파트너 청구 통화)의 145p 제품에 대 한 요금을 포함 하는 또 다른 청구서 PDF 및 조정 파일을 받게 됩니다. 


## <a name="understanding-invoice-pdf"></a>송장 PDF 이해 

**사용량 및 라이선스 기반 요금 청구서**: Office 365 및 Azure와 같은 서비스에 대 한 요금 청구서는 선택한 청구 날짜의 2 일 (UTC) 이내에 사용할 수 있습니다.  

**Onetime 및 반복 요금 청구서**: azure RI, azure 요금제, Marketplace와 같은 서비스에 대 한 요금 청구서는 매월 8 일 이후에는 사용할 수 있습니다.  

다음은 청구서 PDF 문서에 있는 몇 가지 주요 필드입니다.

**청구서 번호**: 각 청구 기간에 대해 생성 된 청구서 문서에 대 한 고유 식별자입니다. 

**청구 기간**: 사용 및 라이선스 기반 서비스를 사용 하는 기간입니다. 

**청구서 날짜**: 청구서가 매월 생성 되는 청구 날짜 또는 기념일입니다. 

**지불 기한**: 지불을 받아야 하는 날짜입니다. 

**요금**: 각 청구 기간에 대 한 청구 통화로 인 한 금액입니다. 

**크레딧**: 크레딧 (예: SLA) 또는 구독에 대 한 변경 내용 조정 (예: 라이선스의 늘어나거나 감소). 

**지불 지침**: 지역을 기준으로 청구서를 지불 하는 방법에 대 한 설명입니다. 지불 시 청구서 번호를 반드시 포함 해야 합니다. 

청구서 파일 (일회성 요금에 대 한 필드 포함)의 모든 필드에 대 한 자세한 설명은 [청구서 파일 필드](invoice-file.md)를 참조 하세요. 

## <a name="understand-reconciliation-files"></a>조정 파일 이해

 요금에 대한 드릴다운/항목별 세부 정보를 제공하는 조정 파일은 청구서 PDF와 함께 다운로드할 수 있습니다. 조정 파일에는 고객 청구서를 만드는 데 사용할 수 있는 고객 식별자 및 구독 식별자가 포함됩니다.  [조정 파일을 사용하는 방법을 참조하여](use-the-reconciliation-files.md) 조정 파일에 대한 자세한 내용을 확인하세요. 

## <a name="next-steps"></a>다음 단계

- [조정 파일을 사용하는 방법](use-the-reconciliation-files.md)