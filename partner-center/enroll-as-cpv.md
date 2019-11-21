---
title: 파트너 센터에서 제어판 공급 업체로 등록 | 파트너 센터
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 파트너 센터에서 CPV (제어판 공급 업체)로 등록 하는 방법에 대해 알아봅니다.
author: LauraBrenner
ms.author: labrenne
keywords: 제어판 공급 업체, CPV 앱 등록, CPV 앱 관리
ms.localizationpriority: medium
ms.openlocfilehash: 0edc8aed269f992738f39b6250e51ec5f694727c
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253576"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="9ac86-104">파트너 센터에서 제어판 공급 업체로 등록</span><span class="sxs-lookup"><span data-stu-id="9ac86-104">Enroll in Partner Center as a Control Panel Vendor</span></span>

<span data-ttu-id="9ac86-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="9ac86-105">**Applies to**</span></span>

- <span data-ttu-id="9ac86-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="9ac86-106">Partner Center</span></span>

<span data-ttu-id="9ac86-107">CPV (제어판 공급 업체)는 CSP (클라우드 솔루션 공급자) 파트너가 시스템을 파트너 센터 Api와 통합할 수 있도록 응용 프로그램을 개발 하는 독립 소프트웨어 공급 업체입니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-107">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="9ac86-108">제어판 공급 업체는 파트너 센터 대시보드 또는 파트너 센터 Api에 직접 액세스할 수 있는 CSP 파트너가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-108">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="9ac86-109">현재는 CPV (현재 제어판 공급 업체) 또는 Microsoft 파트너와 함께 작업 하고자 하는 새 CPV를 사용 하 여 응용 프로그램을 등록 하 고 클라우드 솔루션 공급자 파트너를 지원 하기 위해 이제 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-109">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="9ac86-110">계정을 만들기 위해 CPV 파트너는 기존 CSP 파트너 테 넌 트 또는 기존 CPV 테 넌 트를 사용 하거나 온 보 딩 프로세스의 일부로 새 테 넌 트를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-110">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="9ac86-111">CPV 파트너가 기존 CSP 테 넌 트를 사용 하도록 선택 하는 경우 별도의 다중 테 넌 트 응용 프로그램을 만들고이를 CPV 활동의 파트너 센터에 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-111">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="9ac86-112">응용 프로그램을 CSP 및 CPV 응용 프로그램으로 등록할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-112">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="9ac86-113">파트너 센터에 등록 하 고 응용 프로그램을 등록 한 후에는 파트너 센터 Api에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-113">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="9ac86-114">Microsoft는 샌드박스 정보를 사용 하 여 파트너 센터 알림을 통해 사용자에 게 연락 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-114">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="9ac86-115">그러나 샌드박스 계정이 이미 있는 경우 계속 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-115">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="9ac86-116">새 샌드박스가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-116">You won't need a new sandbox.</span></span>   

<span data-ttu-id="9ac86-117">[Microsoft 제어판 공급 업체 규약](https://go.microsoft.com/fwlink/?linkid=2055198) 검토</span><span class="sxs-lookup"><span data-stu-id="9ac86-117">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="9ac86-118">파트너 센터에서 작업</span><span class="sxs-lookup"><span data-stu-id="9ac86-118">Working in Partner Center</span></span>
<span data-ttu-id="9ac86-119">파트너 센터 CPV 환경에 등록 하 고 CPV 규약을 승인한 후 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-119">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="9ac86-120">다중 테 넌 트 응용 프로그램 관리 (파트너 센터에서 응용 프로그램을 Azure Portal에 추가 하 고 등록 및 등록 취소).</span><span class="sxs-lookup"><span data-stu-id="9ac86-120">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="9ac86-121">CPVs는 파트너 센터 Api에 대 한 권한을 부여 받으려면 파트너 센터에서 해당 응용 프로그램을 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-121">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="9ac86-122">Azure Portal에 애플리케이션을 추가하는 것만으로는 파트너 센터 API에 대한 권한이 CPV 애플리케이션에 부여되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-122">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="9ac86-123">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-123">View and manage your CPV profile</span></span> 

- <span data-ttu-id="9ac86-124">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-124">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="9ac86-125">CPV가 가질 수 있는 유일한 역할은 전역 관리자입니다.</span><span class="sxs-lookup"><span data-stu-id="9ac86-125">The only role a CPV can have is global admin.</span></span>


