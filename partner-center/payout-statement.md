---
title: 지급 명세서
description: 지급 문과 요약 및 Microsoft 파트너 센터에서 지불 데이터를 보고 내보내는 방법에 대해 알아봅니다.
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/2/2021
ms.openlocfilehash: 681080b654ca1a12523a7ff63fc75a44daaab9b7
ms.sourcegitcommit: 7ef441a0e4dbef11012212bfc087c5244a75765e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "102185352"
---
# <a name="payout-statements"></a>지급 명세서

**적절한 역할:**

- 계정 관리자
- 글로벌 관리자

**지급 문은** 상업적 marketplace를 통해 판매 되는 제품의 지급에 대 한 개요를 제공 합니다. 수익의 트랜잭션 기록을 표시 하 고, 다음 지불을 예측 하 고, 지불 추세를 표시 합니다. 트랜잭션 기록과 지불 문을 다운로드할 수도 있습니다. 이 문서에서는 지급 문에 액세스 하는 방법과 파트너 센터에서 액세스할 수 있는 다양 한 지급 페이지 및 다운로드를 설명 합니다.

>[!NOTE]
>연결 된 MPN Id 및 프로그램에 대 한 데이터만 볼 수 있습니다. 추가 데이터를 확인 하려면 계정 관리자에 게 사용 권한을 문의 하세요. 

## <a name="roles-and-permissions"></a>역할 및 권한

지급 문에 액세스 하려면 **계정 소유자** 또는 **재무 참가자** 역할을 할당 받아야 합니다.

| 보고서/페이지 | 계정 소유자 | Manager | Developer | 비즈니스 기여자 | 재무 기여자 | 마케터 |
| --- | --- | --- | --- | --- | --- | --- |
| 취득 보고서(근 실시간 데이터 포함) | 보기 가능 | 보기 가능 | 액세스 권한 없음 | 액세스 권한 없음 | 보기 가능 | 액세스 권한 없음 |
| 사용자 의견 보고서/응답 | 사용자 의견을 보고 보낼 수 있음 | 사용자 의견을 보고 보낼 수 있음 | 사용자 의견을 보고 보낼 수 있음 | 액세스 권한 없음 | 액세스 권한 없음 | 사용자 의견을 보고 보낼 수 있음 |
| 상태 보고서(근 실시간 데이터 포함) | 보기 가능 | 보기 가능 | 보기 가능 | 보기 가능 | 액세스 권한 없음 | 액세스 권한 없음 |
| 사용량 보고서 | 보기 가능 | 보기 가능 | 보기 가능 | 보기 가능 | 액세스 권한 없음 | 액세스 권한 없음 |
| 지급 계정 | 업데이트할 수 있음 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 | 업데이트할 수 있음 | 액세스 권한 없음 |
| 세금 프로필 | 업데이트할 수 있음 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 | 업데이트할 수 있음 | 액세스 권한 없음 |
| 지급 요약 | 보기 가능 | 액세스 권한 없음 | 액세스 권한 없음 | 액세스 권한 없음 | 보기 가능 | 액세스 권한 없음 |
|

## <a name="access-your-payout-statement"></a>지급 문에 액세스

