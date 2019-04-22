---
title: 조정 파일 사용 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 7022f1e3d26751e66f90db96bf6d881cb2a694d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/18/2019
ms.locfileid: "59430202"
---
# <a name="use-the-reconciliation-files"></a>조정 파일 사용

**적용 대상**

-  파트너 센터
-  Microsoft Cloud for US Government 파트너 센터


각 요금 청구 주기에서 보려면 자세한 품목을 파트너 센터에서 조정 파일을 다운로드 합니다. 세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.

## <a name="formatting-issues"></a>서식 지정 문제

경우에 따라 여러 파일에 서식 지정 문제 있을 수 있습니다. (이 경우 발생할 수 있습니다, 예를 들어 EN-US 로캘을 사용 되지 않습니다.) 이러한 문제를 해결 하려면 다음 단계를 수행 합니다. 

<ol>
<li>Excel에서.csv 파일을 열고 첫 번째 열을 선택 합니다. 리본에서 선택 <strong>데이터</strong>를 선택한 후 <strong>열에 텍스트</strong>합니다.</li>

<li>텍스트 변환 마법사에서에서 선택 <strong>파일 형식을 구분</strong>를 선택한 후 <strong>다음</strong>합니다.</li> 

<li>구분 기호 필드에서 선택 <strong>쉼표로</strong>합니다. 하는 경우 <strong>탭</strong> 은 이미 선택 상태로 남겨둘 수 있습니다. <strong>다음</strong>을 선택합니다.</li>

<li>열 데이터 형식 필드에서 선택 <strong>날짜: MDY</strong>를 선택한 후 <strong>다음</strong>합니다.</li> 

<li>열 데이터 형식 필드에서 선택 <strong>텍스트</strong> 열을 선택한 후 모든 금액에 대 한 <strong>마침</strong>합니다.</li>
</ol>

## <a href="" id="itemizebypartner"></a>파트너가 항목별로 정리


간접 모델의 파트너는 라이선스 기준 및 사용량 기준 조정 파일에서 모두 이러한 추가 필드를 사용하여 재판매인을 기준으로 항목별로 구분할 수 있습니다.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>MPN ID</th>
<th>설명</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>MPN ID</td>
<td><p>CSP 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) ID.</p></td>
</tr>
<tr class="even">
<td>재판매인 MPN ID</td>
<td><p>간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</p>
<p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. 파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</p>
<p>eTo 확인 하거나 업데이트 대리점에서 파트너 센터 메뉴에서 선택 <strong>고객</strong>, 다음 목록에서 고객을 선택 합니다. 고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다. <strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</p>
<p>CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</p>
<p>CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</p>
<p>CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> 라이선스 기반 파일 필드


