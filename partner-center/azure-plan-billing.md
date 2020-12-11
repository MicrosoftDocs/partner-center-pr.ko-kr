---
title: Azure 플랜 청구 - 청구서 및 조정 파일
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure 요금제에 대한 청구와 관련된 청구서 및 조정 파일 구조에 액세스하고 이해하는 방법을 알아봅니다.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 1dc683c194de158dc7a4dac541b37631f3be1f1e
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534695"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP의 새로운 상거래 환경 - Azure 청구 

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 글로벌 관리자

이 문서에서는 Azure 플랜의 대금 청구와 관련된 청구서 및 조정 파일 구조에 액세스하고 이해하는 방법을 설명합니다. Azure 플랜에 따른 청구는 잘 조정된 단일 청구 날짜와 월별 청구 기간을 사용하는 간소화된 청구 환경입니다.

## <a name="summary-of-billing-essentials"></a>청구 기본 정보 요약

- **청구서 날짜**: 청구서 및 조정 파일은 8일(UTC 자정)에 파트너 센터 대시보드/API에서 사용할 수 있습니다.

- **청구서 청구 기간**: 청구서 청구 기간은 달력의 월을 기준으로 조정됩니다(예: 10/1-10/31, 11/1-11/30).

- **서비스 기간 요금 청구**: 요금은 달력의 월을 기준으로 조정됩니다. 예를 들어 청구 파트너가 10/15에 Azure 플랜을 통해 Azure 서비스를 추가하고 고객이 10/15에 Azure 서비스 사용을 시작하는 경우 청구 파트너는 서비스 기간 10/15 - 10/31에 고객이 사용한 요금에 대한 청구서/조정 파일을 11/8에 받게 됩니다. 12/8에 생성될 다음 달 청구서에는 서비스 기간 11/1 - 11/31의 모든 요금이 포함됩니다.

- **청구서 결제 기간**: 순 60일.

- **청구서 통화** : 파트너는 고객의 국가에 할당된 통화로 계속 요금이 청구됩니다. 예를 들어 청구 파트너가 아일랜드에 있고 고객은 영국, 노르웨이 및 독일에 있는 경우 청구 파트너는 GBP, NOK 및 EUR 청구서/조정 파일을 받습니다.

- **파트너 인센티브**: 청구 월이 끝나고 45일 후에 결제됩니다.

## <a name="access-your-invoices-and-reconciliation-files"></a>청구서 및 조정 파일 액세스

청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다.

청구서 및 조정 파일에 액세스하려면 다음을 수행합니다.

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. 파트너 센터 메뉴에서 **청구** 를 선택합니다.

3. **되풀이** 및 **일회성** 탭과 관심 있는 통화를 선택합니다.

   :::image type="content" source="images/azure/billing3.png" alt-text="청구":::

4. **청구서** 또는 **조정 파일** 을 선택합니다.  

   과거의 청구서 및 조정 파일을 보려면 아래쪽에서 청구 기록 행을 확장합니다.

## <a name="understanding-usage-data"></a>사용량 데이터 이해 

1. Azure 플랜은 사용량에 대한 루트 또는 최상위 컨테이너입니다. 모든 사용량은 단일 Azure 플랜에 다시 연결됩니다.

2. 플랜 내에는 하나 이상의 Azure 구독이 있습니다. 이러한 구독은 리소스 관리 및 배포에 사용되는 컨테이너입니다. 

3. 구독 내에서 리소스 그룹은 그룹 리소스에 추가됩니다. 모든 리소스는 하나의 리소스 그룹에 배포됩니다. 

4. 리소스의 예로 가상 머신 및 스토리지 계정이 있습니다. 

5. 리소스 내보내기 측정기: 측정기는 리소스의 사용량을 측정하며, 하나의 리소스에서 여러 측정기의 사용량을 내보낼 수 있습니다. 측정기는 ProductId, SKUId 및 AvailabilityId로 식별됩니다. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>구독 리소스 그룹 및 계량의 계층 구조

**Azure 계정(테넌트)**

- 구독 A
    - ResourceGroup 1
        - 가상 머신(리소스)
            - 컴퓨팅 측정기
        - 가상 네트워크(리소스)
            - 청구 측정기 없음

    - ResourceGroup 2
        - 가상 머신(리소스)
            - 컴퓨터 측정기
        - 프리미엄 SSD 관리 디스크(리소스)
            - 스토리지 용량 측정기
            - 스토리지 작업 수 측정기

- 구독 B   -ResourceGroup 1       - Azure SQL(리소스)           - DTU 측정기       - VPN Gateway(리소스)           - VPN Gateway 측정기

    - ResourceGroup 2
        - Virtual Network 인터페이스(리소스)
            - 청구 측정기 없음

## <a name="read-the-invoice"></a>청구서 읽기

1. 청구서는 매월 8일 이후에 사용할 수 있습니다.

2. 파트너는 60일 내에 결제 금액을 송금해야 합니다.

