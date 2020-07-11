---
title: 제어판 공급 업체로 등록
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 파트너 센터에서 CPV (제어판 공급 업체)로 등록 하는 방법에 대해 알아봅니다.
author: kbangalore
ms.author: kiranban
keywords: 제어판 공급 업체, CPV 앱 등록, CPV 앱 관리
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 819c814333878efc882749a1597e993eb9002545
ms.sourcegitcommit: 13b0e1358dc306f896190088d31a0d883644850f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/10/2020
ms.locfileid: "86219611"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="4aa62-104">CSP 파트너 시스템을 파트너 센터 Api와 통합 하는 데 도움이 되는 제어판 공급 업체로 등록</span><span class="sxs-lookup"><span data-stu-id="4aa62-104">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="4aa62-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="4aa62-105">**Applies to**</span></span>

- <span data-ttu-id="4aa62-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4aa62-106">Partner Center</span></span>

<span data-ttu-id="4aa62-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="4aa62-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4aa62-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="4aa62-108">Global admin</span></span>

<span data-ttu-id="4aa62-109">CPV (제어판 공급 업체)는 CSP (클라우드 솔루션 공급자) 파트너가 시스템을 파트너 센터 Api와 통합할 수 있도록 응용 프로그램을 개발 하는 독립 소프트웨어 공급 업체입니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-109">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="4aa62-110">제어판 공급 업체는 파트너 센터 대시보드 또는 파트너 센터 Api에 직접 액세스할 수 있는 CSP 파트너가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-110">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="4aa62-111">현재는 CPV (현재 제어판 공급 업체) 또는 Microsoft 파트너와 함께 작업 하고자 하는 새 CPV를 사용 하 여 응용 프로그램을 등록 하 고 클라우드 솔루션 공급자 파트너를 지원 하기 위해 이제 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-111">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="4aa62-112">계정을 만들기 위해 CPV 파트너는 기존 CSP 파트너 테 넌 트 또는 기존 CPV 테 넌 트를 사용 하거나 온 보 딩 프로세스의 일부로 새 테 넌 트를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-112">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="4aa62-113">CPV 파트너가 기존 CSP 테 넌 트를 사용 하도록 선택 하는 경우 별도의 다중 테 넌 트 응용 프로그램을 만들고이를 CPV 활동의 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-113">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="4aa62-114">응용 프로그램을 CSP 및 CPV 응용 프로그램으로 등록할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-114">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="4aa62-115">파트너 센터에 등록 하 고 응용 프로그램을 등록 한 후에는 파트너 센터 Api에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-115">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="4aa62-116">Microsoft는 샌드박스 정보를 사용 하 여 파트너 센터 알림을 통해 사용자에 게 연락 합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-116">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="4aa62-117">샌드박스 계정이 이미 있는 경우 계속 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-117">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="4aa62-118">새 샌드박스가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-118">You won't need a new sandbox.</span></span>

<span data-ttu-id="4aa62-119">[Microsoft 제어판 공급 업체 규약](https://go.microsoft.com/fwlink/?linkid=2055198) 검토</span><span class="sxs-lookup"><span data-stu-id="4aa62-119">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="4aa62-120">파트너 센터에서 작업</span><span class="sxs-lookup"><span data-stu-id="4aa62-120">Working in Partner Center</span></span>
<span data-ttu-id="4aa62-121">파트너 센터 CPV 환경을 등록 하 고 CPV 규약을 승인한 후 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-121">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="4aa62-122">다중 테 넌 트 응용 프로그램을 관리 합니다 (파트너 센터에서 응용 프로그램을 Azure Portal, 등록 및 등록 취소 하는 응용 프로그램 추가).</span><span class="sxs-lookup"><span data-stu-id="4aa62-122">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="4aa62-123">CPVs는 파트너 센터 Api에 대 한 권한을 부여 받으려면 파트너 센터에서 해당 응용 프로그램을 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-123">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="4aa62-124">Azure Portal에 애플리케이션을 추가하는 것만으로는 파트너 센터 API에 대한 권한이 CPV 애플리케이션에 부여되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-124">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="4aa62-125">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-125">View and manage your CPV profile</span></span> 

- <span data-ttu-id="4aa62-126">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-126">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="4aa62-127">전역 관리자는 CPV가 가질 수 있는 유일한 역할입니다.</span><span class="sxs-lookup"><span data-stu-id="4aa62-127">Global admin is the only role a CPV can have.</span></span>


