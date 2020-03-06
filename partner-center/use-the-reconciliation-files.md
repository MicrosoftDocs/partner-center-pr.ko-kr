---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 11/21/2019
description: 조정 파일을 사용 하 여 파트너 센터 요금에 대 한 자세한 라인 항목 보기를 이해 합니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340221"
---
# <a name="use-your-reconciliation-files"></a>조정 파일 사용

적용 대상:

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 위해 파트너 센터에서 조정 파일을 다운로드할 수 있습니다. 품목 세부 정보에는 각 고객의 구독에 대 한 요금 및 자세한 이벤트 (예: 구독에 대 한 좌석 추가)가 포함 됩니다.

적절 한 역할:

- 청구 관리자
- 전역 관리자

**청구서**를 읽는 방법에 대 한 자세한 내용은 [청구서 읽기](read-your-bill.md)를 참조 하세요.

## <a name="understand-reconciliation-file-fields"></a>조정 파일 필드 이해

- [라이선스 기반 조정 파일 필드](license-based-recon-files.md)
- [사용 빈도 기반 조정 파일 필드](usage-based-recon-files.md)
- [일회성 및 되풀이 조정 파일 필드](one-time-recurring-recon-files.md)
- [매일 등급 사용 조정 파일 필드](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>조정 파일의 요금 유형 이해

조정 파일 ( **Chargetype** 열)의 요금 유형을 이해 하려면 [조정 파일 요금 유형](recon-file-charge-types.md)을 참조 하세요.

## <a name="fix-formatting-issues"></a>서식 지정 문제 해결

경우에 따라 조정 파일에 서식 문제가 있을 수 있습니다. 예를 들어 en-us 로캘이 사용 되지 않는 경우이 문제가 발생할 수 있습니다.

조정 파일에서 서식 지정 문제를 해결 하려면 다음 단계를 수행 합니다.

1. Microsoft Excel에서 조정 파일 (.csv 형식)을 엽니다.
2. 파일의 첫 번째 열을 선택 합니다.
3. **텍스트를 열로 변환 마법사**를 엽니다. 리본 메뉴에서 **데이터**를 선택 **하 고 열 텍스트를**선택 합니다.
4. 마법사에서 **구분 기호로 분리 된 파일 형식**을 선택 합니다. 그런 후 **다음**을 선택 합니다.
5. **구분 기호** 필드에서 **쉼표**를 선택 합니다. **탭** 이 이미 선택 되어 있으면이 옵션을 선택 된 상태로 둘 수 있습니다. 그런 후 **다음**을 선택 합니다.
6. **열 데이터 형식** 필드에서 **날짜: MDY**를 선택 합니다. 그런 후 **다음**을 선택 합니다.
7. **열 데이터 형식** 필드에서 모든 금액 열에 대해 **텍스트** 를 선택 합니다. 그런 다음 **마침**을 선택 합니다.

## <a name="download-reconciliation-files-programmatically"></a>프로그래밍 방식으로 조정 파일 다운로드

조정 파일은 매우 클 수 있으며 다운로드 하기 어려울 수도 있습니다. 프로그래밍 방식으로 조정 파일을 다운로드 하려면 [청구서 품목 가져오기 항목](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)을 참조 하세요.

## <a name="map-taxes-or-vat"></a>세금 또는 VAT 지도

청구서에 세금 또는 부가 액 (VAT)을 매핑하려면 다음을 수행 합니다.

- 라이선스 기반 파일에서 **세금** 열 합계를 계산 합니다.
- 사용량 기반 파일에서 **taxationitem.taxamount** 열의 합계를 계산 합니다.

## <a name="itemize-reconciliation-files-by-partner"></a>파트너 별로 조정 파일 정리

**간접 모델** 의 파트너는 라이선스 기반 조정 파일의 이러한 추가 필드를 사용 하 여 재판매인의 파일을 정리 합니다.

| MPN ID | 설명 |
| ------ | ----------- |
| MPN ID | CSP (클라우드 솔루션 공급자) 파트너 (직접 또는 간접)의 Microsoft 파트너 네트워크 (MPN) 식별자입니다. |
| [대리점 MPN ID](#reseller-mpn-id) | [구독에 대 한 레코드 대리점의 MPN 식별자](#reseller-mpn-id)입니다. 이 필드는 파트너 센터의 특정 구독에 대해 나열 된 재판매인 ID에 해당 합니다. 간접 모델의 파트너를 위한 조정 파일에만 나타납니다. |

### <a name="reseller-mpn-id"></a>재판매인 MPN ID

CSP 파트너가 직접 구독을 고객에 게 판매 하는 경우 **MPN id** 는 **MPN ID** 와 **재판매인 MPN id**로 두 번 나열 됩니다.

CSP 파트너에 **MPN ID**가 없는 재판매인이 있는 경우이 값은 파트너의 **MPN id** 로 대신 설정 됩니다.

CSP 파트너가 **재판매인 MPN ID**를 제거 하는 경우이 값은 *-1*로 설정 됩니다.

**재판매인 MPN ID**를 보거나 업데이트 하려면:

1. 파트너 센터에 로그인합니다.
2. 파트너 센터 메뉴에서 **고객**을 선택합니다.
3. 목록에서 고객을 선택합니다.
4. 고객 메뉴에서 **구독**을 선택 합니다.
5. 목록에서 구독을 선택 합니다.
6. **업데이트**를 선택하여 **재판매인(MPN ID)** 을 변경합니다.
