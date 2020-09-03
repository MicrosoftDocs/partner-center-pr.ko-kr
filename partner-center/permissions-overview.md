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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040769"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="c548e-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="c548e-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="c548e-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c548e-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-105">Global admin</span></span>
- <span data-ttu-id="c548e-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-106">User admin</span></span>
- <span data-ttu-id="c548e-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-107">MPN partner admin</span></span>

<span data-ttu-id="c548e-108">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c548e-109">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c548e-110">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="c548e-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c548e-111">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c548e-112">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c548e-113">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 글로벌 관리자 같은 표준 Azure AD 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c548e-114">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c548e-115">AAD(Azure Active Directory) 테넌트 역할에는 글로벌 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c548e-116">비 AAD 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c548e-117">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="c548e-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c548e-118">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-118">**Role**</span></span>|<span data-ttu-id="c548e-119">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="c548e-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="c548e-120">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-120">Global admin</span></span>|<span data-ttu-id="c548e-121">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="c548e-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="c548e-122">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-123">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="c548e-124">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c548e-125">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="c548e-126">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="c548e-127">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="c548e-127">User management admin</span></span>   | <span data-ttu-id="c548e-128">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="c548e-129">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="c548e-130">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="c548e-131">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-132">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="c548e-133">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-133">Billing admin</span></span> | <span data-ttu-id="c548e-134">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="c548e-135">\*    가격 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-135">\*    View pricing</span></span>
||<span data-ttu-id="c548e-136">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-137">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="c548e-138">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="c548e-138">Default user</span></span>|  <span data-ttu-id="c548e-139">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-139">View My profile</span></span>   |
|<span data-ttu-id="c548e-140">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="c548e-140">Admin agent</span></span> | <span data-ttu-id="c548e-141">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-141">\*    Customer management</span></span>
||<span data-ttu-id="c548e-142">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="c548e-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="c548e-143">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="c548e-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="c548e-144">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-144">\*    Subscription management</span></span>
||<span data-ttu-id="c548e-145">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="c548e-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="c548e-146">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="c548e-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="c548e-147">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="c548e-148">\*    청구</span><span class="sxs-lookup"><span data-stu-id="c548e-148">\*    Billing</span></span>
||<span data-ttu-id="c548e-149">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="c548e-150">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="c548e-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="c548e-151">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-152">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="c548e-153">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="c548e-153">Sales agent</span></span> | <span data-ttu-id="c548e-154">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-154">\*    Customer management</span></span>
||<span data-ttu-id="c548e-155">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="c548e-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="c548e-156">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-156">\*    Subscription management</span></span>
||<span data-ttu-id="c548e-157">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-157">\*    View support tickets</span></span>
||<span data-ttu-id="c548e-158">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="c548e-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="c548e-159">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="c548e-160">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="c548e-161">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="c548e-162">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="c548e-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="c548e-163">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-164">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="c548e-165">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="c548e-165">Helpdesk agent</span></span>| <span data-ttu-id="c548e-166">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="c548e-167">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="c548e-167">\*    Edit customer details</span></span>
||<span data-ttu-id="c548e-168">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="c548e-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c548e-169">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="c548e-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="c548e-170">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="c548e-171">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-172">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="c548e-173">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="c548e-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c548e-174">(CSP 역할 및 비 AAD 역할)</span><span class="sxs-lookup"><span data-stu-id="c548e-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="c548e-175">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c548e-176">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-176">**Role**</span></span>   |<span data-ttu-id="c548e-177">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="c548e-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="c548e-178">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-178">Global admin</span></span>| <span data-ttu-id="c548e-179">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="c548e-180">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="c548e-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="c548e-181">게스트 사용자(AAD 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="c548e-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="c548e-182">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="c548e-182">**Guest user**</span></span>   | <span data-ttu-id="c548e-183">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="c548e-184">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-184">MPN partner admin</span></span>|
||<span data-ttu-id="c548e-185">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-185">Accounts admin</span></span>|
||<span data-ttu-id="c548e-186">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-186">Incentives admin</span></span>|
||<span data-ttu-id="c548e-187">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-187">Business profile admin</span></span>|
||<span data-ttu-id="c548e-188">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="c548e-189">MPN 멤버 자격과 회사 관리(비 AAD 역할: 이 역할은 테넌트가 아닌 회사 비즈니스를 관리)</span><span class="sxs-lookup"><span data-stu-id="c548e-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="c548e-190">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-190">**Role**</span></span> | <span data-ttu-id="c548e-191">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="c548e-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="c548e-192">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-192">MPN partner admin</span></span>|<span data-ttu-id="c548e-193">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="c548e-194">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="c548e-195">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="c548e-196">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-196">\*    View competencies</span></span>
||<span data-ttu-id="c548e-197">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="c548e-198">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="c548e-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="c548e-199">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c548e-200">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="c548e-201">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="c548e-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c548e-202">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="c548e-203">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="c548e-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="c548e-204">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-205">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="c548e-206">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-206">Account admin</span></span>| <span data-ttu-id="c548e-207">위치 추가</span><span class="sxs-lookup"><span data-stu-id="c548e-207">Add locations</span></span>
|| <span data-ttu-id="c548e-208">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c548e-209">\*    테넌트의 사용자에 대한 역할을 비 AAD 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="c548e-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="c548e-210">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="c548e-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="c548e-211">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-212">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="c548e-213">조회 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-213">Manage referrals</span></span> 

|<span data-ttu-id="c548e-214">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-214">**Role**</span></span>|<span data-ttu-id="c548e-215">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="c548e-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="c548e-216">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-216">Referrals admin</span></span>       |<span data-ttu-id="c548e-217">\*    비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="c548e-218">\*    조회 받기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="c548e-219">\* 공동 판매 조회 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="c548e-220">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="c548e-221">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-221">Business profile admin</span></span>   |<span data-ttu-id="c548e-222">\* 비즈니스 프로필 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="c548e-223">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="c548e-224">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-225">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="c548e-226">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-226">Manage incentives</span></span> 

|<span data-ttu-id="c548e-227">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-227">**Role**</span></span> | <span data-ttu-id="c548e-228">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="c548e-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c548e-229">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="c548e-229">Incentives admin</span></span>|<span data-ttu-id="c548e-230">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="c548e-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="c548e-231">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="c548e-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c548e-232">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="c548e-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c548e-233">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="c548e-234">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="c548e-234">\*    Access support</span></span>
||<span data-ttu-id="c548e-235">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="c548e-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="c548e-236">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="c548e-236">Incentives user</span></span>|<span data-ttu-id="c548e-237">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="c548e-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="c548e-238">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="c548e-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c548e-239">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="c548e-240">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="c548e-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c548e-241">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="c548e-242">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="c548e-243">**역할**</span><span class="sxs-lookup"><span data-stu-id="c548e-243">**Role**</span></span> | <span data-ttu-id="c548e-244">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="c548e-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c548e-245">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="c548e-245">Executive report viewer</span></span>|<span data-ttu-id="c548e-246">모든 보고 데이터 세트에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="c548e-247">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="c548e-247">Report viewer</span></span>|<span data-ttu-id="c548e-248">수익 및 고객과 직원 개인 데이터를 제외한 데이터 보고서에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="c548e-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
