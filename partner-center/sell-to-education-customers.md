---
title: 교육 고객에게 제안을 판매하는 방법
description: 교육 고객을 만들고 파트너 센터 고객에게 제안을 판매하는 방법을 알아봅니다. 교육 고객의 확인 상태를 확인하는 것을 포함합니다.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d0cff4883e084ccc0acb37d8c3119d91e3f5530
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276453"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>교육 고객에게 제안을 판매하는 방법 및 파트너 센터 교육 고객을 만드는 방법

**적절한 역할:** 전역 관리자 | 관리 에이전트 | 판매 에이전트

## <a name="create-an-education-customer"></a>교육 고객 만들기

이 문서에서는 파트너 센터 교육 고객을 만들고 교육 제품을 판매하는 방법을 설명합니다. 또한 확인 상태를 보고 필요한 경우 확인 요청을 다시 제출하는 방법을 다룹니다. 교육 제안은 현재 Microsoft 365, Dynamics, Intune 등과 같은 **라이선스 기반 서비스에만 사용할 수 있습니다.** 다른 유형(소프트웨어 구독, 영구 소프트웨어 또는 Azure 제품)에는 사용할 수 없습니다.

> [!IMPORTANT]
> Microsoft는 새로 만든 각 교육 고객 테넌트에서 교육 제공을 받을 자격이 있는지 확인합니다.  확인 프로세스의 지연을 방지하기 위해 필요한 정보를 최대한 정확하고 완전히 입력해야 합니다.

1. 파트너 센터에 로그인합니다.

2. **고객을** 선택한 다음, **고객 추가를** 선택합니다. 특별 자격 드롭다운에서 **교육** **을** 선택합니다.  필요에 따라 나머지 계정 정보를 입력합니다.  확인 프로세스를 지원하는 주요 필드는 다음과 같습니다.

   - **회사 이름:** 법적 엔터티 이름 입력 - 확인에 필요
   - **국가/지역 및 주소 줄:** 전체 엔터티 메일 주소 입력 – 확인에 필요합니다.
   - **이메일 주소:** 확인에 필요한 엔터티 소유 메일(무료 또는 on.microsoft.com 메일이 아닌)을 입력합니다.
   - **고객 연락처 정보:** 이러한 세부 정보는 확인 프로세스의 일부로 사용됩니다.
   - **기본 도메인 이름:** 고객의 계정 및 이메일 주소를 만드는 데 사용됩니다.  공백이나 특수 문자가 없는 회사 이름과 비슷한 이름을 선택합니다.  이 이름은 나중에 변경할 수 없습니다.

3. 완료되면 **검토를** 선택합니다.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="교육 고객 계정.":::

4. **검토를** 확인한 후 제출된 정보가 유효한 경우 **InReview** 상태가 표시됩니다. 

    :::image type="content" source="images/edu/create-review.png" alt-text="검토하는 교육 고객 계정."lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>교육 고객의 확인 상태 확인

고객의 **계정** 페이지에서 **특별 자격 상태를 참조하세요.**
상태 예제:

- 고객이 확인을 통과한 경우: 교육

   :::image type="content" source="images/edupassedvetting.png" alt-text="교육 확인에 성공했습니다.":::

- 고객이 확인을 통과하지 못한 경우: 교육 고객이 아닙니다.

   :::image type="content" source="images/edu/fail-reason.png" alt-text="교육 확인에 실패했습니다." lightbox="images/edu/fail-reason-expanded.png":::

- 고객이 교육 고객으로 태그가 지정되지 않은 경우: 없음

   :::image type="content" source="images/edu/account-one.png" alt-text="교육 고객은 이와 같이 태그가 지정되지 않습니다." lightbox="images/edu/account-one-expanded.png":::

- 고객이 교육 고객으로 검토 중인 경우: 검토 중

    :::image type="content" source="images/edu/in-review.png" alt-text="교육 고객이 검토 중입니다." lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>고객 계정 정보를 수정하고 확인을 위해 다시 제출합니다.

고객이 초기 확인에 실패하면 이제 정보를 수정하고 다시 제출할 수 있습니다.

### <a name="correct-the-customer-account-information"></a>고객 계정 정보 수정

고객 정보를 업데이트하려면 전역 관리자 권한이 있어야 합니다. 이 데이터는 파트너 센터 포털에서 업데이트할 수 없으므로 Office 365 포털에서 정보를 업데이트합니다.

1. **계정** 페이지에는 고객 자격이 "교육 고객이 아닌 고객"으로 간주된다는 정보가 표시됩니다.

2. 브라우저를 새로 고쳐 페이지를 다시 설정합니다. **업데이트** 단추가 있고 **특수 한정 상태가** **없음** 으로 설정됩니다.

3. **업데이트** 를 선택합니다. 서비스 **관리** 페이지에서 **Office 365를** 선택합니다.

4. 브라우저의 새 탭에서 Office 365 관리 센터로 리디렉션됩니다. 자격 증명으로 로그인하라는 요청이 있을 수 있습니다.

5. **설정** 을 선택합니다.

6. 화면 맨 위에 있는 **조직 프로필** 탭을 선택한 **다음, 조직 정보** 를 선택합니다. 이제 고객 세부 정보를 업데이트할 수 있습니다.

7. 사이드바 아래쪽에서 **변경 내용 저장을** 선택합니다.  

### <a name="resubmit-for-verification"></a>확인을 위해 다시 제출

1. 파트너 센터 탭 및 고객 **계정** 페이지로 이동합니다. 브라우저를 새로 고치고 회사 페이지가 새 정보로 업데이트되었는지 확인합니다. **업데이트** 단추를 선택하여 교육 재확인을 요청합니다.

2. 업데이트된 고객 세부 정보가 Education 제안에 적합한 경우 **특별 자격이** **Education으로** 업데이트됩니다. Not an **Education Customer가** 계속 표시되는 경우 수동 확인을 위해 지원에 문의하세요.

## <a name="next-steps"></a>다음 단계

- [특수 산업을 대상으로 판매](get-special-pricing-for-offers.md)

- [새 고객 추가](add-a-new-customer.md)

- [교육 고객에게 Minecraft: Education Edition 구독 판매](minecraft-subscriptions.md)
