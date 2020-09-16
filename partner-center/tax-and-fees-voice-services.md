---
title: 지역 PSTN 서비스 세금 및 수수료
description: Microsoft 365 음성 제품을 엔터티입니다 하는 Office 365 파트너는 PSTN 서비스에 대 한 지역 세금, 요금 또는 규제 요구 사항이 적용 될 수 있습니다.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "90594465"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>지역 세금, PTSN (공개 전환 전화 네트워크) 서비스에 대 한 규정

**적용 대상**

- 파트너 센터
- Office 365 파트너 거래 Microsoft 365 음성 제품

**적절한 역할**
-    글로벌 관리자
-    사용자 관리자
-    관리 에이전트

일부 관할지의 공개 PSTN (스위치 전화 네트워크) 서비스에는 파트너 주문 및 청구에 영향을 줄 수 있는 특별 한 세금 및 규정 요구 사항이 적용 될 수 있습니다. 푸에르토리코를 비롯 한 미국에서 오디오 회의, 호출 계획 및 통신 크레딧을 포함 하는 PSTN 서비스는 특별 한 세금 및 규정 요구 사항에 따라 결정 됩니다. 미국 및 푸에르토리코에서 Microsoft는 PSTN 서비스를 세금 포함으로 가격으로 포함 합니다.  고유한 PSTN 세금 및 규정은 Microsoft 365 음성 제품 거래 Office 365 파트너에 게 영향을 줍니다.  파트너가 Microsoft PSTN 서비스의 가격을 표시 하는 경우 PSTN 세금 및 수수료를 계산 하 고 remitting 하는 일을 담당할 수 있습니다.

## <a name="partner-recommendations"></a>파트너 권장 사항

세금 및 법률 자문 위원에 참여 하 여 PSTN 서비스의 규정, 세금 및 수수료, 기타 잠재적인 부채에 대 한 조직의 책임을 파악 합니다.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>송장 프레젠테이션 및 파트너 조정 파일

비즈니스 PSTN 및 Microsoft 365 음성 서비스에 대 한 Skype를 포함 하는 미국, 푸에르토리코 및 캐나다의 CSP 청구서 및 CSP 조정 파일은 PSTN 및 비-PSTN 구성 요소에 대 한 별도의 품목을 제공 합니다.

또한 CSP 청구서에는 다음 각주가 표시 됩니다.

* 표시 되는 가격은 오디오 회의 및 호출 계획 서비스에 대 한 요금이 부과 됩니다.  해당 하는 모든 트랜잭션 세금은 미국 내 판매를 제외 하 고 표시 된 금액에 대해서만 요금이 부과 됩니다.  미국에서 표시 되는 가격은 호출 계획 및 오디오 회의 서비스에 대 한 요금을 포함 하 고 있으며 요금이 부과 되어야 하는 세금 및 요금에 대 한 요금을 포함 하는 세율을 포함 합니다.  오디오 회의 및 호출 계획 서비스는 이러한 서비스를 제공 하는 Microsoft 관련 인증에 의해 처리 됩니다.  자세한 내용은 [Microsoft 볼륨 라이선싱](https://go.microsoft.com/fwlink/?LinkId=690247)을 참조하세요.

## <a name="reconciliation-file-example"></a>조정 파일 예제

Office 365 Enterprise E5는 동일한 이름 및 동일한 Id를 사용 하는 두 개의 품목으로 조정 파일을 제공 하지만 각 품목에는 고유한 단가 (예: $28.40 및 $2.00)가 있습니다. 이는 Office 365 제품의 비즈니스용 Skype PSTN 회의 구성 요소를 분리 하므로 세금을 정확 하 게 적용할 수 있습니다.

**파트너 조정 예제 #1 (열 선택):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |요금 주기   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |요금 주기   |2.00   |

**파트너 조정 예 #2**

캐나다에서 사용할 수 있는 Microsoft 365 Business 음성에는 CSP 청구서에 통합 되는 추가 PSTN taxable 구성 요소가 있습니다 (Office 365 E5와 마찬가지로, 두 개의 품목은 PSTN 구성 요소이 고 다른 하나는 비 PSTN 구성 요소에 대해 표시 됨).  Microsoft 365 Business 음성의 CSP 조정 파일은 모든 PSTN taxable 구성 요소를 개별적으로 표시 합니다. 개별 PSTN 구성 요소는 통합 되지 않습니다. CSV 또는 API 도구).  조정 파일에서 찾은 고객에 대 한 주문 정보 및 청구 금액의 합계는 CSP 청구서와 일치 하 게 됩니다.

## <a name="additional-resources"></a>추가 리소스
자세한 내용은 [파트너 사이트 Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) 를 참조 하세요.

