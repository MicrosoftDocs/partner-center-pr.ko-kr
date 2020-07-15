---
title: 사용자 계정 만들기 및 역할 할당
description: 파트너 센터에 액세스하기 전에 모든 직원에게 역할을 할당해야 합니다. 사용자 계정을 만들고, 역할을 할당하고, 사용 권한을 설정하는 방법에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
Keywords: 역할, 사용 권한, 사용자 추가, 역할 할당, 관리자, 에이전트,
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 9ec8e98f77d49e34b6747b0f580502e9df25a950
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265194"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a>사용자 계정 만들기 및 역할과 사용 권한 할당

**적절한 역할**

- 계정 관리자
- 글로벌 관리자
- 사용자 관리 담당자

파트너 센터에 액세스해야 하는 직원의 사용자 계정을 만듭니다. 이러한 작업은 사용자 관리, 계정 관리 또는 글로벌 관리 권한이 있는 관리자가 수행해야 합니다. 이러한 작업을 수행하는 사용자에게는 사용자 관리자 또는 글로벌 관리자의 AAD(Azure Active Directory) 역할도 할당되어야 합니다. AAD 역할에 대한 자세한 내용은 [Azure Active Directory의 관리자 역할 권한](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)을 참조하세요.


## <a name="add-a-new-user"></a>새 사용자 추가

1. 파트너 센터 오른쪽 위의 **설정** 아이콘에서 **사용자 관리**를 선택합니다.

2. **사용자 추가**를 선택합니다.

3. 사용자의 전체 이름과 고유의 이메일 주소를 입력합니다.

4. 에이전트 유형 및/또는 사용자에게 할당할 관리자 유형을 선택합니다. 파트너 센터 액세스는 역할 기반이므로 사용자가 특정 작업을 완료하는 데 필요한 기능만 표시하도록 사용자의 보기를 사용자 지정하는 권한을 할당할 수 있습니다.  역할 할당을 원하는 사용자는 **사용자 관리**로 이동하여 글로벌 관리자에 대한 필터링을 수행하여 연락할 글로벌 관리자를 찾을 수 있습니다.

5. **추가**를 선택하여 사용자 계정을 만듭니다. 다음 페이지에서 사용자의 세부 정보를 확인합니다.

> [!IMPORTANT]  
> 이 페이지에 표시되는 새 사용자의 로그인 정보를 기록해 두세요. 나중에 이 정보에 다시 액세스할 수 없으므로 이 정보를 복사하여 새 사용자에게 보내야 합니다. 


사용자는 사용자 이름 및 임시 암호를 사용하여 파트너 센터에 로그인해야 합니다. 사용자가 파트너 센터에 처음으로 로그인하면 암호를 변경하라는 메시지가 표시됩니다. 


### <a name="find-your-global-admin"></a>글로벌 관리자 찾기

사용자가 역할을 변경해야 하거나 새 사용자가 특정 역할 할당을 원하는 경우가 있을 수 있습니다.  
역할을 변경하거나 새 사용자에게 역할을 할당할 수 있는 글로벌 관리자를 찾으려면 파트너 센터의 오른쪽 위에 있는 **설정 아이콘**에서 **사용자 관리**를 선택하고 글로벌 관리자를 필터링합니다. 


### <a name="new-global-admin"></a>새 글로벌 관리자

글로벌 관리자가 조직을 떠나고 다른 사용자가 이 역할을 수행해야 하는 경우 Azure 또는 Office 365 팀에 티켓을 제출할 수 있습니다. 이 작업을 수행하는 방법에 대한 자세한 내용을 보려면 아래 옵션 중 하나를 선택하세요.

[Azure의 새 글로벌 관리자](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Office 365의 새 글로벌 관리자](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>사용자 역할 할당

파트너 센터에서 작업하려면 할당된 역할이 있어야 합니다.  현재 역할에는 Azure Active Directory 테넌트 역할, CSP(클라우드 솔루션 공급자) 역할 및 비 AAD 회사 역할이 포함됩니다. 개별 회사에 이러한 모든 역할이 필요할 수 있습니다.

>[!Important]
>파트너 센터에 액세스하려면 개별 회사가 테넌트에 나열되어야 합니다. 역할 할당은 추가 액세스 권한을 제공합니다.


**AAD 테넌트 역할에는 다음이 포함됩니다**.
- 글로벌 관리자
- 사용자 관리자

**CSP 역할에는 다음이 포함됩니다**.
- 관리 에이전트
- 청구 관리자
- 영업 상담원
- 기술 지원팀 상담원

**MPN 멤버십과 회사를 관리하는 역할(비 AAD)**
- MPN 파트너 관리자
- 계정 관리자
- 추천 관리자
- 비즈니스 프로필 관리자
- 인센티브 관리자 및 사용자

**제어판 공급업체는 CSP 및 비 AAD 역할입니다**.
- 글로벌 관리자

**게스트 사용자**은 AAD 테넌트의 일부여야 하며 모든 비 AAD 역할을 가질 수 있습니다.

역할과 각 역할이 수행할 수 있는 작업에 대한 자세한 내용은 [사용자 권한 할당](permissions-overview.md)을 참조하세요.

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>파트너 센터에서 사용자의 Microsoft Learn 계정 연결

사용자가 역량 달성을 위해 취하고 있는 교육 및 학습 경로를 볼 수 있으려면 해당 MCP ID를 파트너 센터 계정에 연결해야 합니다. 글로벌 관리자로서, 새 사용자를 추가할 때 계정에 MCP ID를 연결하도록 알려 주어야 합니다. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>파트너 센터 계정에 MCP ID를 연결하는 방법

1. 파트너 센터 대시보드에서, 대시보드 오른쪽 모서리에 있는 **계정** 아이콘을 선택한 다음, **내 프로필**을 선택합니다.

2. **학습** 아래에서 Microsoft Learning 계정을 연결할 수 있으며, 또한 Microsoft 계정을 파트너 대학에 연결할 수 있습니다.
