---
title: MPN 프로그램에 대 한 유일한 관리자가 회사를 떠난 경우 어떻게 해야 하나요?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 새 MPN 관리자를 찾거나 회사의 전역 관리자에 게 도움을 받으려면 어떻게 해야 하는지 알아보세요. 또한 새 파트너 센터 전역 관리자를 추가 하는 방법에 대해 알아봅니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277677"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN 프로그램에 대 한 유일한 관리자가 회사를 떠난 경우 어떻게 해야 하나요?

**적절 한 역할**: MPN partner admin | 계정 관리자 | 전역 관리자

다음 문서에서는 MPN 관리자가 회사를 떠난 경우 수행할 작업에 대 한 세 가지 일반적인 시나리오를 안내 합니다.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>시나리오 1: MPN Partner Admin/Account Admin이 회사를 떠난 상태 이지만 계정에 전역 관리자가 있습니다.

이 경우 회사의 다른 사용자에 게 MPN Partner admin의 역할을 할당할 수 있습니다. 특정 MPN 파트너 관리자/계정 관리자 역할의 역할을 할당 하려면 다음을 수행 합니다.

1. 회사 계정 (예:)을 사용 하 여 파트너 센터 계정에 로그인 tom@contoso.com 합니다.
1. 전역 관리자의 **사용자 관리** 페이지 필터를 사용 하 여 회사의 전역 관리자가 누구 인지 확인할 수 있습니다. 
1. 전역 관리자 중 한 명에 게 연락 하 여 필요한 MPN 역할을 할당 해 달라고 요청 합니다. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>시나리오 2: MPN Partner Admin/Account Admin이 회사를 떠난 후 계정에 전역 관리자가 없습니다. 

**사용자 관리** 페이지로 이동 하 여 전역 관리자를 필터링 했지만 회사에 MPN 역할을 얻을 수 있는 전역 관리자가 없다는 것을 발견 한 경우 다음 단계를 수행 합니다.

1. [Portal.azure.com](https://ms.portal.azure.com/)으로 이동 하 여 회사 계정으로 로그인 합니다 (예: tom@contoso.com ). 
1. 왼쪽 메뉴 탐색 모음에서 **도움말 + 지원** 옵션을 선택 합니다.
1. 다음 페이지의 드롭다운 메뉴에서 **새로 만들기 지원 요청** 및 **기술 문제** 유형을 선택 하 고 추가 세부 정보를 삽입 하 고 **다음을 클릭 합니다. 솔루션.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Azure Portal에서 관리자를 찾습니다.":::

4. 다음 페이지에서 권장 해결 방법을 검토 한 후 **다음: 세부 정보** 를 선택 하 고 필요한 필드를 완료 합니다.
1. 지원 요청을 검토 하 고 만듭니다.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>시나리오 3: MPN Partner admin/Account admin/Global admin이 회사를 떠난 경우 회사의 Azure AD에 액세스할 수 있는 다른 사용자가 없습니다. 이는 액세스의 전체 손실입니다.

[관리자 인수](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) 단계에 따라 관리 되지 않는 디렉터리를 Azure Active Directory 관리자 권한으로 사용 합니다.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>회사 계정이 있는지 확실하지 않은가요?

회사에 회사 계정이 있는지 확실 하지 않은 경우 다음 단계를 수행 하 여 확인 합니다.

1. [Azure 관리 포털](https://ms.portal.azure.com)에 로그인 합니다.
2. 왼쪽 메뉴에서 **Azure Active Directory** 를 선택한 다음 **도메인 이름** 을 선택 합니다.
이미 회사 계정이 있는 경우 도메인 이름이 나열됩니다.

>[!Note]
>Microsoft Azure 또는 Office 365에 대 한 활성 구독이 있는 경우 이미 회사 계정이 있으며 로그인 자격 증명은 해당 서비스에 액세스 하는 데 사용 되는 자격 증명과 동일 해야 합니다.