---
title: 유효 단가 계산
ms.topic: how-to
ms.date: 11/10/2020
description: 유효 단가 및 계산 방법에 대해 알아봅니다. 또한이 문서에는 샘플 계산이 포함 되어 있습니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556330"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure 계획 소비에 대 한 유효 단위 가격 계산

## <a name="the-effective-unit-price"></a>유효 단가

유효 단가는 리소스 수준과 달리 미터 수준에서 계산 되며 미터 사용에 따라 매일 조정 됩니다.

다음 세 가지 요소를 사용 하 여 유효 단가를 계산 합니다.

- 사용량-청구 주기 전체에 걸쳐 매일 모니터링 됩니다.
- 측정기에 대 한 청구 가능 비용
- 계층화 (해당 하는 경우)

청구 주기 동안 매일 사용량을 모니터링 하므로 유효 단가가 변동 됩니다. 지정 된 청구 주기에 대 한 최종 가격은 소비 계산을 중지 하 고 청구 기간을 종결 한 후에 사용할 수 있습니다. 네 번째 또는 다섯 번째 소수 자릿수 뒤의 소비에 대 한 대부분의 변경 내용이 표시 됩니다.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>측정기에서 계층화 된 가격 책정을 사용 하는지 확인

측정기에서 계층화 된 가격 책정을 사용 하는지 여부를 모르는 경우 아래 절차를 사용 하 여 확인 합니다. 

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. **판매** 를 선택 하 고 **가격 책정 및 제품** 을 선택한 후 **Azure 계획 가격 책정** 을 선택 합니다.
3. ID로 측정기를 찾은 후 가격 데이터를 다운로드 합니다. 

## <a name="sample-calculation"></a>샘플 계산

아래 표에서는 여는 기간 동안 유효 단가를 계산 하는 방법의 예를 제공 합니다.

테이블에서 다음 값이 적용 됩니다. 

- **UP** = 리소스의 단가 = 0.868

- **Bcu** = 청구 가능한 소비 단위 (측정기)

- **BC** = 측정기 = BCU * UP * 0.85에 대 한 청구 가능 비용입니다. 이는 15%의 PEC 할인에 대 한 조정을 반영 합니다. 그런 다음 최소 금액을 청구 하기 위해 함수의 하한값을 사용 하 여 소수점이 하 두 자리로 값을 제한 합니다. 

- **유효 단가** = bcu/BC

>[!NOTE]
>참고:이 예제의 미터는 가격 책정의 계층을 포함 하지 않습니다.

| Date | BCU (청구 가능한 소비 단위) | BC (청구 가능 비용) | 유효 단가 |
| ------ | ----------- | ----------- | ----------- |  
| 3-8 월 | 29 | 21.39 | 0.737586206896552 |
| 10-8 월 | 210.950039 | 155.63 | 0.737757626107858 |
| 25-8 월 | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>다음 단계

- [청구 및 세금](billing.md)
