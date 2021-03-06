---
title: 상업용 마켓플레이스 제품에 대한 청구
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 내 상업용 Marketplace에서 고객을 위해 구매한 ISV SaaS 제품 또는 구독에 대해 청구가 작동하는 방식을 알아봅니다.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148026"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>파트너 센터 상업용 Marketplace 제품 및 구독에 대한 청구


**적절한 역할:** 전역 관리자 | 청구 관리자

CSP 프로그램의 파트너는 파트너 센터 사용하여 상업용 Marketplace의 ISV 게시자로부터 라이선스 기반 SaaS 제품을 구매할 수 있습니다. 이렇게 하면 이러한 유형의 구매에 대한 청구서에 액세스할 수 있습니다. 청구 기간은 해당 월의 첫째 날에 시작하여 해당 월의 마지막 날에 끝납니다. 청구서는 다음 달 8일에 제공됩니다.

파트너 센터 [대시보드에서](https://partner.microsoft.com/dashboard/) 또는 파트너 센터 API를 사용하여 청구서에 액세스할 수 [있습니다.](/partner-center/develop/)

CSP 프로그램의 파트너는 파트너 센터 또는 Azure Portal 제품을 구매할 때(고객의 이전 CSP 구매 Azure 테넌트 사용) 고객에게 구매한 ISV 상업용 Marketplace 솔루션에 대해 요금이 청구됩니다.

>[!NOTE]
>고객이 자신의 Azure AD 테넌트(CSP 프로그램의 파트너에서 구매하지 않음)를 사용하는 경우 고객은 ( Microsoft AppSource 또는[Azure Marketplace](https://appsource.microsoft.com/) )에서 [](https://azuremarketplace.microsoft.com/)직접 자신의 ISV SaaS 솔루션을 구매하도록 선택할 수도 있습니다. 이렇게 하면 Microsoft에서 직접 자신의 청구서를 받게 됩니다. 마찬가지로 CSP 프로그램의 파트너가 Azure 구독 또는 새 Azure 플랜을 고객에게 판매하여 고객(또는 간접 대리점)에게 해당 테넌트(읽기 권한자 외의 고객에게 역할 할당)에 [대한 역할 기반 액세스 권한을](/azure/role-based-access-control/built-in-roles) 부여하는 경우 해당 고객(또는 간접 대리점)은 CSP 파트너에게 사전 승인이나 알림 없이 상업용 Marketplace 제안을 구매할 수도 있습니다. 이러한 경우 Microsoft는 CSP 프로그램의 파트너에게 고객의 구매에 대해 직접 알리지 않습니다. 그러나 Microsoft는 Azure 구독에 대 한 작업에 대 한 알림 또는 알림을 설정 하는 데 사용할 수 있는 선택적 [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) 메커니즘을 제공 합니다.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>상용 marketplace 제품에 대 한 청구 정보 액세스

청구서를 볼 수 있게 되면 회사의 글로벌 관리자 또는 대금 청구 관리자에게 이메일을 전송됩니다. 상용 marketplace 제품 구매를 위한 최신 청구서 및 조정 파일에 액세스 하려면:

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.

2. 파트너 센터 메뉴에서 **청구** 를 선택합니다. 

    청구 페이지의 맨 위에 **되풀이** 및 **되풀이 및 일회성 구매** 라는 두 개의 탭이 표시 됩니다. 각 탭에서 여러 marketplace 제품에 대 한 정찰 (청구서 및 조정) 파일에 액세스할 수 있습니다.

    - **되풀이** 탭: Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro 및 Microsoft Azure 관련 된 구독의 청구서 및 조정 파일을 표시 합니다.

    - **되풀이 및 일회성 구매** 탭: azure 요금제, azure 예약, 소프트웨어 및 상업적 marketplace 제품에 대 한 송장 및 조정 파일이 표시 됩니다.
  
3. **되풀이 및 일회성 구매** 탭을 선택 합니다. 다른 통화로 고객에 대 한 구독을 구매한 경우 각 통화에 대 한 탭이 표시 됩니다. 이 페이지에서 몇 가지 작업을 수행할 수 있습니다.

    - 최신 청구서 및 조정 파일을 보려면 **청구서** 또는 **조정 파일** 을 선택 합니다. 원할 경우 [파트너 센터 api](/partner-center/develop/)를 사용 하 여 최신 청구서 및 정찰 파일 데이터에 액세스할 수도 있습니다.

    - 이전 청구서 및 정찰 파일을 보려면 아래 **청구 기록** 행을 확장 하십시오.

    - 최근 계정 작업을 기준으로 언제 든 지 예상 계정 잔액 또는 청구서를 확인 하려면 **견적** 제목에서 링크를 선택 합니다.  

    >[!NOTE]
    > 해당 월의 여덟 번째 날에 청구서를 게시할 때 세금 및 기타 적용 가능한 모든 요금 및 크레딧이 포함 됩니다. 즉, 최종 금액이 청구 기간 중에 표시 되는 것과 다를 수 있습니다.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>상업적 marketplace 제품에 대 한 청구서 및 정찰 파일에 대 한 자세한 정보

이 섹션에서는 타사 ISV 게시자의 고객을 위해 구매한 상용 marketplace SaaS 구독의 청구서 및 조정 파일에 대해 자세히 설명 합니다.

파트너 센터 메뉴의 **청구** 옵션에서 **되풀이 및 일회성 구매** 를 선택 하는 경우 Microsoft (자사) 및 ISV (타사) 구매와 관련 된 요금에 대 한 청구서 및 조정 파일에 액세스할 수 있습니다. 이러한 구매는 다음에 연결 될 수 있습니다.

- SaaS 구독 (Microsoft 또는 ISV 게시자)

- Azure 플랜

- Azure 예약

- 기타 구독 기반 소프트웨어 (Microsoft 또는 ISV 게시자)

이러한 구매의 예로는 SUSE Linux software (소프트웨어 구독) 또는 Azure ISV SaaS 제품 구독이 포함 될 수 있습니다.

>[!NOTE]
> 청구서 및 정찰 파일을 읽는 방법에 대 한 자세한 내용은 [청구 개요](billing.md)를 참조 하세요.

### <a name="tips-on-reading-your-invoice"></a>청구서 읽기 팁

타사 ISV 게시자 로부터 라이선스 기반 SaaS 제품을 구매 하는 경우 청구서에 대 한 라이선스 요금에 대 한 요금이 표시 됩니다. ISV의 SaaS 제품이 기본 Azure 인프라 리소스를 사용 하거나 소비 하는 경우에도 마찬가지입니다. ISV의 SaaS 제품에 대 한 고객의 Azure 인프라 사용 요금은 ISV에 직접 청구 되기 때문입니다. Isv는 자신의 Azure 사용량이 매일 등급 청구 조정 파일에 연결 된 Azure 사용량 요금을 볼 수 있습니다.

청구서에는 다음과 같은 여러 페이지가 포함 됩니다.

- **청구서의 1 페이지:** CSP 프로그램 파트너의 청구 정보에 대 한 요약 개요를 포함 합니다. 여기에는 청구 기간에 대 한 요금, 청구서 번호, 지불 약관 (순 60 일) 및 요금 청구 지불 방법에 대 한 요약 (통신 또는 확인)이 포함 됩니다.

- **청구서의 2 페이지 (및 모든 후속 페이지):** 상업적 marketplace의 자사 Microsoft 구매 및 타사 ISV (라이선스 기반) 구매에 대 한 요금을 청구 합니다. 각 제품 이름 아래의 **게시자** 줄에서 ISV 라이선스 기반 구매를 식별할 수 있습니다. 관련 조정 파일은 특정 청구서 요금에 대한 더 많은 청구 세부 정보를 제공합니다.

- **청구서의 마지막 페이지:** ISV에서 라이선스 기반 마켓플레이스 제품에 대한 요금이 청구된 경우 이 마지막 페이지에 ISV 게시자의 이름 및 주소에 대한 자세한 정보가 표시됩니다.

### <a name="tips-on-reading-your-reconciliation-file"></a>조정 파일 읽기에 대한 팁

**되풀이 및 일회성 구매** 조정 파일에는 청구서의 요금에 매핑되는 추가 세부 정보가 포함된 여러 열이 포함되어 있습니다. **PublisherName** 열에는 구매가 Microsoft인지 타사 ISV 게시자인지가 표시됩니다.

조정 파일의 일부 요금은 $0의 비용으로 표시할 수 있습니다. ISV "평가판" 제안(일반적으로 30일 또는 60일) 또는 사용자 라이선스 가져오기 제안 때문일 수 있습니다.

평가판 ISV 제안의 경우:

- 평가판 기간에는 해당 기간 동안 ISV 라이선스 기반 SaaS 제품의 비용이 포함됩니다. 또한 해당 SaaS 제품의 연결된 Azure 인프라 사용에 대해서도 요금이 청구되지 않습니다.  그러나 사용량 기반 ISV 제안을 사용하는 경우 평가판에는 기본 Azure 인프라 사용 비용이 포함되지 않습니다. 이 경우 Azure 인프라 사용 요금은 별도의 Azure 조정 파일에 표시됩니다.

- 고객을 위해 ISV의 평가판 제품을 구매하고 배포하는 경우 고객은 ISV 게시자에 의해 평가판에 자동으로 등록됩니다. 평가판 기간은 ISV 게시자가 정의한 기간이 지나면 자동으로 종료됩니다. 기간이 끝나면 고객에게 요금이 청구됩니다. 즉, 조정 파일에 평가판 적격 제품에 대한 두 개의 행이 표시될 수 있습니다. 하나는 평가 기간을 추적하고 다른 하나는 유료 제품을 추적합니다(평가 기간이 종료될 때까지 $0의 비용이 표시). 평가판이 종료되면 유료 제안을 보여주는 행이 요금을 표시하기 시작합니다. 

각 열이 나타내는 항목에 대한 자세한 내용은 [조정 파일 사용을 참조하세요.](use-the-reconciliation-files.md) 파트너 센터 [청구 유형도](./billing-basics.md) 참조하세요.

## <a name="next-steps"></a>다음 단계

- [고객을 위한 상용 마켓플레이스 제품 관리](csp-commercial-marketplace-manage.md)
- [상용 마켓플레이스 제품 지원에 대 한 자세한 정보](csp-commercial-marketplace-support.md)