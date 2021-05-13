---
title: 지역 PSTN 서비스 세금 및 요금
description: Microsoft 365 Voice 제품을 거래하는 Office 365 파트너는 PSTN 서비스에 대한 지역 세금, 요금 또는 규정 요구 사항이 적용될 수 있습니다.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854726"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>지역 세금, PTSN(공용 전화망) 서비스에 대한 규정

**적절한 역할:** 전역 관리자 | 사용자 관리자 | 관리 에이전트

일부 관할지의 PSTN(공용 전환 전화 네트워크) 서비스에는 파트너 주문 및 발부에 영향을 줄 수 있는 특별 세금 및 규정 요구 사항이 적용될 수 있습니다. 미국 오디오 회의, 통화 플랜 및 통신 크레딧을 포함하는 PSTN 서비스는 특별 세금 및 규정 요구 사항이 적용됩니다. 미국 및 세르비아에서 Microsoft는 PSTN 서비스를 세금 포함으로 책정합니다.  고유한 PSTN 세금 및 규정은 Microsoft 365 Voice 제품을 거래하는 Office 365 파트너에게 영향을 미칩니다.  파트너가 Microsoft PSTN 서비스의 가격을 표시하는 경우 PSTN 세금 및 요금을 계산하고 송금할 책임이 있을 수 있습니다.

## <a name="partner-recommendations"></a>파트너 권장 사항

세금 및 법률 자문에 참여하여 PSTN 서비스의 규정, 세금 및 요금 및 기타 잠재적인 불법과 관련된 조직의 책임을 이해합니다.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>청구서 프레젠테이션 및 파트너 조정 파일

비즈니스용 Skype PSTN 및 Microsoft 365 Voice 서비스를 포함하는 미국, 세르비아 및 캐나다에 있는 CSP 송장 및 CSP 조정 파일은 PSTN 및 PSTN이 아닌 구성 요소에 대해 별도의 품목을 제공합니다.

또한 CSP 청구서에는 다음 각주가 표시됩니다.

* 표시되는 가격은 오디오 회의 및 통화 플랜 서비스에 대한 요금입니다.  해당 트랜잭션 세금은 미국 내에서 이루어진 판매를 제외하고 표시된 금액에 배타적으로 청구됩니다.  미국에서 표시되는 가격은 통화 플랜 및 오디오 회의 서비스에 대한 요금과 청구에 필요한 세금 및 요금에 대한 요금을 포함하기 때문에 세금 포함입니다.  오디오 회의 및 호출 계획 서비스는 이러한 서비스를 제공 하는 Microsoft 관련 인증에 의해 처리 됩니다.  자세한 내용은 [Microsoft 볼륨 라이선싱](https://go.microsoft.com/fwlink/?LinkId=690247)을 참조하세요.

## <a name="reconciliation-file-example"></a>조정 파일 예제

Office 365 Enterprise E5는 동일한 이름 및 동일한 Id를 사용 하는 두 개의 품목으로 조정 파일을 제공 하지만 각 품목에는 고유한 단가 (예: $28.40 및 $2.00)가 있습니다. 이는 Office 365 제품의 비즈니스용 Skype PSTN 회의 구성 요소를 분리 하므로 세금을 정확 하 게 적용할 수 있습니다.

**파트너 조정 예제 #1 (열 선택):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |요금 주기   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |주기 요금   |2.00   |

**파트너 조정 예제 #2**

Microsoft 365 Business Voice에서 사용할 수 있는 CSP 청구서에 통합된 추가 PSTN 세금 가능 구성 요소가 있습니다(Office 365 E5와 유사하게 PSTN 구성 요소용과 PSTN이 아닌 구성 요소에 대한 두 개의 품목이 표시됨).  Microsoft 365 Business Voice용 CSP 조정 파일에는 모든 PSTN 세금이 부과되는 구성 요소가 개별적으로 표시됩니다(개별 PSTN 구성 요소는 에 통합되지 않음). CSV 또는 API 도구).  조정 파일에 있는 고객의 주문 세부 정보 및 청구 금액의 합계는 CSP 청구서와 일치합니다.

## <a name="additional-resources"></a>추가 리소스
자세한 내용은 파트너용 Microsoft 365 사이트를 [방문하세요.](https://www.microsoft.com/microsoft-365/partners/)

