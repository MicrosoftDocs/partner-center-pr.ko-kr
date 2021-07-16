---
title: 파트너 센터 Insights 역할 기반 액세스
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터 Insights 보고서를 보는 데 필요한 특정 역할에 대해 알아봅니다. 여기에는 임원 보고서 뷰어와 보고서 뷰어의 역할이 포함 됩니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 836ae2ab193437fca501dc5c5713a4fe09b49ef4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375779"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="f0d4c-104">파트너 센터 Insights 대시보드에 대 한 역할 기반 액세스 제어</span><span class="sxs-lookup"><span data-stu-id="f0d4c-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="f0d4c-105">**적절 한 역할**: 전역 관리자 | 관리 에이전트 | 보고서 뷰어 | 임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="f0d4c-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="f0d4c-106">Insights 대시보드는 파트너 센터에서 두 개의 새로운 역할을 사용 하 여 보고서-임원 보고서 뷰어와 보고서 뷰어에 대 한 직원 액세스를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="f0d4c-107">임원 보고서 뷰어 역할의 사용자는 모든 보고 데이터 집합에 액세스할 수 있으며, 보고서 뷰어 역할의 사용자는 수익 및 고객/직원 개인 데이터와 같은 중요 한 데이터 집합에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="f0d4c-108">다른 파트너 센터 역할과 마찬가지로 전역 관리자 또는 계정 관리자는 사용자 관리 페이지에서 해당 역할에 사용자를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="f0d4c-109">역할은 전체 회사 전체 또는 특정 Microsoft 파트너 네트워크 (MPN) 위치에 적용 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-109">The roles can be applicable across the entire company or for specific Microsoft Partner Network (MPN) location(s).</span></span> <span data-ttu-id="f0d4c-110">특정 MPN 위치에 대해 할당 된 역할은 사용자가 선택한 MPN 위치에만 연결 된 보고 데이터를 볼 수 있도록 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="f0d4c-111">파트너는 아래 보기에서 하나 또는 여러 위치를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/insights/roles.png" alt-text="보고서 뷰어 및 임원 보고서 뷰어에 대 한 위치 관련 파트너 센터 Insights 역할 설정을 표시 합니다.":::

>[!Note]
> <span data-ttu-id="f0d4c-113">2020 년 1 월 20 일에 MPN 파트너 관리자 인 사용자는 해당 테 넌 트의 모든 위치에 대 한 회사 전체의 **임원 보고서 뷰어** 역할에 자동으로 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-113">Users who are MPN partner admins as of January 20, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="f0d4c-114">따라서 이러한 사용자는 전역 관리자 또는 계정 관리자에 게 필요한 명시적인 조치 없이도 보고서를 임원 보고서 뷰어로 액세스할 수 있습니다. 전역 관리자 및 계정 관리자는 이러한 사용자의 자동 할당 된 역할을 재정의 하 여 해당 기능을 추가로 늘리거나 제한할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f0d4c-115">다음 단계</span><span class="sxs-lookup"><span data-stu-id="f0d4c-115">Next steps</span></span>

- <span data-ttu-id="f0d4c-116">[파트너 센터 Insights](partner-center-insights.md) 와 다양 한 보고서에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="f0d4c-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
