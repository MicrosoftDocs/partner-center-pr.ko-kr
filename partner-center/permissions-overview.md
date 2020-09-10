---
title: 사용자에게 역할 및 사용 권한 할당
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 상업 거래, 조회, 인센티브 또는 MPN 멤버십을 관리하는 회사 사용자에게 가장 적합한 역할에 대해 알아보세요.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 2e8608c194057ea811890c9c575f8964b63564f0
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/04/2020
ms.locfileid: "89490601"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="305e3-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="305e3-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="305e3-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="305e3-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-105">Global admin</span></span>
- <span data-ttu-id="305e3-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-106">User admin</span></span>
- <span data-ttu-id="305e3-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-107">MPN partner admin</span></span>

<span data-ttu-id="305e3-108">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="305e3-109">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="305e3-110">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="305e3-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="305e3-111">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="305e3-112">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="305e3-113">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 글로벌 관리자 같은 표준 Azure AD 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="305e3-114">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="305e3-115">AAD(Azure Active Directory) 테넌트 역할에는 글로벌 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="305e3-116">비 AAD 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="305e3-117">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="305e3-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="305e3-118">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-118">**Role**</span></span>|<span data-ttu-id="305e3-119">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="305e3-119">**What they can do**</span></span>|<span data-ttu-id="305e3-120">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="305e3-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="305e3-121">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-121">Global admin</span></span>|<span data-ttu-id="305e3-122">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="305e3-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="305e3-123">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="305e3-124">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-125">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="305e3-126">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="305e3-127">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="305e3-128">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="305e3-129">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="305e3-129">User management admin</span></span>   | <span data-ttu-id="305e3-130">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="305e3-131">파트너 센터에서 Microsoft 파트너 네트워크 멤버십 혜택 및 제품 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="305e3-132">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="305e3-133">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-134">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="305e3-135">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-135">Billing admin</span></span> | <span data-ttu-id="305e3-136">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="305e3-137">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="305e3-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="305e3-138">\*    가격 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-138">\*    View pricing</span></span>
||<span data-ttu-id="305e3-139">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-140">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="305e3-141">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="305e3-141">Default user</span></span>|  <span data-ttu-id="305e3-142">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-142">View My profile</span></span>   |[<span data-ttu-id="305e3-143">암호 재설정</span><span class="sxs-lookup"><span data-stu-id="305e3-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="305e3-144">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="305e3-144">Admin agent</span></span> | <span data-ttu-id="305e3-145">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-145">\*    Customer management</span></span>|[<span data-ttu-id="305e3-146">파트너 센터에서 재판매인 파트너를 위한 고객 계정 설정 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-146">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)
||<span data-ttu-id="305e3-147">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="305e3-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="305e3-148">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="305e3-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="305e3-149">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-149">\*    Subscription management</span></span>
||<span data-ttu-id="305e3-150">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="305e3-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="305e3-151">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="305e3-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="305e3-152">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="305e3-153">\*    청구</span><span class="sxs-lookup"><span data-stu-id="305e3-153">\*    Billing</span></span>
||<span data-ttu-id="305e3-154">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="305e3-155">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="305e3-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="305e3-156">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-157">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="305e3-158">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="305e3-158">Sales agent</span></span> | <span data-ttu-id="305e3-159">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-159">\*    Customer management</span></span>|[<span data-ttu-id="305e3-160">고객에 대한 청구 지원 제공 및 청구 질문에 대한 답변 지원</span><span class="sxs-lookup"><span data-stu-id="305e3-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="305e3-161">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="305e3-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="305e3-162">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-162">\*    Subscription management</span></span>
||<span data-ttu-id="305e3-163">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-163">\*    View support tickets</span></span>
||<span data-ttu-id="305e3-164">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="305e3-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="305e3-165">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="305e3-166">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="305e3-167">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="305e3-168">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="305e3-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="305e3-169">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-170">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="305e3-171">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="305e3-171">Helpdesk agent</span></span>| <span data-ttu-id="305e3-172">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="305e3-173">Microsoft로 문제를 에스컬레이션하고 Microsoft 에스컬레이션에 더 적합한 문제 알아보기</span><span class="sxs-lookup"><span data-stu-id="305e3-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="305e3-174">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="305e3-174">\*    Edit customer details</span></span>
||<span data-ttu-id="305e3-175">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="305e3-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="305e3-176">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="305e3-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="305e3-177">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="305e3-178">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-179">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="305e3-180">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="305e3-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="305e3-181">(CSP 역할 및 비 AAD 역할)</span><span class="sxs-lookup"><span data-stu-id="305e3-181">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="305e3-182">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="305e3-183">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-183">**Role**</span></span>   |<span data-ttu-id="305e3-184">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="305e3-184">**What you can do**</span></span>|<span data-ttu-id="305e3-185">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="305e3-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="305e3-186">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-186">Global admin</span></span>| <span data-ttu-id="305e3-187">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="305e3-188">CSP 파트너 시스템을 파트너 센터 API와 통합하는 데 도움이 되도록 제어판 공급업체로 등록</span><span class="sxs-lookup"><span data-stu-id="305e3-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="305e3-189">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="305e3-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="305e3-190">게스트 사용자(AAD 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="305e3-190">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="305e3-191">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="305e3-191">**Guest user**</span></span>   | <span data-ttu-id="305e3-192">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="305e3-193">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-193">MPN partner admin</span></span>|
||<span data-ttu-id="305e3-194">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-194">Accounts admin</span></span>|
||<span data-ttu-id="305e3-195">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-195">Incentives admin</span></span>|
||<span data-ttu-id="305e3-196">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-196">Business profile admin</span></span>|
||<span data-ttu-id="305e3-197">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-197">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="305e3-198">MPN 멤버 자격과 회사 관리(비 AAD 역할: 이 역할은 테넌트가 아닌 회사 비즈니스를 관리)</span><span class="sxs-lookup"><span data-stu-id="305e3-198">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="305e3-199">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-199">**Role**</span></span> | <span data-ttu-id="305e3-200">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="305e3-200">**What you can do**</span></span>|<span data-ttu-id="305e3-201">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="305e3-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="305e3-202">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-202">MPN partner admin</span></span>|<span data-ttu-id="305e3-203">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="305e3-204">Microsoft Action Pack 구독 또는 실버 및 골드 역량 구입 또는 갱신</span><span class="sxs-lookup"><span data-stu-id="305e3-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="305e3-205">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="305e3-206">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="305e3-207">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-207">\*    View competencies</span></span>
||<span data-ttu-id="305e3-208">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="305e3-209">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="305e3-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="305e3-210">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="305e3-211">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="305e3-212">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="305e3-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="305e3-213">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="305e3-214">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="305e3-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="305e3-215">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-216">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="305e3-217">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-217">Account admin</span></span>| <span data-ttu-id="305e3-218">위치 추가</span><span class="sxs-lookup"><span data-stu-id="305e3-218">Add locations</span></span>|[<span data-ttu-id="305e3-219">위치 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="305e3-220">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="305e3-221">\*    테넌트의 사용자에 대한 역할을 비 AAD 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="305e3-221">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="305e3-222">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="305e3-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="305e3-223">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-224">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-224">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="305e3-225">조회 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-225">Manage referrals</span></span> 

|<span data-ttu-id="305e3-226">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-226">**Role**</span></span>|<span data-ttu-id="305e3-227">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="305e3-227">**What you can do**</span></span>|<span data-ttu-id="305e3-228">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="305e3-228">**Learn more**</span></span>|
|-----------------------------|:------------------------|---|
|<span data-ttu-id="305e3-229">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-229">Referrals admin</span></span>       |<span data-ttu-id="305e3-230">\*    비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-230">\*    View, create, and manage business profiles</span></span>|[<span data-ttu-id="305e3-231">고객 문의, 마케팅 한정 잠재 고객 및 판매 한정 잠재 고객과 같은 다양한 잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-231">Manage different leads like customer inquiries, marketing-qualified leads, and sales-qualified leads</span></span>](manage-leads.md)
||<span data-ttu-id="305e3-232">\*    조회 받기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-232">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="305e3-233">\* 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-233">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="305e3-234">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-234">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="305e3-235">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-235">Business profile admin</span></span>   |<span data-ttu-id="305e3-236">\* 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-236">\* View, create, and manage business profile</span></span> |[<span data-ttu-id="305e3-237">비즈니스 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-237">Create a business profile</span></span>](create-a-marketing-profile.md)
||<span data-ttu-id="305e3-238">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-238">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="305e3-239">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-239">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-240">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-240">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="305e3-241">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-241">Manage incentives</span></span> 

|<span data-ttu-id="305e3-242">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-242">**Role**</span></span> | <span data-ttu-id="305e3-243">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="305e3-243">**What you can do**</span></span>|<span data-ttu-id="305e3-244">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="305e3-244">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="305e3-245">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="305e3-245">Incentives admin</span></span>|<span data-ttu-id="305e3-246">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="305e3-246">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="305e3-247">인센티브를 시작하는 데 도움이 되도록 다음 리소스 사용</span><span class="sxs-lookup"><span data-stu-id="305e3-247">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="305e3-248">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="305e3-248">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="305e3-249">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="305e3-249">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="305e3-250">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-250">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="305e3-251">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="305e3-251">\*    Access support</span></span>
||<span data-ttu-id="305e3-252">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="305e3-252">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="305e3-253">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="305e3-253">Incentives user</span></span>|<span data-ttu-id="305e3-254">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="305e3-254">\*    Can view incentives programs</span></span>
||<span data-ttu-id="305e3-255">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="305e3-255">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="305e3-256">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-256">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="305e3-257">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="305e3-257">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="305e3-258">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-258">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="305e3-259">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-259">View Partner Center Insights data</span></span>

|<span data-ttu-id="305e3-260">**역할**</span><span class="sxs-lookup"><span data-stu-id="305e3-260">**Role**</span></span> | <span data-ttu-id="305e3-261">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="305e3-261">**What you can do**</span></span>|<span data-ttu-id="305e3-262">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="305e3-262">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="305e3-263">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="305e3-263">Executive report viewer</span></span>|<span data-ttu-id="305e3-264">모든 보고 데이터 세트에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-264">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="305e3-265">파트너 센터 인사이트에서 사용할 수 있는 개요 대시보드 보고서</span><span class="sxs-lookup"><span data-stu-id="305e3-265">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="305e3-266">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="305e3-266">Report viewer</span></span>|<span data-ttu-id="305e3-267">수익 및 고객과 직원 개인 데이터를 제외한 데이터 보고서에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="305e3-267">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="305e3-268">다음 단계</span><span class="sxs-lookup"><span data-stu-id="305e3-268">Next steps</span></span>

- [<span data-ttu-id="305e3-269">사용자 계정 만들기 및 역할과 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="305e3-269">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="305e3-270">새 파트너 센터 프로그램에 등록할 때 계정 정보 확인</span><span class="sxs-lookup"><span data-stu-id="305e3-270">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)










                                    
