---
title: 사용자 역할 및 권한 할당 | 파트너 센터
ms.topic: article
ms.date: 3/5/2019
description: 파트너 센터에서 작업 해야 하는 모든 직원에 게 역할을 할당 해야 합니다.
author: LauraBrenner
ms.author: labrenne
keywords: 역할, 권한, 관리자, 에이전트
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708863"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="7bf54-104">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="7bf54-104">Assign users roles and permissions</span></span>


<span data-ttu-id="7bf54-105">법적 이름과 주소, 지원 세부 정보, 파일 세금 면제, 은행 정보 및 회사의 기본 연락처를 포함 하 여 파트너 프로필을 설정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7bf54-106">다음 단계: 파트너 센터에서 작업을 시작할 수 있도록 사용자에 게 암호 및 역할로 설정 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="7bf54-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7bf54-107">파트너 센터에서 작업 하도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="7bf54-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7bf54-108">파트너 센터에서 사용자에 게 부여 하는 액세스 유형 (역할 및 권한 부여)을 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7bf54-109">역할은 비즈니스와 관련 된 프로그램에 관련 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7bf54-110">예를 들어 비즈니스는 CSP (클라우드 솔루션 공급자) 비즈니스 인 경우 전역 관리자와 같은 표준 Azure AD 테 넌 트 관리 역할이 있지만 CSP 프로그램과 관련 된 역할이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7bf54-111">각 프로그램에는 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7bf54-112">AAD (Azure Active Directory) 테 넌 트 역할에는 전역 관리자, 사용자 관리자 및 CSP 역할이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7bf54-113">비 AAD 역할은 테 넌 트를 관리 하지 않는 역할이 며 MPN admin, business profile admin, 조회 관리자, 동기 관리자 및 동기 사용자를 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7bf54-114">파트너 센터에서 상업적 트랜잭션 관리 (Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="7bf54-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7bf54-115">**역할**</span><span class="sxs-lookup"><span data-stu-id="7bf54-115">**Role**</span></span>|<span data-ttu-id="7bf54-116">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="7bf54-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7bf54-117">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-117">Global admin</span></span>|<span data-ttu-id="7bf54-118">• 모든 권한이 있는 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7bf54-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7bf54-119">• 파트너 센터에 대 한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="7bf54-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7bf54-120">• 계약, 가격 목록 및 제안 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7bf54-121">• 파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7bf54-122">청구, 송장 및 정찰 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7bf54-123">사용자 관리 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-123">User management admin</span></span>   | <span data-ttu-id="7bf54-124">• 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="7bf54-125">• 모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-125">• View all partner profiles</span></span>
||<span data-ttu-id="7bf54-126">• 파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="7bf54-127">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-127">Billing admin</span></span> | <span data-ttu-id="7bf54-128">-청구, 송장 및 정찰 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="7bf54-129">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="7bf54-129">Default user</span></span>|  <span data-ttu-id="7bf54-130">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-130">View My profile</span></span>   |
|<span data-ttu-id="7bf54-131">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="7bf54-131">Admin agent</span></span> | <span data-ttu-id="7bf54-132">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-132">•    Customer management</span></span>
||<span data-ttu-id="7bf54-133">• 파트너 센터에 장치 목록 추가</span><span class="sxs-lookup"><span data-stu-id="7bf54-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="7bf54-134">• 프로필을 만들어 장치에 적용</span><span class="sxs-lookup"><span data-stu-id="7bf54-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="7bf54-135">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-135">• Subscription management</span></span>
||<span data-ttu-id="7bf54-136">• 고객에 대 한 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="7bf54-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="7bf54-137">• 위임 된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="7bf54-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="7bf54-138">• 가격 책정 및 제안 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-138">• View pricing and offers</span></span>
||<span data-ttu-id="7bf54-139">• 청구</span><span class="sxs-lookup"><span data-stu-id="7bf54-139">• Billing</span></span>
||<span data-ttu-id="7bf54-140">• 고객을 대신 하 여 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="7bf54-141">• 추가 된 재판매인 값 등록</span><span class="sxs-lookup"><span data-stu-id="7bf54-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="7bf54-142">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="7bf54-142">Sales agent</span></span> | <span data-ttu-id="7bf54-143">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-143">•    Customer management</span></span>
||<span data-ttu-id="7bf54-144">• 파트너 센터에 장치 목록 추가</span><span class="sxs-lookup"><span data-stu-id="7bf54-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="7bf54-145">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-145">• Subscription management</span></span>
||<span data-ttu-id="7bf54-146">• 가격 목록 및 제안 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-146">• View price lists and offers</span></span>
||<span data-ttu-id="7bf54-147">• 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-147">• View support tickets</span></span>
||<span data-ttu-id="7bf54-148">• 고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="7bf54-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="7bf54-149">• 고객 리더 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-149">• Manage customer leads</span></span>
||<span data-ttu-id="7bf54-150">• 고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-150">• View the customer agreement</span></span>
||<span data-ttu-id="7bf54-151">• 부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="7bf54-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="7bf54-152">기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="7bf54-152">Helpdesk agent</span></span>| <span data-ttu-id="7bf54-153">• 고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="7bf54-154">• 고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="7bf54-154">• Edit customer details</span></span>
||<span data-ttu-id="7bf54-155">• 청구 또는 구독 관리를 통해 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="7bf54-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7bf54-156">• 고객을 대신 하 여 지원 요청 (참고: Office 365 구독에 대해이 작업을 완료 하려면 관리 에이전트 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="7bf54-157">• 고객을 대신 하 여 구독 및 청구 문제를 관리 합니다 (참고: Office 365 구독에 대해이 작업을 완료 하려면 관리 에이전트 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7bf54-158">CPV (제어판 공급 업체).</span><span class="sxs-lookup"><span data-stu-id="7bf54-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7bf54-159">(CSP 역할 및 비 AAD 역할)</span><span class="sxs-lookup"><span data-stu-id="7bf54-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7bf54-160">CPVs는 CSP (클라우드 솔루션 공급자) 파트너가 사용 하는 앱을 개발 하 여 해당 시스템을 파트너 센터 Api와 통합할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7bf54-161">**역할**</span><span class="sxs-lookup"><span data-stu-id="7bf54-161">**Role**</span></span>   |<span data-ttu-id="7bf54-162">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="7bf54-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7bf54-163">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-163">Global admin</span></span>| <span data-ttu-id="7bf54-164">CPV 프로필 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7bf54-165">CPV 기능에 액세스 해야 하는 사용자를 보고 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7bf54-166">게스트 사용자 (AAD 테 넌 트에 추가 해야 함)</span><span class="sxs-lookup"><span data-stu-id="7bf54-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7bf54-167">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="7bf54-167">**Guest user**</span></span>   | <span data-ttu-id="7bf54-168">**Roles**</span><span class="sxs-lookup"><span data-stu-id="7bf54-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7bf54-169">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-169">MPN partner admin</span></span>|
||<span data-ttu-id="7bf54-170">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-170">Accounts admin</span></span>|
||<span data-ttu-id="7bf54-171">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-171">Incentives admin</span></span>|
||<span data-ttu-id="7bf54-172">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-172">Business profile admin</span></span>|
||<span data-ttu-id="7bf54-173">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7bf54-174">MPN 멤버 자격과 회사 (비 AAD 역할: 이러한 역할은 테 넌 트가 아닌 회사 비즈니스를 관리)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7bf54-175">**역할**</span><span class="sxs-lookup"><span data-stu-id="7bf54-175">**Role**</span></span> | <span data-ttu-id="7bf54-176">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="7bf54-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7bf54-177">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-177">MPN partner admin</span></span>|<span data-ttu-id="7bf54-178">• 파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7bf54-179">• 법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7bf54-180">• 사용자 세부 정보 및 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-180">• View user details and their skills data</span></span>
||<span data-ttu-id="7bf54-181">• 보기 능력</span><span class="sxs-lookup"><span data-stu-id="7bf54-181">• View competencies</span></span>
||<span data-ttu-id="7bf54-182">• 혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-182">• View and manage benefits</span></span>
||<span data-ttu-id="7bf54-183">• MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="7bf54-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="7bf54-184">• 보기 MPN 제공 주문 기록 및 청구서</span><span class="sxs-lookup"><span data-stu-id="7bf54-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7bf54-185">• 파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="7bf54-186">• 무료 정품 유효성 검사 도구에서 작업할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7bf54-187">-고객 데이터 분석 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-187">- View customer data analytics</span></span>
|| <span data-ttu-id="7bf54-188">회사 내의 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수 없음</span><span class="sxs-lookup"><span data-stu-id="7bf54-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="7bf54-189">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-189">Account admin</span></span>| <span data-ttu-id="7bf54-190">위치 추가</span><span class="sxs-lookup"><span data-stu-id="7bf54-190">Add locations</span></span>
|| <span data-ttu-id="7bf54-191">관리자 계정에 관련 된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7bf54-192">• 비 AAD 역할에 테 넌 트의 사용자에 대 한 역할 할당</span><span class="sxs-lookup"><span data-stu-id="7bf54-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7bf54-193">• 프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="7bf54-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7bf54-194">조회 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-194">Manage referrals</span></span> 

|<span data-ttu-id="7bf54-195">**역할**</span><span class="sxs-lookup"><span data-stu-id="7bf54-195">**Role**</span></span>|<span data-ttu-id="7bf54-196">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="7bf54-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7bf54-197">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-197">Referrals admin</span></span>       |<span data-ttu-id="7bf54-198">• 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="7bf54-199">• 조회 수신 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="7bf54-200">• 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7bf54-201">• 파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7bf54-202">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-202">Business profile admin</span></span>   |<span data-ttu-id="7bf54-203">• 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="7bf54-204">• 파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7bf54-205">성과급 관리</span><span class="sxs-lookup"><span data-stu-id="7bf54-205">Manage incentives</span></span> 

|<span data-ttu-id="7bf54-206">**역할**</span><span class="sxs-lookup"><span data-stu-id="7bf54-206">**Role**</span></span> | <span data-ttu-id="7bf54-207">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="7bf54-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7bf54-208">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="7bf54-208">Incentives admin</span></span>|<span data-ttu-id="7bf54-209">• 성과급을 시작 하 고 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="7bf54-210">• 성과급 프로그램의 모든 측면을 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7bf54-211">• 은행 및 세금 세부 정보를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7bf54-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7bf54-212">• 리베이트 및 공동 op 수익 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="7bf54-213">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="7bf54-213">• Access support</span></span>
||<span data-ttu-id="7bf54-214">• 분쟁의 성과급 상환</span><span class="sxs-lookup"><span data-stu-id="7bf54-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="7bf54-215">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="7bf54-215">Incentives user</span></span>|<span data-ttu-id="7bf54-216">• 성과급 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="7bf54-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="7bf54-217">• 성과급 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="7bf54-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7bf54-218">• 리베이트 및 공동 op 수익 보기</span><span class="sxs-lookup"><span data-stu-id="7bf54-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="7bf54-219">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="7bf54-219">• Access support</span></span>












