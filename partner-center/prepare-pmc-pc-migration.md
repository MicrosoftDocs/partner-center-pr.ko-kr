---
title: 파트너 구성원 센터에서 파트너 센터로의 이동 준비 | 파트너 센터
ms.topic: article
ms.date: 06/13/2019
description: 비즈니스를 PMC에서 파트너 센터로 전환 하기 전에 고려해 야 할 사항
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 411093a885abf2144df218d8ef28a07a10f09061
ms.sourcegitcommit: dd961f85bc790e56c70479a5926177454dd8e855
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/12/2019
ms.locfileid: "67854527"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="befbb-103">파트너 구성원 센터 (PMC)에서 파트너 센터로의 이동 준비</span><span class="sxs-lookup"><span data-stu-id="befbb-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="befbb-104">PMC (파트너 구성원 센터)에서 파트너 센터 (Microsoft와의 비즈니스 관계를 관리 하는 단일 대상)로 회원 관리를 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-104">We are moving membership management from Partner Membership Center (PMC) to the partner center – the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="befbb-105">파트너 센터로 이동 하는 것이 효율적이 고 쉽게 가능 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-105">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="befbb-106">파트너 센터가 PMC와 다른 몇 가지 영역을 확인 하 고, 이동 하기 전에이를 이해 하 고 준비 하려고 한다고 생각 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-106">We’ve identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="befbb-107">계정 및 id 설정</span><span class="sxs-lookup"><span data-stu-id="befbb-107">Account and identity setup</span></span>

<span data-ttu-id="befbb-108">**Azure Active Directory (Azure AD) 회사 계정 이란?**</span><span class="sxs-lookup"><span data-stu-id="befbb-108">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="befbb-109">어떤 회사에서 Azure, Microsoft Intune, Office 365 같은 Microsoft 클라우드 서비스를 구독하면 Azure 공용 클라우드에 그 회사만을 위해 격리된 전용 가상 공간이 생성되는데, 이것이 바로 Azure 회사 계정입니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-109">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="befbb-110">회사 계정은 Azure AD 사용자와 해당 사용자에 대 한 정보 (전자 메일, 암호, 프로필 데이터, 권한 등)를 호스트 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-110">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="befbb-111">회사 계정에는 회사 및 보안과 관련 된 그룹, 응용 프로그램 및 기타 정보도 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-111">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> <span data-ttu-id="befbb-112">자세한 내용은 다음을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-112">For more information see …</span></span>

<span data-ttu-id="befbb-113">파트너 센터에서 회사 전자 메일을 사용 하 여 개인 이메일이 아닌 계정에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-113">In the Partner Center you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="befbb-114">회사 계정:john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="befbb-114">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="befbb-115">개인 계정:John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="befbb-115">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="befbb-116">회사 전자 메일은 Azure active directory 테 넌 트의 일부입니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-116">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="befbb-117">파트너 센터에 계정을 포함 하려면 AAD 테 넌 트가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-117">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="befbb-118">Azure Active Directory에 대 한 자세한 내용은 [AZURE AD에서 디렉터리 만들기](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-118">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="befbb-119">**PMC에서 파트너 센터로 이동 하는 경우 Microsoft에 AAD 테 넌 트 (예: Office 365 용)가 있고 CSP 비즈니스에 대 한 테 넌 트가 있는 경우 파트너 센터에 로그인 해야 하는 계정은 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-119">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="befbb-120">CSP 계정 또는 MPN work 전자 메일 계정을 사용 하 여 파트너 센터에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-120">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="befbb-121">CSP 회사 전자 메일을 사용 하 여 로그인 하도록 선택 하는 경우 대시보드의 왼쪽 탐색은 MPN 및 CSP 프로그램 정보를 모두 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-121">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="befbb-122">MPN Azure AD 테 넌 트 회사 전자 메일을 사용 하 여 로그인 하는 경우에는 MPN 프로그램 정보만 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-122">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="befbb-123">MPN와 CSP의 사용자 역할은 서로 다르므로, MPN 및 CSP 비즈니스 모두에 동일한 계정을 사용 하는 경우에는 그에 따라 사용자 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-123">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="befbb-124">사용자 역할에 대 한 자세한 내용은 [사용자 역할 및 사용 권한 할당](permissions-overview.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-124">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="befbb-125">**AAD 전역 관리자 역할과 PMC MPN 전역 관리자 역할의 차이점은 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-125">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="befbb-126">이러한 역할은 사용 권한이 서로 다른 두 개의 완전히 다른 역할입니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-126">These are two completely different roles with different permissions.</span></span> <span data-ttu-id="befbb-127">파트너 센터의 AAD 테 넌 트 전역 관리자는 테 넌 트를 관리 합니다.-사용자를 추가 또는 제거 하 고, 암호, 역할 및 권한을 제공 하 고 관리 하며, 파트너 센터의 모든 회사 프로그램에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-127">The AAD tenant global admin in Partner Center administers the tenant – adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company’s programs in Partner Center.</span></span> 

