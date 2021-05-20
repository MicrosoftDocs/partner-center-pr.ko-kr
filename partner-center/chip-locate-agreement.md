---
title: 데스크톱 수 및 요금 수준 찾기
ms.topic: how-to
ms.date: 02/18/2021
description: 채널 성과급 플랫폼 (칩)을 사용 하 여 규약에 대 한 데스크톱 수와 요금 정보를 찾는 방법에 대해 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148995"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>계약에 대한 데스크톱 수 및 요금 수준 찾기

**적절 한 역할**: 기본 연락처 또는 프로그램 관리자

[Explore.ms](https://www.explore.ms/) 에 로그인 하 여 규약을 검토 하거나 데스크톱 수와 요금 수준에 대 한 계약 정보를 제공 하는 파일을 다운로드할 수 있습니다.

## <a name="to-locate-the-information"></a>정보를 찾으려면

### <a name="method-1--explorems"></a>메서드 1 – Explore.ms

1. Internet Explorer에서 [explore.ms](https://www.explore.ms/) 를 엽니다. 

>[!Note]
>Google Chrome 또는 Microsoft Edge에서는이 기능을 수행할 수 없습니다.

2. 회사/학교 계정 또는 live ID로 로그인 합니다.  

3. **보고서** 필드에서 **계약** 을 선택 합니다.

4. 결과 페이지에서 **검색** 필드에 계약 번호를 입력 한 다음 **열 선택/순서** 를 선택 합니다.

5. 팝업 창의 사용 가능한 열 목록에서 **규약 데스크톱 수** 를 선택 하 고 오른쪽 화살표를 선택 하 여 열을 추가 합니다. **확인** 을 선택합니다.

6. **검색을 선택 합니다.**

7. 결과 화면에서 결과를 스크롤하여 **규약 데스크톱 수** 열을 찾습니다. 

8. 데스크톱 수를 사용 하 여 아래의 rate 테이블을 기준으로 요금 수준을 결정 합니다.  

| 요금 수준 | 데스크톱 수 |
| ------ | :-----------: |
|  A | 0 – 2399    |
|  b | 2400 – 5999    |
|  C | 6000 – 14999    |
|  D | 15,000+   |

>[!NOTE]
>엔터프라이즈 인센티브 수준은 PS(상용 및 공공 부문) 등록의 데스크톱 또는 사용자 수(둘 중 더 높음)를 기반으로 합니다. 자연스럽게 연결된 데스크톱 또는 사용자 수가 없는 등록의 경우 Microsoft는 함께 제공되는 EA의 데스크톱 수 또는 사용자 수에 따라 데스크톱 수를 적용합니다. <br><br>함께 제공되는 EA가 없는 경우 요금 수준은 등록의 가격 책정 수준을 기반으로 합니다. www.explore.ms 거래 가격 책정 수준을 볼 수도 [있습니다.](https://www.explore.ms/) <br><br>기존 EA/EAS에 여러 풀 및/또는 가격 책정 수준이 있는 경우 Microsoft는 가장 높은 할당 가격 책정/풀 수준에서 인센티브 비용을 지불하며, 수준 A는 가장 낮고 수준 D는 가장 높습니다.

#### <a name="pool-and-pricing-levels"></a>풀 및 가격 책정 수준

위에서 설명한 단계를 사용하여 explore.ms 계약 번호를 검색한 후 계약 번호를 선택합니다. 이렇게 하면 계약 요약 및 제품 이 표시된 **계약** 세부 정보 **페이지로 열립니다.** 제품 섹션에는 가격 책정 수준이 포함되어 있습니다.

## <a name="method-2---chip"></a>방법 2 - CHIP

1. CHIP에 로그인하고 LSP 인센티브를 선택합니다.

2. 파트너 **결제 요약** 페이지에서 보려는 보고 월을 선택한 다음 **Excel로 내보내기** 아래의 드롭다운에서 **계산 세부 정보를** 선택합니다.

:::image type="content" source="images/chip/chiplocate.png" alt-text="프로그램 세부 정보 찾기":::

3. 내보내기가 시작되고 파일을 열거나 다른 이름으로 대상에 저장/저장할 수 있습니다.

4. 보고서가 열리면 맨 아래 왼쪽에 있는 **DetailReport-FlatFile** 탭으로 이동합니다.

:::image type="content" source="images/chip/flatfile.png" alt-text="플랫 파일 다운로드":::

이제 J열에서 찾고 있는 계약 번호를 검색할 수 있습니다. 할당된 데스크톱 수는 Agreement_DesktopCount 레이블이 지정된 R 열에서 찾을 수 있습니다. 'AI' 레이블이 계층인 열에서 이 계약의 요금 수준을 확인할 수도 있습니다.

## <a name="next-steps"></a>다음 단계

- [CHIP 액세스 문제 해결](chip-access-trouble.md)
