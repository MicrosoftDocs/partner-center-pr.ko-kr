---
title: Partner Membership Center에서 파트너 센터로 이동 준비 | 파트너 센터
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 비즈니스를 PMC에서 파트너 센터로 이동하기 전에 유용한 정보와 FAQ를 검토하세요.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 06167a667152ddaf65702547783df93726f6cadc
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340108"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="f4c74-103">PMC(Partner Membership Center)에서 파트너 센터로 이동 준비</span><span class="sxs-lookup"><span data-stu-id="f4c74-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="f4c74-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="f4c74-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="f4c74-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="f4c74-105">Global admin</span></span>
-    <span data-ttu-id="f4c74-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="f4c74-106">User admin</span></span>
-    <span data-ttu-id="f4c74-107">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="f4c74-107">Sales agent</span></span>
-    <span data-ttu-id="f4c74-108">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="f4c74-108">Admin agent</span></span>

<span data-ttu-id="f4c74-109">멤버십 관리를 PMC(파트너 구성원 센터)에서 파트너 센터(Microsoft와의 비즈니스 관계를 관리하는 단일 대상)로 이전할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-109">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="f4c74-110">파트너가 쉽고 효율적으로 파트너 센터로 이전할 수 있도록 도와드리고자 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-110">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="f4c74-111">저희는 파트너 센터가 PMC와 다른 몇 가지 부분을 확인했으며, 파트너 센터로 이전하기 전에 이러한 부분을 이해하고 미리 대비한다면 도움이 될 것이라 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-111">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="f4c74-112">계정 및 ID 설정</span><span class="sxs-lookup"><span data-stu-id="f4c74-112">Account and identity setup</span></span>

