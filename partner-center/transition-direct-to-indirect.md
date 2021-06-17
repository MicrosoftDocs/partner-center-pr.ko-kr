---
title: 직접 청구 파트너를 간접 대리점으로 전환
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 프로그램 파트너가 파트너 센터 사용하여 직접 청구 파트너에서 간접 대리점으로 전환하는 방법을 알아봅니다.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57c4a5d0a02079e887b38fa9754d276062d20cc
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276419"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a>CSP(클라우드 솔루션 공급자) 직접 청구 파트너에서 CSP 간접 재판매인으로 전환

**적절한 역할**: 전역 관리자

>[!Note]
>이 문서는 간접 대리점으로 전환하기로 결정한 직접 청구 파트너를 위한 것입니다. 그러나 아직 간접 대리점으로 등록하기로 명시적으로 결정하지 않은 경우에도 CSP 직접 청구 파트너 프로그램에 대한 새로운 [요구 사항을](direct-partner-new-requirements.md) 충족하지 않는 직접 청구 파트너는 직접 청구 [기능이 제한될](restricted-direct-bill-capabilities.md)때 Microsoft에서 알림을 받습니다.
<br>2021년 1월부터 새 수익 요구 사항이 추가됩니다. 직접 청구 파트너로 등록된 파트너는 지난 12개월 동안 파트너 글로벌 계정 수준에서 클라우드 솔루션 공급자 프로그램 수익에서 최소 USD$300K를 거래해야 합니다.

기존 직접 청구 테넌트를 사용하여 간접 대리점 프로그램에 등록할 수 있습니다.

## <a name="get-started"></a>시작하기

1. 파트너 센터 및 MPN ID의 파트너 프로필이 최신 상태인지 확인합니다.

2. 간접 대리점으로 전환하는 직접 청구 테넌트에서 전역 관리자로 파트너 센터 로그인합니다.

   :::image type="content" source="images/direct/direct1.png" alt-text="개요.":::

3. 등록 양식에서 파트너 세부 정보를 검토합니다.

   :::image type="content" source="images/direct/direct2a.png" alt-text="지금 등록합니다.":::

4. 지금 등록을 선택합니다. 간접 대리점 비즈니스는 직접 비즈니스에 사용하는 것과 동일한 AAD 테넌트 를 사용합니다.

    > [!NOTE]
    > 처음에 이 새로운 전환 기능은 9월에서 12월 12일로 파트너에게 제공됩니다. 9월에서 12월 사이에 1주년 날짜가 없는 경우 현재 기능이 표시되지 않습니다. 2018년 12월 이후의 1주년 날짜가 있는 파트너는 나중에 파트너에 대해 기능을 사용하도록 설정하면 알림을 받게 됩니다.

5. 등록이 승인되면 다시 파트너 센터 로그인합니다.

    > [!NOTE]
    > 승인은 일반적으로 즉시 처리되지만 영업일은 최대 5일이 걸릴 수 있습니다. 승인되면 등록 양식의 기본 연락처에서 지정한 이메일 주소에 대한 알림을 받게 됩니다. **설정**  >  **계정 설정** 파트너 프로필 > 프로그램 정보에서 등록 상태를 확인할 수도  >   있습니다.

6. **개요** 페이지에 간접 대리점 계약이 표시됩니다. 수락을 선택하고 **을 계속합니다.** 이 작업을 통해 간접 대리점 기능을 사용할 수 있습니다.

간접 대리점 계약에 동의하면 파트너 프로필이 직접 청구 및 간접 **대리점으로** 식별됩니다.

:::image type="content" source="images/direct/direct3.png" alt-text="간접 대리점 계약.":::

> [!IMPORTANT]
> 새 기능을 사용하여 간접 대리점으로 등록하면 직접 청구 전용 테넌트로 롤백할 수 있는 옵션이 없습니다. 간접 대리점으로 등록하기 전에 비즈니스 요구 사항을 완전히 평가해야 합니다.

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a>직접에서 간접 대리점으로 전환하는 동안

이 단계에서는 청구 프로세스를 포함하여 직접 고객의 구독 요구 사항을 계속 관리합니다. 간접 공급자의 고객을 수락하고 간접 대리점으로 운영할 수도 있습니다.

:::image type="content" source="images/direct/direct4.png" alt-text="직접 청구 및 간접 대리점입니다.":::