3. 청구 기간에는 지정된 달력 월(예: 10/1-10/31)이 포함됩니다.

4. 요금은 순 조정액입니다(금액은 "관리형 서비스에 대해 파트너가 획득한 순 크레딧").

5. 자세한 청구 정보는 청구서 조정 파일 및 일일 평가 사용량 파일을 검토하세요.

   :::image type="content" source="images/azure/invoice1.png" alt-text="청구서":::

## <a name="read-the-invoice-reconciliation-file"></a>청구서 조정 파일 읽기

1. 각 Azure 플랜과 측정기의 조합은 조정 파일에 최대 두 개의 청구 줄을 포함할 수 있습니다.

2. 측정기가 한 달 전체에 걸쳐 모든 유형의 할인 또는 크레딧(예: 계층화된 할인 또는 관리형 서비스에 대한 파트너 획득 크레딧)에 적합한 경우 조정 파일에는 하나의 청구 줄만 포함됩니다. **PriceAdjusmentDescription** 열은 할인 또는 획득 크레딧을 참조합니다.

3. 할인 또는 파트너 획득 크레딧에 적합한 특정 측정기에 대한 리소스가 없으면, 조정 파일에 하나의 청구 줄만 포함되며 유효 단가는 소매 가격(단가)이 됩니다.

4. 측정기 또는 해당 측정기를 내보내는 리소스가 월의 일부 동안 **관리형 서비스에 대한 파트너 획득 크레딧** 에 적합한 경우 조정 파일에는 두 줄의 청구가 포함됩니다. 하나는 미터가 자격을 획득한 날을 표시하고 다른 하나는 미터가 자격을 획득하지 못한 날을 나타냅니다.

## <a name="read-the-daily-usage-file"></a>일일 사용량 파일 읽기

- Azure 플랜 하의 구독 미터는 날마다 평가하여 누적됩니다.

- **관리형 서비스에 대한 파트너 획득 크레딧** 은 매일 확인 및 적용됩니다.

- 모든 구독 미터에는 서비스가 사용된 월의 모든 날에 대한 행이 하나 포함됩니다.

- 아래 예제를 살펴보세요.

  - 미터가 7/1 – 7/3에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).

  - 미터가 7/4 – 7/7에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득하지 못했습니다(유효 단가는 소매 가격).

  - 미터가 7/8 – 7/31에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>고객 통화로 작성된 청구서

Azure 플랜을 통한 Azure 서비스는 USD로 가격이 책정되며 고객의 국가에 할당된 통화 요금이 청구됩니다. 청구 통화가 USD가 아닌 경우 사용되는 환율은 청구서의 마지막 페이지에 표시됩니다. 환율은 매월 결정되며 다음 청구서부터 적용됩니다. 국가 통화의 전체 목록은 [최신 상거래 제품 사용 가능 국가 및 고객 통화표](https://go.microsoft.com/fwlink/?linkid=2112354)를 참조하세요.

Microsoft는 Thomson Reuters를 사용하여 가격 책정 통화를 청구 통화로 변환하는 데 사용되는 환율을 결정합니다. 환율은 적용되는 월의 첫 번째 날짜 이전에 새로 고쳐지고 사용할 수 있습니다.

**예**:  8월 1일 – 8월 31일의 서비스 기간에 대한 사용량 요금은 7월 31일에 게시된 환율을 사용하여 청구됩니다. 이 요금은 9월 청구서에 표시되며, 청구서의 마지막 페이지에 환율이 표시됩니다.

## <a name="azure-reservations"></a>Azure Reservations


Azure 플랜을 통해 [Azure 예약](azure-reservations.md)을 구매하는 경우 일회성 또는 월간 청구를 선택할 수 있습니다.


## <a name="azure-spending"></a>Azure 지출

기존의 Azure 지출 환경이 파트너 센터에서 새 Azure 플랜 청구서를 지원하도록 업데이트되었습니다. 이를 통해 파트너는 다음을 수행할 수 있습니다.

- 고객 수준에서 설정된 예산에 대한 경고 보기, 관리 및 받기 

- Azure 플랜에 대한 총 예상 지출 보기(리소스 및 측정기 수준별로 세분화됨)

Azure 플랜을 통한 Azure 서비스의 청구 모델은 후불 사용량 요금제이므로 청구 금액이 예상 금액을 초과하지 않도록 파트너는 월별 예산을 적용하고 사용률을 추적할 수 있습니다. 예산을 한 고객에게 또는 동시에 여러 고객에게 적용할 수 있습니다. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure 지출":::

## <a name="next-steps"></a>다음 단계

- PEC(파트너 획득 크레딧)를 계산하는 방법을 참조하세요. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/)에 로그인하고 사용 가능한 가격표를 찾습니다.

- [Azure 플랜 구매](purchase-azure-plan.md)에 대한 자세한 정보

- [CSP의 새로운 상거래 환경에 대한 가격표](azure-plan-price-list.md) 참조
