---
title: 고객이 CSP에서 자신의 서비스를 구입할 수 있도록 허용
description: CSP 프로그램 파트너가 파트너 센터에서 구매한 구독에 대해 Azure 예약과 같은 고유한 서비스를 구입할 수 있도록 하는 방법을 알아봅니다.
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amrava
ms.author: amrava
Keywords: 구독, 셀프 서비스 구매, 셀프 서비스 RI, RI 사용, ri 사용 안 함, 셀프 서비스, 고객 구매, 고객 권한, 고객 구매 예약 인스턴스, 고객 구입 Azure 예약, 셀프 서비스를 사용 하도록 설정
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0c507aae75dad4a1dce5dc9746ebe9f7ed48f040
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947468"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>파트너 센터에서 고객에 게 자신의 제품 또는 서비스를 구매할 수 있는 권한 부여

**적용 대상**

- 파트너 센터
- CSP 프로그램의 파트너

**적절한 역할**

- 관리 에이전트
- 영업 상담원

이 문서에서는 CSP (클라우드 솔루션 공급자) 프로그램의 파트너가 고객에 게 자신의 서비스 또는 리소스 중 일부를 구매할 수 있는 권한을 부여 하는 방법을 보여 줍니다.

CSP 프로그램의 파트너는 파트너 센터와 상용 마켓플레이스를 사용 하 여 고객을 위한 솔루션 및 서비스를 구입 하는 경우가 많습니다. 파트너는 일부 고객이 Azure Portal에서 직접 이러한 서비스를 프로 비전 할 수 있도록 허용 합니다.

예를 들면 다음과 같습니다. 파트너 센터에서 고객에 대 한 Azure 계획 구독을 구매 한다고 가정해 보겠습니다. 그런 다음 고객을 대신 하 여 해당 구독에 다른 리소스 또는 서비스를 추가 하기로 결정 합니다. 이 경우 고객의 구독 (예: 예약 된 가상 머신 인스턴스 추가)에 Azure 예약을 추가할 수 있습니다. 그런 다음 고객이 Azure Portal에서 Azure 예약 리소스를 추가로 프로 비전 하도록 허용할 수 있습니다.

이제 **고객 권한** 기능을 사용 하 여 고객에 게 Azure 리소스를 통해 더 많은 셀프 서비스 옵션을 제공 합니다. 고객에 대 한 권한을 설정 하 여 고객은 자신의 리소스 (예: 자신의 Azure 예약 구입)를 구매할 수 있습니다.  

## <a name="overview-of-customer-permissions-in-partner-center"></a>파트너 센터의 고객 권한 개요

고객 **계정** 페이지를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다. 현재이 기능은 다음을 지원 합니다.

- **Azure 예약:** 이 권한을 설정 하면 고객이 구매한 특정 Azure 구독에 대해 자신의 Azure 예약을 구매할 수 있습니다.

고객 권한을 설정 하기 전에 다음과 같은 중요 한 사항에 유의 하십시오.

- 기본적으로 고객 권한은 파트너 센터에서 자동으로 사용 하지 않도록 설정 (해제) 됩니다.

- 고객에 대 한 권한을 설정 하거나 해제 하려면 먼저 파트너 센터에서 관리 에이전트의 역할을 할당 받아야 합니다.

  판매 에이전트 또는 지원 센터 에이전트의 역할이 할당 된 파트너는 읽기 전용 액세스 권한을 가지 며 고객 권한을 설정 하거나 해제할 수 없습니다.

- 선택한 모든 고객에 대 한 사용 권한을 설정할 수 있습니다.

