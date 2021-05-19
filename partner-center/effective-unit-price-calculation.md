---
title: 유효 단가 계산
ms.topic: how-to
ms.date: 04/02/2021
description: 유효 단가 및 계산 방법에 대해 알아봅니다. 이 문서에는 샘플 계산도 포함되어 있습니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147125"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure 플랜 사용량에 대한 유효 단가 계산

**적절한 역할:** 청구 관리자

## <a name="the-effective-unit-price"></a>유효 단가

유효 단가는 리소스 수준과 달리 미터 수준에서 계산되며 측정기 사용량에 따라 매일 조정됩니다.

다음 세 가지 요소를 사용하여 유효 단가를 계산합니다.

- 사용량- 청구 주기 전체에서 매일 모니터링됩니다.
- 미터에 대한 청구 가능 비용
- 계층화(해당하는 경우)

청구 주기 동안 매일 사용량을 모니터링하기 때문에 유효 단가가 변동됩니다. 사용량 계산을 중지하고 청구 기간을 닫으면 지정된 청구 주기에 대한 최종 가격을 사용할 수 있습니다. 네 번째 또는 다섯 번째 소수점 이하의 사용량에 대부분의 변경 내용이 표시됩니다.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>미터에서 계층형 가격 책정을 사용하는지 확인

측정기에서 계층형 가격 책정을 사용하는지 여부를 모르는 경우 아래 절차를 사용하여 확인합니다. 

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.
2. **판매를** 선택하고 **가격 책정 및 제안을** 선택한 **다음, Azure 플랜 가격 책정을** 선택합니다.
3. ID로 미터를 찾은 다음 가격 책정 데이터를 다운로드합니다. 

## <a name="sample-calculation"></a>샘플 계산

아래 표에서는 오픈 기간 동안 유효 단가를 계산하는 방법의 예를 제공합니다.

표에서 다음 값이 적용합니다. 

- **UP** = 리소스의 단가 = 0.868

- **Bcu** = 청구 가능한 소비 단위 (측정기)

- **BC** = 측정기 = BCU * UP * 0.85에 대 한 청구 가능 비용입니다. 이는 15%의 PEC 할인에 대 한 조정을 반영 합니다. 그런 다음 최소 금액을 청구 하기 위해 함수의 하한값을 사용 하 여 소수점이 하 두 자리로 값을 제한 합니다. 

- **유효 단가** = bcu/BC

>[!NOTE]

>참고:이 예제의 미터에는 가격 책정 또는 기타 할인이 포함 되지 않습니다. 할인 백분율 및 기타 조정의 유효 단가 요소가 있습니다.


| Date | BCU (청구 가능한 소비 단위) | BC (청구 가능 비용) | 유효 단가 |
| ------ | ----------- | ----------- | ----------- |  
| 3-8 월 | 29 | 21.39 | 0.737586206896552 |
| 10-8 월 | 210.950039 | 155.63 | 0.737757626107858 |
| 25-8 월 | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>다음 단계

- [청구 및 세금](billing.md)
