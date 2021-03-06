---
title: Azure Portal에서 SaaS 제품을 구매 하는 방법
description: Azure Portal에서 SaaS 제품을 찾고 구입 하는 방법에 대해 알아봅니다.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221443"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Azure Portal에서 SaaS 제품 구매

이 문서에서는 Azure Portal에서 SaaS (software as a service) 제품을 검색, 시도 및 구매 하기 위한 다양 한 옵션 및 요구 사항에 대해 설명 합니다.

## <a name="create-a-saas-subscription"></a>SaaS 구독 만들기

SaaS 구독을 구매 하려면 적절 한 Azure 구독에 대 한 액세스 권한이 있는 Azure 사용자 계정이 필요 합니다. 이 구독은 대금 청구 뿐만 아니라 구매한 클라우드 리소스를 compartmentalization 하는 데 사용 됩니다. Azure 구독에 대해 자세히 알아보려면 [추가 azure 구독 만들기](/azure/cost-management-billing/manage/create-subscription)를 참조 하세요.

Azure Portal의 **Marketplace** 섹션에서 원하는 SaaS 제품을 선택 합니다.

Software as a Service 구독은 개별 컴퓨터에 로컬로 설치 하는 대신 온라인 구독을 통해 지정 된 시간 동안 서비스를 사용할 수 있는 권한을 제공 합니다. 구독은 하나 이상의 클라우드 플랫폼 또는 서비스를 사용 하는 규약으로, 사용자 당 라이선스 요금 또는 클라우드 기반 리소스 사용량을 기준으로 요금이 청구 됩니다. 조직에는 여러 SaaS 구독이 있을 수 있습니다.

SaaS 구독에 대 한 제한 사항은 다음과 같습니다.

- 학생 구독 없음.
- Visual Studio Enterprise 구독이 없습니다.
- 무료 크레딧 구독은 없습니다.
- 유료 제품의 경우 결제 수단이 필요 합니다.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS는 Azure Portal에서 검색을 제공 합니다.

Azure Portal 되 면 SaaS 제품에 초점을 맞추기 위해 검색 범위를 좁힐 수 있는 몇 가지 방법이 있습니다.

### <a name="narrowing-your-search"></a>검색 범위 좁히기

홈페이지의 **Azure 서비스** 에서 **+ 리소스** 또는 **Marketplace** 만들기를 선택 합니다. 또는 플랫폼의 모든 위치에서 바로 가기 **G + N** 을 사용 합니다.

- **제품 유형** 필터를 사용 하 고 **saas** 를 선택 하 여 saas 제품으로 결과 범위를 좁힙니다.
- 위쪽 탐색 영역에 있는 전역 검색 표시줄을 사용 하 여 특정 SaaS 제안을 찾을 수 있습니다.

**Marketplace** 홈페이지의 위쪽에 있는 배너를 선택 하 여 [개인 SaaS 제품](/marketplace/private-offers) 을 찾습니다. 모든 제품 또는 요금제를 모든 지역에서 사용할 수 있는 것은 아닙니다. 일부는 특정 테 넌 트에 대해서만 표시 될 수 있습니다.

필터링 된 보기에는 제목으로 표시 되는 사용 가능한 각 SaaS 제품이 표시 됩니다. 하나를 선택 하 여 제품 정보 페이지를 표시 합니다. 여기에는 다음 섹션이 포함 됩니다.

- 개요 – 서비스, 마케팅 및 학습 자료에 대 한 세부 정보
- 요금제 + 가격 책정 – 각 제품은 청구 사용 약관 및 가격이 다른 계획을 하나 이상 포함 합니다.
- 사용 정보 + 지원 – Publisher id, 제품 id 및 계획 id를 포함 합니다.
- 특정 SaaS 제품의 등급 및 리뷰

## <a name="available-billing-models-plansskus-for-saas-offers"></a>SaaS 제품에 대 한 사용 가능한 청구 모델 (요금제/Sku)

각 SaaS 제품은 하나 이상의 계획을 갖습니다. 각 제품에는 연결 된 가격 책정 모델 (플랫 요금 또는 사용자 단위)이 있습니다. 각 요금제 가격은 0 달러 일 수 있는 되풀이 요금입니다. 나열 된 가격은 예를 들기 위한 것 이며 실제 비용을 반영 하지는 않습니다. 이 요금은 정액 요금 이거나 사용자 당 가격입니다. 사용 가능한 계획 유형:

