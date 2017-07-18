---
title: "Azure Active Directory 테넌트 및 파트너 센터 | 파트너 센터"
description: "파트너 센터 계정을 만들려면 회사에 Azure AD(Azure Active Directory) 테넌트가 있어야 합니다. Azure AD는 Microsoft의 클라우드 기반 디렉터리 및 ID 관리 서비스입니다."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="b7e63-104">Azure Active Directory 테넌트 및 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b7e63-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="b7e63-105">적용 대상</span><span class="sxs-lookup"><span data-stu-id="b7e63-105">Applies to</span></span>**

-  <span data-ttu-id="b7e63-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b7e63-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="b7e63-107">Azure AD 테넌트가 필요한 이유</span><span class="sxs-lookup"><span data-stu-id="b7e63-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="b7e63-108">테넌트 사용자가 자신의 Azure AD(Microsoft 계정) 사용자 이름 및 암호를 사용하여 파트너 센터에 로그인 할 수 있도록 조직의 Azure AD 테넌트를 새 파트너 센터 계정에 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="b7e63-109">회사에 이미 Azure AD 테넌트가 있는 경우 해당 테넌트를 파트너 센터 계정에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="b7e63-110">참고</span><span class="sxs-lookup"><span data-stu-id="b7e63-110">Note</span></span>**<br> <span data-ttu-id="b7e63-111">기존 Azure AD 테넌트를 사용하기로 결정하기 전에 테넌트의 사용자 중 파트너 센터에서 작업해야 하는 인원이 몇 명인지 생각해 보세요.</span><span class="sxs-lookup"><span data-stu-id="b7e63-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="b7e63-112">파트너 센터에서 작업할 필요가 없는 사용자가 테넌트에 포함된 경우 파트너 센터에서 작업해야 하는 사용자만을 위한 새 테넌트를 만드는 방안을 고려해 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="b7e63-113">회사에 아직 Azure AD 테넌트가 없는 경우 등록 과정에서 무료 테넌트를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="b7e63-114">**Azure Active Directory에 로그인** 페이지에서 **새 테넌트 만들기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="b7e63-115">회사에 Azure AD 테넌트가 있는지 확실하지 않은가요?</span><span class="sxs-lookup"><span data-stu-id="b7e63-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="b7e63-116">회사에 Azure AD 테넌트가 있는지 확실하지 않은 경우 다음 단계에 따라 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="b7e63-117">Microsoft Azure 또는 Office 365의 활성 구독이 있는 회사는 이미 Azure AD 테넌트를 갖고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="b7e63-118">https://ms.portal.azure.com에서 Azure 관리 포털에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="b7e63-119">메뉴에서 Azure Active Directory를 선택한 다음 도메인 이름을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="b7e63-120">이미 테넌트가 있는 경우 도메인 이름이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="b7e63-121">기존 테넌트를 사용하세요?</span><span class="sxs-lookup"><span data-stu-id="b7e63-121">Using an existing tenant?</span></span>

<span data-ttu-id="b7e63-122">기존 Azure AD 테넌트를 사용하고 싶지만 로그인하는 데 문제가 있는 경우 아래 다이어그램에서 현재 상황과 가장 잘 맞는 시나리오를 찾아 권장 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![Azure AD 테넌트가 있나요 아니면 새로 만들어야 하나요?](images/onboardingAADFlow.png)

<span data-ttu-id="b7e63-124">Azure AD에서 도메인 추가에 대한 자세한 내용은 [Azure Active Directory에 사용자 지정 도메인 이름 추가](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b7e63-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="b7e63-125">Microsoft Azure에 대한 정보</span><span class="sxs-lookup"><span data-stu-id="b7e63-125">About Microsoft Azure</span></span>

<span data-ttu-id="b7e63-126">Microsoft Azure는 Microsoft에서 관리하는 전체 데이터 센터 네트워크에서 응용 프로그램을 빌드, 구축 및 관리하는 데 사용할 수 있는 공개 클라우드 플랫폼입니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="b7e63-127">회사에서는 Azure를 사용하여 실제 컴퓨터 대신 가상 기능 또는 서비스를 통해 가상 IT 인프라를 구축할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="b7e63-128">Azure 구독을 구입한다는 것은 근본적으로 Azure 공용 클라우드 내에 안전한 전용 공간을 임대한다는 의미입니다. 회사의 물리적 비즈니스를 수용하기 위해 사무용 건물의 한 층을 임대하는 것과 크게 다르지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="b7e63-129">사무용 건물의 소유자 입장에서 볼 때 회사는 임차인입니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="b7e63-130">어떤 회사에서 Azure, Microsoft Intune, Office 365 같은 Microsoft 클라우드 서비스를 구독하면 Azure 공용 클라우드에 그 회사만을 위해 격리된 전용 가상 공간이 생성되는데, 이것이 바로 Azure AD 테넌트입니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="b7e63-131">테넌트는 Azure AD 사용자 및 사용자에 대한 정보(암호, 프로필 데이터, 권한 등)를 호스팅합니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="b7e63-132">또한 테넌트에는 그룹, 응용 프로그램, 회사 및 보안에 관련된 기타 정보가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b7e63-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="b7e63-133">Azure AD에 대한 자세한 내용은 [Azure Active Directory 설명서](https://docs.microsoft.com/ azure/active-directory/)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b7e63-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 