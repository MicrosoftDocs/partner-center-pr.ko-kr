---
title: 고객의 Microsoft 고객 계약 동의 확인 | 파트너 센터
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft 고객 계약의 고객 동의를 확인 하는 방법에 대해 알아봅니다. 고객을 위한 Microsoft 제품 및 서비스를 주문 하는 데 필요할 수 있습니다.
author: LauraBrenner
ms.author: labrenne
keywords: 고객, 고객, 동의, MCA, Microsoft 클라우드 계약, Microsoft 고객 계약, 고객 계약 템플릿
ms.localizationpriority: medium
ms.openlocfilehash: 8beee9ed9035ff846c6e9d84fefd0c5c2ba255de
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721365"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Microsoft 고객 계약의 고객 승인 확인

**적절한 역할**

- 관리자 에이전트
- 영업 에이전트

현재는 CSP 파트너가 고객을 대신 하 여 주문할 수 있기 전에 해당 하는 **Microsoft 클라우드 계약**에 동의 하 고 서명 해야 합니다. 그러면 파트너가 Microsoft에 서명자에 대한 정보를 제공하여 고객의 동의 여부를 확인해야 합니다. 확인이 제공되지 않는 경우:
- 이 고객에 대 한 새 주문을 만들 수 없습니다.
- 이 고객에 대 한 기존 사용자 기반 구독의 좌석 수를 변경할 수 없습니다.

파트너 센터 대시보드 또는 API를 사용하여 고객의 Microsoft 클라우드 계약 동의 여부를 확인하는 방법에 대한 자세한 내용은 [Microsoft 클라우드 계약에 대한 고객 동의 여부 확인](confirm-consent.md)을 참조하세요.

2019년 10월 1일에 Microsoft는 CSP 프로그램에 Microsoft 클라우드 계약을 대체하는 **Microsoft 고객 계약**을 도입할 예정입니다. 파트너가 새 계약으로 원활하게 마이그레이션할 수 있도록 2020년 1월 31일까지 현재 Microsoft 클라우드 계약이 CSP 프로그램에서 지원될 예정입니다. 일정에 대한 자세한 내용은 다음 표를 참조하세요.

| 날짜 | 마일스톤 | 세부 정보 |
|------------|------------|--------------------------------|
|2019년 8월 1일|샌드박스 환경에서 UX 미리 보기 사용 가능|파트너는 CSP 샌드박스 환경에서 파트너 센터 대시보드를 사용하여 Microsoft 고객 계약에 대한 고객의 동의 여부를 확인할 수 있습니다. CSP 샌드박스 환경에 액세스할 수 있는 파트너는 사용자 환경 변경 사항을 미리 볼 수 있습니다. 샌드박스 액세스 권한이 없는 파트너는 이 항목의 변경 사항에 대해 알아볼 수 있습니다.|
|2019년 9월 3일|샌드박스 환경에서 API 미리 보기를 사용할 수 있습니다.|파트너는 CSP 샌드박스 환경에서 파트너 센터 API를 사용하여 Microsoft 고객 계약에 대한 고객의 동의 여부를 확인할 수 있습니다. API 파트너는 이 기회를 사용하여 API 변경 사항을 미리 보고 API 통합 작업을 시작하여 새 계약을 지원할 수 있습니다.|
|2019 년 9 월 20 일|샌드박스 환경에서 .NET SDK 미리 보기를 사용할 수 있습니다.|파트너는 CSP 샌드박스 환경에서 파트너 센터 .NET SDK를 사용하여 Microsoft 고객 계약에 대한 고객의 동의 여부를 확인할 수 있습니다. API 파트너는 이 기회를 사용하여 .NET SDK 변경 사항을 미리 보고 API 통합 작업을 시작하여 새 계약을 지원할 수 있습니다.|
|2019년 10월 1일|프로덕션 환경에서 Microsoft 고객 계약 사용 가능|Microsoft는 CSP 프로그램에 Microsoft 클라우드 계약을 대체하는 Microsoft 고객 계약을 도입합니다. 파트너는 프로덕션 환경에서 파트너 센터 대시보드 및 API를 사용하여 Microsoft 고객 계약에 대한 고객의 동의 여부를 확인할 수 있습니다. Microsoft 클라우드 계약은 CSP 파트너 프로그램 내에서 계속 지원됩니다. 그러나 파트너는 Microsoft 고객 계약으로 마이그레이션을 시작하는 것이 좋습니다. 신규 구매 및 기존 구독의 사용자 수 변경에는 Microsoft 고객 계약 또는 Microsoft 클라우드 계약의 파트너 확인이 필요합니다. 특정 새 제품(예: 새 Azure 요금제)은 Microsoft 고객 계약을 확인해야 합니다.|
|2020년 1월 31일|프로덕션 환경에서 Microsoft 클라우드 계약이 제거됨|Microsoft 클라우드 계약은 CSP 파트너 프로그램 내에서 더 이상 허용되지 않습니다. 신규 구매 및 기존 구독의 사용자 수 변경에는 Microsoft 고객 계약의 파트너 확인이 필요합니다. 이 요구 사항은 새 고객과 이전에 Microsoft 클라우드 계약에 동의한 기존 고객에게 적용됩니다.|

