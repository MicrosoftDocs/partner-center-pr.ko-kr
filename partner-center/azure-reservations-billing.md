---
title: Azure 예약에 대한 청구 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
Description: Information about billing for Azure reservations.
author: v-petand
ms.author: v-petand
keywords: Azure RI, azure reserved instances, 예약, vm, 관리, 청구, 구입
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: 7aec5102d2ff76d321474e6e580acde6a854a9b5
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796726"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Microsoft Azure Reserved VM Instances 청구

**적용 대상**

-  파트너 센터
-  Microsoft Azure Portal
-  CSP 파트너

클라우드 솔루션 공급자(CSP) 프로그램의 파트너는 이제 Microsoft Azure 가상 컴퓨터에서 고객에게 예약한 인스턴스를 제공할 수 있습니다. 고객은 1년 또는 3년의 기간 동안 미리 가상 컴퓨터를 예약하여 Azure 사용량을 상당 부분 절약할 수 있습니다.   

고객은 Azure Reserved VM Instances에 대한 비용을 미리 지불합니다. 고객을 대신하여 Azure Reserved VM Instances를 구입하면 이러한 일회성 요금에 대한 송장 및 조정 파일을 받게 됩니다. 

>[!IMPORTANT]
>다른 통화를 사용하는 시장의 고객을 위해 Azure Reserved VM Instances를 구입한 경우에는 여러분의 위치가 아니라 고객의 시장을 기준으로 기본 청구 통화가 결정됩니다. 여러 시장의 고객을 확보하고 있는 경우에는 해당 통화로 고객에게 청구를 할 수 있도록 비용이 청구되는 각 통화에 대해 별도의 송장과 조정 파일을 받게 됩니다. 

일회성 요금 송장 및 조정 파일에 액세스 하려면 파트너 센터에서 **청구** 를 선택 하 고 **한 번**을 선택 합니다. 

클라우드 솔루션 공급자 프로그램의 청구에 대한 자세한 내용은 [청구의 기본 사항](billing-basics.md)을 참조하세요.

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Azure Reserved VM Instance 송장 파일 정의

**일반 청구 정보**

|**필드** |**정의**|
|:----------------|:-----------------------------|
|US FEIN |연방 세금 ID 번호입니다. |
|청구지 |세금 목적으로 사용되는 법적 비즈니스 주소입니다. 이 주소를 변경하려면 계정 설정 > 파트너 청구 프로필로 이동합니다. |
|요금 |현재 총 요금입니다. |
|크레딧 |초기 구매 이후 환불 활동에 대한 크레딧입니다. |
|할인: |Azure 예약이나 고객 주문서의 기타 항목에 적용되는 할인입니다. |
|세금 |송장 2페이지의 시작 부분에 있는 세부 정보 섹션에 합산되어 있는 현재 요금의 총 세금입니다. |
|현재 총 요금 |기한이 결제 기한까지인 청구 기간의 결제액(청구 통화로 된 금액)입니다. |
|결제 관련 지침 |지역을 기준으로 송장 요금을 지불하는 시기와 방법을 설명합니다. 결제 시 항상 송장 번호를 포함합니다. |
|송장 번호 |송장의 번호입니다. |
|송장 날짜 |송장이 생성된 날짜입니다. |
|지급 조건 |일회성 구매에 대해서는 항상 60일 이내입니다. |
|결제 기한 |이 날짜에 결제 금액이 들어와야 합니다. |


**일회성 요금의 항목별 목록**

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


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Azure Reserved VM Instance 조정 파일 설명

