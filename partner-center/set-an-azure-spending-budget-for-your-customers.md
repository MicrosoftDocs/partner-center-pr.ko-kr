---
title: 고객에 대한 Azure 지출 예산 설정
ms.topic: how-to
ms.date: 03/17/2021
description: 고객에 대한 월간 Azure 지출 예산을 설정하거나 제거하는 방법과 Azure 지출 데이터를 보고 예산 관련 알림을 설정하는 방법을 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855355"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>파트너 센터 고객에 대한 월간 Azure 지출 예산 설정, 확인 또는 제거

**적절한 역할:** 관리 에이전트

파트너 센터 [고객에 대한 월간 Azure 지출 예산을 설정할](#set-azure-spending-budget) 수 있습니다. 이렇게 하면 고객이 Azure 지출을 관리하는 데 도움이 됩니다. 이 옵션을 사용하면 고객의 Azure 지출을 해당 월의 예산과 비교할 수 있습니다. 또한 월별 청구서가 예상보다 높지 않도록 고객이 Azure 지출을 예산으로 책정하는 데 도움이 됩니다.

> [!NOTE]  
> 이 기능은 샌드박스 또는 TIP(프로덕션에서 테스트) 계정에서 사용할 수 없습니다.

[고객에 대한 Azure 지출 예산을 설정한](#set-azure-spending-budget)후 다음과 같은 방법으로 고객 사용량을 검토할 수도 있습니다. 이러한 옵션은 잘못 구성된 서비스 또는 사기 행위가 발생할 수 있는 비정상적인 추세를 파악하는 데 도움이 될 수 있습니다. 그런 다음 고객과 협력하여 근본 원인을 파악하고 비용을 관리할 수 있습니다. 필요한 경우 고객의 [예산을](#set-azure-spending-budget) 더 높은 금액으로 변경할 수도 있습니다.

- [현재 Azure 지출 확인](#check-current-azure-spending)

- [고객의 지출이 예산 한도에 근접하는 경우에 대한 이메일 알림을 켭니다.](#notifications-for-budget-limits)

- [사용량 기반 구독에 대한 서비스별 항목별 비용 보기](#itemized-costs-by-service)

언제든지 [고객에](#remove-azure-spending-budget) 대한 Azure 지출 예산을 제거할 수도 있습니다.

## <a name="azure-spending-data"></a>Azure 지출 데이터

Azure 지출 데이터는 *예상* 금액이며 *실제 청구 금액은 달라질 수 있습니다.* 데이터 값은 세금, 크레딧, 조정 또는 적용할 수 있는 기타 요금을 *반영하지 않습니다.*

지출 데이터는 *하루에 한 번 새로 고쳐집니다.* Azure Portal에서 계정 설정을 변경 하지 않는 한 고객은 Azure 서비스 및 리소스에 대 한 사용을 계속 하 고 요금이 부과 될 수 있습니다.

## <a name="set-azure-spending-budget"></a>Azure 지출 예산 설정

파트너 센터에서 여러 고객에 대 한 *월간 Azure 지출 예산을 설정할* 수 있습니다.

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. **CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.

3. **Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 설정 하려는 고객을 선택 합니다.

4. **월별 예산** 에 대 한 값을 입력 합니다.

5. **적용** 을 선택 하 여 변경 내용을 저장 합니다.

구독 설정에서 *개별 고객에 대 한 예산을 설정할* 수도 있습니다.

1. 파트너 센터 대시보드에 로그인합니다.

2. **CSP** 의 왼쪽 메뉴에서 **고객** 을 선택 합니다.

3. **고객** 페이지에서 고객의 **회사 이름을** 선택 합니다.

4. 고객의 **구독** 페이지의 **사용량 기반 구독** 에서 **예산 변경** 을 선택 합니다.

5. 예산 값을 입력 합니다.

6. **적용** 을 선택 하 여 변경 내용을 저장 합니다.

## <a name="remove-azure-spending-budget"></a>Azure 지출 예산 제거

파트너 센터에서 고객에 대 한 *월간 Azure 지출 예산을 제거할* 수 있습니다.

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. **CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.

3. **Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 제거 하려는 고객을 선택 합니다.

4. **예산 제거** 를 선택 합니다.

## <a name="check-current-azure-spending"></a>현재 Azure 지출 확인

언제 든 지 *고객의 현재 Azure 지출 및 월별 예산을 추적할* 수 있습니다.

1. [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. **CSP** 아래의 왼쪽 메뉴에서 **Azure 지출을** 선택합니다.

3. Azure **지출** 페이지의 Microsoft Azure **구독이 있는 고객** 아래에서 고객의 월별 예산 개요, 현재 지출 예측 및 사용된 예산의 백분율을 볼 수 있습니다.

## <a name="notifications-for-budget-limits"></a>예산 한도에 대한 알림

고객의 월별 *지출이* 예산 한도에 근접하는 경우에 대한 이메일 알림을 설정할 수 있습니다. 이 옵션을 켜면 고객이 월간 예산의 80% 이상을 사용할 때 알림이 제공됩니다. 이 옵션을 사용하면 Azure 청구서를 계속 감시할 수 있습니다. 이메일 알림을 구성하려면 다음을 수행합니다.

1. 파트너 센터에 로그인합니다.

2. **설정** 으로 이동합니다.

3. **내 기본 설정을** 선택합니다.

4. 기본 설정 이메일 주소를 구성하지 않은 경우 구성합니다.

5. 알림에 대한 기본 설정 언어를 구성합니다.

6. 알림 기본 설정 섹션에서 **CSP** **탭을** 선택합니다.

7. **Azure 지출** 알림에 대한 이메일 옵션을 확인하고 **을 저장합니다.**


## <a name="itemized-costs-by-service"></a>서비스별 항목별 비용

*사용량 기반 구독에 대한 서비스별로 항목별 비용(및 예상 사용량)을 볼* 수 있습니다.

1. 파트너 센터에 로그인합니다.

2. **CSP** 아래의 왼쪽 메뉴에서 **고객을** 선택합니다.

3. **고객** 페이지에서 고객의 **회사 이름** 를 선택합니다.

4. 고객의 **구독** 페이지의 **사용량 기반 구독에서 구독의** 이름을 선택합니다. 

5. 구독 페이지에서 서비스별 **항목별 비용** 및 이번 달의 **예상 사용량을** 검토할 수 있습니다.


## <a name="next-steps"></a>다음 단계

- [CSP의 새로운 상거래 환경 - Azure 청구](azure-plan-billing.md)
