---
title: Azure Marketplace 파트너 통합
description: Azure 환경과 통합 되는 Azure Marketplace 솔루션에 대해 알아보고 Microsoft 파트너의 배포 가이드에 대 한 링크를 가져옵니다.
ms.service: partner-services
ms.topic: conceptual
author: dsindona
ms.author: dsindona
ms.date: 11/16/2020
ms.openlocfilehash: 7c97936e7764361c21503eca174433029707cf69
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691658"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace 파트너 통합

파트너 솔루션을 Azure 환경에 통합 하는 방법에 대해 알아봅니다. 이 문서에서는 각 솔루션에 대 한 개요와 자세한 배포 가이드에 대 한 링크를 제공 합니다. 솔루션은 알파벳 순서로 나열 됩니다. 

## <a name="apache-kafka-on-confluent-cloud"></a>Confluent 클라우드의 Apache Kafka

![Confluent 클라우드](./media/partners/confluent-cloud.png)

Azure를 사용 하면 클라우드 응용 프로그램 뿐만 아니라 Confluent 클라우드와 통합할 수 있습니다. Confluent 고객은 종종 Azure Portal와 Confluent 클라우드 간을 이동 합니다. 예를 들어 사용자가 Azure Marketplace에서 Confluent 클라우드 제품을 구매한 후 Confluent Cloud를 사용 하 여 계정을 설정 해야 합니다. 이 프로세스는 복잡성과 시간을 추가 하 고 사용자가 두 포털 간에 구성 및 리소스를 관리 해야 합니다. Confluent 클라우드와의 파트너 관계에서 Microsoft는 여러 플랫폼에서 관리 하는 부담을 줄이기 위해 Azure에서 Confluent Cloud로 통합 된 프로 비전 계층을 구축 했습니다. 이 솔루션은 Azure Marketplace에서 사용할 수 있으며 Azure에서 Confluent 클라우드 제품을 사용 하기 위한 원활한 환경을 제공 합니다.

이 솔루션은 Azure에서 사용 하도록 설정 된 리소스 공급자를 사용 하 여 Confluent 클라우드 리소스를 프로 비전 합니다. 이를 통해 사용자는 Azure Portal, Azure CLI 및 Azure Sdk를 통해 실시간 이벤트 스트리밍에 액세스할 수 있습니다. Confluent Cloud는 환경, 클러스터, 토픽, API 키 및 관리 되는 커넥터를 포함 하는 SaaS 응용 프로그램을 소유 하 고 실행 합니다.

Confluent Cloud와 긴밀 하 게 통합 되어 다음과 같은 기능을 사용할 수 있습니다.

- 완전히 관리 되는 인프라를 사용 하 여 Azure Portal에서 새로운 Confluent 클라우드 조직 리소스를 프로 비전 합니다.
- Azure Active Directory를 사용 하 여 Azure에서 Confluent Cloud로 Single Sign-On 간소화 Confluent 클라우드 포털에서 별도의 인증이 필요 하지 않습니다.
- Azure 구독 청구를 통해 Confluent 클라우드 소비 요금에 대 한 통합 청구를 받습니다.
- Azure Portal에서 Confluent 클라우드 리소스를 관리 하 고 Azure 리소스와 함께 **모든 리소스** 페이지에서 추적 합니다.

[Confluent 클라우드 배포 가이드](https://docs.confluent.io/current/cloud/marketplace/index.html)

Azure의 Confluent 관련 된 문제는로 이동 [https://support.confluent.io](https://support.confluent.io) 합니다. 처음 사용자 인 경우 Confluent 지원 포털에 로그인 하기 전에 암호를 다시 설정 합니다. Confluent가 포함 된 계정이 없는 경우로 전자 메일을 보내 주시기 바랍니다 [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![DataDog 로고](./media/partners/datadog.png)

Datadog는 하이브리드 및 다중 클라우드 환경에서 응용 프로그램의 상태와 성능을 이해 하기 위해 Azure 사용자를 위한 관찰성 및 보안 도구를 제공 합니다. 그러나 필요한 통합을 구성 하려면 Azure Portal와 Datadog 사이를 이동 해야 하는 경우가 많습니다. 포털에서 구성 및 리소스 관리를 간소화 하기 위해 Microsoft는 Datadog와 협력 하 여 Azure에서 통합 Datadog 솔루션을 만듭니다. Azure Marketplace를 통해 제공 되는이 솔루션은 Azure 고객이 Datadog의 클라우드 모니터링 솔루션을 사용 하는 원활한 환경을 제공 합니다.

이 솔루션에 대 한 자세한 내용을 알아보고 공개 미리 보기에 등록 하려면 [Azure Monitor 설명서](/azure/azure-monitor/platform/partners#datadog) 를 참조 하세요.

## <a name="next-steps"></a>다음 단계

- [온라인 스토어 Azure Marketplace](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Azure 계정 만들기](/learn/modules/create-an-azure-account/)
