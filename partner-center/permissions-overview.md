---
title: 사용자에게 역할 및 사용 권한 할당
ms.topic: article
ms.date: 09/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 상업 거래, 조회, 인센티브 또는 MPN 멤버십을 관리하는 회사 사용자에게 가장 적합한 역할에 대해 알아보세요.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 32df86887ccbea5d18d1bd8c7c34add2b1ab60e4
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006804"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="4ccd1-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="4ccd1-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="4ccd1-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4ccd1-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-105">Global admin</span></span>
- <span data-ttu-id="4ccd1-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-106">User admin</span></span>
- <span data-ttu-id="4ccd1-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-107">MPN partner admin</span></span>

<span data-ttu-id="4ccd1-108">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="4ccd1-109">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="4ccd1-110">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="4ccd1-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="4ccd1-111">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="4ccd1-112">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="4ccd1-113">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 전역 관리자 같은 표준 Azure Active Directory 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="4ccd1-114">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="4ccd1-115">Azure Active Directory 테넌트 역할에는 전역 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="4ccd1-116">비 Azure-Active-Directory 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="4ccd1-117">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="4ccd1-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="4ccd1-118">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-118">**Role**</span></span>|<span data-ttu-id="4ccd1-119">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-119">**What they can do**</span></span>|<span data-ttu-id="4ccd1-120">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="4ccd1-121">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-121">Global admin</span></span>|<span data-ttu-id="4ccd1-122">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="4ccd1-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="4ccd1-123">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="4ccd1-124">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-125">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="4ccd1-126">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="4ccd1-127">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="4ccd1-128">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="4ccd1-129">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-129">User management admin</span></span>   | <span data-ttu-id="4ccd1-130">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="4ccd1-131">파트너 센터에서 Microsoft 파트너 네트워크 멤버십 혜택 및 제품 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="4ccd1-132">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="4ccd1-133">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-134">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="4ccd1-135">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-135">Billing admin</span></span> | <span data-ttu-id="4ccd1-136">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="4ccd1-137">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="4ccd1-138">\*    가격 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-138">\*    View pricing</span></span>
||<span data-ttu-id="4ccd1-139">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-140">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="4ccd1-141">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-141">Default user</span></span>|  <span data-ttu-id="4ccd1-142">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-142">View My profile</span></span>   |[<span data-ttu-id="4ccd1-143">암호 재설정</span><span class="sxs-lookup"><span data-stu-id="4ccd1-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="4ccd1-144">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="4ccd1-144">Admin agent</span></span> | <span data-ttu-id="4ccd1-145">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-145">\*    Customer management</span></span>|[<span data-ttu-id="4ccd1-146">고객과의 관계 구축</span><span class="sxs-lookup"><span data-stu-id="4ccd1-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="4ccd1-147">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="4ccd1-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="4ccd1-148">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="4ccd1-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="4ccd1-149">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-149">\*    Subscription management</span></span>
||<span data-ttu-id="4ccd1-150">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="4ccd1-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="4ccd1-151">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="4ccd1-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="4ccd1-152">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="4ccd1-153">\*    청구</span><span class="sxs-lookup"><span data-stu-id="4ccd1-153">\*    Billing</span></span>
||<span data-ttu-id="4ccd1-154">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="4ccd1-155">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="4ccd1-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="4ccd1-156">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-157">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="4ccd1-158">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="4ccd1-158">Sales agent</span></span> | <span data-ttu-id="4ccd1-159">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-159">\*    Customer management</span></span>|[<span data-ttu-id="4ccd1-160">고객에 대한 청구 지원 제공 및 청구 질문에 대한 답변 지원</span><span class="sxs-lookup"><span data-stu-id="4ccd1-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="4ccd1-161">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="4ccd1-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="4ccd1-162">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-162">\*    Subscription management</span></span>
||<span data-ttu-id="4ccd1-163">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-163">\*    View support tickets</span></span>
||<span data-ttu-id="4ccd1-164">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="4ccd1-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="4ccd1-165">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="4ccd1-166">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="4ccd1-167">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="4ccd1-168">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="4ccd1-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="4ccd1-169">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-170">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="4ccd1-171">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="4ccd1-171">Helpdesk agent</span></span>| <span data-ttu-id="4ccd1-172">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="4ccd1-173">Microsoft로 문제를 에스컬레이션하고 Microsoft 에스컬레이션에 더 적합한 문제 알아보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="4ccd1-174">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="4ccd1-174">\*    Edit customer details</span></span>
||<span data-ttu-id="4ccd1-175">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="4ccd1-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="4ccd1-176">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="4ccd1-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="4ccd1-177">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="4ccd1-178">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-179">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="4ccd1-180">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="4ccd1-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="4ccd1-181">(CSP 역할 및 비 Azure AD 역할)</span><span class="sxs-lookup"><span data-stu-id="4ccd1-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="4ccd1-182">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="4ccd1-183">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-183">**Role**</span></span>   |<span data-ttu-id="4ccd1-184">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-184">**What you can do**</span></span>|<span data-ttu-id="4ccd1-185">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="4ccd1-186">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-186">Global admin</span></span>| <span data-ttu-id="4ccd1-187">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="4ccd1-188">CSP 파트너 시스템을 파트너 센터 API와 통합하는 데 도움이 되도록 제어판 공급업체로 등록</span><span class="sxs-lookup"><span data-stu-id="4ccd1-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="4ccd1-189">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="4ccd1-190">게스트 사용자(Azure Active Directory 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="4ccd1-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="4ccd1-191">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-191">**Guest user**</span></span>   | <span data-ttu-id="4ccd1-192">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="4ccd1-193">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-193">MPN partner admin</span></span>|
||<span data-ttu-id="4ccd1-194">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-194">Accounts admin</span></span>|
||<span data-ttu-id="4ccd1-195">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-195">Incentives admin</span></span>|
||<span data-ttu-id="4ccd1-196">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-196">Business profile admin</span></span>|
||<span data-ttu-id="4ccd1-197">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-197">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="4ccd1-198">MPN 멤버십 및 회사 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-198">Manage MPN membership and your company</span></span> 

