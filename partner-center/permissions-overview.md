---
title: 사용자에게 역할 및 사용 권한 할당
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 상업 거래, 조회, 인센티브 또는 MPN 멤버십을 관리하는 회사 사용자에게 가장 적합한 역할에 대해 알아보세요.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565086"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="853e2-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="853e2-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="853e2-104">**적절한 역할**: 전역 관리자 | 사용자 관리 관리자 | MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-104">**Appropriate roles**: Global admin | User management admin | MPN partner admin</span></span>

<span data-ttu-id="853e2-105">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="853e2-106">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-106">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="853e2-107">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="853e2-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="853e2-108">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="853e2-109">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="853e2-110">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 전역 관리자 같은 표준 Azure AD(Azure Active Directory) 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-110">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory (Azure AD) tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="853e2-111">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="853e2-112">Azure AD 테넌트 역할에는 전역 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-112">Azure AD tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="853e2-113">비 Azure-AD 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN(Microsoft 파트너 네트워크) 파트너 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-113">Non-Azure-AD roles are those roles that do not manage the tenant, and they include MPN (Microsoft Partner Network) partner admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="853e2-114">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="853e2-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="853e2-115">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-115">**Role**</span></span>|<span data-ttu-id="853e2-116">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-116">**What they can do**</span></span>|<span data-ttu-id="853e2-117">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="853e2-117">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="853e2-118">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-118">Global admin</span></span>|<span data-ttu-id="853e2-119">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="853e2-119">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="853e2-120">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-120">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="853e2-121">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-121">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-122">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-122">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="853e2-123">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="853e2-124">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="853e2-125">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="853e2-126">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="853e2-126">User management admin</span></span>   | <span data-ttu-id="853e2-127">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-127">\*    View, create, and manage users</span></span>|[<span data-ttu-id="853e2-128">파트너 센터에서 Microsoft 파트너 네트워크 멤버십 혜택 및 제품 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-128">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="853e2-129">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="853e2-130">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-130">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-131">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-131">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="853e2-132">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-132">Billing admin</span></span> | <span data-ttu-id="853e2-133">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-133">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="853e2-134">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="853e2-134">Read your bill</span></span>](billing.md)
||<span data-ttu-id="853e2-135">\*    가격 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-135">\*    View pricing</span></span>
||<span data-ttu-id="853e2-136">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-137">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="853e2-138">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="853e2-138">Default user</span></span>|  <span data-ttu-id="853e2-139">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-139">View My profile</span></span>   |[<span data-ttu-id="853e2-140">암호 재설정</span><span class="sxs-lookup"><span data-stu-id="853e2-140">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="853e2-141">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="853e2-141">Admin agent</span></span> | <span data-ttu-id="853e2-142">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-142">\*    Customer management</span></span>|[<span data-ttu-id="853e2-143">고객과의 관계 구축</span><span class="sxs-lookup"><span data-stu-id="853e2-143">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="853e2-144">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="853e2-144">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="853e2-145">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="853e2-145">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="853e2-146">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-146">\*    Subscription management</span></span>
||<span data-ttu-id="853e2-147">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="853e2-147">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="853e2-148">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="853e2-148">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="853e2-149">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-149">\*    View pricing and offers</span></span>
||<span data-ttu-id="853e2-150">\*    청구</span><span class="sxs-lookup"><span data-stu-id="853e2-150">\*    Billing</span></span>
||<span data-ttu-id="853e2-151">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-151">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="853e2-152">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="853e2-152">\*    Register a value added reseller</span></span>
||<span data-ttu-id="853e2-153">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-153">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-154">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-154">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="853e2-155">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="853e2-155">Sales agent</span></span> | <span data-ttu-id="853e2-156">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-156">\*    Customer management</span></span>|[<span data-ttu-id="853e2-157">고객에 대한 청구 지원 제공 및 청구 질문에 대한 답변 지원</span><span class="sxs-lookup"><span data-stu-id="853e2-157">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="853e2-158">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="853e2-158">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="853e2-159">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-159">\*    Subscription management</span></span>
||<span data-ttu-id="853e2-160">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-160">\*    View support tickets</span></span>
||<span data-ttu-id="853e2-161">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="853e2-161">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="853e2-162">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-162">\*    View pricing and offers</span></span>
||<span data-ttu-id="853e2-163">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-163">\*    Manage customer leads</span></span>
||<span data-ttu-id="853e2-164">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-164">\*    View the customer agreement</span></span>
||<span data-ttu-id="853e2-165">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="853e2-165">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="853e2-166">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-166">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-167">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-167">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="853e2-168">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="853e2-168">Helpdesk agent</span></span>| <span data-ttu-id="853e2-169">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-169">\*    Search for and view a customer</span></span>|[<span data-ttu-id="853e2-170">Microsoft로 문제를 에스컬레이션하고 Microsoft 에스컬레이션에 더 적합한 문제 알아보기</span><span class="sxs-lookup"><span data-stu-id="853e2-170">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="853e2-171">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="853e2-171">\*    Edit customer details</span></span>
||<span data-ttu-id="853e2-172">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="853e2-172">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="853e2-173">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="853e2-173">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="853e2-174">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-174">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="853e2-175">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-175">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-176">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-176">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="853e2-177">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="853e2-177">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="853e2-178">(CSP 역할 및 비 Azure AD 역할)</span><span class="sxs-lookup"><span data-stu-id="853e2-178">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="853e2-179">CPV는 CSP 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-179">CPVs develop apps for use by CSP partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="853e2-180">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-180">**Role**</span></span>   |<span data-ttu-id="853e2-181">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-181">**What you can do**</span></span>|<span data-ttu-id="853e2-182">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="853e2-182">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="853e2-183">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-183">Global admin</span></span>| <span data-ttu-id="853e2-184">CPV(제어판 공급업체) 프로필 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-184">View and manage your Control Panel Vendor (CPV) profile</span></span>|[<span data-ttu-id="853e2-185">CSP 파트너 시스템을 파트너 센터 API와 통합하는 데 도움이 되도록 제어판 공급업체로 등록</span><span class="sxs-lookup"><span data-stu-id="853e2-185">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="853e2-186">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-186">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a><span data-ttu-id="853e2-187">게스트 사용자(Azure AD 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="853e2-187">Guest user (must be added to the Azure AD tenant)</span></span>

|<span data-ttu-id="853e2-188">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="853e2-188">**Guest user**</span></span>   | <span data-ttu-id="853e2-189">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-189">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="853e2-190">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-190">MPN partner admin</span></span>|
||<span data-ttu-id="853e2-191">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-191">Business profile admin</span></span>|
||<span data-ttu-id="853e2-192">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-192">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="853e2-193">MPN 멤버십 및 회사 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-193">Manage MPN membership and your company</span></span> 

<span data-ttu-id="853e2-194">이러한 역할은 Azure AD 역할이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-194">These roles are not Azure AD roles.</span></span> <span data-ttu-id="853e2-195">이러한 역할은 테넌트가 아니라 회사 비즈니스를 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-195">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="853e2-196">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-196">**Role**</span></span> | <span data-ttu-id="853e2-197">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-197">**What you can do**</span></span>|<span data-ttu-id="853e2-198">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="853e2-198">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="853e2-199">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-199">MPN partner admin</span></span>|<span data-ttu-id="853e2-200">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-200">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="853e2-201">Microsoft Action Pack 구독 또는 실버 및 골드 역량 구입 또는 갱신</span><span class="sxs-lookup"><span data-stu-id="853e2-201">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="853e2-202">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-202">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="853e2-203">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-203">\*    View user details and their skills data</span></span>
||<span data-ttu-id="853e2-204">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-204">\*    View competencies</span></span>
||<span data-ttu-id="853e2-205">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-205">\*    View and manage benefits</span></span>
||<span data-ttu-id="853e2-206">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="853e2-206">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="853e2-207">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-207">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="853e2-208">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-208">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="853e2-209">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="853e2-209">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="853e2-210">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-210">\*    View customer data analytics</span></span>
||<span data-ttu-id="853e2-211">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="853e2-211">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="853e2-212">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-212">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-213">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-213">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="853e2-214">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-214">Account admin</span></span>| <span data-ttu-id="853e2-215">위치 추가</span><span class="sxs-lookup"><span data-stu-id="853e2-215">Add locations</span></span>|[<span data-ttu-id="853e2-216">위치 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-216">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="853e2-217">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-217">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="853e2-218">\*    테넌트의 사용자에 대한 역할을 Azure-AD 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="853e2-218">\*    Assign roles for users in tenant to non-Azure-AD roles</span></span> 
||<span data-ttu-id="853e2-219">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="853e2-219">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="853e2-220">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-220">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-221">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-221">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="853e2-222">조회 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-222">Manage referrals</span></span>

|<span data-ttu-id="853e2-223">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-223">**Role**</span></span> | <span data-ttu-id="853e2-224">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-224">**What you can do**</span></span>|<span data-ttu-id="853e2-225">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="853e2-225">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="853e2-226">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-226">Referrals admin</span></span>|<span data-ttu-id="853e2-227">파트너 센터의 추천 탭에서 모든 항목 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-227">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="853e2-228">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-228">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="853e2-229">공동 판매 기회 및 잠재 고객을 모두 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-229">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="853e2-230">거래에 팀 멤버를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-230">Can assign team members for a deal</span></span>
||    <span data-ttu-id="853e2-231">비즈니스 프로필을 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-231">Can view and edit business profiles</span></span>
||    <span data-ttu-id="853e2-232">성사로 표시되고 거래 등록 자격이 있는 기회에 대한 거래를 보고 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-232">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="853e2-233">지원 티켓을 만들고 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-233">Can create and view support tickets</span></span>
|<span data-ttu-id="853e2-234">추천 사용자</span><span class="sxs-lookup"><span data-stu-id="853e2-234">Referrals user</span></span>|<span data-ttu-id="853e2-235">팀의 일부인 경우에만 공동 판매 기회 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-235">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="853e2-236">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-236">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="853e2-237">역할이 할당된 위치에 대한 공동 판매 기회를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-237">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="853e2-238">팀 멤버인 경우 성사로 표시되고 거래 등록 자격이 있는 기회에 대한 거래를 보고 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-238">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="853e2-239">지원 티켓을 만들고 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-239">Can create and view support tickets</span></span>
|<span data-ttu-id="853e2-240">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-240">Business profile admin</span></span>|<span data-ttu-id="853e2-241">비즈니스 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-241">Create and manage business profiles</span></span> | [<span data-ttu-id="853e2-242">비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-242">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="853e2-243">지원 티켓을 만들고 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-243">Can create and view support tickets</span></span>

<span data-ttu-id="853e2-244">새로운 추천 사용자 역할과 함께 거래의 위치 범위도 소개합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-244">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="853e2-245">아래 표는 위치에 따른 거래 액세스를 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-245">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="853e2-246">**범위**</span><span class="sxs-lookup"><span data-stu-id="853e2-246">**Scope**</span></span> | <span data-ttu-id="853e2-247">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-247">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="853e2-248">회사 전체</span><span class="sxs-lookup"><span data-stu-id="853e2-248">Entire company</span></span> | <span data-ttu-id="853e2-249">관리자와 사용자 모두 회사 내 모든 위치에 대한 거래를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-249">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="853e2-250">추천 관리자는 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-250">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="853e2-251">추천 사용자는 팀의 일부인 경우에만 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-251">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="853e2-252">하나 이상의 위치</span><span class="sxs-lookup"><span data-stu-id="853e2-252">One or more locations</span></span> | <span data-ttu-id="853e2-253">관리자와 사용자 모두 회사에 할당된 위치에 대한 거래를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-253">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="853e2-254">추천 관리자는 할당된 위치에 속하는 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-254">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="853e2-255">추천 사용자는 팀의 일부인 경우 할당된 위치에 속하는 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853e2-255">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="853e2-256">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-256">Manage incentives</span></span>

|<span data-ttu-id="853e2-257">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-257">**Role**</span></span> | <span data-ttu-id="853e2-258">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-258">**What you can do**</span></span>|<span data-ttu-id="853e2-259">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="853e2-259">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="853e2-260">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="853e2-260">Incentives admin</span></span>|<span data-ttu-id="853e2-261">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="853e2-261">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="853e2-262">인센티브를 시작하는 데 도움이 되도록 다음 리소스 사용</span><span class="sxs-lookup"><span data-stu-id="853e2-262">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="853e2-263">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="853e2-263">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="853e2-264">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="853e2-264">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="853e2-265">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-265">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="853e2-266">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="853e2-266">\*    Access support</span></span>
||<span data-ttu-id="853e2-267">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="853e2-267">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="853e2-268">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="853e2-268">Incentives user</span></span>|<span data-ttu-id="853e2-269">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="853e2-269">\*    Can view incentives programs</span></span>
||<span data-ttu-id="853e2-270">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="853e2-270">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="853e2-271">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-271">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="853e2-272">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="853e2-272">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="853e2-273">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-273">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="853e2-274">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-274">View Partner Center Insights data</span></span>

|<span data-ttu-id="853e2-275">**역할**</span><span class="sxs-lookup"><span data-stu-id="853e2-275">**Role**</span></span> | <span data-ttu-id="853e2-276">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="853e2-276">**What you can do**</span></span>|<span data-ttu-id="853e2-277">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="853e2-277">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="853e2-278">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="853e2-278">Executive report viewer</span></span>|<span data-ttu-id="853e2-279">모든 보고 데이터 세트에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-279">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="853e2-280">파트너 센터 인사이트에서 사용할 수 있는 개요 대시보드 보고서</span><span class="sxs-lookup"><span data-stu-id="853e2-280">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="853e2-281">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="853e2-281">Report viewer</span></span>|<span data-ttu-id="853e2-282">수익 및 고객과 직원 개인 데이터를 제외한 데이터 보고서에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="853e2-282">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="853e2-283">다음 단계</span><span class="sxs-lookup"><span data-stu-id="853e2-283">Next steps</span></span>

- [<span data-ttu-id="853e2-284">사용자 계정 만들기 및 역할과 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="853e2-284">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="853e2-285">새 파트너 센터 프로그램에 등록할 때 계정 정보 확인</span><span class="sxs-lookup"><span data-stu-id="853e2-285">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
