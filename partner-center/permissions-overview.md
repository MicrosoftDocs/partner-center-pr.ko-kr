---
title: 사용자 역할 및 권한 할당 | 파트너 센터
ms.topic: article
ms.date: 3/5/19
description: 파트너 센터에서 작동 해야 하는 모든 직원에 게를 할당 되어야 합니다.
author: LauraBrenner
ms.author: labrenne
keywords: 역할, 권한, 관리자, 에이전트
ms.localizationpriority: medium
ms.openlocfilehash: 65a2f7f373fc57f86cfffa73aafd3b7095fe2c04
ms.sourcegitcommit: be8086534ec73937f2be9bcc495c2627423c50f6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/26/2019
ms.locfileid: "67396734"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="a902d-104">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="a902d-104">Assign users roles and permissions</span></span>


<span data-ttu-id="a902d-105">올바른 이름 및 주소, 지원 세부 정보, 파일 거래 세 면제, 은행 정보 및 회사에 대 한 기본 연락처를 포함 하 여 파트너 프로필을 설정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="a902d-106">다음 단계: 사용자 수를 사용 하 여 파트너 센터에서 작업을 시작할 수 있도록 암호 및 역할을 사용 하 여 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="a902d-107">직원이 파트너 센터에서 작동 하도록 설정</span><span class="sxs-lookup"><span data-stu-id="a902d-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="a902d-108">사용자는 역할 및 사용 권한을 제공 하 여 파트너 센터 해야 하는 액세스 형식을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="a902d-109">역할 업무에 관련 되어 있으면 관련 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="a902d-110">예를 들어 비즈니스 클라우드 솔루션 공급자 (CSP) 비즈니스 이면 없습니다만 해야 표준 Azure AD 테 넌 트 전역 관리자와 같은 관리 역할 있지만 CSP 프로그램에 특정 역할을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="a902d-111">각 프로그램에는 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="a902d-112">Azure Active Directory (AAD) 테 넌 트 역할 전역 관리자, 사용자 관리자 및 CSP 역할을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="a902d-113">비-AAD 역할은 테 넌 트를 관리 하지 않는 해당 역할 등이 MPN 관리, 비즈니스 프로필 관리, 조회 관리자, 인센티브 관리자 인센티브 사용자입니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-113">Non-AAD roles are those roles that do not manage the tenant and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="a902d-114">파트너 센터에서 상업용 트랜잭션 관리 (Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="a902d-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="a902d-115">**역할**</span><span class="sxs-lookup"><span data-stu-id="a902d-115">**Role**</span></span>|<span data-ttu-id="a902d-116">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="a902d-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="a902d-117">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-117">Global admin</span></span>|<span data-ttu-id="a902d-118">• 모든 Microsoft 계정/서비스 전체 권한으로 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="a902d-119">• 파트너 센터에 대 한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="a902d-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a902d-120">• 보기 계약, 가격 목록 및 제품</span><span class="sxs-lookup"><span data-stu-id="a902d-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="a902d-121">• 뷰를 만들고 파트너 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="a902d-122">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-122">User Admin</span></span>   | <span data-ttu-id="a902d-123">• 뷰를 만들고 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="a902d-124">• 모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="a902d-124">• View all partner profiles</span></span>
||<span data-ttu-id="a902d-125">• 뷰를 만들고 파트너 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="a902d-126">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-126">Billing admin</span></span> | <span data-ttu-id="a902d-127">-보기, 만들기 및 대금 청구, 송장 및 여러 파일 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="a902d-128">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="a902d-128">Default user</span></span>|  <span data-ttu-id="a902d-129">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="a902d-129">View My profile</span></span>   |
|<span data-ttu-id="a902d-130">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="a902d-130">Admin agent</span></span> | <span data-ttu-id="a902d-131">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-131">•    Customer management</span></span>
||<span data-ttu-id="a902d-132">• 파트너 센터에 장치 목록을 추가 <</span><span class="sxs-lookup"><span data-stu-id="a902d-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="a902d-133">• 만들기 및 장치에 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="a902d-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="a902d-134">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-134">• Subscription management</span></span>
||<span data-ttu-id="a902d-135">• 고객에 대 한 상태 및 서비스 요청 서비스</span><span class="sxs-lookup"><span data-stu-id="a902d-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="a902d-136">위임 된 관리자 권한에 • 요청</span><span class="sxs-lookup"><span data-stu-id="a902d-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="a902d-137">• 보기 가격 책정 및 제품</span><span class="sxs-lookup"><span data-stu-id="a902d-137">• View pricing and offers</span></span>
||<span data-ttu-id="a902d-138">• 청구</span><span class="sxs-lookup"><span data-stu-id="a902d-138">• Billing</span></span>
||<span data-ttu-id="a902d-139">• 고객 대신 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="a902d-140">• 레지스터 값 reseller 추가</span><span class="sxs-lookup"><span data-stu-id="a902d-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="a902d-141">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="a902d-141">Sales agent</span></span> | <span data-ttu-id="a902d-142">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-142">•    Customer management</span></span>
||<span data-ttu-id="a902d-143">• 파트너 센터에 장치 목록을 추가</span><span class="sxs-lookup"><span data-stu-id="a902d-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="a902d-144">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-144">• Subscription management</span></span>
||<span data-ttu-id="a902d-145">• 보기 가격을 나열 하며</span><span class="sxs-lookup"><span data-stu-id="a902d-145">• View price lists and offers</span></span>
||<span data-ttu-id="a902d-146">• 뷰 지원 티켓</span><span class="sxs-lookup"><span data-stu-id="a902d-146">• View support tickets</span></span>
||<span data-ttu-id="a902d-147">• 요청 고객과 관계</span><span class="sxs-lookup"><span data-stu-id="a902d-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="a902d-148">• 잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-148">• Manage customer leads</span></span>
||<span data-ttu-id="a902d-149">• 고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="a902d-149">• View the customer agreement</span></span>
||<span data-ttu-id="a902d-150">• 등록 부가가치 재판매인</span><span class="sxs-lookup"><span data-stu-id="a902d-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="a902d-151">기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="a902d-151">Helpdesk agent</span></span>| <span data-ttu-id="a902d-152">• 검색 하 고 고객 보기</span><span class="sxs-lookup"><span data-stu-id="a902d-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="a902d-153">• 고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="a902d-153">• Edit customer details</span></span>
||<span data-ttu-id="a902d-154">• 도움말 고객 관련 문제를 해결 대금 청구 또는 구독 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="a902d-155">• 고객을 대신해 서 지원을 요청 (참고: Office 365 구독에 대 한이 작업을 완료 하려면 관리 에이전트 여야 함)</span><span class="sxs-lookup"><span data-stu-id="a902d-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="a902d-156">• 구독 관리 및 고객을 대신해 서 문제를 청구 합니다. (참고: Office 365 구독에 대 한이 작업을 완료 하려면 관리 에이전트 여야 함)</span><span class="sxs-lookup"><span data-stu-id="a902d-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="a902d-157">컨트롤 패널 공급 업체 (CPV)입니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="a902d-158">(CSP 역할 및 AAD가 아닌 역할)</span><span class="sxs-lookup"><span data-stu-id="a902d-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="a902d-159">CPVs는 파트너 센터 Api를 사용 하 여 해당 시스템을 통합할 수 있도록 클라우드 솔루션 공급자 (CSP) 파트너에서 사용할 앱을 개발 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="a902d-160">**역할**</span><span class="sxs-lookup"><span data-stu-id="a902d-160">**Role**</span></span>   |<span data-ttu-id="a902d-161">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="a902d-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="a902d-162">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-162">Global admin</span></span>| <span data-ttu-id="a902d-163">보기 및 CPV 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="a902d-164">보기 및 CPV 기능에 대 한 액세스가 필요한 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="a902d-165">게스트 사용자 (AAD 테 넌 트에 추가 해야 합니다)</span><span class="sxs-lookup"><span data-stu-id="a902d-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="a902d-166">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="a902d-166">**Guest user**</span></span>   | <span data-ttu-id="a902d-167">**Roles**</span><span class="sxs-lookup"><span data-stu-id="a902d-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="a902d-168">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-168">MPN partner admin</span></span>|
||<span data-ttu-id="a902d-169">계정 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-169">Accounts admin</span></span>|
||<span data-ttu-id="a902d-170">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-170">Incentives admin</span></span>|
||<span data-ttu-id="a902d-171">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-171">Business profile admin</span></span>|
||<span data-ttu-id="a902d-172">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="a902d-173">MPN 멤버 자격 및 회사 관리 (비 AAD 역할: 이러한 역할을 테 넌 트 대신 회사 비즈니스 관리)</span><span class="sxs-lookup"><span data-stu-id="a902d-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="a902d-174">**역할**</span><span class="sxs-lookup"><span data-stu-id="a902d-174">**Role**</span></span> | <span data-ttu-id="a902d-175">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="a902d-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="a902d-176">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-176">MPN partner admin</span></span>|<span data-ttu-id="a902d-177">•Can 비 테 넌 트 사용자를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-177">•Can add non-tenant users</span></span>
||<span data-ttu-id="a902d-178">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-178">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="a902d-179">• 보기 법적, 조직, 비즈니스 및 MPN 프로필</span><span class="sxs-lookup"><span data-stu-id="a902d-179">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="a902d-180">• 사용자 세부 정보 보기 및 기술 데이터</span><span class="sxs-lookup"><span data-stu-id="a902d-180">• View user details and their skills data</span></span>
||<span data-ttu-id="a902d-181">• 보기 역량</span><span class="sxs-lookup"><span data-stu-id="a902d-181">• View competencies</span></span>
||<span data-ttu-id="a902d-182">• 보기 및 혜택 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-182">• View and manage benefits</span></span>
||<span data-ttu-id="a902d-183">MPN 제공 • 뷰와 구매</span><span class="sxs-lookup"><span data-stu-id="a902d-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="a902d-184">• 보기 MPN 제공 주문 기록 및 송장</span><span class="sxs-lookup"><span data-stu-id="a902d-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="a902d-185">• 파트너 기여 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="a902d-185">• View partner contribution data</span></span>
||<span data-ttu-id="a902d-186">•는 바우처 유효성 검사 도구에서 작업할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="a902d-187">--고객 데이터 분석을 보고 하는 중</span><span class="sxs-lookup"><span data-stu-id="a902d-187">- View customer data analytics</span></span>
|<span data-ttu-id="a902d-188">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-188">Account admin</span></span>| <span data-ttu-id="a902d-189">• 비 테 넌 트 사용자를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-189">•   Can add non-tenant users</span></span>
||<span data-ttu-id="a902d-190">• 추가 또는 위치를 삭제 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-190">• Add or delete locations</span></span>
||<span data-ttu-id="a902d-191">--관리자는 계정과 관련 하 여 프로필을 관리 하는 중</span><span class="sxs-lookup"><span data-stu-id="a902d-191">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="a902d-192">• 사용자 아닌 AAD 역할을 테 넌 트에 대 한 역할 할당</span><span class="sxs-lookup"><span data-stu-id="a902d-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="a902d-193">• 프로그램에 대 한 위치를 등록 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="a902d-194">조회를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-194">Manage referrals</span></span> 

|<span data-ttu-id="a902d-195">**역할**</span><span class="sxs-lookup"><span data-stu-id="a902d-195">**Role**</span></span>|<span data-ttu-id="a902d-196">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="a902d-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="a902d-197">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-197">Referrals admin</span></span>       |<span data-ttu-id="a902d-198">• 뷰를 만들고 비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="a902d-199">• 받기 및 조회를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="a902d-200">• 뷰를 만들고 공동 판매 조회를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="a902d-201">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="a902d-202">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-202">Business profile admin</span></span>   |<span data-ttu-id="a902d-203">• 뷰를 만들고 비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="a902d-204">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="a902d-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="a902d-205">인센티브를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-205">Manage incentives</span></span> 

|<span data-ttu-id="a902d-206">**역할**</span><span class="sxs-lookup"><span data-stu-id="a902d-206">**Role**</span></span> | <span data-ttu-id="a902d-207">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="a902d-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="a902d-208">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="a902d-208">Incentives admin</span></span>|<span data-ttu-id="a902d-209">• 시작 하 고 인센티브를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="a902d-210">• 본 인센티브 프로그램의 모든 측면을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="a902d-211">• 볼 수 있으며 은행 및 세금 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="a902d-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="a902d-212">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="a902d-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="a902d-213">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="a902d-213">• Access support</span></span>
||<span data-ttu-id="a902d-214">• 분쟁 인센티브 지불</span><span class="sxs-lookup"><span data-stu-id="a902d-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="a902d-215">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="a902d-215">Incentives user</span></span>|<span data-ttu-id="a902d-216">•는 인센티브 프로그램을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a902d-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="a902d-217">• 볼 수 있으며 인센티브 클레임 시작</span><span class="sxs-lookup"><span data-stu-id="a902d-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="a902d-218">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="a902d-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="a902d-219">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="a902d-219">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="a902d-220">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="a902d-220">• Access support</span></span>












