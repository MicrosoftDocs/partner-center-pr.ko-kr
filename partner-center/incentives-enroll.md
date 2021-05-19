---
title: 인센티브 등록
ms.topic: how-to
ms.date: 04/15/2021
description: 인센티브 프로그램에 등록하고 사용자 관리에 필요한 역할을 할당합니다. 이 문서에서는 등록 프로세스에 대해 설명합니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 670fae58a9a0e25127eb746f38063ea300d5ee2f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152089"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a><span data-ttu-id="29820-104">인센티브 프로그램의 등록 및 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="29820-104">Enrollment and user management in the incentives program</span></span>

<span data-ttu-id="29820-105">**적절한 역할:** 인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="29820-105">**Appropriate roles**: Incentives admin</span></span>

>[!NOTE]
><span data-ttu-id="29820-106">인센티브 프로그램에 등록하려면 [먼저 마이그레이션을](prepare-pmc-pc-migration.md)파트너 센터 Partner Membership Center 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-106">Before you can enroll in the incentives program you must have completed the Partner Membership Center to Partner Center [migration](prepare-pmc-pc-migration.md).</span></span>

<span data-ttu-id="29820-107">등록 프로세스는 두 단계로 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-107">The enrollment process consists of two steps.</span></span>

<span data-ttu-id="29820-108">**1단계. 사용자 관리:** 이 단계에서는 파트너 센터 인센티브 관리자를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-108">**Step 1. User management:** This step involves establishing the Incentive Administrator in Partner Center.</span></span>

<span data-ttu-id="29820-109">**2단계. 등록:** Microsoft에서 인센티브 프로그램에 등록하라는 초대를 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="29820-109">**Step 2. Enrollment:** Microsoft sends you an invitation to enroll in your incentive program.</span></span>

## <a name="user-management"></a><span data-ttu-id="29820-110">사용자 관리</span><span class="sxs-lookup"><span data-stu-id="29820-110">User Management</span></span>

