---
title: Azure AD 서비스 사용자| 파트너 센터
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD 테넌트에 서비스 사용자 추가
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure 플랜, 서비스 사용자, Azure AD 애플리케이션
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2020
ms.locfileid: "75716894"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="98656-104">파트너 센터에서 Azure AD 애플리케이션(서비스 사용자) 추가</span><span class="sxs-lookup"><span data-stu-id="98656-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="98656-105">파트너 센터의 상용 마켓플레이스 프로그램에서 이제 Azure AD 애플리케이션(서비스 사용자)을 파트너 센터 계정의 사용자로 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98656-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="98656-106">(이전에 CPP(Cloud Partner Portal) 계정에서 이 작업을 수행할 수 있었지만, 이제 파트너 센터로 마이그레이션했으므로 CPP 계정은 읽기 전용입니다.) 서비스 사용자는 Azure AD 애플리케이션과 동의어입니다.</span><span class="sxs-lookup"><span data-stu-id="98656-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="98656-107">Azure AD 애플리케이션(서비스 사용자) 추가</span><span class="sxs-lookup"><span data-stu-id="98656-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="98656-108">파트너 센터 대시보드에서 **설정**을 선택한 다음, **개발자 설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="98656-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="98656-109">**사용자**를 선택한 다음, **Azure AD 애플리케이션 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="98656-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="98656-110">기존 Azure AD 애플리케이션을 선택하거나 새로 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="98656-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="98656-111">새 Azure AD 애플리케이션을 만드는 경우 다음 정보를 포함시킵니다.</span><span class="sxs-lookup"><span data-stu-id="98656-111">If you create a new Azure AD Application, include the following information:</span></span>  

  


<span data-ttu-id="98656-112">**회신 URL**: 사용자가 Azure AD 애플리케이션을 사용하기 위해 로그인할 수 있는 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="98656-112">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="98656-113">**앱 ID URI**: Azure AD에 Single Sign-On 요청을 보낼 때 제공되는 Azure AD 애플리케이션의 논리적 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="98656-113">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="98656-114">**보안 역할**: **관리자** 역할(CPP의 '소유자' 역할과 동일) 및 **개발자** 역할(CPP의 '기여자' 역할과 동일)은 파트너 센터의 상업용 마켓플레이스 프로그램에 적용되며, 이 Azure AD 애플리케이션과 연결될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="98656-114">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

  