- **월별 요금제** – 월간 요금을 반복 합니다. 월별 되풀이에서 요금을 지불 하는 정액 또는 사용자별 월간 요금입니다. 기간이 종료 되 면 계획이 자동으로 갱신 됩니다.
- **연간 요금제** – 연간 요금을 반복 합니다. 연간 되풀이에서 요금을 지불 하는 정액 또는 사용자 당 연간 요금입니다. 기간이 종료 되 면 계획이 자동으로 갱신 됩니다.
- **사용자 지정 미터** – 되풀이 수수료와 함께 플랫 요금제에는 초과분 사용에 대 한 선택적 사용자 지정 계량 차원이 포함 되지 않을 수도 있습니다. 각 차원은 청구 가능 단위를 나타냅니다. 이는 대역폭, 티켓 또는 전자 메일 처리와 같은 요금제 단위 사용에 따라 변경 되는 가변 비용입니다. 이러한 차원의 사용량에 따라 월별 요금이 청구 됩니다. 초과분 소비는 기본 요금에 포함 된 모든 요금제 단위를 사용 하는 경우에만 시작 됩니다.
- **무료 평가판** -경우에 따라 요금제는 한 달의 평가 기간을 포함 하며,이 기간 동안에는 소프트웨어를 무료로 사용할 수 있습니다.  평가 기간이 지나면 요금제에 따라 요금이 청구 됩니다. 평가판 제안은 사용자 지정 미터와 호환 되지 않습니다.

이러한 가격 책정 모델은 공용 및 개인 계획 모두에 사용할 수 있습니다.

## <a name="saas-purchase-experience"></a>SaaS 구매 환경

1. 제품 페이지에서 요구 사항을 충족 하는 계획을 선택 하 고 **+ 구독** 을 계속 설정 합니다.
2. 구매 프로세스의 일부로 **기본** 탭으로 리디렉션되고 다음 작업을 수행 해야 합니다.
    1. 청구에 사용할 *구독* 을 정의 합니다. 사용 하는 Azure 구독에는 유효한 구매 방법이 정의 되어 있어야 합니다. 올바른 수준의 사용 권한이 있거나 적절 한 수준의 사용 권한이 있는 해당 구독 아래에 리소스 그룹이 있어야 합니다. 또한 청구 국가는 제품이 구매할 수 있는 국가 여야 합니다. 유효한 지불 방법이 없는 Azure 구독 (예: MSDN 구독)은 무료 요금제를 구입 하는 데만 사용할 수 있습니다.
    1. SaaS 리소스가 속하게 될 **리소스 그룹* 을 선택 하거나 만듭니다.
    1. 나중에 쉽게 식별할 수 있도록 SaaS 구독의 *이름을* 입력 합니다. 구매한 후에는 이름을 변경할 수 없습니다.
    1. **요금제** 에는 제품 세부 정보 페이지 (PDP)에서 선택한 계획이 표시 됩니다. PDP에서 활성 선택을 수행 하지 않은 경우 기본 계획이 표시 됩니다. **계획 변경** 링크를 선택 하 여 선택 항목을 변경할 수 있습니다. 관련 청구 기간을 선택한 다음 다른 계획을 선택 합니다. 게시자가 지 원하는 경우 구매 후 계획을 변경할 수 있습니다. 그러나이 경우에는 월간에서 연간으로 또는 연간에서 월별으로 용어를 변경할 수 없습니다.
    1. 가격 책정 모델이 *사용자 당* 인 경우 *사용자* 수를 지정 해야 할 수 있습니다. 표시 되는 가격은 선택한 구독, 계획 및 조건에 따라 변경 됩니다.
3. **태그** 탭 *태그* 는 리소스 또는 리소스 그룹에 직접 배치할 수 있는 사용자 정의 키/값 쌍입니다. 태그를 사용 하 여 나중에 SaaS 리소스를 쉽게 찾을 수 있습니다. Azure는 현재 리소스 및 리소스 그룹당 최대 50개의 태그를 지원합니다. 태그를 만들 때 리소스에 배치하거나 기존 리소스에 추가할 수 있습니다.
4. 계속 해 서 **검토 + 구독** 으로 이동 하 여 제품 및 계획 세부 정보를 살펴봅니다.
    1. 게시자 및 Azure Marketplace에 대 한 *사용 약관*, *개정* 및 *개인 정보 취급 방침* 을 검토 합니다.
    1. 연락처 세부 정보를 추가 하 라는 메시지가 표시 될 수 있습니다.
    1. *기본 사항* 및 *태그* 세부 정보 검토
5. 확인 되 면 **구독** 을 선택 합니다.

## <a name="saas-subscription-and-configuration"></a>SaaS 구독 및 구성

구독을 선택 하면 "SaaS 구독이 진행 중입니다." 라는 메시지가 표시 됩니다. 이 프로세스는 몇 분 정도 걸리며 완료 될 때까지 창이 닫히지 않습니다.

