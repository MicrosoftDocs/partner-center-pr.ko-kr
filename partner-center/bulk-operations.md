---
title: 참조에서 excel 파일을 통한 대량 작업
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Excel 파일을 사용 하 여 공동 판매 기회를 다운로드, 생성 또는 업데이트 하는 방법을 알아봅니다.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 16975e78c10aeb73bf141c1a1d0a215ac885039c
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645642"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>쉼표로 구분 된 값 (CSV) 파일을 사용 하 여 공동 판매 기회를 위한 대량 작업

**적절한 역할**

- 조회 관리자
- 추천 사용자

파트너 센터에서 대량 작업을 수행 하면 회사에서 공동 판매 기회 데이터를 내보내고 가져올 수 있습니다. 공동 판매 기회 페이지로 이동 하 여 페이지 제목 배너의 오른쪽 위에 있는 가져오기 및 내보내기 링크를 찾습니다. **조회 관리자** 및 **조회 사용자** 권한이 있는 사용자는이 기능을 사용할 수 있습니다.

> [!IMPORTANT]
> 대량 가져오기를 통해 수행 된 만들기/업데이트 작업은 되돌릴 수 없습니다. 많은 수의 레코드를 수정 하거나 만들 때 주의 하십시오. 거래를 만든 후에는 필드의 하위 집합만 수정할 수 있습니다. **거절/만료 됨/성공/손실와 같은 터미널 상태에 도달 하면 어떤 동작도 허용 되지 않습니다.**

## <a name="exporting-co-sell-opportunities"></a>공동 판매 기회 내보내기

내보내기 기능에 대 한 자세한 내용은 다음과 같습니다.

