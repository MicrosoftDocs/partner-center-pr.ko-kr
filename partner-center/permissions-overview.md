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
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 8ae4bed8536907c59f1b22e72896cfbe7f7aff9a
ms.sourcegitcommit: 445c7b70943f71cc4b2cb48a327b9dcc1814974d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "94670153"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="9d5ab-103">파트너 센터에서 작업해야 하는 회사 사용자에 대한 사용자 역할 및 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="9d5ab-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="9d5ab-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9d5ab-105">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-105">Global admin</span></span>
- <span data-ttu-id="9d5ab-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-106">User admin</span></span>
- <span data-ttu-id="9d5ab-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-107">MPN partner admin</span></span>

<span data-ttu-id="9d5ab-108">법적 이름과 주소, 지원 세부 정보, 면세 정보, 은행 정보, 회사의 기본 연락처를 비롯한 파트너 프로필을 설정했습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="9d5ab-109">다음 단계: 사용자가 파트너 센터에서 작업을 시작할 수 있도록 암호와 역할을 사용하여 사용자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="9d5ab-110">파트너 센터에서 작업할 수 있도록 직원 설정</span><span class="sxs-lookup"><span data-stu-id="9d5ab-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="9d5ab-111">사용자에게 부여할 파트너 센터에 대한 액세스 유형을 역할 및 권한을 기준으로 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="9d5ab-112">역할은 비즈니스가 개입된 프로그램과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="9d5ab-113">예를 들어 비즈니스가 CSP(클라우드 솔루션 공급자) 비즈니스인 경우 전역 관리자 같은 표준 Azure Active Directory 테넌트 관리 역할을 갖게 되겠지만, CSP 프로그램과 관련된 역할도 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="9d5ab-114">프로그램마다 특정 역할이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="9d5ab-115">Azure Active Directory 테넌트 역할에는 전역 관리자, 사용자 관리자 및 CSP 역할이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="9d5ab-116">비 Azure-Active-Directory 역할은 테넌트를 관리하지 않는 역할이며, 여기에는 MPN 관리자, 비즈니스 프로필 관리자, 조회 관리자, 인센티브 관리자 및 인센티브 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="9d5ab-117">파트너 센터에서 상업 트랜잭션 관리(Azure AD 및 CSP 역할)</span><span class="sxs-lookup"><span data-stu-id="9d5ab-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="9d5ab-118">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-118">**Role**</span></span>|<span data-ttu-id="9d5ab-119">**수행할 수 있는 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-119">**What they can do**</span></span>|<span data-ttu-id="9d5ab-120">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="9d5ab-121">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-121">Global admin</span></span>|<span data-ttu-id="9d5ab-122">\*    전체 권한으로 모든 Microsoft 계정/서비스에 액세스할 수 있음</span><span class="sxs-lookup"><span data-stu-id="9d5ab-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="9d5ab-123">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="9d5ab-124">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-125">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="9d5ab-126">\*    계약, 가격표 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="9d5ab-127">\*    파트너 사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="9d5ab-128">청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="9d5ab-129">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-129">User management admin</span></span>   | <span data-ttu-id="9d5ab-130">\*    사용자 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="9d5ab-131">파트너 센터에서 Microsoft 파트너 네트워크 멤버십 혜택 및 제품 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="9d5ab-132">\*    모든 파트너 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="9d5ab-133">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-134">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="9d5ab-135">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-135">Billing admin</span></span> | <span data-ttu-id="9d5ab-136">- 청구 정보, 청구서 및 조정 파일 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="9d5ab-137">청구서 읽기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="9d5ab-138">\*    가격 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-138">\*    View pricing</span></span>
||<span data-ttu-id="9d5ab-139">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-140">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="9d5ab-141">기본 사용자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-141">Default user</span></span>|  <span data-ttu-id="9d5ab-142">내 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-142">View My profile</span></span>   |[<span data-ttu-id="9d5ab-143">암호 재설정</span><span class="sxs-lookup"><span data-stu-id="9d5ab-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="9d5ab-144">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="9d5ab-144">Admin agent</span></span> | <span data-ttu-id="9d5ab-145">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-145">\*    Customer management</span></span>|[<span data-ttu-id="9d5ab-146">고객과의 관계 구축</span><span class="sxs-lookup"><span data-stu-id="9d5ab-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="9d5ab-147">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="9d5ab-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="9d5ab-148">\*    프로필을 만들고 디바이스에 적용</span><span class="sxs-lookup"><span data-stu-id="9d5ab-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="9d5ab-149">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-149">\*    Subscription management</span></span>
||<span data-ttu-id="9d5ab-150">\*    고객의 서비스 상태 및 서비스 요청</span><span class="sxs-lookup"><span data-stu-id="9d5ab-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="9d5ab-151">\*    위임된 관리자 권한 요청</span><span class="sxs-lookup"><span data-stu-id="9d5ab-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="9d5ab-152">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="9d5ab-153">\*    청구</span><span class="sxs-lookup"><span data-stu-id="9d5ab-153">\*    Billing</span></span>
||<span data-ttu-id="9d5ab-154">\*    고객을 대신하여 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="9d5ab-155">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="9d5ab-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="9d5ab-156">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-157">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="9d5ab-158">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="9d5ab-158">Sales agent</span></span> | <span data-ttu-id="9d5ab-159">\*    고객 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-159">\*    Customer management</span></span>|[<span data-ttu-id="9d5ab-160">고객에 대한 청구 지원 제공 및 청구 질문에 대한 답변 지원</span><span class="sxs-lookup"><span data-stu-id="9d5ab-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="9d5ab-161">\*    파트너 센터에 디바이스 목록 추가</span><span class="sxs-lookup"><span data-stu-id="9d5ab-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="9d5ab-162">\*    구독 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-162">\*    Subscription management</span></span>
||<span data-ttu-id="9d5ab-163">\*    지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-163">\*    View support tickets</span></span>
||<span data-ttu-id="9d5ab-164">\*    고객과의 관계 요청</span><span class="sxs-lookup"><span data-stu-id="9d5ab-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="9d5ab-165">\*    가격 책정 및 제품 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="9d5ab-166">\*    잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="9d5ab-167">\*    고객 계약 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="9d5ab-168">\*    부가 가치 재판매인 등록</span><span class="sxs-lookup"><span data-stu-id="9d5ab-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="9d5ab-169">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-170">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="9d5ab-171">기술 지원팀 상담원</span><span class="sxs-lookup"><span data-stu-id="9d5ab-171">Helpdesk agent</span></span>| <span data-ttu-id="9d5ab-172">\*    고객 검색 및 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="9d5ab-173">Microsoft로 문제를 에스컬레이션하고 Microsoft 에스컬레이션에 더 적합한 문제 알아보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="9d5ab-174">\*    고객 세부 정보 편집</span><span class="sxs-lookup"><span data-stu-id="9d5ab-174">\*    Edit customer details</span></span>
||<span data-ttu-id="9d5ab-175">\*    청구 또는 구독 관리와 관련된 고객 문제 해결 지원</span><span class="sxs-lookup"><span data-stu-id="9d5ab-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="9d5ab-176">\*    고객을 대신하여 지원 요청</span><span class="sxs-lookup"><span data-stu-id="9d5ab-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="9d5ab-177">\*    고객을 대신하여 구독 및 청구 이슈 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="9d5ab-178">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-179">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="9d5ab-180">CPV(제어판 공급업체).</span><span class="sxs-lookup"><span data-stu-id="9d5ab-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="9d5ab-181">(CSP 역할 및 비 Azure AD 역할)</span><span class="sxs-lookup"><span data-stu-id="9d5ab-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="9d5ab-182">CPV는 CSP(클라우드 솔루션 공급자) 파트너가 사용하는 앱을 개발하여 해당 시스템을 파트너 센터 API와 통합할 수 있게 해줍니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="9d5ab-183">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-183">**Role**</span></span>   |<span data-ttu-id="9d5ab-184">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-184">**What you can do**</span></span>|<span data-ttu-id="9d5ab-185">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="9d5ab-186">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-186">Global admin</span></span>| <span data-ttu-id="9d5ab-187">CPV 프로필을 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="9d5ab-188">CSP 파트너 시스템을 파트너 센터 API와 통합하는 데 도움이 되도록 제어판 공급업체로 등록</span><span class="sxs-lookup"><span data-stu-id="9d5ab-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="9d5ab-189">CPV 기능에 액세스해야 하는 사용자를 보고 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="9d5ab-190">게스트 사용자(Azure Active Directory 테넌트에 추가해야 함)</span><span class="sxs-lookup"><span data-stu-id="9d5ab-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="9d5ab-191">**게스트 사용자**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-191">**Guest user**</span></span>   | <span data-ttu-id="9d5ab-192">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="9d5ab-193">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-193">MPN partner admin</span></span>|
||<span data-ttu-id="9d5ab-194">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-194">Business profile admin</span></span>|
||<span data-ttu-id="9d5ab-195">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="9d5ab-196">MPN 멤버십 및 회사 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="9d5ab-197">이러한 역할은 Azure Active Directory 역할이 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="9d5ab-198">이러한 역할은 테넌트가 아니라 회사 비즈니스를 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="9d5ab-199">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-199">**Role**</span></span> | <span data-ttu-id="9d5ab-200">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-200">**What you can do**</span></span>|<span data-ttu-id="9d5ab-201">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="9d5ab-202">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-202">MPN partner admin</span></span>|<span data-ttu-id="9d5ab-203">\*    파트너 서비스 요청 보기, 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="9d5ab-204">Microsoft Action Pack 구독 또는 실버 및 골드 역량 구입 또는 갱신</span><span class="sxs-lookup"><span data-stu-id="9d5ab-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="9d5ab-205">\*    법률, 회사, 비즈니스 및 MPN 프로필 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="9d5ab-206">\*    사용자 정보 및 해당 기술 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="9d5ab-207">\*    역량 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-207">\*    View competencies</span></span>
||<span data-ttu-id="9d5ab-208">\*    혜택 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="9d5ab-209">\*    MPN 제품 보기 및 구매</span><span class="sxs-lookup"><span data-stu-id="9d5ab-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="9d5ab-210">\*    MPN 제품 주문 기록 및 청구서 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="9d5ab-211">\*    파트너 기여 지표 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="9d5ab-212">\*    바우처 유효성 검사 도구에서 작업 가능</span><span class="sxs-lookup"><span data-stu-id="9d5ab-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="9d5ab-213">\*    고객 데이터 분석 정보 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="9d5ab-214">\*    회사 내 다른 사용자 역할을 볼 수 있지만 역할을 할당할 수는 없음</span><span class="sxs-lookup"><span data-stu-id="9d5ab-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="9d5ab-215">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-216">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="9d5ab-217">계정 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-217">Account admin</span></span>| <span data-ttu-id="9d5ab-218">위치 추가</span><span class="sxs-lookup"><span data-stu-id="9d5ab-218">Add locations</span></span>|[<span data-ttu-id="9d5ab-219">위치 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="9d5ab-220">관리자로 있는 계정과 관련된 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="9d5ab-221">\*    테넌트의 사용자에 대한 역할을 비 Azure-Active-Directory 역할에 할당</span><span class="sxs-lookup"><span data-stu-id="9d5ab-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="9d5ab-222">\*    프로그램에 위치 등록</span><span class="sxs-lookup"><span data-stu-id="9d5ab-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="9d5ab-223">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-224">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-224">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="9d5ab-225">조회 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-225">Manage referrals</span></span>

