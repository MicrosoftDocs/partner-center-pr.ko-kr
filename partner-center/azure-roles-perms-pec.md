---
title: 역할, 파트너 획득 크레딧을 위한 사용 권한
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너의 역할 및 권한에 대 한 자세한 내용을 확인 하 여 파트너 획득 크레딧을 받을 수 있습니다. 이러한 작업은 파트너 센터에서 작업 하는 역할과 다릅니다.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011743"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>파트너의 획득 크레딧을 획득 하는 데 적합 한 역할 및 사용 권한

다음 역할은 파트너가 파트너의 획득 크레딧을 사용할 수 있는지 여부를 결정 하는 사용 권한 수준에 매핑됩니다.

>[!Important]
>이러한 역할 및 사용 권한은 사용자가 파트너 센터에서 작업 해야 하는 역할 및 사용 권한과는 다릅니다.

|**역할**   |**설명**   |**PEC 적격**   |
|-----------------|:------------------|:--------------|
|소유자  |리소스에 대 한 액세스를 포함 하 여 모든 것을 관리 합니다.|예|
|참가자 |리소스 액세스 권한을 부여 하는 것을 제외 하 고 모든 항목을 관리 합니다.|예|
|판독기|모든 항목을 볼 수 있지만 변경할 수는 없습니다.|No|
|ACRDelete|acr 삭제|예|
|ACRImageSigner|acr 이미지 서명자|예|
|ACRPull|acr pull|예|
|AcrPush|acr push|예|
|AcrQuarantineReader|acr 격리 데이터 읽기 권한자|No|
|AcrQuarantineWriter| acr 격리 데이터 작성자|예|
|API Management 서비스 참가자|서비스 및 API를 관리할 수 있습니다.|예|
|API Management 서비스 운영자 역할|서비스를 관리할 수 있지만 API는 관리할 수 없습니다.|예|
|Azure API Management 읽기 권한자 역할|서비스 및 API에 대한 읽기 전용 액세스|No|
|Application Insights 구성 요소 참가자|Application Insights 구성 요소 관리|예|
|Application Insights 스냅샷 디버거|Application Insights 스냅샷 디버거를 사용하여 수집한 디버그 스냅샷을 보고 다운로드할 수 있는 사용자 권한을 제공합니다. 이러한 사용 권한은 소유자 또는 기여자 역할에 포함되지 않습니다.|예|
Automation 작업 연산자 | Automation Runbook을 사용하여 작업을 만들고 관리합니다. | 예 | 
Automation 운영자 | 자동화 연산자는 작업을 시작, 중지, 일시 중단 및 다시 시작할 수 있습니다. | 예 | 
Automation Runbook 연산자 | Runbook 작업을 만들려면 Runbook 속성을 읽어보세요. | 예 | 
Avere 기여자 | Avere vFXT 클러스터를 만들고 관리할 수 있습니다. | 예 | 
Avere 운영자 | Avere vFXT 클러스터에서 클러스터를 관리하는 데 사용됩니다. | 예 | 
Azure Event Hubs 데이터 소유자 | Azure Event Hubs 리소스에 대한 전체 액세스를 허용합니다. | 예 | 
Azure Event Hubs 데이터 받는 사람 | Azure Event Hubs 리소스에 대한 받기 액세스 권한을 허용합니다. | 예 | 
Azure Event Hubs 데이터 보내는 사람 | Azure Event Hubs 리소스에 대한 보내기 액세스 권한을 허용합니다. | 예 | 
Azure Kubernetes Service 클러스터 관리자 역할 | 클러스터 관리자 자격 증명 작업을 나열합니다. | 예 | 
Azure Kubernetes Service 클러스터 사용자 역할 | 클러스터 사용자 자격 증명 작업을 나열합니다. | 예 | 
Azure Maps 데이터 판독기(미리 보기) | Azure 맵 계정에서 맵 관련 데이터를 읽을 수 있는 액세스 권한을 부여합니다. | No | 
Azure Service Bus 데이터 소유자 | Azure Service Bus 리소스에 대한 전체 액세스를 허용합니다. | 예 | 
Azure Service Bus 데이터 받는 사람 | Azure Service Bus 리소스에 대한 받기 액세스 권한을 허용합니다. | 예 | 
Azure Service Bus 데이터 보내는 사람 | Azure Service Bus 리소스에 대한 보내기 액세스 권한을 허용합니다. | 예 | 
Azure Stack 등록 소유자 | Azure Stack 등록을 관리할 수 있습니다. | 예 | 
Backup 참가자 | 백업 서비스를 관리할 수 있지만, 자격 증명 모음을 만들고 다른 사용자에게 액세스 권한을 부여할 수는 없습니다. | 예 | 
Backup 운영자 | 백업 제거를 제외한 백업 서비스를 관리하고 자격 증명 모음 만들고 다른 사람에게 액세스 권한을 부여할 수 있습니다. | 예 | 
Backup 읽기 권한자 | 백업 서비스를 볼 수 있지만 변경할 수는 없습니다. | No | 
청구 읽기 권한자 | 결제 데이터에 대해 읽기 권한 허용 | No | 
BizTalk 참가자 | BizTalk Services를 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
블록체인 멤버 노드 액세스(미리 보기) | 블록체인 멤버 노드에 액세스할 수 있습니다. | 예 | 
청사진 기여자 | 청사진 정의를 관리할 수 있지만 할당할 수는 없습니다. | 예 | 
청사진 운영자 | 게시된 기존 청사진을 할당할 수 있지만 새 청사진을 만들 수는 없습니다. 참고: 사용자 할당 관리 id를 사용 하 여 할당을 수행 하는 경우에만 작동 합니다. | 예 | 
CD 엔드포인트 참가자 | CDN 엔드포인트를 관리할 수 있지만 다른 사용자에게 액세스 권한을 부여할 수는 없습니다. | 예 | 
CDN 엔드포인트 독자 | CDN 엔드포인트를 볼 수 있지만 변경할 수는 없습니다. | No | 
CDN 프로필 참가자 | CDN 프로필과 해당 엔드포인트를 관리할 수 있지만 다른 사용자에게 액세스 권한을 부여할 수는 없습니다. | 예 | 
CDN 프로필 독자 | CDN 프로필과 해당 엔드포인트를 볼 수 있지만 변경할 수는 없습니다. | No | 
클래식 네트워크 참가자 | 기본 네트워크를 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
클래식 Storage 계정 참가자 | 클래식 Storage 계정을 관리할 수 있지만 여기에 액세스할 수는 없습니다. | 예 | 
클래식 스토리지 계정 키 운영자 서비스 역할 | 클래식 스토리지 계정 키 운영자가 클래식 스토리지 계정에서 키를 나열하고 다시 생성할 수 있습니다. | 예 | 
클래식 Virtual Machine 참가자 | 클래식 가상 머신을 관리할 수 있지만 가상 머신이나 연결된 가상 네트워크 또는 스토리지 계정에 액세스할 수는 없습니다. | 예 | 
Cognitive Services 기여자 | Cognitive Services의 키를 만들고, 읽고, 업데이트하고, 삭제 및 관리할 수 있습니다. | 예 | 
Cognitive Services 데이터 읽기 권한자(미리 보기) | Cognitive Services 데이터를 읽을 수 있습니다. | No | 
Cognitive Services 사용자 | Cognitive Services의 키를 읽고 나열할 수 있습니다. | No | 
Cosmos DB 계정 독자 역할 | Azure Cosmos DB 계정 데이터를 읽을 수 있음. Azure Cosmos DB 계정 관리는 DocumentDB 계정 참가자를 참조하세요. | No | 
Cosmos DB 운영자 | Azure Cosmos DB 계정을 관리할 수 있지만 계정의 데이터에 액세스할 수는 없습니다. 계정 키 및 연결 문자열에 대한 액세스를 차단합니다. | 예 | 
CosmosBackupOperator | Cosmos DB 데이터베이스 또는 계정의 컨테이너에 대한 복원 요청을 제출할 수 있습니다. | 예 | 
Cost Management 기여자 | 비용을 확인하고 비용 구성(예: 예산, 내보내기)을 관리할 수 있음 | 예 | 
Cost Management 읽기 권한자 | 비용 데이터 및 구성(예: 예산, 내보내기)을 확인할 수 있음 | No | 
Data Box 기여자 | 다른 사람에게 액세스 권한을 부여하는 것을 제외한 모든 항목을 Data Box 서비스에서 관리할 수 있습니다. | 예 | 
Data Box 읽기 권한자 | 주문하기나 주문 세부 정보 편집 및 다른 사용자에게 액세스 권한 부여 외에 Data Box 서비스를 관리할 수 있습니다. | No | 
Data Factory 참가자 | 데이터 팩터리를 만들고 관리하며 해당 하위 리소스도 만들고 관리합니다. | 예 | 
Data Lake Analytics 개발자 | 사용자 자신의 작업을 제출, 모니터링 및 관리할 수 있지만 Data Lake Analytics 계정을 만들거나 삭제할 수는 없습니다. | 예 | 
데이터 제거자 | 분석 데이터를 제거할 수 있습니다. | 예 | 
DevTest Lab 사용자 | Azure DevTest Labs의 가상 머신을 연결, 시작, 다시 시작 및 종료할 수 있습니다. | 예 | 
DNS 영역 참가자 | Azure DNS의 DNS 영역과 레코드 집합을 관리할 수 있지만 액세스할 수 있는 사람을 제어할 수는 없습니다. | 예 | 
DocumentDB 계정 참가자 | Azure Cosmos DB 계정을 관리할 수 있습니다. Azure Cosmos DB는 이전의 DocumentDB입니다. | 예 | 
EventGrid EventSubscription 기여자 | EventGrid 이벤트 구독 작업을 관리할 수 있습니다. | 예 | 
EventGrid EventSubscription 읽기 권한자 | EventGrid 이벤트 구독을 읽을 수 있습니다. | No | 
HDInsight 클러스터 운영자 | HDInsight 클러스터 구성을 읽고 수정할 수 있습니다. | 예 | 
HDInsight 도메인 서비스 기여자 | HDInsight Enterprise Security Package에 필요한 도메인 서비스 관련 작업을 읽고, 만들고, 수정하고, 삭제할 수 있음 | 예 | 
지능형 시스템 계정 참가자 | 인텔리전트 시스템 계정을 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
Key Vault 참가자 | 키 자격 증명 모음을 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
랩 작성자 | Azure Lab 계정 하에서 관리 랩을 만들고, 관리하고, 삭제할 수 있습니다. | 예 | 
Log Analytics 참가자 | Log Analytics 참가자는 모든 모니터링 데이터를 읽고 모니터링 설정을 편집할 수 있습니다. 모니터링 설정 편집에는 VM에 VM 확장 추가, Azure Storage에서 로그 컬렉션을 구성할 수 있는 스토리지 계정 키 읽기, Automation 계정 생성 및 구성, 솔루션 추가 및 모든 Azure 리소스에 대한 Azure 진단을 구성하는 기능도 포함되어 있습니다. | 예 | 
Log Analytics 독자 | Log Analytics 독자는 모든 Azure 리소스에 대한 Azure 진단의 구성 보기를 비롯하여 모니터링 설정 보기 및 모든 모니터링 데이터를 보고 검색할 수 있습니다. | No | 
논리 앱 참가자 | 논리 앱을 관리할 수 있지만 앱을 변경할 수는 없습니다. | 예 | 
논리 앱 운영자 | 논리 앱을 읽고 사용하도록 설정하고 사용하지 않도록 설정할 수 있지만 편집하거나 업데이트할 수는 없습니다. | 예 | 
관리되는 애플리케이션 운영자 역할 | 관리되는 애플리케이션 리소스에서 작업을 읽고 수행할 수 있습니다. | 예 | 
Managed Applications 읽기 권한자 | 관리 앱 및 요청 JIT 액세스에서 리소스를 읽을 수 있습니다. | No | 
관리 ID 참가자 | 사용자 할당 ID를 만들고, 읽고, 업데이트하고, 삭제합니다. | 예 | 
관리 ID 운영자 | 사용자 할당 ID를 읽고 할당합니다. | 예 | 
관리 그룹 참가자 | 관리 그룹 참가자 역할 | 예 | 
관리 그룹 읽기 권한자 | 관리 그룹 읽기 권한자 역할 | No | 
Monitoring Contributor | 모든 모니터링 데이터를 읽고 모니터링 설정을 편집할 수 있음 Azure Monitor에서의 역할, 권한 및 보안 시작도 참조하세요. | 예 | 
모니터링 메트릭 게시자 | Azure 리소스에 대한 게시 메트릭 사용 | 예 | 
Monitoring Reader | 모든 모니터링 데이터를 읽을 수 있음(메트릭, 로그 등) Azure Monitor에서의 역할, 권한 및 보안 시작도 참조하세요. | No | 
네트워크 참가자 | 네트워크를 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
NewRelic APM 계정 참가자 | New Relic Application Performance Management 계정 및 애플리케이션을 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
읽기 권한자 및 데이터 액세스 | 모든 것을 볼 수 있지만, 스토리지 계정 또는 포함된 리소스를 삭제하거나 만들 수는 없습니다. 또한 스토리지 계정 키에 액세스하여 스토리지 계정에 포함된 모든 데이터를 읽고 쓸 수 있습니다. | 예 | 
Redis Cache 참가자 | Redis Cache를 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
리소스 정책 참가자(미리 보기) | (미리 보기) 리소스 정책을 생성/수정하고, 지원 티켓을 만들고, 리소스/계층 구조를 읽을 수 있는 권한을 가진 EA의 백필된 사용자입니다. | 예 | 
Scheduler 작업 컬렉션 참가자 | Scheduler 작업 컬렉션을 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
Search 서비스 참가자 | Search 서비스를 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
보안 관리자 | Security Center에서만: 보안 정책 보기, 보안 상태 보기, 보안 정책 편집, 경고 및 권장 사항 보기, 경고 및 권장 사항 해제 | 예 | 
보안 관리자(레거시) | 레거시 역할입니다. 보안 관리자를 대신 사용하세요. | 예 | 
보안 Reader | Security Center에서만: 권장 사항 및 경고 보기, 보안 정책 보기, 보안 상태 보기 가능, 변경 불가 | No | 
Site Recovery 참가자 | 자격 증명 모음 만들기 및 역할 할당을 제외한 Site Recovery 서비스를 관리할 수 있습니다. | 예 | 
Site Recovery 운영자 | 장애 조치(failover) 및 장애 복구(failback)를 수행할 수 있지만 다른 Site Recovery 관리 작업은 수행할 수 없습니다. | 예 | 
Site Recovery 구독자 | Site Recovery 상태를 볼 수 있지만 다른 관리 작업은 수행할 수 없습니다. | No | 
Spatial Anchors 계정 기여자 | 계정의 공간 앵커를 관리할 수 있지만 삭제할 수는 없습니다. | 예 | 
Spatial Anchors 계정 소유자 | 계정의 공간 앵커를 관리할 수 있고 삭제할 수도 있습니다. | 예 | 
Spatial Anchors 계정 읽기 권한자 | 계정의 공간 앵커 속성을 찾아서 읽을 수 있습니다. | No | 
SQL DB 참가자 | SQL 데이터베이스를 관리할 수 있지만 액세스할 수는 없습니다. 또한 보안 관련 정책이나 부모 SQL 서버를 관리할 수 없습니다. | 예 | 
SQL Managed Instance 기여자 | SQL 관리 되는 인스턴스 및 필요한 네트워크 구성을 관리할 수 있지만 다른 사용자에 게는 액세스할 수 없습니다. | 예 | 
SQL 보안 관리자 | SQL Server 및 데이터베이스의 보안과 관련된 정책을 관리할 수 있지만 여기에 액세스할 수는 없습니다. | 예 | 
SQL Server 참가자 | SQL Server 및 데이터베이스를 관리할 수 있지만 여기에 액세스할 수는 없으며, 해당하는 보안과 관련된 정책에도 액세스할 수 없습니다. | 예 | 
Storage 계정 참가자 | 스토리지 계정을 관리할 수 있도록 허용합니다. 공유 키 권한 부여를 통해 데이터에 액세스하는 데 사용할 수 있는 계정 키에 대한 액세스 권한을 제공합니다. | 예 | 
스토리지 계정 키 운영자 서비스 역할 | 스토리지 계정 액세스 키를 나열하고 다시 생성할 수 있도록 허용합니다. | 예 | 
Storage Blob 데이터 기여자 | Azure Storage 컨테이너 및 BLOB을 읽고, 쓰고, 삭제합니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | 예 | 
Storage Blob 데이터 소유자 | POSIX 액세스 제어 할당을 포함하여 Azure Storage BLOB 컨테이너 및 데이터에 대한 모든 액세스 권한을 제공합니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | 예 | 
Storage Blob 데이터 읽기 권한자 | Azure Storage 컨테이너 및 BLOB을 읽고 나열합니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | No | 
Storage Blob 위임자 | Azure AD 자격 증명으로 서명된 컨테이너 또는 BLOB의 공유 액세스 서명을 만드는 데 사용할 수 있는 사용자 위임 키를 가져옵니다. 자세한 내용은 사용자 위임 SAS 만들기를 참조하세요. | 예 | 
스토리지 파일 데이터 SMB 공유 Contributor | SMB를 통한 Azure Storage 파일 공유에 대 한 읽기, 쓰기 및 삭제 액세스를 허용 합니다. | 예 | 
스토리지 파일 데이터 SMB 공유 관리자 권한 Contributor | SMB를 통한 Azure Storage 파일 공유에서 NTFS 권한 액세스를 읽고, 쓰고, 삭제 하 고, 수정할 수 있습니다. | 예 | 
스토리지 파일 데이터 SMB 공유 Reader | SMB를 통해 Azure 파일 공유에 대 한 읽기 액세스를 허용 합니다. | No | 
Storage 큐 데이터 기여자 | Azure Storage 큐 및 큐 메시지를 읽고, 쓰고, 삭제할 수 있습니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | 예 | 
Storage 큐 데이터 메시지 처리자 | Azure Storage 큐의 메시지를 선택, 검색 및 삭제할 수 있습니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | 예 | 
Storage 큐 데이터 메시지 보내는 사람 | Azure Storage 큐에 메시지를 추가할 수 있습니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | 예 | 
Storage 큐 데이터 읽기 권한자 | Azure Storage 큐 및 큐 메시지를 읽고 나열할 수 있습니다. 특정 데이터 연산에 어떤 작업이 필요한지 알아보려면 BLOB 및 큐 데이터 연산을 호출하기 위한 권한을 참조하세요. | No | 
지원 요청 참가자 | 지원 요청을 만들고 관리할 수 있습니다. | 예 | 
Traffic Manager 참가자 | Traffic Manager 프로필을 관리할 수 있지만 액세스할 수 있는 사람을 제어할 수는 없습니다. | 예 | 
사용자 액세스 관리자 | Azure 리소스에 대한 사용자 액세스를 관리할 수 있습니다. | 예 | 
가상 머신 관리자 로그인 | 포털에서 Virtual Machines를 보고 관리자 권한으로 로그인합니다. | 예 | 
가상 머신 참가자 | 가상 머신을 관리할 수 있지만 가상머신이나 연결된 가상 네트워크 또는 스토리지 계정에 액세스할 수는 없습니다. | 예 | 
가상 머신 사용자 로그인 | 포털에서 Virtual Machines를 보고 일반 사용자 권한으로 로그인합니다. | 예 | 
웹 계획 참가자 | 웹 사이트의 웹 계획을 관리할 수 있지만 액세스할 수는 없습니다. | 예 | 
웹 사이트 참가자 | 웹 사이트 (웹 요금제 아님)를 관리할 수 있지만 액세스할 수는 없습니다. | 예 |
