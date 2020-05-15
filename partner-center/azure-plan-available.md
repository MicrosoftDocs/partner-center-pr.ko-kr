---
title: Azure CSP에서 사용 가능한 Azure 서비스
description: 이 섹션에서는 Azure CSP(클라우드 솔루션 공급자) 프로그램에서 사용할 수 있거나 사용할 수 없는 Azure 서비스에 대해 설명합니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.date: 03/05/2020
ms.openlocfilehash: 29020fc4861bb11f15f7a892dda4d92f0c19fe07
ms.sourcegitcommit: af3ecd7f35e5bb3b87f5f683335c76e287f2a9b8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83369280"
---
# <a name="available-azure-services-in-azure-csp"></a>Azure CSP에서 사용 가능한 Azure 서비스

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 글로벌 관리자
- 기술 지원팀 상담원
- 영업 상담원
- 사용자 관리 담당자

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP에서 사용 가능한 Azure 서비스

이 문서에는 Azure CSP(클라우드 솔루션 공급자) 프로그램에서 사용할 수 있거나 사용할 수 없는 Azure 서비스가 나열되어 있습니다. 또한 [Microsoft Azure 독일](https://azure.microsoft.com/overview/clouds/germany/) 및 [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) 국가 클라우드의 서비스 가용성에 대해서도 설명합니다.

>[!Note]
>[Azure 중국]( https://www.azure.cn/)은 Azure CSP 프로그램에서 사용할 수 없습니다.

## <a name="global-cloud"></a>글로벌 클라우드

Azure Resource Manager 모델 기반의 모든 서비스는 CSP 프로그램에서 사용할 수 있습니다.  Azure Resource Manager 기반 이외의 서비스는 CSP 프로그램에서 사용할 수 없습니다.  

## <a name="csp-specific-service-configurations"></a>CSP 특정 서비스 구성

특수한 CSP 구성이 필요한 서비스는 다음과 같습니다.

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) - 고객 테넌트의 사용자만 Time Series Insight 환경의 데이터에 액세스할 수 있습니다. 파트너는 기본적으로 고객의 Time Series Insights 환경을 관리할 수 있지만, 이 환경의 데이터에 액세스해야 하는 경우 해당 환경을 고객 테넌트에 추가해야 합니다.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

이제 타사 확장을 제외하고 Visual Studio Marketplace에서 아래에 나열된 항목을 구입할 수 있습니다.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio 구독](https://www.visualstudio.com/subscriptions/)

- [Xamarin University 교육](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

시작하는 데 도움이 되도록 CSP에서 [Azure DevOps를 설정, 구매 및 관리하는 방법](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer)에 대한 비디오와 설명서를 만들었습니다.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP의 Azure Marketplace 항목

일부 Azure Marketplace 항목은 현재 Azure CSP 구독에서 사용할 수 없습니다.

- Microsoft 기반 Azure 서비스: 이러한 서비스는 사용할 수 있습니다. 이전 표와 설명을 검토하세요.

- BYOL(사용자 라이선스 필요) 항목: 이러한 항목은 사용할 수 있습니다. BYOL 지원 Azure Marketplace 항목의 전체 목록은 [Azure Marketplace BYOL 페이지](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)에서 사용할 수 있습니다.

- 타사 Azure Marketplace 종량제 항목: 공급자가 CSP 채널에 게시한 경우에 이러한 항목을 사용할 수 있습니다. 자세한 내용은 [Azure Marketplace 제품 구독 판매](https://aka.ms/marketplaceincsp)를 참조하세요.

- Citrix XenApp Essentials: 파트너는 CSP에서 고객을 대신하여 XenApp Essentials를 구입할 수 있습니다. 자세한 내용은 [이제 Microsoft 클라우드 솔루션 공급자 채널을 통해 사용할 수 있는 XenApp Essentials 배포](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) Citrix 블로그를 참조하세요.

## <a name="national-clouds"></a>국가 클라우드

다음 표에는 국가 클라우드에서 CSP에 사용할 수 있는 자사 Azure 제품, 서비스 및 기능이 정기적으로 업데이트된 목록이 나와 있습니다.

| Azure 제품, 서비스 또는 기능 | US Government | 독일 |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Virtual Machines  |  X  |  X  |
|  Cloud Services  |    |    |
|  가상 머신 확장 집합  |  X  |  X  |
|  함수  |    |    |
|  Azure Container Service  |    |    |
|  **네트워킹**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  부하 분산 장치  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **스토리지**  |    |    |
|  스토리지  |  X  |  X  |
|  백업  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **웹 + 모바일**  |    |    |
|  App Service  |  X  |  X  |
|  App Service on Linux  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Azure App Service의 Logic Apps 기능  |    |    |
|  **컨테이너**  |    |    |
|  App Service  |  X  |  X  |
|  App Service on Linux  |    |  X  |
|  Batch (배치)  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **데이터베이스**  |    |    |
|  SQL Database  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **데이터 + 분석**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + Cognitive Services**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **사물 인터넷**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based Services  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **엔터프라이즈 통합**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  서비스 버스  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Azure App Service의 Logic Apps 기능  |    |    |
|  **보안 + ID**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Security Center  |  X  |  X  |
|  **개발자 도구**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **모니터링 + 관리**  |    |    |
|  Advisor  |    |    |
|  백업  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  스케줄러  |  X  |  X  |
|  자동화  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure-Managed Applications  |    |    |
|  Azure Migrate  |    |    |
|  관리 그룹  |    |  

## <a name="next-steps"></a>다음 단계

- 파트너 센터에서 Azure에 사용할 수 있는 기능에 대해 [알아봅니다](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview).

- Azure CSP에서 첫 번째 고객을 [만들고](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) Azure 서비스를 배포합니다.
