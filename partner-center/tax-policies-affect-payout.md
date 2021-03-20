---
title: 세금 정책이 Azure Marketplace 지급에 미치는 영향
description: 세금 정책이 Azure Marketplace 지급에 미치는 영향에 대해 알아봅니다.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712956"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>세금 정책이 Azure Marketplace 지급에 미치는 영향

**적절한 역할**
-    글로벌 관리자
-    사용자 관리자
-    관리 에이전트

## <a name="introduction"></a>소개

Microsoft 상업적 marketplace는 전 세계에 도달 했습니다. 트랜잭션은 테두리를 통해 발생 하며 ISV와 고객의 위치에 따라 세금 영향이 달라질 수 있습니다. 파트너 센터 세금 프로필 정보를 사용 하 Microsoft AppSource 및 Azure Marketplace 하 여 ISV의 국가를 확인 합니다. 고객의 국가를 확인 하려면 고객의 청구 정보를 사용 하거나 고객이 EU에 있는 경우 두 가지 정보를 사용 합니다.

다음 시나리오를 더 잘 이해 하려면 Microsoft에서 게시자를 대신 하 여 세금을 수집 하 고 지불 하는지 또는 해당 책임이 게시자에 속한 경우를 표시 하는 [세금 정보](tax-details-marketplace.md) 테이블을 참조 하세요.

> [!NOTE]
> 이 항목의 모든 예제 판매 값과 세금 백분율은 정확한 수치가 아니라 설명 목적 으로만 사용 됩니다.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Microsoft에서 관리 하는 세금 국가의 게시자 엔터티입니다

**시나리오 A** – Microsoft에서 관리 하는 [세금 국가의](tax-details-marketplace.md#microsoft-managed-countries)게시자와 고객 간에 발생 하는 트랜잭션입니다. 이러한 트랜잭션은 판매 당시에 적용 되는 세금을 보유 하 고 있으며 Microsoft는 해당 국가의 세금을 보냅니다. 지급에서 보안상 이유로 하는 세금은 없고 지급 계산은 세금을 제외 합니다.

미국 이외 게시자와 미국 고객 간의 트랜잭션은 [시나리오 D](#foreign-publisher-transacts-with-us-customer) 를 참조 하세요.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="지급 process 시나리오 A에 대 한 워크플로를 표시 합니다.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Marketplace 요금은 Taxable 서비스인 Microsoft에서 관리 하는 세율의 게시자 엔터티입니다

**시나리오 B** -미국 기반 게시자 (파트너 센터 세금 프로필 정보로 정의 됨) 간에 발생 하는 트랜잭션은 시장 요금 (taxable 서비스)에 세금을 부과 하는 Microsoft 관리형 세금 국가에서 고객에 게 적용 됩니다. 이 시나리오에서 매장 서비스 요금에 대 한 세금은 게시자의 지급에서 뺍니다.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="지급 process 시나리오 B에 대 한 워크플로를 표시 합니다.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>게시자 엔터티입니다의 게시자 관리 세금 국가

**시나리오 C** – 고객에 게 원천 세금을 적용 하지 않는 게시자 관리 세금 국가의 게시자와 고객 간에 발생 하는 트랜잭션입니다. 고객은 판매 시점에서 세금을 지불 하지 않으며 해당 세금을 지불 하기 위한 게시자의 의무입니다.

국가별 가격 책정 (예: 예정 된 세금 오프셋)에 대 한 자세한 내용은 [상용 marketplace 제품에 대 한 계획 및 가격 책정](/azure/marketplace/plans-pricing#custom-prices)을 참조 하세요.

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="지급 process 시나리오 C에 대 한 워크플로를 표시 합니다.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>미국 고객과의 외부 게시자 엔터티입니다

**시나리오 D** – 미국 조약이 없는 국가에서 모든 외부 게시자 (파트너 센터 세금 프로필 정보로 정의 [됨)는](#foreign-publisher-with-a-treaty-transacts-with-us-customer)미국 조약 (고객 계정 주소로 정의 됨)에 따라 미국 기반 고객에 대 한 판매를 수행 합니다. 미국 정부에서는 게시자를 대신 하 여 Microsoft 보유 세금을 요구 합니다. 지급에서 publisher로 세금 보안상 이유로은 제공 가격을 기준으로 계산 됩니다.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="지급 process 시나리오 D에 대 한 워크플로를 표시 합니다.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>미국 고객과 협약 엔터티입니다 있는 외부 게시자

**시나리오 E** – 미국 협약에 의해 정의 된 모든 외부 게시자 (고객 계정 주소에 정의 된 대로 미국 협약 프로필 정보로 정의 됨) 미국 정부에서는 게시자를 대신 하 여 Microsoft에서 세금을 보유 필요가 없습니다.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="지급 process 시나리오 E에 대 한 워크플로를 표시 합니다.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>외부 게시자는 Microsoft에서 관리 하는 국가 (아일랜드 외부)에서 EU VAT로 등록 된 고객에 게 판매 됩니다.

**시나리오 F** -Microsoft-Managed 국가에서 외부 게시자와 EU (아일랜드 외부)에 등록 된 고객 간의 모든 트랜잭션입니다. 고객은 판매에 대 한 세금을 지불 하지 않습니다.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="지급 process 시나리오 F에 대 한 워크플로를 보여 줍니다.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>외부 게시자는 Microsoft에서 관리 하는 국가 (아일랜드)에서 EU VAT로 등록 된 고객에 게 판매 됩니다.

**시나리오 G** -Microsoft-Managed 국가에서 외부 게시자와 EU (아일랜드 내)에 등록 된 고객 간의 모든 트랜잭션입니다. 고객은 아일랜드 VAT를 지불 하 고 Microsoft는이 세금을 아일랜드 정부에 게 지불 합니다.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="지급 process 시나리오 G에 대 한 워크플로를 표시 합니다.":::

## <a name="next-steps"></a>다음 단계

- [게시자 FAQ](/azure/marketplace/marketplace-faq-publisher-guide)
- [결제 및 세금 프로필을 만들기 위한 지침](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)