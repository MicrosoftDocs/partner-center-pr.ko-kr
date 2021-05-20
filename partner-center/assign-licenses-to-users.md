---
title: 고객 계정에 대한 사용자 관리
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 고객에 대한 사용자 관리 - 사용자 계정을 만들고, 사용자 라이선스를 추가 또는 제거하고, 암호를 재설정하고, 사용자 계정을 삭제하거나 복원합니다.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149896"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>고객 계정에 대한 사용자 및 사용자 라이선스 관리 

**적절한 역할:** 전역 관리자 | 사용자 관리 관리자 | 관리 에이전트


고객의 계정에서 새 사용자를 만들고 삭제할 수 있습니다. 삭제 후 30일 이내에 이전에 삭제한 사용자 계정을 하나 이상 복원할 수도 있습니다. 사용자의 이전 구독 할당도 복원됩니다(이전 할당을 사용할 수 있다고 가정).

고객에 대한 새 구독을 구입하는 경우 고객은 계정이 필요한 모든 사용자 목록, 사용자 권한 및 각 사용자에게 필요한 서비스를 제공해야 합니다.  

>[!NOTE]
>**고객** 탭의 **사용자 및 라이선스** 섹션에는 다른 CSP 파트너 또는 다른 구매 채널에서 구매한 라이선스가 있는 사용자를 포함하여 특정 고객의 테넌트에서 만든 모든 사용자가 표시됩니다.

[Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)를 사용하여 이름을 가져와서 한 번에 여러 사용자에게 [구독을 할당할](bulk-license-provisioning-for-multiple-users.md) 수 있습니다.

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>고객의 사용자 계정 만들기

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서 사용자 **및 라이선스를 선택합니다.**

4. 추가하는 각 사용자에 대해 **구독 추가를** 선택한 다음, 사용 권한 및 라이선스를 포함한 정보를 입력합니다. 변경 내용을 **저장** 합니다.

5. 사용자에게 보낼 사용자 이름과 임시 암호를 기록해야 합니다.

6. 여러 사용자를 한 번에 하나씩 추가하는 경우 **다른 사용자 추가** 를 사용합니다.

7. [Excel 호환 .csv 스프레드시트 파일](adding-multiple-users-to-a-customer-account.md)를 가져와서 한 번에 여러 사용자를 추가할 수도 있습니다. 확인 화면에서 이름과 암호를 전자 메일로 보내거나 인쇄하기 전에 전체 집합을 완료할 때까지 기다릴 수 있습니다.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>고객에 대한 사용자 라이선스 추가 또는 제거

다음 단계는 Microsoft 제품에 대한 사용자 라이선스를 추가하거나 제거하는 데 적용됩니다. 상업용 Marketplace에서 라이선스 기반 SaaS 구독에 대한 사용자 라이선스를 추가하거나 제거하려면 [SaaS 구독에 대한 라이선스 추가 또는 제거를](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)참조하세요.

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서 **사용자 및 라이선스** 를 선택 합니다.

4. 목록에서 한 명 이상의 사용자를 선택합니다. 예를 들어 고객이 새 라이선스를 구매 했 고 아직 없는 사용자에 게 해당 라이선스를 할당 하려는 경우 **사용자 필터** ... 옵션을 사용 하 여 올바른 그룹을 찾을 수 있습니다.

5. **라이선스 관리** 를 선택합니다. 변경한 후 **저장** 을 클릭 합니다.

> [!NOTE]
> 제품을 게시 한 ISV (독립 소프트웨어 공급 업체)를 통해 라이선스 할당 및 활성화를 관리 하는 [Azure Marketplace 제품](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)입니다.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>고객에 대 한 사용자 암호 재설정

1. 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.

2. 파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.

3. 고객 메뉴에서 **사용자 및 라이선스** 를 선택 합니다. 목록에서 사용자를 선택합니다.

4. 화면 아래쪽에서 **암호 재설정** 을 선택 합니다. 

5. 새 임시 암호를 사용자에 게 보냅니다.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>고객에 대 한 사용자 계정 삭제

1. **파트너 센터** 메뉴에서 **고객** 을 선택 합니다. 목록에서 고객을 선택합니다.

2. 고객 메뉴에서 **사용자 및 라이선스** 를 선택 합니다. 목록에서 사용자를 선택합니다.

3. 화면 맨 아래에서 **사용자 계정 삭제** 를 선택합니다.

이 계정을 복원 해야 하는 경우 고객의 **사용자 및 라이선스** 목록의 **삭제 된 사용자** 탭에서 찾을 수 있습니다. 삭제 된 사용자를 복원 하는 데 30 일이 있습니다.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>삭제 된 사용자 계정 복원

1. **파트너 센터** 메뉴에서 **고객** 을 선택한 다음 목록에서 고객을 선택 합니다.

2. **사용자 및 라이선스** 를 선택 합니다.

3. 삭제 된 **사용자 ()** 탭을 선택 합니다. 복원할 수 있는 삭제 된 사용자가 있는 경우에는 **(1)** 이상을 읽어야 합니다.

4. 삭제 된 사용자의 확인란을 하나 이상 선택 하 고 **복원** 을 선택 합니다.

    선택한 모든 사용자 계정이 **사용자 및 라이선스** 페이지에 다시 나타납니다.

## <a name="next-steps"></a>다음 단계

- [여러 사용자에게 라이선스 할당 또는 해지](bulk-license-provisioning-for-multiple-users.md)

- [고객 계정에 대 한 여러 사용자 만들기](adding-multiple-users-to-a-customer-account.md)