구독이 완료 된 후에는 SaaS 구독이 완료 되었음을 알리는 메시지가 표시 되 고, 구매를 위해 계정을 구성 해야 합니다. 새 구독을 활성화 하도록 요청 하는 전자 메일도 받게 됩니다. SaaS 계정을 구성 하는 사람이 아닌 경우이 전자 메일을 관련 사용자에 게 전달 합니다.

프로세스를 완료 하 고 SaaS 사용을 시작 하려면 구독 구성을 시작 해야 합니다. **지금 계정 구성** 단추를 선택 하면 게시자의 웹 사이트로 리디렉션됩니다.

머리글의 오른쪽 위 모퉁이에 있는 ' 종 모양 ' 아이콘을 선택 하 여 구독 상태를 확인할 수도 있습니다.

*30 일* 이내에 구성 프로세스를 완료 하지 않으면이 SaaS 구독이 자동으로 *삭제* 됩니다. 계정이 게시자의 웹 사이트에서 구성 된 후 대금 청구는 시작 됩니다.

프로세스 중에 발생할 수 있는 오류 메시지:

- *선택한 계획의 계획 이름을* 무료 구독에서 구매할 수 없습니다.
  - 계정 업그레이드에 대 한 자세한 내용은을 참조 하세요 https://aka.ms/UpgradeFreeSub .

- 유효한 신용 카드를 찾을 수 없거나 Azure 구독과 연결 된 결제 방법을 찾을 수 없어 구매가 실패 했습니다.
  - 다른 Azure 구독을 사용 하거나이 구독에 대해 현재 신용 카드 또는 지불 방법을 add\update 후 다시 시도 하세요.

- 게시자 *게시자의* 제품 제공 *이름* 중에서 *선택한 계획의 이름은* IT 관리자가 설정한 규칙에 따라 구매할 수 없습니다.
  - IT 관리자에 게 문의 하세요.

- 테 넌 트의 IT 관리자가 만든 개인 marketplace 설정 때문에 제품 *의 게시자 게시자* 가 *선택한 제안 계획* 의 계획 *이름을* 구매할 수 없습니다.
  - IT 관리자에 게 문의

- 요청한 청구 기간이 비어 있거나 잘못 되어 구매 하지 못했습니다.
  - 다른 플랜/청구 기간을 구매해 보세요.

- 법적 계약에 대한 서명을 확인할 수 없어 구매에 실패했습니다.
  - 다시 시도 오류가 지속되면 다른 Azure 구독을 사용하여 구매하거나 고객 지원 담당자에게 문의하세요.

- publisher *publisherID별 제안* *제안ID를* 구매하지 못했습니다. 이 제안은 현재 구매할 수 없습니다.
  - 나중에 다시 시도하십시오. 1시간 후에도 이 오류 메시지가 계속 발생하면 고객 지원 담당자에게 문의하세요.  

- 게시자 *publisherID에* 의한 제안  *제안의 planID* 구매에 실패했습니다. 이 플랜은 현재 구매할 수 없습니다.
  - 나중에 다시 시도하십시오. 1시간 후에도 이 오류 메시지가 계속 발생하면 고객 지원 담당자에게 문의하세요. 

- 개체 *ID가 ObjectID인* 클라이언트 *이메일 주소에는* ResourceGroup 범위에 대해 *DeploymentValidationAction* 작업을 수행할 수 있는 권한이 없습니다. *DeploymentScope* 또는 범위가 잘못되었습니다.  
  - Azure 구독/리소스 그룹에 대한 올바른 권한이 없는 경우 이 메시지가 표시됩니다.  
    액세스 권한이 최근에 부여된 경우 자격 증명을 새로 고치세요.  
    리소스 그룹에 리소스를 배포하려면 기여자 이상의 액세스 권한이 있어야 합니다. **리소스 그룹에서** 액세스 상태를 확인한 다음, **를 Access Control.** 그러면 '소유자'가 누구인지, '참가자'로 할당하도록 요청할 수 있는 사람이 표시됩니다.

- 이 구매에 사용되는 구독은 Marketplace 구매를 허용하지 않습니다.  
  - 다른 구독을 사용하거나 관리자에게 이 구독에 대한 정의를 변경하고 다시 시도하도록 요청하세요.

## <a name="next-steps"></a>다음 단계

- 마켓플레이스에서 이미 제안을 구매한 경우 [청구 및 청구서로](/marketplace/billing-invoicing) 이동합니다.
- [프라이빗 계획](/marketplace/private-offers) 옵션에 대해 자세히 알아볼 수도 있습니다.