<span data-ttu-id="4ccd1-199">이러한 역할은 Azure Active Directory 역할이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-199">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="4ccd1-200">이러한 역할은 테넌트가 아니라 회사 비즈니스를 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="4ccd1-200">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="4ccd1-201">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-201">**Role**</span></span> | <span data-ttu-id="4ccd1-202">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-202">**What you can do**</span></span>|<span data-ttu-id="4ccd1-203">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-203">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="4ccd1-204">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-204">MPN partner admin</span></span>|<span data-ttu-id="4ccd1-205">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-205">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="4ccd1-206">Microsoft Action Pack 구독 또는 실버 및 골드 역량 구입 또는 갱신</span><span class="sxs-lookup"><span data-stu-id="4ccd1-206">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="4ccd1-207">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-207">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="4ccd1-208">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-208">\*    View user details and their skills data</span></span>
||<span data-ttu-id="4ccd1-209">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-209">\*    View competencies</span></span>
||<span data-ttu-id="4ccd1-210">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-210">\*    View and manage benefits</span></span>
||<span data-ttu-id="4ccd1-211">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="4ccd1-211">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="4ccd1-212">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-212">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="4ccd1-213">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-213">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="4ccd1-214">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="4ccd1-214">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="4ccd1-215">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-215">\*    View customer data analytics</span></span>
||<span data-ttu-id="4ccd1-216">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="4ccd1-216">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="4ccd1-217">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-217">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-218">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-218">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="4ccd1-219">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-219">Account admin</span></span>| <span data-ttu-id="4ccd1-220">위치 추가</span><span class="sxs-lookup"><span data-stu-id="4ccd1-220">Add locations</span></span>|[<span data-ttu-id="4ccd1-221">위치 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-221">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="4ccd1-222">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-222">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="4ccd1-223">\*    테넌트의 사용자에 대한 역할을 비 Azure-Active-Directory 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="4ccd1-223">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="4ccd1-224">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="4ccd1-224">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="4ccd1-225">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-225">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-226">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-226">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="4ccd1-227">조회 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-227">Manage referrals</span></span> 

|<span data-ttu-id="4ccd1-228">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-228">**Role**</span></span>|<span data-ttu-id="4ccd1-229">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-229">**What you can do**</span></span>|<span data-ttu-id="4ccd1-230">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-230">**Learn more**</span></span>|
|-----------------------------|:------------------------|---|
|<span data-ttu-id="4ccd1-231">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-231">Referrals admin</span></span>       |<span data-ttu-id="4ccd1-232">\*    비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-232">\*    View, create, and manage business profiles</span></span>|[<span data-ttu-id="4ccd1-233">고객 문의, 마케팅 한정 잠재 고객 및 판매 한정 잠재 고객과 같은 다양한 잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-233">Manage different leads like customer inquiries, marketing-qualified leads, and sales-qualified leads</span></span>](manage-leads.md)
||<span data-ttu-id="4ccd1-234">\*    조회 받기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-234">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="4ccd1-235">\* 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-235">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="4ccd1-236">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-236">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="4ccd1-237">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-237">Business profile admin</span></span>   |<span data-ttu-id="4ccd1-238">\* 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-238">\* View, create, and manage business profile</span></span> |[<span data-ttu-id="4ccd1-239">비즈니스 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-239">Create a business profile</span></span>](create-a-marketing-profile.md)
||<span data-ttu-id="4ccd1-240">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-240">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="4ccd1-241">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-241">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-242">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-242">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="4ccd1-243">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-243">Manage incentives</span></span> 

|<span data-ttu-id="4ccd1-244">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-244">**Role**</span></span> | <span data-ttu-id="4ccd1-245">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-245">**What you can do**</span></span>|<span data-ttu-id="4ccd1-246">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-246">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="4ccd1-247">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-247">Incentives admin</span></span>|<span data-ttu-id="4ccd1-248">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="4ccd1-248">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="4ccd1-249">인센티브를 시작하는 데 도움이 되도록 다음 리소스 사용</span><span class="sxs-lookup"><span data-stu-id="4ccd1-249">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="4ccd1-250">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="4ccd1-250">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="4ccd1-251">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="4ccd1-251">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="4ccd1-252">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-252">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="4ccd1-253">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="4ccd1-253">\*    Access support</span></span>
||<span data-ttu-id="4ccd1-254">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="4ccd1-254">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="4ccd1-255">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="4ccd1-255">Incentives user</span></span>|<span data-ttu-id="4ccd1-256">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="4ccd1-256">\*    Can view incentives programs</span></span>
||<span data-ttu-id="4ccd1-257">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="4ccd1-257">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="4ccd1-258">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-258">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="4ccd1-259">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-259">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4ccd1-260">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-260">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="4ccd1-261">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-261">View Partner Center Insights data</span></span>

|<span data-ttu-id="4ccd1-262">**역할**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-262">**Role**</span></span> | <span data-ttu-id="4ccd1-263">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-263">**What you can do**</span></span>|<span data-ttu-id="4ccd1-264">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="4ccd1-264">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="4ccd1-265">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="4ccd1-265">Executive report viewer</span></span>|<span data-ttu-id="4ccd1-266">모든 보고 데이터 세트에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-266">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="4ccd1-267">파트너 센터 인사이트에서 사용할 수 있는 개요 대시보드 보고서</span><span class="sxs-lookup"><span data-stu-id="4ccd1-267">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="4ccd1-268">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="4ccd1-268">Report viewer</span></span>|<span data-ttu-id="4ccd1-269">수익 및 고객과 직원 개인 데이터를 제외한 데이터 보고서에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="4ccd1-269">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="4ccd1-270">다음 단계</span><span class="sxs-lookup"><span data-stu-id="4ccd1-270">Next steps</span></span>

- [<span data-ttu-id="4ccd1-271">사용자 계정 만들기 및 역할과 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="4ccd1-271">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="4ccd1-272">새 파트너 센터 프로그램에 등록할 때 계정 정보 확인</span><span class="sxs-lookup"><span data-stu-id="4ccd1-272">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
