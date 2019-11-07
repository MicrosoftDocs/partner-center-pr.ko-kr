---
title: 미결제, 사기 또는 오용 | 파트너 센터
ms.topic: article
ms.date: 10/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객의 제품 및 서비스 미결제와 부정한 활동 또는 오용을 포함하여 온라인 트랜잭션의 위험을 관리하기 위한 전략입니다.
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: 사기, 오용, 사용 제한, 사용 제한 정책, 고객이 대금을 지불하지 않은 경우, 온라인 위험, 서비스 도용, 서비스 남용, 구독 일시 중단
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 4cda8426d29fd2bf290cac2d7478bcb08641c5c3
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652971"
---
# <a name="non-payment-fraud-or-misuse"></a>미결제, 사기 또는 오용

**적용 대상**

-  파트너 센터
-  Microsoft Cloud for US Government 파트너 센터



사용자는 귀하의 고객에 의한 사기성 구매 및/또는 구매한 서비스에 대한 고객의 미결제에 대해 재정적인 책임을 집니다. 그러므로 사기 예방 및 검색 위험 완화 제어 기능을 구현하는 것이 좋습니다.

## <a name="types-of-online-risk"></a>온라인 위험의 유형

사기성 활동 또는 남용을 방지 또는/및 처리하기 위해 잠재적인 위험을 이해하고 노출의 줄일 수 있는 정책과 모범 사례를 구축하는 것이 중요합니다.

#### <a name="risk-exposure-to-be-mitigated"></a>완화해야 할 위험 노출

- **서비스의 도용** 고객이 도난된 결제 방법을 사용하거나, 거짓 결제 정보를 제공하거나, 또는 미결제 잔액을 지불하지 않음으로 인해 사용한 서비스에 대한 대가를 지불할 의도가 없는 경우

- **서비스 남용** Microsoft의 적절 한 사용 정책을 위반 하 여 클라우드 서비스를 사용 하는 고객

#### <a name="examples-of-possible-fraud-or-service-abuse"></a>가능한 사기 또는 남용 서비스의 예
- 스팸
- 해킹
- DDOS 공격
- 비트코인 마이닝
- 맬웨어 배포
- 불법 복제 구독 재판매 

#### <a name="examples-of-online-transaction-risk"></a>온라인 트랜잭션 위험의 예
- "신용 카드 없는" 거래. 즉, 직접 거래가 발생하지 않음
- 잘못된 신원
- 초기 결제 이전에 제공 및 사용된 서비스를 받음
- 신흥 온라인 사기 위험 시장/고위험 지역
- 범죄자가 계정 생성 및 구매를 자동화할 수 있도록 하는 기능

## <a name="strategies-for-managing-online-risk"></a>온라인 위험 관리 전략

이러한 권장 사항은 고객과의 관계 수명주기 전체에서 온라인 트랜잭션 위험에 대한 노출을 줄일 수 있는 정책 및 모범 사례를 개발하는 데 도움이 됩니다.  

#### <a name="when-onboarding-new-customers"></a>새 고객을 유치할 때
- 가능한 경우 전화와 같은 연락처를 사용하여 고객과 개인적인 관계 설립
- 고객의 자격 증명 및 배경을 확인할 보다 나은 방법 모색(신용 조사 기관/비즈니스 상용 보고서 기관) 
- 로봇 계정 생성 및 구매에 대한 노출을 최소화하기 위해 등록 시 SMS 인증을 사용
- 디지털 ID 서비스와 같은 서비스를 사용하여 ID 관리 및 추적
- 고객의 금융 상태를 평가하는 엄격한 신용 카드 사기 탐지 시스템
- 컬렉션 처리 및 구독에 대한 액세스에 영향을 미치는 경우를 상기한 뚜렷한 컬렉션 정책 수립(미결제에 대해 액세스를 비활성화하거나 [고객의 구독을 일시 중단](suspend-a-subscription.md)할 수 있음)

#### <a name="post-purchase-customer-account-management"></a>구매 후 고객 계정 관리
- 고객과 협력하여 적절한 모니터링 임계값을 설정하는 동시에 클라우드 사용 비즈니스 요구를 이해
    > [!NOTE]  
    >  파트너 센터에서 [월별 Azure 지출 예산을 설정](set-an-azure-spending-budget-for-your-customers.md) 하 여 해당 월에 고객 사용량을 모니터링 하 고 고객이 예산에 근접 한 경우 통보 받을 수 있습니다.
- [고객 활동 로그](activity-logs.md)를 정기적으로 모니터링하여 초기에 사기를 감지
- 의심스러운 활동이 감지되면 빠른 초치 시행
- 위험 완화 컨트롤을 구현하지 않은 경우 고객에게 구독에 대한 전체 관리자 액세스 권한을 부여하지 않도록 함
- Microsoft 알림을 신속하게 받고, 검토하고, 이에 응답하고 조치를 취하는 프로세스를 구현

#### <a name="post-purchase-customer-billing-management"></a>구매 후 고객 청구 관리
- 처음 거래 및 청구 전에 예약 결제 요청 
- 위험한 결제 기기(예: 선불 또는 가치 저장 카드)를 받지 않음
- 고객 결제 및 오래된 계정 미수금을 받을 수 있는지 모니터링하고 늦은 결제 또는 미결제에 대한 표준화된 재촉 프로세스를 적극적으로 적용

온라인 위험을 완화하는 전략에 대한 자세한 내용은 [온라인 트랜잭션 위험 관리 가이드](https://assets.windowsphone.com/7d885238-e13b-4f10-a682-3d5adacd2859/CSP-PartnerRiskGuide-APSFinal_InvariantCulture_Default.zip)를 참조하세요.

> [!IMPORTANT]  
> Microsoft에서 사용 제한 정책의 위반을 확인하거나 의심하는 파트너 또는 고객 활동을 감지한 경우 적용 단계를 진행합니다. 고객 활동은 즉시 일시 중단될 수 있습니다. 또한 요청 시 Microsoft에서 적용 작업에 대해 알리거나 업데이트할 수 있습니다.

 보안 및 multi-factor authentication에 대 한 자세한 내용은 [파트너 보안 요구 사항](partner-security-requirements.md) 을 참조 하세요.

 



