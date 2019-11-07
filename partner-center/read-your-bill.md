---
title: 청구서 읽기 | 파트너 센터
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 송장은 현재 월별 기간의 모든 요금(프로그램, 제품 및 고객 전체)에 대한 요약입니다. 파트너 센터에서 사용할 수 있습니다.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: 구독 청구, 청구, 파트너 센터에서 청구, 파트너 센터 청구, 내 청구 보기, 송장, 파트너 센터 송장, CSP 송장, 내 청구서 위치
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652181"
---
# <a name="read-your-bill"></a>청구서 읽기

**적용 대상**

-  파트너 센터
-  Microsoft Cloud for US Government 파트너 센터


청구서의 경우 **파트너 센터** 메뉴로 이동 하 고 **청구** 를 선택 하 여 청구 기록과 추세, 청구서 및 조정 파일에 대 한 링크 및 가장 최근의 지불을 확인 합니다.

월별 청구를 선택한 클라우드 솔루션 공급자 프로그램의 파트너는 고객의 구독(라이선스 및 사용량 기준 모두)에 대해 60일 후불제 방식으로 Microsoft에 결제하게 됩니다.

> [!NOTE]  
> 청구서는 프로그램, 제품 및 고객에 대 한 모든 요금에 대 한 요약으로, 현재 청구 기간에 대해 UTC 시간에 선택한 청구 날짜의 2 일 이내에 사용할 수 있습니다. 예를 들어 9 월 12 일의 청구 날짜가 있는 경우 청구서 생성 프로세스는 13 분 오전 12 시에 시작 되 고 14 일에서 오전 12 시에 오전 12 시에 완료 됩니다. 15:59PM UTC로 청구서가 표시 되지 않는 경우에는 Service Level Agreement(서비스 수준 약정)를 제외 하 고 서비스 요청을 파일에 써야 합니다. 

라이선스 기반(Office365) 및 사용량 기반(Azure) 요금에 대한 송장 하나와 일회성(Azure Reserved VM Instances) 요금에 대한 별도의 송장을 받게 됩니다.

부과되는 요금에 대한 항목별 세부 정보를 보려면 함께 제공되는 조정 파일을 참조하세요. 조정 파일에는 고객 송장을 만드는 데 사용하는 고객 ID와 구독 ID가 포함되어 있습니다. 자세한 내용은 [조정 파일 사용 방법](use-the-reconciliation-files.md)을 참조하세요.

## <a name="invoice-file-definitions"></a>송장 파일 정의


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>필드</strong></td>
<td><strong>설명</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>연방 세금 ID 번호입니다.</td>
</tr>
<tr class="odd">
<td>고객 번호</td>
<td>고객 번호입니다.</td>
</tr>
<tr class="even">
<td>청구지</td>
<td>송장을 보내는 주소입니다. 회사 이름 또는 주소를 변경 하려면 파트너 센터 청구 프로필을 편집 합니다. </td>
</tr>
<tr class="odd">
<td>라이선스 기반 요금</td>
<td>구입한 사용량 기준 라이선스에 대한 고정 월(또는 연간) 요금으로, 서비스 전에 청구됩니다. 이 숫자는 라이선스 기준 조정 파일의 &quot;Subtotal&quot; 열(열 T)에 있는 모든 요금의 합계입니다.</td>
</tr>
<tr class="even">
<td>사용량 기반 청구</td>
<td>청구 월 동안 사용하도록 설정되고 사용된 새 서비스 또는 응용 프로그램을 포함한 Azure 사용량입니다. 이 숫자는 사용량 기준 조정 파일의 &quot;PretaxCharges&quot; 열(열 Z)에 있는 모든 요금의 합계입니다.</td>
</tr>
<tr class="odd">
<td>할인</td>
<td>예를 들어 고객이 구독의 정상 가격에서 받은 할인입니다. 이 항목은 단가 또는 라이선스당 가격이 아니라 고정 금액으로 표시됩니다.</td>
</tr>
<tr class="odd">
<td>크레딧</td>
<td>구독에 대해 수행된 변경 내용에 대한 크레딧 또는 조정입니다(예: 실제 사용자 수 증가 또는 감소).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Subtotal</td>
<td>세금 및 세금이 포함되지 않은 요금 및 크레딧 이전의 총계입니다.</td>
</tr>
<td>Tax</td>
<td>송장 2페이지의 시작 부분에 있는 세부 정보 섹션에 합산되어 있는 현재 요금의 총 세금입니다. 이 숫자의 다음 열에 있는 모든 요금의 합계입니다.
<ul>
<li>사용량 기준 조정 파일의 &quot;TaxAmount&quot; 열(열 AA) 및</li>
<li>라이선스 기준 파일의 &quot;Tax&quot; 열(열 U)</li>
</ul></td>
</tr>
<tr class="odd">
<td>다른 크레딧</td>
<td>세금이 포함되지 않은 크레딧입니다.</td>
</tr>
<tr class="even">
<td>현재 총 요금</td>
<td>기한이 결제 기한까지인 청구 기간의 결제액(청구 통화로 된 금액)입니다.</td>
</tr>
<tr class="odd">
<td>결제 관련 지침</td>
<td>지역을 기준으로 송장 요금 지불 방법을 설명합니다. 결제 시 항상 송장 번호를 포함합니다.</td>
</tr>
<tr class="even">
<td>송장 번호</td>
<td>송장의 번호입니다.</td>
</tr>
<tr class="odd">
<td>청구 기간</td>
<td>매월 청구서 날짜로 계산 되는 기간입니다. 사용 빈도 기반 서비스가 사용 되는 기간으로, 라이선스 기반 서비스는 크레딧 조정 또는 라이선스 수 변화에 맞게 조정 됩니다.</td>
</tr>
<tr class="even">
<td>송장 날짜</td>
<td>송장이 매월 생성 되는 청구 날짜 또는 기념일입니다.</td>
</tr>
<tr class="odd">
<td>지급 조건</td>
<td>일회성 구매에 대해서는 항상 60일 이내입니다.</td>
</tr>
<tr class="even">
<td>결제 기한</td>
<td>이 날짜에 결제 금액이 들어와야 합니다.</td>
</tr>
<tr class="odd">
<td>고객 PO</td>
<td>구매 주문 번호입니다.</td>
</tr>
<tr class="even">
<td>고객 서비스</td>
<td>고객 서비스에 액세스하기 위한 웹 사이트 주소입니다.</td>
</tr>
<tr class="odd">
<td>서비스 수령인</td>
<td>서비스가 사용되는 주소입니다. (회사 심사와 연결 된 법적 회사 주소입니다.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>일회성 요금의 항목별 목록

|**필드** |**정의**|
|:----------------|:-----------------------------|
|날짜 |구매 날짜입니다. |
|설명 |제품 이름입니다. |
|Quantity |구입한 제품(예: 예약)의 수입니다. |
|단가 |각 제품(예: 예약)의 가격입니다. |
|할인 |적용 가능한 모든 할인 혜택입니다. |
|세전 금액 |세금 부과 전 구입액의 소계입니다. |
|판매세 |세금 액수입니다. |
|총액 |지불해야 할 총액입니다. |
 



