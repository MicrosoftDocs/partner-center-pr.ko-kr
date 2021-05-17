---
title: 2021년 3월 공지
description: 새로운 기능, 프로모션, 제품, 시장 또는 기존 제품의 변경 사항 등 Microsoft 파트너 센터에 대한 2021년 3월 공지입니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 3d91eb26f98005b92a48c6f242ea4439e42cde05
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702878"
---
# <a name="march-2021-announcements"></a>2021년 3월 공지

이 페이지에서는 2021년 3월 Microsoft 파트너 센터에 대한 공지를 제공합니다.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>준비: CSP(클라우드 솔루션 공급자) 고객 주소 유효성 검사 API에 대한 변경 사항이 6월부터 적용. 현재 테스트 기능 사용 가능

### <a name="categories"></a>범주

- 날짜: 2021-03-30
- 준비

### <a name="summary"></a>요약

파트너와 고객이 신뢰를 기반으로 비즈니스를 운영할 수 있도록 전 세계 모든 국가에서 주소 유효성 검사 API의 변경 사항을 테스트하도록 파트너를 초대합니다.

### <a name="impacted-audience"></a>영향을 받는 대상

새 고객 주소 정보를 만들거나 기존 고객 주소 정보를 업데이트하는 CSP 직접 청구 파트너 및 간접 공급자.

### <a name="details"></a>세부 정보

Microsoft는 신뢰할 수 있는 방식으로 운영되며, 규정을 준수하고 안전하며 보안이 유지되는 고객 주소 유효성 검사 방법을 제공하여 CSP 프로그램에서 고객 구독을 거래할 수 있도록 최선을 다하고 있습니다. 2021년 3월 31일에 2021년 6월 변경 사항을 적용하기 전에 파트너를 초대하여 테스트한 주소 유효성 검사 API에 대한 변경 사항을 도입했습니다.

변경 사항은 주소 유효성 검사 API에만 적용됩니다. 고객 만들기 및 청구 프로필 업데이트 API는 영향을 받지 않습니다.

응답에서 다음 상태 메시지 중 하나를 반환합니다.

| 상태     | Description |    반환되는 추천 주소 수 |
|-------|---------------|-------------------|
|배송 가능 확인됨 | 주소가 확인되어 제품을 배송할 수 있습니다. | Single |
|확인됨 | 주소가 확인되었습니다. | 한 개 |
|상호 작용 필요 | 제안된 주소가 많이 변경되어 사용자 확인이 필요합니다. | 한 개 |
|거리명 부분 | 주소에 입력된 거리명이 완전하지 않아 추가 정보가 필요합니다. | 여러 개(최대 3개) |
|부지 부분 | 입력된 부지(건물 번호, 다세대 동호수 등)가 완전하지 않아 추가 정보가 필요합니다. | 여러 개(최대 3개) |
|여러 개 | 주소에서 완전하지 않은 필드가 여러 개 있습니다(거리명 부분과 부지 부분 포함). | 여러 개(최대 3개) |
|없음 | 주소가 올바르지 않습니다. | 없음 |
|확인 안 함 | 유효성 검사 프로세스를 통해 주소를 보낼 수 없습니다. | 없음 |

미국 우편 번호는 추가 4자리 + 하이픈(-)을 반환합니다(예: 12345-6789).

주소 유효성 검사 API를 통해 유효성 검사를 위해 주소가 제출되면 다음 응답 스키마가 반환됩니다.

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

이 샘플 응답을 잘 보세요. 미국의 경우 우편 번호에 5자리 숫자만 입력하면 우편 번호 줄에 4자리 숫자 접미사가 추가된 응답이 반환됩니다.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>다음 단계

- 업데이트 준비를 시작할 수 있도록 테스트에 참여하는 실무 전문가 Ali Khaki씨와 샌드박스 테넌트 ID를 공유합니다.

- CPV(제어판 공급업체) 솔루션을 사용하는 경우 CPV에 문의하세요.

### <a name="questions"></a>질문이 있으신가요?

Microsoft 제품을 사용한 작업에 대해 지원이 필요한 경우 파트너 지원 Yammer 그룹에 문의하세요.

### <a name="change-log"></a>로그 변경:

- 2020년 3월 31일: 최초 게시

- 2021년 4월 30일: 샘플 응답 및 우편 번호 정보 업데이트

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>새 EAC(Exchange 관리 센터) 환경

### <a name="categories"></a>범주

- 날짜: 2021-03-29
- 기능

### <a name="summary"></a>요약

2021년 4월 27일부터 EAC(Exchange 관리 센터)는 사용자의 일상적인 효율성을 개선하는 새로운 환경을 도입합니다.

### <a name="impacted-audience"></a>영향을 받는 대상

파트너 센터를 통해 Exchange에 액세스하는 위임된 관리자

### <a name="details"></a>세부 정보

2021년 4월 27일부터 파트너 센터를 통해 Exchange로 이동하는 파트너는 새 EAC로 리디렉션됩니다.

이 새로운 환경은 현재 미리 보기로 제공되며, 관리자는 기존 EAC 내에서 오른쪽 위 모서리의 토글을 선택하여 이 환경을 활성화할 수 있습니다. 모든 페이지에 표시되는 "지금 사용해 보기" 배너를 선택하여 새 EAC로 이동할 수도 있습니다.

새 EAC의 이점은 다음과 같습니다.

- 메일 흐름 관련 문제에 대한 인사이트, 보고서 및 경고 메커니즘이 추가되었습니다. 

