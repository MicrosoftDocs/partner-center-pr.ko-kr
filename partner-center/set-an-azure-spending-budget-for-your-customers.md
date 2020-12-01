---
title: 고객에 대 한 Azure 지출 예산 설정
ms.topic: how-to
ms.date: 06/03/2020
description: 고객에 대 한 월간 Azure 지출 예산을 설정 또는 제거 하는 방법과 Azure 지출 데이터를 보고 예산 관련 알림을 설정 하는 방법을 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438990"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>파트너 센터에서 고객에 대 한 월간 Azure 지출 예산 설정, 확인 또는 제거

적용 대상:

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

파트너 센터에서 [고객에 대 한 월간 Azure 지출 예산을 설정할](#set-azure-spending-budget) 수 있습니다. 이렇게 하면 고객이 Azure 지출를 관리할 수 있습니다. 이 옵션을 사용 하면 고객의 Azure 지출를 해당 월의 예산과 비교할 수 있습니다. 또한 고객은 자신의 Azure 지출에 대 한 비용을 청구 하는 데 도움이 됩니다.

> [!NOTE]  
> 이 기능은 샌드박스 또는 프로덕션 (TIP) 계정의 테스트에서 사용할 수 없습니다.

[고객에 대 한 Azure 지출 예산을 설정한](#set-azure-spending-budget)후에는 다음과 같은 방법으로 고객 사용량을 검토할 수도 있습니다. 이러한 옵션은 잘못 구성 된 서비스 또는 사기 행위를 제안할 수 있는 비정상적인 추세를 찾는 데 도움이 될 수 있습니다. 그런 다음 고객을 사용 하 여 근본 원인을 파악 하 고 비용을 관리할 수 있습니다. 필요한 경우 [고객의 예산을](#set-azure-spending-budget) 더 높은 값으로 변경할 수도 있습니다.

- [현재 Azure 지출 확인](#check-current-azure-spending)

- [고객의 예산이 예산 제한에 근접 한 경우에 대 한 전자 메일 알림 설정](#notifications-for-budget-limits)

- [사용량 기반 구독에 대해 서비스 별로 항목별 비용 보기](#itemized-costs-by-service)

또한 언제 든 지 고객에 대 한 [Azure 지출 예산을 제거할](#remove-azure-spending-budget) 수 있습니다.

## <a name="azure-spending-data"></a>Azure 지출 데이터

Azure 지출 데이터는 *예상치* 이며 *실제 청구 금액은 다를 수 있습니다*. 데이터 값에는 세금, 크레딧, 조정 또는 적용 될 수 있는 기타 요금이 *반영 되지 않습니다* .

지출 데이터는 *하루에 한 번 새로 고쳐집니다*. Azure Portal에서 계정 설정을 변경 하지 않는 한 고객은 Azure 서비스 및 리소스에 대 한 사용을 계속 하 고 요금이 부과 될 수 있습니다.

## <a name="set-azure-spending-budget"></a>Azure 지출 예산 설정

파트너 센터에서 여러 고객에 대 한 *월간 Azure 지출 예산을 설정할* 수 있습니다.

1. [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 합니다.

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

1. [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 합니다.

2. **CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.

3. **Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 예산을 제거 하려는 고객을 선택 합니다.

4. **예산 제거** 를 선택 합니다.

## <a name="check-current-azure-spending"></a>현재 Azure 지출 확인

언제 든 지 *고객의 현재 Azure 지출 및 월별 예산을 추적할* 수 있습니다.

1. [파트너 센터 대시보드에](https://partner.microsoft.com/dashboard/)로그인 합니다.

2. **CSP** 의 왼쪽 메뉴에서 **Azure 지출** 을 선택 합니다.

3. **Azure 지출** 페이지의 **Microsoft Azure 구독이 있는 고객** 에서 고객의 월간 예산, 현재 지출 예상 및 사용 된 예산 백분율에 대 한 개요를 볼 수 있습니다.

## <a name="notifications-for-budget-limits"></a>예산 제한에 대 한 알림

고객의 월간 지출을 예산 제한에 근접 한 경우에 대 한 *전자 메일 알림을 켤* 수 있습니다. 이 옵션을 켜면 고객이 매월 예산 중 80% 이상을 사용할 때 알림이 표시 됩니다. 이 옵션을 사용 하면 Azure 청구서에 대 한 정보를 유지할 수 있습니다. 전자 메일 알림을 구성 하려면:

1. 파트너 센터에 로그인합니다.

2. **설정** 으로 이동합니다.

3. **내 기본 설정** 을 선택 합니다.

4. 없는 경우 기본 설정 전자 메일 주소를 구성 합니다.

5. 알림의 기본 설정 언어를 구성 합니다.

6. **알림 기본 설정** 섹션에서 **CSP** 탭을 선택 합니다.

7. **Azure 지출** 알림에 대 한 전자 메일 옵션을 확인 하 고 **저장** 합니다.


## <a name="itemized-costs-by-service"></a>서비스 별로 항목별 비용

*사용량 기반 구독에 대해 서비스 별로 항목별 비용 (및 예상 사용량)을 볼* 수 있습니다.

1. 파트너 센터에 로그인합니다.

2. **CSP** 의 왼쪽 메뉴에서 **고객** 을 선택 합니다.

3. **고객** 페이지에서 고객의 **회사 이름을** 선택 합니다.

4. 고객의 **구독** 페이지의 **사용량 기반 구독** 에서 **구독의** 이름을 선택 합니다.

5. 구독 페이지에서 서비스 별로 **항목별 비용** 및 현재 달의 **예상 사용량** 을 검토할 수 있습니다.
