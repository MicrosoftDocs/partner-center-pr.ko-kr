---
title: 고객의 Microsoft 클라우드 계약 동의 확인 | 파트너 센터
ms.topic: article
ms.date: 04/5/2019
Description: 파트너는 해당 고객에 대해 Microsoft 제품 및 서비스를 주문하기 전에 Microsoft 클라우드 계약에 대한 고객 동의를 받아야 합니다. 보다 잘 파트너 규정 준수 요구 사항을 충족 Microsoft 파트너 요청 규약 동의 사용자에 대 한 특정 세부 정보를 제공 하 여 동의 확인 합니다.
author: LauraBrenner
ms.author: v-petand
keywords: 고객, 고객, 고객 계약 템플릿 MCA, Microsoft Cloud 계약 동의
ms.localizationpriority: medium
ms.openlocfilehash: 28bc7c1dea842f9fbfc2778dfad1a8e5615a6bd7
ms.sourcegitcommit: 275d3eee5613d52f0ac7b8c78f7a7ddd74f56c9e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/10/2019
ms.locfileid: "59430132"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>고객의 Microsoft 클라우드 계약 동의 확인

**적용 대상**
-  파트너 센터

파트너는 해당 고객에 대해 Microsoft 제품 및 서비스를 주문하기 전에 Microsoft 클라우드 계약에 대한 고객 동의를 받아야 합니다. 파트너가 규정 준수 요구 사항을 충족하도록 돕기 위해 Microsoft는 계약에 동의한 사람과 관련해 다음과 같은 세부 정보를 제공함으로써 파트너에게 동의 여부를 확인하도록 요구하고 있습니다. 

-   이름

-   성

-   메일 주소

-   전화 번호

-   동의 날짜

자세한 내용은 Microsoft 클라우드 계약 고객 승인 확인을 참조 하세요 [Frequently Asked Questions](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq)합니다.

직접 청구 파트너 및 간접 공급자는 파트너 센터 또는 파트너 센터 API를 통해 구속력 있는 경우 Microsoft 클라우드 계약의 고객 승인을 확인 해야 합니다. 확인이 *필수 사항*입니다.

해당 고객에 대해 확인 여부가 제공되지 않으면 다음과 같은 결과가 초래됩니다.

-   이 고객에 대해 새로운 주문을 생성할 수 없습니다.

-   이 고객에 대해 기존의 사용자 수 기준 구독의 사용자 수를 변경할 수 없습니다.

파트너 센터 또는 파트너 센터 API를 통해 고객 승인의 확인을 수행할 수 있습니다. 파트너 센터 API를 통해이 작업을 수행 하려면 다음 항목을 참조 합니다. 

-   [가져오기의 고객 동의 확인](https://docs.microsoft.com/en-us/partner-center/develop/get-confirmation-of-customer-consent)

-   [계약 메타 데이터 가져오기](https://docs.microsoft.com/en-us/partner-center/develop/get-agreement-metadata)

-   [고객 동의 확인](https://docs.microsoft.com/en-us/partner-center/develop/confirm-customer-consent)


고객의 동의 여부 확인은 Microsoft 공용 클라우드에서만 지원됩니다.

이 프로덕션 및 샌드박스 환경 모두에 적용 됩니다.

## <a name="confirming-customer-acceptance-in-partner-center"></a>파트너 센터에서 고객 승인 확인

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>신규 고객에 대한 고객의 동의 여부를 확인합니다.

다음 절차를 사용 하 여 파트너 센터에서 새 고객 테 넌 트를 만드는 동안 고객 동의 확인 합니다. 관리자 에이전트 또는 판매 에이전트만 이러한 확인이 가능하다는 점에 유의하세요.
 
1.  선택 **고객이**를 차례로 **새 고객** 선택한 후 **계정 정보**합니다.

2.  **회사** 및 **기본 연락처**에 대한 정보를 입력합니다.

![회사 정보](images/mca/mca1.png)

3.  **Microsoft 클라우드 계약**에서 **고객이 최신 Microsoft 클라우드 계약에 동의했음**을 선택합니다. 

4.  **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

5.  동의를 표한 사용자에 대한 세부 정보를 입력합니다. 

![승인 날짜를 추가 합니다.](images/mca/MCA3.png)

기본적으로 기본 연락처의 고객 정보가 표시됩니다. 이 정보가 틀린 경우에는 **업데이트**를 선택하고 계약에 동의한 사람의 **이름**, **성**, **이메일 주소** 및 **전화 번호*(선택 사항)를 입력합니다.

6.  고객 테넌트를 생성하기 위한 나머지 단계들을 계속하려면 **다음**을 선택합니다.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>기존 고객에 대한 고객의 동의 여부를 확인

관리자 에이전트 또는 판매 에이전트만 이러한 확인이 가능합니다. 

1.  **고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다. 

2.  선택 **계정 정보**합니다.

3.  **Microsoft 클라우드 계약**에서 **업데이트**를 선택합니다.

![Update](images/mca/mca4.png)

4.  계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.

5.  **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

6.  **저장하고 계속하기**를 선택합니다.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>기존 고객에 대해 새로운 주문을 만드는 동안 고객의 동의 여부를 확인

앞서 동의 여부를 확인하지 않은 기존 고객에 대해 새로운 주문을 생성하려고 하면 확인을 완료하라는 메시지를 받게 됩니다. 다음 절차를 사용 하 여이 작업을 수행 합니다. 

1.  계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.

2.  **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

3.  **저장하고 계속하기**를 선택합니다.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>기존 고객에 대해 고객의 동의 여부를 확인

아래 절차를 사용하여 이전에 제공한 기존 고객에 대한 고객의 동의 여부를 확인할 수 있습니다. 관리자 에이전트 또는 판매 에이전트만 이러한 확인이 가능합니다. 

1.  **고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다. 

2.  선택 **계정 정보**합니다.

3.  **Microsoft 클라우드 계약**에서 이 고객에 대해 확인이 제공되었는지 여부를 볼 수 있습니다.

