---
title: 사용자 계정 만들기 및 역할 할당
description: 파트너 센터에 액세스하기 전에 모든 직원에게 역할을 할당해야 합니다. 사용자 계정을 만들고, 역할을 할당하고, 사용 권한을 설정하는 방법에 대해 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006764"
---
# <a name="create-user-accounts"></a>사용자 계정 만들기  

**적절한 역할**

- 계정 관리자
- 글로벌 관리자
- 사용자 관리 담당자

파트너 센터에 액세스해야 하는 직원의 사용자 계정을 만듭니다. 이러한 작업은 사용자 관리, 계정 관리 또는 글로벌 관리 권한이 있는 관리자가 수행해야 합니다. 이러한 작업을 수행하는 사용자에게는 사용자 관리자 또는 글로벌 관리자의 AAD(Azure Active Directory) 역할도 할당되어야 합니다. AAD 역할에 대한 자세한 내용은 [Azure Active Directory의 관리자 역할 권한](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)을 참조하세요.

## <a name="add-a-new-user"></a>새 사용자 추가

1. 파트너 센터 오른쪽 위의 **설정** 아이콘에서 **계정 설정**을 선택한 다음, **사용자 관리**를 선택합니다.

2. **사용자 추가**를 선택합니다.

3. 사용자의 전체 이름과 고유의 이메일 주소를 입력합니다.

4. 에이전트 유형 및/또는 사용자에게 할당할 관리자 유형을 선택합니다. 파트너 센터 액세스는 역할 기반이므로 사용자가 특정 작업을 완료하는 데 필요한 기능만 표시하도록 사용자의 보기를 사용자 지정하는 권한을 할당할 수 있습니다.  역할 할당을 원하는 사용자는 **사용자 관리**로 이동하여 글로벌 관리자에 대한 필터링을 수행하여 연락할 글로벌 관리자를 찾을 수 있습니다.

5. **추가**를 선택하여 사용자 계정을 만듭니다. 다음 페이지에서 사용자의 세부 정보를 확인합니다.

> [!IMPORTANT]  
> 이 페이지에 표시되는 새 사용자의 로그인 정보를 기록해 두세요. 나중에 이 정보에 다시 액세스할 수 없으므로 이 정보를 복사하여 새 사용자에게 보내야 합니다. 

사용자는 사용자 이름 및 임시 암호를 사용하여 파트너 센터에 로그인해야 합니다. 사용자가 파트너 센터에 처음으로 로그인하면 암호를 변경하라는 메시지가 표시됩니다.

## <a name="assign-user-roles"></a>사용자 역할 할당

파트너 센터에서 작업하려면 할당된 역할이 있어야 합니다.  현재 역할에는 Azure Active Directory 테넌트 역할, CSP(클라우드 솔루션 공급자) 역할 및 비 AAD 회사 역할이 포함됩니다. 개별 회사에 이러한 모든 역할이 필요할 수 있습니다.

>[!Important]
>파트너 센터에 액세스하려면 개별 회사가 테넌트에 나열되어야 합니다. 역할 할당은 추가 액세스 권한을 제공합니다.

## <a name="next-steps"></a>다음 단계

- [파트너 센터에서 작업해야 하는 직원에 대한 사용자 역할 및 권한 할당](permissions-overview.md)
