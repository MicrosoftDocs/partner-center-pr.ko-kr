---
title: Microsoft 고객 계약에 대한 고객의 동의 확인
description: Microsoft 고객 계약에 대한 고객의 동의 여부를 확인하는 방법을 알아봅니다. 이는 고객을 위해 Microsoft 제품 및 서비스를 주문하는 데 필요할 수 있습니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354613"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Microsoft 고객 계약에 대한 고객의 동의 여부를 확인하는 방법이 업데이트됨


**적절한 역할**

- 관리 에이전트
- 영업 상담원

> [!NOTE]
> 계약 리소스는 현재 Microsoft 퍼블릭 클라우드의 파트너 센터에서만 지원됩니다. 다음 센터에는 적용되지 않습니다.
> * 21Vianet에서 운영하는 파트너 센터
> * Microsoft 클라우드 독일 파트너 센터
> * Microsoft Cloud for US Government 파트너 센터

>[!NOTE]
>2020년 1월 31일부로 모든 기존 고객과 신규 고객은 새로운 Microsoft 고객 계약에 서명해야 합니다. 자세한 내용은 [Microsoft 고객 계약에 대한 고객 동의 확인](confirm-customer-agreement.md)을 참조하세요.

파트너는 고객 대신 Microsoft 제품 및 서비스를 주문하려면 Microsoft 고객 계약에 대한 고객 동의를 받아야 합니다. 파트너가 규정을 잘 준수할 수 있도록, Microsoft는 계약에 동의한 사람과 관련해 다음과 같은 세부 정보를 제공함으로써 파트너에게 동의 여부를 확인하도록 요구하고 있습니다.

- 이름

- 성

- 메일 주소

- 전화 번호(선택 사항)

- 동의 날짜

직접 청구 파트너 및 간접 공급자는 파트너 센터 또는 파트너 센터 API를 통해 거래할 때 고객의 Microsoft 고객 계약 동의 여부를 확인해야 합니다. 확인은 *필수 사항* 입니다.

고객이 계약에 동의한 것으로 확인되지 않으면 다음과 같은 결과가 초래됩니다.

- 해당 고객의 신규 주문을 작성할 수 없습니다.

- 해당 고객의 기존 라이선스 기반 구독의 라이선스 수를 변경할 수 없습니다.

파트너 센터 또는 파트너 센터 API를 통해 고객 동의 여부를 확인할 수 있습니다. 파트너 센터 API를 통해 확인하려면 다음 토픽을 참조하세요.

- [고객 동의 확인 정보 가져오기](/partner-center/develop/get-confirmation-of-customer-consent)

- [계약 메타데이터 가져오기](/partner-center/develop/get-agreement-metadata)

- [고객 동의 확인](/partner-center/develop/confirm-customer-consent)

프로덕션 환경과 샌드박스 환경에 모두 적용됩니다.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>신규 고객의 고객 동의 확인

파트너 센터에서 신규 고객 테넌트를 생성하는 동안 다음 절차에 따라 고객의 동의 여부를 확인합니다. 관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.

1. **고객**, **새 고객**, **계정 정보** 를 차례로 선택합니다.

2. **회사** 및 **기본 연락처** 정보를 입력합니다.

   :::image type="content" source="images/mca/mca1.png" alt-text="회사 정보":::

3. **Microsoft 고객 계약** 에서 **고객이 최신 Microsoft 고객 계약에 동의했음** 을 선택합니다.

4. **계약 동의 날짜** 에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

5. 동의를 표한 사용자의 세부 정보를 입력합니다.

   :::image type="content" source="images/mca/MCA3.png" alt-text="동의 날짜 추가":::

   기본적으로 사용자의 기본 연락처 정보가 표시됩니다. 이 정보가 틀린 경우에는 **업데이트** 를 선택하고, 계약에 동의한 사람의 **이름**, **성**, **이메일 주소** 및 **전화 번호*(선택 사항)를 입력합니다.

6. 고객 테넌트를 생성하기 위한 나머지 단계를 계속하려면 **다음** 을 선택합니다.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>기존 고객의 동의 여부 확인

관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.

1. **고객** 을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.

2. **계정 정보** 를 선택합니다.

3. **Microsoft 고객 계약** 에서 **업데이트** 를 선택합니다.

   :::image type="content" source="images/mca/mca4.png" alt-text="Update":::

4. 계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.

5. **계약 동의 날짜** 에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

6. **저장하고 계속** 을 선택합니다.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>기존 고객의 신규 주문을 작성할 때 고객의 동의 여부 확인

앞서 동의 여부를 확인하지 않은 기존 고객의 신규 주문을 작성하려고 시도하면 확인을 완료하라는 메시지를 받게 됩니다. 다음 절차를 사용 하 여이 작업을 수행 합니다.

1. 계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.

2. **계약 동의 날짜** 에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

3. **저장하고 계속** 을 선택합니다.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>기존 고객의 동의 여부 검색

아래 절차에 따라 이전에 제공한 기존 고객의 동의 여부를 검색할 수 있습니다. 관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.

1. **고객** 을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.

2. **계정 정보** 를 선택합니다.

3. **Microsoft 고객 계약** 에서 이 고객의 확인 여부를 볼 수 있습니다.

## <a name="next-steps"></a>다음 단계

- [CSP 파트너 프로그램에서 고객의 Microsoft 고객 계약 동의 확인](confirm-customer-agreement.md)

- [고객을 대신하여 Microsoft 고객 계약 동의 증명](attest-acceptance-customer-agreement.md)