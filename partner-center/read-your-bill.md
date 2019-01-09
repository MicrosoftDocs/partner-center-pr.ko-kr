---
title: 청구서 읽기 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 송장은 현재 월별 기간의 모든 요금(프로그램, 제품 및 고객 전체)에 대한 요약입니다. 이 파트너 센터에서 사용할 수 있습니다.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: 구독 청구, 청구, 파트너 센터에서 청구, 파트너 센터 청구, 내 청구 보기, 송장, 파트너 센터 송장, CSP 송장, 내 청구서 위치
ms.localizationpriority: medium
ms.openlocfilehash: aec344eb7e4ed6e0a4d5e7e506c9bcf195654293
ms.sourcegitcommit: 9eadb7ff6c38a08c694710a8c14b899d0f48059a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/09/2019
ms.locfileid: "8997342"
---
# <a name="read-your-bill"></a>청구서 읽기

**적용 대상**

-  파트너 센터
-  미국 정부용 Microsoft 클라우드 파트너 센터


청구서를 **파트너 센터** 메뉴로 이동 하 고 하면 청구 내역과 추세, 송장 및 조정 파일, 최근 결제가 표시 링크를 보려면 **청구** 를 선택 합니다.

월별 청구를 선택한 클라우드 솔루션 공급자 프로그램의 파트너는 고객의 구독(라이선스 및 사용량 기준 모두)에 대해 60일 후불제 방식으로 Microsoft에 결제하게 됩니다.

> [!NOTE]  
> 송장 모든 요금 요약 송장은 프로그램, 제품 및 고객-현재 청구 기간에 대 한 이며 UTC 시간에 선택한 청구 날짜 2 일에 제공 됩니다. 예를 들어가 경우 9 월 12 청구 날짜 송장 생성 프로세스는 13에 오전 12 시 UTC에서 시작 하 고는 14th에서 오전 12 시 UTC에 의해 완료 합니다. 15 일에 송장을 오후 11시 59분 utc 표시 되지 않으면, 서비스 수준 계약 부재 및 파일 서비스 요청을 해야 합니다. 

일회성 (Azure reserved VM instances)에 대 한 별도 송장과 라이선스 기준 (Office365) 및 사용량 기준 (Azure) 요금에 대 한 송장을 하나 받게 됩니다 요금.

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
<td>송장을 보내는 주소입니다. 회사 이름 또는 주소를 변경 하려면 해당 파트너 센터 청구 프로필을 편집 합니다. </td>
</tr>
<tr class="odd">
<td>라이선스 기준 청구</td>
<td>구입한 사용량 기준 라이선스에 대한 고정 월(또는 연간) 요금으로, 서비스 전에 청구됩니다. 이 숫자는 라이선스 기준 조정 파일의 &quot;Subtotal&quot; 열(열 T)에 있는 모든 요금의 합계입니다.</td>
</tr>
<tr class="even">
<td>사용량 기준 청구</td>
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
<td>소계</td>
<td>세금 및 세금 단독 요금 및 크레딧이 하기 전의 총액.</td>
</tr>
<td>세금</td>
<td>송장 2페이지의 시작 부분에 있는 세부 정보 섹션에 합산되어 있는 현재 요금의 총 세금입니다. 이 숫자의 다음 열에 있는 모든 요금의 합계입니다.
<ul>
<li>사용량 기준 조정 파일의 &quot;TaxAmount&quot; 열(열 AA) 및</li>
<li>라이선스 기준 파일의 &quot;Tax&quot; 열(열 U)</li>
</ul></td>
</tr>
<tr class="odd">
<td>다른 크레딧</td>
<td>세금 단독 크레딧입니다.</td>
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
<td>송장 날짜에 이르는 월별 기간입니다. 이는 사용량 기준 서비스를 사용 하 고 라이선스 기반 서비스는 모든 신용 조정 또는 라이선스 수의 변경에 대 한 조정 기간입니다.</td>
</tr>
<tr class="even">
<td>송장 날짜</td>
<td>청구 날짜 또는 1 주년 날짜는 송장 매달 생성 됩니다.</td>
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
<td>서비스가 사용되는 주소입니다. (회사 자격 심사와 연결 된 법적 회사 주소입니다.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>일회성 요금의 항목별 목록

|**필드** |**정의**|
|:----------------|:-----------------------------|
|날짜 |구매 날짜입니다. |
|설명 |제품 이름입니다. |
|수량 |구입한 제품(예: 예약)의 수입니다. |
|단가 |각 제품(예: 예약)의 가격입니다. |
|할인 |적용 가능한 모든 할인 혜택입니다. |
|세전 금액 |세금 부과 전 구입액의 소계입니다. |
|판매세 |세금 액수입니다. |
|총액 |지불해야 할 총액입니다. |
 



