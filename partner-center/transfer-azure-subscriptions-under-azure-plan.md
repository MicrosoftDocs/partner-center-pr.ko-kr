---
title: Azure 계획의 Azure 구독을 다른 CSP 파트너에 게 전송
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure 요금제에서 고객의 Azure 구독과 연결 된 클라우드 솔루션 공급자 프로그램 파트너를 변경 하는 방법에 대해 알아봅니다.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284505"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>고객의 Azure 계획 구독을 다른 파트너에 게 전송

**적절한 역할**

- 계정 관리자
- 영업 상담원
- 청구 에이전트

이 문서에서는 고객이 Azure 계획을 통해 azure 구독을 한 클라우드 솔루션 공급자 (CSP)에서 다른 클라우드 솔루션 공급자로 전환할 수 있는 방법을 설명 합니다.

다른 파트너에서 고객의 Azure 구독을 전환 하려면 다음 단계를 수행 합니다. 파트너와 고객 모두 완료 하는 단계가 있습니다.

>[!Note]  
>Microsoft와 직접 청구 관계가 있는 파트너만 전환 도구에 액세스할 수 있습니다. 간접 재판매인은 간접 공급자와 협력 하 여이 전환 도구를 활용 해야 합니다.

이 도구를 사용 하기 전에 고객은 파트너 (현재 및 미래)를 모두 사용 하 여 대화에 속해야 합니다. 혼동 및 변동 방지를 방지 하려면 오프 라인 대화를 해야 합니다. 또한 파트너와 고객은 전환을 시작 하기 전에 이러한 고려 사항 및 필수 구성 요소를 이해 해야 합니다.

**주요 고려 사항:**

- Azure Reservations는 이후 파트너에 대 한 구독과 함께 이동 하지 않습니다.
- 현재 파트너의 Azure 서비스에 대 한 CSP 가격은 전환 되지 않습니다.  
- 고객에 대 한 지원 책임이 이후 파트너로 이동 합니다.
- 전송 시 청구 및 청구는 이후 파트너로 이동 합니다.
- Azure Role-Based Access Control (RBAC)는 전송의 영향을 받지 않습니다.
- (AOBO)를 대신 하 여 관리자는 이후 파트너에 게 기본적으로 부여 되지 않습니다.
- 타사 marketplace 제품은 제품이 Marketplace 자격 검사를 통과 하는 동안 전송 됩니다.
    - 특별 한 할인이 나 지역 제한은 없습니다.
    - 제품이 비등록 기반입니다.
    - 이후 파트너는 게시자와 협력 하 여 제품 배포에 대 한 allowlist에 있는지 확인 해야 합니다.
    - Marketplace 제품을 전송 하기 위해 이러한 조건을 모두 충족 하지 않는 경우 Azure 구독을 전송 하 고 새 파트너와 마켓플레이스 제품을 다시 구매 해야 합니다.

**사전 요구 사항:**

- 고객은 자신의 의도에 따라 현재 CSP 파트너를 전환 합니다.
- 향후 CSP 파트너는 고객과 협력 하 여 고객의 요구 사항을 충족할 수 있는지 확인 합니다.
- 이후 CSP 파트너는 고객과의 관계를 설정 하 고 전환을 시작 하기 전에 Azure 계획을 구입 합니다.  
- 고객이 향후 CSP 파트너와 Microsoft 고객 계약에 서명 해야 합니다.
- 이 도구를 사용 하려면 향후 CSP 파트너가 Microsoft 파트너 계약에 서명 해야 합니다.

## <a name="customer-tasks-to-be-completed"></a>완료할 고객 작업

Azure 계획에 따라 Azure 구독을 전송 하려면 고객이 현재 파트너에 게 연락 하 여 프로세스를 시작 해야 합니다. 현재 파트너의 회사 이름 및 도메인을 수집 하 여 이후 파트너가 전송 요청 양식을 대신 완료할 수 있도록 해야 합니다.

또한 고객은 현재 파트너 로부터 전송 하려는 구독을 식별 해야 합니다. Office 365, Enterprise Mobility Suite 또는 Microsoft Dynamics CRM 구독의 파트너를 변경할 수 없습니다.

>[!Note]  
>전송 프로세스를 시작 하는 전송 요청 양식을 완료 하는 것은 향후 파트너의 책임입니다. Microsoft는 고객 또는 현재 파트너를 대신 하 여 개입 하지 않습니다. 고객은 이후 및 현재 파트너와 긴밀 하 게 협력 하 여 전환을 원활 하 게 진행할 수 있도록 계획 해야 합니다.

## <a name="future-partner-tasks-to-be-completed"></a>완료할 이후 파트너 작업

이후 구독 파트너는 파트너 센터에서 전송 요청 양식을 완료 하 여 구독 전송을 요청 해야 합니다.

1.  파트너 센터 메뉴에서 **고객** 을 선택한 다음 대신 전송 요청 양식을 완료 하려는 고객을 선택 합니다.
2.  고객 메뉴에서 **구독** 을 선택 합니다.
3.  **전송 요청** 섹션을 선택 합니다.
4.  **전송 요청 섹션** 에서 **새 요청 추가** 를 선택 합니다.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="전송 섹션":::

5.  **새 전송 요청** 양식을 작성 합니다.

