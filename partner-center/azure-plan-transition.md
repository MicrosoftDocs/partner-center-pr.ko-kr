---
title: Azure 플랜으로 고객 전환 | 파트너 센터
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객을 Azure 플랜으로 쉽게 이동시키는 방법을 알아봅니다.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567239"
---
# <a name="transition-your-customers-to-azure-plan"></a>고객을 Azure 플랜으로 전환

**적절한 역할**

- 관리 에이전트
- 청구 관리자
- 글로벌 관리자
- 기술 지원팀 상담원
- 영업 상담원
- 사용자 관리 담당자

간접 공급자와 직접 청구 파트너는 Azure용 CSP(클라우드 서비스 공급자) 프로그램에서 사용할 수 있는 새로운 상거래 환경으로 전환할 수 있습니다. (직접 재판매인은 간접 공급자를 통해 작업해야 합니다.) 고객은 파트너 또는 Microsoft 판매자에게 구입하든 아니면 웹에서 직접 구입하든, 간편하게 클라우드 서비스를 구입할 수 있습니다.

전환 기능은 Azure의 새로운 상거래 환경으로 전환하는 고객과 Microsoft 고객 계약에 서명한 고객을 위한 것이며, Office 365 또는 Dynamics 365와 같은 CSP의 다른 제품을 위한 것이 아닙니다.

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP에서 사용 가능한 Azure 서비스

