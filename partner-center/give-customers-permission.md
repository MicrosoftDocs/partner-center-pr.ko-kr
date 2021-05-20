---
title: 고객이 CSP에서 자신의 서비스를 구매할 수 있도록 허용
description: CSP 프로그램 파트너가 고객이 파트너 센터 구매한 구독에 대해 Azure 예약과 같은 자체 서비스를 구매할 수 있도록 하는 방법을 알아봅니다.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150763"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>고객에게 파트너 센터 자신의 제품 또는 서비스를 구매할 수 있는 권한 부여

**적절한 역할:** 관리 에이전트 | 판매 에이전트

이 문서에서는 CSP(클라우드 솔루션 공급자) 프로그램의 파트너가 자신의 서비스 또는 리소스 중 일부를 구매할 수 있는 권한을 고객에게 부여하는 방법을 보여 줍니다.

CSP 프로그램의 파트너는 종종 파트너 센터 및 상업용 Marketplace를 사용하여 고객을 위한 솔루션과 서비스를 구입합니다. 그런 다음 파트너는 일부 고객이 Azure Portal 직접 이러한 서비스를 프로비전할 수 있도록 허용합니다.

예를 들면 다음과 같습니다. 파트너 센터 고객에 대한 Azure 플랜 구독을 구입한다고 가정해 보겠습니다. 그런 다음, 고객을 대신하여 해당 구독에 다른 리소스 또는 서비스를 추가하기로 결정합니다. 이 경우 고객의 구독에 Azure 예약을 추가할 수 있습니다(예: 예약된 가상 머신 인스턴스 추가). 그런 다음 고객이 Azure Portal Azure 예약 리소스를 추가로 프로비저닝하도록 허용할 수 있습니다.

이제 고객 **권한** 기능을 통해 고객에게 Azure 리소스를 통해 더 많은 셀프 서비스 옵션을 제공합니다. 고객에 대한 권한을 설정하여 고객이 자신의 리소스(예: 자신의 Azure 예약 구매)를 구매할 수 있도록 허용합니다.  

## <a name="overview-of-customer-permissions-in-partner-center"></a>파트너 센터 고객 권한 개요

고객 **계정** 페이지를 사용하여 고객 권한을 설정(또는 해제)할 수 있습니다. 현재 이 기능은 다음을 지원합니다.

- **Azure 예약:** 이 권한을 설정하면 고객이 구매한 특정 Azure 구독에 대해 자신의 Azure 예약을 구매할 수 있습니다.

고객 권한을 설정하기 전에 다음 중요한 사항에 유의하세요.

- 기본적으로 고객 권한은 파트너 센터 자동으로 비활성화(해제)됩니다.

- 고객에 대한 사용 권한을 설정(또는 해제)하려면 먼저 파트너 센터 관리 에이전트의 역할이 할당되어야 합니다.

  영업 담당자 또는 지원 센터 에이전트 역할이 할당된 파트너는 읽기 전용 액세스 권한을 가지며 고객 권한을 설정하거나 해제할 수 없습니다.

- 선택한 모든 고객에 대해 사용 권한을 설정(사용)할 수 있습니다.

- 파트너 센터 대시보드 또는 파트너 센터 API를 사용하여 고객 권한을 설정(또는 해제)할 수 [있습니다.](/partner-center/develop/manage-customers)

- 특정 고객에 대한 사용 권한을 설정(사용)한 후에는 해당 고객이 구매한 후속 구매에 대해 요금을 지불할 책임이 있습니다. 고객이 구매한 구매를 교환, 취소 또는 갱신하려는 경우(또는 예약의 초기 범위를 변경하려는 경우) 고객이 직접 교환하거나 취소하거나 갱신할 수 없습니다. 파트너는 구매를 교환, 취소 및 갱신하거나 나중에 예약 범위를 변경할 수 있도록 파트너에게 요청해야 합니다.  

- 특정 고객에 대한 사용 권한을 설정하면 고객이 나중에 구매한 내용에 대한 알림이 **없습니다.**

- 고객이 나중에 구매한 내용은 고객이 구매한 내용과 함께 파트너 센터 표시됩니다. 이러한 구매는 고객의 **주문 기록** 페이지, **예약** 페이지 또는 [**활동 로그**](activity-logs.md)에서 찾을 수 있습니다.

