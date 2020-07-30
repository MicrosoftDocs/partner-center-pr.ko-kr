---
title: 파트너 센터 계정에 테 넌 트 추가
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 계정을 통해 여러 테 넌 트 관리
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389518"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="399e2-103">파트너 센터 계정에서 여러 테 넌 트 추가 및 관리</span><span class="sxs-lookup"><span data-stu-id="399e2-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="399e2-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="399e2-104">**Applies to**</span></span>

- <span data-ttu-id="399e2-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="399e2-105">Partner Center</span></span>

<span data-ttu-id="399e2-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="399e2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="399e2-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="399e2-107">Global admin</span></span>

<span data-ttu-id="399e2-108">파트너 센터 계정에서 여러 Azure AD 테 넌 트를 관리 해야 하는 이유는 여러 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="399e2-109">예를 들어 회사에서 다른 회사를 구매 하 고 새 회사의 직원이 파트너 센터를 사용할 수 있도록 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="399e2-110">그러나 두 회사를 분리 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="399e2-111">이 경우 새 회사의 Azure AD 테 넌 트를 파트너의 PNG (global account)와 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="399e2-112">이 연결을 통해 두 회사의 사용자가 파트너 센터에서 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="399e2-113">계정에 다른 Azure AD 테 넌 트 추가</span><span class="sxs-lookup"><span data-stu-id="399e2-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="399e2-114">전역 관리자 권한으로 파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="399e2-115">**설정** 아이콘에서 **계정 설정** 을 선택 하 고 **테 넌 트**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="테 넌 트 연결"::: 

3. <span data-ttu-id="399e2-117">**다른 AD 테 넌 트 연결** 을 선택 하 고 연결 하려는 테 넌 트를 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="399e2-118">전역 관리자 권한으로 연결 하려는 테 넌 트에 로그인 하 고 연결을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="테 넌 트 연결 확인"::: 

5. <span data-ttu-id="399e2-120">확인 한 후에는 **모든 설정** 된 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="399e2-121">**테 넌 트 관리로 돌아가기** 를 선택 하면 새로 추가 된 테 넌 트가 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="399e2-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="399e2-122">다음 단계</span><span class="sxs-lookup"><span data-stu-id="399e2-122">Next steps</span></span>

- [<span data-ttu-id="399e2-123">사용자 추가</span><span class="sxs-lookup"><span data-stu-id="399e2-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