- 맞춤형 대시보드로 생산성을 향상할 수 있습니다.

새 환경을 탐색하는 방법을 안내하기 위해 새 EAC 환경의 **학습 및 가이드** 섹션에 비디오가 제공됩니다. 새 포털을 최대로 활용하는 방법을 알아볼 수 있습니다.

>[!NOTE]
>이 변경 내용이 적용되면 기존 EAC 환경은 더 이상 사용되지 않습니다. 변경 내용이 구현되기 전에 미리 통보됩니다.

### <a name="next-steps"></a>다음 단계

- 새 환경의 스크린샷을 볼 수 있는 [이 토픽에 대한 리소스](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)를 확인하세요.

- 이 정보를 조직의 적절한 관련자와 공유합니다. 

### <a name="questions"></a>궁금한 점이 더 있나요?

이 변경 내용에 대해 궁금한 점이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: 제품 출시 일정 소개

### <a name="categories"></a>범주

- 날짜: 2021-03-25
- 제품 | 최신 작업 공간

### <a name="summary"></a>요약

파트너 피드백에 대응하기 위한 조치로 Microsoft Operations에서는 제품 출시에 대한 통신문을 간소화할 것입니다.

### <a name="impacted-audience"></a>영향을 받는 대상

CSP(클라우드 솔루션 공급자) 파트너

### <a name="details"></a>세부 정보

Microsoft는 파트너 환경을 지속적으로 개선하기 위해 최선을 다하고 있습니다. 제품 출시에 대한 중복 공지를 포함하여 Microsoft에서 보내는 통신문이 너무 많다는 피드백을 받았습니다.

이러한 피드백에 대응하기 위해 Microsoft는 새 제품과 기존 제품의 제품 출시를 위한 준비 환경을 간소화했습니다.

이제 제품 출시 정보 보기가 한 달에 한 번만 제공되며, Operations Readiness 리소스 갤러리에 게시됩니다. 이 월간 [제품 출시 일정 보기](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)는 Operations Readiness 리소스 갤러리와 파트너 센터 공지의 개별 제품 출시 통신문을 대체합니다.

