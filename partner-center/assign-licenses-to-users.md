---
title: 고객 계정에 대 한 사용자 관리 작업 | 파트너 센터
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객에 대 한 사용자 계정을 만들고, 사용자 라이선스를 추가 또는 제거 하 고, 사용자 암호를 다시 설정 하거나, 사용자 계정을 삭제 하거나, 복원 하는 방법에 대해 알아봅니다.
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: LauraBrenner
ms.author: labrenne
Keywords: 고객 관리, 계정, 계정 만들기, 라이선스, 라이선스 할당, 사용자 관리, 암호, 암호 재설정, 암호 변경
ms.localizationpriority: medium
ms.openlocfilehash: 15647d55b1e7a43ca78b2285808f8602dba80f41
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798621"
---
# <a name="user-management-tasks-for-customer-accounts"></a>고객 계정에 대 한 사용자 관리 작업

**적용 대상**

- 파트너 센터

**적절한 역할**

- 글로벌 관리자
- 사용자 관리 관리자
- 관리자 에이전트
- 영업 에이전트
- 기술 지원팀 에이전트

고객의 계정에서 새 사용자를 만들고 삭제할 수 있습니다. 삭제 후 30 일 이내에 이전에 삭제 한 사용자 계정을 하나 이상 복원할 수도 있습니다. 사용자의 이전 구독 할당도 복원 됩니다 (이전 할당을 사용할 수 있는 것으로 가정).

고객에 대 한 새 구독을 구입 하는 경우 고객은 계정, 해당 사용자 권한 및 각 사용자가 요구 하는 서비스를 필요로 하는 모든 사용자의 목록을 제공 해야 합니다.  

[Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)을 사용 하 여 [여러 사용자에 게 한 번에 여러 사용자에 게 구독을 할당할](bulk-license-provisioning-for-multiple-users.md) 수 있습니다.

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>고객의 사용자 계정 만들기

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서**사용자 및 라이선스**를 선택합니다.

4. 추가 하는 각 사용자에 대해 **구독 추가**를 선택 하 고 사용 권한 및 라이선스를 포함 한 정보를 입력 합니다. 변경 내용을 **저장**합니다.

5. 사용자에 게 보낼 사용자 이름 및 임시 암호를 기록해 두어야 합니다.

6. 한 번에 여러 사용자를 추가 하는 경우 **다른 사용자 추가**를 사용 합니다.

7. [Excel 호환 .csv 스프레드시트 파일을 가져오면](adding-multiple-users-to-a-customer-account.md)여러 사용자를 한 번에 추가할 수도 있습니다. 전자 메일을 보내거나 확인 화면에서 이름 및 암호를 인쇄 하기 전에 전체 설정이 완료 될 때까지 기다릴 수 있습니다.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>고객에 대 한 사용자 라이선스 추가 또는 제거

다음 단계는 Microsoft 제품에 대 한 사용자 라이선스를 추가 하거나 제거 하는 경우에 적용 됩니다. 상업적 marketplace에서 라이선스 기반 SaaS 구독의 사용자 라이선스를 추가 하거나 제거 하려면 [SaaS 구독에 대 한 라이선스 추가 또는 제거](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)를 참조 하세요.

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서**사용자 및 라이선스**를 선택합니다.

4. 목록에서 하나 이상의 사용자를 선택 합니다. 예를 들어 고객이 새 라이선스를 구매 했 고 아직 없는 사용자에 게 해당 라이선스를 할당 하려는 경우 **사용자 필터** ... 옵션을 사용 하 여 올바른 그룹을 찾을 수 있습니다.

5. **라이선스 관리**를 선택 합니다. 변경한 후 **저장**을 클릭 합니다.

> [!NOTE]
> 제품을 게시 한 ISV (독립 소프트웨어 공급 업체)를 통해 라이선스 할당 및 활성화를 관리 하는 [Azure Marketplace 제품](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)입니다.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>고객에 대 한 사용자 암호 재설정

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3.  고객 메뉴에서**사용자 및 라이선스**를 선택합니다. 목록에서 사용자를 선택합니다.

4.  화면 아래쪽에서 **암호 재설정**을 선택 합니다. 

5.  새 임시 암호를 사용자에 게 보냅니다.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>고객에 대 한 사용자 계정 삭제

1.  **파트너 센터** 메뉴에서 **고객**을 선택 합니다. 목록에서 고객을 선택합니다.

2.  고객 메뉴에서**사용자 및 라이선스**를 선택합니다. 목록에서 사용자를 선택합니다.

3.  화면 맨 아래에서 **사용자 계정 삭제**를 선택합니다.

이 계정을 복원 해야 하는 경우 고객의 **사용자 및 라이선스** 목록의 **삭제 된 사용자** 탭에서 찾을 수 있습니다. 삭제 된 사용자를 복원 하는 데 30 일이 있습니다.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>삭제 된 사용자 계정 복원

1.  **파트너 센터** 메뉴에서 **고객**을 선택한 다음 목록에서 고객을 선택 합니다.

2.  **사용자 및 라이선스**를 선택 합니다.

3.  삭제 된 **사용자 ()** 탭을 선택 합니다. 복원할 수 있는 삭제 된 사용자가 있는 경우에는 **(1)** 이상을 읽어야 합니다.

4.  삭제 된 사용자의 확인란을 하나 이상 선택 하 고 **복원**을 선택 합니다.

    선택한 모든 사용자 계정이 **사용자 및 라이선스** 페이지에 다시 나타납니다.

## <a name="related-topics"></a>관련 항목


[여러 사용자에게 라이선스 할당 또는 해지](bulk-license-provisioning-for-multiple-users.md)

[고객 계정에 대 한 여러 사용자 만들기](adding-multiple-users-to-a-customer-account.md)