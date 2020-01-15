---
title: 파트너 센터 정보-역할 기반 액세스 제어 | 파트너 센터
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 정보 보고서를 보려면 특정 역할이 필요 합니다.
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI, 성능, 고객 성공, 측정, 역할
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945865"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="ec55a-104">Insights 대시보드에 대 한 역할 기반 액세스 제어</span><span class="sxs-lookup"><span data-stu-id="ec55a-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="ec55a-105">Insights 대시보드는 파트너 센터에서 두 개의 새로운 역할을 사용 하 여 보고서-임원 보고서 뷰어와 보고서 뷰어에 대 한 직원 액세스를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="ec55a-106">임원 보고서 뷰어 역할의 사용자는 모든 보고 데이터 집합에 액세스할 수 있으며, 보고서 뷰어 역할의 사용자는 수익 및 고객/직원 개인 데이터와 같은 중요 한 데이터 집합에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="ec55a-107">다른 파트너 센터 역할과 마찬가지로 전역 관리자 또는 계정 관리자는 사용자 관리 페이지에서 해당 역할에 사용자를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="ec55a-108">역할은 전체 회사 또는 특정 MPN 위치에서 적용 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="ec55a-109">특정 MPN 위치에 대해 할당 된 역할은 사용자가 선택한 MPN 위치에만 연결 된 보고 데이터를 볼 수 있도록 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="ec55a-110">파트너는 아래 보기에서 하나 또는 여러 위치를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-110">Partner can select one or multiple locations from the below view.</span></span>

![역할](images/pci/roles.png)

><span data-ttu-id="ec55a-112">두고 MPN 관리자가 1 월 20, 2020 인 사용자는 해당 테 넌 트의 모든 위치에 대 한 회사 전체의 ' 임원 보고서 뷰어 ' 역할에 자동으로 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="ec55a-113">따라서 이러한 사용자는 전역 관리자 또는 계정 관리자에 게 필요한 명시적인 조치 없이도 보고서를 임원 보고서 뷰어로 액세스할 수 있습니다. 전역 관리자 및 계정 관리자는 이러한 사용자의 자동 할당 된 역할을 재정의 하 여 해당 기능을 추가로 늘리거나 제한할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec55a-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>