고객의 주문에 따라 요금을 조정하려면 조정 파일의 Syndication\_Partner\_Subscription\_Number와 파트너 센터의 구독 ID를 비교합니다.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>열</strong></td>
<td><strong>설명</strong></td>
<td><strong>샘플 값</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>특정 청구 엔터티의 고유 식별자(GUID 형식). 조정에는 필요하지 않지만 유용한 정보일 수 있습니다. 모든 행에서 같습니다.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 청구 플랫폼에서 주문의 고유 식별자. 지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 청구 플랫폼에서 구독의 고유 식별자. 지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p>
<p>이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다. Syndication_Partner_Subscription_Number를 참조하세요.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>구독의 고유 식별자. 고객은 같은 계획으로 여러 구독을 사용할 수 있으므로 이 식별자는 조정 파일 분석에 중요합니다.</p>
<p>이 필드는 파트너 관리 콘솔에서 구독 ID에 매핑됩니다.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>고유 제품 ID. 가격표에 따른 표준 제품 ID.</p>
<p><b>참고</b>: 이 값은 가격 목록에서 제품 ID를 일치 하지 않습니다. 아래의 DurableOfferID를 참조하세요.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>고유 지속형 제품 ID(가격표에 정의됨).</p>
<p><b>참고</b>: 이 값에는 가격 목록에서 제품 ID와 일치합니다.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>고객이 구매한 서비스 제품의 이름(가격표에 정의됨).</p></td>
<td>Microsoft Office 365(계획 E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>구독 시작 날짜(주문이 제출된 다음 날로 설정됨). 구독 시작 날짜와 함께 종료 날짜를 살펴보면 고객이 아직 구독의 첫 번째 해에 속하는지 아니면 구독이 다음 연도에 대해 갱신되었는지를 확인할 수 있습니다.</p>
<p>시간은 항상 해당하는 날의 시작인 0:00입니다.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>구독 종료 날짜: 12 개월 + x 일 후 시작 날짜 (종료 날짜를 청구 하는 파트너와 맞춤) 또는 갱신 날짜 로부터 12 개월입니다.</p>
<p>갱신 시 가격은 현재 가격표로 업데이트됩니다. 자동 갱신에 앞서 고객과 연락해야 할 수 있습니다.</p>
<p>시간은 항상 해당하는 날의 시작인 0:00입니다.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>요금 시작일.</p>
<p>고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</p>
<p>시간은 항상 해당하는 날의 시작인 0:00입니다.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>요금 종료일.</p>
<p>고객이 실제 사용자 수를 변경하면 이 사용자 수는 요금을 일별로 부과(비례하는 계산)하는 데 사용됩니다.</p>
<p>시간은 항상 해당 일의 마지막인 23:59입니다.</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>요금 또는 조정 유형. <a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</p></td>
<td><p><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>실제 사용자 수당 가격. 구매 시 가격표에 게시된 바와 같음. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>수량</td>
<td><p>실제 사용자 수. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Amount</td>
<td><p>수량의 가격 합계. 금액 계산이 귀하가 고객에 대해 이 값을 계산하는 방법과 일치하는지를 확인하는 데 유용합니다.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>이러한 요금에 적용된 할인 금액. 인센티브를 받을 수 있는 새 구독 또는 IUR도 이 열에 할인 금액을 포함합니다.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>세금을 적용하기 전의 총액. 할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Tax</td>
<td><p>세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>세금을 적용한 후의 총액. 송장에 세금이 부과되었는지 확인합니다.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. 통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>고객&#39;파트너 센터에 보고 된 s 조직 이름. 시스템 정보로 송장을 조정할 때 매우 중요합니다.</p></td>
<td>테스트 고객 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>CSP 파트너의 MPN ID</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다. 이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>구독 애칭. 애칭을 지정하지 않으면 파트너 센터에서 OfferName을 사용합니다.</p></td>
<td>프로젝트 온라인</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>고객이 구매한 서비스 제품의 이름(가격표에 정의됨). (제품 이름과 동일한 필드).</p></td>
<td>프로젝트 클라이언트 없는 프로젝트 온라인 프리미엄</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>사용량 기반 파일 필드


고객의 사용량에 따라 요금을 조정하려면 조정 파일의 ResellerID/ResellerName/ResellerBillableAccount, 파트너 센터의 구독 ID 및 고객 이름을 비교합니다.

다음 필드에서는 사용된 서비스와 요금을 설명합니다.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>열</strong></td>
<td><strong>설명</strong></td>
<td><strong>샘플 값</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>GUID 형식의 파트너 ID</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>파트너 이름</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>파트너 계정 ID</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>고객&#39;파트너 센터에 보고 된 s 조직 이름. 시스템 정보로 송장을 조정할 때 매우 중요합니다.</p></td>
<td>테스트 고객 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>CSP 파트너의 MPN ID입니다.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">파트너를 기준으로 항목별로 구분</a>을 참조하세요.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>지정한 트랜잭션이 표시되는 송장 번호</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜.</p>
<p>시간은 항상 해당하는 날의 시작인 0:00입니다.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜.</p>
<p>시간은 항상 해당 일의 마지막인 23:59입니다.</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 청구 플랫폼에서 구독의 고유 식별자. 지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p>
<p>이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>서비스의 애칭.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>서비스 제품의 LOB(기간 업무)</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 청구 플랫폼에서 주문의 고유 식별자. 지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>해당 Azure 서비스의 이름</p></td>
<td>VIRTUAL MACHINES</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Microsoft Azure 서비스의 특정 유형</p></td>
<td><ul>
<li>서비스 버스 - 개별 또는 팩</li>
<li>SQL Azure 데이터베이스 - Business 또는 Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>모든 서비스 데이터 및 가격 구조에 대 한 특정 고유 식별자</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Resource Name</td>
<td><p>Azure 리소스의 이름</p></td>
<td><ul>
<li>데이터 수신(GB)</li>
<li>데이터 발신(GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>사용이 적용되는 지역입니다. 요금이 지역별로 다르므로 주로 데이터 전송에 요금을 할당하는 데 사용됩니다.</p></td>
<td>아시아 태평양, 유럽, 라틴 아메리카, 북아메리카</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>제품에 대한 MSFT 고유 식별자</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>지정된 청구 기간의 서비스 또는 리소스에 대한 다양한 요금을 항목별로 구분하기 위한 ID 및 수량. Azure 계층형 등급의 경우 특정 수량의 청구 가능 단위까지 한 등급이고 그 후에는 다른 등급이 지정될 수 있습니다.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>보고 기간 중 소비된 서비스 양(시간, GB 등).</p>
<p>이전 보고 기간의 미청구 사용량도 포함됩니다.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>제품의 일부로 포함된 단위. 일반적으로 CSP에는 없습니다.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>제품의 일부로 포함되지 않고 파트너가 요금을 지불해야 하는 단위.</p>
<p>ConsumedQuantity에서 IncludedQuantity를 뺀 값입니다.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>구독 시작 날짜에 유효한 제품 가격</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrice에 OverageQuantity를 곱한 값으로, 가장 가까운 센트로 반올림됩니다.</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>세 금액 요금을 시장에 따라&#39;s 세금 규칙 및 특정 한 상황입니다.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>세금을 적용할 수 있는 경우 세금을 적용한 후의 총액</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. 통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>세전 단가. PretaxCharges를 OverageQuantity로 나눈 값으로, 가장 가까운 센트로 반올림됩니다.</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>세후 단가. PostTaxTotal을 OverageQuantity로 나눈 값 또는 PretaxEffectiveRate에 단위 금액당 세율을 더한 값으로, 가장 가까운 센트로 반올림됩니다.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>요금 또는 조정 유형. <a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</p></td>
<td><p><a href="#charge_types">송장과 조정 파일 간 요금 매핑</a>을 참조하세요.</p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>MSFT 청구 플랫폼에서 고유한 계정 ID</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>서비스 배포 날짜</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</p></td>
<td>동아시아, 동남 아시아, 북유럽, 서유럽, 미국 중북부, 미국 중남부</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>이 열은 Service_Name 열에서 구체적으로 식별할 수 없는 개별 Microsoft Azure 서비스를 추적하는 데 사용됩니다. 예를 들어 Service_Name 열에서 데이터 전송이 &quot;Microsoft Azure - 전체 서비스&quot;로 보고됩니다. 이 MeteredService 열은 사용이 관련된 특정 서비스를 나타냅니다.</p></td>
<td>AccessControl, CDN, 계산, 데이터베이스, ServiceBus, 저장소</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>개별 Microsoft Azure 서비스를 MeteredService 필드에 제공된 수준보다 자세히 설명하는 부제목</p></td>
<td>EXTERNAL</td>
</tr>
<tr class="even">
<td>프로젝트</td>
<td><p>해당 서비스 인스턴스에 대한 고객 정의 이름</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>지정일에 프로비전 및 사용된 ServiceBus 연결 수</p></td>
<td>예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다. 해당 날짜에 대 한 일일 사용량 명세서 477860 경우 프로 비전 하는 service Bus 연결 25 팩 있고 해당 일 동안 1을 사용 하면, "25 개 연결 / 30 일 – 사용: 1.000000”.</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>고객&#39;s 도메인 이름, 고객을 식별 하는 데 사용 합니다. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>단위</td>
<td><p>리소스 이름의 단위</p></td>
<td>GB 또는 시간</td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a>일회성 및 되풀이 파일 필드

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Column</th>
<th>설명</th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td>PartnerId</td>
<td><p>특정 청구 엔터티 GUID 형식에서에 대 한 고유한 Microsoft Azure Active Directory 테 넌 트 식별자입니다. 조정에는 필요하지 않지만 유용한 정보일 수 있습니다. 모든 행에서 같습니다.</p></td>
</tr>

<tr class="even">
<td>Customer Id</td>
<td><p>고유한 Microsoft Azure Active Directory 테 넌 트 ID를 GUID 형식으로 고객을 식별 하는 데 사용 합니다.</p></td>
</tr>

<tr class="odd">
<td>고객 이름</td>
<td><p>파트너 센터에 보고된 고객의 조직 이름.</p></td>
</tr>

<tr class="even">
<td>CustomerDomainName</td>
<td><p>고객을 식별하는 데 사용되는 고객의 도메인 이름입니다. 이렇게 해서는 안으로 고객/파트너 수 O365 포털을 통해 베 니 티/기본 도메인을 업데이트 하는 고객을 고유 하 게 식별 합니다. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다.</p></td>
</tr>

<tr class="odd">
<td>고객 국가</td>
<td><p>고객이 위치한 국가입니다.</p></td>
</tr>

<tr class="even">
<td>송장 번호</td>
<td><p>지정한 트랜잭션이 표시되는 송장 번호</p></td>
</tr>

<tr class="odd">
<td>MpnId</td>
<td><p>CSP 파트너의 MPN ID입니다.</p></td>
</tr>

<tr class="even">
<td>Reseller MpnId</td>
<td><p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다.</p></td>
</tr>

<tr class="odd">
<td>주문 ID</td>
<td><p>Microsoft commerce platform은 주문에 대 한 고유 식별자입니다. 지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p></td>
</tr>

<tr class="even">
<td>주문 날짜</td>
<td><p>주문이 이루어진 날짜입니다.</p></td>
</tr>

<tr class="odd">
<td>ProductId</td>
<td><p>제품의 ID입니다.</p></td>
</tr>

<tr class="even">
<td>SkuId</td>
<td><p>특정 SKU의 ID입니다.</p></td>
</tr>

<tr class="odd">
<td>AvailabilityId</td>
<td><p>특정 가용성에 대한 ID입니다. "가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</p></td>
</tr>

<tr class="even">
<td>SKU 이름</td>
<td><p>특정 SKU의 제목입니다.</p></td>
</tr>

<tr class="odd">
<td>제품 이름</td>
<td><p>제품 이름입니다.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>제품의 게시자의 이름입니다.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>이 게시자에 대 한 고유 ID입니다.</p></td>
</tr>

<tr class="even">
<td>구독 설명</td>
<td><p>구독의 이름입니다.</p></td>
</tr>

<tr class="odd">
<td>구독 ID</td>
<td><p>Microsoft commerce platform은 구독에 대 한 고유 식별자입니다. 지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다. 이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>요금 시작일. 시간은 항상 해당하는 날의 시작인 0:00입니다.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>요금 종료일. 시간은 항상 해당 일의 마지막인 23:59입니다.</p></td>
</tr>

<tr class="even">
<td>용어 및 Billingcycle</td>
<td><p>기간 및 구매에 대 한 청구 주기입니다. 예를 들어, "1 년, 월."</p></td>
</tr>

<tr class="odd">
<td>청구 유형</td>
<td><p>요금 또는 조정 유형.</p></td>
</tr>

<tr class="even">
<td>Unit Price</td>
<td><p>구매 시 게시 된 가격표의 가격입니다. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
</tr>

<tr class="odd">
<td>효과적인 단가</td>
<td><p>단위 가격 조정을 만든 후입니다.</p></td>
</tr>

<tr class="even">
<td>수량</td>
<td><p>단위 수입니다. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
</tr>

<tr class="odd">
<td>단위 형식</td>
<td><p>구매 되는 단위의 형식입니다.</p></td>
</tr>

<tr class="even">
<td>DiscountDetails</td>
<td><p>적용 가능한 할인을 설명 합니다.</p></td>
</tr>

<tr class="odd">
<td>Sub Total</td>
<td><p>세금을 적용하기 전의 총액. 할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다.</p></td>
</tr>

<tr class="even">
<td>세금 합계</td>
<td><p>해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</p></td>
</tr>

<tr class="odd">
<td>Total</td>
<td><p>세금을 적용한 후의 총액. 송장에 세금이 부과되었는지 확인합니다.</p></td>
</tr>

<tr class="even">
<td>Currency</td>
<td><p>통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. 통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다.</p></td>
</tr>

<tr class="odd">
<td>AlternateID</td>
<td><p>대체 식별자에는 주문 id입니다.</p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a>매일 배분 사용 현황 파일 필드


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Column</th>
<th>설명</th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td>PartnerId</td>
<td><p>GUID 형식의 파트너 ID</p></td>
</tr>

<tr class="even">
<td>PartnerName</td>
<td><p>파트너 이름</p></td>
</tr>

<tr class="odd">
<td>CustomerId</td>
<td><p>고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다.</p></td>
</tr>

<tr class="even">
<td>CustomerCompanyName</td>
<td><p>파트너 센터에 보고된 고객의 조직 이름. 시스템 정보로 송장을 조정할 때 매우 중요합니다.</p></td>
</tr>

<tr class="odd">
<td>CustomerDomainName</td>
<td><p>고객의 도메인 이름입니다. 현재 작업에 사용할 수 없습니다.</p></td>
</tr>

<tr class="even">
<td>고객 국가</td>
<td><p>고객이 위치한 국가입니다.</p></td>
</tr>

<tr class="odd">
<td>MPNID</td>
<td><p>CSP 파트너의 MPN ID입니다.</p></td>
</tr>

<tr class="even">
<td>Reseller MPNID</td>
<td><p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. 현재 작업에 사용할 수 없습니다.</p></td>
</tr>

<tr class="odd">
<td>InvoiceNumber</td>
<td><p>지정한 트랜잭션이 표시되는 송장 번호 현재 작업에 사용할 수 없습니다.</p></td>
</tr>

<tr class="even">
<td>ProductId</td>
<td><p>제품의 ID입니다.</p></td>
</tr>

<tr class="odd">
<td>SkuId</td>
<td><p>특정 SKU의 ID입니다.</p></td>
</tr>

<tr class="even">
<td>AvailabilityId</td>
<td><p>특정 가용성에 대한 ID입니다. "가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다.</p></td>
</tr>

<tr class="odd">
<td>SKU 이름</td>
<td><p>특정 SKU의 제목입니다.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>게시자의 이름입니다.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>GUID 형식으로 게시자의 ID입니다. 현재 작업에 사용할 수 없습니다.</p></td>
</tr>

<tr class=”even">
<td>구독 설명</td>
<td><p>고객이 구매한 서비스 제품의 이름(가격표에 정의됨). (제품 이름과 동일한 필드).</p></td>
</tr>

<tr class="odd">
<td>구독 ID</td>
<td><p>Microsoft 청구 플랫폼에서 구독의 고유 식별자. 지원 센터에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다. 이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 시작 날짜. 시간은 항상 해당하는 날의 시작인 0:00입니다.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>이전 청구 주기에서 이전에 요금이 청구되지 않은 숨은 사용 데이터의 날짜를 표시하는 경우를 제외하고 청구 주기의 종료 날짜. 시간은 항상 해당 일의 마지막인 23:59입니다.</p></td>
</tr>

<tr class="even">
<td>사용 날짜</td>
<td><p>서비스 사용의 날짜입니다.</p></td>
</tr>

<tr class="odd">
<td>미터 종류</td>
<td><p>측정기의 형식입니다.</p></td>
</tr>

<tr class="even">
<td>미터 범주</td>
<td><p>사용에 대 한 최상위 수준 서비스입니다.</p></td>
</tr>

<tr class="odd">
<td>미터 Id</td>
<td><p>사용 중인 미터에 대 한 ID입니다.</p></td>
</tr>

<tr class="even">
<td>미터 하위 범주</td>
<td><p>속도 영향을 줄 수 있는 Azure 서비스의 형식입니다.</p></td>
</tr>

<tr class="odd">
<td>미터 이름</td>
<td><p>사용 중인 미터에 대 한 측정 단위입니다.</p></td>
</tr>

<tr class="even">
<td>요금제 지역</td>
<td><p>이 열은 이 열이 적용 가능하고 채워진 서비스 지역 내에 있는 데이터 센터의 위치를 식별합니다.</p></td>
</tr>

<tr class="odd">
<td>단위</td>
<td><p>단위 리소스 이름입니다.</p></td>
</tr>

<tr class="even">
<td>사용한 수량</td>
<td><p>보고 기간 중 소비된 서비스 양(시간, GB 등). 이전 보고 기간의 미청구 사용량도 포함됩니다.</p></td>
</tr>

<tr class="odd">
<td>리소스 위치</td>
<td><p>측정기 실행 되 고 있는 데이터 센터입니다.</p></td>
</tr>

<tr class="even">
<td>사용 되는 서비스</td>
<td><p>사용한 Azure 플랫폼 서비스입니다.</p></td>
</tr>

<tr class="odd">
<td>리소스 그룹</td>
<td><p>배포 된 측정기 실행 되는 리소스 그룹입니다.</p></td>
</tr>

<tr class="even">
<td>리소스 URI</td>
<td><p>사용 중인 리소스의 URI입니다.</p></td>
</tr>

<tr class="odd">
<td>청구 유형</td>
<td><p>요금 또는 조정 유형. 현재 작업에 사용할 수 없습니다.</p></td>
</tr>

<tr class="even">
<td>단가</td>
<td><p>라이선스를 구매 시 가격표를 게시 하는 대로 당 가격입니다. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
</tr>

<tr class="odd">
<td>수량</td>
<td><p>라이선스의 수입니다. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
</tr>

<tr class="even">
<td>단위 형식</td>
<td><p>측정기 요금이 청구 되는 단위의 형식입니다. 현재 작업에 사용할 수 없습니다.</p></td>
</tr>

<tr class="odd">
<td>청구 전 세금</td>
<td><p>세금 전에 총 공간입니다.</p></td>
</tr>

<tr class="even">
<td>청구 통화</td>
<td><p>고객의 지리적 지역에 통화</p></td>
</tr>

<tr class="odd">
<td>세금 공제 전 가격 책정 요약</td>
<td><p>가격 책정 세금 추가 되기 전에 합니다.</p></td>
</tr>

<tr class="even">
<td>통화 가격 책정</td>
<td><p>가격표에서 통화입니다.</p></td>
</tr>

<tr class="odd">
<td>서비스 정보 1</td>
<td><p>지정일에 프로비전 및 사용된 ServiceBus 연결 수</p></td>
</tr>

<tr class="even">
<td>서비스 정보 2</td>
<td><p>선택적 서비스 특정 메타 데이터를 캡처하는 레거시 필드입니다.</p></td>
</tr>

<tr class="odd">
<td>Tags</td>
<td><p>청구 레코드를 그룹화 하려면 측정기에 할당 하는 태그입니다. 예를 들어를 측정기를 사용 하는 부서에서 비용을 배분 하는데 태그를 사용할 수 있습니다.</p></td>
</tr>

<tr class="even">
<td>추가 정보</td>
<td><p>다른 열에서 다루지 않는 추가 정보.</p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a>청구서 및 조정 파일 간 요금 매핑

송장은 요금 요약 정보를 제공하는 반면 조정 파일은 요금 종류를 비롯한 거래 품목의 구체적인 분류 정보를 제공합니다.

송장과 조정 파일의 요금을 교차 참조하려면 Microsoft Excel의 필터 옵션을 통해 조정 파일을 요금 종류별로 필터링하여 송장 요금을 조정 파일의 요금 분류 집합에 매핑하면 됩니다.

사용량 기준 및 라이선스 기준 모두 조정 파일은 사용량 관련 거래 및 요금만 표시합니다(사용 및 관련 요금 단위). 송장에 "조정"으로 표시되는 크레딧, 할인, 또는 환불 내역은 조정 파일에 표시되지 않습니다.

아래는 송장 섹션과 조정 파일에 표시될 수 있는 관련 요금 종류 간의 매핑을 보여주는 표입니다. 

<table>
<tbody>
<tr>
<td>
<p><strong>청구서 금액 충전 설명</strong></p>
</td>
<td>
<p><strong>조정 파일 금액 설명 (ChargeType 열)</strong></p>
</td>
<td>
<p><strong>이 요금 이란 무엇 인가요?</strong></p>
</td>
<td>
<p><strong>이러한 ChargeTypes를 청구서에 매핑하려면 어떻게 하나요?</strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong>라이선스 기반 요금</strong></p>
</td>
<td>
<p>활성화 수수료</p>
</td>
<td>
<p>고객이 구독을 구매한 후 구독을 사용할 때 고객에게 청구되는 요금</p>
</td>
<td rowspan="10">
<p>라이선스 기반 파일에서 <strong>Amount</strong> 열을 모두 합산</p>
</td>
</tr>
<tr>
<td>
<p>취소 수수료</p>
</td>
<td>
<p>연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</p>
</td>
</tr>
<tr>
<td>
<p>주기 수수료</p>
</td>
<td>
<p>구독에 대한 정기 요금</p>
</td>
</tr>
<tr>
<td>
<p>주기 인스턴스 비례 배분</p>
</td>
<td>
<p>연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</p>
</td>
</tr>
<tr>
<td>
<p>취소 시 비례 배분 방식 요금</p>
</td>
<td>
<p>취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</p>
</td>
</tr>
<tr>
<td>
<p>구매 시 비례 배분 방식 요금</p>
</td>
<td>
<p>연간 청구를 사용 하는 경우 구독에 대 한 요금 유형</p>
</td>
</tr>
<tr>
<td>
<p>구매 요금</p>
</td>
<td>
<p>월 청구 비용은 사용 하는 경우 구독에 대 한 요금 유형</p>
</td>
</tr>
<tr>
<td>
<p>갱신 시 비례 배분 방식 요금</p>
</td>
<td>
<p>구독 갱신 시 비례 배분 방식 요금</p>
</td>
</tr>
<tr>

<td>
<p>갱신 요금</p>
</td>
<td>
<p>구독 갱신에 대한 요금</p>
</td>
</tr>
<tr>
<td>
<p>활성화 시 비례 배분 방식 요금</p>
</td>
<td>
<p>활성화 시점부터 청구 기간 마지막 날까지의 비례 배분 방식 요금</p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>사용 요금</strong></p>
</td>
<td>
<p>취소 시 사용 요금 계산</p>
</td>
<td>
<p>현재 청구 기간 중 결제되지 않은 사용량에 대해 취소 시 사용 요금 계산</p>
</td>
<td rowspan="2">
<p>사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</p>
</td>
</tr>
<tr>
<td>
<p>현재 주기의 사용 요금 계산</p>
</td>
<td>
<p>현재 청구 기간의 사용 요금 계산</p>
</td>
</tr>
<tr>
<td>
<p><strong>크레딧</strong></p>
</td>
<td>
<p>품목 오프셋</p>
</td>
<td>
<p>세금을 포함하여 품목의 전액 또는 일부 금액 환불</p>
</td>
<td>
<p>라이선스 기반 파일에서 <strong>TotalForCustomer</strong> 열을 모두 합산</p>
<p>사용량 기반 파일에서 <strong>PostTaxTotal</strong> 열을 모두 합산</p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong>사용량 기반 할인</strong></p>
</td>
<td>
<p>활성화 할인</p>
</td>
<td>
<p>구독을 활성화할 때 적용되는 할인</p>
</td>

<td rowspan="4">
<p>사용량 기반 파일에서 <strong>PretaxCharges</strong> 열을 모두 합산</p>
</td>
</tr>
<tr>
<td>
<p>주기 할인</p>
</td>
<td>
<p>정기 요금에 적용되는 할인</p>
</td>
</tr>
<tr>
<td>
<p>갱신 할인</p>
</td>
<td>
<p>구독을 갱신할 때 적용되는 할인</p>
</td>
</tr>
<tr>
<td>
<p>취소 할인</p>
</td>
<td>
<p>할인이 취소될 때 적용되는 요금</p>
</td>
</tr>


<tr>
<td>
<p><strong>라이선스 기반 할인</strong></p>
</td>
<td>
<p><em>여러 요금 유형에 적용할 수 있습니다.</em></p>
</td>
<td>
<p></p>
</td>
<td>
<p>라이선스 기반 파일에서 <strong>TotalOtherDiscount</strong> 열을 모두 합산</p>
</td>
</tr>
<tr>
<td>
<p><strong>세금</strong>&nbsp;또는&nbsp;<strong>VAT</strong></p>
</td>
<td>
<p><em>여러 요금 유형에 적용할 수 있습니다.</em></p>
<p><em>예외: &quot;품목 요금 차감&quot; 이미 세금이 포함 되어 있습니다. 위의 크레딧을 참조 하세요.</em></p>
</td>
<td>
<p>세금 또는 VAT(부가가치세)</p>
</td>
<td>
<p>라이선스 기반 파일에서 <strong>Tax</strong> 열을 모두 합산</p>
<p>사용량 기반 파일에서 <strong>TaxAmount</strong> 열을 모두 합산</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