<span data-ttu-id="f4c74-113">**Azure AD(Azure Active Directory) 회사 계정이란?** .</span><span class="sxs-lookup"><span data-stu-id="f4c74-113">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="f4c74-114">어떤 회사에서 Azure, Microsoft Intune, Office 365 등의 Microsoft 클라우드 서비스를 구독하면 Azure 퍼블릭 클라우드에 그 회사만을 위한 격리된 전용 가상 공간이 생성되는데, 이것이 바로 Azure 회사 계정입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-114">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="f4c74-115">회사 계정은 Azure AD 사용자 및 사용자에 대한 정보(이메일, 암호, 프로필 데이터, 권한 등)를 호스팅합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-115">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="f4c74-116">또한 회사 계정에는 그룹, 애플리케이션, 회사 및 보안에 관련된 기타 정보가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-116">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="f4c74-117">파트너 센터에서는 개인 이메일이 아닌 회사 이메일을 사용하여 계정에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-117">In Partner Center, you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="f4c74-118">회사 계정: john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="f4c74-118">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="f4c74-119">개인 계정: John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="f4c74-119">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="f4c74-120">회사 이메일은 Azure Active Sirectory 테넌트의 일부입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-120">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="f4c74-121">파트너 센터에서 계정을 보유하려면 AAD 테넌트가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-121">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="f4c74-122">Azure Active Directory에 대한 자세한 내용은 [Azure AD에서 디렉터리 만들기](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-122">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="f4c74-123">**PMC에서 파트너 센터로 이동할 때, Microsoft를 사용하는 AAD 테넌트가 있고(예: Office 365) CSP 비즈니스용 테넌트도 있는 경우 어떤 계정으로 파트너 센터에 로그인해야 할까요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-123">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="f4c74-124">CSP 계정 또는 MPN 회사 이메일 계정으로 파트너 센터에 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-124">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="f4c74-125">CSP 회사 이메일로 로그인하도록 선택하는 경우 대시보드의 왼쪽 탐색 창에 MPN 및 CSP 프로그램 정보가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-125">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="f4c74-126">MPN Azure AD 테넌트 회사 이메일로 로그인하는 경우에는 MPN 프로그램 정보만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-126">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="f4c74-127">MPN과 CSP의 사용자 역할이 서로 다르므로 MPN과 CSP 비즈니스에 동일한 계정을 사용하는 경우에는 그에 따라 사용자 역할을 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-127">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="f4c74-128">사용자 역할에 대한 자세한 내용은 [사용자 역할 및 권한 할당](permissions-overview.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-128">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="f4c74-129">**파트너 센터에 기존 Office 365 Azure AD 테넌트를 사용하지 않으려는 경우에는 PMC에서 마이그레이션하기 전에 새 테넌트를 만들면 됩니다.**</span><span class="sxs-lookup"><span data-stu-id="f4c74-129">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="f4c74-130">파트너 센터 계정 설정에 기존 Azure AD 테넌트를 사용하지 않으려는 여러 가지 이유가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-130">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="f4c74-131">파트너 센터로 마이그레이션하기 전에 [Azure Portal](https://ms.portal.azure.com/#home)로 이동하여 새 Azure AD 테넌트를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-131">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="f4c74-132">[Azure Active Directory에서 새 테넌트 만들기](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)의 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-132">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="f4c74-133">새 테넌트를 만든 후에는 PMC에서 파트너 센터로 이동할 때 이 AAD 테넌트를 사용하여 파트너 센터 계정을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-133">Once you have created the new tenant, use this AAD tenant to set up your Partner Center account when you move from PMC to Partner Center.</span></span> <span data-ttu-id="f4c74-134">테넌트를 만들려면 글로벌 관리자여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-134">You must be a global admin to create the tenant.</span></span> <span data-ttu-id="f4c74-135">이 새 디렉터리를 사용하여 파트너 센터로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-135">Use this new directory to migrate to Partner Center.</span></span>


<span data-ttu-id="f4c74-136">**AAD 글로벌 관리자 역할과 PMC MPN 글로벌 관리자 역할의 차이점은 무엇인가요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-136">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="f4c74-137">두 역할의 권한이 서로 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-137">These are two different roles with different permissions.</span></span> <span data-ttu-id="f4c74-138">파트너 센터의 AAD 테넌트 글로벌 관리자는 파트너 센터에서 사용자를 추가 또는 제거하고, 암호/역할/권한을 제공 및 관리하고, 회사의 모든 프로그램에 액세스하는 등 테넌트를 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-138">The AAD tenant global admin in Partner Center administers the tenant - adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company's programs in Partner Center.</span></span> 

<span data-ttu-id="f4c74-139">PMC의 MPN 글로벌 관리자 역할은 다음과 같은 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-139">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="f4c74-140">회사 및 회사의 모든 장소와 연결된 모든 데이터를 살펴보고 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-140">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="f4c74-141">글로벌 또는 로컬 수준에서 관리자를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-141">Add administrators at the global or local level.</span></span>  <span data-ttu-id="f4c74-142">또한 글로벌 관리자는 모든 위치에서 모든 사용자에게 글로벌 관리자 액세스 권한을 할당할 수 있으며, 이렇게 하면 사용자의 위치에 관계없이 글로벌 액세스 권한이 부여됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-142">Also, Global admins can assign any person at any location Global Administrator Access, which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="f4c74-143">다음을 비롯한 파트너용 UI 기능을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-143">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="f4c74-144">사용자 추가/제거</span><span class="sxs-lookup"><span data-stu-id="f4c74-144">Add/remove users</span></span>

 - <span data-ttu-id="f4c74-145">역할 할당/제거</span><span class="sxs-lookup"><span data-stu-id="f4c74-145">Assign/remove roles</span></span> 

 - <span data-ttu-id="f4c74-146">위치 추가/제거/업데이트</span><span class="sxs-lookup"><span data-stu-id="f4c74-146">Add/remove/update locations</span></span> 

 - <span data-ttu-id="f4c74-147">역량/맵 구매</span><span class="sxs-lookup"><span data-stu-id="f4c74-147">Purchase competency/maps</span></span> 

-  <span data-ttu-id="f4c74-148">혜택 보기</span><span class="sxs-lookup"><span data-stu-id="f4c74-148">View benefits</span></span>

<span data-ttu-id="f4c74-149">MPN 글로벌 관리자가 파트너 센터로 이동하면 MPN 파트너 관리자 역할이 되며, 이 역할은 파트너 센터 글로벌 관리자와는 권한 및 작업이 다릅니다. 파트너 센터의 역할 및 권한에 대한 자세한 내용은 [사용자 역할 및 권한 할당](permissions-overview.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-149">When the MPN global admin moves to Partner Center the role is called the MPN partner admin, which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="f4c74-150">**파트너 센터의 게스트 사용자 역할을 비롯한 사용자 역할**</span><span class="sxs-lookup"><span data-stu-id="f4c74-150">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="f4c74-151">파트너 센터에는 수행할 작업 유형에 따라 여러 가지 유형의 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-151">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="f4c74-152">Azure AD 역할인 글로벌 관리자와 같은 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-152">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="f4c74-153">클라우드 서비스 공급자 프로그램 또는 인센티브와 같은 프로그램에만 적용되는 역할도 있고, MPN에만 적용되는 역할도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-153">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="f4c74-154">모든 파트너 센터 역할을 확인하려면 [사용자 역할 및 권한 할당](permissions-overview.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-154">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="f4c74-155">**사용자가 PMC에서 파트너 센터로 이동하면 사용자의 역할은 어떻게 되나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-155">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="f4c74-156">마이그레이션을 수행하는 MPN 글로벌 관리자 또는 기본 프로그램 담당자를 제외하고, PMC의 모든 사용자는 관리자 역할을 잃게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-156">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="f4c74-157">마이그레이션을 완료하는 개인은 파트너 센터에서 역할을 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-157">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="f4c74-158">파트너 센터의 역할은 PMC의 역할과 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-158">The roles in Partner Center differ from the roles in PMC.</span></span> <span data-ttu-id="f4c74-159">파트너 센터의 사용자 역할에 대한 자세한 내용은 [사용자 역할 및 권한 할당](permissions-overview.md) 및 [PMC에서 파트너 센터로 이동](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-159">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="f4c74-160">**회사 프로필과 비즈니스 프로필 간의 차이점은 무엇인가요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-160">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="f4c74-161">회사 프로필은 주소, 위치, 기본 연락처, 은행 및 세금 세부 정보를 비롯한 회사 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-161">Your company profile is the information about your company that includes address, locations, primary contact, bank, and tax details.</span></span>

<span data-ttu-id="f4c74-162">비즈니스 프로필은 고객에게 회사를 소개하는 방법이자 회사의 로고, 핵심 비즈니스 및 전문 지식을 알리는 마케팅 페이지입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-162">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="f4c74-163">**계정을 통합하면 계정이 어떻게 되나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-163">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="f4c74-164">동일한 Azure AD 테넌트를 사용하여 여러 MPN 계정을 파트너 센터로 마이그레이션하면 시스템에서 이를 자동으로 인식하고 계정을 통합하라는 메시지를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-164">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="f4c74-165">여러 도메인이 동일한 Azure AD 테넌트에 연결된 경우에도 마찬가지입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-165">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="f4c74-166">별도의 AAD 테넌트를 사용하여 파트너 센터로 마이그레이션하도록 선택할 수도 있지만, 이렇게 하면 역량과 추가 구매 비용이 별도로 평가됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-166">You could still decide to migrate to Partner Center using separate AAD tenants, but note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="f4c74-167">**AAD 테넌트가 여러 개 있고 MPN 계정이 하나 있는 경우 파트너 센터에서 연결할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-167">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="f4c74-168">예, 파트너 센터에서 여러 Azure AD 테넌트를 단일 파트너 센터 계정에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-168">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="f4c74-169">여기서 자세한 내용을 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-169">Learn more here.</span></span> 

<span data-ttu-id="f4c74-170">**단일 파트너 센터 계정에 여러 Azure AD 테넌트를 추가할 때 제한 사항이 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-170">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="f4c74-171">Azure AD 테넌트가 이미 기존 파트너 센터 계정에 연결되어 있는 경우에는 다중 테넌트 기능을 사용하여 새 파트너 센터 계정에 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-171">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="f4c74-172">생각해 볼 또 다른 사항으로, Azure AD 테넌트는 하나의 파트너 센터 계정에만 연결할 수 있지만, 파트너 센터 계정은 여러 테넌트를 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-172">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="f4c74-173">MPN(Microsoft 파트너 네트워크) 구성원 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="f4c74-173">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="f4c74-174">**PMC에서 파트너 센터로 이동할 수 있는 사람은 누구인가요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-174">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="f4c74-175">회사의 MPN 글로벌 관리자 또는 기본 프로그램 담당자(이 두 역할을 같은 사람이 수행하는 경우가 많음)는 이동을 시작하고 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-175">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="f4c74-176">**마이그레이션을 완료하는 사람이 파트너 센터에서 회사 법적 프로필의 기본 담당자가 되나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-176">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="f4c74-177">꼭 그런 것은 아니지만, 기본 담당자는 서명 권한이 있는 사람이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-177">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="f4c74-178">**Microsoft에서 내 MPN 멤버 자격을 대신 마이그레이션할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-178">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="f4c74-179">아니요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-179">No.</span></span> <span data-ttu-id="f4c74-180">Microsoft는 구성원 계정을 파트너 센터로 이동하는 데 도움을 줄 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-180">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="f4c74-181">파트너는 마이그레이션 프로세스를 시작하려면 회사 계정(로그인 자격 증명)으로 PMC에 로그인하여 계정을 이동해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-181">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="f4c74-182">계정 이동 단계를 완료한 후에는 멤버 자격 관리를 시작하고 사용자 역할 및 권한을 할당할 수 있습니다. 그러면 사용자가 혜택에 액세스하여 멤버 자격을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-182">After you've completed the steps to move your account, you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="f4c74-183">Microsoft는 현재 역량, 혜택, 위치 정보, 인센티브 지급을 위한 은행/세금 정보, 파트너 대학 액세스를 포함한 MCP 연결을 자동으로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-183">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="f4c74-184">Microsoft는 현재 역량, 혜택, 위치 정보, 인센티브 지급을 위한 은행/세금 정보, 파트너 대학 액세스를 포함한 MCP 연결을 자동으로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-184">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="f4c74-185">**갱신 정책은 어떻게 달라지나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-185">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="f4c74-186">파트너 센터의 갱신 기간은 계정 연주기일부터 30일입니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-186">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="f4c74-187">**파트너 센터로 이동한 후에도 역량이 그대로 유지되나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-187">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="f4c74-188">예, 파트너 센터로 이동해도 역량에는 아무 영향이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-188">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="f4c74-189">다른 점이 발견되면 [고객 지원팀](https://partner.microsoft.com/support)에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-189">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="f4c74-190">**이동 후 혜택(클라우드 혜택, 기술 지원, 소프트웨어 혜택, Visual Studio 포함)이 달라지나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-190">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="f4c74-191">적격 혜택은 변경되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-191">Your eligible benefits will not change.</span></span> <span data-ttu-id="f4c74-192">다른 점이 발견되면 [고객 지원팀](https://partner.microsoft.com/support)에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-192">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="f4c74-193">**Visual Studio 혜택이 할당된 Microsoft 계정을 그대로 사용할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-193">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="f4c74-194">예.</span><span class="sxs-lookup"><span data-stu-id="f4c74-194">Yes.</span></span> <span data-ttu-id="f4c74-195">MSA에 할당된 Visual Studio 혜택이 적용되고 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-195">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="f4c74-196">또한 갱신 후 파트너 센터에 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-196">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="f4c74-197">그러나 파트너 센터에서 마이그레이션된 MSA 할당을 제거하면 파트너 센터에 다시 추가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-197">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="f4c74-198">파트너 센터에서 파트너는 동일한 테넌트(여기서 파트너는 Azure AD 테넌트의 MPN 관리자임)의 MSA인 회사 계정 및 게스트 사용자 계정을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-198">In Partner Center, a partner can add work accounts and guest user accounts, which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="f4c74-199">파트너가 여러 Azure AD 테넌트에서 전역 관리자이고 이러한 모든 테넌트가 동일한 파트너 센터 계정과 연결된 경우 파트너는 이러한 모든 테넌트의 사용자를 Visual Studio 혜택 및 Azure 사용량 기반 할당에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-199">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="f4c74-200">MPN 관리자 또는 전역 관리가 Visual Studio의 사용량 기반 구독을 게스트 사용자에게 할당할 수 있지만 게스트 사용자는 해당 MSA를 사용하여 파트너 센터에 로그인할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-200">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="f4c74-201">그러나 게스트 사용자는 Azure 및 Visual Studio에 로그인하여 할당된 혜택을 확인하고 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-201">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="f4c74-202">**MCP 연결 및 파트너 대학 액세스를 어떻게 관리해야 하나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-202">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="f4c74-203">PMC에서 이동하는 MCP 연결은 아무 것도 달라지지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-203">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="f4c74-204">그러나 파트너 센터로 이동한 이후의 신규 직원은 파트너 센터에서 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-204">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="f4c74-205">기존 사용자의 모든 파트너 대학 권한은 그대로 유지되지만, 신규 직원은 [교육 센터](https://partner.microsoft.com/training)로 이동하여 파트너 대학 액세스 권한을 얻는 방법을 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-205">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="f4c74-206">**파트너 센터로 이동한 후 MCP 정보를 보려면 어떻게 해야 하나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-206">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="f4c74-207">대시보드의 왼쪽 탐색 영역에서 **역량**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-207">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="f4c74-208">**역량** 페이지에서 기술 보고서를 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-208">From the **Competencies** page, you are able to download the skills report.</span></span> <span data-ttu-id="f4c74-209">기술 보고서에는 파트너 센터의 역량 및 프로그램과 관련된 기술을 획득한 사용자가 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-209">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="f4c74-210">사용자가 기술을 획득했지만 해당 기술이 현재 진행 중인 역량과 관련이 없는 경우에는 보고서에 나열되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-210">If your users have gained skills but those skills are not relevant to the competencies you're working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="f4c74-211">**파트너 센터에서 고객 참조가 사용되나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-211">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="f4c74-212">아니요, 파트너 센터에서 역량 요구 사항을 충족하기 위해 고객 참조를 사용할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-212">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="f4c74-213">**POR(Partner of Record) 협회도 파트너 센터로 이동하나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-213">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="f4c74-214">예, POR(Partner of Record)과 관련된 변경 사항은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-214">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="f4c74-215">[파트너 ID를 고객과 연결](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-215">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="f4c74-216">**파트너 센터로 이동하면 인센티브에 영향이 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-216">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="f4c74-217">아니요, 위치를 통합하지 않고 계정을 이동한 경우에는 인센티브에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-217">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="f4c74-218">회사가 PMC에서 계정을 여러 개 가지고 있는데 파트너 센터로 이동할 때 글로벌 계정 하나에 통합하기로 결정하는 경우에는 인센티브 손실이 발생하지 않지만 인센티브 지급이 지연될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-218">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="f4c74-219">인센티브 프로그램과 관련된 PMC 계정 중 일부를 이동하지 않으면 해당 계정과 연결된 인센티브를 더 이상 받을 수 없게 될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-219">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="f4c74-220">**파트너 센터의 인센티브 사용자 역할은 무엇인가요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-220">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="f4c74-221">파트너 센터의 인센티브 역할은 위치 기반이며 인센티브 관리자 및 인센티브 사용자를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-221">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="f4c74-222">인센티브 역할이 수행할 수 있는 작업에 대한 자세한 내용은 [사용자 역할 및 권한 할당](permissions-overview.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f4c74-222">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="f4c74-223">**글로벌 및 위치 수준에서 인센티브 사용자를 할당할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-223">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="f4c74-224">예.</span><span class="sxs-lookup"><span data-stu-id="f4c74-224">Yes.</span></span> <span data-ttu-id="f4c74-225">모든 위치의 인센티브 관리자가 될 인센티브 관리자를 할당할 수도 있고, 위치마다 별도의 인센티브 관리자를 둘 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-225">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="f4c74-226">**인센티브를 글로벌 또는 위치 수준에서 지급할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-226">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="f4c74-227">인센티브는 위치 수준에서만 지급됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-227">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="f4c74-228">**추천과 관련하여 비즈니스 프로필을 몇 개나 만들 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-228">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="f4c74-229">기업은 기업의 관심사를 완벽하게 표현하는 데 필요한 만큼 비즈니스 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-229">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="f4c74-230">각 비즈니스 프로필에 국가당 하나씩 최대 5개 위치를 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-230">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="f4c74-231">각 비즈니스 프로필은 각 위치에 대한 추천을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-231">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="f4c74-232">**추천은 어떻게 할당되며, 어떻게 달라지나요? 예를 들어 한 지역/국가에 글로벌 회사가 있고 다른 지역/국가에 여러 위치가 있는 경우에는 어떻게 추천이 할당되나요?**</span><span class="sxs-lookup"><span data-stu-id="f4c74-232">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="f4c74-233">추천은 고객이 정의하는 검색 매개 변수를 기반으로 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-233">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="f4c74-234">따라서 파트너의 위치 수와 상관 없이, 고객이 원하는 위치를 지정하고 다른 매개 변수를 충족하는 파트너의 회사가 그 위치에 있다면 해당 위치로 추천이 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="f4c74-234">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








