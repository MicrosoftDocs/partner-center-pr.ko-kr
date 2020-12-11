---
title: 2020년 12월 공지
description: 새로운 기능, 프로모션, 제품, 시장 또는 기존 제품의 변경 사항 등 Microsoft 파트너 센터에 대한 2020년 12월 공지입니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 12/02/2020
ms.openlocfilehash: 1341e60fd9914f421fd59335a8f037f3d915b72f
ms.sourcegitcommit: bc44a6e0c5ef048cda6e882fdb543c13c5b64912
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "96869302"
---
# <a name="december-2020-announcements"></a>2020년 12월 공지

이 페이지에서는 2020년 11월 Microsoft 파트너 센터에 대한 공지를 자세히 설명합니다.

2020년 공지: [4월](2020-april.md) | [5월](2020-may.md) | [6월](2020-june.md) | [7월](2020-july.md) | [8월](2020-august.md) | [9월](2020-september.md) | [10월](2020-October.md) | [11월](2020-november.md) | 12월

______________

## <a name="sdk-release-on-net-standard-v1163"></a><a name="4"></a>.NET Standard(v1.16.3)의 SDK 릴리스

### <a name="categories"></a>범주

- 날짜: 2020-12-8
- 기능

### <a name="impacted-audience"></a>영향을 받는 대상

파트너 센터 .NET SDK를 사용하는 CSP 프로그램에 참여하는 Direct Bill 파트너 및 간접 공급자

### <a name="details"></a>세부 정보

