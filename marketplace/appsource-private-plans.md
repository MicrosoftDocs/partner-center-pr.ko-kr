---
title: Microsoft AppSource의 비공개 요금제
description: Microsoft AppSource (Azure Marketplace)에서 전용 요금제를 설정 합니다.
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008551"
---
# <a name="private-plans-in-microsoft-appsource"></a>Microsoft AppSource의 비공개 요금제

개인 계획은 게시자가 특정 고객에 게 사용자 지정 계획을 제공 하는 방법입니다. 이 옵션은 현재 Microsoft AppSource에서 사용할 수 있습니다. 비공개 요금제는 **이제 Get** 을 사용 하 여 작업을 호출할 수 있는 SaaS (software as a service) 제품에 대 한 appsource에서 판매 될 수 있습니다.

## <a name="ask-your-isv-for-a-private-plan"></a>ISV에 게 개인 요금제 요청

비공개 요금제를 AppSource에서 사용할 수 있도록 하려면 ISV에 직접 문의 하 고 사용자 지정 가격 및 기술 사양을 협상 해야 합니다. 비공개 요금제의 조건에 동의한 후에는 ISV가 계획을 만들어 조직의 테 넌 트 ID (제공 해야 함)에 할당 합니다.

### <a name="finding-your-tenant-id"></a>테 넌 트 ID 찾기

1. AppSource의 오른쪽 위 모서리에서 계정 프로필 아이콘을 선택 하 고 **테 넌 트를 봅니다**.
2. 테 넌 트 ID를 복사 하 여 ISV에 제공 합니다.

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="테 넌 트 ID를 찾는 방법을 보여 줍니다.":::

## <a name="find-a-private-plan-in-appsource"></a>AppSource에서 비공개 요금제 찾기

ISV가 AppSource에 표시 되기 전에 새 개인 계획을 게시 한 후 최대 48 시간까지 걸릴 수 있습니다. 테 넌 트 ID와 연결 된 개인 계획을 찾으려면 AppSource의 오른쪽 위에서 **비공개 계획** (잠금 아이콘)을 선택 합니다.

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="위쪽 도구 모음에서 자물쇠 아이콘 (자물쇠)을 표시 합니다.":::

로그인 하지 않은 경우 메시지가 표시 됩니다. 그런 다음 **요금제 + 가격 책정** 탭에서 테 넌 트 ID와 연결 된 비공개 요금제를 구입할 수 있습니다.

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="요금제 및 가격 책정 탭에서 비공개 제품을 표시 합니다.":::

테 넌 트에 대해 비공개 요금제를 사용할 수 없는 경우 개인 계획 또는 제안이 없다는 메시지가 표시 됩니다.

## <a name="purchase-a-private-plan"></a>비공개 요금제 구매

ISV는 제품 내에서 하나 이상의 비공개 계획을 포함할 수 있습니다. 각 제품에는 공용 및 비공개 요금제가 모두 포함 될 수 있지만 비공개 요금제는 페이지의 오른쪽 위에 있는 개인 제안 아이콘 (자물쇠)에서 액세스 하는 별도의 제안 목록 페이지 아래에 나타납니다.

**요금제 + 가격 책정** 탭에 사용 가능한 비공개 요금제가 표시 됩니다. 비공개 요금제에는 독특한 파란색 배지가 있습니다.

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="개인 제안 옆에 파란색 개인 제품 배지를 표시 합니다.":::

선택한 계획을 구매 하려면 **지금 가져오기** 를 선택 하 고 제공 된 단계를 따릅니다.

## <a name="next-steps"></a>다음 단계

- [Microsoft AppSource란?](appsource-overview.md)
