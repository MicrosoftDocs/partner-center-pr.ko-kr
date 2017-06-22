---
title: "청구서 읽기 | 파트너 센터"
description: "송장은 현재 월별 기간의 모든 요금(프로그램, 제품 및 고객 전체)에 대한 요약입니다. 송장은 파트너 센터 대시보드에서 확인할 수 있습니다."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: d51bb3d8cf637e50e47c211c00d90b14e55a1c6d
ms.sourcegitcommit: 0b00306bfb0b406e64ad857cb360de4533740e6a
ms.translationtype: HT
ms.contentlocale: ko-KR
---
# <a name="read-your-bill"></a>청구서 읽기

**적용 대상**

-  파트너 센터
-  미국 정부용 Microsoft 클라우드 파트너 센터
-  Microsoft 클라우드 독일 파트너 센터

송장은 현재 월별 기간의 모든 요금(프로그램, 제품 및 고객 전체)에 대한 요약입니다. 송장은 파트너 센터 대시보드에서 확인할 수 있습니다.

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
<td>송장을 보내는 주소입니다. 이 주소를 변경하려면 파트너 센터 계정 프로필을 편집하세요.</td>
</tr>
<tr class="odd">
<td>반복 청구 요금</td>
<td>구입한 사용량 기준 라이선스에 대한 고정 월(또는 연간) 요금으로, 서비스 전에 청구됩니다. 이 숫자는 라이선스 기준 조정 파일의 &quot;Subtotal&quot; 열(열 T)에 있는 모든 요금의 합계입니다.</td>
</tr>
<tr class="even">
<td>사용 요금</td>
<td>청구 월 동안 사용하도록 설정되고 사용된 새 서비스 또는 응용 프로그램을 포함한 Azure 사용량입니다. 이 숫자는 사용량 기준 조정 파일의 &quot;PretaxCharges&quot; 열(열 Z)에 있는 모든 요금의 합계입니다.</td>
</tr>
<tr class="odd">
<td>크레딧 및 조정</td>
<td>구독에 대해 수행된 변경 내용에 대한 크레딧 또는 조정입니다(예: 실제 사용자 수 증가 또는 감소).</td>
</tr>
<tr class="even">
<td>기타 할인</td>
<td>예를 들어 고객이 구독의 정상 가격에서 받은 할인입니다. 이 항목은 단가 또는 라이선스당 가격이 아니라 고정 금액으로 표시됩니다.</td>
</tr>
<tr class="odd">
<td>세금</td>
<td>송장 2페이지의 시작 부분에 있는 세부 정보 섹션에 합산되어 있는 현재 요금의 총 세금입니다. 이 숫자의 다음 열에 있는 모든 요금의 합계입니다.
<ul>
<li>사용량 기준 조정 파일의 &quot;TaxAmount&quot; 열(열 AA) 및</li>
<li>라이선스 기준 파일의 &quot;Tax&quot; 열(열 U)</li>
</ul></td>
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
<td>CSP 파트너는 월 단위로 요금이 청구됩니다.</td>
</tr>
<tr class="even">
<td>송장 날짜</td>
<td>송장을 받는 날짜입니다.</td>
</tr>
<tr class="odd">
<td>결제 기한</td>
<td>이 날짜에 결제 금액이 들어와야 합니다.</td>
</tr>
<tr class="even">
<td>고객 PO</td>
<td>구매 주문 번호입니다.</td>
</tr>
<tr class="odd">
<td>고객 서비스</td>
<td>고객 서비스에 액세스하기 위한 웹 사이트 주소입니다.</td>
</tr>
<tr class="even">
<td>서비스 수령인</td>
<td>서비스가 사용되는 주소입니다. (회사 자격 심사와 연결된 법적 회사 주소이며 변경할 수 없습니다.)</td>
</tr>
</tbody>
</table>

 

 

 



