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
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434322"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="13981-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="13981-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="13981-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="13981-104">**Appropriate roles**</span></span>

- <span data-ttu-id="13981-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-105">Global admin</span></span>
- <span data-ttu-id="13981-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-106">User admin</span></span>
- <span data-ttu-id="13981-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-107">MPN partner admin</span></span>

<span data-ttu-id="13981-108">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="13981-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="13981-109">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="13981-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="13981-110">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="13981-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="13981-111">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="13981-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="13981-112">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="13981-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="13981-113">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 글로벌 관리자 같은 표준 Azure AD 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="13981-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="13981-114">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="13981-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="13981-115">AAD(Azure Active Directory) 테넌트 역할에는 글로벌 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="13981-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="13981-116">비 AAD 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="13981-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="13981-117">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="13981-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="13981-118">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-118">**Role**</span></span>|<span data-ttu-id="13981-119">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="13981-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="13981-120">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-120">Global admin</span></span>|<span data-ttu-id="13981-121">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="13981-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="13981-122">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="13981-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="13981-123">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="13981-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="13981-124">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="13981-125">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="13981-126">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="13981-126">User management admin</span></span>   | <span data-ttu-id="13981-127">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="13981-128">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="13981-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="13981-129">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="13981-130">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-130">Billing admin</span></span> | <span data-ttu-id="13981-131">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="13981-132">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="13981-132">Default user</span></span>|  <span data-ttu-id="13981-133">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="13981-133">View My profile</span></span>   |
|<span data-ttu-id="13981-134">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="13981-134">Admin agent</span></span> | <span data-ttu-id="13981-135">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="13981-135">\*    Customer management</span></span>
||<span data-ttu-id="13981-136">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="13981-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="13981-137">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="13981-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="13981-138">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="13981-138">\*    Subscription management</span></span>
||<span data-ttu-id="13981-139">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="13981-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="13981-140">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="13981-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="13981-141">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="13981-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="13981-142">\*    청구</span><span class="sxs-lookup"><span data-stu-id="13981-142">\*    Billing</span></span>
||<span data-ttu-id="13981-143">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="13981-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="13981-144">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="13981-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="13981-145">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="13981-145">Sales agent</span></span> | <span data-ttu-id="13981-146">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="13981-146">\*    Customer management</span></span>
||<span data-ttu-id="13981-147">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="13981-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="13981-148">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="13981-148">\*    Subscription management</span></span>
||<span data-ttu-id="13981-149">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="13981-149">\*    View support tickets</span></span>
||<span data-ttu-id="13981-150">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="13981-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="13981-151">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="13981-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="13981-152">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="13981-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="13981-153">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="13981-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="13981-154">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="13981-154">Helpdesk agent</span></span>| <span data-ttu-id="13981-155">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="13981-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="13981-156">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="13981-156">\*    Edit customer details</span></span>
||<span data-ttu-id="13981-157">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="13981-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="13981-158">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="13981-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="13981-159">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="13981-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="13981-160">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="13981-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="13981-161">(CSP 역할 및 비 AAD 역할)</span><span class="sxs-lookup"><span data-stu-id="13981-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="13981-162">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="13981-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="13981-163">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-163">**Role**</span></span>   |<span data-ttu-id="13981-164">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="13981-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="13981-165">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-165">Global admin</span></span>| <span data-ttu-id="13981-166">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="13981-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="13981-167">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="13981-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="13981-168">게스트 사용자(AAD 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="13981-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="13981-169">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="13981-169">**Guest user**</span></span>   | <span data-ttu-id="13981-170">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="13981-171">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-171">MPN partner admin</span></span>|
||<span data-ttu-id="13981-172">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-172">Accounts admin</span></span>|
||<span data-ttu-id="13981-173">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-173">Incentives admin</span></span>|
||<span data-ttu-id="13981-174">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-174">Business profile admin</span></span>|
||<span data-ttu-id="13981-175">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="13981-176">MPN 멤버 자격과 회사 관리(비 AAD 역할: 이 역할은 테넌트가 아닌 회사 비즈니스를 관리)</span><span class="sxs-lookup"><span data-stu-id="13981-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="13981-177">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-177">**Role**</span></span> | <span data-ttu-id="13981-178">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="13981-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="13981-179">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-179">MPN partner admin</span></span>|<span data-ttu-id="13981-180">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="13981-181">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="13981-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="13981-182">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="13981-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="13981-183">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="13981-183">\*    View competencies</span></span>
||<span data-ttu-id="13981-184">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="13981-185">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="13981-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="13981-186">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="13981-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="13981-187">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="13981-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="13981-188">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="13981-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="13981-189">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="13981-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="13981-190">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="13981-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="13981-191">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-191">Account admin</span></span>| <span data-ttu-id="13981-192">위치 추가</span><span class="sxs-lookup"><span data-stu-id="13981-192">Add locations</span></span>
|| <span data-ttu-id="13981-193">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="13981-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="13981-194">\*    테넌트의 사용자에 대한 역할을 비 AAD 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="13981-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="13981-195">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="13981-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="13981-196">조회 관리</span><span class="sxs-lookup"><span data-stu-id="13981-196">Manage referrals</span></span> 

|<span data-ttu-id="13981-197">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-197">**Role**</span></span>|<span data-ttu-id="13981-198">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="13981-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="13981-199">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-199">Referrals admin</span></span>       |<span data-ttu-id="13981-200">\*    비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="13981-201">\*    조회 받기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="13981-202">\* 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="13981-203">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="13981-204">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-204">Business profile admin</span></span>   |<span data-ttu-id="13981-205">\* 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="13981-206">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="13981-207">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="13981-207">Manage incentives</span></span> 

|<span data-ttu-id="13981-208">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-208">**Role**</span></span> | <span data-ttu-id="13981-209">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="13981-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="13981-210">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="13981-210">Incentives admin</span></span>|<span data-ttu-id="13981-211">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="13981-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="13981-212">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="13981-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="13981-213">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="13981-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="13981-214">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="13981-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="13981-215">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="13981-215">\*    Access support</span></span>
||<span data-ttu-id="13981-216">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="13981-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="13981-217">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="13981-217">Incentives user</span></span>|<span data-ttu-id="13981-218">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="13981-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="13981-219">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="13981-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="13981-220">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="13981-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="13981-221">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="13981-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="13981-222">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="13981-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="13981-223">**역할**</span><span class="sxs-lookup"><span data-stu-id="13981-223">**Role**</span></span> | <span data-ttu-id="13981-224">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="13981-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="13981-225">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="13981-225">Executive report viewer</span></span>|<span data-ttu-id="13981-226">모든 보고 데이터 세트에 액세스</span><span class="sxs-lookup"><span data-stu-id="13981-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="13981-227">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="13981-227">Report viewer</span></span>|<span data-ttu-id="13981-228">수익, 고객 및 직원 개인 데이터를 제외한 데이터 보고서에 액세스</span><span class="sxs-lookup"><span data-stu-id="13981-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    