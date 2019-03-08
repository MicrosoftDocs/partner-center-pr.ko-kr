---
title: 사용자 역할 및 권한 할당 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 파트너 센터에서 작동 해야 하는 모든 직원에 게를 할당 되어야 합니다.
author: LauraBrenner
ms.author: labrenne
keywords: 역할, 권한, 관리자, 에이전트
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587746"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="e1138-104">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="e1138-104">Assign users roles and permissions</span></span>


<span data-ttu-id="e1138-105">올바른 이름 및 주소, 지원 세부 정보, 파일 거래 세 면제, 은행 정보 및 회사에 대 한 기본 연락처를 포함 하 여 파트너 프로필을 설정 했습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="e1138-106">다음 단계: 사용자 수를 사용 하 여 파트너 센터에서 작업을 시작할 수 있도록 암호 및 역할을 사용 하 여 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="e1138-107">직원이 파트너 센터에서 작동 하도록 설정</span><span class="sxs-lookup"><span data-stu-id="e1138-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="e1138-108">사용자는 역할 및 사용 권한을 제공 하 여 파트너 센터 해야 하는 액세스 형식을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="e1138-109">역할 업무에 관련 되어 있으면 관련 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="e1138-110">예를 들어 비즈니스 클라우드 솔루션 공급자 (CSP) 비즈니스 이면 없습니다만 해야 표준 Azure AD 테 넌 트 전역 관리자와 같은 관리 역할 있지만 CSP 프로그램에 특정 역할을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="e1138-111">각 프로그램에는 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="e1138-112">Azure Active Directory (AAD) 테 넌 트 역할 전역 관리자, 사용자 관리자 및 CSP 역할을 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="e1138-113">MPN 관리, 비즈니스 프로필 관리, 조회 관리자, 인센티브 관리자 및 인센티브 사용자 비 AAD 역할에 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="e1138-114">파트너 센터에서 상업용 트랜잭션 관리 (Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="e1138-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="e1138-115">**역할**</span><span class="sxs-lookup"><span data-stu-id="e1138-115">**Role**</span></span>|<span data-ttu-id="e1138-116">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="e1138-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="e1138-117">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-117">Global admin</span></span>|<span data-ttu-id="e1138-118">• 모든 Microsoft 계정/서비스 전체 권한으로 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="e1138-119">• 파트너 센터에 대 한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="e1138-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="e1138-120">• 보기 계약, 가격 목록 및 제품</span><span class="sxs-lookup"><span data-stu-id="e1138-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="e1138-121">• 뷰를 만들고 파트너 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="e1138-122">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-122">User Admin</span></span>   | <span data-ttu-id="e1138-123">• 뷰를 만들고 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="e1138-124">• 모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="e1138-124">• View all partner profiles</span></span>
||<span data-ttu-id="e1138-125">• 뷰를 만들고 파트너 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="e1138-126">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="e1138-126">Default user</span></span>|  <span data-ttu-id="e1138-127">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="e1138-127">View My profile</span></span>   |
|<span data-ttu-id="e1138-128">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="e1138-128">Admin agent</span></span> | <span data-ttu-id="e1138-129">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-129">•    Customer management</span></span>
||<span data-ttu-id="e1138-130">• 파트너 센터에 장치 목록을 추가 <</span><span class="sxs-lookup"><span data-stu-id="e1138-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="e1138-131">• 만들기 및 장치에 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="e1138-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="e1138-132">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-132">• Subscription management</span></span>
||<span data-ttu-id="e1138-133">• 고객에 대 한 상태 및 서비스 요청 서비스</span><span class="sxs-lookup"><span data-stu-id="e1138-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="e1138-134">위임 된 관리자 권한에 • 요청</span><span class="sxs-lookup"><span data-stu-id="e1138-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="e1138-135">• 보기 가격 책정 및 제품</span><span class="sxs-lookup"><span data-stu-id="e1138-135">• View pricing and offers</span></span>
||<span data-ttu-id="e1138-136">• 청구</span><span class="sxs-lookup"><span data-stu-id="e1138-136">• Billing</span></span>
||<span data-ttu-id="e1138-137">• 고객 대신 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="e1138-138">• 레지스터 값 reseller 추가</span><span class="sxs-lookup"><span data-stu-id="e1138-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="e1138-139">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="e1138-139">Sales agent</span></span> | <span data-ttu-id="e1138-140">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-140">•    Customer management</span></span>
||<span data-ttu-id="e1138-141">• 파트너 센터에 장치 목록을 추가</span><span class="sxs-lookup"><span data-stu-id="e1138-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="e1138-142">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-142">• Subscription management</span></span>
||<span data-ttu-id="e1138-143">• 뷰 지원 티켓</span><span class="sxs-lookup"><span data-stu-id="e1138-143">• View support tickets</span></span>
||<span data-ttu-id="e1138-144">• 요청 고객과 관계</span><span class="sxs-lookup"><span data-stu-id="e1138-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="e1138-145">• 잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-145">• Manage customer leads</span></span>
||<span data-ttu-id="e1138-146">• 고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="e1138-146">• View the customer agreement</span></span>
||<span data-ttu-id="e1138-147">• 등록 부가가치 재판매인</span><span class="sxs-lookup"><span data-stu-id="e1138-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="e1138-148">기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="e1138-148">Helpdesk agent</span></span>| <span data-ttu-id="e1138-149">• 검색 하 고 고객 보기</span><span class="sxs-lookup"><span data-stu-id="e1138-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="e1138-150">• 고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="e1138-150">• Edit customer details</span></span>
||<span data-ttu-id="e1138-151">• 도움말 고객 관련 문제를 해결 대금 청구 또는 구독 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="e1138-152">• 고객을 대신해 서 지원을 요청 (참고: Office 365 구독에 대 한이 작업을 완료 하려면 관리 에이전트 여야 함)</span><span class="sxs-lookup"><span data-stu-id="e1138-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="e1138-153">• 구독 관리 및 고객을 대신해 서 문제를 청구 합니다. (참고: Office 365 구독에 대 한이 작업을 완료 하려면 관리 에이전트 여야 함)</span><span class="sxs-lookup"><span data-stu-id="e1138-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="e1138-154">컨트롤 패널 공급 업체 (CPV)입니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="e1138-155">(CSP 역할 및 AAD가 아닌 역할)</span><span class="sxs-lookup"><span data-stu-id="e1138-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="e1138-156">CPVs는 파트너 센터 Api를 사용 하 여 해당 시스템을 통합할 수 있도록 클라우드 솔루션 공급자 (CSP) 파트너에서 사용할 앱을 개발 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="e1138-157">**역할**</span><span class="sxs-lookup"><span data-stu-id="e1138-157">**Role**</span></span>   |<span data-ttu-id="e1138-158">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="e1138-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="e1138-159">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-159">Global admin</span></span>| <span data-ttu-id="e1138-160">보기 및 CPV 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="e1138-161">보기 및 CPV 기능에 대 한 액세스가 필요한 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="e1138-162">MPN 멤버 자격 및 회사 (AAD가 아닌 역할)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="e1138-163">**역할**</span><span class="sxs-lookup"><span data-stu-id="e1138-163">**Role**</span></span> | <span data-ttu-id="e1138-164">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="e1138-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="e1138-165">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-165">MPN partner admin</span></span>|<span data-ttu-id="e1138-166">•Can 비 테 넌 트 사용자를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="e1138-167">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="e1138-168">• 보기 법적, 조직, 비즈니스 및 MPN 프로필</span><span class="sxs-lookup"><span data-stu-id="e1138-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="e1138-169">• 사용자 세부 정보 보기 및 기술 데이터</span><span class="sxs-lookup"><span data-stu-id="e1138-169">• View user details and their skills data</span></span>
||<span data-ttu-id="e1138-170">• 보기 역량</span><span class="sxs-lookup"><span data-stu-id="e1138-170">• View competencies</span></span>
||<span data-ttu-id="e1138-171">• 보기 및 혜택 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-171">• View and manage benefits</span></span>
||<span data-ttu-id="e1138-172">MPN 제공 • 뷰와 구매</span><span class="sxs-lookup"><span data-stu-id="e1138-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="e1138-173">• 보기 MPN 제공 주문 기록 및 송장</span><span class="sxs-lookup"><span data-stu-id="e1138-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="e1138-174">• 파트너 기여 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="e1138-174">• View partner contribution data</span></span>
||<span data-ttu-id="e1138-175">•는 바우처 유효성 검사 도구에서 작업할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="e1138-176">--고객 데이터 분석을 보고 하는 중</span><span class="sxs-lookup"><span data-stu-id="e1138-176">- View customer data analytics</span></span>
|<span data-ttu-id="e1138-177">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-177">Account admin</span></span>| <span data-ttu-id="e1138-178">• 비 테 넌 트 사용자를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="e1138-179">• 추가 또는 위치를 삭제 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-179">• Add or delete locations</span></span>
||<span data-ttu-id="e1138-180">--관리자는 계정과 관련 하 여 프로필을 관리 하는 중</span><span class="sxs-lookup"><span data-stu-id="e1138-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="e1138-181">• 사용자 아닌 AAD 역할을 테 넌 트에 대 한 역할 할당</span><span class="sxs-lookup"><span data-stu-id="e1138-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="e1138-182">• 프로그램에 대 한 위치를 등록 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="e1138-183">조회 (AAD가 아닌 역할)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="e1138-184">**역할**</span><span class="sxs-lookup"><span data-stu-id="e1138-184">**Role**</span></span>|<span data-ttu-id="e1138-185">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="e1138-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="e1138-186">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-186">Referrals admin</span></span>       |<span data-ttu-id="e1138-187">• 뷰를 만들고 비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="e1138-188">• 받기 및 조회를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="e1138-189">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="e1138-190">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-190">Business profile admin</span></span>   |<span data-ttu-id="e1138-191">•View를 만들고 비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="e1138-192">• 뷰를 만들고 파트너 서비스 요청 관리</span><span class="sxs-lookup"><span data-stu-id="e1138-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="e1138-193">인센티브 (AAD가 아닌 역할)를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="e1138-194">**역할**</span><span class="sxs-lookup"><span data-stu-id="e1138-194">**Role**</span></span> | <span data-ttu-id="e1138-195">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="e1138-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="e1138-196">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="e1138-196">Incentives admin</span></span>|<span data-ttu-id="e1138-197">• 시작 하 고 인센티브를 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="e1138-198">• 본 인센티브 프로그램의 모든 측면을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="e1138-199">• 볼 수 있으며 은행 및 세금 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="e1138-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="e1138-200">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="e1138-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e1138-201">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="e1138-201">• Access support</span></span>
||<span data-ttu-id="e1138-202">• 분쟁 인센티브 지불</span><span class="sxs-lookup"><span data-stu-id="e1138-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="e1138-203">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="e1138-203">Incentives user</span></span>|<span data-ttu-id="e1138-204">•는 인센티브 프로그램을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1138-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="e1138-205">• 볼 수 있으며 인센티브 클레임 시작</span><span class="sxs-lookup"><span data-stu-id="e1138-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="e1138-206">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="e1138-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e1138-207">• 보기 환불 및 co-op 수익</span><span class="sxs-lookup"><span data-stu-id="e1138-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e1138-208">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="e1138-208">• Access support</span></span>