## <a name="find-an-indirect-provider"></a>간접 공급자 찾기

등록하면 간접 공급자에 대한 링크가 왼쪽 탐색에 표시됩니다. 간접 대리점은 간접 공급자와 관계를 설정합니다. 간접 공급자는 청구를 처리하고 고객을 위해 제품을 구매하며 인프라를 지원할 수 있습니다.

다양한 간접 공급자가 다양한 지원과 서비스를 제공하므로 간접 재판매인은 해당 지역의 공급자를 평가하여 요구 사항을 가장 잘 만족하는 공급자를 선정하면 됩니다. 일반적으로 대부분 공급자는 다음과 같은 일을 합니다.

- 간접 재판매인에게 기술 지원 제공
- 제품 및 서비스 마케팅 지원
- 입사 및 크레딧 조건 관리

공식 Microsoft 간접 공급자 목록을 [검색합니다.](https://partnercenter.microsoft.com/partner/find-a-provider)

자세한 내용은  [간접 공급자와 파트너 관계를 참조하세요.](indirect-reseller-tasks-in-partner-center.md)

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a>간접 공급자의 파트너 관계 초대 수락

파트너 관계를 맺을 간접 공급자를 찾으면 파트너 센터 간접 공급자와 파트너 관계를 설정합니다.

선택한 간접 공급자는 파트너 센터 초대로 연결되는 파트너 관계 초대 링크를 전자 메일로 보냅니다. 전역 관리자가 파트너 센터 로그인하고 초대 링크를 따라가야 합니다. 초대를 수락하면 공급자 이름이 간접 공급자 목록에 표시됩니다.

## <a name="acquire-new-customers-as-indirect-reseller"></a>간접 대리점으로 신규 고객 확보

사용자와 간접 공급자는 모두 고객과 대리점 관계를 맺어야 합니다. 이러한 대리점 관계를 통해 고객을 대신하여 고객의 구독 및 서비스를 관리할 수 있습니다. 기존 Azure AD 테넌트인 새 고객을 확보하려면 고객을 초대하여 사용자와 공급자 모두와 동시에 대리점 관계를 설정할 수 있습니다.

간접 대리점 초대를 만들려면 다음을 수행합니다.

1. 파트너 센터 왼쪽 탐색에서 **간접 공급자를** 선택합니다.

2. **새 고객 초대** 를 선택하여 귀사 및 간접 공급자와 동시에 재판매인 관계를 맺도록 고객을 초대합니다. 공급자는 고객과 대리점 관계를 맺어야 하므로 고객이 새 구독을 구입하거나 기존 구독에 새 라이선스를 추가하려는 경우 고객을 대신하여 주문을 제출할 수 있습니다.

3. 다음 페이지에서 임시 이메일 메시지를 검토합니다. 전자 메일로 초안 메시지를 열거나 클립보드에 메시지를 복사하여 메일에 붙여넣을 수 있습니다.

4. 이메일의 텍스트를 편집하여 필요한 내용을 말하지만 고객을 계정과 공급자 계정 모두에 직접 연결하도록 개인 설정될 때 링크를 포함해야 합니다. 그런 후 **완료** 를 선택합니다.

5. 고객이 귀사와 공급자를 공식 재판매인으로 승인하면 귀사에는 고객을 대신하여 고객의 구독, 라이선스 및 사용자를 관리할 관리자 권한이 부여되고 간접 공급자는 고객을 대신하여 주문을 제출할 수 있게 됩니다.
6. 고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장합니다.

직접 청구 파트너와 달리 간접 대리점은 파트너 센터 새 고객을 위한 Azure AD 테넌트 만들기를 할 수 없습니다. 공급자가 테넌트 를 만들고 이 고객의 간접 대리점으로 지정합니다. 이렇게 하면 고객이 파트너 센터 고객 목록에 표시됩니다.

>[!Note]
>직접 청구 기능을 사용하여 간접 대리점으로 획득한 고객을 위한 구매를 만들 수 없습니다.

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a>직접 청구 고객 및 간접 대리점 고객 관리

직접 청구 고객과 간접 대리점 고객을 다르게 관리합니다.

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a>직접 청구 고객(간접 대리점으로 수행하지 않는 것)

- 제품에 대한 주문 만들기
- Azure 예약 관리
- 주문 기록 관리
- 소프트웨어 구매
- 고객에게 직접 청구

### <a name="indirect-reseller-customers"></a>간접 대리점 고객

- 간접 공급자가 고객을 위해 제품을 주문합니다.
- 고객의 라이선스 및 사용자 관리
- 구독 갱신 처리

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a>직접 청구 파트너로 획득한 고객을 식별하려면

1. **고객** 을 선택합니다.

2. 세부 정보를 볼 고객을 선택합니다.

3. 이 고객이 직접 청구 파트너로 획득한 고객인 경우 제품을 **추가하거나** **보는** 옵션이 표시되고 해당 구독이 표시됩니다.

4. 고객이 귀하와 간접 대리점 관계를 맺은 경우 해당 옵션을 사용할 수 없습니다.

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a>직접 청구 고객을 간접 공급자로 이동

간접 공급자는 기존 직접 청구 고객에 대한 주문 또는 기존 구독 양도를 대리점과 관계를 맺을 때까지 제출할 수 없습니다. 간접 공급자와 기존 직접 청구 고객 간에 대리점 관계를 설정하려면 다음 방법 중 하나를 사용할 수 있습니다.

- [Reseller 관계 확장](#reseller-relationship-extension)

- [고객에게 간접 대리점 초대 보내기](#send-an-indirect-reseller-invitation-to-the-customer)

[직접-간접 전환 문서에서](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) 단계별 프로세스에 대한 자세한 개요를 찾을 수 있습니다.

### <a name="reseller-relationship-extension"></a>Reseller 관계 확장

파트너 센터 대시보드를 사용하여 기존 직접 청구 고객과 간접 공급자 간에 대리점 관계를 설정하려면 대리점 관계 확장 기능을 사용할 수 있습니다. 이 기능을 사용하기 전에 다음을 참고하세요.

- 이 기능은 간접 대리점으로 전환하는 직접 청구 파트너가 [간접 대리점 등록을](#get-started)완료한 경우에만 사용할 수 있습니다.

- 이 기능은 기존 직접 청구 고객에게만 적용할 수 있습니다. [간접 대리점 고객에게는](#acquire-new-customers-as-indirect-reseller)적용되지 않습니다.

- 간접 공급자 [의 파트너 초대를 수락한 간접 공급자만](#accept-a-partnership-invitation-from-your-indirect-provider)선택할 수 있습니다.

- 이 고객에 대해 보유하고 있는 청구 정보 복사본을 간접 공급자가 사용할 수 있습니다. 파트너 센터 대시보드에서 이 고객의 계정 페이지에 액세스하여 청구 정보에 액세스할 수 있습니다.

    > [!NOTE]
    > 대리점 관계 확장 기능을 사용하면 이 고객에 대해 보유한 청구 정보를 간접 공급자와 공유하는 데 동의하게 됩니다.

- 간접 공급자에게 고객 테넌트에게 [위임된 관리 권한이](customers-revoke-admin-privileges.md) 제공되지 않습니다. 간접 공급자에게 위임된 관리 권한이 필요한 경우 대신 고객에게 간접 대리점 초대를 보내야 합니다.

- 대리점 관계가 설정되면 간접 공급자는 Microsoft 365 관리 센터의 파트너 관계 페이지에서 고객에게 CSP 파트너로 표시되고 [을](https://admin.microsoft.com/AdminPortal/Home#/partners) [비즈니스용 Microsoft Store.](/microsoft-store/work-with-partner-microsoft-store-business)

    > [!IMPORTANT]
    > 혼동과 오해를 방지하기 위해 관계 확장 기능을 사용하여 기존 직접 청구 고객과 간접 공급자 간에 대리점 관계를 설정하기 전에 파트너 계약에 따라 직접 청구 고객에게 알리고 동의를 얻어야 합니다.

기존 고객 테넌트에서 이 기능을 사용하려면 다음을 수행합니다.

1. **관리 에이전트로** 파트너 센터 로그인합니다.

2. 고객 **페이지에서** 기존 고객을 선택하고 **빠른 링크** 아이콘을 클릭하여 고객의 요약 보기를 확장합니다.

3. **간접 공급자 아래에서 간접** **공급자 에서 고객 이전을** 클릭합니다.

    :::image type="content" source="images/direct/direct5-1.png" alt-text="간접 공급자에게 고객을 이전합니다.":::

4. 팝업 대화 상자에서 고객과 대리점 관계를 맺을 **간접 공급자를** 선택합니다.

5. **저장 후 계속** 을 클릭합니다.

6. 선택한 간접 공급자가 간접 공급자 아래에 **표시되는지 확인합니다.**

    :::image type="content" source="images/direct/direct5-2.png" alt-text="간접 공급자가 나열됩니다.":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a>고객에게 간접 대리점 초대 보내기

간접 공급자는 기존 직접 청구 고객과 대리점 관계를 맺을 때까지 주문을 제출할 수 없습니다. 기존 고객과 간접 공급자 간에 대리점 관계를 설정하려면 간접 대리점 초대를 사용하여 고객을 초대합니다.

1. 파트너 센터 왼쪽 탐색에서 **간접 공급자를** 선택합니다.

2. **새 고객 초대** 를 선택하여 귀사 및 간접 공급자와 동시에 재판매인 관계를 맺도록 고객을 초대합니다. 공급자는 고객과 대리점 관계를 맺어야 하므로 고객이 새 구독을 구입하거나 기존 구독에 새 라이선스를 추가하려는 경우 고객을 대신하여 주문을 제출할 수 있습니다.

    :::image type="content" source="images/direct/direct6.png" alt-text="새 고객을 초대합니다.":::

3. 다음 페이지에서 임시 이메일 메시지를 검토합니다. 전자 메일로 초안 메시지를 열거나 클립보드에 메시지를 복사하여 메일에 붙여넣을 수 있습니다.

4. 이메일의 텍스트를 편집하여 필요한 내용을 말하지만 고객을 계정과 공급자 계정 모두에 직접 연결하도록 개인 설정될 때 링크를 포함해야 합니다. 그런 후 **완료** 를 선택합니다.

5. 고객이 귀사와 공급자를 공식 재판매인으로 승인하면 귀사에는 고객을 대신하여 고객의 구독, 라이선스 및 사용자를 관리할 관리자 권한이 부여되고 간접 공급자는 고객을 대신하여 주문을 제출할 수 있게 됩니다.

6. 고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장합니다.

### <a name="microsoft-customer-agreement-acceptance"></a>Microsoft 고객 계약 동의

Microsoft 클라우드 계약 2020년 1월 31일까지 유효합니다. 해당 날짜 이후에는 기존 및 신규 고객인 모든 고객이 새 [Microsoft 고객 계약](confirm-customer-agreement.md)서명해야 합니다. 고객 전환의 경우 다음을 수행합니다.

- **고객이 아직 Microsoft 고객 계약 수락하지 않았습니다.**

   간접 공급자와 협력하여 고객이 [Microsoft 고객 계약 수락하도록](confirm-customer-agreement.md)하세요.

- **고객이 Microsoft 365 관리 센터를 통해 사용자와 Microsoft 고객 계약 수락했습니다.**

   간접 공급자와 대리점 관계가 설정되면 동의가 유지됩니다. 수행할 필요가 없습니다.

- **고객이 파트너 증명을 통해 사용자와 Microsoft 고객 계약 수락했습니다.**

   동의는 유지되지 않습니다. 간접 공급자와 협력하여 [파트너 센터 고객의 동의를 업데이트하세요.](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a>간접 공급자에게 기존 직접 청구 구독 전송

CSP 간접 모델에서 간접 대리점은 Microsoft와 청구 관계가 없습니다. 대신 간접 대리점은 간접 공급자를 통해 고객에 대한 구독을 얻습니다. 직접 청구 파트너에서 간접 대리점으로 전환하는 동안 직접 청구 파트너로 있는 기존 구독을 간접 공급자에게 양도해야 합니다. 파트너 센터 대시보드에서 셀프 서비스 구독 양도 기능을 사용하여 구독을 양도할 수 있습니다.

### <a name="prerequisites"></a>필수 구성 요소

- 이 기능은 기존 직접 청구 파트너 테넌트를 사용하여 간접 대리점 등록을 완료한 전환 파트너만 사용할 수 있습니다.

- 지정된 고객과 연결된 구독을 양도하기 전에 전환 파트너는 고객을 간접 공급자로 이동해야 합니다.

- 고객은 [간접 공급자 를 통해 Microsoft 고객 계약 수락해야](#microsoft-customer-agreement-acceptance)합니다.

### <a name="how-to-transition-to-indirect-reseller-status"></a>간접 대리점 상태로 전환하는 방법

이 기능은 다음과 같은 4단계 프로세스입니다.

- 전환 파트너가 구독 전송 요청을 만듭니다. 요청에는 동일한 고객과 연결된 하나 이상의 기존 구독이 포함되며 간접 공급자에게 주소가 지정됩니다.

- 간접 공급자는 전송 요청을 검토하고 수락(또는 거부)합니다.

- 간접 공급자는 전송 요청이 완료된 것을 확인합니다.

- 전환 파트너는 전송 요청이 완료된 것을 확인합니다.

### <a name="transitioning-partner"></a>전환 파트너

> [!NOTE]
> [파트너 센터 API/SDK를](/partner-center/develop/manage-customers) 사용하여 기존 구독을 간접 공급자에게 전송할 수도 있습니다.
>
> - [고객의 구독 이전 자격 가져오기](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [고객의 이전 만들기](/partner-center/develop/create-a-transfer)
> - [고객의 이전 철회](/partner-center/develop/withdraw-a-transfer)
> - [고객의 이전 수락](/partner-center/develop/accept-a-transfer)
> - [고객의 양도 거부](/partner-center/develop/reject-a-transfer)
> - [고객의 이전 가져오기](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [ID별 전송 세부 정보 얻기](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a>전환 파트너 - 전송 요청 만들기

전환 파트너로 전송 요청을 만들려면 다음을 수행합니다.

1. **관리 에이전트로** 파트너 센터 로그인합니다.

2. **고객** 페이지에서 원하는 고객을 선택하고 빠른 링크 아이콘을 클릭하여 고객의 요약 보기를 확장합니다.

3. **간접 공급자에서** 의도한 간접 공급자가 나열되어 있는지 확인합니다.

4. **구독 보기를 클릭합니다.**

5. 구독 페이지에서 **구독** **이전** 을 찾습니다.

6. **구독 전송에서** **구독 전송 요청을** 클릭합니다.

    :::image type="content" source="images/direct/direct8.png" alt-text="구독 전송을 요청합니다.":::

7. 전송 요청 대화 상자에서 전송할 구독을 하나 이상 선택합니다.

    :::image type="content" source="images/direct/direct9.png" alt-text="전송 요청을 만듭니다.":::

8. **만들기** 를 클릭합니다.

9. 활성 구독 전송 요청이 **구독 전송** 아래에 표시됩니다.

    :::image type="content" source="images/direct/direct10.png" alt-text="전송 요청 목록입니다.":::

10. 간접 공급자에게 구독 이전 요청을 만들었다고 알릴 수 있습니다.

### <a name="indirect-provider---accept-transfer-request"></a>간접 공급자 - 전송 요청 수락

간접 공급자로서 전송 요청을 검토하고 수락하려면 다음을 수행합니다.

1. **관리** 에이전트 또는 **판매 에이전트로** 파트너 센터 로그인합니다.

2. **고객** 페이지에서 원하는 고객을 선택하고 빠른 링크 아이콘을 클릭하여 고객의 요약 보기를 확장합니다.

3. **간접 대리점에서** 전환 파트너가 나열되어 있는지 확인합니다.

4. **구독 보기를 클릭합니다.**

5. 구독 페이지에서 **구독** **이전** 을 찾습니다.

    :::image type="content" source="images/direct/direct11.png" alt-text="전송 요청을 봅니다.":::

6. **구독 전송** 에서 검토할 전송 요청을 클릭합니다.

7. **적절하게 수락(또는** **거부)을** 클릭합니다.

    :::image type="content" source="images/direct/direct12.png" alt-text="전송 요청을 수락합니다.":::

8. 전송 요청이 완료되기를 기다립니다.

### <a name="indirect-provider---verify-transfer-request-is-complete"></a>간접 공급자 - 전송 요청이 완료되었는지 확인

1. 전송 요청이 성공적으로 완료되면 구독 아래에 구독이 표시되는지 **확인합니다.**

2. 전환 파트너에게 알릴 수 있습니다.

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a>전환 파트너 - 전송 요청이 완료되었는지 확인

전환 파트너는 다음을 수행해야 합니다.

1. 관리 에이전트 또는 **판매 에이전트로** 파트너 센터 로그인합니다. 

2. **고객** 페이지에서 원하는 고객을 선택하고 **빠른 링크** 아이콘을 클릭하여 고객의 요약 보기를 확장합니다.

3. **구독 보기를 클릭합니다.**

4. 구독 페이지에서 **구독** **이전** 을 찾습니다.

5. 전송 요청이 완료 로 표시되는지 **확인합니다.**

6. 구독 페이지에서 구독이 더 이상 활성으로 표시되지 않는지 **확인합니다.**

   1. Azure 구독(MS-AZR-0145P)인 경우 더 이상 나열되지 않습니다.

   2. 라이선스 기반 구독(Office 365, Dynamics, Intune)이면 상태가 **일시 중단으로 나열됩니다.**

   :::image type="content" source="images/direct/direct13.png" alt-text="구독이 일시 중단되었습니다.":::

### <a name="considerations"></a>고려 사항

- **구독 ID는 양도 후 다릅니다.** Azure 구독(MS-AZR-0145P)인 경우 이전 소유자로부터 유지되는 Azure 구독 ID가 있으며 Azure 관리 포털에 표시됩니다.

- **여러 전송 요청에서 동일한 구독을 참조할 수 없습니다.** 기존 구독을 포함하는 전송 요청을 만든 후에는 첫 번째 전송 요청이 취소될 때까지 동일한 구독을 포함한 추가 전송 요청을 만들 수 없습니다.

- **라이선스 기반 구독에 대한 추가 기능도 기본 구독과 함께 양도해야 합니다.** 전송 요청을 만들 때 하나 이상의 추가 기능으로 기존 구독을 선택하면 추가 항목이 전송 요청에 자동으로 포함됩니다.

- **구독에 대한 라이선스 수 변경 내용은 기존 전송 요청에 반영되지 않습니다.** 기존 구독을 포함하는 전송 요청을 만든 후에는 구독(또는 연결된 추가 기능)의 라이선스 수량을 업데이트하지 않아야 합니다. 이렇게 하면 새 수량이 전송 요청에 반영되지 않습니다. 간접 공급자가 전송 요청을 수락하면 결과 구독에는 이전 수량이 있습니다. 새 수량을 간접 공급자에게 전송하려면 기존 전송 요청을 취소하고 새 수량을 다시 만들어야 합니다.

- **셀프 서비스 구독 양도를 사용하여 모든 구매를 양도할 수 있는 것은 아닙니다.** 현재 이 기능을 사용하여 O365 구독 및 Azure PAYG 구독(MS-AZR-0145P)만 양도할 수 있습니다. Azure Plans, Azure Reserved Instances, 기간 기반 구독 및 Azure Marketplace 대한 SaaS 구독을 포함한 다른 구매는 지원되지 않습니다. 전송 요청 제출 페이지에서 구독을 양도할 수 없는 이유가 표시됩니다. 이러한 구독을 양도하려면 간접 공급자를 통해 [기존 구독을 취소하고](create-a-new-subscription.md#suspend-or-cancel-a-subscription) 고객을 위한 새 제안을 구매해야 합니다.

- **샌드박스 환경을 사용하여 테스트할 수 없습니다.**

## <a name="enroll-for-indirect-reseller-incentives"></a>간접 대리점 인센티브 등록

기존 직접 청구 파트너 테넌트에서 간접 대리점으로 성공적으로 등록한 후에는 30일 이내에 간접 대리점 인센티브에 등록하라는 초대를 받게 됩니다. 초대는 현재 CSP 파트너 테넌트와 연결된 파트너 MPN 계정을 기반으로 합니다. 파트너 MPN 계정과 연결된 이메일 주소로 초대가 전송됩니다.

또한 동일한 파트너 테넌트에서 직접 청구 인센티브 프로그램에 등록할 수 있습니다. 프로그램을 별도로 관리해야 합니다.

## <a name="next-steps"></a>다음 단계

- [간접 재판매인이 되기 위한 추가 정보](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [CSP 직접 파트너 새로운 요구 사항](direct-partner-new-requirements.md)
- [제한된 직접 청구 기능](restricted-direct-bill-capabilities.md)
