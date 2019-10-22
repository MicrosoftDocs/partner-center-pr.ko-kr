---
title: 사용자 역할 및 권한 할당 | 파트너 센터
ms.topic: article
ms.date: 10/10/2019
description: 파트너 센터에서 작업을 해야 하는 모든 직원에게 역할을 할당해야 합니다.
author: LauraBrenner
ms.author: labrenne
keywords: 역할, 권한, 관리자, 에이전트
ms.localizationpriority: high
ms.openlocfilehash: 0bbc9af84b8a1464f255c17147fdc10a7504eb43
ms.sourcegitcommit: 1ccc27092949deb6f6404e64fd6a628fd7b5fd5c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/11/2019
ms.locfileid: "72276094"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="1161e-104">사용자 역할 및 권한 할당</span><span class="sxs-lookup"><span data-stu-id="1161e-104">Assign users roles and permissions</span></span>


<span data-ttu-id="1161e-105">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="1161e-106">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="1161e-107">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="1161e-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="1161e-108">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="1161e-109">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="1161e-110">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 글로벌 관리자 같은 표준 Azure AD 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="1161e-111">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="1161e-112">AAD(Azure Active Directory) 테넌트 역할에는 글로벌 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="1161e-113">비 AAD 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="1161e-114">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="1161e-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="1161e-115">**역할**</span><span class="sxs-lookup"><span data-stu-id="1161e-115">**Role**</span></span>|<span data-ttu-id="1161e-116">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="1161e-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="1161e-117">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-117">Global admin</span></span>|<span data-ttu-id="1161e-118">• 전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="1161e-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="1161e-119">• 파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="1161e-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="1161e-120">• 계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="1161e-121">• 파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="1161e-122">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="1161e-123">사용자 관리 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-123">User management admin</span></span>   | <span data-ttu-id="1161e-124">• 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="1161e-125">• 모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-125">• View all partner profiles</span></span>
||<span data-ttu-id="1161e-126">• 파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="1161e-127">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-127">Billing admin</span></span> | <span data-ttu-id="1161e-128">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="1161e-129">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="1161e-129">Default user</span></span>|  <span data-ttu-id="1161e-130">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-130">View My profile</span></span>   |
|<span data-ttu-id="1161e-131">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="1161e-131">Admin agent</span></span> | <span data-ttu-id="1161e-132">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-132">•    Customer management</span></span>
||<span data-ttu-id="1161e-133">• 파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="1161e-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="1161e-134">• 프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="1161e-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="1161e-135">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-135">• Subscription management</span></span>
||<span data-ttu-id="1161e-136">• 고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="1161e-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="1161e-137">• 위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="1161e-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="1161e-138">• 가격 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-138">• View pricing and offers</span></span>
||<span data-ttu-id="1161e-139">• 청구</span><span class="sxs-lookup"><span data-stu-id="1161e-139">• Billing</span></span>
||<span data-ttu-id="1161e-140">• 고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="1161e-141">• 부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="1161e-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="1161e-142">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="1161e-142">Sales agent</span></span> | <span data-ttu-id="1161e-143">• 고객 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-143">•    Customer management</span></span>
||<span data-ttu-id="1161e-144">• 파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="1161e-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="1161e-145">• 구독 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-145">• Subscription management</span></span>
||<span data-ttu-id="1161e-146">• 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-146">• View support tickets</span></span>
||<span data-ttu-id="1161e-147">• 고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="1161e-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="1161e-148">• 잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-148">• Manage customer leads</span></span>
||<span data-ttu-id="1161e-149">• 고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-149">• View the customer agreement</span></span>
||<span data-ttu-id="1161e-150">• 부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="1161e-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="1161e-151">기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="1161e-151">Helpdesk agent</span></span>| <span data-ttu-id="1161e-152">• 고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="1161e-153">• 고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="1161e-153">• Edit customer details</span></span>
||<span data-ttu-id="1161e-154">• 청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="1161e-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="1161e-155">• 고객을 대신하여 지원 요청(참고: Office 365 구독에 대해 이 작업을 완료하려면 관리 에이전트여야 함)</span><span class="sxs-lookup"><span data-stu-id="1161e-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="1161e-156">• 고객을 대신하여 구독 및 청구 이슈 관리(참고: Office 365 구독에 대해 이 작업을 완료하려면 관리 에이전트여야 함)</span><span class="sxs-lookup"><span data-stu-id="1161e-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="1161e-157">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="1161e-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="1161e-158">(CSP 역할 및 비 AAD 역할)</span><span class="sxs-lookup"><span data-stu-id="1161e-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="1161e-159">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="1161e-160">**역할**</span><span class="sxs-lookup"><span data-stu-id="1161e-160">**Role**</span></span>   |<span data-ttu-id="1161e-161">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="1161e-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="1161e-162">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-162">Global admin</span></span>| <span data-ttu-id="1161e-163">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="1161e-164">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="1161e-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="1161e-165">게스트 사용자(AAD 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="1161e-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="1161e-166">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="1161e-166">**Guest user**</span></span>   | <span data-ttu-id="1161e-167">**역할**</span><span class="sxs-lookup"><span data-stu-id="1161e-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="1161e-168">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-168">MPN partner admin</span></span>|
||<span data-ttu-id="1161e-169">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-169">Accounts admin</span></span>|
||<span data-ttu-id="1161e-170">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-170">Incentives admin</span></span>|
||<span data-ttu-id="1161e-171">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-171">Business profile admin</span></span>|
||<span data-ttu-id="1161e-172">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="1161e-173">MPN 멤버 자격과 회사 관리(비 AAD 역할: 이 역할은 테넌트가 아닌 회사 비즈니스를 관리)</span><span class="sxs-lookup"><span data-stu-id="1161e-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="1161e-174">**역할**</span><span class="sxs-lookup"><span data-stu-id="1161e-174">**Role**</span></span> | <span data-ttu-id="1161e-175">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="1161e-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="1161e-176">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-176">MPN partner admin</span></span>|<span data-ttu-id="1161e-177">• 파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="1161e-178">• 법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="1161e-179">• 사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-179">• View user details and their skills data</span></span>
||<span data-ttu-id="1161e-180">• 역량 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-180">• View competencies</span></span>
||<span data-ttu-id="1161e-181">• 혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-181">• View and manage benefits</span></span>
||<span data-ttu-id="1161e-182">• MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="1161e-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="1161e-183">• MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="1161e-184">• 파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="1161e-185">• 바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="1161e-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="1161e-186">- 고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-186">- View customer data analytics</span></span>
|| <span data-ttu-id="1161e-187">회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="1161e-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="1161e-188">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-188">Account admin</span></span>| <span data-ttu-id="1161e-189">위치 추가</span><span class="sxs-lookup"><span data-stu-id="1161e-189">Add locations</span></span>
|| <span data-ttu-id="1161e-190">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="1161e-191">• 테넌트의 사용자에 대한 역할을 비 AAD 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="1161e-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="1161e-192">• 프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="1161e-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="1161e-193">조회 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-193">Manage referrals</span></span> 

|<span data-ttu-id="1161e-194">**역할**</span><span class="sxs-lookup"><span data-stu-id="1161e-194">**Role**</span></span>|<span data-ttu-id="1161e-195">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="1161e-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="1161e-196">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-196">Referrals admin</span></span>       |<span data-ttu-id="1161e-197">• 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="1161e-198">• 조회 받기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="1161e-199">• 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="1161e-200">• 파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="1161e-201">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-201">Business profile admin</span></span>   |<span data-ttu-id="1161e-202">• 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="1161e-203">• 파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="1161e-204">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-204">Manage incentives</span></span> 

|<span data-ttu-id="1161e-205">**역할**</span><span class="sxs-lookup"><span data-stu-id="1161e-205">**Role**</span></span> | <span data-ttu-id="1161e-206">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="1161e-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="1161e-207">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="1161e-207">Incentives admin</span></span>|<span data-ttu-id="1161e-208">• 인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="1161e-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="1161e-209">• 인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="1161e-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="1161e-210">• 은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="1161e-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="1161e-211">• 리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="1161e-212">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="1161e-212">• Access support</span></span>
||<span data-ttu-id="1161e-213">• 분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="1161e-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="1161e-214">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="1161e-214">Incentives user</span></span>|<span data-ttu-id="1161e-215">• 인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="1161e-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="1161e-216">• 인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="1161e-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="1161e-217">• 리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="1161e-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="1161e-218">• 액세스 지원</span><span class="sxs-lookup"><span data-stu-id="1161e-218">• Access support</span></span>