>[!NOTE]
> 고객이 지불할 가격 및 고객이 구매를 관리하는 방법에 대한 자세한 내용은 고객이 [구매한 예약을 관리하는 데 도움을](give-customers-permission.md#help-customers-manage-reservations-they-purchase)참조하세요.

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>고객에게 자신의 Azure 예약을 구매할 수 있는 권한 부여

Azure 예약은 할인된 요금으로 Azure 서비스를 구입할 수 있는 좋은 방법입니다. Azure 예약의 이점에 대한 자세한 내용은 [Azure Reservations란?을 참조하세요.](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

이제 이미 수행 중일 수 있는 것처럼 고객을 대신하여 Azure 예약을 구매할 수 있습니다. 또는 고객에게 자신의 Azure 예약을 구매할 수 있는 권한을 부여할 수 있습니다.

>[!NOTE]
> 고객에게 자신의 Azure 예약을 구매할 수 있는 권한을 부여한 후 구매한 모든 예약을 관리하는 데 도움을 줍니다. 자세한 내용은 [고객이 구매한 예약 관리 지원](give-customers-permission.md#help-customers-manage-reservations-they-purchase)을 참조 하세요.

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>고객이 자신의 Azure 예약을 구매할 수 있도록 하려면

1. 고객이 대신 구매한 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 합니다.

2. 이 구독에 대 한 **소유자** 역할이 사용자에 게 할당 되었는지 확인 합니다.

3. 고객 권한 (이 기능 **을** 설정)을 사용 하 여 자신의 Azure 예약을 구매 합니다.

각 단계가 아래에 나타납니다.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>고객이 기존 Azure 구독을 보유 하 고 있는지 확인

고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하기 전에 고객이 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 해야 합니다. 고객이 파트너 센터에 현재 Azure 구독을 표시 하지 않는 경우 고객 권한을 설정 하기 전에 구독을 구입 해야 합니다.

- 고객이 이미 Azure 구독을 보유 하 고 있는지 확인 하려면 파트너 센터 대시보드에 로그인 한 다음 **CSP** 와 **고객** 을 차례로 선택 합니다. 목록에서 특정 고객을 선택 합니다. 그런 다음 **구독** 을 선택 하 고 azure 요금제 또는 azure Global에 대 한 사용 빈도 기반 구독을 찾습니다.

- 고객이 기존 Azure 구독을 보유 하 고 있지 않은 경우 해당 구독을 구매할 수 있습니다. [Azure 계획 구매를](purchase-azure-plan.md)참조 하세요.

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Azure에서 고객이 올바른 역할을 할당 했는지 확인 합니다.

고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후에는 고객과 연결 된 키 사용자에 게 해당 Azure 구독에 대 한 올바른 **소유자** 역할이 할당 되었는지도 확인 해야 합니다. 사용자가 구매한 Azure 구독에 대해 Azure 예약을 구입 해야 하는 RBAC (역할 기반 액세스)입니다.

일부 파트너는 자신의 Azure 리소스를 적극적으로 관리 하 고 프로 비전 하려는 고객에 게 **소유자** 역할을 이미 할당 했을 수 있습니다. 구매한 이전 구독을 관리 하기 위해 고객에 게 **소유자** 상태를 이미 할당 한 경우이 단계를 건너뛸 수 있습니다.  

> [!IMPORTANT]
> 담당자에 게 **소유자** 역할이 할당 되지 않은 경우 Azure 예약을 구매 하지 못하도록 하는 Azure Portal 오류가 표시 됩니다.

고객에 게 Azure 구독에 대 한 **소유자** 역할이 할당 되었는지 확인 하려면 다음을 수행 합니다.

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. **CSP**, **고객** 을 차례로 선택 하 고 특정 고객을 선택 합니다.

3. 해당 고객에 대 한 **구독** 을 선택 하 고 특정 Azure 구독을 찾습니다.

4. 해당 고객의 구독 옆에 있는 **관리** 단추를 선택 합니다. 이렇게 하면 [Azure Portal](https://portal.azure.com/)열립니다.

5. 특정 사용자에 게 **소유자** 역할을 할당 하려면 다음 단계에 따라 [사용자를 관리자로 할당](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)합니다.

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>고객 권한을 설정 하거나 해제 하 여 자신의 Azure 예약을 구매 합니다.

고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후 사용자에 게 해당 구독에 대 한 **소유자** 역할이 할당 되 면 고객 권한을 설정할 수 있습니다. 이러한 단계를 사용 하 여 고객 권한을 해제 (해제) 할 수도 있습니다. 파트너 센터 대시보드 또는 [파트너 센터 api](/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.

파트너 센터에서 고객 권한을 설정 하거나 해제 하려면 다음을 수행 합니다.

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 왼쪽 탐색 메뉴에서 **CSP**, **고객** 을 차례로 선택 합니다. 고객 목록이 표시 됩니다.

3. 특정 고객 이름을 선택 합니다.

4. 고객 메뉴에서 **계정** 을 선택 합니다. 고객 **계정** 페이지가 나타납니다.

5. 페이지 맨 아래에 있는 **고객 권한** 영역을 찾습니다.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="계정 페이지에 대 한 고객 권한입니다." border="true":::

6. **Azure 예약** 에서 **고객이 구매할 수 있음** 옵션을 찾습니다.

7. 고객 권한을 켜려면 이 옵션 옆에 있는 스위치를 **켜기** 위치로 이동합니다. 고객 권한을 해제하려면 스위치를 **끄기** 위치로 이동합니다.

>[!NOTE]
> 고객의 사용 권한을 설정하여 자신의 Azure 예약을 구매할 때 발생하는 다른 일을 알아보려면 [파트너 센터 고객 권한 개요를](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)참조하세요.
>
>고객 권한을 설정(또는 해제)하면 활동 로그는 각 작업을 기록합니다. (이 로그는 파트너 센터 대시보드의 위쪽에서 기어 아이콘을 선택하면 액세스할 수 있습니다. 고객 권한을 설정하거나 해제하면 활동 로그에서 **고객 구매 권한 만들기** 또는 고객 구매 **권한 삭제로** 작업이 표시됩니다.

## <a name="help-customers-manage-reservations-they-purchase"></a>고객이 구매한 예약을 관리하는 데 도움을 주세요.

고객에게 자신의 Azure 예약을 구매할 수 있는 권한을 부여하면 구매한 리소스를 더 잘 관리할 수 있습니다. 고객은 [Azure Portal](https://portal.azure.com/)직접 Azure 예약의 여러 측면을 직접 관리할 수 있습니다. CSP 구독 내에서 구매하는 Azure 예약의 몇 가지 다른 측면을 관리하는 데 도움이 필요합니다.  

고객이 Azure 예약의 이러한 측면을 관리하는 데 대한 자세한 내용을 이해하게 합니다.

- 고객이 Azure 예약에 대해 지불하는 가격
- 고객이 Azure 예약 사용을 최적화하는 방법
- 고객이 공유 범위의 예약을 구매하면 어떻게 되나요?
- 고객이 예약을 변경, 취소 및 갱신하거나 범위를 변경하려는 경우 어떻게 되나요?

**가격 고객은 예약 비용을 지불합니다.** 고객은 CSP 파트너 청구 계정에서 이전에 구매한 구독에 따라 Azure 예약을 구매하게 됩니다. 이 구독을 기반으로 구매한 Azure 예약에 대한 고객의 가격도 설정됩니다. 이 가격은 Azure Portal 고객이 보는 웹 직접 가격과 다를 수 있습니다.

**고객이 예약 사용을 최적화할 수 있는 방법입니다.** 일부 고객은 예약 사용을 최적화 하는 방법 또는 구매 중에 예약의 초기 범위를 할당 하는 방법에 대해 자세히 알아볼 수 있습니다. 자세한 내용은 고객이 [Azure 리소스에 대 한 예약 관리](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)를 읽도록 요청 하세요.

**고객이 공유 범위를 사용 하 여 예약을 구매 하면 어떻게 되나요?** 고객이 이전 CSP 구독을 기반으로 하는 예약을 구매 하 고 해당 예약에 공유 범위를 할당 하는 경우 해당 고객에 게 제공 된 모든 구독에 대해 CSP가 제공 하는 모든 할인의 일치 사용에 적용 됩니다.

**고객이 수행한 구매를 교환, 취소 또는 갱신 하거나 예약의 초기 범위를 변경 하려는 경우에는 어떻게 해야 하나요?** 고객은 파트너에 게 예약의 초기 범위를 변경 하는 데 도움을 요청 해야 합니다. 또한 예약을 교환, 취소 또는 갱신 하기 위한 파트너의 도움이 필요 합니다. CSP 파트너가 구매한 구독에 기반 하 여 예약으로 이러한 작업을 수행할 수 없습니다.

## <a name="next-steps"></a>다음 단계

- [고객을 대신 하 여 Azure 예약 구입](azure-reservations-buying.md)

- [파트너 센터-Microsoft 예약 판매](azure-reservations.md)

- [고객을 대신 하 여 Azure 예약 관리](azure-reservations-manage.md)