|**필드** |**정의**|
|:----------------|:-----------------------------|
|PartnerId |GUID 형식의 파트너 ID입니다. |
|CustomerId |고객을 식별하는 데 사용되는 GUID 형식의 고유한 Microsoft ID입니다. |
|CustomerName |파트너 센터에 보고된 고객의 조직 이름. 시스템 정보로 송장을 조정할 때 매우 중요합니다. |
|CustomerDomainName |고객의 도메인 이름입니다. |
|CustomerCountry |고객이 위치한 국가입니다. |
|InvoiceNumber |지정한 트랜잭션이 표시되는 송장 번호입니다. |
|MpnId |CSP 파트너(직접 또는 간접)의 MPN ID입니다. |
|재판매인 MPN ID |간접 모델의 파트너를 위한 조정 파일에만 나타납니다. 예약에 대한 ROR(Reseller of Record)의 MPN ID입니다. 파트너 센터에서 특정 예약에 대해 나열된 재판매인 ID에 해당합니다. CSP 파트너가 고객에게 직접 예약을 판매하는 경우 해당 MPN ID가 두 번 나열됩니다(MPN ID와 재판매인 MPN ID 모두). CSP 파트너에게 MPN ID가 없는 재판매인이 있는 경우 이 값은 대신 파트너의 MPN ID로 설정됩니다. CSP 파트너가 재판매인 ID를 제거하는 경우 이 값은 -1로 설정됩니다. |
|OrderId |Microsoft 청구 플랫폼에서 주문의 고유 식별자입니다. 지원 팀에 문의할 때는 Azure 예약을 식별하는 것이 유용할 수 있지만, 조정에서는 아닙니다. |
|OrderDate |주문이 이루어진 날짜입니다. |
|ProductId |제품의 ID입니다. |
|SkuId  |특정 SKU의 ID입니다. |
|AvailabilityId |특정 가용성에 대한 ID입니다. "가용성"이란 주어진 국가, 통화, 산업 분류 등에서 특정 SKU의 구입이 가능한지 여부를 말합니다. |
|SkuName  |특정 SKU의 제목입니다. |
|ProductName |제품 이름입니다. |
|ChargeType |요금 또는 조정 유형입니다. |
|UnitPrice |주문한 각 제품의 가격입니다. |
|수량 |주문한 제품의 수입니다. |
|소계 |세금을 적용하기 전의 총액. 할인이 있을 경우 소계가 예상 총액과 일치하는지 확인합니다. |
|TaxTotal |적용 가능한 모든 세금의 총액입니다. |
|총액 |총 구입 금액입니다. |
|통화 |통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. 통화가 첫 번째 송장과 일치하는지 확인한 다음 주요 청구 플랫폼 업데이트 후에 다시 확인합니다. |
|DiscountDetails |모든 관련 할인에 대한 상세 목록입니다. |


## <a name="manage-your-billing"></a>청구 관리

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>현재 청구 상태, 송장 및 조정 파일 보기

1.  파트너 센터에서 **청구** , 그런 다음 **한 번** 에 청구 상태를 확인을 선택 합니다. 
2.  자세한 정보를 보려면 송장 또는 조정 파일을 선택합니다. 

### <a name="view-a-customers-order-history"></a>고객의 주문 내역 보기

1.  파트너 센터 메뉴에서 **고객** 을 선택 합니다.
2.  **고객** 페이지에서 주문 내역을 확인하려는 고객을 찾고 아래쪽 화살표를 선택하여 고객의 기록을 펼쳐봅니다. 
3.  **주문 보기**를 선택하여 주문 내역을 표시합니다.

### <a name="create-a-credit-or-void-note"></a>크레딧 또는 빈 어음 만들기

송장을 취소한 다음 새 송장을 발행해야 하는 상황이 발생할 수 있습니다. 예를 들어, 고객이 기업 이름을 변경했는데 기존 이름으로 송장을 수신하는 경우입니다. 

송장을 취소하고 새 송장을 발급 받으려면 조정 아래 청구 페이지에서 양식을 다운로드합니다.

## <a name="azure-reservations-resources"></a>Azure 예약 리소스
|**자세한 내용**   |**이 글 읽기**    |
|:-----------------------------|:-----------------|
|CSP의 Azure 예약 개요  | [Microsoft Azure Reserved VM Instances 판매](azure-reservations.md)
|파트너 센터에서 고객을 위한 Azure 예약 구입   |[Azure 예약 구입](azure-reservations-buying.md)
| 파트너 센터에서 Azure 예약 관리 | [파트너 센터에서 Azure 예약 관리](azure-reservations-manage.md)
|Azure Portal에서 Azure 예약 구입 | Azure 도움말의 [Azure Reserved VM Instances에서 가상 컴퓨터에 대한 사전 지불](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)을 참조하세요. |
|Azure Portal에서 Azure 예약 관리   |Azure 도움말의 [예약된 VM 인스턴스 관리](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)를 참조하세요.  |
|파트너 센터 API를 사용하여 Azure 예약 구입 | 파트너 센터 개발자 설명서의 [Azure Reserved VM Instances 구입](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)을 참조하세요.

 
