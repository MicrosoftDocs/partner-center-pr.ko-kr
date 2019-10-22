---
title: Azure 플랜 - 청구 | 파트너 센터
ms.topic: article
ms.date: 10/04/2019
description: 청구서 및 조정 파일 구조에 대해 설명
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171296"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP의 새로운 상거래 환경 - Azure 청구 

Azure 플랜 하에서는 잘 조정된 단일 청구 날짜와 월 기반 청구 기간을 사용하여 간편하게 청구할 수 있습니다. 청구 플랫폼에 대한 자세한 내용은 [파트너 센터 최신 상거래 운영 가이드](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)를 참조하세요.

## <a name="summary-of-billing-essentials"></a>청구 기본 정보 요약

- **청구서 날짜**: 청구서 및 조정 파일은 8일(UTC 자정)에 파트너 센터 대시보드/API에서 사용할 수 있습니다.

- **청구서 청구 기간**: 청구서 청구 기간은 달력의 월을 기준으로 조정됩니다(예: 10/1-10/31, 11/1-11/30).

- **서비스 기간 요금 청구**: 요금은 달력의 월을 기준으로 조정됩니다. 예를 들어 청구 파트너가 10/15에 Azure 플랜을 통해 Azure 서비스를 추가하고 고객이 10/15에 Azure 서비스 사용을 시작하는 경우 청구 파트너는 서비스 기간 10/15 - 10/31에 고객이 사용한 요금에 대한 청구서/조정 파일을 11/8에 받게 됩니다. 12/8에 생성될 다음 달 청구서에는 서비스 기간 11/1 - 11/31의 모든 요금이 포함됩니다.

- **청구서 결제 기간**: 순 60일.

- **청구서 통화** : 파트너는 고객의 국가에 할당된 통화로 계속 요금이 청구됩니다. 예를 들어 청구 파트너가 아일랜드에 있고 고객은 영국, 노르웨이 및 독일에 있는 경우 청구 파트너는 GBP, NOK 및 EUR 청구서/조정 파일을 받습니다.

- **파트너 인센티브**: 청구 월이 끝나고 45일 후에 결제됩니다.

##  <a name="access-your-invoices-and-recon-files"></a>청구서 및 조정 파일 액세스

청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다. 

**청구서 및 조정 파일에 액세스하려면**

1. 파트너 센터에 로그인합니다.

2. 파트너 센터 메뉴에서 **청구**를 선택합니다.

3. 원하는 **달력 기반**  및 통화에 대한 탭을 선택합니다.

![청구](images/azure/billing1.png)

4. **청구서 및 조정 파일**을 선택합니다.  

과거의 청구서 및 조정 파일을 보려면 아래쪽에서 청구 기록 행을 확장합니다.

## <a name="read-the-invoice"></a>청구서 읽기

1. 청구서는 매월 8일 이후에 사용할 수 있습니다.

2. 파트너는 60일 내에 결제 금액을 송금해야 합니다.

3. 청구 기간에는 지정된 달력 월(예: 10/1-10/31)이 포함됩니다.

4. 요금은 순 조정액입니다(금액은 "관리형 서비스에 대해 파트너가 획득한 순 크레딧").

5. 자세한 청구 정보는 청구서 조정 파일 및 일일 평가 사용량 파일을 검토하세요.

![청구서](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a>조정 파일 읽기

1. 각 Azure 구독 미터의 조정 파일에 최대 2개의 청구 항목이 있을 수 있습니다.

2. 미터가 월 전체에 걸쳐 할인 또는 크레딧 자격을 획득한 경우(예: 계층 1 할인 또는 관리형 서비스에 대한 파트너 획득 크레딧) 조정 파일에는 청구 항목이 하나만 포함됩니다. **PriceAdjusmentDescription** 열은 할인 또는 획득한 크레딧을 참조합니다. 유효 단가는 소매 가격에서 파트너가 획득한 크레딧 또는 기타 할인을 뺀 금액입니다.

3. 미터가 월 전체에 걸쳐 관리형 서비스에 대한 파트너 획득 크레딧 자격을 얻지 못하면 조정 파일에는 청구 항목이 하나만 포함되고 유효 단가는 소매 가격(단가)이 됩니다.

4. 미터가 월의 일부 기간에 대해 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득한 경우에는 조정 파일에 두 개의 청구 항목이 포함됩니다. 하나는 미터가 자격을 획득한 날을 표시하고 다른 하나는 미터가 자격을 획득하지 못한 날을 나타냅니다. 

## <a name="read-the-daily-usage-file"></a>일일 사용량 파일 읽기

- Azure 플랜 하의 구독 미터는 날마다 평가하여 누적됩니다. 

- **관리형 서비스에 대한 파트너 획득 크레딧**은 매일 확인 및 적용됩니다.

- 모든 구독 미터에는 서비스가 사용된 월의 모든 날에 대한 행이 하나 포함됩니다.

- 아래 예제를 살펴보세요.

  - 미터가 7/1 – 7/3에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).

   - 미터가 7/4 – 7/7에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득하지 못했습니다(유효 단가는 소매 가격).

    - 미터가 7/8 – 7/31에 **관리형 서비스에 대한 파트너 획득 크레딧** 자격을 획득했습니다(유효 단가는 소매 가격에서 파트너 획득 크레딧을 뺀 가격).

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a>고객 통화로 작성된 청구서 

