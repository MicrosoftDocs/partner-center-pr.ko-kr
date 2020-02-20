---
title: Microsoft에서 SLA 크레딧 요청 | 파트너 센터
ms.topic: article
ms.date: 11/21/2019
description: 고객이 서비스 중단을 경험 하는 경우 Microsoft 로부터 SLA 크레딧을 요청 하기 위한 이점, 제한 사항 및 절차를 알아보세요.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: bcc094b877d0128c73041044ce6304123d895fdb
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943146"
---
# <a name="request-an-sla-credit-from-microsoft"></a>Microsoft에서 SLA 크레딧 요청 

고객에 대해 제공 하는 서비스의 작동이 중단 되는 경우 Microsoft에서 **SLA (서비스 수준 계약) 크레딧을** 요청할 수 있습니다.

## <a name="sla-credit-calculation"></a>SLA 크레딧 계산

Microsoft의 SLA 크레딧을 영향을 받는 서비스에 따라 결정 됩니다. 예를 들어 고객에 게 Office 365 제품군이 있지만 SharePoint 중단이 발생 한 경우 SLA 크레딧을 SharePoint에 대해서만 승인 되 고 고객의 전체 요금제는 승인 되지 않습니다.

*크레딧은 영향을 받는 서비스 및 가동 중단 기간을 기준으로 비례 배분 됩니다.* SLA 크레딧을 충족 하는 시나리오의 유형을 확인 하려면 [온라인 서비스 통합 SLA 문서](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)를 참조 하세요. 이 정보는 클라우드 솔루션 공급자 프로그램을 통해 판매 되는 서비스에도 적용 됩니다.

## <a name="request-an-sla-credit"></a>SLA 크레딧 요청

*CSP (클라우드 솔루션 공급자) 파트너는 인시던트가 발생 한 월 뒤에 월의 끝에 클레임 및 모든 필수 정보를 제출 해야 합니다.* 예를 들어 인시던트가 2 월 15 일에 발생 한 경우 Microsoft는 3 월 31 일까 지 클레임 및 모든 필수 정보를 받아야 합니다. 최종 고객 및 간접 대리점은 SLA 크레딧 청구를 제출할 수 없습니다. 간접 공급자 또는 직접 청구 파트너는 대신 클레임을 제출 해야 합니다.

### <a name="required-information"></a>필요한 정보

[SLA 신용 요청](#submit-sla-credit-request) 을 Microsoft에 제출 하기 전에 지원 티켓에 포함할 다음 정보를 수집 해야 합니다.

- 고객 테 넌 트의 GUID입니다.
- [중단 인시던트 식별자](#outage-incident-identifier)인가요?
- CSP를 통해 구매한 영향을 받는 구독이 있나요? (*예* 또는 *아니요*)

#### <a name="outage-incident-identifier"></a>중단 인시던트 식별자

Microsoft 365 관리 센터의 **Service Health** 페이지에서 중단 인시던트에 대 한 식별자를 찾을 수 있습니다. **중단 인시던트 ID** 는 영향을 받는 서비스 (예: Exchange Online 작동 중단에 대 한 *EX25194* )를 나타내는 두 문자로 된 약어 앞에 오는 숫자입니다. 다음 표에서는 일반적인 서비스 약어에 대해 설명 합니다.

| 2 자 약어 | Microsoft 서비스 |
| ----------------------- | ----------------- |
| 고급 | Exchange Online |
| FO | Exchange Online 보호 |
| SB | 비즈니스용 Skype Online (이전의 Lync Online) |
| OS | Office 구독 |
| PB | Office 365용 Power BI |
| SP | SharePoint Online |
| 구 | Yammer 엔터프라이즈 |
| MO | 포털 오류 |

### <a name="submit-sla-credit-request"></a>SLA 신용 요청 제출

파트너 센터 대시보드를 통해 Microsoft에 SLA 신용 요청을 제출 하려면:

1. 파트너 센터 대시보드에 로그인 합니다.
2. 왼쪽 메뉴에서 **서비스 요청**을 선택한 다음 **파트너 지원 요청**을 선택 합니다.
3. **파트너 요청** 페이지에서 **새 요청**을 선택 합니다.
4. **요청 시작** 페이지에서 **CSP-고객, 주문 및 구독**섹션을 찾습니다. 이 섹션에서 **문제 유형 선택**을 선택한 다음 **고객 서비스 크레딧 요청**을 선택 합니다.
5. **권장 솔루션** 페이지의 **추가 도움이 필요 하세요?** 에서 **예**를 선택 합니다.
6. **세부 정보** 페이지에서 **문제 세부 정보** 섹션을 작성 합니다. **세부 정보** 텍스트 상자에서 이전에 수집한 [필수 정보](#required-information) 를 입력 해야 합니다.
7. **제출** 을 선택 하 여 SLA 신용 요청을 보냅니다.
