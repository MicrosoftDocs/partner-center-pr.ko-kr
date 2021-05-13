---
title: Azure 플랜의 Azure 구독을 다른 CSP 파트너에게 이전
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure 플랜에 따라 고객의 Azure 구독과 연결된 클라우드 솔루션 공급자 프로그램 파트너를 변경하는 방법을 알아봅니다.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856052"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>고객의 Azure 플랜 구독을 다른 파트너에게 전송

**적절한 역할:** 계정 관리자 | 영업 에이전트 | 청구 에이전트

이 문서에서는 고객이 Azure 플랜에 따라 Azure 구독을 CSP(한 클라우드 솔루션 공급자)에서 다른 클라우드 솔루션 공급자 전환할 수 있는 방법을 설명합니다.

다른 파트너에서 고객의 Azure 구독을 전환하려면 다음 단계를 수행합니다. 파트너와 고객 모두 완료할 단계가 있습니다.

>[!Note]  
>Microsoft와 직접 청구 관계가 있는 파트너만 전환 도구에 액세스할 수 있습니다. 간접 대리점은 간접 공급자와 협력하여 이 전환 도구를 활용해야 합니다.

고객은 이 도구를 활용하기 전에 두 파트너(현재 및 미래)와 대화해야 합니다. 혼동과 변동을 피하려면 오프라인 대화가 필요합니다. 또한 파트너 및 고객은 전환을 시작하기 전에 이러한 고려 사항과 필수 구성을 이해해야 합니다.

**주요 고려 사항:**

- Azure Reservations는 구독과 함께 향후 파트너로 이동되지 않습니다.
- 현재 파트너의 Azure 서비스에 대한 CSP 가격 책정은 전환되지 않습니다.  
- 고객에 대한 지원 책임은 향후 파트너로 이전됩니다.
- 청구 및 청구서는 양도 시 향후 파트너에게 이전됩니다.
- Azure Role-Based ACCESS CONTROL(RBAC)는 전송의 영향을 받지 않습니다.
- AOBO(관리자 대신)는 향후 파트너에게 기본적으로 부여되지 않습니다.
- 타사 마켓플레이스 제품은 제품이 Marketplace 자격 확인을 통과하는 한 양도됩니다.
    - 특별 할인 또는 지역 제한은 없습니다.
    - 제품이 비구독 기반입니다.
    - 향후 파트너는 판매자와 협력하여 제품 배포 허용 목록에 있는지 확인해야 합니다.
    - Marketplace 제품을 양도하기 위해 이러한 조건이 모두 충족되지 않는 경우 Azure 구독이 이전된 다음 새 파트너와 Marketplace 제품을 다시 구입해야 합니다.

**사전 요구 사항:**

- 고객이 전환 의도에 현재 CSP 파트너 참여
- 향후 CSP 파트너는 고객과 협력하여 고객의 요구 사항을 충족할 수 있도록 합니다.
- 향후 CSP 파트너는 고객과 관계를 설정하고 전환이 시작되기 전에 Azure 플랜을 구매합니다.  
- 고객은 향후 CSP 파트너와 Microsoft 고객 계약 서명해야 합니다.
- 이 도구를 사용하려면 향후 CSP 파트너가 Microsoft 파트너 계약 서명해야 합니다.

## <a name="customer-tasks-to-be-completed"></a>완료할 고객 작업

Azure 플랜에 따라 Azure 구독을 양도하려면 고객이 현재 파트너에게 문의하여 프로세스를 시작해야 합니다. 향후 파트너가 대신 전송 요청 양식을 완료할 수 있도록 현재 파트너의 회사 이름 및 도메인을 수집해야 합니다.

또한 고객은 현재 파트너로부터 이전하려는 구독을 식별해야 합니다. Office 365, Enterprise Mobility Suite 또는 Microsoft Dynamics CRM 구독에 대한 파트너는 변경할 수 없습니다.

>[!Note]  
>전송 프로세스를 시작하는 전송 요청 양식을 완료하는 것은 향후 파트너의 책임입니다. Microsoft는 고객 또는 현재 파트너를 대신하여 개입할 수 없습니다. 고객은 미래 및 현재 파트너와 긴밀하게 협력하여 전환이 원활하게 진행되도록 계획해야 합니다.

## <a name="future-partner-tasks-to-be-completed"></a>완료할 향후 파트너 작업

구독의 미래 파트너는 구독 양도를 요청하려면 파트너 센터 전송 요청 양식을 작성해야 합니다.

1.  파트너 센터 메뉴에서 **고객을** 선택한 다음, 대신 전송 요청 양식을 작성하려는 고객을 선택합니다.
2.  고객 메뉴에서 **구독을 선택합니다.**
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

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="검토용":::

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