- 내보내기 단추를 클릭 하 여 **최대 5000 레코드** 를 내보낼 수 있습니다.
- 다운로드 되는 거래는 액세스 수준에 따라 달라 집니다. 조회 관리자 및 조회 사용자는 해당 범위에 따라 다른 결과를 얻을 수 있으며 거래 팀 구성원으로 포함 될 수 있습니다. [조회 권한에](permissions-overview.md#manage-referrals)대해 자세히 알아보세요.
- Export 함수는 공동 판매 기회 페이지에서 현재 탭을 고려 하 고 적용 된 필터를 사용 합니다.
- 적용 된 필터를 기반으로 하는 모든 데이터가 포함 된 CSV 파일이 생성 됩니다.
- 레코드를 다운로드 하는 데 최대 1 분 정도 걸릴 수 있습니다.
- 다운로드 작업이 완료 될 때까지 기다릴 필요가 없습니다. 파트너 센터의 다른 페이지로 이동 하더라도 내보내기 함수가 완료 되는 즉시 파일이 다운로드 됩니다.
- 다운로드 한 파일을 다시 사용 하 여 거래 정보를 수정 하 고 업로드 하 여 모든 레코드를 업데이트할 수 있습니다.

## <a name="importing-co-sell-opportunities"></a>공동 판매 기회 가져오기

- 가져오기 기능을 사용 하 여 **최대 1000 레코드** 를 만들거나 업데이트할 수 있습니다.
- 파트너 센터의 가져오기 페이지에서 템플릿을 다운로드 하 여 템플릿을 처음부터 빌드할 수 있습니다.
- 내보내기 기능을 사용 하 여 기존 레코드를 다운로드 하 고 업데이트할 수도 있습니다.
- 파일에 포함 된 레코드가 1000 개를 초과 하는 경우에는 처리할 수 없습니다.
- 파일이 처리 된 후에는 마지막 프로세스 파일 카드에 생성, 업데이트 및 처리 되지 않은 조회 수가 포함 된 요약이 표시 됩니다.
- 처리 된 레코드의 세부 정보를 다운로드 하 고, 오류를 수정 하 고, 동일한 파일을 업로드 하 여 이전 실행에서 실패 한 레코드를 만들거나 업데이트할 수 있습니다. **이전 실행에서 실패 한 수정 된 레코드를 업로드 하기 전에 파일에서 모든 성공한 레코드를 제거 합니다.**
- 솔루션을 더 추가 하려면 솔루션 1 옆에 열을 추가 하 고 열 이름을 Solution X로 사용 합니다. 여기서 X는 거래의 솔루션 번호를 나타냅니다. 예를 들어 솔루션 2, 솔루션 3입니다.
- 최대 50 개의 솔루션을 거래에 추가할 수 있습니다.
- 팀 멤버를 더 추가 하려면 팀 멤버 1 옆에 열을 추가 하 고 열 이름을 팀 멤버 X로 사용 합니다. 여기서 X는 거래의 팀 멤버 번호를 나타냅니다. 예를 들어 팀 멤버 2, 팀 멤버 3입니다.
- 거래에 최대 50 팀 멤버를 추가할 수 있습니다.

> [!NOTE]
> 처리가 완료 될 때까지 기다릴 필요가 없습니다. 처리가 완료 되 면 마지막으로 처리 된 파일에 대 한 세부 정보를 다운로드할 수 있습니다. **1000 레코드를 사용 하 여 파일을 업로드 하는 경우 최대 10 분이 걸릴 수 있습니다.**

> [!IMPORTANT]
> 파트너 센터에서 CSV 파일을 사용 하 여 거래를 만들거나 업데이트 하기 전에 모든 지침을 신중 하 게 읽고 아래 표에서 각 열의 형식을 확인 하세요.

|**열 이름**|**필수 여부**|**설명**|**샘플 값**|
|-----|:-----|:---------|:---|
오류|아니요|조회에 대 한 만들기/업데이트 작업에 관련 된 내용이이 열에 포함 되는 경우 오류가 발생 합니다. 오류가 여러 개 있는 경우 모두 세미콜론으로 구분 하 여 나열 됩니다.|필수 필드 솔루션 1 누락|
Engagement ID|아니요|Engagement ID는 Microsoft 파트너 센터 조회 시스템에 의해 생성 됩니다. 새 조회를 만들 때는 필요 하지 않습니다. 레코드를 업데이트 하는 경우 기존 engagement ID를 사용할 수 있습니다.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
추천 ID|아니요|Microsoft 파트너 센터 조회 시스템에서 조회 ID를 생성 합니다. 새 조회를 만들 때는 필요 하지 않습니다. 기존 레코드를 업데이트 하는 경우이를 조회 ID로 채웁니다.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
거래 이름|예|참조의 식별 이름입니다.|영국 스프링 거래
고객 이름|예|고객 회사의 이름입니다. Microsoft 쪽에서 신속 하 게 일치 하는 조직의 법적 이름을 사용 합니다.|Contoso Corporation
고객 주소 줄 1|예|고객 회사의 주소란 1입니다. |한 Contoso 방법
고객 주소 줄 2|아니요|고객 회사의 주소 줄 2입니다.|NE 148 번
고객 구/군/시|예|고객 조직이 있는 구/군/시입니다.|Redmond
고객 시/도|아니요|고객 조직이 있는 상태입니다.|워싱턴
고객 우편 번호|아니요|고객 조직이 있는 지역의 우편 번호입니다.|98052
고객 국가|예|고객 조직이 있는 국가/지역입니다. [여기]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)에 설명 된 대로 두 문자 국가 코드를 사용 합니다.|US
고객 D-U-N-S ID|아니요|고객 조직의 DUNS ID를 인출 해 보세요. 이렇게 하면 Microsoft 쪽에서 고객 조직과 빠르게 일치 하 여 더 빠르게 판매자를 할당 하는 데 도움이 됩니다. 이 [웹 사이트](https://www.dnb.com/duns-number/lookup.html)에서 DUNS ID를 무료로 받을 수 있습니다.|81466849
고객 연락처 이름|개체|이름은 Microsoft 도움말이 필요한 경우에만 필수입니다. 이 거래에 대해 작업 하는 고객 조직의 기본 연락처 이름입니다.|John
고객 연락처 성|개체|Last name은 Microsoft 도움말이 필요한 경우에만 필수입니다. 이 거래에 대해 작업 하는 고객 조직의 기본 연락처 이름입니다.|Customer
고객 연락처 전화 번호|개체|전화 번호는 Microsoft 도움말이 필요한 경우에만 필수입니다. 이 거래에 대해 작업 하는 고객 조직의 기본 연락처 전화 번호입니다.|9999999999
고객 연락처 전자 메일 주소|개체|전자 메일 주소는 Microsoft 도움말이 필요한 경우에만 필수입니다. 이 거래에 대해 작업 하는 고객 조직의 기본 연락처 전자 메일 주소입니다.|john.customer@contoso.com
파트너 조회 상태|예|회사 관점에서의 거래 상태를 나타냅니다. 조회를 만들거나 수정 하려는 경우에 필요 합니다. 새 거래를 만들려고 하는 경우 **new** 를 사용 합니다. 허용 되는 값은 [여기](https://docs.microsoft.com/partner/develop/referral-resources#referralstatus)에 설명 되어 있습니다.|활성
파트너 조회 하위 상태|예|정확한 거래 상태를 나타냅니다. 새 거래를 만들려고 하는 경우 **동의** 함을 사용 합니다. 기존 조회를 수정 하는 경우에도 필요 합니다. 허용 되는 값은 [여기](https://docs.microsoft.com/partner/develop/referral-resources#referralsubstatus)에 설명 되어 있습니다.|수락됨
Microsoft 조회 상태|개체|Microsoft에서 도움을 받는 공동 판매 요청의 상태를 나타냅니다. 이 필드는 읽기 전용 필드입니다. 데이터를 가져올 때이 필드에 적용 된 모든 변경 내용은 무시 됩니다.| Pending
거부 됨/손실 이유|개체| 필드의 하위 상태를 거부 됨 또는 손실로 변경 하는 경우에만이 정보를 제공 해야 합니다. 그렇지 않으면이 열을 무시할 수 있습니다. <br/> **아래 옵션에 따라 숫자를 입력 하십시오.** <br/><br/> **1**-프로젝트 예산이 적절 하지 않음  <br/> **2**-고객이 응답 하지 않음  <br/> **3**-고객이 다른 공급 업체를 선택 했습니다.  <br/> **4** -고객 요구 사항 충족 안 됨  <br/> **5** -고객이 아닙니다. <br/> **6**-제안 된 시간 줄이 너무 짧습니다. <br/> **7** -남용, 스팸 또는 피싱으로 보고 <br/> **8** -기타 |6|
판매 단계|아니요|이 필드는 조회의 세부 판매 단계를 표시 합니다. [여기](https://aka.ms/salesStages) 에서 판매 단계에 대해 자세히 알아보세요.|40
예상 거래 값|예|"고객과의 초기 대화를 기반으로 하는 거래의 가치입니다. 이는 거래가 터미널 상태 중 하나에 도달할 때까지 변경할 수 있습니다.| 성공 또는 손실 됨 "|12563
통화|예|거래 값이 입력 되는 통화입니다. [여기](https://en.wikipedia.org/wiki/ISO_4217)에서 통화 코드를 찾을 수 있습니다.|USD
예상 종료 날짜|예|MM/DD/YYYY 형식의 고객에 대 한 초기 대화를 기반으로 하는 거래의 예상 종료 날짜입니다. <br/> **날짜는 UTC 표준 시간대 여야 합니다. 파트너 센터 UI에 표시 되는 모든 날짜는 지역화 된 timezones를 기반으로 합니다. UTC 표준 시간대로 날짜를 제공한 조회를 살펴보면 파트너 센터 UI에 +/-1 일 차이가 있을 수 있습니다.**|1/30/2020
CRM ID|아니요|CRM 시스템의이 특정 조회에 대 한 식별자입니다 (있는 경우). 자유 형식 텍스트 입력 필드입니다.|34234324-sdfsdf-345345-sfd
마케팅 캠페인 ID|아니요|이 필드는이 특정 조회를 발생 시킨 마케팅 캠페인을 나타냅니다. 일반적으로 ROI 계산에 사용 됩니다.|BingSummer2020
참고|아니요|조회와 관련 된 업데이트를 나타내는 자세한 정보|샘플 노트입니다.
Microsoft 도움이 필요 하세요?|예|Microsoft에서이 공동 판매 요청을 지원 하도록 할지 여부를 지정 합니다.|예
Microsoft의 특정 도움말|개체|Microsoft에서 도울 수 있는 6 가지 방법 중 하나입니다. 이는 "Microsoft 도움말이 필요 한가요?" 라는 질문에 대해 아니요를 선택 하는 경우에만 적용 됩니다. " <br/> **아래 옵션에 따라 숫자를 입력 하십시오.** <br/><br/> **1**-워크 로드 별 가치 제안  <br/> **2**-고객 기술 아키텍처  <br/> **3**-개념 증명/데모  <br/> **4**-따옴표 및 라이선스  <br/> **5**-판매 후 고객 성공  <br/> **6**-일반 또는 기타|1|
Microsoft 영업 팀과 공유|예|이는 Microsoft 영업 팀과 거래 정보를 공유 하는지 여부를 나타내는 것입니다. 이는 "Microsoft 도움말이 필요 한가요?" 라는 질문에 대해 아니요를 선택 하는 경우에만 적용 됩니다. "|예
Microsoft에 대 한 참고 사항|아니요|Microsoft에서 도움을 받아야 하는 경우 Microsoft에 대 한 특정 참고 사항|Contoso 고객용 POC에 대 한 도움이 필요
고객/파트너 연락처 공유에 동의|예|고객 연락처 세부 정보를 공유 하 고 회사 직원에 게 거래에 대해 작업 하는 세부 정보를 공유 하는 데 동의 합니다. **이 열에 대해 아니요를 선택 하는 경우에는 거래를 만들거나 업데이트할 수 없습니다.** |예
해결 방법 1|예|솔루션 ID (필수), 통화 값을 입력 하는 통화 (옵션)입니다. [여기](https://en.wikipedia.org/wiki/ISO_4217)에서 통화 코드, sku 가격 (선택 사항) 및 sku 수량 (선택 사항)을 찾을 수 있습니다.  |SOL-1234-PQRS, USD, 10, 100
팀 멤버 1|예|각 팀 멤버의 이름, 성, 휴대폰 번호 및 전자 메일 ID를 표시 합니다.| Bob, 파트너, 999999, Bob.partner@Contoso.com