이 섹션에서는 Azure CSP(클라우드 솔루션 공급자) 프로그램에서 사용할 수 있거나 사용할 수 없는 Azure 서비스에 대해 설명합니다. 또한 [Microsoft Azure 독일](https://azure.microsoft.com/overview/clouds/germany/) 및 [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) 국가 클라우드의 서비스 가용성에 대해서도 설명합니다.

>[!Note]
>[Azure 중국]( https://www.azure.cn/)은 Azure CSP 프로그램에서 사용할 수 없습니다.

### <a name="global-cloud"></a>글로벌 클라우드 

Azure Resource Manager 모델 기반의 모든 서비스는 CSP 프로그램에서 사용할 수 있습니다.  Azure Resource Manager 기반 이외의 서비스는 CSP 프로그램에서 사용할 수 없습니다.  

### <a name="csp-specific-service-configurations"></a>CSP 특정 서비스 구성

특수한 CSP 구성이 필요한 서비스는 다음과 같습니다.

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) - 고객 테넌트의 사용자만 Time Series Insight 환경의 데이터에 액세스할 수 있습니다. 파트너는 기본적으로 고객의 Time Series Insights 환경을 관리할 수 있지만, 이 환경의 데이터에 액세스해야 하는 경우 해당 환경을 고객 테넌트에 추가해야 합니다. 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

이제 타사 확장을 제외하고 Visual Studio Marketplace에서 아래에 나열된 항목을 구입할 수 있습니다.

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Visual Studio 구독](https://www.visualstudio.com/subscriptions/)

- [Xamarin University 교육](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

시작하는 데 도움이 되도록 CSP에서 [Azure DevOps를 설정, 구매 및 관리하는 방법](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer)에 대한 비디오와 설명서를 만들었습니다.

### <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP의 Azure Marketplace 항목

일부 Azure Marketplace 항목은 현재 Azure CSP 구독에서 사용할 수 없습니다.

- Microsoft 기반 Azure 서비스: 이러한 서비스는 사용할 수 있습니다. 이전 표와 설명을 검토하세요.

- BYOL(사용자 라이선스 필요) 항목: 이러한 항목은 사용할 수 있습니다. BYOL 지원 Azure Marketplace 항목의 전체 목록은 [Azure Marketplace BYOL 페이지](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)에서 사용할 수 있습니다.

- 타사 Azure Marketplace 종량제 항목: 공급자가 CSP 채널에 게시한 경우에 이러한 항목을 사용할 수 있습니다. 자세한 내용은 [Azure Marketplace 제품 구독 판매](https://aka.ms/marketplaceincsp)를 참조하세요.   

- Citrix XenApp Essentials: 파트너는 CSP에서 고객을 대신하여 XenApp Essentials를 구입할 수 있습니다. 자세한 내용은 [이제 Microsoft 클라우드 솔루션 공급자 채널을 통해 사용할 수 있는 XenApp Essentials 배포](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) Citrix 블로그를 참조하세요.

### <a name="national-clouds"></a>국가 클라우드 
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

### <a name="next-steps"></a>다음 단계

- 파트너 센터에서 Azure에 사용할 수 있는 기능에 대해 [알아봅니다](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview).

- Azure CSP에서 첫 번째 고객을 [만들고](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) Azure 서비스를 배포합니다.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>기존 CSP 제품을 Azure 플랜으로 전환

파트너 센터 내에서 고객을 기존 CSP Azure 제품에서 CSP 프로그램의 새로운 상거래 환경에서 제공하는 Azure 플랜 하의 Azure 서비스로 전환할 수 있습니다. 이렇게 하려면 파트너와 고객에게 파트너 센터를 통해 설정된 재판매인 관계가 있어야 하고, 고객은 Microsoft 고객 계약에 서명해야 합니다.

### <a name="select-transition-to-azure-plan"></a>Azure 플랜으로 전환 선택

1. 고객에게 Azure 플랜을 선택합니다.

2. **청구를 Azure 플랜으로 전환**을 선택합니다.

![전환](images/azure/transition1.png)

3. **계속**을 선택합니다.

![전환](images/azure/transition2.png)

고객이 Azure 플랜으로 전환됩니다.

**전환 워크플로는 다음과 같은 필수 조건 단계를 자동화합니다**.

- Azure 플랜 구입
- 직접 CSP 시나리오에서는 고객당 플랜 하나  
- 재판매인당 플랜 하나  

예를 들어 파트너가 Microsoft Azure 제품을 2개 구입하고 별도의 POR 2개를 구매에 포함했습니다. 이 경우 전환 워크플로에서는 Azure 플랜을 2개 구입하고(재판매인당 하나) Azure 플랜에 따라 각 Azure 구독을 자동으로 매핑합니다.  

**Azure 구독을 Azure 플랜에 매핑**

Azure 플랜을 구입한 후에는 시스템에서 기존 Azure 구독을 Azure 플랜에 매핑합니다. 진행률은 Azure Portal과 파트너 센터에서 볼 수 있습니다. 

4. 고객의 파트너 센터 **구독** 페이지로 돌아와서 고객의 예산 한도를 고객의 현지 통화로 업데이트합니다. 

![전환](images/azure/transition3.png)

>[!NOTE]
>파트너 센터에서 설정한 예산이 Azure Portal로 전달되지 않습니다. Azure Portal에서도 예산과 경고를 설정해야 합니다.

Azure 플랜으로 이동하면 더 이상 이 고객에 대한 Azure 구독을 구매할 수 없습니다. Azure Portal에서 Azure 플랜에 따라 구독을 만들어야 합니다.

>[!NOTE]
> Azure 플랜에서 RBAC를 통해 구입한 모든 Azure 구독은 현지 통화로 가격이 책정되고 요금이 청구됩니다. 환율은 사용되지 않습니다.

### <a name="track-your-transition-details"></a>전환 세부 정보 추적

Azure Portal과 파트너 센터에서 전환 단계를 수행하세요.

![세부 정보 표시](images/azure/details1.png)

**파트너에게 미치는 청구 영향**

기존 CSP Azure 제품을 사용하는 고객을 전환하면 다음과 같은 청구 영향이 있습니다.

- 원래의 CSP Azure 구독이 종료될 때까지의 모든 사용량에 대한 요금은 기존 CSP 청구서로 청구됩니다.

- 기존 CSP 구독에 대한 관리자 액세스 권한이 있는 경우 해당 구독이 마이그레이션되어도 계속 액세스할 수 있습니다.

직접 기업 계약을 CSP로 전환하고 서버 및 클라우드 등록을 Azure 서비스로 전환하려면 [Microsoft 파트너 계약에 대한 Azure 구독의 청구 소유권 얻기](https://docs.microsoft.com/azure/billing/mpa-request-ownership)를 읽어 보세요.

**감사 로그**:

청구를 조정하려면 **구독** 페이지에서 "Microsoft Azure"(0145P) 구독의 기록을 확인하세요. 

"Microsoft Azure"(0145P) 구독은 다음과 같은 두 부분으로 구성됩니다.
1. 상거래 구독 
2. Azure 구독(자격)

전환이 완료되면 Azure 구독이 새 Azure 플랜으로 이동되고 상거래 구독이 일시 중단되어 더 이상 서비스 사용이 보고되지 않습니다.  

>[참고]\: CSP에서 Microsoft Azure(0145P) 구독을 구매한 경우 상거래 구독과 Azure 구독(자격)의 가격이 동일합니다. 청구 소유권이 변경되거나 이전되는 경우에만 가격이 달라집니다. 

**전환 문제**

전환하는 동안에는 문제가 발생하지 않습니다. 만약 오류가 발생할 경우 전환 워크플로 자체에서 업데이트해 드리겠습니다. Azure 사용에 방해가 되는 일은 없을 것입니다.  

## <a name="next-steps"></a>다음 단계

- [Azure 플랜 하에서 구독 및 리소스 관리](azure-plan-manage.md)

- [파트너 획득 크레딧 - 개요](partner-earned-credit.md)



