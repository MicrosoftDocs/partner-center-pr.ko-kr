---
title: 사용자 역할 및 권한 할당 | 파트너 센터
ms.topic: article
ms.date: 3/5/19
description: 파트너 센터에서 작동 해야 하는 모든 직원에 게를 할당 되어야 합니다.
author: LauraBrenner
ms.author: labrenne
keywords: 역할, 권한, 관리자, 에이전트
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133903"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="43e6b-104">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="43e6b-104">Assign users roles and permissions</span></span>


<span data-ttu-id="43e6b-105">올바른 이름 및 주소, 지원 세부 정보, 파일 거래 세 면제, 은행 정보 및 회사에 대 한 기본 연락처를 포함 하 여 파트너 프로필을 설정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="43e6b-106">다음 단계: 사용자 수를 사용 하 여 파트너 센터에서 작업을 시작할 수 있도록 암호 및 역할을 사용 하 여 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="43e6b-107">직원이 파트너 센터에서 작동 하도록 설정</span><span class="sxs-lookup"><span data-stu-id="43e6b-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="43e6b-108">사용자는 역할 및 사용 권한을 제공 하 여 파트너 센터 해야 하는 액세스 형식을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="43e6b-109">역할 업무에 관련 되어 있으면 관련 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="43e6b-110">예를 들어 비즈니스 클라우드 솔루션 공급자 (CSP) 비즈니스 이면 없습니다만 해야 표준 Azure AD 테 넌 트 전역 관리자와 같은 관리 역할 있지만 CSP 프로그램에 특정 역할을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="43e6b-111">각 프로그램에는 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="43e6b-112">Azure Active Directory (AAD) 테 넌 트 역할 전역 관리자, 사용자 관리자 및 CSP 역할을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="43e6b-113">MPN 관리, 비즈니스 프로필 관리, 조회 관리자, 인센티브 관리자 및 인센티브 사용자 비 AAD 역할에 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="43e6b-114">파트너 센터에서 상업용 트랜잭션 관리 (Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="43e6b-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="43e6b-115">**역할**</span><span class="sxs-lookup"><span data-stu-id="43e6b-115">**Role**</span></span>|<span data-ttu-id="43e6b-116">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="43e6b-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="43e6b-117">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-117">Global admin</span></span>|<span data-ttu-id="43e6b-118">• 모든 Microsoft 계정/서비스 전체 권한으로 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="43e6b-119">• 파트너 센터에 대 한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="43e6b-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="43e6b-120">• 보기 계약, 가격 목록 및 제품</span><span class="sxs-lookup"><span data-stu-id="43e6b-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="43e6b-121">• 뷰를 만들고 파트너 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="43e6b-122">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-122">User Admin</span></span>   | <span data-ttu-id="43e6b-123">• 뷰를 만들고 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="43e6b-124">• 모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="43e6b-124">• View all partner profiles</span></span>
||<span data-ttu-id="43e6b-125">• 뷰를 만들고 파트너 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="43e6b-126">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-126">Billing admin</span></span> | <span data-ttu-id="43e6b-127">-보기, 만들기 및 대금 청구, 송장 및 여러 파일 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="43e6b-128">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="43e6b-128">Default user</span></span>|  <span data-ttu-id="43e6b-129">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="43e6b-129">View My profile</span></span>   |
|<span data-ttu-id="43e6b-130">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="43e6b-130">Admin agent</span></span> | <span data-ttu-id="43e6b-131">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-131">•    Customer management</span></span>
||<span data-ttu-id="43e6b-132">• 파트너 센터에 장치 목록을 추가 <</span><span class="sxs-lookup"><span data-stu-id="43e6b-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="43e6b-133">• 만들기 및 장치에 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="43e6b-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="43e6b-134">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-134">• Subscription management</span></span>
||<span data-ttu-id="43e6b-135">• 고객에 대 한 상태 및 서비스 요청 서비스</span><span class="sxs-lookup"><span data-stu-id="43e6b-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="43e6b-136">위임 된 관리자 권한에 • 요청</span><span class="sxs-lookup"><span data-stu-id="43e6b-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="43e6b-137">• 보기 가격 책정 및 제품</span><span class="sxs-lookup"><span data-stu-id="43e6b-137">• View pricing and offers</span></span>
||<span data-ttu-id="43e6b-138">• 청구</span><span class="sxs-lookup"><span data-stu-id="43e6b-138">• Billing</span></span>
||<span data-ttu-id="43e6b-139">• 고객 대신 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="43e6b-140">• 레지스터 값 reseller 추가</span><span class="sxs-lookup"><span data-stu-id="43e6b-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="43e6b-141">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="43e6b-141">Sales agent</span></span> | <span data-ttu-id="43e6b-142">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-142">•    Customer management</span></span>
||<span data-ttu-id="43e6b-143">• 파트너 센터에 장치 목록을 추가</span><span class="sxs-lookup"><span data-stu-id="43e6b-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="43e6b-144">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-144">• Subscription management</span></span>
||<span data-ttu-id="43e6b-145">• 뷰 지원 티켓</span><span class="sxs-lookup"><span data-stu-id="43e6b-145">• View support tickets</span></span>
||<span data-ttu-id="43e6b-146">• 요청 고객과 관계</span><span class="sxs-lookup"><span data-stu-id="43e6b-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="43e6b-147">• 잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-147">• Manage customer leads</span></span>
||<span data-ttu-id="43e6b-148">• 고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="43e6b-148">• View the customer agreement</span></span>
||<span data-ttu-id="43e6b-149">• 등록 부가가치 재판매인</span><span class="sxs-lookup"><span data-stu-id="43e6b-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="43e6b-150">기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="43e6b-150">Helpdesk agent</span></span>| <span data-ttu-id="43e6b-151">• 검색 하 고 고객 보기</span><span class="sxs-lookup"><span data-stu-id="43e6b-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="43e6b-152">• 고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="43e6b-152">• Edit customer details</span></span>
||<span data-ttu-id="43e6b-153">• 도움말 고객 관련 문제를 해결 대금 청구 또는 구독 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="43e6b-154">• 고객을 대신해 서 지원을 요청 (참고: Office 365 구독에 대 한이 작업을 완료 하려면 관리 에이전트 여야 함)</span><span class="sxs-lookup"><span data-stu-id="43e6b-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="43e6b-155">• 구독 관리 및 고객을 대신해 서 문제를 청구 합니다. (참고: Office 365 구독에 대 한이 작업을 완료 하려면 관리 에이전트 여야 함)</span><span class="sxs-lookup"><span data-stu-id="43e6b-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="43e6b-156">컨트롤 패널 공급 업체 (CPV)입니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="43e6b-157">(CSP 역할 및 AAD가 아닌 역할)</span><span class="sxs-lookup"><span data-stu-id="43e6b-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="43e6b-158">CPVs는 파트너 센터 Api를 사용 하 여 해당 시스템을 통합할 수 있도록 클라우드 솔루션 공급자 (CSP) 파트너에서 사용할 앱을 개발 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="43e6b-159">**역할**</span><span class="sxs-lookup"><span data-stu-id="43e6b-159">**Role**</span></span>   |<span data-ttu-id="43e6b-160">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="43e6b-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="43e6b-161">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-161">Global admin</span></span>| <span data-ttu-id="43e6b-162">보기 및 CPV 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="43e6b-163">보기 및 CPV 기능에 대 한 액세스가 필요한 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="43e6b-164">MPN 멤버 자격 및 회사 (AAD가 아닌 역할)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="43e6b-165">**역할**</span><span class="sxs-lookup"><span data-stu-id="43e6b-165">**Role**</span></span> | <span data-ttu-id="43e6b-166">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="43e6b-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="43e6b-167">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-167">MPN partner admin</span></span>|<span data-ttu-id="43e6b-168">•Can 비 테 넌 트 사용자를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="43e6b-169">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="43e6b-170">• 보기 법적, 조직, 비즈니스 및 MPN 프로필</span><span class="sxs-lookup"><span data-stu-id="43e6b-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="43e6b-171">• 사용자 세부 정보 보기 및 기술 데이터</span><span class="sxs-lookup"><span data-stu-id="43e6b-171">• View user details and their skills data</span></span>
||<span data-ttu-id="43e6b-172">• 보기 역량</span><span class="sxs-lookup"><span data-stu-id="43e6b-172">• View competencies</span></span>
||<span data-ttu-id="43e6b-173">• 보기 및 혜택 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-173">• View and manage benefits</span></span>
||<span data-ttu-id="43e6b-174">MPN 제공 • 뷰와 구매</span><span class="sxs-lookup"><span data-stu-id="43e6b-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="43e6b-175">• 보기 MPN 제공 주문 기록 및 송장</span><span class="sxs-lookup"><span data-stu-id="43e6b-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="43e6b-176">• 파트너 기여 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="43e6b-176">• View partner contribution data</span></span>
||<span data-ttu-id="43e6b-177">•는 바우처 유효성 검사 도구에서 작업할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="43e6b-178">--고객 데이터 분석을 보고 하는 중</span><span class="sxs-lookup"><span data-stu-id="43e6b-178">- View customer data analytics</span></span>
|<span data-ttu-id="43e6b-179">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-179">Account admin</span></span>| <span data-ttu-id="43e6b-180">• 비 테 넌 트 사용자를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="43e6b-181">• 추가 또는 위치를 삭제 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-181">• Add or delete locations</span></span>
||<span data-ttu-id="43e6b-182">--관리자는 계정과 관련 하 여 프로필을 관리 하는 중</span><span class="sxs-lookup"><span data-stu-id="43e6b-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="43e6b-183">• 사용자 아닌 AAD 역할을 테 넌 트에 대 한 역할 할당</span><span class="sxs-lookup"><span data-stu-id="43e6b-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="43e6b-184">• 프로그램에 대 한 위치를 등록 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="43e6b-185">게스트 사용자 (AAD 테 넌 트에 추가 해야 합니다)</span><span class="sxs-lookup"><span data-stu-id="43e6b-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="43e6b-186">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="43e6b-186">**Guest user**</span></span>   | <span data-ttu-id="43e6b-187">**Roles**</span><span class="sxs-lookup"><span data-stu-id="43e6b-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="43e6b-188">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-188">MPN partner admin</span></span>|
||<span data-ttu-id="43e6b-189">계정 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-189">Accounts admin</span></span>|
||<span data-ttu-id="43e6b-190">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-190">Incentives admin</span></span>|
||<span data-ttu-id="43e6b-191">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-191">Business profile admin</span></span>|
||<span data-ttu-id="43e6b-192">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="43e6b-193">조회 (AAD가 아닌 역할)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="43e6b-194">**역할**</span><span class="sxs-lookup"><span data-stu-id="43e6b-194">**Role**</span></span>|<span data-ttu-id="43e6b-195">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="43e6b-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="43e6b-196">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-196">Referrals admin</span></span>       |<span data-ttu-id="43e6b-197">• 뷰를 만들고 비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="43e6b-198">• 받기 및 조회를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="43e6b-199">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="43e6b-200">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-200">Business profile admin</span></span>   |<span data-ttu-id="43e6b-201">•View를 만들고 비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="43e6b-202">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="43e6b-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="43e6b-203">인센티브 (AAD가 아닌 역할)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="43e6b-204">**역할**</span><span class="sxs-lookup"><span data-stu-id="43e6b-204">**Role**</span></span> | <span data-ttu-id="43e6b-205">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="43e6b-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="43e6b-206">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="43e6b-206">Incentives admin</span></span>|<span data-ttu-id="43e6b-207">• 시작 하 고 인센티브를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="43e6b-208">• 본 인센티브 프로그램의 모든 측면을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="43e6b-209">• 볼 수 있으며 은행 및 세금 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="43e6b-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="43e6b-210">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="43e6b-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="43e6b-211">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="43e6b-211">• Access support</span></span>
||<span data-ttu-id="43e6b-212">• 분쟁 인센티브 지불</span><span class="sxs-lookup"><span data-stu-id="43e6b-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="43e6b-213">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="43e6b-213">Incentives user</span></span>|<span data-ttu-id="43e6b-214">•는 인센티브 프로그램을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43e6b-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="43e6b-215">• 볼 수 있으며 인센티브 클레임 시작</span><span class="sxs-lookup"><span data-stu-id="43e6b-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="43e6b-216">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="43e6b-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="43e6b-217">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="43e6b-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="43e6b-218">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="43e6b-218">• Access support</span></span>












