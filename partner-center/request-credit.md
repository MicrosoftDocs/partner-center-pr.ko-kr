---
title: Microsoft로부터 SLA 크레딧 요청
ms.topic: article
ms.date: 03/31/2021
description: 고객이 서비스 중단이 발생하는 경우 Microsoft에서 SLA(서비스 수준 계약) 크레딧을 요청하는 이점, 제한 사항 및 절차에 대해 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 100a3d2988c19d57f7426c7212b7464d8e96dc94
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152956"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft에서 SLA(서비스 수준 계약) 크레딧을 요청하는 방법 및 시기

**적절한 역할:** 관리 에이전트 | 전역 관리자

고객에게 제공하는 서비스가 중단된 경우 Microsoft에서 **SLA(서비스 수준 계약) 크레딧을** 요청할 수 있습니다.

## <a name="sla-credit-calculation"></a>SLA 크레딧 계산

Microsoft의 SLA 크레딧은 영향을 받은 서비스에 따라 결정됩니다. 예를 들어 고객에게 Office 365 제품군이 있지만 SharePoint 중단만 발생한 경우 SLA 크레딧은 고객의 전체 계획이 아닌 SharePoint에 대해서만 승인됩니다.

*크레딧은 영향을 받는 서비스 및 중단 기간에 따라 비례 배분됩니다.* SLA 크레딧을 받을 수 있는 시나리오 유형을 보려면 [온라인 서비스 통합 SLA 문서를 참조하세요.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) 이 정보는 클라우드 솔루션 공급자 프로그램을 통해 판매된 서비스에도 적용됩니다.


## <a name="request-an-sla-credit"></a>SLA 크레딧 요청

*CSP(클라우드 솔루션 공급자) 파트너는 인시던트 발생 월 이후 월말까지 클레임 및 모든 필수 정보를 제출해야 합니다.* 예를 들어 2월 15일에 인시던트 발생 시 Microsoft는 3월 31일까지 클레임 및 모든 필수 정보를 받아야 합니다. 최종 고객 및 간접 대리점은 SLA 크레딧 클레임을 제출할 수 없습니다. 간접 공급자 또는 직접 청구 파트너는 대신 클레임을 제출해야 합니다.

>[!NOTE]
>권고 인시던트(Microsoft 365[서비스 상태를 확인하는 방법)는](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)SLA 크레딧을 받을 수 없습니다.

### <a name="required-information"></a>필요한 정보

고객 이름, 테넌트 식별자, 파트너 티켓#및 만든 티켓 날짜/타임스탬프는 클레임을 처리하기에 충분하지 않습니다.

Microsoft에 [SLA 크레딧 요청을 제출하기](#submit-sla-credit-request) 전에 지원 티켓에 포함할 다음 정보를 **모두** 수집해야 합니다.

- 고객 테넌트의 GUID
- [중단 인시던트 식별자?](#outage-incident-identifier)
- 고객이 중단의 영향을 받고 SLA 크레딧을 요청 하는 증거입니다.
- CSP를 통해 구매한 영향을 받는 구독이 있나요? (*예* 또는 *아니요*)

#### <a name="evidence-that-proves-customer-impact"></a>고객의 영향을 증명 하는 증명 정보

- 가동 중지 시간의 시간 및 기간에 대 한 정보
- 영향을 받는 사용자의 수 및 위치 (해당 하는 경우)
- 발생할 때 인시던트를 해결 하려는 시도에 대 한 설명
- 영향을 요청 하는 고객의 전자 메일 및 이후 크레딧
- 서비스 영향 해결에 관한 고객 연락처의 지원 티켓 번호 및 세부 정보


#### <a name="outage-incident-identifier"></a>중단 인시던트 식별자

Microsoft 365 관리 센터의 **Service Health** 페이지에서 중단 인시던트에 대 한 식별자를 찾을 수 있습니다. **중단 인시던트 ID** 는 영향을 받는 서비스 (예: Exchange Online 작동 중단에 대 한 *EX25194* )를 나타내는 두 문자로 된 약어 앞에 오는 숫자입니다. 다음 표에서는 일반적인 서비스 약어에 대해 설명 합니다.

| 2 자 약어 | Microsoft 서비스 |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online 보호 |
| SB | 비즈니스용 Skype Online (이전의 Lync Online) |
| OS | Office 구독 |
| PB | Office 365용 Power BI |
| SP | SharePoint Online |
| 구 | Yammer 엔터프라이즈 |
| MO | 포털 오류 |

### <a name="submit-sla-credit-request"></a>SLA 크레딧 요청 제출

파트너 센터 대시보드를 통해 Microsoft에 SLA 크레딧 요청을 제출하려면 다음을 수행합니다.

1. 파트너 센터 대시보드에 로그인합니다.
2. 왼쪽 메뉴에서 **서비스 요청을** 선택한 다음, 파트너 **지원 요청을** 선택합니다.
3. 파트너 **요청** 페이지에서 **새 요청** 를 선택합니다.
4. 요청 **시작** 페이지에서 **CSP - 고객, 주문 및 구독 섹션을 찾습니다.** 이 **섹션에서는 문제 유형 선택을 선택한** **다음, 고객 서비스 크레딧 요청을 선택합니다.**
5. 권장 **솔루션** 페이지의 도움이 **더 필요하세요?** 아래에서 **예를** 선택합니다.
6. 세부 **정보** 페이지에서 문제 **세부 정보** 섹션을 입력합니다. 세부 **정보** 텍스트 상자에 이전에 수집한 [필수 정보를](#required-information) 입력해야 합니다.
7. **제출을** 선택하여 SLA 크레딧 요청을 보냅니다.

## <a name="next-steps"></a>다음 단계

- [고객을 대신하여 문제 보고](report-problems-on-behalf-of-a-customer.md)
