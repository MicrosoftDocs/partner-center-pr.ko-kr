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
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839188"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="880d0-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="880d0-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="880d0-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="880d0-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-105">Global admin</span></span>
- <span data-ttu-id="880d0-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-106">User admin</span></span>
- <span data-ttu-id="880d0-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-107">MPN partner admin</span></span>

<span data-ttu-id="880d0-108">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="880d0-109">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="880d0-110">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="880d0-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="880d0-111">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="880d0-112">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="880d0-113">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 글로벌 관리자 같은 표준 Azure AD 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="880d0-114">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="880d0-115">AAD(Azure Active Directory) 테넌트 역할에는 글로벌 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="880d0-116">비 AAD 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="880d0-117">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="880d0-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="880d0-118">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-118">**Role**</span></span>|<span data-ttu-id="880d0-119">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="880d0-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="880d0-120">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-120">Global admin</span></span>|<span data-ttu-id="880d0-121">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="880d0-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="880d0-122">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="880d0-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="880d0-123">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="880d0-124">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="880d0-125">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="880d0-126">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="880d0-126">User management admin</span></span>   | <span data-ttu-id="880d0-127">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="880d0-128">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="880d0-129">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="880d0-130">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-130">Billing admin</span></span> | <span data-ttu-id="880d0-131">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="880d0-132">\*    가격 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-132">\*    View pricing</span></span>
|<span data-ttu-id="880d0-133">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="880d0-133">Default user</span></span>|  <span data-ttu-id="880d0-134">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-134">View My profile</span></span>   |
|<span data-ttu-id="880d0-135">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="880d0-135">Admin agent</span></span> | <span data-ttu-id="880d0-136">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-136">\*    Customer management</span></span>
||<span data-ttu-id="880d0-137">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="880d0-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="880d0-138">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="880d0-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="880d0-139">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-139">\*    Subscription management</span></span>
||<span data-ttu-id="880d0-140">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="880d0-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="880d0-141">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="880d0-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="880d0-142">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="880d0-143">\*    청구</span><span class="sxs-lookup"><span data-stu-id="880d0-143">\*    Billing</span></span>
||<span data-ttu-id="880d0-144">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="880d0-145">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="880d0-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="880d0-146">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="880d0-146">Sales agent</span></span> | <span data-ttu-id="880d0-147">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-147">\*    Customer management</span></span>
||<span data-ttu-id="880d0-148">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="880d0-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="880d0-149">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-149">\*    Subscription management</span></span>
||<span data-ttu-id="880d0-150">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-150">\*    View support tickets</span></span>
||<span data-ttu-id="880d0-151">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="880d0-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="880d0-152">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="880d0-153">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="880d0-154">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="880d0-155">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="880d0-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="880d0-156">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="880d0-156">Helpdesk agent</span></span>| <span data-ttu-id="880d0-157">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="880d0-158">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="880d0-158">\*    Edit customer details</span></span>
||<span data-ttu-id="880d0-159">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="880d0-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="880d0-160">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="880d0-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="880d0-161">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="880d0-162">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="880d0-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="880d0-163">(CSP 역할 및 비 AAD 역할)</span><span class="sxs-lookup"><span data-stu-id="880d0-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="880d0-164">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="880d0-165">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-165">**Role**</span></span>   |<span data-ttu-id="880d0-166">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="880d0-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="880d0-167">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-167">Global admin</span></span>| <span data-ttu-id="880d0-168">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="880d0-169">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="880d0-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="880d0-170">게스트 사용자(AAD 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="880d0-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="880d0-171">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="880d0-171">**Guest user**</span></span>   | <span data-ttu-id="880d0-172">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="880d0-173">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-173">MPN partner admin</span></span>|
||<span data-ttu-id="880d0-174">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-174">Accounts admin</span></span>|
||<span data-ttu-id="880d0-175">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-175">Incentives admin</span></span>|
||<span data-ttu-id="880d0-176">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-176">Business profile admin</span></span>|
||<span data-ttu-id="880d0-177">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="880d0-178">MPN 멤버 자격과 회사 관리(비 AAD 역할: 이 역할은 테넌트가 아닌 회사 비즈니스를 관리)</span><span class="sxs-lookup"><span data-stu-id="880d0-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="880d0-179">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-179">**Role**</span></span> | <span data-ttu-id="880d0-180">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="880d0-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="880d0-181">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-181">MPN partner admin</span></span>|<span data-ttu-id="880d0-182">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="880d0-183">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="880d0-184">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="880d0-185">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-185">\*    View competencies</span></span>
||<span data-ttu-id="880d0-186">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="880d0-187">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="880d0-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="880d0-188">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="880d0-189">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="880d0-190">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="880d0-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="880d0-191">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="880d0-192">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="880d0-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="880d0-193">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-193">Account admin</span></span>| <span data-ttu-id="880d0-194">위치 추가</span><span class="sxs-lookup"><span data-stu-id="880d0-194">Add locations</span></span>
|| <span data-ttu-id="880d0-195">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="880d0-196">\*    테넌트의 사용자에 대한 역할을 비 AAD 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="880d0-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="880d0-197">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="880d0-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="880d0-198">조회 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-198">Manage referrals</span></span> 

|<span data-ttu-id="880d0-199">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-199">**Role**</span></span>|<span data-ttu-id="880d0-200">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="880d0-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="880d0-201">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-201">Referrals admin</span></span>       |<span data-ttu-id="880d0-202">\*    비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="880d0-203">\*    조회 받기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="880d0-204">\* 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="880d0-205">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="880d0-206">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-206">Business profile admin</span></span>   |<span data-ttu-id="880d0-207">\* 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="880d0-208">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="880d0-209">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-209">Manage incentives</span></span> 

|<span data-ttu-id="880d0-210">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-210">**Role**</span></span> | <span data-ttu-id="880d0-211">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="880d0-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="880d0-212">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="880d0-212">Incentives admin</span></span>|<span data-ttu-id="880d0-213">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="880d0-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="880d0-214">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="880d0-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="880d0-215">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="880d0-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="880d0-216">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="880d0-217">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="880d0-217">\*    Access support</span></span>
||<span data-ttu-id="880d0-218">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="880d0-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="880d0-219">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="880d0-219">Incentives user</span></span>|<span data-ttu-id="880d0-220">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="880d0-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="880d0-221">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="880d0-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="880d0-222">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="880d0-223">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="880d0-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="880d0-224">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="880d0-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="880d0-225">**역할**</span><span class="sxs-lookup"><span data-stu-id="880d0-225">**Role**</span></span> | <span data-ttu-id="880d0-226">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="880d0-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="880d0-227">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="880d0-227">Executive report viewer</span></span>|<span data-ttu-id="880d0-228">모든 보고 데이터 세트에 액세스</span><span class="sxs-lookup"><span data-stu-id="880d0-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="880d0-229">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="880d0-229">Report viewer</span></span>|<span data-ttu-id="880d0-230">수익, 고객 및 직원 개인 데이터를 제외한 데이터 보고서에 액세스</span><span class="sxs-lookup"><span data-stu-id="880d0-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