> [!Note]
><span data-ttu-id="9d5ab-226">새로운 추천 사용자 역할은 2020년 11월 18일부터 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-226">The new Referrals user role will be available starting 18th November 2020.</span></span> <span data-ttu-id="9d5ab-227">기존 추천 관리자는 전체 회사로 범위가 지정된 추천 관리자 역할을 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-227">Existing referral admins will retain their referral admin role scoped to the entire company.</span></span>

|<span data-ttu-id="9d5ab-228">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-228">**Role**</span></span> | <span data-ttu-id="9d5ab-229">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-229">**What you can do**</span></span>|<span data-ttu-id="9d5ab-230">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-230">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="9d5ab-231">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-231">Referrals admin</span></span>|<span data-ttu-id="9d5ab-232">파트너 센터의 추천 탭에서 모든 항목 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-232">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="9d5ab-233">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-233">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="9d5ab-234">공동 판매 기회 및 잠재 고객을 모두 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-234">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="9d5ab-235">거래에 팀 멤버를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-235">Can assign team members for a deal</span></span>
||    <span data-ttu-id="9d5ab-236">비즈니스 프로필을 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-236">Can view and edit business profiles</span></span>
||    <span data-ttu-id="9d5ab-237">성사로 표시되고 거래 등록 자격이 있는 기회에 대한 거래를 보고 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-237">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="9d5ab-238">지원 티켓을 만들고 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-238">Can create and view support tickets</span></span>
|<span data-ttu-id="9d5ab-239">추천 사용자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-239">Referrals user</span></span>|<span data-ttu-id="9d5ab-240">팀의 일부인 경우에만 공동 판매 기회 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-240">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="9d5ab-241">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-241">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="9d5ab-242">역할이 할당된 위치에 대한 공동 판매 기회를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-242">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="9d5ab-243">팀 멤버인 경우 성사로 표시되고 거래 등록 자격이 있는 기회에 대한 거래를 보고 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-243">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="9d5ab-244">지원 티켓을 만들고 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-244">Can create and view support tickets</span></span>
|<span data-ttu-id="9d5ab-245">비즈니스 프로필 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-245">Business profile admin</span></span>|<span data-ttu-id="9d5ab-246">비즈니스 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-246">Create and manage business profiles</span></span> | [<span data-ttu-id="9d5ab-247">비즈니스 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-247">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="9d5ab-248">지원 티켓을 만들고 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-248">Can create and view support tickets</span></span>

<span data-ttu-id="9d5ab-249">새로운 추천 사용자 역할과 함께 거래의 위치 범위도 소개합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-249">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="9d5ab-250">아래 표는 위치에 따른 거래 액세스를 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-250">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="9d5ab-251">**범위**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-251">**Scope**</span></span> | <span data-ttu-id="9d5ab-252">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-252">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="9d5ab-253">회사 전체</span><span class="sxs-lookup"><span data-stu-id="9d5ab-253">Entire company</span></span> | <span data-ttu-id="9d5ab-254">관리자와 사용자 모두 회사 내 모든 위치에 대한 거래를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-254">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="9d5ab-255">추천 관리자는 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-255">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="9d5ab-256">추천 사용자는 팀의 일부인 경우에만 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-256">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="9d5ab-257">하나 이상의 위치</span><span class="sxs-lookup"><span data-stu-id="9d5ab-257">One or more locations</span></span> | <span data-ttu-id="9d5ab-258">관리자와 사용자 모두 회사에 할당된 위치에 대한 거래를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-258">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="9d5ab-259">추천 관리자는 할당된 위치에 속하는 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-259">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="9d5ab-260">추천 사용자는 팀의 일부인 경우 할당된 위치에 속하는 모든 거래를 보고 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d5ab-260">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="9d5ab-261">인센티브 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-261">Manage incentives</span></span>

|<span data-ttu-id="9d5ab-262">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-262">**Role**</span></span> | <span data-ttu-id="9d5ab-263">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-263">**What you can do**</span></span>|<span data-ttu-id="9d5ab-264">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-264">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="9d5ab-265">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-265">Incentives admin</span></span>|<span data-ttu-id="9d5ab-266">\*    인센티브 시작 및 관리</span><span class="sxs-lookup"><span data-stu-id="9d5ab-266">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="9d5ab-267">인센티브를 시작하는 데 도움이 되도록 다음 리소스 사용</span><span class="sxs-lookup"><span data-stu-id="9d5ab-267">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="9d5ab-268">\*    인센티브 프로그램의 모든 측면을 보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="9d5ab-268">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="9d5ab-269">\*    은행 및 세금 정보를 살펴보고 편집할 수 있음</span><span class="sxs-lookup"><span data-stu-id="9d5ab-269">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="9d5ab-270">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-270">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="9d5ab-271">\*    액세스 지원</span><span class="sxs-lookup"><span data-stu-id="9d5ab-271">\*    Access support</span></span>
||<span data-ttu-id="9d5ab-272">\*    분쟁 인센티브 결제</span><span class="sxs-lookup"><span data-stu-id="9d5ab-272">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="9d5ab-273">인센티브 사용자</span><span class="sxs-lookup"><span data-stu-id="9d5ab-273">Incentives user</span></span>|<span data-ttu-id="9d5ab-274">\*    인센티브 프로그램을 볼 수 있음</span><span class="sxs-lookup"><span data-stu-id="9d5ab-274">\*    Can view incentives programs</span></span>
||<span data-ttu-id="9d5ab-275">\*    인센티브 클레임을 보고 시작할 수 있음</span><span class="sxs-lookup"><span data-stu-id="9d5ab-275">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="9d5ab-276">\*    리베이트 및 협력 수익 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-276">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="9d5ab-277">\*    파트너 센터에 대한 지원 티켓 만들기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-277">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9d5ab-278">\*    내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-278">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="9d5ab-279">파트너 센터 인사이트 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-279">View Partner Center Insights data</span></span>

|<span data-ttu-id="9d5ab-280">**역할**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-280">**Role**</span></span> | <span data-ttu-id="9d5ab-281">**수행 가능한 작업**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-281">**What you can do**</span></span>|<span data-ttu-id="9d5ab-282">**자세히 알아보기**</span><span class="sxs-lookup"><span data-stu-id="9d5ab-282">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="9d5ab-283">임원 보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="9d5ab-283">Executive report viewer</span></span>|<span data-ttu-id="9d5ab-284">모든 보고 데이터 세트에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-284">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="9d5ab-285">파트너 센터 인사이트에서 사용할 수 있는 개요 대시보드 보고서</span><span class="sxs-lookup"><span data-stu-id="9d5ab-285">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="9d5ab-286">보고서 뷰어</span><span class="sxs-lookup"><span data-stu-id="9d5ab-286">Report viewer</span></span>|<span data-ttu-id="9d5ab-287">수익 및 고객과 직원 개인 데이터를 제외한 데이터 보고서에 액세스, 파트너 지원 티켓 만들기, 내가 만든 파트너 지원 티켓 보기</span><span class="sxs-lookup"><span data-stu-id="9d5ab-287">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="9d5ab-288">다음 단계</span><span class="sxs-lookup"><span data-stu-id="9d5ab-288">Next steps</span></span>

- [<span data-ttu-id="9d5ab-289">사용자 계정 만들기 및 역할과 사용 권한 할당</span><span class="sxs-lookup"><span data-stu-id="9d5ab-289">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="9d5ab-290">새 파트너 센터 프로그램에 등록할 때 계정 정보 확인</span><span class="sxs-lookup"><span data-stu-id="9d5ab-290">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
