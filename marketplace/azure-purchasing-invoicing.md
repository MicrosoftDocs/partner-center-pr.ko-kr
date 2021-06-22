---
title: Azure Marketplace 소프트웨어 및 솔루션 구매
description: Azure Marketplace 소프트웨어 구매 및 관리를 간소화하고 간소화하는 도구에 대해 알아봅니다.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431555"
---
# <a name="azure-marketplace-purchasing"></a>구매 Azure Marketplace

Azure Marketplace 구매, 계산 및 구매 정책 관리 프로세스를 간소화하고 간소화하는 다양한 도구와 기능이 있습니다.

## <a name="simplified-procurement"></a>간소화된 조달

Azure Marketplace의 다양한 구매 옵션을 사용하면 조달 프로세스를 간소화하는 데 도움이 됩니다. Azure 계정과 연결된 신용 카드를 사용하여 제품을 구매하는 경우 모든 구매는 단일 청구서에 통합되고 선택한 신용 카드로 청구됩니다. 대규모 고객인 경우 기업계약 사용하여 구매할 수 있습니다. EA를 사용하면 모든 소프트웨어 구매가 Azure 청구서에 자동으로 포함됩니다. 청구서에는 먼저 Azure 사용 요금이 포함되고 그 다음에 Azure Marketplace 요금이 포함됩니다.

Azure Marketplace 통해 구매하는 경우 개별 공급업체 관계 및 청구서를 관리하는 복잡성을 제거합니다. Microsoft에서 Azure Marketplace 구매와 Azure 요금을 모두 포함하는 단일 통합 월별 청구서를 받게 됩니다.

## <a name="permission-to-purchase"></a>구매할 수 있는 권한

올바른 소프트웨어 애플리케이션을 찾은 후에는 구매를 완료하는 것이 간단합니다. 그러나 Azure 구독 내에서 적절한 권한이 필요합니다. Azure는 RBAC(역할 [기반 Access Control)](/azure/role-based-access-control/overview) 모델에서 작동하기 때문에 계정을 구매하려면 **구독 소유자** 또는 **기여자** 권한이 필요합니다.

구매를 완료하기 전에 사용자가 Azure 테넌트에서 올바른 구성을 가지고 있는지 확인합니다. 이렇게 하면 구매하는 동안 오류를 방지할 수 있습니다.

Azure Portal Azure Marketplace 경험에서 구매할 애플리케이션을 찾고 **만들기** 또는 **설정 + 구독을** 선택합니다. 새 솔루션을 사용하기 전에 일부 정보를 완료하라는 메시지가 표시됩니다.

> [!CAUTION]
> 프라이빗 마켓플레이스에 대한 승인은 솔루션 조달을 나타내지 않습니다.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="제안 만들기 단추입니다.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="설정 + 구독 단추입니다.":::

Azure Marketplace 온라인 스토어에서 솔루션을 배포하려면 제품 설명 페이지에서 **지금 받기를** 선택한 다음, Azure 계정 자격 증명으로 로그인합니다.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketplace 로그인 대화 상자입니다.":::

로그인하면 구매를 완료하기 위해 Azure Portal 제품으로 리디렉션됩니다.

## <a name="purchase-policy-management"></a>구매 정책 관리

Microsoft를 사용하면 Azure 구독 관리자로서 청구 프로필을 통해 사용자 구매를 관리할 수 있습니다. 다음 세 가지 옵션 중에서 선택합니다.

- **무료 + 유료** – 사용자가 Azure Marketplace 소프트웨어 애플리케이션을 획득할 수 있습니다.
- **무료** – 사용자가 Azure Marketplace 무료 소프트웨어만 배포할 수 있습니다.
- **아니요** – 사용자가 Azure Marketplace 소프트웨어를 배포할 수 없습니다.

이러한 설정은 Azure 구독에 액세스할 수 있는 모든 사용자에게 적용되며, 이를 통해 Azure Portal 통해 IT 조달을 제어할 수 있습니다.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure Portal 통해 IT 조달을 제어합니다.":::

## <a name="cost-management"></a>비용 관리

Azure Marketplace 제품을 구매할 때 비용을 관리하는 데 도움이 되는 인사이트를 얻고자 합니다. Azure Cost Management 구매한 제품에 대한 정보를 볼 수 있는 무료 도구입니다. Cost Management 사용하여 시간에 따라 비용을 지출하는 서비스와 해당 비용이 설정한 예산에 대해 어떻게 추적되는지에 대한 세부 정보를 볼 수 있습니다. 예산을 설정하는 것 외에도 보고서를 예약하고 구독 비용을 분석할 수 있습니다. 비용 분석 및 Azure Cost Management 예산 [만들기에서](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)Microsoft Learn 모듈을 완료하여 Azure Cost Management 대해 자세히 알아봅니다.

Azure Cost Management의 비용 분석 도구에서 Azure Marketplace 요금 및 청구서를 볼 수 있습니다.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Azure Cost Management 사용하여 구매한 제품에 대한 인사이트를 얻습니다.":::

## <a name="purchase-validation-checks"></a>구매 유효성 검사

Azure Marketplace 통해 제품을 구매하는 것은 여러 가지 이유로 실패할 수 있습니다. 구매에 CLI(명령줄 인터페이스)를 사용하면 Azure Marketplace 사용할 수 없거나 표시되지 않는 제안을 구매하려고 할 수 있기 때문에 오류가 발생할 가능성이 높습니다. 다음은 구매 실패를 일으킬 수 있는 검사입니다.

1. 구독은 EA(기업계약)에 속하며 EA 관리자는 Azure Marketplace 구매를 사용하지 않도록 설정했습니다.
1. EA 관리자는 무료 제안에 대해서만 구매를 사용하도록 설정했으며, 이 제안은 유료 제안입니다.
1. 마켓플레이스에서 제안을 찾을 수 없습니다.
1. ISV(Independent Software Vendor)는 적어도 해당 지역에서 제안 판매를 중지했습니다.
1. 사용 중인 구독은 제안을 사용할 수 없는 지역의 청구 계정에 속합니다.
1. 구독/청구 계정은 유효한 결제 방법(예: 유효한 신용 카드)과 연결되지 않습니다.
1. 구독이 CSP(클라우드 솔루션 공급자)에 속하고 ISV가 CSP를 통한 판매를 거부했습니다.
1. 프라이빗 마켓플레이스는 구독에 대해 사용하도록 설정되며 허용된 제품 목록에는 없습니다.
1. 이 제안은 특정 고객에 대한 프라이빗/미리 보기이며 구독은 허용된 고객 목록에 없습니다.

## <a name="next-steps"></a>다음 단계

- [청구 및 송장 작성](billing-invoicing.md)