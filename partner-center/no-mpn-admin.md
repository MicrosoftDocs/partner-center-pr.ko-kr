---
title: MPN 프로그램의 유일한 관리자가 퇴사한 경우 어떻게 해야 할까요?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 새 MPN 관리자를 찾거나 회사의 전역 관리자로부터 도움을 받으려면 어떻게 해야 하는지 알아봅니다. 또한 새 파트너 센터 전역 관리자를 추가하는 방법을 알아봅니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151171"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN 프로그램의 유일한 관리자가 퇴사한 경우 어떻게 해야 할까요?

**적절한 역할:** MPN 파트너 관리자 | 계정 관리자 | 전역 관리자

다음 문서에서는 MPN 관리자가 퇴사한 경우 수행할 수 있는 세 가지 일반적인 시나리오를 안내합니다.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>시나리오 1: MPN 파트너 관리자/계정 관리자가 퇴사했지만 여전히 계정에 전역 관리자가 있습니다.

이 경우 회사의 다른 사람에게 MPN 파트너 관리자 역할을 할당할 수 있습니다. 특정 MPN 파트너 관리자/계정 관리자 역할의 역할을 할당하려면 다음을 수행합니다.

1. 파트너 센터 계정으로 로그인합니다(예: tom@contoso.com ).
1. 전역 관리자의 **사용자 관리** 페이지 필터에서 회사의 전역 관리자가 누구인지 확인합니다. 
1. 전역 관리자 중 한 명에게 문의하고 필요한 MPN 관련 역할을 할당하도록 요청합니다. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>시나리오 2: MPN 파트너 관리자/계정 관리자가 퇴사했으며 계정에 전역 관리자가 없음 

**사용자 관리** 페이지로 이동하여 전역 관리자를 필터링하지만 MPN 관련 역할을 얻는 데 도움을 줄 수 있는 글로벌 관리자가 회사에 없는 경우 다음 단계를 수행합니다.

1. [portal.azure.com](https://ms.portal.azure.com/)으로 이동하여 작업 계정으로 tom@contoso.com 로그인합니다(예: ). 
1. 왼쪽 메뉴 탐색 모음에서 **도움말 + 지원** 옵션을 선택합니다.
1. 다음 페이지의 드롭다운 메뉴에서 **새 지원 요청** 및 **기술 문제** 유형을 선택하고, 추가 세부 정보를 삽입하고, **다음: 솔루션을 클릭합니다.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Azure Portal 관리자 찾기":::

4. 다음 페이지에서 권장 솔루션을 검토한 후 **다음: 세부 정보를** 선택하고 필요한 필드를 완료합니다.
1. 지원 요청을 검토하고 만듭니다.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>시나리오 3: MPN Partner admin/Account admin/Global admin이 회사를 떠난 경우 회사의 Azure AD에 액세스할 수 있는 다른 사용자가 없습니다. 이는 액세스의 전체 손실입니다.

[관리자 인수](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) 단계에 따라 관리 되지 않는 디렉터리를 Azure Active Directory 관리자 권한으로 사용 합니다.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>회사 계정이 있는지 확실하지 않은가요?

회사에 회사 계정이 있는지 확실 하지 않은 경우 다음 단계를 수행 하 여 확인 합니다.

1. [Azure 관리 포털](https://ms.portal.azure.com)에 로그인 합니다.
2. 왼쪽 메뉴에서 **Azure Active Directory** 를 선택한 다음 **도메인 이름** 을 선택 합니다.
이미 회사 계정이 있는 경우 도메인 이름이 나열됩니다.

>[!Note]
>Microsoft Azure 또는 Office 365에 대 한 활성 구독이 있는 경우 이미 회사 계정이 있으며 로그인 자격 증명은 해당 서비스에 액세스 하는 데 사용 되는 자격 증명과 동일 해야 합니다.