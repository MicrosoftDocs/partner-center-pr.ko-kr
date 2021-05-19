---
title: 제어판 공급 업체로 등록
description: CSP 파트너 시스템을 파트너 센터 API와 더 잘 통합할 수 있도록 파트너 센터 CPV(제어판 Vendor)로 등록하는 방법을 알아봅니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147142"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="c5359-103">CSP 파트너 시스템을 파트너 센터 API와 통합하는 데 도움이 되도록 제어판 공급업체로 등록</span><span class="sxs-lookup"><span data-stu-id="c5359-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="c5359-104">**적절한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="c5359-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c5359-105">CPV(제어판 공급업체)는 CSP(클라우드 솔루션 공급자) 파트너가 사용할 애플리케이션을 개발하여 시스템을 파트너 센터 API와 통합할 수 있도록 하는 독립 소프트웨어 공급업체입니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="c5359-106">제어판 공급업체는 파트너 센터 대시보드 또는 파트너 센터 API에 직접 액세스할 수 있는 CSP 파트너가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="c5359-107">현재 CPV(제어판 공급업체) 또는 Microsoft 파트너와 협력하려는 새 CPV 중 어느 것이든 Microsoft는 이제 애플리케이션을 등록하고 클라우드 솔루션 공급자 파트너를 지원하기 위해 파트너 센터 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="c5359-108">계정을 만들기 위해 CPV 파트너는 기존 CSP 파트너 테넌트 또는 기존 CPV 테넌트를 사용하거나 온보딩 프로세스의 일부로 새 테넌트를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="c5359-109">CPV 파트너가 기존 CSP 테넌트 사용을 선택하는 경우 별도의 다중 테넌트 애플리케이션을 만들고 CPV 활동에 대한 파트너 센터 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="c5359-110">애플리케이션은 CSP 및 CPV 애플리케이션으로 등록할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="c5359-111">파트너 센터 등록하고 애플리케이션을 등록하면 파트너 센터 API에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="c5359-112">샌드박스 계정이 필요한 경우 Microsoft 지원 요청을 통해 Microsoft에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="c5359-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="c5359-113">샌드박스 계정이 이미 있는 경우 계속 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="c5359-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="c5359-114">새 샌드박스가 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-114">You won't need a new sandbox</span></span>

<span data-ttu-id="c5359-115">Microsoft [제어판 공급업체 계약](https://go.microsoft.com/fwlink/?linkid=2055198) 검토</span><span class="sxs-lookup"><span data-stu-id="c5359-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="c5359-116">파트너 센터에서 작업</span><span class="sxs-lookup"><span data-stu-id="c5359-116">Working in Partner Center</span></span>

<span data-ttu-id="c5359-117">파트너 센터 CPV 환경을 등록하고 CPV 계약에 동의하면 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="c5359-118">다중 테넌트 애플리케이션을 관리합니다(파트너 센터 애플리케이션을 Azure Portal, 등록 및 등록 취소하는 애플리케이션 추가).</span><span class="sxs-lookup"><span data-stu-id="c5359-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="c5359-119">CPV는 파트너 센터 API에 대한 권한을 얻으려면 파트너 센터 애플리케이션을 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="c5359-120">Azure Portal에 애플리케이션을 추가하는 것만으로는 파트너 센터 API에 대한 권한이 CPV 애플리케이션에 부여되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="c5359-121">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="c5359-122">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="c5359-123">전역 관리자는 CPV가 가질 수 있는 유일한 역할입니다.</span><span class="sxs-lookup"><span data-stu-id="c5359-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c5359-124">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c5359-124">Next steps</span></span>

<span data-ttu-id="c5359-125">-[파트너 센터 계정에 테넌트 추가](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="c5359-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>