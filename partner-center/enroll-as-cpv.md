---
title: 제어판 공급 업체로 등록
description: 파트너 센터 Api와 CSP 파트너 시스템을 더 효율적으로 통합할 수 있도록 파트너 센터에서 CPV (제어판 공급 업체)로 등록 하는 방법에 대해 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560513"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="012e7-103">CSP 파트너 시스템을 파트너 센터 API와 통합하는 데 도움이 되도록 제어판 공급업체로 등록</span><span class="sxs-lookup"><span data-stu-id="012e7-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="012e7-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="012e7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="012e7-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="012e7-105">Global admin</span></span>

<span data-ttu-id="012e7-106">CPV (제어판 공급 업체)는 CSP (클라우드 솔루션 공급자) 파트너가 시스템을 파트너 센터 Api와 통합할 수 있도록 응용 프로그램을 개발 하는 독립 소프트웨어 공급 업체입니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="012e7-107">제어판 공급 업체는 파트너 센터 대시보드 또는 파트너 센터 Api에 직접 액세스할 수 있는 CSP 파트너가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="012e7-108">현재는 CPV (현재 제어판 공급 업체) 또는 Microsoft 파트너와 함께 작업 하고자 하는 새 CPV를 사용 하 여 응용 프로그램을 등록 하 고 클라우드 솔루션 공급자 파트너를 지원 하기 위해 이제 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="012e7-109">계정을 만들기 위해 CPV 파트너는 기존 CSP 파트너 테 넌 트 또는 기존 CPV 테 넌 트를 사용 하거나 온 보 딩 프로세스의 일부로 새 테 넌 트를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="012e7-110">CPV 파트너가 기존 CSP 테 넌 트를 사용 하도록 선택 하는 경우 별도의 다중 테 넌 트 응용 프로그램을 만들고이를 CPV 활동의 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="012e7-111">응용 프로그램을 CSP 및 CPV 응용 프로그램으로 등록할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="012e7-112">파트너 센터에 등록 하 고 응용 프로그램을 등록 한 후에는 파트너 센터 Api에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="012e7-113">샌드박스 계정이 필요한 경우 Microsoft 지원 요청을 통해 Microsoft에 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="012e7-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="012e7-114">샌드박스 계정이 이미 있는 경우 계속 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="012e7-115">새 샌드박스가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-115">You won't need a new sandbox</span></span>

<span data-ttu-id="012e7-116">[Microsoft 제어판 공급 업체 규약](https://go.microsoft.com/fwlink/?linkid=2055198) 검토</span><span class="sxs-lookup"><span data-stu-id="012e7-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="012e7-117">파트너 센터에서 작업</span><span class="sxs-lookup"><span data-stu-id="012e7-117">Working in Partner Center</span></span>

<span data-ttu-id="012e7-118">파트너 센터 CPV 환경을 등록 하 고 CPV 규약을 승인한 후 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="012e7-119">다중 테 넌 트 응용 프로그램을 관리 합니다 (파트너 센터에서 응용 프로그램을 Azure Portal, 등록 및 등록 취소 하는 응용 프로그램 추가).</span><span class="sxs-lookup"><span data-stu-id="012e7-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="012e7-120">CPVs는 파트너 센터 Api에 대 한 권한을 부여 받으려면 파트너 센터에서 해당 응용 프로그램을 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="012e7-121">Azure Portal에 애플리케이션을 추가하는 것만으로는 파트너 센터 API에 대한 권한이 CPV 애플리케이션에 부여되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="012e7-122">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="012e7-123">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="012e7-124">전역 관리자는 CPV가 가질 수 있는 유일한 역할입니다.</span><span class="sxs-lookup"><span data-stu-id="012e7-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="012e7-125">다음 단계</span><span class="sxs-lookup"><span data-stu-id="012e7-125">Next steps</span></span>

<span data-ttu-id="012e7-126">-[파트너 센터 계정에 테 넌 트 추가](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="012e7-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>