---
title: 조정 파일 사용
ms.topic: article
ms.date: 03/26/2021
description: 파트너 센터 조정 파일 및 지정된 청구 주기에 대한 요금의 자세한 품목 보기를 해석하는 방법에 대해 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431567"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>파트너 센터 조정 파일에서 품목을 읽는 방법 알아보기

**적절한 역할:** 청구 관리자 | 전역 관리자

청구 주기의 각 요금에 대한 자세한 품목 보기를 보려면 파트너 센터 조정 파일을 다운로드할 수 있습니다. 품목 세부 정보는 각 고객의 구독에 대한 요금 및 자세한 이벤트(예: 구독에 대한 라이선스의 중간 기간 추가)를 포함합니다.

**청구서를** 읽는 방법에 대한 자세한 내용은 [청구서 읽기를 참조하세요.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>조정 파일 필드 이해

- [라이선스 기반 조정 파일 필드](license-based-recon-files.md)
- [사용량 기반 조정 파일 필드](usage-based-recon-files.md)
- [일일 요금 지정 사용량 조정 파일 필드](daily-rated-usage-recon-files.md)
- [일회성 구매 CSP 조정 파일 필드](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>조정 파일의 요금 유형 이해

조정 파일의 요금 **유형(ChargeType** 열)을 이해하려면 [조정 파일 요금 유형을 참조하세요.](recon-file-charge-types.md)

## <a name="fix-formatting-issues"></a>서식 지정 문제 해결

경우에 따라 조정 파일에 서식 문제가 포함될 수 있습니다. 예를 들어 en-US 로케일을 사용하지 않는 경우 이 문제가 발생할 수 있습니다.

조정 파일의 서식 문제를 해결하려면 다음 단계를 수행합니다.

1. Microsoft Excel에서 조정 파일(.csv 형식)을 엽니다.
2. 파일의 첫 번째 열을 선택합니다.
3. 텍스트를 **열로 변환 마법사 를 엽니다.** 리본에서 **데이터** 를 선택한 다음, **텍스트에서 열로를** 선택합니다.
4. 마법사에서 구분 **기호로 분리된 파일 형식 을** 선택합니다. 그다음에 **다음** 을 선택합니다.
5. 구분 **기호** 필드에서 **쉼표** 를 선택합니다. **(탭이** 이미 선택된 경우 이 옵션을 선택한 상태로 둘 수 있습니다.) 그런 다음, **다음을** 선택합니다.
6. 열 **데이터 형식** 필드에서 **날짜:MDY** 를 선택합니다. 그다음에 **다음** 을 선택합니다.
7. 열 **데이터 형식** 필드에서 모든 양 열에 대해 **텍스트를** 선택합니다. **마침** 을 선택합니다.

## <a name="download-reconciliation-files-programmatically"></a>프로그래밍 방식으로 조정 파일 다운로드

조정 파일은 매우 클 수 있으며 다운로드하기 어려운 경우도 있습니다. 조정 파일을 프로그래밍 방식으로 다운로드하려면 [청구서 품목 받기를 참조하세요.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>파일이 Excel의 행 제한을 초과하는 경우

조정 파일을 다운로드할 수 있지만 Microsoft Excel에서 열 수 없는 경우 파일에 Excel에서 허용하는 것보다 더 많은 행이 포함되어 있는 것일 수 있습니다. 이 경우 아래 절차 중 하나를 사용하여 파일을 열 수 있습니다.

### <a name="open-a-recon-file-in-power-bi"></a>Power BI 정찰 파일 열기

1. 정상적으로 조정 파일을 다운로드합니다.
2. Microsoft Power BI 인스턴스를 다운로드, 설치 및 엽니다.
3. Power BI **홈** 탭에서 **데이터 받기를** 선택합니다.
4. 일반 데이터 **원본** 목록에서 **Text/CSV를** 선택합니다.
5. 메시지가 표시되면 recon 파일을 엽니다.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Excel 피벗 테이블에서 recon 파일 열기

1. 정상적으로 조정 파일을 다운로드합니다.
2. Microsoft Excel에서 새 파일을 엽니다.
3. **데이터** 탭에서 **데이터 받기를** 선택하고 **파일에서** 를 선택한 **다음, Text/CSV** 를 선택합니다.
4. 메시지가 표시되면 recon 파일을 엽니다. 데이터가 표시됩니다.
5. **로드** 드롭다운 메뉴에서 **로 로드를** 선택한 **다음, 확인을** 선택합니다.
6. 데이터 **가져오기** 대화 상자에서 **피벗 테이블 보고서를** 선택하여 파일을 엽니다.

## <a name="negative-amount-displayed"></a>음수 양 표시

조정 파일에 음수 금액이 표시되었을 수 있습니다. 이는 다음 중 하나에 의해 발생할 수 있습니다.

- 최근에 라이선스 수를 취소하거나 줄임
- SLA(서비스 사용권 계약) 또는 Azure 사용량에 대한 크레딧을 받았습니다.

이 트랜잭션에 대한 자세한 정보를 보려면 조정 파일에서 해당 청구 유형 특성을 검토합니다.

## <a name="map-taxes-or-vat"></a>세금 또는 VAT 매핑

세금 또는 VAT(부가가치세)를 청구서에 매핑하려면 다음을 수행합니다.

- 라이선스 기반 파일에서 **Tax** 열의 합계를 계산합니다.
- 사용량 기반 파일에서 **TaxAmount** 열의 합계를 계산합니다.

## <a name="itemize-reconciliation-files-by-partner"></a>파트너별 조정 파일 항목화

**간접 모델의** 파트너는 라이선스 기반 및 사용량 기반 조정 파일 모두에서 이러한 추가 필드를 사용하여 대리점별로 파일을 항목화할 수 있습니다.

| MPN ID | 설명 |
| ------ | ----------- |
| MPN ID | CSP(클라우드 솔루션 공급자) 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) 식별자입니다. |
| [Reseller MPN ID](#reseller-mpn-id) | [구독에 대한 레코드의 대리점 MPN 식별자입니다.](#reseller-mpn-id) 이 필드는 파트너 센터 특정 구독에 대해 나열된 대리점 ID에 해당합니다. 간접 모델의 파트너에 대한 조정 파일에만 표시됩니다. |

### <a name="reseller-mpn-id"></a>Reseller MPN ID

CSP 파트너가 구독을 고객에게 직접 판매한 경우 **MPN ID는 MPN ID와** Reseller **MPN ID** 둘 다로 두 번 **나열됩니다.**

CSP 파트너에 **MPN ID가** 없는 대리점이 있는 경우 이 값은 대신 파트너의 **MPN ID로** 설정됩니다.

CSP 파트너가 **Reseller MPN ID** 를 제거하는 경우 이 값은 *-1로* 설정됩니다.

**Reseller MPN ID** 를 보거나 업데이트하려면:

1. 파트너 센터에 로그인합니다.
2. 파트너 센터 메뉴에서 **고객을** 선택합니다.
3. 목록에서 고객을 선택합니다.
4. 고객 메뉴에서 **구독을 선택합니다.**
5. 목록에서 구독을 선택합니다.
6. **업데이트를** 선택하여 **Reseller(MPN ID) 를 변경합니다.**

## <a name="next-steps"></a>다음 단계

- [청구 & 재구성 파일을 읽는 방법](read-your-bill.md) 