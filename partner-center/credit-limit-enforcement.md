---
title: 신용 한도 적용
ms.topic: how-to
ms.date: 05/11/2021
description: 신용 한도 및 계산 방법에 대해 알아보세요. FAQ를 포함 합니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148111"
---
# <a name="credit-limit-enforcement-cle"></a>신용 한도 적용 (CLE)

**적절 한 역할**: 대금 청구 관리자

## <a name="your-credit-limit-and-how-it-works"></a>신용 한도 및 작동 방식

신용 한도는 파트너 센터에서 제품이 나 구독을 구매 하는 데 사용할 수 있는 최대 금액 (미국 달러)입니다. 신용 한도를 초과 하는 경우에는 충분 한 지불이 완료 될 때까지 새로운 구매를 수행할 수 없습니다. 기존 구독은 중단 없이 계속 됩니다.

크레딧 제한은 Azure 계획, Azure 예약, 소프트웨어, Marketplace, Azure 145 P, Office 및 Dynamics 제품의 제안에 적용 됩니다. 신용 한도는 갱신 및 진행 중인 소비에는 적용 되지 않습니다.

온 보 딩 기간 동안에는 테 넌 트 수준에서 신용 한도를 할당 합니다. 예측 수익, 구매 prowess 및 지불 기록을 기반으로 합니다. 그런 다음, 다음 수식을 사용 하 여 사용 가능한 잔액을 계산 합니다.

**[크레딧 한도 – (수신 구매 + 미결 미지불 청구서 + 청구 되지 않은 요금-과잉 지불)]**

## <a name="frequently-asked-questions"></a>질문과 대답

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>내 크레딧 한도가 테 넌 트 또는 글로벌 수준에서 설정 되나요?

테 넌 트 수준입니다. 예를 들어 미국, 캐나다 및 일본에서 작업 한다고 가정 합니다. 캐나다 테 넌 트가 신용 한도에 도달 하면 파트너 센터에서 구매 하려고 할 때 해당 테 넌 트가 알림을 받게 됩니다. 다른 테 넌 트는 영향을 받지 않습니다. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>내 신용 한도를 초과 하는 경우 모든 권한으로 기존 고객 및 구독 서비스를 계속 제공할 수 있나요?

예. 고객의 기존 구독은 중단 없이 계속됩니다. 그러나 고객에 대한 새 구독은 구입할 수 없습니다.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>직접 청구 파트너 및 간접 공급자 모두에 대한 CLE가 적용됩니까?

예, 둘 다에 적용됩니다.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>내 계정을 복구하기 위해 지급액을 제출한 후 언제 더 많은 구독을 구매할 수 있나요? 

Microsoft가 신용 조회 프로세스를 진행하기 위한 모든 요구 사항을 수신했다고 가정하면 결제 후 24시간 이내에 구매를 다시 시작할 수 있어야 합니다.

### <a name="how-can-i-check-my-credit-limit"></a>크레딧 한도를 확인하려면 어떻게 해야 합니까?

[ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com)크레딧 한도를 확인하고 최근 구매에 대한 정보를 얻으려면 에 문의하세요.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>분쟁에 있는 청구서는 신용 한도에 대해 계산합니까?

예. 그러나 에서 Microsoft에 문의하여 문제를 해결할 수 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 있습니다.

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>에 쓰면 얼마나 빨리 다시 들 수 ucmwrcsp@microsoft.com 있나요?

24시간 이내에 응답이 있어야 합니다. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Microsoft는 파트너의 크레딧 한도를 설정하는 데 어떤 기준을 사용하나요?

예상 수익, 구매 장점 및 지불 내역에 따라 크레딧 한도를 결정합니다.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>신용 한도가 현재 새 상거래 경험에 적용되고 있나요?

예. 크레딧 한도는 파트너 센터 모든 CSP 프로그램 및 제품에 적용됩니다.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>조직에서 크레딧 한도에 근접할 때 알림을 받는 사람은 누구인가요?

조직의 재무 계정 지불 가능 연락처가 알림을 받아야 합니다.

## <a name="next-steps"></a>다음 단계

[청구 기본 사항](./billing-basics.md)
