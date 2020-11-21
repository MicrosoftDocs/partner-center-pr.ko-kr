---
title: 전송 자격 – 청구 계정 간에 구독을 전송 하기 위한 지침 Azure Marketplace
description: Azure Portal에서 청구 계정 간에 구독을 전송 하기 전에 상업적 검사에 대 한 지침입니다.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007350"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>청구 계정 간 구독에 대 한 자격 전송

Azure Portal의 청구 섹션에서 한 청구 계정에서 다른 계정으로 [구독을 전송할](/azure/cost-management-billing/understand/subscription-transfer) 수 있습니다. 전송 전에는 타사 제품에 대 한 구독이 검색 됩니다. 전송은 *모든* 제품을 이전에 삭제 한 경우에만 허용 됩니다 (아래 [조건을](#criteria-for-transfer-approval-or-denial) 참조). 시스템은 다음 단계를 결정 하는 데 도움이 되도록 지우지 못한 앱에 대 한 관련 오류 메시지를 생성 합니다.

> [!NOTE]
> SaaS 리소스는 구독이 아닌 테 넌 트에 연결 되어 있으므로이 문서는 SaaS 제품에는 적용 되지 않습니다. SaaS 리소스는 한 청구 계정에서 다른 요금으로 전송할 수 있지만이는 리소스 및 Azure 지원에서 지원 요청으로 수행 됩니다.

## <a name="criteria-for-transfer-approval-or-denial"></a>전송 승인 또는 거부 조건

다음 조건 중 하나를 충족 하는 타사 앱이 있으면 구독을 전송할 수 없습니다.

- 대상 계정은 상업적 이며 앱은 파트너를 통해 판매 되도록 옵트아웃 (opt out) 됩니다.
- 앱이 선택한 파트너에 대해 옵트인 (opt in) 되 고 대상 계정이 허용 목록에 없습니다.
- 제품은 이전에 선택한 구독에 대 한 미리 보기 제품 이거나 비공개 제품 이며 구독은 더 이상 허용 목록에 없습니다.
- 새 청구 계정은 제품이 판매 되는 위치와 다른 지역에 있으며 제품을 해당 지역에서 판매 하지 않습니다.

차단 된 전송은 구독에서 리소스를 제거할 때까지 계속 적용 되며, 그 후에는 전송을 다시 시도할 수 있습니다.

## <a name="next-steps"></a>다음 단계

[Microsoft AppSource 및 Azure Marketplace에 대 한 지원 받기](get-support.md)

