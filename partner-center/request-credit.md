---
title: Microsoft로부터 SLA 크레딧 요청
ms.topic: article
ms.date: 03/31/2021
description: 고객이 서비스 중단을 경험 하는 경우 Microsoft의 SLA (서비스 수준 계약) 크레딧을 요청 하는 이점, 제한 사항 및 절차를 알아보세요.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519442"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft의 SLA (서비스 수준 계약) 크레딧을 요청 하는 방법 및 시기

**적절 한 역할**: 관리 에이전트 | 전역 관리자

고객에 대해 제공 하는 서비스의 작동이 중단 되는 경우 Microsoft에서 **SLA (서비스 수준 계약) 크레딧을** 요청할 수 있습니다.

## <a name="sla-credit-calculation"></a>SLA 크레딧 계산

Microsoft의 SLA 크레딧을 영향을 받는 서비스에 따라 결정 됩니다. 예를 들어 고객에 게 Office 365 제품군이 있지만 SharePoint 중단이 발생 한 경우 SLA 크레딧을 고객의 전체 계획이 아닌 SharePoint에 대해서만 승인 됩니다.

*크레딧은 영향을 받는 서비스 및 가동 중단 기간을 기준으로 비례 배분 됩니다.* SLA 크레딧을 충족 하는 시나리오의 유형을 확인 하려면 [온라인 서비스 통합 SLA 문서](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)를 참조 하세요. 이 정보는 CSP (클라우드 솔루션 공급자) 프로그램을 통해 판매 되는 서비스에도 적용 됩니다.


## <a name="request-an-sla-credit"></a>SLA 크레딧 요청

*CSP 파트너는 인시던트가 발생 한 월 뒤에 월의 끝에 클레임 및 모든 필수 정보를 제출 해야 합니다.* 예를 들어 인시던트가 2 월 15 일에 발생 한 경우 Microsoft는 3 월 31 일까 지 클레임 및 모든 필수 정보를 받아야 합니다. 최종 고객 및 간접 대리점은 SLA 크레딧 청구를 제출할 수 없습니다. 간접 공급자 또는 직접 청구 파트너는 대신 클레임을 제출 해야 합니다.

> [!NOTE]
> 일반적으로 advise 인시던트에는 SLA 크레딧을 사용할 수 없습니다. Service Health 대시보드에 게시 된 인시던트는 테 넌 트가 영향을 받을 수 있고 Microsoft에서 게시 시 Microsoft가 보유 하 고 있는 최상의 정보를 나타낼 *수* 있음을 나타냅니다. 상태 페이지 데이터는 서비스의 일반 공급을 나타냅니다. 개별 서비스 영향, 완화 및 해결 방법은 다를 수 있습니다. 자세한 내용은 최종 인시던트 게시 및 사후 인시던트 검토를 검토할 수 있습니다. 자세한 내용은 [Microsoft 365 서비스 상태를 확인 하는 방법을](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) 참조 하세요.

### <a name="required-information"></a>필요한 정보

고객 이름, 테 넌 트 식별자, 파트너 티켓 # 및 티켓 생성 날짜/시간 스탬프가 충분 하지 않아 클레임을 처리할 수 없습니다.

[SLA 신용 요청](#submit-sla-credit-request) 을 Microsoft에 제출 하기 전에 다음 정보를 **모두** 수집 하 여 지원 티켓에 포함 해야 합니다.

- 고객 테 넌 트의 GUID입니다.
- [중단 인시던트 식별자](#outage-incident-identifier)인가요?
- 고객이 중단의 영향을 받고 SLA 크레딧을 요청 하는 증거입니다.
- CSP를 통해 구매한 영향을 받는 구독이 있나요? (*예* 또는 *아니요*)

#### <a name="evidence-that-proves-customer-impact"></a>고객의 영향을 증명 하는 증명 정보

- 가동 중지 시간의 시간 및 기간에 대 한 정보
- 영향을 받는 사용자의 수 및 위치 (해당 하는 경우)
- 발생할 때 인시던트를 해결 하려는 시도에 대 한 설명
- 영향을 요청 하는 고객의 전자 메일 및 이후 크레딧
- 서비스 영향 해결에 관한 고객 연락처의 지원 티켓 번호 및 세부 정보


#### <a name="outage-incident-identifier"></a>중단 인시던트 식별자

Microsoft 365 관리 센터의 **Service Health** 페이지에서 중단 인시던트에 대 한 식별자를 찾을 수 있습니다. **중단 인시던트 ID** 는 영향을 받는 서비스 (예: Exchange Online 중단에 대 한 *EX25194* )를 나타내는 두 문자로 된 약어 앞에 오는 숫자입니다. 다음 표에서는 일반적인 서비스 약어에 대해 설명 합니다.

| 2 자 약어 | Microsoft 서비스 |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | 비즈니스용 Skype 온라인 (이전의 Lync Online) |
| OS | Office 구독 |
| PB | Office 365용 Power BI |
| SP | SharePoint Online |
| 구 | Yammer Enterprise |
| MO | 포털 오류 |

### <a name="submit-sla-credit-request"></a>SLA 신용 요청 제출

파트너 센터 대시보드를 통해 Microsoft에 SLA 신용 요청을 제출 하려면:

1. 파트너 센터 대시보드에 로그인합니다.
2. 왼쪽 메뉴에서 **서비스 요청** 을 선택한 다음 **파트너 지원 요청** 을 선택 합니다.
3. **파트너 요청** 페이지에서 **새 요청** 을 선택 합니다.
4. **요청 시작** 페이지에서 **CSP-고객, 주문 및 구독** 섹션을 찾습니다. 이 섹션에서 **문제 유형 선택** 을 선택한 다음 **고객 서비스 크레딧 요청** 을 선택 합니다.
5. **권장 솔루션** 페이지의 **추가 도움이 필요 하세요?** 에서 **예** 를 선택 합니다.
6. **세부 정보** 페이지에서 **문제 세부 정보** 섹션을 작성 합니다. **세부 정보** 텍스트 상자에서 이전에 수집한 [필수 정보](#required-information) 를 입력 해야 합니다.
7. **제출** 을 선택 하 여 SLA 신용 요청을 보냅니다.

## <a name="next-steps"></a>다음 단계

- [고객을 대신 하 여 문제 보고](report-problems-on-behalf-of-a-customer.md)
