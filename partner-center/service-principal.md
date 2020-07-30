---
title: Azure AD 서비스 사용자
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD 테넌트에 서비스 사용자를 추가하는 방법을 알아봅니다. 이렇게 하면 파트너 센터에서 Azure AD 애플리케이션(서비스 사용자)을 추가하는 것을 의미합니다.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d75c5c7311feaa3ca53139f2abf2702035b1069
ms.sourcegitcommit: 2e206627323ff175c0e0d10646cdba80e9881891
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87365759"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="824c3-104">파트너 센터에서 Azure AD 애플리케이션(서비스 사용자) 추가</span><span class="sxs-lookup"><span data-stu-id="824c3-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="824c3-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="824c3-105">**Applies to**</span></span>

- <span data-ttu-id="824c3-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="824c3-106">Partner Center</span></span>

<span data-ttu-id="824c3-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="824c3-107">**Appropriate roles**</span></span>

- <span data-ttu-id="824c3-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="824c3-108">Global admin</span></span>

<span data-ttu-id="824c3-109">파트너 센터의 상용 마켓플레이스 프로그램에서 이제 Azure AD 애플리케이션(서비스 사용자)을 파트너 센터 계정의 사용자로 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="824c3-110">(이전에 Cloud 파트너 포털 또는 CPP 계정에서 이 작업을 수행할 수 있었습니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="824c3-111">파트너 센터로 마이그레이션되었으므로 CPP 계정은 읽기 전용입니다.)</span><span class="sxs-lookup"><span data-stu-id="824c3-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="824c3-112">서비스 사용자는 Azure AD 애플리케이션과 동의어입니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="824c3-113">Azure AD 애플리케이션(서비스 사용자) 추가</span><span class="sxs-lookup"><span data-stu-id="824c3-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="824c3-114">파트너 센터 대시보드에서 **설정**을 선택한 다음, **개발자 설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="824c3-115">**사용자**를 선택한 다음, **Azure AD 애플리케이션 추가**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="824c3-116">기존 Azure AD 애플리케이션을 선택하거나 새로 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="824c3-117">새 Azure AD 애플리케이션을 만드는 경우 다음 정보를 포함시킵니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="824c3-118">**회신 URL**: 사용자가 Azure AD 애플리케이션을 사용하기 위해 로그인할 수 있는 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="824c3-119">**앱 ID URI**: Azure AD에 Single Sign-On 요청을 보낼 때 제공되는 Azure AD 애플리케이션의 논리적 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="824c3-120">**보안 역할**: **관리자** 역할(CPP의 '소유자' 역할과 동일) 및 **개발자** 역할(CPP의 '기여자' 역할과 동일)은 파트너 센터의 상업용 마켓플레이스 프로그램에 적용되며, 이 Azure AD 애플리케이션과 연결될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="824c3-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="824c3-121">다음 단계</span><span class="sxs-lookup"><span data-stu-id="824c3-121">Next steps</span></span>

- [<span data-ttu-id="824c3-122">파트너 센터의 상업용 Marketplace 개요</span><span class="sxs-lookup"><span data-stu-id="824c3-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)