<span data-ttu-id="29820-111">파트너 센터 인센티브 프로그램에 등록하려면 전역 관리자 또는 계정 관리자가 회사 사용자를 인센티브 관리자로 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-111">To enroll in a Partner Center incentive program, the Global administrator or Account administrator needs to set up your company users as Incentive administrators.</span></span> <span data-ttu-id="29820-112">파트너 계정, 역할 및 권한에 대한 자세한 내용은 [파트너 센터 계정 관리를 참조하세요.](partner-center-account-setup.md)</span><span class="sxs-lookup"><span data-stu-id="29820-112">For information on partner accounts, roles, and permissions, see [Manage your Partner Center account](partner-center-account-setup.md).</span></span> <span data-ttu-id="29820-113">전역 관리자 Azure AD(Azure Active Directory)를 통해 회사 사용자를 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-113">The Global administrator can also set up your company users through the Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="29820-114">인센티브 관리자만 인센티브 프로그램에 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-114">Only the Incentive administrator can enroll in incentive programs.</span></span> <span data-ttu-id="29820-115">해당 위치에 대한 인센티브 관리자가 없는 경우 전역 관리자 및 계정 관리자가 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-115">If there is no Incentive administrator for your location, the Global administrator and Account administrator must assign one.</span></span> <span data-ttu-id="29820-116">위치 MPN ID에 대한 인센티브 관리자를 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-116">The Incentive administrator must be assigned for the location MPN IDs.</span></span> <span data-ttu-id="29820-117">전역 관리자 또는 계정 관리자를 인센티브 관리자로 할당할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-117">The Global administrator or Account administrator can also be assigned as the Incentive administrator.</span></span> <span data-ttu-id="29820-118">다양한 역할에 대한 자세한 내용은 [인센티브 관리를 참조하세요.](permissions-overview.md#manage-incentives)</span><span class="sxs-lookup"><span data-stu-id="29820-118">To learn more about different roles, see [Manage incentives](permissions-overview.md#manage-incentives).</span></span>

## <a name="enrollment-process"></a><span data-ttu-id="29820-119">등록 프로세스</span><span class="sxs-lookup"><span data-stu-id="29820-119">Enrollment Process</span></span>

<span data-ttu-id="29820-120">조직이 인센티브에 적합한 경우 Microsoft는 적격 MPNLocationID의 인센티브 관리자에게 초대를 보내 등록 프로세스를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-120">Once your organization is eligible for incentives, Microsoft will send an invitation to the Incentive administrator of the eligible MPNLocationID to begin the enrollment process.</span></span> <span data-ttu-id="29820-121">이 전자 메일은 **Microsoft 파트너 센터** 전송되며 파트너 인센티브 등록 **초대를** 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-121">This email will be sent from **Microsoft Partner Center**, and will have the subject **Partner Incentive Enrollment Invitation**.</span></span> <span data-ttu-id="29820-122">초대를 열고 **시작** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-122">Open the invitation and select **Get Started**.</span></span>

<span data-ttu-id="29820-123">파트너 센터 홈페이지에 대 한 초대도 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-123">You’ll also see an invitation on the Partner Center home page.</span></span> <span data-ttu-id="29820-124">해당 메시지를 선택 하면 다시 볼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-124">Once you select that message, you won’t be able to see it again.</span></span> <span data-ttu-id="29820-125">그러나 동기 관리자는 [파트너 센터 대시보드](https://partner.microsoft.com/dashboard/) 에 로그인 하 고 왼쪽 탐색의 **성과급** 아래에서 **개요** 를 선택 하 여 프로세스를 완료할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-125">However, the Incentive Administrator can still complete the process by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) and selecting **Overview** under **Incentives** on the left nav.</span></span> <span data-ttu-id="29820-126">**등록** 을 선택 하 고 프로그램에 대 한 지급 및 세금 프로필을 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-126">Select **Enroll**, and then complete the payout and tax profile for the program.</span></span>

<span data-ttu-id="29820-127">MPN 위치에 대 한 기본 은행 프로필 설정이 이미 있고 동기 프로그램에서 동일한 MPN 위치를 등록 하려고 하는 경우 **등록** 을 선택 하 고 초대에 동의 하면 기본 은행 프로필이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-127">If you already have a default bank profile setup for an MPN location and you are trying to enroll for the same MPN location in an incentive program, when you select **Enroll** and accept the invitation, you will see the default bank profile.</span></span> <span data-ttu-id="29820-128">해당 MPN 위치에 대해 만든 경우 사용 가능한 세금 프로필도 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-128">You will also be shown any available tax profile if you've created it for that MPN location.</span></span> <span data-ttu-id="29820-129">Microsoft에 필요한 모든 은행 및 세금 프로필 정보가 있는 경우 **제출** 을 선택 하 여 등록을 완료 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-129">If Microsoft has all the required bank and tax profile detail, you'll be prompted to select **Submit** to complete the enrollment.</span></span> <span data-ttu-id="29820-130">[기본 은행 프로필 설정을](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="29820-130">See [Set up a default bank profile](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile).</span></span>

<span data-ttu-id="29820-131">또한 기본 은행 프로필 이외의 은행 프로필을 선택 하는 옵션도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-131">You also have the option to choose a bank profile other than the default bank profile.</span></span> <span data-ttu-id="29820-132">Microsoft에서 지불 또는 세금 프로필 또는 통화에 대 한 추가 세부 정보를 요구 하는 경우에도 **계속** 하 라는 메시지가 표시 되며 누락 된 세부 정보를 제공 하기 위해 **결제 및 세금 프로필** 페이지로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-132">If Microsoft requires additional details for the payment or tax profiles or currency, you will be prompted to **Continue** and will be redirected to the **Payment and Tax profile** page to provide the missing details.</span></span> 

<span data-ttu-id="29820-133">등록은 Microsoft에서 등록에 대해 제공한 지급 및 세금 프로필의 유효성을 검사 하는 경우에만 완료 된 것으로 간주 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-133">An enrollment is considered complete only when the payout and tax profile you provide for the enrollment is validated by Microsoft.</span></span>

<span data-ttu-id="29820-134">특정 동기 프로그램은 자격 조건이 없으며 모든 파트너에 게 공개 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-134">Certain incentive programs have no eligibility criteria, and are open to all partners.</span></span> <span data-ttu-id="29820-135">동기 관리자는 해당 프로그램에 대 한 초대를 제공 합니다 .이 페이지에는 관련 된 동기 프로그램 및 MPN에 대 한 권한이 있는 경우 동기 개요 페이지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-135">The Incentive administrator will see invitations for these programs on the incentive overview page, provided they have permissions for the relevant incentive program and MPN.</span></span> <span data-ttu-id="29820-136">Microsoft는 이러한 프로그램에 대 한 전자 메일 초대를 보내지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-136">Microsoft does not send email invitations for these programs.</span></span>

<span data-ttu-id="29820-137">등록 프로세스에 대 한 자세한 내용은 [성과급 등록 가이드](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (로그인 필요)를 다운로드 하세요.</span><span class="sxs-lookup"><span data-stu-id="29820-137">For more information on the enrollment process, download the [Incentives Enrollment Guide](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (sign-in required).</span></span>

## <a name="expiration-and-renewal"></a><span data-ttu-id="29820-138">만료 및 갱신</span><span class="sxs-lookup"><span data-stu-id="29820-138">Expiration and renewal</span></span>

<span data-ttu-id="29820-139">성과급 등록은 회계 연도가 종료 될 때 만료 됩니다.</span><span class="sxs-lookup"><span data-stu-id="29820-139">Incentives enrollment expires at the end of the fiscal year.</span></span> <span data-ttu-id="29820-140">그러나 활성 계약이 있는 적격 파트너를 유지 하는 한, Microsoft는 다음 회계 연도에 성과급 등록을 롤포워드 합니다.</span><span class="sxs-lookup"><span data-stu-id="29820-140">However, as long as you remain an eligible partner with an active agreement, Microsoft will roll forward your incentives enrollment into the next fiscal year.</span></span> <span data-ttu-id="29820-141">동기 프로그램에 필요한 지급 및 세금 정보가 동기 프로그램의 규칙에 따라 완료 되는 동안에는 어떤 조치도 취할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="29820-141">You don't need to take any action, as long as the payout and tax information required for the incentive program is complete as per the rules of the incentive program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="29820-142">다음 단계</span><span class="sxs-lookup"><span data-stu-id="29820-142">Next steps</span></span>

- [<span data-ttu-id="29820-143">프로그램 자격 확인</span><span class="sxs-lookup"><span data-stu-id="29820-143">Determine your program eligibility</span></span>](incentives-determined-your-program-eligibility.md)
- [<span data-ttu-id="29820-144">지급 및 세금 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="29820-144">Create and manage your payout and tax profiles</span></span>](incentives-create-and-manage-your-payout-and-tax-profiles.md)
