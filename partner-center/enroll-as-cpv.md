---
title: 컨트롤 패널 공급 업체와 파트너 센터에 등록 | 파트너 센터
ms.topic: article
ms.date: 12/11/2018
Description: How to enroll in Partner Center as a Control Panel Vendor
author: labrenne
ms.author: labrenne
keywords: 패널 공급 업체 제어, CPV 앱을 등록, CPV 앱 관리
ms.localizationpriority: medium
ms.openlocfilehash: 687165520ca68d390ad2ca0d5468085734de7755
ms.sourcegitcommit: 92f5e5c3d42d968719d70b1cadc021a918fdd97e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2018
ms.locfileid: "8963065"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="b4c92-103">컨트롤 패널 공급 업체와 파트너 센터에 등록</span><span class="sxs-lookup"><span data-stu-id="b4c92-103">Enroll in Partner Center as a Control Panel Vendor</span></span>

**<span data-ttu-id="b4c92-104">적용 대상</span><span class="sxs-lookup"><span data-stu-id="b4c92-104">Applies to</span></span>**

- <span data-ttu-id="b4c92-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b4c92-105">Partner Center</span></span>

<span data-ttu-id="b4c92-106">컨트롤 패널 공급 업체 (CPV) 파트너 센터 Api를 사용 하 여 시스템을 통합할 수 있도록 클라우드 솔루션 공급자 (CSP) 파트너가 사용 하기 위해 응용 프로그램을 개발 하는 독립 소프트웨어 공급 업체입니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="b4c92-107">제어판 공급 업체는 CSP 파트너는 파트너 센터 대시보드에서에 직접 액세스할 수 있는 또는 파트너 센터 Api가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="b4c92-108">CSP 파트너에 게 CPV 서비스를 제공 하려면 파트너 센터 계정을 만들고 CPV 파트너로 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-108">To provide CPV services to CSP partners, Partner Center requires you to create an account and enroll as a CPV partner.</span></span> <span data-ttu-id="b4c92-109">파트너 센터에 등록 된 응용 프로그램을 등록 한 후 파트너 센터 Api에 액세스를 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-109">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="b4c92-110">Microsoft에서 샌드박스 정보에 연락 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-110">Microsoft will contact you with your sandbox information.</span></span> <span data-ttu-id="b4c92-111">그러나 샌드박스 계정이 이미 있는지, 하는 경우 계속 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-111">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="b4c92-112">새 샌드박스가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-112">You won’t need a new sandbox.</span></span> 


## <a name="working-in-partner-center"></a><span data-ttu-id="b4c92-113">파트너 센터에서 작업</span><span class="sxs-lookup"><span data-stu-id="b4c92-113">Working in Partner Center</span></span>
<span data-ttu-id="b4c92-114">파트너 센터 CPV 환경에 등록 하 고 하면 CPV 계약을 수락 했습니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-114">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="b4c92-115">다중 테 넌 트 응용 프로그램 (응용 프로그램 Azure 포털을 파트너 센터에서 응용 프로그램을 등록 하 고 응용 프로그램을 등록 취소 추가)을 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-115">Manage multi-tenant applications (add applications to Azure portal, register applications in Partner Center, and unregister applications).</span></span>

>[!Note] 
><span data-ttu-id="b4c92-116">CPVs는 파트너 센터 Api에 액세스 하기 위해 파트너 센터에서 응용 프로그램을 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-116">CPVs must register their applications in Partner Center in order to get access to Partner Center APIs.</span></span> <span data-ttu-id="b4c92-117">만 Azure 포털에 응용 프로그램을 추가 하는 파트너 센터 Api에 대 한 응용 프로그램 CPV 승인 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-117">Adding applications to the Azure portal alone does not authorize CPV applications for partner Center APIs.</span></span>

- <span data-ttu-id="b4c92-118">CPV 프로필 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="b4c92-118">View and manage your CPV profile</span></span> 

- <span data-ttu-id="b4c92-119">보고 CPV 기능에 대 한 사용자 액세스를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4c92-119">View and manage user access to CPV capabilities.</span></span> <span data-ttu-id="b4c92-120">CPV 파트너 센터 역할은 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="b4c92-120">The CPV Partner Center role is global admin.</span></span>