Azure 플랜을 통한 Azure 서비스는 USD로 가격이 책정되며 고객의 국가에 할당된 통화 요금이 청구됩니다. 청구 통화가 USD가 아니면 사용되는 환율이 청구서의 마지막 페이지에 표시됩니다. 환율은 매월 결정되며 다음 청구서부터 적용됩니다. 국가 통화의 전체 목록은 [최신 상거래 제품 사용 가능 국가 및 고객 통화표](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V)를 참조하세요. 

Microsoft는 [톰슨 로이터](https://developers.thomsonreuters.com/content/wm-company)의 환율을 사용하여 청구서 통화 전환에 사용할 가격 책정 통화를 결정합니다. 환율은 매월 1일의 전날에 갱신되어 1일부터 적용됩니다.

**예**:  서비스 기간 8월 1일 – 8월 31일의 사용 요금은 8월 1일에 게시된 환율로 청구됩니다. 이 요금은 9월 청구서에 표시되며, 청구서의 마지막 페이지에 환율이 표시됩니다. 

파트너 테넌트 사용자는 청구 통화에 관계없이 모든 고객과 모든 주문에 대한 역할 관련 정보를 계속 볼 수 있습니다. 또한 사용자는 모든 청구서를 모든 통화로 볼 수 있습니다.  
 
## <a name="azure-reservations"></a>Azure Reservations 

Azure 플랜을 통해 [Azure 예약](https://docs.microsoft.com/partner-center/azure-reservations)을 구매하는 경우 파트너 센터에서 일회성 청구를 선택할 수 있습니다. 월별 청구는 Azure Portal에서 사용할 수 있습니다. 파트너 센터에서도 향후 월별 청구를 제공할 예정입니다. 

## <a name="azure-cost-management"></a>Azure Cost Management 

조직에서는 Azure Cost Management 도구를 사용하여 Microsoft Azure의 비용을 시각화하고 관리하고 최적화할 수 있습니다. 이 기능은 Azure Portal에서 사용할 수 있습니다. 파트너는 다음과 같은 기능을 제공하는 상시 사용 가능하고 대기 시간이 짧은 솔루션을 사용할 수 있게 될 것입니다. 

- 풍부한 분석 및 예산 경고 
- API 및 Power BI 커넥터 
- 다중 고객 보기 
- 무료로 Azure 비용 관리 
- 역할/사용자 확장 

이 기능에 대한 자세한 내용은 2019년 2월부터 기업 계약에 사용할 수 있게 된 [Azure Cost Management](https://azure.microsoft.com/services/cost-management)를 참조하세요. 이 도구는 CSP에서 새 Azure 상거래 환경의 일부로 구매한 Azure 서비스에만 제공됩니다. 
 
## <a name="azure-spending"></a>Azure 지출 

조만간 CSP의 새로운 상거래 환경을 위한 파트너 센터에서 Azure 지출 도구를 사용할 수 있습니다. 이 기능이 적용되면 파트너는 다음 정보를 볼 수 있습니다.  

- 고객의 총 예산 
- 기존 Azure 플랜의 총 예상 지출 
- 각 청구 기간의 고객 사용 백분율 

Azure 플랜을 통한 Azure 서비스의 청구 모델은 종량제이므로, 청구 금액이 예상을 초과하지 않도록 파트너는 월별 예산을 적용하고 사용량 비율을 추적할 수 있습니다. 예산을 한 고객에게 또는 동시에 여러 고객에게 적용할 수 있습니다. 

![Azure 지출](images/azure/azurespend.png)

**자세한 내용**

-  PEC(파트너 획득 크레딧) 계산 방식은 파트너 센터 대시보드를 통해 사용할 수 있는 가격표에서 확인할 수 있습니다. 
   
-  [Azure 플랜 구매](purchase-azure-plan.md)

-  [CSP의 새로운 상거래 환경에 대한 가격표](azure-plan-price-list.md)
