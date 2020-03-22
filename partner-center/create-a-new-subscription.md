---
title: 고객 구독 만들기, 일시 중단, 또는 취소 | 파트너 센터
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 고객 레코드를 만든 후 카탈로그의 제품에 고객 구독을 판매 하는 방법에 대해 알아봅니다.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
Keywords: 구독, 새로 만들기, 구독 추가, 일시 중단, 취소, 일시 중단, 일시 중단, SaaS, 라이선스, ISV, 타사
ms.localizationpriority: medium
ms.openlocfilehash: 05df57bc744263fd0bbd0eb52411a6e9368926f4
ms.sourcegitcommit: 36b8242cc8c47ed36d16f86338a075080c2441e1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/21/2020
ms.locfileid: "80114995"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>고객 구독 만들기, 일시 중단 또는 취소

**적용 대상**

-  파트너 센터
-  Microsoft Cloud for US Government 파트너 센터
-  CSP 파트너

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 글로벌 관리자
- 기술 지원팀 상담원
- 영업 상담원

파트너 센터에서 고객 기록을 만들면 카탈로그에서 제품의 구독을 판매할 수 있습니다. 여기에는 타사 Isv (독립 소프트웨어 공급 업체)가 [상업적 marketplace](https://azuremarketplace.microsoft.com/marketplace)에 게시 한 SaaS (Software As a Service) 제품 뿐만 아니라 Microsoft에서 게시 한 제품이 포함 됩니다. 

일부 제품은 고객당 구독 하나로 제한됩니다. 제한되는 제품 목록을 보려면 파트너 센터 가격 책정 및 제품 페이지를 방문하세요.

>[!IMPORTANT]
CSP 프로그램의 파트너는 파트너 센터 내에서 ISV 게시자의 **라이선스 기반** SaaS 구독만 구매할 수 있습니다. 즉, 사용자가 액세스할 수 있는 [전용 제품](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 을 비롯 하 여 ISV 게시자가 사용할 수 있도록 설정한 모든 **라이선스 기반** SaaS 제품을 구매할 수 있습니다. Isv (Azure 응용 프로그램, 컨테이너 또는 Vm과 관련 된 **사용량 기반**, 요금제 또는 소비 기반 제품)에서 기타 상업적 marketplace 제품을 구매 하거나 관리 하려면 [azure 관리 포털](https://portal.azure.com/)로 이동 해야 합니다. 자세한 내용은 [상용 마켓플레이스 제품 구매](csp-commercial-marketplace-purchase.md)를 참조 하세요.

## <a name="create-a-new-subscription"></a>새 구독 만들기

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. **구독 추가**를 선택합니다. **온라인 서비스** 탭에는 사용 가능한 Marketplace SaaS 제품이 모두 표시 됩니다.

4. 특정 유형의 구독만 표시하려면 사용 가능한 필터 중에서 원하는 필터를 선택합니다.
   - **게시자** **: microsoft를 선택 하** 여 isv가 게시 한 상용 마켓플레이스 **제품을 볼 수 있습니다** .
   - **청구 유형**: 사용 하려는 구독 청구 유형 ( **라이선스** 또는 **사용**)을 선택 합니다. 월간 청구 주기와 연간 청구 주기 중 어떤 것을 선택할지 결정할 때 도움이 되는 정보는 [새 청구 기능에 대한 FAQ](faq-about-new-billing-features.md)를 참조하세요.
   - **범주**: **Enterprise**, **Small business**또는 **평가판**을 선택 합니다. 평가판 구독에 대한 자세한 내용은 [고객에게 Microsoft 제품의 평가판 제공](offer-your-customers-trials-of-microsoft-products.md)을 참조하세요.

5. 고객을 위해 구매할 제품 구독을 선택 합니다. 표시 되는 제품은 고객 부문 유형 (교육, 정부 등) 및 적용 한 필터에 따라 달라 집니다. Marketplace에 표시 된 일부 제안은 특정 고객 또는 특정 CSP 파트너에 게 제공 되지 않을 수 있습니다. 이는 다음과 같은 경우에 발생할 수 있습니다.

    - 고객은 이미 해당 제품에 대 한 구독을 보유 하 고 있으며 하나만 허용 됩니다.

    - 고객의 구독이 일시 중단 되었을 수 있습니다 .이 경우에는 새 구독을 구입 하는 대신 구독을 다시 활성화할 수 있습니다.
    
    - ISV SaaS 제품의 경우 제품을 구매할 수 없는 몇 가지 이유가 있을 수 있습니다. ISV는 고객의 청구 국가 또는 지역을 지원 하지 않을 수 있습니다. ISV는 CSP 프로그램을 통해 제공 서비스를 제공 하지 않도록 선택할 수 있습니다. 또는 ISV는 특정 CSP 파트너 [에게만 제공 되는 제품을 만들](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 수 있습니다. ISV 제품은 파트너 센터 (예: 컨테이너 또는 몇 가지 사용량 기반 제품)를 통해 불가능 않을 수도 있습니다.  

6. 추가 하려는 각 구독에 대해 라이선스 수 (필요한 경우)를 입력 하 고 **카트에 추가를**선택 합니다.

7. 구독 추가가 완료 되 면 **검토** 를 선택 하 고 주문을 검토 합니다.

8. 주문을 검토 하 고 이러한 구독을 구매할 준비가 되 면 **구매**를 선택 합니다.

9. 고객에 대 한 구독을 구매한 후에는 다음이 발생 합니다.

    - 해당 고객의 **구독** 페이지에서 구독 이름을 선택 하 여 구독을 검토 하거나 편집할 수 있습니다. 여기에서 사용 가능한 경우 추가 기능 라이선스를 선택하거나, 라이선스 수를 변경하거나, 구독을 일시 중단할 수 있습니다.

    **ISV SaaS (라이선스 기반) 구독의 경우:**
    - ISV 게시자 사이트에 대 한 링크를 받게 됩니다. 이 링크를 통해 고객 구독의 배포 또는 계정 설정을 완료할 수 있습니다. (이 유형의 ISV 구독에 대 한 계정 설정/프로 비전을 완료 하는 지침이 포함 된 전자 메일을 받는 사용자와 고객 모두에 게 제공 되지 않습니다.)
    
    - 구독에 30 일 무료 평가판이 제공 되는 경우 무료 평가판 기간이 자동으로 적용 됩니다. CSP 프로그램의 파트너는 고객을 위해 구매한 제품에 대 한 무료 평가판 기간을 되지 않으며 수 없습니다. 무료 평가판 기간이 종료 되 면 구독 기간이 시작 되 고 구독이 유료으로 변환 됩니다. 그러면 구독은 동일한 일정에 따라 자동 갱신 됩니다.

## <a name="suspend-or-cancel-a-subscription"></a>구독 일시 중단 또는 취소

고객의 요청이 있거나 사기 또는 미결제 발생 시 파트너는 구독을 일시 중단하거나 취소할 수 있습니다.

### <a name="suspend-a-subscription"></a>구독 일시 중단

구독 상태를 **일시 중단됨**으로 변경하면 사용자가 로그인하거나 서비스에 액세스할 수 없습니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 관리할 구독을 선택합니다.

4. **상태** 섹션에서 **일시 중단**을 선택합니다. 그런 다음 변경 내용을 **제출**합니다.

5. 90일 이내에 또는 90일에 계정이 개설된 시간과 첫 번째 청구 기간 사이의 일 수를 더한 기간(최대 120일) 이내에 구독을 다시 활성화하지 않으면 모든 데이터가 삭제됩니다.

구독을 일시 중단할 경우, **일시 중단** 버튼 아래에 표시된 날짜는 구독을 다시 활성화하지 않을 경우 자동으로 구독이 만료되는 시점을 나타냅니다. 자세한 내용은 [새로운 청구 기능에 대 한 FAQ](faq-about-new-billing-features.md)를 참조 하세요.

### <a name="cancel-a-subscription"></a>구독 취소

파트너 센터 [상업적 marketplace](csp-commercial-marketplace-overview.md)내에서 타사 ISV 게시자의 라이선스 기반 SaaS 구독을 취소 하는 옵션이 있습니다. 취소 기간 내에 취소 하는 동안에는 전체 환불을 받을 수 있습니다.

매월 청구 되는 ISV 제품의 경우:

- 주문을 넣은 후 24 시간 이내에 취소 하면 다음 청구서에 전체 크레딧을 받게 됩니다.

- 주문을 넣은 후 24 시간 이상 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.

매년 청구 되는 제품의 경우:

- 주문을 입력 한 후 14 일 이내에 취소 하면 다음 청구서에서 전체 크레딧을 받게 됩니다.

- 주문을 입력 한 후 14 일이 지난 후에 취소 하면 갱신 시 취소가 발생 하도록 예약 됩니다.

이러한 기간이 끝난 후에는 구독을 취소 하는 옵션이 더 이상 표시 되지 않습니다.

> [!NOTE]
> 사용량 기반 및 요금제로, 가상 컴퓨터 또는 컨테이너를 사용 하는 타사 ISV 서비스는 반환 대상이 아닙니다. 사용 빈도 기반 서비스를 취소 메서드로 프로 비전 해제할 수 있습니다. 요금 청구는 사용 후 청구 되므로 이러한 서비스는 환불을 받을 수 없습니다.

ISV 게시자에서 라이선스 기반 SaaS 구독을 취소 하려면 다음을 수행 합니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 취소 하려는 구독을 찾습니다.

4. **상태** 열에서 **취소**를 선택 합니다. 그런 다음 변경 내용을 **제출**합니다.

5. 대화 상자가 표시 되 면 관련 세부 정보를 입력 한 다음 **제출**을 선택 합니다.

6. 취소를 확인 하려면 **예, 취소**를 선택 합니다.

> [!NOTE]
> Api를 사용 하 여 Azure Marketplace 구독을 취소 하도록 선택할 수도 있습니다. 이렇게 하려면 [Azure Marketplace 구독 취소](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)를 참조 하세요.

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>상업용 마켓플레이스 구독을 자동으로 갱신할지 선택

기본적으로 활성 구독은 구독 기간이 만료되면 자동으로 갱신되도록 설정됩니다. [상업용 마켓플레이스 제품 구독](csp-commercial-marketplace-overview.md)의 경우 필요에 따라 구독을 자동으로 갱신하지 않도록 선택할 수 있습니다.

활성 상업적 marketplace 구독이 자동으로 갱신 되지 않도록 하려면 다음을 수행 합니다.

1. 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3.  **구독**을 선택 합니다. 고객에 대해 구매한 라이선스 기반 구독을 나열 합니다.

4.  **구독** 열에서 수정 하려는 구독을 선택 합니다.

5. 구독 정보 페이지에서 **상태** 섹션을 찾고 **자동 갱신** 확인란의 선택을 취소 합니다. 

6. **제출**을 선택합니다.

## <a name="see-also"></a>참고 항목

- [고객을 위한 상용 마켓플레이스 제품 구매](csp-commercial-marketplace-purchase.md)
- [고객을 위한 상업적 마켓플레이스 제품 관리](csp-commercial-marketplace-manage.md)
- [상용 마켓플레이스 개요](csp-commercial-marketplace-overview.md)