[파트너 센터](https://partner.microsoft.com/dashboard/home) 에 로그인 하 고 화면 오른쪽 위 모서리에서 지급 아이콘을 선택 하 여 다음과 같은 다양 한 요약에 액세스 합니다.

- 거래 기록
- 결제
- 데이터 내보내기

:::image type="content" source="images/payouts/payout-overview.png" alt-text="파트너 센터 포털의 오른쪽 위 모퉁이에 있는 지급 아이콘을 보여 줍니다.":::

또한 [Partner 지급 API](https://apidocs.microsoft.com/services/partnerpayouts) 를 사용 하 여 지급 트랜잭션 및 지불 데이터를 직접 연결 하 고 가져올 수 있습니다.


## <a name="transaction-history"></a>거래 기록

**트랜잭션 기록** 페이지에는 수익, 예상 된 다음 지불 및 지난 36 개월 동안의 수입 및 지불 추세에 대 한 요약이 표시 됩니다. 이 섹션에서 트랜잭션 세부 정보를 다운로드할 수도 있습니다.<br><br>이 보고서는 아직 보내지 않은 지불을 포함 하 여 지급에 적합 한 모든 수익을 보여 줍니다. 지급는 ISV가 파트너 센터에서 모든 은행 및 세금 정보를 완료 했 $50 >을 때, ISV 계정이 활성 상태이 고, 고객에 게 요금이 청구 되었거나 (EA 거래의 경우) 지불이 수신 된 경우 (ea가 아닌 트랜잭션에 대 한)에 적합 합니다.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="트랜잭션 개요.":::

- **올해 수입** -지불 되었으며 향후 달에 지불 되는 수익의 총 수입 및 분석입니다.
- **예상 지불 월** – 예정 된 달에 예상 되는 총 수익입니다.
- **수입 및 지불 추세** – 지난 36 개월 동안의 월간 획득 및 지불 금액입니다.
- **다운로드** – 트랜잭션 세부 정보를 .csv 또는. tsv 형식으로 다운로드 합니다.

페이지의 오른쪽 위 모퉁이에 있는 날짜 범위 선택을 사용 하 여 지난 3, 6, 12 또는 36 개월이 표시 되도록 페이지의 출력을 필터링 합니다. 또는 최대 36 개월의 사용자 지정 날짜 범위를 선택 합니다. 기본 날짜 범위는 12 개월입니다. 등록 ID, 프로그램, 지불 ID, 획득 유형, 레버 및 상태별로 필터링 할 수도 있습니다. 현재 회계 연도 (7 월 1 일-6 월 30 일)와 이전 두 회계 연도에 대해 데이터를 사용할 수 있습니다.

:::image type="content" source="images/payouts/search-filter.png" alt-text="페이지의 오른쪽 위에 있는 검색 필터입니다.":::

수익에 대한 자세한 내용을 보려면 페이지 오른쪽에 있는 아래쪽 화살표를 선택합니다. 이렇게 하면 레버, 수익 금액, 제품 및 고객을 표시 합니다. 어떤 이유로 든이 데이터를 사용할 수 없지만 액세스 권한이 필요한 경우 지원 담당자에 게 문의 하세요. 트랜잭션이 아닌 조정 결과가 발생 하는 경우에는 Product 및 Customer 필드가 표시 되지 않습니다.

### <a name="transaction-history-summary"></a>트랜잭션 기록 요약

이는 판매 된 제품의 날짜, 상태 및 예상 지불 월 획득의 출처를 포함 하 여 자세한 정보를 표시 합니다.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="트랜잭션 기록.":::

- **진척 날짜** – 구매 날짜입니다.
- 획득 **유형** – 판매, 리베이트, 공동 op 등의 획득 유형입니다.
- **총 금액** – 순 획득 금액입니다. 상업적 marketplace에서이는 표준 마켓플레이스 요금을 빼는 한 후에이를 의미 합니다.
- **상태** – 세 가지 옵션이 있습니다.
    - **예정** 된 – 소득은 냉각 기간 보류 중입니다.
    - **처리** 됨 – 소득은 다음 지불에 대해 준비 됩니다.
    - **Sent** – 소득이 지불 되었습니다.
- **예상 지불 월** – 소득이 지불 될 것으로 예상 되는 월입니다. 자세한 내용은 [다음 섹션](#estimated-payment-month) 을 참조 하세요.

트랜잭션이 지급 자격을 충족 하면 트랜잭션이 표시 됩니다. 수익 누락 또는 예상치 못한 수익을 이해 하려면 [상업적 marketplace 지급에 대 한 일반적인 질문](payout-faq.md#why-are-my-earnings-missing)을 참조 하세요.

#### <a name="estimated-payment-month"></a>예상 지불 월

이제 트랜잭션 기록 페이지에는 향후 몇 개월 동안의 예상 지불 금액을 보여 주는 표가 포함 되어 있습니다. 트랜잭션 기록과 요약 보고서 내보내기에서이 정보를 보고 다운로드할 수도 있습니다. 이 정보를 통해 reconciliations 지불 프로젝션을 더 쉽게 수행할 수 있습니다.

예상 지불 월은 프로그램 구성 규칙과 타임 라인을 기준으로 계산 되며 다음/예정 된 지불 주기에 처리 됩니다.

현재는 **적용 되지 않는** 것으로 표시 되는 공동 op를 제외한 모든 획득 형식에 대해 예상 지불 월을 사용할 수 있습니다. 2020 년 7 월 1 일 이전 소득의 경우 예상 지불 월은 **사용할 수 없음** 으로 표시 됩니다.

다음 표에서는 예상 지불 월 예를 보여 줍니다.

| 월 | 금액 |
| ------ | :-----------: |
|  9 월-2020 |  $7273.99   |
|  Oct-2020 | $8692.30  |
|  2020년 11월 | $107.89  |

예상 금액은 다음과 같은 다양 한 이유로 실제 양과 다를 수 있습니다.

- 재작성 획득: 수익을 다시 계산 하는 경우 실제 금액은 다를 수 있습니다.
- 조정: 실제 크기는 발생 했거나 제출 된 조정에 따라 달라 집니다.
- 규칙 변경: 규칙의 변경 내용에 따라 실제 지불 금액의 다시 계산이 반영 될 수 있습니다.
- 지불 오류가 발생 하는 경우 실제 금액은 다를 수 있습니다.

프로그램의 임계값과 지불 자격 규칙이 충족 되는 경우에만 지불 된 달에 지불 됩니다. 이러한 규칙은 다음 목록에만 포함 되어 있습니다.

- 세금 프로필은 최신 이어야 합니다.
- 소득은 프로그램 가이드에 정의 된 최소 획득 임계값을 충족 하거나 초과 해야 합니다.
- 보류 중 지급: 프로필 할당 페이지에서 "지불 유지" 옵션을 선택 하는 경우
- 지급 계측을 사용할 수 없음: 지불 또는/및 세금 프로필이 완료 되지 않았습니다.

### <a name="transaction-history-download"></a>트랜잭션 기록 다운로드

획득에 대 한 자세한 내용을 보려면 페이지 위쪽에서 **다운로드** 를 선택 합니다. 다음 표에서는 보고서의 각 열에 대해 설명 합니다.

>[!NOTE]
>트랜잭션 기록 다운로드 내보내기에는 8 월 2020의 새로운 두 필드가 있습니다.
>
>- **lastPaymentCurrency**  현재 로그인 한 파트너에 게 액세스 권한이 있는 모든 MPNs에서 가장 최근의 지불을 받은 통화입니다. 지불이 수신 되지 않으면 마지막 지불 통화는 미국 달러입니다.
>- **earningAmountInLastPaymentCurrency**  마지막 지불 통화의 양입니다.

| 열 이름 | 설명 | 동기 프로그램/마켓플레이스에 대 한 적용 가능성 |
| --- | --- | --- |
| agreementEndDate | 계약 종료 날짜 | 인센티브 - 일부 프로그램만 해당 |
| agreementNumber | 계약 번호 | 인센티브 - 일부 프로그램만 해당 |
| agreementStartDate | 계약 시작 날짜 | 인센티브 - 일부 프로그램만 해당 |
| calculationDate | 시스템에서 수익을 계산한 날짜 | 모두 |
| claimId | 클레임에 대한 고유 식별자 | 인센티브 - 일부 프로그램만 해당 |
| customerCountry | 고객 국가/지역 | marketplaces |
| customerEmail |  |  |
| customerName | 비워 둘 수 있음 | 프로그램을 동기 (예외: OEM) 하 고 마켓플레이스 합니다. CSP 트랜잭션의 경우 마켓플레이스는 CSP의 이름을 표시 합니다. |
| customerTenantId |  |  |
| distributorId | 배포자 식별자 | 인센티브 - 일부 프로그램만 해당 |
| distributorName | 배포자 이름 | 인센티브 - 일부 프로그램만 해당 |
| earningAmount | 원래 거래 통화의 수익 금액 | 모두 |
| earningAmountInLastPaymentCurrency | 마지막 지불 통화의 수익금(이전 지불액을 지불하지 않은 경우 필드는 비어 있음) |  |
| earningAmountUSD | 수익 금액(USD) | 모두 |
| earningDate | 수익 창출 날짜 | 모두 |
| earningExchangeRate | 해당 USD 금액을 표시하는 데 사용되는 환율 | 모두 |
| earningId | 각 수익에 대한 고유 식별자 | 모두 |
| earningRate | 획득을 생성 하기 위해 트랜잭션 양에 적용 되는 성과급 율 | 모두 |
| earningType | 수수료, 환불, 협업, 판매 등인지를 나타냅니다. | 모두 |
| exchangeRateDate | EarningAmount USD를 계산하는 데 사용되는 환율 날짜 | 모두 |
| externalReferenceId | 프로그램에 대한 고유 식별자 | 직접 지불 프로그램 (성과급 및 마켓플레이스) |
| externalReferenceIdLabel | 고유 식별자 레이블 | 직접 지불 프로그램 (성과급 및 마켓플레이스) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | 송장 번호 (enterprise에만 적용 가능) | 성과급 및 마켓플레이스-일부 프로그램만 |
| lastPaymentCurrency | 마지막 지불 통화(이전 지불액을 지불하지 않은 경우 필드는 비어 있음) |  |
| lever | 수익에 대한 비즈니스 규칙을 나타냅니다. | 모두 |
| LicensingProgramName | 라이선스 프로그램의 이름 |  |
| LineItemId | 고객 청구서의 개별 품목 |  |
| localProviderSeller | 레코드의 로컬 공급자/판매자 |  |
| 완성 월 | 예상 지불 월 | 모두 |
| OrderID | 고객의 청구서와 관련이 있음  | marketplaces |
| parentProductId | 고유한 부모 제품 식별자. 거래에 대한 부모 제품이 없는 경우 부모 제품 ID는 제품 ID입니다. | marketplaces |
| parentProductName | 부모 제품의 이름. 거래에 대한 부모 제품이 없는 경우 부모 제품 이름은 제품 이름입니다. | marketplaces |
| participantId | 프로그램에 따라 수익을 창출하는 파트너의 기본 ID | 모두 |
| participantIdType | 마켓플레이스 인 경우 일반적으로 동기 프로그램 및 판매자의 프로그램 ID | 모두 |
| participantName | 수익 파트너의 이름 | 모두 |
| partnerCountryCode | 수익 파트너의 위치/국가/지역 | 모두 |
| partNumber | 항상 비어 있음 | 일부 동기 프로그램 및 마켓플레이스 |
| paymentId | 결제에 대한 고유 식별자. 이 번호는 일반적으로 은행 거래 내역서에 표시됩니다. | SAP 결제 전용 |
| paymentStatus | 결제 상태 | 모두 |
| paymentStatusDescription | 결제 상태에 대한 친숙한 설명 | 모두 |
| productId | 고유 제품 식별자 | marketplaces |
| productName | 거래에 연결된 제품 이름 | 모두 |
| productType | 제품의 유형(예: 앱, 추가 기능 또는 게임) | marketplaces |
| 프로그램 코드 | 프로그램 이름으로 매핑할 문자열 |  |
| programName | 인센티브/Store 프로그램 이름 | 모두 |
| purchaseOrderCoverageEndDate | 항상 비어 있음 | 인센티브 프로그램 - CRI |
| purchaseOrderCoverageStartDate | 항상 비어 있음 | 인센티브 프로그램 - CRI |
| purchaseOrderType | 항상 비어 있음 | 인센티브 프로그램 - CRI |
| purchaseTypeCode | 항상 비어 있음 | 인센티브 프로그램 - CRI |
| quantity | 프로그램에 따라 다릅니다. 거래 프로그램에 청구된 수량을 나타냅니다. | 모두 |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | 재판매인 식별자 | 인센티브 - 일부 프로그램만 해당 |
| resellerName | 재판매인 이름 |  |
| SkuId | 게시 중에 정의한 SKU ID. 한 제품에 여러 SKU가 포함될 수는 있지만 각 SKU는 제품 하나에만 연결할 수 있습니다. 인센티브 - 일부 프로그램만 해당 |  |
| storeFee | Store에서 앱 또는 추가 기능을 사용할 수 있도록 하기 위한 수수료로 Microsoft에서 보유하는 금액 | marketplaces |
| subscriptionEndDate | 구독 종료 날짜 | 인센티브 - 일부 프로그램만 해당 |
| subscriptionId | 고객에 연결된 구독 식별자 | 인센티브 - 일부 프로그램만 해당 |
| subscriptionStartDate | 구독 시작 날짜 | 인센티브 - 일부 프로그램만 해당 |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | 세금(판매세, 사용세 또는 VAT/GST 세금)을 납부할 책임이 있는 당사자 | marketplaces |
| taxRemitted | 세금 납부 금액(판매세, 사용세 또는 VAT/GST 세금) | marketplaces |
| taxState | 고객 상태 |  |
| taxZipCode | 고객 우편 번호 |  |
| tpan | 타사 광고 네트워크를 나타냅니다. | 마켓플레이스 광고만 |
| transactionAmount | 생성된 수익에 기반한 거래 금액(원래 거래 통화) | 모두 |
| transactionAmountUSD | 거래 금액(USD) | 모두 |
| transactionCountryCode | 거래가 발생한 국가/지역 코드 |  |
| transactionCurrency | 원래 고객 거래가 발생한 지역의 통화(파트너 위치의 통화가 아님) | 모두 |
| transactionDate | 거래 날짜. 많은 거래가 하나의 수익에 기여하는 프로그램에 유용합니다. | 모두 |
| transactionExchangeRate | 해당 거래 USD 금액을 표시하는 데 사용되는 환율 날짜 | 모두 |
| transactionId | 거래에 대한 고유 식별자 | 모두 |
| transactionPaymentMethod | 카드, 이동 통신 회사 청구 또는 PayPal과 같은 거래에 사용되는 고객 결제 수단 | marketplaces |
| transactionType | 거래의 유형(예: 구매, 환불, 환입 또는 지급 거절) | marketplaces |
| workload | 워크로드 | 인센티브 - 일부 프로그램만 해당 |
|

### <a name="transaction-adjustment-codes"></a>트랜잭션 조정 코드

다음 표에서는 조정에 대 한 이유 코드와 그에 대 한 설명을 보여 줍니다.

|**이유 코드**   |**설명**   |
|------------------|:-------------------------------------|
| AR 규정 준수 | 파트너의 시간에 Microsoft 송장이 지불 되지 않는 경우 수익을 감소 시키는 조정. |
| 공동 op 롤오버 | 공동 op 소득을 다른 기간으로 전송 하거나 공동 op 소득을 리베이트로 변환 하는 조정입니다. |
| Ops 조정 | Microsoft 시스템 계산 오류를 해결 하는 조정입니다. |
| Ops 조정 Microsoft 잘못 된 계산 | 사용할 경우 해당를 수정 하는 조정입니다. |
| Ops 조정 Microsoft 잘못 된 등록 | 등록 관련 사용할 경우 해당을 조정 합니다. |
| 파트너 매핑 (구독) MCI/CSP | 구독 불일치를 해결 하는 조정입니다. |
| 정책 예외 | 프로그램 규칙을 재정의 하는 조정입니다.  |
| 이전 기간 소득 | 현재 획득 기간을 벗어나 수익을 조정 합니다. |

## <a name="payments"></a>결제

**지불** 페이지에는 Microsoft에서 사용한 금액이 자세히 나와 있습니다. 또한 지불 되는 시기와 방법을 보여 줍니다.

>[!Note]
> 지급을 사용할 수 있으려면 수익이 $50의 [결제 임계값](payment-thresholds-methods-timeframes.md)에 도달해야 합니다. 자세한 내용은 [Microsoft Publisher 계약](https://go.microsoft.com/fwlink/?LinkID=699560)을 참조 하십시오.

:::image type="content" source="images/payouts/payments-overview.png" alt-text="지불 개요 화면입니다.":::

- **올해 총 지불** – 모든 프로그램에 대해 올해에 지불 된 총 판매액 (미국 달러)입니다.
- **다음으로 예상** 되는 지불 – 귀하에 게 제공 되는 한 번의 지불 (다른 사용자가 곧 제공 되는 경우에도)은 미국 달러입니다.
- **마지막 지불** – 가장 최근의 지불 금액 (미국 달러), 프로그램 이름 및 프로그램입니다.
- **원본에** 의 한 지불-지난 12 개월 동안 프로그램 당 지불 금액 (미국 달러)입니다.

### <a name="payments-list"></a>지불 목록

지불 및 보류 중인 지불액을 보여 주는 **지불 테이블 목록** 입니다. 서비스 요금 세금 정보를 PDF 형식으로 다운로드 하 고 지정 된 결제에 대 한 세부 정보를 볼 수 있습니다.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="트랜잭션 기록 내보내기":::

- **유료** – 모든 지불이 성공적으로 전송 되었습니다. 드롭다운 메뉴에서 연도를 선택 하 여 해당 연도에 릴리스되는 지불로 필터링 합니다.
- **보류 중** – 예정 된 지불액.
- **서비스 요금 세금 (PDF 양식)** – 서비스 요금 세금을 지불 하는 데 사용할 수 있습니다. 서비스 요금 세금이 **다른 세금이** 표시 됩니다.
- **보기** – 지불에 포함 된 소득 목록이 포함 된 트랜잭션 기록으로 리디렉션합니다.

수익 누락 또는 예상치 못한 수익을 이해 하려면 [상업적 marketplace 지급에 대 한 일반적인 질문](payout-faq.md#why-are-my-earnings-missing)을 참조 하세요.

### <a name="payment-status"></a>결제 상태

다음 표에서는 다양 한 획득 상태를 설명 합니다.

| 수익 상태 | 이유 | 파트너 작업이 필요한가요? |
| --- | --- | --- |
| 처리 안 됨 | 지급해야 하는 수익입니다. 이 상태는 성과급 프로그램 프로그램 가이드에 정의 된 대로 냉각 기간 동안 유지 됩니다. | 예 |
| 예정 | 지불을 처리 하기 전에 지불 주문에서 내부 검토를 생성 했습니다. | 예 |
| 세금 계산서 보류 중 | 세금 송장이 불완전 하거나 잘못 되었습니다. | 지급하기 전에 세금 계산서를 업데이트해야 합니다. |
| 검토 중 거부됨 | 검토 하는 동안 결제를 거부 했습니다. | 자세한 내용은 Microsoft 지원에 문의하세요. |
| 실패 | Microsoft 시스템 오류로 인해 지불 하지 못했습니다. | 자세한 내용은 Microsoft 지원에 문의 하세요. |
| 진행 중 | 지불이 진행 중입니다. | 예 |
| 잘못된 결제 | 지불 recouping 진행 중입니다. | 예 |
| 송금 | 요금을 은행으로 보냈습니다. | 예 |
| 다시 처리 중 | 지불 중에 Microsoft 시스템 오류가 발생 하 여 다시 처리 하는 중입니다. | 예 |
| Reversed | 결제는 은행에 의해 반대 되었으며 다음 지불 주기에 다시 전송 됩니다. | 예 |
| 세금계산서 거부됨 | 검토 중에 세금 계산서가 거부되었습니다. 세금계산서 검토가 완료될 때까지 보류 중인 모든 결제가 보류됩니다. | 자세한 내용은 Microsoft 지원에 문의 하세요. |
| 세금계산서 검토 중 | 세금계산서를 검토하고 있습니다. 세금계산서가 승인되면 결제가 해제됩니다. | 예 |
| 거부됨 | 사용자의 은행이 결제를 거부 했습니다. | 자세한 내용은 은행 담당자에게 문의하세요. |
|

### <a name="payments-download"></a>지불 다운로드

 다음 표에서는 보고서의 각 열에 대해 설명 합니다. 지불에 대 한 자세한 내용을 보려면 지불 페이지의 위쪽에서 **다운로드** 를 선택 합니다.

| 열 이름 | Description |
| --- | --- |
| participantID | 프로그램에 따라 수익을 창출하는 파트너의 기본 ID |
| participantIDType | 일반적으로 프로그램에 대 한 프로그램 ID 및 스토어 프로그램용 판매자 ID |
| participantName | 수익 파트너의 이름 |
| programName | 성과급/매장 프로그램 이름 |
| earned | 해당 프로그램/participantID에 대한 수익 금액(결제 통화) |
| earnedUSD | 프로그램/participantID에 대한 수익 금액(USD) |
| withheldTax | 프로그램/participantID에 대한 원천징수세액(결제 통화) |
| salesTax | Program/participantID에 대 한 유료 통화의 총 판매 세금 (성과급 프로그램에만 해당) |
| serviceFeeTax | 프로그램/participantID에 대한 serviceFeeTax 총액(결제 통화)(Store 프로그램 및 Azure Marketplace에만 적용 가능) |
| totalPayment | 프로그램/participantID에 대한 원천징수세를 제외하고 판매세를 포함한(해당하는 경우) 총 지급액(현지 통화) |
| currencyCode | 결제 통화 코드 |
| paymentMethod | 파트너에게 지급하는 데 사용되는 방법(예: 전자 은행 송금, 신용 메모) |
| paymentID | 결제에 대한 고유 식별자. 이 번호는 일반적으로 은행 거래 내역서에 표시됩니다(SAP 결제에만 해당). |
| paymentStatus | 결제 상태 |
| paymentStatusDescription | 결제 상태에 대한 친숙한 설명 |
| paymentDate | Microsoft에서 결제한 날짜 |
|

## <a name="export-data"></a>데이터 내보내기

**데이터 내보내기** 페이지는 자체적으로 새로 고쳐지지 않습니다. 최신 데이터를 보려면 페이지를 수동으로 새로 고쳐야 할 수도 있습니다. 세 개의 탭 중 하나를 선택 하 여 **트랜잭션 기록**, **지불**, **트랜잭션 요약** 또는 **기록 문을** 내보냅니다.

필터를 사용 하면 데이터를 **사용할 수 없음** 오류가 발생할 수 있습니다. 이 문제는 세 달에 선택한 기본 기간을 남은 후 해당 기간 외의 획득에서 지불 ID를 선택한 경우에 발생할 수 있습니다. 이 문제가 발생 하면 해당 기간을 확장 하 고 다시 시도 하세요.

샘플 지불 내보내기는 다음과 같습니다.

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="지불 보고서를 내보냅니다.":::

### <a name="historical-statements"></a>거래 기록 명세서

**데이터 내보내기** 요약은 기록 문에 대 한 액세스도 제공 합니다.

> [!NOTE]
> 기록 문은 스냅숏이 며 새로 고쳐지지 않습니다. [지원](https://partner.microsoft.com/support/v2/?stage=1) 팀에 문의 하 고 필요한 경우 최신 데이터를 요청 하세요.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="기록 문을 내보냅니다.":::

- 2019 년 7 월 1 일 이전의 트랜잭션 기록은 별도로 처리 되며 이후 기록 보고서의 다른 필드를 사용 합니다.
- 레거시 트랜잭션 기록에는 최신 기록의 "소득" 열에 해당 하는 "예약 됨" 이라는 열이 있습니다. 단, 상태와 "지불 전송 됨"과 같은 모든 소득은 제외 됩니다.
- 3M, 6M 또는 12M과 같은 필터는 거래 기록 명세서 섹션에 적용되지 않습니다.

### <a name="historical-statement-downloads"></a>기록 문 다운로드

다음 표에서는 기록 문의 각 열에 대해 설명 합니다.

| 필드 이름 | Description |
| --- | --- |
| 수입원 | 거래가 발생한 위치(예: Microsoft Store, Windows Phone Store, Windows Store 8 또는 광고)에 기반한 수입의 출처 |
| 주문 ID | 고유한 주문 식별자. 이 ID를 통해 구매 이외의 해당 거래(예: 환불 또는 지급 거절)를 사용하여 구매 거래를 식별할 수 있습니다. 둘 다 동일한 주문 ID를 사용합니다. 또한 단일 구매에 여러 결제 방법을 사용 하는 분할 된 요금이 있는 경우 구매 트랜잭션을 연결할 수 있습니다. |
| Transaction ID | 고유한 거래 식별자 |
| 거래 날짜/시간 | 거래가 발생한 날짜 및 시간(UTC) |
| 부모 제품 ID | 고유한 부모 제품 식별자. 거래에 대한 부모 제품이 없는 경우 부모 제품 ID는 제품 ID입니다. |
| Product ID | 고유한 제품 식별자 |
| 부모 제품 이름 | 부모 제품의 이름. 거래에 대한 부모 제품이 없는 경우 부모 제품 이름은 제품 이름입니다. |
| 제품 이름 | 제품의 이름 |
| 제품 유형 | 제품의 유형(예: 앱, 추가 기능 또는 게임) |
| 수량 | 수입원이 비즈니스용 Microsoft Store인 경우 수량은 구매한 라이선스 수를 나타냅니다. 다른 모든 수입원의 경우 수량은 항상 1입니다. 서로 다른 두 가지 결제 방법이 사용되어 하나의 거래가 두 개의 품목으로 분할된 경우에도 각 품목의 수량은 1로 표시됩니다. |
| 트랜잭션 유형 | 거래의 유형(예: 구매, 환불, 환입 또는 지급 거절) |
| 결제 방법 | 카드, 이동 통신 회사 청구 또는 PayPal과 같은 거래에 사용되는 고객 결제 수단 |
| 국가/지역 | 거래가 발생한 국가/지역 |
| 로컬 공급자/판매자 | 레코드의 로컬 공급자/판매자 |
| 거래 통화 | 거래의 통화 |
| 거래 금액 | 거래의 금액 |
| 세금 납부 | 세금 납부 금액(판매세, 사용세 또는 VAT/GST 세금) |
| 순 수령액 | 거래 금액에서 세금 납부 금액을 뺀 금액 |
| Store 수수료 | Store에서 앱 또는 추가 기능을 사용할 수 있도록 하기 위한 수수료로 Microsoft에서 보유하는 순 수령액에 대한 백분율 |
| 앱 수익 | 순 수령액에서 Store 수수료를 뺀 금액 |
| 원천징수세 | 수입에서 원청징수된 세액(또는 **예약됨** CSV 파일에 포함된 세액) |
| 결제 | 앱 수익에서 적용 가능한 원천징수세를 뺀 금액(거래 통화로 표시되는 금액) **예약됨** CSV 파일에는 포함되지 않습니다. |
| 환율 | 거래 통화를 결제 통화로 변환하는 데 사용되는 환율 |
| 결제 통화 | 결제되는 통화 |
| 변환된 결제 | 환율을 사용하여 결제 통화로 변환된 결제 금액 |
| 세금 납부 모델 | 세금(판매세, 사용세 또는 VAT/GST 세금)을 납부할 책임이 있는 당사자 |
| 적격 날짜/시간 | 거래 수익이 지급될 수 있는 날짜 및 시간(UTC). 지급이 만들어지면 지급을 만든 날짜 이전의 적격 날짜/시간이 포함된 거래 수익이 포함됩니다(**예약됨** CSV 파일에만 포함됨). |
| Charges | 거래 금액 열에 집계된 모든 요금 세부 정보에 대한 분석이 표시됩니다(Azure Marketplace에만 포함됨, **예약됨** CSV 파일에는 포함되지 않음). |
|||

## <a name="next-steps"></a>다음 단계

- [파트너 지급 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [지급 정책 세부 정보](payout-policy-details.md)
- 청구 지원에 대해서는 상업용 Marketplace [게시자 지원 서비스](https://partner.microsoft.com/support/v2/?stage=1)에 문의하세요.
