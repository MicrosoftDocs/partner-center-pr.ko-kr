---
title: 테 넌 트 ID, 도메인 이름, 사용자 개체 ID 찾기
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Portal에서 Id를 찾는 방법에 대해 알아봅니다. 조직의 Azure AD 테 넌 트 ID, 도메인 이름 또는 특정 사용자 개체 ID입니다. 일부 작업에는이 정보가 필요 합니다.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360074"
---
# <a name="locate-important-ids-for-a-user"></a>사용자에 대 한 중요 한 Id 찾기

이 문서에서는 [Azure Portal](https://portal.azure.com/) 를 사용 하 여 사용자에 대 한 다음 정보를 찾는 방법을 설명 합니다.

- 사용자의 조직 또는 회사의 Microsoft Azure Active Directory (Azure AD) 테 넌 트 ID

- Azure AD 테 넌 트와 연결 된 조직 또는 회사의 주 도메인 이름

- 사용자 개체 ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Microsoft Azure AD 테 넌 트 ID 및 주 도메인 이름 찾기

Azure Portal 내에서 Azure AD 테 넌 트 ID 또는 주 도메인 이름을 찾으려면 다음 단계를 수행 합니다. (테 넌 트 ID를 프로그래밍 방식으로 찾으려면 [PowerShell 또는 CLI를 사용 하 여 테 넌 트 Id 찾기](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)를 참조 하세요.)

> [!NOTE]
> 테 넌 트 ID는 다른 응용 프로그램 또는 리소스에서 다른 이름으로 호출 될 수 있습니다. 예를 들어 테 넌 트 ID를 디렉터리 ID, Azure Active Directory (Azure AD) 테 넌 트, Microsoft ID 또는 *tenantguid* 를 비롯 한 특정 보고서에 대해 참조할 수 있습니다.

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.

2. 메뉴에서 **Azure Active Directory** 를 선택합니다.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="메뉴에서 Azure Active Directory 옵션을 선택 하 Azure Portal 표시 합니다.":::

3. Azure Active Directory **개요** 페이지가 나타납니다. Azure AD 테 넌 트 ID 또는 주 도메인 이름을 찾으려면 **테 넌 트 id** 필드 및 **주 도메인** 필드를 확인 합니다. 이러한 필드는 테 넌 트 정보 섹션에 표시 됩니다.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="두 개의 강조 표시 된 필드, 테 넌 트 ID 및 주 도메인 이름이 있는 개요 페이지를 표시 합니다.":::

4. Azure Portal에서 테 넌 트 ID는 몇 가지 다른 방법으로 찾을 수 있습니다. 메뉴에서 **Azure Active Directory** 를 선택합니다. 그런 다음 메뉴에서 **관리** 섹션을 찾아 **속성** 을 선택 합니다.

   속성 페이지에는 사용자의 연결 된 테 넌 트 ID도 표시 됩니다.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="강조 표시 된 테 넌 트 ID 필드가 있는 속성 페이지를 표시 합니다.":::

## <a name="find-the-user-object-id"></a>사용자 개체 ID 찾기

도메인 이름 및 테 넌 트 ID를 찾는 것 만으로는 항상 충분 하지 않을 수 있습니다. 사용자에 게 할당 된 특정 개체 ID를 찾아야 할 수도 있습니다. Azure Portal에서 사용자의 개체 ID를 찾으려면 다음 단계를 수행 합니다.

1. [Azure Portal](https://portal.azure.com/)에 로그인합니다.

2. 메뉴에서 **Azure Active Directory** 를 선택합니다.

3. 메뉴에서 **관리** 섹션을 찾은 다음 **사용자** 를 선택 합니다.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="강조 표시 된 사용자 옵션을 사용 하 여 Azure Active Directory 메뉴를 표시 합니다.":::

4. 사용자 페이지의 검색 상자에 사용자 이름을 입력 합니다.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="특정 사용자를 검색 하는 검색 상자가 있는 사용자 페이지를 표시 합니다.":::

5. 목록에 표시 되는 사용자 이름을 선택 합니다.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="검색 된 사용자에 대 한 행을 표시 하는 사용자 페이지를 표시 합니다.":::

6. 사용자의 프로필 페이지에서 Id 섹션을 찾습니다. 개체 ID 필드는 사용자의 고유 개체 ID와 함께 여기에 표시 됩니다.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id 섹션이 있는 사용자 프로필 페이지 및 개체 ID에 대해 하나의 강조 표시 된 필드를 표시 합니다.":::

## <a name="next-steps"></a>다음 단계

- [PowerShell 또는 CLI를 사용 하 여 프로그래밍 방식으로 테 넌 트 ID 찾기](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Azure Active Directory의 사용자 프로필에 대 한 자세한 정보](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [파트너가 파트너 센터에서 고객 세부 정보를 보거나 내보내는 방법 알아보기](see-your-customer-list.md)
