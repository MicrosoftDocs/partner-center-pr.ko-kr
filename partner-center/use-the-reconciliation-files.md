---
title: "조정 파일 사용 | 파트너 센터"
description: "청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 8024efe9149ff224a8b2c7d76f46b664df328a3a

---

# 조정 파일 사용


청구 주기에서 각 요금 항목의 세부 정보를 보려면 파트너 센터 대시보드에서 조정 파일을 다운로드합니다. 세부 정보에는 각 고객 구독에 대한 요금 및 자세한 이벤트(예: 중간에 사용자를 구독에 추가)가 포함됩니다.

## 이 섹션의 내용


-   [파트너를 기준으로 항목별로 구분](#itemizebypartner)
-   [라이선스 기준 조정 파일](#licencebasedfiles)
-   [사용량 기준 조정 파일](#usagebasedfiles)

## <a href="" id="itemizebypartner"></a>파트너를 기준으로 항목별로 구분


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
<td><p>CSP 파트너(직접 또는 간접)의 MPN ID입니다.</p></td>
</tr>
<tr class="even">
<td>재판매인 MPN ID</td>
<td><p>간접 모델의 파트너를 위한 조정 파일에만 나타납니다.</p>
<p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. 파트너 센터에서 특정 구독에 대해 나열된 재판매인 ID에 해당합니다.</p>
<p>재판매인을 보거나 업데이트하려면 파트너 센터 메뉴에서 <strong>고객</strong>을 선택한 다음 목록에서 고객을 선택합니다. 고객 메뉴에서 <strong>구독</strong>을 선택한 다음 목록에서 구독을 선택합니다. <strong>업데이트</strong>를 선택하여 <strong>재판매인(MPN ID)</strong>을 변경합니다.</p>
<p>CSP 파트너가 고객에게 직접 구독을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두).</p>
<p>CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다.</p>
<p>CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licencebasedfiles"></a> 라이선스 기준 파일 필드


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
<td>OperatingUnit</td>
<td><p>특정 청구 엔터티의 고유 식별자(GUID 형식). 조정에는 필요하지 않지만 유용한 정보일 수 있습니다. 모든 행에서 같습니다.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerNumber</td>
<td><p>Microsoft 청구 플랫폼에서 고객의 고유 식별자. 지원 센터에 문의할 때 고객을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p></td>
<td>123456789</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 청구 플랫폼에서 주문의 고유 식별자. 지원 센터에 문의할 때 주문을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 청구 플랫폼에서 구독의 고유 식별자. 지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p>
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
<td><p>고유 제품 ID. 가격표에 따른 표준 제품 ID.</p></td>
<td>306855</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>고유 지속형 제품 ID(가격표에 정의됨).</p></td>
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
<td><p>구독 종료 날짜: 12개월 + 시작 날짜 이후 x일(파트너 청구 날짜에 맞추기 위해) 또는 갱신 날짜로부터 12개월.</p>
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
<td><p>요금 또는 조정 유형.</p>
<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Charges:</td>
<td><ul>
<li>PURCHASE_FEE: 구독에 대한 초기 충전</li>
<li>CYCLE_FEE: 구독에 대한 정기 요금</li>
</ul></td>
</tr>
<tr class="even">
<td>ConvertResources</td>
<td><ul>
<li>CANCEL_USAGEFEE: 현재 청구 기간 중 미지불된 사용에 대한 취소 시 액세스 사용 요금</li>
<li>CYCLE_USAGEFEE: 현재 청구 기간에 대한 액세스 사용 요금</li>
</ul></td>
</tr>
<tr class="odd">
<td>Prorations:</td>
<td><ul>
<li>PURCHASE_PRORATE: 구매 시 비례 배분 방식 요금</li>
<li>CANCEL_PRORATE: 취소 시 사용하지 않은 서비스 부분에 대한 비례 배분 방식 환불</li>
<li>ACTIVATION_PRORATE: 활성화부터 청구 기간 끝까지의 비례 배분 방식 요금</li>
<li>RENEW_PRORATE: 구독 갱신 시 비례 배분 방식 요금</li>
</ul></td>
</tr>
<tr class="even">
<td>InstanceProrates:</td>
<td><ul>
<li>CANCEL_INSTANCEPRORATE: 연결된 실제 사용자 수가 변경될 때 고객에게 환불되는 비례 배분 방식 요금</li>
<li>CYCLE_INSTANCEPRORATE: 연결된 실제 사용자 수가 변경될 때 고객이 평가한 비례 배분 방식 요금</li>
</ul></td>
</tr>
<tr class="odd">
<td>Credits:</td>
<td><ul>
<li>CREDIT: 결제 방법에 적용되는 신용</li>
</ul></td>
</tr>
<tr class="even">
<td>Offsets:</td>
<td><ul>
<li>OFFSET_LINEITEM: 품목에 대한 부분 또는 전체 환불</li>
<li>ONE_TIME_REFUND: 고객에 대해 처리된 일회성 환불</li>
<li>TAX_REFUND: 세금 제외 인증서의 유효성으로 인한 환불</li>
</ul></td>
</tr>
<tr class="odd">
<td>Discounts:</td>
<td><ul>
<li>ACTIVATION_DISCOUNT: 구독이 활성화될 때 적용되는 할인</li>
<li>CYCLE_DISCOUNT: 정기 요금에 적용되는 할인</li>
<li>RENEW_DISCOUNT: 구독이 갱신될 때 적용되는 할인</li>
<li>CANCEL_DISCOUNT: 할인이 취소될 때 적용되는 요금</li>
</ul></td>
</tr>
</tbody>
</table>
<p> </p></td>
<td></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>실제 사용자 수당 가격. 조정 중에 대금 청구 시스템에 저장된 정보와 일치하는지 확인합니다.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantity</td>
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
<td><p>해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</p></td>
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
<td><p>파트너 센터에 보고된 고객의 조직 이름. 시스템 정보로 송장을 조정할 때 매우 중요합니다.</p></td>
<td>테스트 고객 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>CSP 파트너의 MPN ID</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. [파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</p></td>
<td>4390934</td>
</tr>
</tbody>
</table>

 

## <a href="" id="usagebasedfiles"></a>사용량 기준 파일 필드


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
<td><p>파트너 센터에 보고된 고객의 조직 이름. 시스템 정보로 송장을 조정할 때 매우 중요합니다.</p></td>
<td>테스트 고객 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>CSP 파트너의 MPN ID입니다.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>구독에 대한 ROR(Reseller of Record)의 MPN ID입니다. [파트너를 기준으로 항목별로 구분](#itemizebypartner)을 참조하세요.</p></td>
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
<td><p>Microsoft 청구 플랫폼에서 구독의 고유 식별자. 지원에 문의할 때 구독을 식별하는 데 유용할 수 있지만 조정에 필요한 것은 아닙니다.</p>
<p>이 ID는 파트너 관리 콘솔의 구독 ID와 다릅니다.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>서비스 제품의 이름</p></td>
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
<td><p>해당 지역/국가의 세금 규칙 및 특정 상황에 따른 세액 요금.</p></td>
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
<td><p>품목 유형에 대한 설명</p></td>
<td>현재 주기에 대한 액세스 사용 요금</td>
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
<td>Project</td>
<td><p>해당 서비스 인스턴스에 대한 고객 정의 이름</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>지정일에 프로비전 및 사용된 ServiceBus 연결 수</p></td>
<td>예: 일수가 30일인 달에 개별적으로 연결을 프로비전한 경우 ServiceInfo1은 "1.000000개 연결/30일"이 됩니다. 25팩 ServiceBus 연결 하나를 프로비전하고 해당 날짜에 연결 1개를 사용한 경우 해당 날짜의 일일 사용 내역서는 "25개 연결/30일 - 사용됨: 1.000000"으로 표시됩니다.</td>
</tr>
</tbody>
</table>

 

 

 






<!--HONumber=Nov16_HO4-->


