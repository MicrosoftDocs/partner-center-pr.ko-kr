---
title: 고객의 Microsoft 클라우드 계약 동의 확인 | 파트너 센터
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft 클라우드 규약의 고객 동의를 확인 하는 방법에 대해 알아봅니다. 고객을 위한 Microsoft 제품 및 서비스를 주문 하는 데 필요할 수 있습니다.
author: LauraBrenner
ms.author: labrenne
keywords: 고객, 고객, 동의, MCA, Microsoft 클라우드 계약, 고객 계약 템플릿
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252586"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>고객의 Microsoft 클라우드 계약 동의 확인

**적용 대상**
-  파트너 센터

> [!NOTE]
> 규약 리소스는 현재 Microsoft 공용 클라우드의 파트너 센터 에서만 지원 됩니다. 다음에는 적용 되지 않습니다.
> * 21Vianet에서 운영하는 파트너 센터
> * Microsoft 클라우드 독일 파트너 센터
> * Microsoft Cloud for US Government 파트너 센터

>[!NOTE]
>이 계약은 2020 년 1 월 31 일까 지 유효 합니다. 이 날짜 이후에는 모든 고객 (기존 및 신규)이 새 Microsoft 고객 계약에 서명 해야 합니다. 자세히 알아보려면 [Microsoft 고객 계약의 고객 승인 확인](confirm-customer-agreement.md)을 참조 하세요.

파트너는 해당 고객에 대 한 Microsoft 제품 및 서비스를 주문 하기 전에 고객의 Microsoft 클라우드 계약에 동의 해야 합니다. 파트너가 규정 준수 요구 사항을 충족하도록 돕기 위해 Microsoft는 계약에 동의한 사람과 관련해 다음과 같은 세부 정보를 제공함으로써 파트너에게 동의 여부를 확인하도록 요구하고 있습니다. 

-   이름

-   성

-   메일 주소

-   전화 번호(선택 사항)

-   동의 날짜

자세히 알아보려면 Microsoft 클라우드 계약 고객 승인 확인 질문과 [대답](https://docs.microsoft.com/partner-center/confirm-consent-faq)을 참조 하세요.

다이렉트 청구서 파트너 및 간접 공급자 Microsoft 클라우드는 파트너 센터 또는 파트너 센터 API를 통해 거래 때 사용자 동의를 확인 해야 합니다. 확인이 *필수 사항*입니다.

해당 고객에 대해 확인 여부가 제공되지 않으면 다음과 같은 결과가 초래됩니다.

-   이 고객에 대 한 새 주문을 만들 수 없습니다.

-   이 고객에 대 한 기존 사용자 기반 구독의 좌석 수를 변경할 수 없습니다.

파트너 센터 또는 파트너 센터 API를 통해 고객 승인 확인을 수행할 수 있습니다. 파트너 센터 API를 통해이 작업을 수행 하려면 다음 항목을 참조 하세요. 

-   [고객 동의 확인](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [규약 메타 데이터 가져오기](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [고객 승인 확인](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


이는 프로덕션 환경과 샌드박스 환경 모두에 적용 됩니다.

## <a name="confirming-customer-acceptance-in-partner-center"></a>파트너 센터에서 고객 승인 확인

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>신규 고객에 대한 고객의 동의 여부를 확인합니다.

파트너 센터에서 새 고객 테 넌 트를 만드는 동안 고객 승인을 확인 하려면 다음 절차를 따르십시오. 관리자 에이전트 또는 판매 에이전트만 이러한 확인이 가능하다는 점에 유의하세요.

1. **고객**, **새 고객** 을 차례로 선택한 다음 **계정 정보**를 선택 합니다.
2. **회사** 및 **기본 연락처**에 대한 정보를 입력합니다.

![회사 정보](images/mca/mca1.png)

3. **Microsoft 클라우드 계약**에서 **고객이 최신 Microsoft 클라우드 계약에 동의했음**을 선택합니다.
4. **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.
5. 동의를 표한 사용자에 대한 세부 정보를 입력합니다.

![승인 날짜 추가](images/mca/MCA3.png)

기본적으로 기본 연락처의 고객 정보가 표시됩니다. 이것이 올바르지 않으면 **업데이트** 를 선택 하 고 규약을 수락한 사용자의 **이름**, **성**, **전자 메일 주소**및 **전화 번호* (선택 사항)를 입력 합니다.

6. 고객 테넌트를 생성하기 위한 나머지 단계들을 계속하려면 **다음**을 선택합니다.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>기존 고객에 대한 고객의 동의 여부를 확인

관리자 에이전트 또는 판매 에이전트만 이러한 확인이 가능합니다.

1. **고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.
2. **계정 정보**를 선택합니다.
3. **Microsoft 클라우드 계약**에서 **업데이트**를 선택합니다.

![업데이트](images/mca/mca4.png)

4. 계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.
5. **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.
6. **저장하고 계속하기**를 선택합니다.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>기존 고객에 대해 새로운 주문을 만드는 동안 고객의 동의 여부를 확인

이전에 확인 하지 않은 기존 고객에 대 한 새 주문을 만들려고 하면 확인을 완료 하 라는 메시지가 표시 됩니다. 다음 절차를 사용 하 여이 작업을 수행 합니다.

1. 계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.
2. **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.
3. **저장하고 계속하기**를 선택합니다.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>기존 고객에 대해 고객의 동의 여부를 확인

아래 절차를 사용하여 이전에 제공한 기존 고객에 대한 고객의 동의 여부를 확인할 수 있습니다. 관리자 에이전트 또는 판매 에이전트만 이러한 확인이 가능합니다.

1. **고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.
2. **계정 정보**를 선택합니다.
3. **Microsoft 클라우드 계약**에서이 고객에 대 한 확인이 제공 되었는지 여부를 확인할 수 있습니다.