## <a name="access-microsoft-customer-agreement-template"></a>Microsoft 고객 계약 템플릿 액세스
파트너는 [여기](https://aka.ms/customeragreement)에서 최신 버전의 Microsoft 고객 계약 템플릿을 수동으로 다운로드할 수 있습니다. Microsoft 고객 계약은 국가별로 지정 되어 있습니다. Microsoft 고객 계약 템플릿을 요청할 때 고객의 위치에 따라 올바른 국가를 선택 해야 합니다. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>파트너 센터 API/SDK를 사용 하 여 고객 승인 확인
파트너는 파트너 센터 API/SDK를 사용 하 여 Microsoft 고객 계약에 대 한 고객의 동의를 확인할 수 있습니다. API/SDK에 대 한 자세한 내용은 다음을 참조 하세요.

- [Microsoft 고객 계약에 대한 계약 메타데이터 가져오기](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [고객의 Microsoft 고객 계약 동의 여부 확인](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [고객의 Microsoft 고객 계약 동의 확인 정보 가져오기](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft 고객 계약 템플릿 다운로드 링크 가져오기](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>파트너 센터에서 고객의 동의 여부 확인
파트너는 새 고객과 기존 고객을 위해 파트너 센터에서 Microsoft 고객 계약에 대 한 고객의 동의를 확인할 수 있습니다.

### <a name="confirm-customer-acceptance-for-new-customers"></a>신규 고객에 대한 고객의 동의 여부 확인

파트너 센터에서 새 고객 테넌트를 만들 때 다음 단계를 따라 고객이 Microsoft 고객 계약에 동의하는지 확인합니다. 이러한 단계는 관리 담당자 또는 판매 담당자가 수행해야 합니다.

1. **고객**을 선택한 다음, **신규 고객**을 선택합니다.

2. **계정 정보**에서 회사 및 기본 연락처의 정보를 입력합니다.

3. **Microsoft 계약**에서 **Microsoft 고객 계약**을 선택합니다.

4. **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

5. 표시된 기본 사용자 연락처 정보가 올바른지 확인합니다. 이 정보가 틀린 경우에는 **업데이트**를 선택하고 계약에 동의한 사람의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.

6. 고객 테넌트를 생성하기 위한 나머지 단계를 계속하려면 **다음**을 선택합니다.

![새 고객](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>기존 고객의 경우 고객 동의 여부 확인

관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.

1. **고객**을 선택합니다. 고객을 찾아 선택합니다.

2. **계정 정보**를 선택합니다.

3. **Microsoft 고객 계약**에서 **업데이트**를 선택합니다.

4. 계약에 동의한 사람의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다. **계약 동의 날짜**에 해당 날짜를 입력합니다. 이 날짜는 미래의 날짜로 설정할 수 없습니다.

5. **저장**을 선택하고 계속합니다.

![기존 고객](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>고객 동의 여부 확인 검색

다음 단계를 따라 기존 고객이 Microsoft 고객 계약에 동의했다는 확인을 검색할 수 있습니다. 관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.

1. **고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.

2. **계정 정보**를 선택합니다.

3. **Microsoft 고객 계약**에서 이 고객이 확인을 제공했는지 여부를 확인합니다.