6.  **전송 전송 요청**  >  **보내기** 를 선택 합니다.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="전송 요청 양식 완료":::

7.  전송 요청 확인 검토

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="보류 중인 전송 검토":::

    >[!Note]
    >이후 파트너는 전송 요청 상태가 "보류 중" 인 경우에만 오른쪽 위 모서리에서 **요청 취소** 를 선택 하 여 전송 요청을 취소할 수 있습니다. 전송 요청 상태가 "진행 중" 또는 "완료" 이면 취소가 가능 하지 않습니다.

## <a name="current-partner-tasks-to-be-completed"></a>완료할 현재 파트너 작업

현재 파트너의 고객 관리 에이전트는 고객의 구독 전송을 요청 하는 전자 메일을 받게 됩니다.

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="검토":::

파트너 센터에서 전송 요청 양식을 검토 하 고 수락 하 여 구독 이전을 완료 합니다.

>[!Note]  
>현재 파트너가 30 일 내에 작업을 수행 하지 않으면 요청이 만료 되 고 이후 파트너는 새 전송 요청을 만들기 위한를 갖게 됩니다.

1.  전자 메일에서 **전송 요청 검토** 를 선택 하거나
1.  파트너 센터 메뉴에서 **고객** 을 선택한 다음를 대신 하 여 전송 요청을 제출 하는 고객을 선택 합니다.
2.  고객 메뉴에서 **구독** 을 선택 합니다.
3.  **전송 요청** 섹션을 선택 합니다.
4.  **받은 요청** 에서 선택한 **전송 요청 ID** 를 선택 하 여 전송 정보를 확장 합니다.

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="원본 검토 전송 요청":::

5.  전송 요청을 검토 합니다. 전송할 요청 된 Azure 구독을 선택 합니다.

>[!Note]  
> 계속 하기 전에 선택한 구독에 대 한 액세스 권한이 더 이상 없습니다.
> 추가 사용을 위해 송장이 청구 되지 않습니다.
> Azure 예약은 구독과 함께 전송 되지 않습니다.

6.  그런 다음 **수락 및 전송** 을 선택 하 여 전송 프로세스를 완료 합니다.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure 요금제로 전송할 구독 선택":::

7.  전송 승인 확인을 표시 합니다.

   이 시점에서 이후 파트너, 고객 및 현재 파트너는 전자 메일을 통해 수락 된 전송 요청에 대 한 알림이 표시 됩니다.

   이후 전환이 수락 되 면 시스템이 업데이트 되는 동안 최대 15 분 동안 보류 중 상태가 유지 될 수 있습니다. 시간이 더 오래 걸리면 시스템은 3 일 동안 계속 시도 하 게 됩니다. 전송 상태가 여전히 보류 중으로 유지 되 면 파트너는 서비스 요청을 제출 해야 합니다.

   전송이 완료 되 면 요청에 포함 된 구독이 향후 파트너의 Azure 계획에 표시 되며 더 이상 표시 되지 않습니다.

>[!Note]  
>간접 공급자의 경우: 전송 요청이 수락 되었음을 간접 재판매인에 게 알려 주세요.

### <a name="managing-your-transferred-customer-subscriptions"></a>전송 된 고객 구독 관리
- Azure RBAC(역할 기반 액세스 제어)를 사용하여 할당된 기존 사용자, 그룹 또는 서비스 주체에 대한 액세스는 전환 중에 영향을 받지 않습니다. Azure [RBAC (](/azure/role-based-access-control/overview) 역할 기반 액세스 제어)를 통해 고객은 azure 리소스에 액세스할 수 있는 사용자, 해당 리소스에서 수행할 수 있는 작업 및 액세스할 수 있는 영역을 관리할 수 있습니다. 새 파트너에 게는 구독 이전에 고객의 리소스에 대 한 RBAC 액세스 권한이 제공 되지 않습니다. 고객의 이전 파트너는 RBAC 액세스를 유지 합니다. 고객에 게 문의 하 여 구독에 대 한 통찰력을 보유 하 고 있는 사람을 파악 하 고 원하는 변경 작업을 수행 하세요.

- 따라서 고객이 이전 파트너에 대 한 Azure RBAC 액세스를 제거 하 고 새 파트너에 대 한 액세스를 추가 하는 것이 중요 합니다. 고객이 새 액세스 권한을 부여 하는 방법에 대 한 자세한 내용은 [azure 역할 기반 액세스 제어 란? (AZURE RBAC)](/azure/role-based-access-control/overview) 을 참조 하세요. 사용자가 이전 파트너의 RBAC 액세스를 제거 하는 방법에 대 한 자세한 내용은 [역할 할당 제거](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)를 참조 하세요.

- 또한 구독에 대 한 액세스 권한 [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 을 자동으로 가져오지 않습니다. AOBO는 파트너의 고객을 대신 하 여 고객의 Azure 구독을 관리 하는 데 필요 합니다. Azure 권한에 대 한 자세한 내용은 [고객의 서비스 또는 구독을 관리할 수 있는 권한 얻기](./customers-revoke-admin-privileges.md) 를 참조 하세요.

## <a name="next-steps"></a>다음 단계:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [고객의 서비스 또는 구독을 관리할 수 있는 권한을 획득 합니다.](./customers-revoke-admin-privileges.md)
