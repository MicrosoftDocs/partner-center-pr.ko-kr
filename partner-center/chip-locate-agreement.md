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
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756108"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>계약에 대한 데스크톱 수 및 요금 수준 찾기

**적절한 역할**

- 기본 연락처 또는 프로그램 관리자

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
|  D | 15000 이상   |

>[!NOTE]
>엔터프라이즈 동기 수준은 상용 및 PS (공개 섹터) 등록의 데스크톱 또는 사용자 수 (어느 쪽 이상)를 기반으로 합니다. 자연 스러운 데스크톱 또는 사용자 수가 없는 등록의 경우 Microsoft는 해당 EA의 데스크톱 수 또는 사용자 수에 따라 데스크톱 수를 적용 합니다. <br><br>해당 EA가 없는 경우 요금 수준은 등록의 가격 책정 수준을 기준으로 합니다. [Www.explore.ms](https://www.explore.ms/)에서 거래 가격 수준을 볼 수도 있습니다. <br><br>기존 EA/EAS에 여러 개의 풀 및/또는 가격 책정 수준이 있는 경우 Microsoft는 가장 높은 할당 된 가격/풀 수준에서 성과급을 지불 하 고 수준이 가장 낮은 것 이며 수준 D가 가장 높습니다.

#### <a name="pool-and-pricing-levels"></a>풀 및 가격 책정 수준

위에 설명 된 단계를 사용 하 여 explore.ms에서 계약 번호를 검색 한 후 계약 번호를 선택 합니다. 그러면 계약 **요약** 및 **제품** 을 표시 하는 계약 정보 페이지로 이동 합니다. 제품 섹션에는 가격 책정 수준이 포함 되어 있습니다.

## <a name="method-2---chip"></a>방법 2-칩

1. 칩에 로그인 하 고 LSP 성과급을 선택 합니다.

2. **파트너 지불 요약** 페이지에서 보려는 보고 월을 선택 하 고 **Excel로 내보내기** 아래의 드롭다운에서 **계산 세부 정보** 를 선택 합니다.

:::image type="content" source="images/chip/chiplocate.png" alt-text="프로그램 세부 정보 찾기":::

3. 내보내기가 시작 되 고 파일을 열거나 대상에 저장/저장할 수 있습니다.

4. 보고서가 열리면 왼쪽 아래에 있는 **DetailReport-FlatFile** 탭으로 이동 합니다.

:::image type="content" source="images/chip/flatfile.png" alt-text="플랫 파일 다운로드":::

이제 J 열에서 찾고 있는 계약 번호를 검색할 수 있습니다. 그러면 Agreement_DesktopCount 레이블이 지정 된 R 열에 할당 된 데스크톱 수가 표시 됩니다. ' AI ' 계층 이라는 열에서이 규약의 요금 수준을 확인할 수도 있습니다.

## <a name="next-steps"></a>다음 단계

- [칩 액세스 문제 해결](chip-access-trouble.md)