<span data-ttu-id="befbb-128">PMC의 MPN 전역 관리자 역할은 다음과 같은 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-128">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="befbb-129">회사 및 모든 회사의 위치와 연결 된 모든 데이터 보기 및 편집</span><span class="sxs-lookup"><span data-stu-id="befbb-129">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="befbb-130">전역 또는 로컬 수준에서 관리자를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-130">Add administrators at the global or local level.</span></span>  <span data-ttu-id="befbb-131">또한 전역 관리자는 모든 위치에 전역 관리자 액세스 권한을 할당 하 여 해당 사용자가 연결 된 위치에 관계 없이 전역 액세스 권한을 부여할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-131">Also, Global admins can assign any person at any location Global Administrator Access which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="befbb-132">다음을 포함 하 여 파트너 지향 UI 함수를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-132">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="befbb-133">사용자 추가/제거</span><span class="sxs-lookup"><span data-stu-id="befbb-133">Add/remove users</span></span>

 - <span data-ttu-id="befbb-134">역할 할당/제거</span><span class="sxs-lookup"><span data-stu-id="befbb-134">Assign/remove roles</span></span> 

 - <span data-ttu-id="befbb-135">위치 추가/제거/업데이트</span><span class="sxs-lookup"><span data-stu-id="befbb-135">Add/remove/update locations</span></span> 

 - <span data-ttu-id="befbb-136">역량/지도 구매</span><span class="sxs-lookup"><span data-stu-id="befbb-136">Purchase competency/maps</span></span> 

-  <span data-ttu-id="befbb-137">혜택 보기</span><span class="sxs-lookup"><span data-stu-id="befbb-137">View benefits</span></span>