[커뮤니티 컬렉션](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [일정 보기](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)및 [CSP 뉴스레터](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)에서도 이 [제품 출시 일정](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)에 액세스할 수 있습니다. 매월 제품 출시 일정을 게시할 때 Operations Readiness 리소스 갤러리에 공지를 올려 소식을 알려 드리겠습니다.

가격표 미리 보기 및 가격표 변경 로그뿐 아니라 제품 블로그, 라이선스 가이드 및 제품 마케팅 페이지에서 신제품과 기존 제품에 대한 정보를 계속 찾을 수 있습니다.

변경 내용은 다음 제품이 출시될 때 적용됩니다.

- Dynamics 온-프레미스
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- 서버  
- 도구
- Teams 및 Telco

Operations Readiness 정보가 필요한 제품 출시에 대한 공지를 계속 보내 드립니다.

### <a name="next-steps"></a>다음 단계

이 토픽에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관련자와 공유합니다.

### <a name="questions"></a>궁금한 점이 더 있나요?

이러한 제품에 대한 추가 질문은 관련 Yammer 커뮤니티를 확인하세요.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>CSP 고객 등록 요구 사항에 대한 변경 내용

### <a name="categories"></a>범주

- 날짜: 2021-03-25
- 기능

### <a name="summary"></a>요약

파트너와 고객이 신뢰를 바탕으로 비즈니스를 운영할 수 있도록 지원하기 위한 노력의 일환으로 Microsoft는 2021년 3월 25일부터 추가 고객 정보를 요청합니다.

### <a name="impacted-audience"></a>영향을 받는 대상

다음 섹션에 나열된 국가에 신규 또는 기존 고객이 있는 CSP(클라우드 솔루션 공급자) 직접 청구 파트너 및 간접 공급자

### <a name="details"></a>세부 정보

Microsoft는 신뢰할 수 있는 방식으로 운영되며, 규정을 준수하고 안전하며 보안이 유지되는 고객 유효성 검사 방법을 제공하여 CSP 프로그램에서 고객 구독을 거래할 수 있도록 최선을 다하고 있습니다. 2021년 3월 25일에 다음 조건을 모두 충족하는 파트너에게 영향을 주는 파트너 센터 API 및 UI(사용자 인터페이스)의 향상된 기능이 도입됩니다.

1. 파트너는 Microsoft와 직접 청구 관계를 맺고 있습니다(즉, 파트너가 직접 청구 파트너 또는 간접 공급자임).

2. 파트너가 다음 국가의 신규 또는 기존 고객과 함께 비즈니스를 수행합니다.

    - 태국
    - 베트남
    - 터키
    - 폴란드
    - 남아프리카
    - 인도
    - 브라질
    - 이라크
    - 미얀마
    - 남수단
    - 사우디아라비아
    - 아랍에미리트연합국
    - 베네수엘라

조건을 충족하는 파트너는 신규 고객을 등록하거나 기존 고객의 세부 정보를 수정할 때 고객의 **회사 등록 ID**(고객의 **조직 INN** 이라고도 함) 및 **전화 번호** 를 제출해야 합니다. 이러한 파트너는 고객에 대한 선택적 **중간 이름** 을 입력할 수도 있습니다.

회사 등록 ID를 추가할 때 고객 개인 ID가 아닌 회사 납세자 식별 번호를 사용해야 합니다.

다음 국가에서 신규 또는 기존 고객과 거래하는 파트너는 이미 2020년 11월의 이전 릴리스에 등록되었습니다.

- 아르메니아
- 아제르바이잔
- 벨라루스
- 헝가리
- 카자흐스탄
- 키르기스스탄
- 몰도바
- 러시아
- 타지키스탄
- 우크라이나
- 우즈베키스탄

전 세계의 나머지 지역에 있는 고객을 대상으로 하는 파트너는 2021년 3월 25일에 고객의 **회사 등록 ID**, **전화 번호** 및 **중간 이름** 을 선택적 세부 정보로 입력할 수 있습니다.

### <a name="next-steps"></a>다음 단계

- [전용 파트너 컬렉션](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)에서 기술 설명서 및 질문과 대답을 검토하여 자세한 지침을 확인합니다.

- 파트너 센터 API 및 웹 사용자 환경을 사용하여 변경 내용을 통합할 준비를 합니다. API/SDK는 테스트에 사용할 수 있습니다.

- 신규 고객을 등록하거나 기존 고객 세부 정보를 수정하는 경우 추가 데이터를 제출해야 합니다.

- CPV(제어판 공급업체) 솔루션을 사용하는 경우 CPV에 문의하세요.

### <a name="questions"></a>질문이 있으신가요?

법인 식별자(INN 또는 TIN이라고도 함)와 관련된 질문이 있는 경우 세무 고문 또는 지역 세무서에 문의하세요. Microsoft는 세금 문제에 대한 지침을 제공할 수 없습니다.

Microsoft와의 작업에 대한 지원이 필요한 경우 [서비스 요청을 여세요](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>2021년 3월 1일 영구 소프트웨어 가격표 수정

### <a name="categories"></a>범주

- 날짜: 2021-03-23
- 제품/시장

### <a name="impacted-audience"></a>영향을 받는 대상

클라우드 솔루션 공급자 프로그램에서 영구 소프트웨어를 거래하는 간접 공급자 및 직접 청구 파트너 

### <a name="details"></a>세부 정보

2021년 3월 1일에 게시된 영구 소프트웨어의 가격표에 잘못된 시장이 포함되었습니다. 2021년 3월 17일에 영구 소프트웨어 가격표에 수정 사항이 업데이트되었습니다. 이러한 수정 사항은 다음에만 적용됩니다.

- 제품 ID: DF77X4D43RKT 
- 제품 이름: Windows 10 Home to Pro Upgrade for Microsoft 365 Business
- 제거되었거나 지원되지 않는 시장: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

이러한 변경 내용은 위의 제품에만 적용됩니다. 다른 제품은 수정되지 않았습니다. 

### <a name="next-steps-and-resources"></a>다음 단계 및 리소스

- 영구 소프트웨어를 거래하는 파트너는 최신 소프트웨어 가격표를 다운로드해야 합니다.
- 두 글자로 된 약어와 해당 국가의 간편한 대응표는 [지역 국가 번호](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)를 참조하세요.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a>.NET Standard(v1.17.0)의 SDK 릴리스

### <a name="categories"></a>범주

- 날짜: 2021-03-23

- 기능
 
### <a name="impacted-audience"></a>영향을 받는 대상

파트너 센터 .NET SDK를 사용하는 CSP 프로그램에 참여하는 Direct Bill 파트너 및 간접 공급자

### <a name="details"></a>세부 정보

2020년 3월 23일부터 파트너는 업데이트된 퍼블릭 파트너 센터 SDK [GitHub 샘플](https://github.com/Microsoft/Partner-Center-DotNet-Samples)과 함께 [MicrosoftPartnerCenter.NETSDK(NuGet 갤러리 | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)를 다운로드할 수 있습니다. 이 버전에는 다음 방법에 대한 업데이트가 포함됩니다.

#### <a name="audit-updated-new-operation-types"></a>감사 업데이트: 새 작업 유형

고객이 DAP를 승인하고 종료한 시점을 파악하기 위한 새 [작업 유형](https://docs.microsoft.com/partner-center/develop/auditing-resources)이 추가되었습니다.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>감사 업데이트: 새 리소스 및 작업 유형

고객 디렉터리 역할 시나리오를 지원하기 위한 새 [리소스 및 작업 유형](https://docs.microsoft.com/partner-center/develop/auditing-resources)이 추가되었습니다.

- 새 리소스 유형 "CustomerDirectoryRole"

- 작업 유형 "AddUserMember" 및 "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>고객 계정에 대한 SDK 업데이트

- GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus 지원

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>추가 변경 내용

다음 변경 내용은 새 상거래의 일부로 도입되었으며 현재 M365/D365 새 상거래 환경 기술 미리 보기에 속하는 파트너에게만 초대를 통해 제공됩니다. 새 상거래 기술 미리 보기에 속하지 않는 파트너는 영향을 인지할 수 없으며 이전 버전과 호환되어야 합니다.

- 카탈로그 변경:

  - GET /products/{product-id}/skus/{sku-id}

- 구매 및 관리:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>다음 단계

- 최신 버전의 [MicrosoftPartnerCenter.NETSDK(NuGet 갤러리 | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) 다운로드
- [GitHub 샘플](https://github.com/Microsoft/Partner-Center-DotNet-Samples) 다운로드 및 검토

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP 상업용 Marketplace 제품 및 적격 제품에 대한 FY21 CSP 인센티브

### <a name="categories"></a>범주

- 날짜: 2021-03-18
- 기능

### <a name="impacted-audience"></a>영향을 받는 대상

클라우드 솔루션 공급자 프로그램의 간접 공급자 및 직접 청구 파트너 

### <a name="details"></a>세부 정보

클라우드 솔루션 공급자 프로그램의 간접 공급자 및 직접 청구 파트너는 타사 제품을 판매하고, 파트너 센터 또는 Azure Portal에서 거래한 각 적격 타사 제품에 대한 리베이트 인센티브를 받을 수 있습니다. 이 인센티브는 적격 제품에 청구된 매출에 대한 리베이트 형태로 **2021년 6월 30일까지 제공** 됩니다.  

아래에서 이 CSP 상업용 Marketplace 제품 인센티브에 대해 계속 알아보고, 오늘 고객에게 연락하여 지속적인 성공 및 디지털 변환을 가능하게 해주는 올바른 제품을 확인하세요.

Microsoft는 ISV(독립 소프트웨어 공급업체)와 협력하여 Microsoft 고객을 위한 최신 IaaS 및 SaaS 솔루션을 출시했습니다. ISV 게시자는 Microsoft 파트너 채널을 통해 제품 판매를 가능하게 할 수 있습니다. Microsoft의 인센티브 지급 대상 제품은 다음과 같은 두 가지 범주로 나뉩니다.

- Azure IP 공동 판매 인센티브화 상태의 SaaS 및 IaaS 타사 제품을 선택합니다. 

- PowerPoint, Word, Excel, Outlook 또는 SharePoint 같은 Microsoft 365 생산성 앱 2개 이상 또는 Teams가 통합된 SaaS 애플리케이션

### <a name="next-steps-and-resources"></a>다음 단계 및 리소스

- 인센티브 지급 대상 Marketplace 앱을 판매한 후 [파트너 인센티브](https://partner.microsoft.com/membership/partner-incentives)를 획득하는 방법에 대해 알아봅니다. 새 제품은 매월 추가됩니다.  
- [클라우드 솔루션 공급자 직접 청구 파트너 인센티브 리소스](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [클라우드 솔루션 공급자 간접 공급자 인센티브 리소스](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- 이 [프레젠테이션](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)을 검토하여 상업용 Marketplace 앱을 판매하는 방법에 대해 자세히 알아보세요. [여기](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)에서 추가 리소스를 확인하세요. 
- [파트너 센터](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) 또는 [Azure Portal](https://ms.portal.azure.com/#home)에서 상업용 Marketplace 카탈로그 살펴보기
- [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)를 사용하여 회사의 Marketplace에 앱 통합
- 함께 비즈니스를 수행하고 싶은 ISV에게 연락하세요.
- 간접 공급자는 API 사용을 통합하고 판매할 앱을 재판매인에게 안내해야 합니다.

### <a name="questions"></a>질문이 있으세요?  

파트너 센터의 상업용 Marketplace에 대한 개요는 [이 문서](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)를 참조하세요.

추가 지원이 필요한 경우 파트너 센터에서 지원 요청을 만들 수 있습니다. [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1)에서 자세히 알아보세요.

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium 제품 이름 지정 및 필수 구성 요소 업데이트

### <a name="categories"></a>범주

- 날짜: 2021-03-18
- 기능

### <a name="summary"></a>요약

Power BI Premium Per User 제품의 명명 및/또는 필수 구성 요소 정보를 명확히 하기 위해 2021년 4월 1일에 최종 가격표가 업데이트됩니다.

### <a name="impacted-audience"></a>영향을 받는 대상

CSP(클라우드 솔루션 공급자) 직접 및 간접 파트너

### <a name="details"></a>세부 정보

Power BI Premium Per User 제품의 명명 및/또는 필수 구성 요소 정보를 명확히 하기 위해 2021년 4월 1일에 최종 가격표가 업데이트됩니다.

최종 가격표가 업데이트될 때까지 이 섹션의 정보를 사용하여 올바른 제품을 주문하도록 하세요.

다음 세부 정보는 영향을 받는 SKU 및 필수 구성 요소를 자세히 보여 줍니다.

| 3월 1일 가격표 미리 보기의 제품 표시 이름 |  4월 1일 최종 가격표에서 업데이트된 제품 표시 이름| 제품 ID |
| ------ | ----------- | ----------- |
| Power BI Premium Per User Add-On(비영리 직원 가격)  |  Power BI Premium Per User 추가 기능 **(Office)** (비영리 직원 가격)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

이 제품을 구매하려는 고객은 다음 필수 구성 요소 중 하나가 있어야 합니다.

| 제품 표시 이름 | 제품 ID |
| ------ | ----------- |
| Microsoft 365 E5(비영리 직원 가격)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   오디오 회의 제외 Microsoft 365 E5(비영리 직원 가격)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5(비영리 직원 가격)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5(비영리 직원 가격) 평가판|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   오디오 회의 제외 Office 365 E5(비영리 직원 가격)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

다음 Power BI Premium 제품을 구매하려면 필수 구성 요소가 있어야 합니다.

| 제품 표시 이름 | 제품 ID |
| ------ | ----------- |
|   Power BI Premium Per User Add-On(비영리 직원 가격)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

이 제품을 구매하려는 고객은 이러한 필수 구성 요소가 있어야 합니다.

| 제품 표시 이름 | 제품 ID |
| ------ |----------|
| Power BI Pro(비영리 직원 가격)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>다음 단계

이 항목에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관련자와 공유합니다.  

### <a name="questions"></a>궁금한 점이 더 있나요?

이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Microsoft 365 F3의 3월 가격 업데이트

### <a name="categories"></a>범주

- 날짜: 2021-03-16
- 제품/시장

### <a name="summary"></a>요약

2021년 3월 가격표에서 Microsoft 365 F3 영국 파운드(GBP) 및 유로(EUR)의 잘못된 가격이 수정되었습니다.

### <a name="impacted-audience"></a>영향을 받는 대상

2021년 3월 1일과 3월 17일 사이에 CSP(클라우드 솔루션 공급자) 프로그램을 통해 GBP 또는 EUR로 Microsoft 365 F3을 구매한 파트너

### <a name="details"></a>세부 정보

Microsoft에서 Microsoft 365 F3의 잘못된 가격을 수정했습니다. 잘못된 가격은 2021년 3월 1일과 3월 17일 사이에 GBP 및 EUR로 구매한 제품에만 해당됩니다. 영향을 받는 제품과 통화는 아래에 나와 있습니다. 

| Offer name | 통화 | 제품 ID | 소재 ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3(자선) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3(상업용) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
3월 및 4월 미리 보기 라이선스 기반 가격표는 태평양 표준시를 기준으로 3월 16일 오후 5시에 업데이트되었습니다.

### <a name="next-steps"></a>다음 단계

- 파트너는 해당하는 경우 이러한 가격 수정 사항이 포함된 최신 라이선스 기반 가격표(3월 및 4월 미리 보기 모두)를 다시 다운로드해야 합니다.  
- Microsoft는 앞으로 몇 주간 이메일을 통해 영향을 받는 파트너에게 연락하여 관련 거래 시정과 관련된 다음 조치를 알려 드릴 예정입니다.

### <a name="questions"></a>궁금한 점이 더 있나요?

추가 질문은 관련 CSP Yammer 커뮤니티를 확인하세요.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a>파트너 센터를 통해 법적 회사 이름 업데이트

### <a name="categories"></a>범주

- 날짜: 2021-03-16
- 효율성 및 스케일링 향상

### <a name="summary"></a>요약

2021년 3월부터 MPN(Microsoft Partner Network) 파트너와 CSP(Cloud Solution Provider) 간접 재판매인은 파트너 센터를 통해 법적 회사 이름을 업데이트할 수 있습니다.

### <a name="impacted-audience"></a>영향을 받는 대상

MPN 파트너 및 CSP 간접 재판매인(CSP 다이렉트 청구 파트너에게는 적용되지 않음)

### <a name="details"></a>세부 정보

2021년 3월부터 MPN 파트너 및 CSP 간접 재판매인은 규정을 준수하는 셀프 서비스 방식으로 파트너 센터를 통해 법적 회사 이름을 업데이트할 수 있습니다. 이 새로운 기능을 통해 파트너는 더 이상 회사 이름을 업데이트하기 위해 파트너 센터 지원 티켓을 제출할 필요가 없습니다. 따라서 파트너는 이 작업을 수행할 때 상당한 시간을 절약할 수 있습니다. 

자세히 알아보려면 [법적 비즈니스 프로필 업데이트](../update-your-partner-profile.md#update-your-legal-business-profile)를 참조하세요.

>[!NOTE]
>법적 비즈니스 프로필에 있는 회사 이름에 철자 오류와 약어가 없으며 정식 회사 비즈니스 등록 기록과 정확히 일치하는지 확인하세요. 조직 프로필을 업데이트하는 방법에 대한 자세한 내용은 [조직 프로필 확인](../update-your-partner-profile.md#update-your-legal-business-profile)을 참조하세요.

### <a name="next-steps"></a>다음 단계

적절한 팀이 프로세스를 검토하고 업데이트할 수 있도록 조직 내에서 이 정보를 공유하세요.

### <a name="questions"></a>궁금한 점이 더 있나요?

추가 질문은 관련 CSP Yammer 커뮤니티를 확인하세요.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a>CSP(클라우드 솔루션 공급자) 프로그램 진화 및 오픈 라이선스 프로그램 변경 사항에 대한 업데이트

### <a name="categories"></a>범주

- 날짜: 2021-03-15
- 기능

### <a name="summary"></a>요약

새로운 상용 및 공공 부문 영구 소프트웨어 제품이 오픈 라이선스 프로그램의 변경 사항과 함께 CSP(클라우드 솔루션 공급자) 프로그램에 제공됩니다.

### <a name="impacted-audience"></a>영향을 받는 대상

오픈 라이선스 프로그램뿐만 아니라 모든 CSP 파트너 거래 영구 소프트웨어를 통해 판매되는 상업적 배포자 및 관리 재판매인

### <a name="details"></a>세부 정보

2020년 9월 Microsoft는 파트너를 위한 온-프레미스 소프트웨어의 가용성을 포함하여 CSP 프로그램의 파트너에 대한 기회를 확장하는 디지털 변환 과정에서 일련의 단계를 [발표](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)했습니다. 이러한 변화를 통해 파트너는 CSP의 소프트웨어 라이선스를 활용하여 비즈니스를 성장시키고 범위를 확장하여 오늘날의 클라우드 우선 세계에서 성공을 거둘 수 있습니다. 또한 고객의 클라우드 전환을 지원하고 파트너에게 고객 하이브리드 클라우드 환경에 필요한 유연성을 제공합니다.

이와 같은 디지털 전환 과정을 계속 진행하면서 다음과 같은 변경 사항을 발표합니다.

- 2021년 7월 1일: 오픈 라이선스 프로그램 가격표에 새 SKU, 제품 또는 프로모션이 추가되지 않습니다.

- 2021년 7월 7일: 두 개의 상용 제품인 Get Genuine Windows 및 Visual Studio Professional과 공공 부문 제품(정부, 교육 및 비영리 – [공지](./2020-december.md#9) 참조)이 CSP 영구 소프트웨어 가격표에 추가됩니다.  가격표는 파트너 센터의 [판매 > 가격 및 제안](https://partnercenter.microsoft.com/pcv/sales) 페이지에 있는 소프트웨어 섹션에서 찾을 수 있으며 이 날짜에 다시 게시됩니다.

CSP 프로그램 발전 및 Open License 프로그램 변경에 대한 자세한 내용은 아래 **다음 단계** 를 참조하세요.

### <a name="next-steps"></a>다음 단계:

- CSP 프로그램 진화: [클라우드 솔루션 공급자 프로그램의 영구 소프트웨어](https://partner.microsoft.com/resources/collection/software-in-csp#/) 준비 자료를 검토하세요. 이 [준비 맵](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)을 사용하여 역할에 필요한 정보를 신속하게 찾을 수 있습니다.

- 오픈 라이선스 프로그램 변경: [CSP 프로그램 진화 및 오픈 라이선스 프로그램 변경](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) 준비 자료를 검토하세요. 이 [준비 맵](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)을 사용하여 역할에 필요한 정보를 신속하게 찾을 수 있습니다.

### <a name="questions"></a>질문

추가 질문은 관련 CSP Yammer 커뮤니티를 확인하세요.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>이전 공지에 대한 업데이트: Compliance Manager의 추가 기능인 프리미엄 평가

### <a name="categories"></a>범주

- 날짜: 2021-03-15
- 비즈니스 성장

### <a name="summary"></a>요약

평가판 제품은 가격표에 나열되지 않으며 제거됩니다.

### <a name="impacted-audience"></a>영향을 받는 대상

클라우드 솔루션 공급자를 통해 거래하는 모든 파트너

### <a name="details"></a>세부 정보

평가판 제품은 가격표에 포함되지 않았어야 했습니다. 이들 제품은 2021년 5월 1일 가격표에서 제거됩니다.

원래 공지는 [여기](./2021-february.md#4)에 있습니다.

### <a name="additional-resources"></a>추가 자료

- [Microsoft 365 E5 보안 및 규정 준수](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Microsoft Compliance Manager에서 평가 빌드 및 관리 - Microsoft 365 Compliance](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>다음 단계

이 항목에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관련자와 공유합니다.

### <a name="questions"></a>궁금한 점이 더 있나요?

이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a>OCP(One Commercial Partner) GTM(Go-to Market)에서 Microsoft 상업용 Marketplace로 솔루션 마이그레이션

### <a name="categories"></a>범주

- 날짜: 2021-03-12
- 기능

### <a name="summary"></a>요약

2021년 3월 29일부터 OCP(One Commercial Partner) GTM(Go-to Market) 기능을 제한하는 것으로 시작합니다. 파트너 센터에서 상업용 Marketplace로 솔루션을 마이그레이션하는 것이 좋습니다.

### <a name="impacted-audience"></a>영향을 받는 대상

OCP GTM에서 솔루션과 공동 판매하는 조직

### <a name="details"></a>세부 정보

2020년 12월에 Microsoft OCP GTM 도구에서 파트너 센터의 Microsoft 상업 시장으로 이동하기 시작했습니다. 이러한 전환은 수백만 고객에게 솔루션을 선보이고 다른 Microsoft 및 파트너 판매자와 양방향으로 기회를 공유하며 혁신적인 솔루션을 공동 판매할 수 있는 상용 시장의 기능을 확장합니다.

전환의 다음 마일스톤은 2021년 3월 29일에 진행됩니다. 이때 일부 필드가 읽기 전용으로 되는 제한된 OCP GTM 기능을 경험하게 됩니다. 현재 OCP GTM의 솔루션과 공동 판매 중인 경우 솔루션을 상용 시장으로 마이그레이션하여 기능을 활용하고 게시 환경을 단순화하는 것이 좋습니다. 

상업용 Marketplace로 전환하면 파트너 센터가 공동 판매 게시 환경의 주 대상이 됩니다. Microsoft 제품에 사용되는 것과 동일한 채널 및 제품 내 환경을 통해 솔루션을 공유 고객과 연결하여 비즈니스를 계속 성장시킬 수 있습니다. [상업용 Marketplace에 대해 자세히 알아보세요](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>다음 단계

- 솔루션을 아직 이동하지 않은 경우 [전환 가이드](/azure/marketplace/co-sell-solution-migration)에 설명된 지침을 따르거나 [단계별 비디오 자습서](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)를 참조하여 모든 마이그레이션 작업을 완료하고 상업용 Marketplace에 솔루션을 게시하기 시작합니다.

- OCP GTM의 제한된 기능 환경과 관련된 질문은 [Microsoft 상업용 Marketplace FAQ에서 게시하기 위한 공동 판매 요구 사항](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)을 참조하세요. ("2021년 3월 29일부터 시작되는 OCP GTM 제한된 기능" 섹션을 참조하세요.)

### <a name="questions"></a>궁금한 점이 더 있나요?

궁금한 사항이 있거나 추가 정보가 필요한 경우 [지원 팀](https://partner.microsoft.com/support/?stage=1)에게 문의하세요.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Azure용 CSP(클라우드 솔루션 공급자) 프로그램의 새로운 상거래 경험을 러시아로 확장

### <a name="categories"></a>범주

- 날짜: 2021-03-10
- 기능

### <a name="impacted-audience"></a>영향을 받는 대상

CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 러시아의 모든 파트너.

### <a name="details"></a>세부 정보

2021년 3월 10일부터 **러시아 Azure용 CSP의 새로운 상거래 환경** 을 사용할 수 있게 되어 기쁘게 생각합니다. 이 경험은 고객이 Azure 서비스를 구매하고 사용하는 방식을 간소화하고 개선합니다. 또한 CSP 프로그램의 파트너에게 판매 활동 전반에 걸친 Azure 가격 책정, 글로벌 일관성을 위한 USD 가격 책정, 청구 날짜 조정 및 Azure Cost Management에 대한 액세스를 일관된 보기로 제공합니다.

### <a name="next-steps"></a>다음 단계

새로운 Azure 상거래 경험을 소개하고 추가 정보를 제공할 수 있는 몇 가지 리소스가 있습니다. [CSP 프로그램 업데이트 리소스 갤러리](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)에서 최신 FAQ, 데크, 비디오 등을 찾아보세요.

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>파트너 센터 소프트웨어 라이선스 키 및 다운로드 이행

### <a name="categories"></a>범주

- 날짜: 2021-03-04
- 기능

### <a name="summary"></a>요약

파트너 센터 소프트웨어 다운로드 및 라이선스 키 이행 기능이 복구되었습니다.

### <a name="impacted-audience"></a>영향을 받는 대상

파트너 센터를 통해 정품 및 서버 구독 소프트웨어 주문을 거래하는 모든 CSP(클라우드 솔루션 공급자) 파트너

### <a name="details"></a>세부 정보

파트너의 피드백에 따라 파트너 센터에서 영구적인 서버 구독 소프트웨어 주문의 소프트웨어 및 라이선스 키를 얻을 수 있도록 파트너 센터 이행 기능을 복원 중입니다. 이 기능은 2021년 1월 19일에 제거되기 이전 상태로 복원됩니다. ([공지](2020-september.md#17)를 참조하세요.)

소프트웨어 라이선스 키와 다운로드 링크는 매우 소중하고 인기가 많은 지적 자산입니다. 유출될 경우 활성화 제한이 빠르게 삭제되어 고객 및 파트너 환경에 부정적인 영향을 미칠 수 있습니다.

### <a name="next-steps"></a>다음 단계

소프트웨어 키 사용 및 배포에 대한 다음 리소스와 중요 지침을 검토하세요.

- [CSP 프로그램을 통해 온-프레미스 소프트웨어 판매](../csp-on-premise-software.md)
- [파트너 센터 새 상거래 운영 가이드](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)(**소프트웨어 키 배포에 대한 지침** 섹션 참조)

### <a name="questions"></a>궁금한 점이 더 있나요?

이 공지에 대한 추가 질문은 관련 Yammer 커뮤니티를 확인하세요.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3">PSC(Partner Sales Connect)에서 파트너 센터로 거래 마이그레이션</a>

### <a name="categories"></a>범주

- 날짜: 2021-03-04
- 기능

### <a name="summary"></a>요약

2021년 3월 31일부터 PSC(Partner Sales Connect)가 읽기 전용 액세스로 전환되므로 PSC의 거래를 파트너 센터로 마이그레이션하는 것이 좋습니다.

### <a name="impacted-audience"></a>영향을 받는 대상

PSC에서 거래하는 파트너

### <a name="details"></a>세부 정보

동반 성장이라는 약속을 지키기 위한 방편 중 하나인 **Microsoft와 공동 판매** 는 파트너가 **검색되고, 전문 지식을 제공하고, 고객 범위를 확장** 하여 긍정적인 고객 결과를 얻을 수 있는 경로입니다. 평균 거래 속도가 일반 판매보다 **3.5배 빠르기 때문에** 파트너 센터에서 공동 판매 환경을 관리하면 직접 고객, 파트너 및 Microsoft 판매자 채널을 통해 판매하고 전체 추천 파이프라인을 한 곳에서 관리할 수 있습니다.

**2021년 3월 31일** 부터 **PSC** 가 **읽기 전용 액세스** 로 전환되므로 파트너 센터로 이동하여 개선된 기능을 사용하는 것이 좋습니다. 

- 필요한 지원의 종류에 따라 Microsoft와 공유하는 거래를 적절한 판매자에게 **보다 정확하게 라우팅** 합니다.
- 인센티브 대상 솔루션을 결정하고 ISV Connect 프로그램 조건을 충족하기 위한 **거래 자격 사전 평가** 를 도입했으며, 승인 프로세스 및 POE(최종 실행 증명서) 입증이 간소화될 것입니다.
- 공동 판매 기회와 영업부에서 확인한 잠재 고객을 모두 한 곳에서 관리하는 **원활한 사용자 환경** 을 제공합니다.

또한 최근에는 파트너의 전환을 도와주기 위해 파트너 센터에 새로운 기능을 추가했습니다.

- [공동 판매 기회를 대량으로 작업](../bulk-operations.md)
- [거래 마이그레이션 기능](../psc-to-pc.md)(**PSC 거래 마이그레이션** 섹션 참조)

파트너 센터에서 공동 판매 환경을 사용하면 영업 팀은 잠재 고객 및 기회를 창출하고, 거래를 완료하고, 지속적인 고객 관계를 만드는 데 더 많은 시간을 투자할 수 있습니다.

### <a name="next-steps"></a>다음 단계

파트너 센터 [전환 가이드](../psc-to-pc.md)를 사용하여 PSC의 거래를 파트너 센터로 마이그레이션하는 단계를 알아보세요.

### <a name="questions"></a>궁금한 점이 더 있나요?

추가 질문은 [고객 지원](https://partner.microsoft.com/support/?stage=1)으로 문의하세요.

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>2021년 4월 1일에 사용 가능한 새로운 Microsoft Dynamics 365 제품 및 제안

### <a name="categories"></a>범주

- 날짜: 2021-03-04
- 기능

### <a name="summary"></a>요약

2021년 4월 1일에 Microsoft는 CSP(클라우드 솔루션 공급자) 프로그램에 대한 여러 가지 신제품을 출시할 예정입니다.

### <a name="impacted-audience"></a>영향을 받는 대상

CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 모든 파트너

### <a name="details"></a>세부 정보

2021년 4월 1일에 Microsoft는 다음과 같은 신제품을 출시할 예정입니다.

- Power BI Premium Per User
- Customer Voice and Marketing USL 지역 및 세그먼트 확장

**Power BI Premium Per User**

Microsoft 최초의 사용자 단위 Power BI Premium 제품이 곧 출시됩니다. Power BI Premium은 현재 용량 구성으로만 판매됩니다. Power BI Premium Per User는 엔터프라이즈 BI(비즈니스 인텔리전스) 및 분석 기능에 대한 액세스를 제공합니다. 유연한 개별 사용자 단위 라이선스는 중소기업에 적합합니다.

이 제품에 대한 자세한 내용은 [Power BI 릴리스 정보](/power-platform-release-plan/2020wave2/power-bi/planned-features)를 검토하세요.


**솔루션 세부 정보**

제품 이름은 가격표 미리 보기와 약간 다릅니다.

| Offer name | 제품 ID |
| ------ |----------- |
| Power BI Premium Per User | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Per User for Faculty | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Per User for Students | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Per User(비영리 직원 가격) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Per User Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Per User Add-On for Faculty | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Per User Add-On for Students | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Per User Add-On(비영리 직원 가격) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Customer Voice and Marketing USL 지역 및 세그먼트 확장**

2020년 12월 출시의 후속 작업으로 Dynamics 365 Customer Voice and Marketing USL 제품이 새로운 국가와 비영리 및 교육 SKU를 추가하도록 변경되었습니다.

| Offer name | 제품 ID |
| ------ |----------- |
| Dynamics 365 Customer Voice USL(비영리 직원 가격) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL for Faculty | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

이 제품에 대해 자세히 알아보려면 다음 페이지를 방문하세요.

- [Dynamics 365 Customer Service Voice 홈 페이지](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 Marketing 홈 페이지](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>다음 단계

이 토픽에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관계자와 공유합니다.  

### <a name="questions"></a>궁금한 점이 더 있나요?

이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a>현재 일부 제품군에서 Microsoft 유니버설 인쇄 사용 가능

### <a name="categories"></a>범주

- 날짜: 2021-03-03
- 기능

### <a name="summary"></a>요약

Microsoft 유니버설 인쇄는 2021년 3월 1일부터 일부 Microsoft 365 제품군 내에서 독립 실행형 추가 기능으로 거래에 사용할 수 있습니다.

### <a name="impacted-audience"></a>영향을 받는 대상

CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 모든 파트너

### <a name="details"></a>세부 정보

[유니버설 인쇄](https://aka.ms/universalprint)는 Windows 디바이스에서 Azure에 등록된 프린터로 인쇄할 수 있게 해주는 Microsoft 365 인쇄 서비스이며, 온-프레미스 인쇄 서버가 필요 없습니다. 2021년 3월 1일부터 거래에 사용할 수 있습니다.

작업자는 드라이버 없는 인쇄, 간소화된 위치 기반 프린터 검색, 오랜 학습 기간이 필요 없는 직관적인 인쇄 환경이라는 장점을 누릴 수 있습니다. Azure AD(Azure Active Directory)에 조인된 디바이스는 기존 Azure AD 자격 증명을 사용하여 안전하게 인쇄합니다. 관리자는 Azure Portal에서 인쇄를 관리하며, 유니버설 인쇄가 기본 지원되므로 프린터를 쉽게 연결할 수 있습니다. 유니버설 인쇄는 유니버설 인쇄 커넥터 소프트웨어를 사용하여 호환되지 않는 프린터와 함께 배포할 수 있습니다.

유니버설 인쇄는 출시 시 Windows E3, A3, E5, A5 및 Microsoft 365 BP, F3, E3, A3, E5, A5에 백필됩니다.  

**솔루션 세부 정보**

제품 이름은 가격표 미리 보기와 약간 다릅니다.

| Offer name | 제품 ID | 소재 ID |
| ------ |----------- |----------- |  
| 유니버설 인쇄 볼륨 추가(작업 500개) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| 교직원용 유니버설 인쇄 볼륨 추가(작업 500개) - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| 유니버설 인쇄 볼륨 추가(작업 500개) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| 교직원용 유니버설 인쇄 볼륨 추가(작업 500개) - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>다음 단계

가격표와 [유니버설 인쇄 개요](/universal-print/fundamentals/universal-print-whatis)를 숙지하세요. 이 정보를 조직 내의 모든 해당 담당자와 공유하세요.

### <a name="questions"></a>질문이 있으세요?

이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.