2020년 12월 8일부터 파트너는 업데이트된 퍼블릭 파트너 센터 SDK [GitHub 샘플](https://github.com/Microsoft/Partner-Center-DotNet-Samples)과 함께 [MicrosoftPartnerCenter.NETSDK(NuGet 갤러리 | Microsoft.Store.PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3)를 다운로드할 수 있습니다. 이 버전에서는 다음과 같은 기능이 업데이트됩니다.
 
**SelfServePolicies - 새 기능 추가**

- [GetSelfServePolicies](/partner-center/develop/get-a-self-serve-policy-by-id.md)
- [GetListOfSelfServicePolicies](/partner-center/develop/get-a-list-of-self-serve-policies.md)
- [CreateSelfServePolicies](/partner-center/develop/create-a-self-serve-policy.md)
- [UpdateSelfServePolicies](/partner-center/develop/update-a-self-serve-policy.md)
- [DeleteSelfServePolicies](/partner-center/develop/delete-a-self-serve-policy.md)
 
**고객 회사 프로필**

- [OrganizationRegistrationNumber](/partner-center/develop/create-a-customer.md) 추가
 
**CustomerBillingProfile.DefaultAddress**

- MiddleName 추가
 
### <a name="next-steps"></a>다음 단계

- 최신 버전의 [MicrosoftPartnerCenter.NETSDK(NuGet 갤러리 | Microsoft.Store.PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3) 다운로드
- [GitHub 샘플](https://github.com/Microsoft/Partner-Center-DotNet-Samples) 다운로드 및 검토

______________

## <a name="december-2020-license-based-price-list-release-notes"></a><a name="3"></a>2020년 12월 라이선스 기반 가격표 릴리스 정보

### <a name="categories"></a>범주

- 날짜: 2020-12-8
- 제품/시장

### <a name="summary"></a>요약 

2020년 12월 라이선스 기반 가격표 및 제품표에 몇 가지 문제가 있습니다.

### <a name="impacted-audience"></a>영향을 받는 대상 

CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 모든 파트너

### <a name="details"></a>세부 정보

12월 라이선스 기반 가격표 및 제품표에 몇 가지 오류가 있습니다. 이러한 문제는 라이선스 기반 가격 책정 파일에만 관련되어 있으며 2021년 1월 업데이트에서 수정될 예정입니다.

#### <a name="incorrect-offers-in-the-license-based-price-list"></a>라이선스 기반 가격표의 잘못된 제품 정보

12월 라이선스 기반 가격표에 포함된 아래 제품은 가격표에 포함되면 안 되는 제품입니다. 이러한 제품은 이전에 가격표에 잘못 포함되었으며 게시되지 않았어야 하는 제품입니다. 현재 이러한 제품의 출시 일정이 전혀 잡혀 있지 않습니다. 나중에 다시 추가되면 향후 미리 보기 가격표에 추가 제품으로 나열될 것입니다.

   |**제품 이름**|**제품 ID**|
   |-------------------|:------|
   |Dynamics 365 Human Resources(비영리 가격)|1596fa61-7da1-4263-98f8-b27dfa4cfbb5|
   |Dynamics 365 Human Resources Attach to Qualifying Dynamics 365 Base Offer(비영리 가격)|8bf0b826-e05b-45aa-9cd1-9a9f742f7731|
   |Dynamics 365 Human Resources Attach to Qualifying Dynamics 365 Base Offer(비영리 가격)(적격 제품)|f906435d-9dc9-42ba-bea6-2a2b08ca60db|
   |Dynamics 365 Human Resources Sandbox(비영리 가격)|079ec5ba-d726-4384-95af-62d135c210d2|
   |Dynamics 365 Human Resources Self Service(비영리 가격)|931acecc-34c3-4f83-913e-c7fdbfd7e2a1|
   |Dynamics 365 Operations – Order Lines(비영리 가격)|7dd6b78a-3d53-47f8-8a64-bd84609a9a70|
   
#### <a name="incorrect-offers-in-the-offer-list-matrix"></a>제품표의 잘못된 제품 정보
   
아래는 제품표에 잘못 포함된 제품입니다. 현재 사용할 수 없으며, 출시 목표 날짜도 없습니다. 파트너는 이러한 제품을 무시해야 합니다.

   |**제품 이름**|**제품 ID**|
   |-------------------|:------|
   |Dynamics 365 Operations - Database Capacity(비영리 가격)|1d3f4d81-89b9-419e-a880-31b2c50b8d66|
   |Dynamics 365 Operations - File Capacity(비영리 가격)|dc173a86-285b-444c-881e-3ece531f67da|

#### <a name="powerapps-offer"></a>Powerapp 제품

이 제품은 제품표에는 포함되어 있지만 12월 가격표에는 없습니다. 현재 이 제품을 사용할 수 있으며 가격은 전월의 가격표 11월 파일에서 찾을 수 있습니다. 이 제품은 1월 가격표에 다시 추가될 예정입니다.

   |**제품 이름**|**제품 ID**|
   |-------------------|:------|
   |앱 플랜별 Power Apps|5e1087b6-246b-4503-b88a-b60bdf0b3840|

### <a name="next-steps"></a>다음 단계

다른 문제가 발견되면 이 공지에 추가되므로 릴리스 정보를 자주 확인하세요.

### <a name="last-updated"></a>마지막으로 업데이트한 날짜

2020년 12월 8일

______________

## <a name="an-update-of-the-us-microsoft-365-business-voice-with-calling-plan-offer-is-coming-soon"></a><a name="2"></a>통화 플랜이 포함된 미국 Microsoft 365 Business Voice 제품 업데이트가 곧 출시될 예정입니다.

### <a name="categories"></a>범주

- 날짜: 2020-12-3
- 제품/시장

### <a name="summary"></a>요약 

2021년 1월 1일부터 Microsoft는 미국 파트너 및 고객을 새로운 통화 플랜이 포함된 Microsoft 365 Business Voice로 전환할 예정입니다. 파트너는 아무 것도 할 필요가 없습니다.

### <a name="impacted-audience"></a>영향을 받는 대상 

CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 모든 파트너

### <a name="details"></a>세부 정보

Microsoft는 통신 제품에 대한 내부 요구 사항을 지원하기 위해 미국에서 판매되는 기존의 통화 플랜이 포함된 Business Voice를 새 제품으로 대체할 예정입니다. 새 제품의 기능과 가격은 기존과 동일합니다. 제품 변경은 Microsoft 내부에 적용되며 CSP 파트너가 통화 플랜이 포함된 Business Voice 제품을 마케팅, 판매 또는 지원하는 방식에 영향을 주지 않습니다. 변경 내용은 이 제품에만 적용됩니다.

신규 판매의 경우 2021년 1월 1일부터 새 제품을 사용하게 됩니다. 가격표의 이전 제품은 새 제품으로 대체됩니다.

기존 고객은 갱신 날짜에 자동으로 새 제품으로 전환됩니다. 파트너와 갱신 고객은 아무 것도 할 필요가 없습니다.


**새 제품 정보
 
   |**제품 이름**|**제품 ID**|**소재 ID**|
   |-------------------|:------|:------|
   |Microsoft 365 Business Voice(미국)|86713ec1-ad33-42cf-a1ce-8397d4d875fe|PZW-00023|
   
**기존 제품 정보

   |**제품 이름**|**제품 ID**|**소재 ID**|
   |-------------------|:------|:------|
   |Microsoft 365 Business Voice(미국)|9f9f2c7b-c961-402b-9421-8e3c9207eeb3|PZW-00009|

### <a name="next-steps"></a>다음 단계

가격표를 숙지하고 이 정보를 조직 내의 모든 해당 담당자와 공유하세요.

______________

## <a name="now-live-partner-center-api-updates-and-user-interface-enhancements-for-the-education-customer-validation-process"></a><a name="1"></a>지금 라이브: 교육 고객 유효성 검사 프로세스에 대한 파트너 센터 API 업데이트 및 사용자 인터페이스 향상

### <a name="categories"></a>범주

- 날짜: 2020-12-3
- 기능

### <a name="impacted-audience"></a>영향을 받는 대상 

클라우드 솔루션 공급자 프로그램을 통해 교육 기관 제품을 판매하는 파트너

### <a name="summary"></a>요약 

Microsoft는 신뢰할 수 있는 방식으로 운영되며, 규정을 준수하고 안전하며 보안이 유지되는 고객 유효성 검사 방법을 제공하여 클라우드 솔루션 공급자 프로그램에서 교육 기관 제품을 거래할 수 있도록 최선을 다하고 있습니다. 이러한 노력의 일환으로, 고객 심사 프로세스에 대한 명확성과 가시성을 높이고, 더 정확한 데이터를 입력하여 향상된 고객 심사 성공을 촉진할 수 있는 파트너 센터 API 및 사용자 인터페이스의 향상된 기능을 도입하고 있습니다. 

**파트너 센터의 향상된 기능** 

- 새로운 GET 및 POST 자격 API - 정확한 데이터 입력을 지원하고 Microsoft의 교육 기관 고객 유효성 검사 프로세스를 향상시킵니다. 

- 향상된 사용자 인터페이스 - 정확한 데이터 입력을 지원하고 Microsoft의 교육 고객 유효성 검사 프로세스를 향상시킵니다. 

**기존 GET 및 PUT Qualification API의 사용 중단** 

기존 GET 및 PUT Qualification API는 **2021년 2월 말 이전** 에 사용이 중지됩니다. 교육 제품을 구매하려면 그 전까지 새 GET 및 POST 파트너 센터 API로 전환해야 합니다.  

테스트 

파트너는 향상된 기능을 테스트하여 성공적인 고객 유효성 검사에 필요한 API 및 데이터 입력에 대한 이해도를 높일 수 있습니다. 테스트에 참여하려는 파트너는 테스트 준비 방법, 테스트 가입 방법 및 테스트 단계 중에 해야 할 일에 대한 지침을 제공하는 [파트너 센터 교육 고객 테스트 가이드](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf)를 다운로드해야 합니다.

**도서관 및 박물관 고객** 

위의 향상된 기능 외에도 기쁜 소식이 있습니다. 도서관 및 박물관 고객을 위해 교육 기관용 수준의 가격이 책정된 제품을 제공할 것이며, 파트너가 CSP 제품을 판매할 수 있는 교육 고객의 범위가 확장될 것입니다. 

Microsoft는 적격 교육 사용자로서 모든 고객 또는 제안된 고객의 상태를 검토할 수 있는 권리를 보유하고 있습니다. 자세한 내용은 [교육 기관 적격 교육 사용자 요구 사항](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)을 참조하세요. 

### <a name="next-stepsadditional-resources"></a>다음 단계/추가 리소스

- 운영 준비 상태 리소스:  [파트너 센터 교육 고객 검증](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/) 프로세스 개선에서 새 파트너 센터 사용자 인터페이스, API 변경 내용 및 가이드를 검토합니다. 

- 조직에서 [교육 기관 적격 교육 사용자 요구 사항](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)을 잘 알고 있는지 확인합니다. 

- 이러한 변경에 대비하는 데 도움이 되도록 이 정보를 조직 내의 적절한 팀 및 재판매인과 공유합니다. 

### <a name="change-log"></a>로그 변경 

_ 2020년 8월 31일:  최초 게시 날짜 

- 2020년 9월 25일:  테스트 창 업데이트가 추가됨 

- 2020년 10월 4일: 테스트 가입 미리 알림 

- 2020년 11월 10일: 테스트 가입 미리 알림 

- 2020년 12월 3일: API 업데이트 라이브 
