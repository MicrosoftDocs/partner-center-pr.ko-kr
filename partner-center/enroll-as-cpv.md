---
title: 패널 컨트롤 공급 업체와 파트너 센터에 등록 | 파트너 센터
ms.topic: article
ms.date: 12/11/2018
Description: 패널 컨트롤 공급 업체와 파트너 센터에 등록 하는 방법
author: LauraBrenner
ms.author: labrenne
keywords: 패널 공급 업체를 제어, CPV 앱을 등록, CPV 앱 관리
ms.localizationpriority: medium
ms.openlocfilehash: 7d00cfc7addf120a3b42597cda3758597533dd5e
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586056"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="8412a-104">패널 컨트롤 공급 업체와 파트너 센터에 등록</span><span class="sxs-lookup"><span data-stu-id="8412a-104">Enroll in Partner Center as a Control Panel Vendor</span></span>

<span data-ttu-id="8412a-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="8412a-105">**Applies to**</span></span>

- <span data-ttu-id="8412a-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="8412a-106">Partner Center</span></span>

<span data-ttu-id="8412a-107">컨트롤 패널 공급 업체 (CPV)는 파트너 센터 Api를 사용 하 여 해당 시스템을 통합할 수 있도록 클라우드 솔루션 공급자 (CSP) 파트너에서 사용 하기 위해 응용 프로그램을 개발 하는 독립 소프트웨어 공급 업체입니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-107">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="8412a-108">제어판 공급 업체 파트너 센터 대시보드에서에 대 한 직접 액세스를 사용 하 여 CSP 파트너 또는 파트너 센터 Api가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-108">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="8412a-109">필요한 지 여부를 현재 컨트롤 패널 공급 업체 (CPV) 또는 Microsoft 파트너를 사용 하려는 새 CPV 인 Microsoft 이제 응용 프로그램을 등록 하 고 클라우드 솔루션 공급자 파트너를 지원 하기 위해 파트너 센터에 등록 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-109">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="8412a-110">계정을 만들려면 CPV 파트너는 기존 CSP 파트너 테 넌 트 또는 기존 CPV 테 넌 트를 사용 또는 새 테 넌 트 온 보 딩 프로세스의 일부로 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-110">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="8412a-111">CPV 파트너는 기존 CSP 테 넌 트를 사용 하도록 선택 하면 다음 해야 별도 다중 테 넌 트 응용 프로그램을 만들고 CPV 활동에 대 한 파트너 센터에 등록 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-111">If the CPV partner chooses to use the existing CSP tenant, then they’ll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="8412a-112">CSP 및 CPV 응용 프로그램으로 응용 프로그램을 등록할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-112">An application can’t be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="8412a-113">파트너 센터에 등록 하 여 응용 프로그램 등록 후에 파트너 센터 Api에 대 한 액세스를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-113">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="8412a-114">Microsoft는 샌드박스 정보를 사용 하 여 파트너 센터 알림을 통해 연락 드립니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-114">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="8412a-115">그러나 이미 있다면 샌드박스 계정을 계속 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-115">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="8412a-116">새 샌드박스를 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-116">You won’t need a new sandbox.</span></span>   

<span data-ttu-id="8412a-117">검토를 [Microsoft 컨트롤 패널 공급 업체 규약](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="8412a-117">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="8412a-118">파트너 센터에서 작업</span><span class="sxs-lookup"><span data-stu-id="8412a-118">Working in Partner Center</span></span>
<span data-ttu-id="8412a-119">파트너 센터 CPV 환경에 등록 하 고 있습니다 CPV 계약을 수락 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-119">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="8412a-120">(Azure portal에 응용 프로그램 등록 및 파트너 센터에서 응용 프로그램을 등록 취소 추가) 하는 다중 테 넌 트 응용 프로그램을 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-120">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="8412a-121">CPVs는 파트너 센터 Api에 대 한 권한을 받기 위해 파트너 센터에서 응용 프로그램을 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-121">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="8412a-122">단독으로 Azure portal에 응용 프로그램 추가 CPV 응용 프로그램 파트너 센터 Api에 대 한 권한을 부여 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-122">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="8412a-123">보기 및 CPV 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="8412a-123">View and manage your CPV profile</span></span> 

- <span data-ttu-id="8412a-124">보기 및 CPV 기능에 대 한 액세스가 필요한 사용자를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="8412a-124">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="8412a-125">역할만 CPV 있을 수 있습니다. 전역 관리자는</span><span class="sxs-lookup"><span data-stu-id="8412a-125">The only role a CPV can have is global admin.</span></span>


