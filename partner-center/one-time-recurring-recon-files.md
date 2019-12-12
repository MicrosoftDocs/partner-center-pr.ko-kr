---
title: 일회성 및 되풀이 조정 파일 | 파트너 센터
ms.topic: article
ms.date: 11/21/2019
description: 파트너 센터에서 일회성 및 되풀이 조정 파일을 이해 합니다.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 51c37c9ea2110b7666c4d1a9bc92a2b01f92209c
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004902"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>일회성 및 되풀이 조정 파일

**적용 대상**

- 파트너 센터
- Microsoft Cloud for US Government 파트너 센터

**적절한 역할**
-   전역 관리자
-   사용자 관리자
-   청구 관리자
-   관리자 에이전트
-   영업 에이전트

이 항목에서는 파트너 센터에서 일회성 및 되풀이 조정 파일을 읽는 방법에 대해 설명 합니다.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>일회성 및 되풀이 조정 파일의 필드

| Column | 설명 |
| ------ | ----------- |
| PartnerId | 특정 청구 엔터티에 대 한 고유 Azure Active Directory (Azure AD) 테 넌 트 식별자 (GUID 형식)입니다. 조정에는 필요 하지 않습니다. 모든 행에서 같습니다. |
| Customer Id | GUID 형식의 고유한 Azure AD 테 넌 트 식별자입니다. 고객을 식별합니다. |
| 고객 이름 | 파트너 센터에 보고 된 고객의 조직 이름입니다. |
| CustomerDomainName | 고객의 도메인 이름입니다. 두 번째 청구 주기가 될 때까지 이 필드는 빈 상태로 나타날 수 있습니다. *이 필드를 고객에 대 한 고유 식별자로 사용 하지 마세요. 고객/파트너는 Office 365 포털을 통해 베 니 티 또는 기본 도메인을 업데이트할 수 있습니다.* |
| 고객 국가 | 고객이 위치한 국가입니다. |
| 송장 번호 | 지정한 트랜잭션이 표시되는 송장 번호입니다. |
| MpnId | CSP 파트너의 MPN 식별자입니다. |
| 대리점 MpnId | 구독에 대 한 레코드 대리점의 MPN 식별자입니다. |
| 주문 ID | Microsoft commerce platform의 주문에 대 한 고유 식별자입니다. 조정에 사용 되지 않습니다. |
| 주문 날짜 | 주문이 이루어진 날짜입니다. |
| ProductId | 제품의 식별자입니다. |
| SkuId | 특정 SKU에 대 한 식별자입니다 (재고 유지 단위). |
| AvailabilityId | 특정 SKU의 가용성에 대 한 식별자입니다. 지정 된 국가, 통화, 산업 부문 등에서 SKU를 구매할 수 있는지 여부를 표시 합니다. |
| SKU 이름 | 특정 SKU의 제목입니다. |
| 제품 이름 | 제품 이름입니다. |
| PublisherName | 제품 게시자의 이름입니다.
| PublisherID | 특정 게시자에 대 한 고유 식별자입니다. |
| 구독 설명 | 구독의 이름입니다. |
| 구독 ID | Microsoft commerce platform의 구독에 대 한 고유 식별자입니다. 조정에 사용 되지 않습니다. *이 식별자는 파트너 관리 콘솔의 **구독 ID** 와 동일 하지 않습니다.* |
| ChargeStartDate | 요금 시작일. 시간은 항상 해당하는 날의 시작인 0:00입니다. |
| ChargeEndDate | 요금 종료일. 시간은 항상 해당 일의 마지막인 23:59입니다. |
| 용어 및 Billingcycle | 구매의 기간 및 청구 주기 (예: *1 년, 매월*). |
| 청구 유형 | 요금 또는 조정 유형입니다. |
| 단가 | 구입 시 가격 목록에 게시 된 단가입니다. *조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다.* |
| 유효 단가 | 조정을 수행한 후 단가입니다. |
| Quantity | 단위 수입니다. *조정 하는 동안 청구 시스템에 저장 된 정보와 일치 해야 합니다.* |
| 단위 형식 | 구입할 단위의 유형입니다. |
| DiscountDetails | 해당 할인에 대 한 설명입니다. |
| 하위 합계 | 세금을 적용하기 전의 총액. 할인이 예상 합계와 일치 하는지 확인 합니다. |
| 세금 합계 | 세금 금액 요금. 시장의 세금 규칙 및 특정 상황을 기준으로 합니다. |
| 총액 | 세금을 적용한 후의 총액. 송장에 세금이 부과되었는지 확인합니다. |
| Currency | 통화 형식. 각 청구 엔터티의 통화는 한 가지만 가능합니다. 첫 번째 청구서와 일치 하는지 확인 하 고 주요 청구 플랫폼 업데이트 후에 다시 확인 합니다. |
| AlternateID | **주문 ID**에 대 한 대체 식별자입니다. |