<span data-ttu-id="befbb-138">MPN 전역 관리자가 파트너 센터로 이동 하면 역할은 파트너 센터 전역 관리자와 다른 권한 및 작업을 포함 하는 MPN Partner admin 이라고 합니다. 파트너 센터의 역할 및 권한에 대 한 자세한 내용은 [사용자 할당 역할 및 사용 권한](permissions-overview.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-138">When the MPN global admin moves to Partner Center the role is called the MPN partner admin which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="befbb-139">**파트너 센터에서 게스트 사용자 역할을 포함 하는 사용자 역할**</span><span class="sxs-lookup"><span data-stu-id="befbb-139">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="befbb-140">파트너 센터에는 수행 해야 하는 작업 유형에 따라 다양 한 유형의 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-140">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="befbb-141">Azure AD 역할에 해당 하는 전역 관리자와 같은 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-141">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="befbb-142">일부 역할은 클라우드 서비스 공급자 프로그램 또는 성과급과 같은 프로그램에만 적용 되며, MPN에만 적용 되는 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-142">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="befbb-143">모든 파트너 센터 역할을 확인 하려면 [사용자 할당 역할 및 사용 권한](permissions-overview.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-143">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="befbb-144">**PMC에서 파트너 센터로 이동 하는 경우 사용자의 역할은 어떻게 되나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-144">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="befbb-145">마이그레이션을 수행 하는 MPN 전역 관리자 또는 기본 프로그램 담당자를 제외 하 고, PMC의 모든 사용자는 자신의 관리자 역할을 잃게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-145">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="befbb-146">마이그레이션을 완료 하는 개인은 파트너 센터에서 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-146">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="befbb-147">파트너 센터의 역할은 PMC의 역할과 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-147">The roles in Partner Center differ from those in PMC.</span></span> <span data-ttu-id="befbb-148">파트너 센터의 사용자 역할에 대 한 자세한 내용은 [사용자 할당 역할 및 사용 권한 할당] (사용 권한-overview.md 및 [PMC에서 파트너 센터로 이동)을](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-148">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="befbb-149">**회사 프로필과 내 비즈니스 프로필 간의 차이점은 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-149">**What’s the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="befbb-150">회사 프로필은 주소, 위치, 기본 연락처, 은행 및 세금 세부 정보를 포함 하는 회사에 대 한 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-150">Your company profile is the information about your company that includes address, locations, primary contact, bank and tax details.</span></span>

<span data-ttu-id="befbb-151">비즈니스 프로필은 고객에 게 자신을 게 제공 하는 방법 이며 로고, 비즈니스 초점에 대 한 세부 정보, 전문 지식 등에 대 한 세부 정보를 표시 하는 마케팅 페이지입니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-151">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="befbb-152">**계정 통합은 계정에 대 한 의미는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-152">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="befbb-153">동일한 Azure AD 테 넌 트를 사용 하 여 여러 MPN 계정을 파트너 센터로 마이그레이션하는 경우 시스템에서 자동으로 인식 하 고 계정을 통합 하도록 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-153">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="befbb-154">동일한 Azure AD 테 넌 트에 여러 도메인이 연결 되어 있는 경우에도 마찬가지입니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-154">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="befbb-155">별도의 AAD 테 넌 트를 사용 하 여 파트너 센터로 마이그레이션하도록 결정할 수는 있지만이로 인해 역량 및 추가 구매 비용이 격리 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-155">You could still decide to migrate to Partner Center using separate AAD tenants, but please note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="befbb-156">**여러 AAD 테 넌 트와 단일 MPN 계정이 있는 경우 파트너 센터에서 연결할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-156">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="befbb-157">예, 파트너 센터에서 여러 Azure AD 테 넌 트를 단일 파트너 센터 계정에 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-157">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="befbb-158">자세한 내용은 여기를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-158">Learn more here.</span></span> 

<span data-ttu-id="befbb-159">**단일 파트너 센터 계정에 여러 Azure AD 테 넌 트를 추가 하는 데 제한이 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-159">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="befbb-160">Azure AD 테 넌 트가 기존 파트너 센터 계정에 이미 연결 되어 있는 경우에는 다중 테 넌 트 기능을 사용 하 여 새 파트너 센터 계정에 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-160">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="befbb-161">Azure AD 테 넌 트는 하나의 파트너 센터 계정에만 연결할 수 있지만 파트너 센터 계정에는 연결 된 여러 테 넌 트가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-161">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="befbb-162">Microsoft 파트너 네트워크 (MPN) 멤버 자격 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="befbb-162">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="befbb-163">**PMC에서 파트너 센터로의 이동을 수행할 수 있는 사람은 누구 인가요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-163">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="befbb-164">회사 MPN 전역 관리자 또는 기본 프로그램 담당자 (이러한 두 역할은 종종 동일한 사람이 보유 하 고 있음)는 이동을 시작 하 고 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-164">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="befbb-165">**마이그레이션을 완료 하는 사람이 파트너 센터의 회사 법적 프로필에 대 한 기본 담당자가 됩니까?**</span><span class="sxs-lookup"><span data-stu-id="befbb-165">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="befbb-166">그러나 기본 연락처는 계약에 서명 하는 데 필요한 권한이 있는 사용자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-166">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="befbb-167">**Microsoft에서 내 MPN 멤버 자격을 마이그레이션할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-167">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="befbb-168">아니요.</span><span class="sxs-lookup"><span data-stu-id="befbb-168">No.</span></span> <span data-ttu-id="befbb-169">Microsoft는 구성원 계정을 파트너 센터로 이동 하는 데 도움을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-169">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="befbb-170">마이그레이션 프로세스를 시작 하려면 회사 계정 (로그인 자격 증명)으로 PMC에 로그인 하 여 계정을 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-170">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="befbb-171">계정을 이동 하는 단계를 완료 한 후 멤버 자격 관리를 시작 하 고, 혜택에 액세스 하 여 멤버 자격을 관리 하는 데 도움이 되도록 팀에 사용자 역할 및 권한을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-171">After you’ve completed the steps to move your account you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="befbb-172">Microsoft는 현재 역량, 혜택, 위치 정보, 성과급을 위한 은행/세금 정보 및 파트너 대학 액세스를 포함 한 MCP 연결을 자동으로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-172">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="befbb-173">Microsoft는 현재 역량, 혜택, 위치 정보, 성과급을 위한 은행/세금 정보 및 파트너 대학 액세스를 포함 한 MCP 연결을 자동으로 마이그레이션합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-173">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="befbb-174">**갱신 정책은 어떻게 변경 되나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-174">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="befbb-175">파트너 센터에서 갱신 기간은 30 일 이내에 시작 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-175">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="befbb-176">**파트너 센터로 전환 하 고 나면 역량은 그대로 유지 되나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-176">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="befbb-177">예, 파트너 센터로의 이동이 compentencies에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-177">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="befbb-178">차이점이 있는 경우 [지원](https://partner.microsoft.com/support)담당자에 게 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-178">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="befbb-179">**이동 후 혜택 (클라우드 혜택, 기술 지원, 소프트웨어 이점, Visual Studio 포함)이 변경 되나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-179">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="befbb-180">적격 혜택은 변경 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-180">Your eligible benefits will not change.</span></span> <span data-ttu-id="befbb-181">차이점이 있는 경우 [지원](https://partner.microsoft.com/support)담당자에 게 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-181">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="befbb-182">**Visual Studio 혜택 할당을 보유 하 고 있는 Microsoft 계정을 사용할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-182">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="befbb-183">예</span><span class="sxs-lookup"><span data-stu-id="befbb-183">Yes.</span></span> <span data-ttu-id="befbb-184">MSAs 할당 된 Visual Studio 혜택은 적용 되 고 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-184">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="befbb-185">파트너 센터에서 갱신 한 후에도 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-185">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="befbb-186">그러나 파트너 센터에서 마이그레이션된 MSA 할당을 제거 하는 경우 파트너 센터에 다시 추가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-186">However, if you remove an MSA allocation once migrated in Partner Center, it can’t be added  back into Partner Center.</span></span>

<span data-ttu-id="befbb-187">파트너 센터에서 파트너는 Azure AD 테 넌 트에서 파트너가 MPN 하는 동일한 테 넌 트의 MSA 인 작업 계정 및 게스트 사용자 계정을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-187">In Partner Center, a partner can add work accounts and guest user accounts which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="befbb-188">파트너가 여러 Azure AD 테 넌 트의 전역 관리자이 고 이러한 모든 테 넌 트가 동일한 파트너 센터 계정에 연결 된 경우 파트너는 이러한 모든 테 넌 트의 사용자를 Visual Studio 혜택 및 Azure 사용 기반 할당에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-188">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="befbb-189">게스트 사용자는 MPN 관리자 또는 전역 관리자가 Visual Studio의 사용량 기반 구독을 할당할 수 있지만, 게스트 사용자는 MSA를 사용 하 여 파트너 센터에 로그인 할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-189">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="befbb-190">그러나 게스트 사용자는 Azure 및 Visual Studio에 로그인 하 여 할당 된 혜택의 유효성을 검사 하 고 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-190">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="befbb-191">**MCP 연결 및 파트너 대학 액세스를 어떻게 관리 해야 하나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-191">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="befbb-192">PMC에서 이동 하는 MCP 연결에 대 한 변경 내용이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-192">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="befbb-193">그러나 파트너 센터로 이동한 후 새로운 새 직원은 파트너 센터에 연결 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-193">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="befbb-194">기존 사용자에 대 한 모든 파트너 대학 권한은 유지 되지만 새 직원은 파트너 대학에 액세스 하는 방법에 대 한 정보를 [학습 센터로](https://partner.microsoft.com/training) 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-194">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="befbb-195">**파트너 센터로 이동 하면 어떻게 할까요? MCP 정보가 표시 되나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-195">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="befbb-196">대시보드의 왼쪽 탐색 모음에서 역량 **을 선택 합니다** .</span><span class="sxs-lookup"><span data-stu-id="befbb-196">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="befbb-197">역량 페이지 **에서** 기술 보고서를 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-197">From the **Competencies** page you are able to download the skills report.</span></span> <span data-ttu-id="befbb-198">기술 보고서에는 파트너 센터의 역량 및 프로그램과 관련 된 기술을 획득 한 사용자가 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-198">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="befbb-199">사용자에 게 기술이 있지만 이러한 기술이 작업 중인 역량에 해당 하지 않는 경우 보고서에 나열 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-199">If your users have gained skills but those skills are not relevant to the competencies which you are working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="befbb-200">**파트너 센터에서 고객 참조를 사용 하나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-200">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="befbb-201">아니요. 파트너 센터에서 역량 요구 사항을 충족 하기 위해 고객 참조가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-201">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="befbb-202">**레코드 연결 파트너는 파트너 센터로 이동 하나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-202">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="befbb-203">예, 레코드의 파트너에 대 한 변경 내용이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-203">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="befbb-204">[파트너 ID를 고객에 게 연결](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)하는 방법에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-204">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="befbb-205">**파트너 센터로 이동 하 여 성과급에 영향이 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-205">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="befbb-206">아니요, 위치를 통합 하지 않고 계정을 이동한 경우에는 성과급에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-206">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="befbb-207">비즈니스에 PMC에 여러 계정이 있고 파트너 센터로 이동 하는 경우에는 전체 계정으로 통합 하기로 결정 하는 경우에는 성과급 손실이 발생 하지 않지만 동기 지급에 지연이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-207">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="befbb-208">성과급 프로그램에 포함 된 모든 PMC 계정을 이동 하지 않는 경우 해당 계정에 연결 된 성과급 획득을 중지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-208">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="befbb-209">**파트너 센터에서 동기 사용자 역할은 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-209">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="befbb-210">파트너 센터의 동기 역할은 위치를 기반으로 하며, 성과급 관리자 및 성과급 사용자를 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-210">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="befbb-211">이러한 역할이 수행할 수 있는 작업에 대 한 자세한 내용은 [사용자 역할 및 사용 권한 할당](permissions-overview.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="befbb-211">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="befbb-212">**사용자가 전역 및 위치 수준에서 할당 될 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-212">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="befbb-213">예</span><span class="sxs-lookup"><span data-stu-id="befbb-213">Yes.</span></span> <span data-ttu-id="befbb-214">모든 위치에 대 한 성과급 관리자가 되도록 성과급 관리자를 할당 하거나 각 위치에 고유한 성과급 관리자를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-214">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="befbb-215">**전역 또는 위치 수준에서 성과급을 지불할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-215">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="befbb-216">성과급은 위치 수준 에서만 지불 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-216">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="befbb-217">**조회와 관련 하 여 얼마나 많은 비즈니스 프로필을 만들 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-217">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="befbb-218">회사는 회사의 관심사를 완전히 나타내는 데 필요한 만큼의 비즈니스 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-218">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="befbb-219">각 비즈니스 프로필에서 국가 당 한 곳에서 최대 5 개의 위치를 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-219">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="befbb-220">각 비즈니스 프로필은 각 위치에 대 한 조회를 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-220">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="befbb-221">**조회를 할당 하는 방법, 무엇이 변경 될 수 있나요? 예를 들어 한 시장에 글로벌 회사가 있고 다른 시장에 위치 하는 경우에는 어떻게 조회가 할당 되나요?**</span><span class="sxs-lookup"><span data-stu-id="befbb-221">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="befbb-222">조회는 고객이 정의 하는 검색 매개 변수를 기반으로 할당 됩니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-222">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="befbb-223">따라서 하나 이상의 위치가 있는지 여부와 상관 없이 고객이 원하는 위치를 지정 하 고 다른 매개 변수를 충족 하는 비즈니스를 보유 하 고 있다면 조회는 해당 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="befbb-223">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