- 파트너 센터 대시보드 또는 [파트너 센터 api](https://docs.microsoft.com/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.

- 특정 고객에 대 한 사용 권한을 설정한 후에는 해당 고객의 이후 구매에 대 한 요금을 지불 해야 합니다. 고객이 만든 구매를 교환, 취소 또는 갱신 하려는 경우 (또는 예약의 초기 범위를 변경 하려는 경우) 스스로 스스로 작업을 수행할 수는 없습니다. 파트너는 구매를 교환 하거나, 취소 하 고, 갱신 하거나, 예약의 범위를 나중에 변경 하는 데 도움을 요청 해야 합니다.  

- 특정 고객에 대 한 사용 권한을 설정한 후에는 고객의 이후 구매에 대 한 알림이 표시 **되지** 않습니다.

- 고객의 나중에 구매한 제품은 사용자가 구입한 모든 구매와 함께 파트너 센터에 표시 됩니다. 고객의 **주문 기록** 페이지, 해당 **예약** 페이지 또는 [**활동 로그**](activity-logs.md)에서 이러한 구매를 찾을 수 있습니다.

>[!NOTE]
> 고객이 지불 하는 가격과 고객이 구매를 관리 하는 데 도움을 주는 방법에 대 한 자세한 내용은 [고객이 구매한 예약을 관리](give-customers-permission.md#help-customers-manage-reservations-they-purchase)하는 방법을 참조 하세요.

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>고객에 게 자신의 Azure 예약을 구매할 수 있는 권한 부여

Azure 예약은 할인된 요금으로 Azure 서비스를 구입할 수 있는 좋은 방법입니다. Azure 예약의 이점에 대 한 자세한 내용은 [Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations) 을 참조 하세요.

이제 이미 수행 했을 수 있으므로 고객을 대신 하 여 Azure 예약을 구매할 수 있습니다. 또는 고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여할 수 있습니다.

>[!NOTE]
> 사용자가 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하면 구매한 예약을 관리 하는 데 도움이 됩니다. 자세한 내용은 [고객이 구매한 예약 관리 지원](give-customers-permission.md#help-customers-manage-reservations-they-purchase)을 참조 하세요.

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>고객이 자신의 Azure 예약을 구매할 수 있도록 하려면

1. 고객이 대신 구매한 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 합니다.

2. 이 구독에 대 한 **소유자** 역할이 사용자에 게 할당 되었는지 확인 합니다.

3. 고객 권한 (이 기능 **을**설정)을 사용 하 여 자신의 Azure 예약을 구매 합니다.

각 단계가 아래에 나타납니다.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>고객이 기존 Azure 구독을 보유 하 고 있는지 확인

고객에 게 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하기 전에 고객이 기존 Azure 요금제 또는 Azure Global 구독을 보유 하 고 있는지 확인 해야 합니다. 고객이 파트너 센터에 현재 Azure 구독을 표시 하지 않는 경우 고객 권한을 설정 하기 전에 구독을 구입 해야 합니다.

- 고객이 이미 Azure 구독을 보유 하 고 있는지 확인 하려면 파트너 센터 대시보드에 로그인 한 다음 **CSP** 와 **고객**을 차례로 선택 합니다. 목록에서 특정 고객을 선택 합니다. 그런 다음 **구독** 을 선택 하 고 azure 요금제 또는 azure Global에 대 한 사용 빈도 기반 구독을 찾습니다.

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

5. 특정 사용자에 게 **소유자** 역할을 할당 하려면 다음 단계에 따라 [사용자를 관리자로 할당](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)합니다.

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>고객 권한을 설정 하거나 해제 하 여 자신의 Azure 예약을 구매 합니다.

고객이 기존 Azure 구독을 보유 하 고 있는지 확인 한 후 사용자에 게 해당 구독에 대 한 **소유자** 역할이 할당 되 면 고객 권한을 설정할 수 있습니다. 이러한 단계를 사용 하 여 고객 권한을 해제 (해제) 할 수도 있습니다. 파트너 센터 대시보드 또는 [파트너 센터 api](https://docs.microsoft.com/partner-center/develop/manage-customers)를 사용 하 여 고객 권한을 설정 하거나 해제할 수 있습니다.

파트너 센터에서 고객 권한을 설정 하거나 해제 하려면 다음을 수행 합니다.

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 왼쪽 탐색 메뉴에서 **CSP**, **고객**을 차례로 선택 합니다. 고객 목록이 표시 됩니다.

3. 특정 고객 이름을 선택 합니다.

4. 고객 메뉴에서 **계정** 을 선택 합니다. 고객 **계정** 페이지가 나타납니다.

5. 페이지 맨 아래에 있는 **고객 권한** 영역을 찾습니다.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="계정 페이지에 대 한 고객 권한입니다." border="true":::

6. **Azure 예약**에서 **고객이 구매할 수 있음** 옵션을 찾습니다.

7. 고객 권한을 설정 하려면이 옵션 옆의 스위치를 **on** 위치로 이동 합니다. 고객 권한을 해제 하려면 스위치를 **off** 위치로 이동 합니다.

>[!NOTE]
> 자신의 Azure 예약을 구매 하기 위해 고객의 권한을 설정할 때 발생 하는 다른 작업에 대해 알아보려면 [파트너 센터에서 고객 권한 개요](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)를 참조 하세요.
>
>고객 권한을 설정 하거나 해제 하면 활동 로그에서 각 작업을 기록 합니다. 파트너 센터 대시보드 위쪽에서 기어 아이콘을 선택 하면이 로그에 액세스할 수 있습니다. 고객 권한을 설정 하거나 해제 하는 경우 작업은 **고객 구매 권한 만들기** 또는 **고객 구매 권한 삭제** 를 활동 로그에 표시 합니다.

## <a name="help-customers-manage-reservations-they-purchase"></a>고객이 구매한 예약을 관리 하는 데 도움을 줍니다.

사용자가 자신의 Azure 예약을 구매할 수 있는 권한을 부여 하면 구매한 리소스를 보다 효율적으로 관리할 수 있습니다. 고객은 [Azure Portal](https://portal.azure.com/)에서 직접 Azure 예약의 여러 측면을 관리할 수 있습니다. CSP 구독 내에서 구매 하는 Azure 예약의 다른 몇 가지 측면을 관리 하는 데 도움이 필요 합니다.  

고객이 Azure 예약의 이러한 측면을 관리 하는 방법을 이해 하는 데 도움을 줍니다.

- 고객이 Azure 예약에 대해 지불 하는 가격
- 고객이 Azure 예약 사용을 최적화 하는 방법
- 고객이 공유 범위를 사용 하 여 예약을 구매 하면 어떻게 되나요?
- 고객이 예약을 변경, 취소 및 갱신 하거나 범위를 변경 하려는 경우 어떻게 되나요?

**가격 고객은 예약에 대 한 비용을 지불 합니다.** 고객은 이전에 CSP 파트너 청구 계정에서 구매한 구독을 기준으로 Azure 예약을 구매 합니다. 이 구독을 기준으로 구매 하는 모든 Azure 예약에 대 한 고객의 가격은 사용자에 의해 설정 됩니다. 이 가격은 Azure Portal 고객에 게 표시 되는 웹 직접 가격과 다를 수 있습니다.

**고객이 예약 사용을 최적화 하는 방법** 일부 고객은 예약 사용을 최적화 하는 방법 또는 구매 중에 예약의 초기 범위를 할당 하는 방법에 대해 자세히 알아볼 수 있습니다. 자세한 내용은 고객이 [Azure 리소스에 대 한 예약 관리](https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance)를 읽도록 요청 하세요.

**고객이 공유 범위를 사용 하 여 예약을 구매 하면 어떻게 되나요?** 고객이 이전 CSP 구독을 기반으로 하는 예약을 구매 하 고 해당 예약에 공유 범위를 할당 하는 경우 해당 고객에 게 제공 된 모든 구독에 대해 CSP가 제공 하는 모든 할인의 일치 사용에 적용 됩니다.

**고객이 수행한 구매를 교환, 취소 또는 갱신 하거나 예약의 초기 범위를 변경 하려는 경우에는 어떻게 해야 하나요?** 고객은 파트너에 게 예약의 초기 범위를 변경 하는 데 도움을 요청 해야 합니다. 또한 예약을 교환, 취소 또는 갱신 하기 위한 파트너의 도움이 필요 합니다. CSP 파트너가 구매한 구독에 기반 하 여 예약으로 이러한 작업을 수행할 수 없습니다.

## <a name="next-steps"></a>다음 단계

- [고객을 대신 하 여 Azure 예약 구입](azure-reservations-buying.md)

- [파트너 센터-Microsoft 예약 판매](azure-reservations.md)

- [고객을 대신 하 여 Azure 예약 관리](azure-reservations-manage.md)
