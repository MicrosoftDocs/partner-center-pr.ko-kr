---
title: 파트너 보안 요구 사항 구현
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 사용자에게 필요한 보안 요구 사항을 구현하는 방법 알아보기
author: LauraBrenner
ms.author: labrenne
keywords: 보안
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133272"
---
# <a name="implement-the-partner-security-requirements"></a><span data-ttu-id="726c9-104">파트너 보안 요구 사항 구현</span><span class="sxs-lookup"><span data-stu-id="726c9-104">Implement the partner security requirements</span></span>

<span data-ttu-id="726c9-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="726c9-105">**Appropriate roles**</span></span>

- <span data-ttu-id="726c9-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-106">Global admin</span></span>

<span data-ttu-id="726c9-107">고객과 파트너의 보안 및 프라이버시는 Microsoft의 최우선 순위입니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-107">Security and privacy of customers and partners are top priorities for Microsoft.</span></span> <span data-ttu-id="726c9-108">주로 ID 손상과 관련된 보안 공격이 더욱 정교해 지고 있으며 그 수도 증가하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-108">We continue to see an increasing number of more sophisticated security attacks, primarily related to compromised identities.</span></span> <span data-ttu-id="726c9-109">예방적 관리는 보안 공격을 방지하기 위한 전반적인 방어 전략에서 매우 중요한 역할을 하므로, Microsoft에서는 파트너 및 고객을 보호하기 위한 일련의 필수 보안 요구 사항을 적용하기 시작할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-109">As preventive controls play a key role in an overall defense strategy to thwart security attacks, we will start enforcing a set of mandatory security requirements to help protect partners and their customers.</span></span>

<span data-ttu-id="726c9-110">이 자습서에서는 파트너 보안 요구 사항, 요구 사항 이행 방법 및 파트너 디렉터리의 사용자에게 미치는 영향에 대해 자세히 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-110">Through this tutorial you will learn more about the partner security requirements, how to fulfill them, and the impact to users in your partner directory.</span></span>

<span data-ttu-id="726c9-111">클라우드 솔루션 공급자 프로그램에 참가하는 모든 파트너, 제어판 공급업체 및 Advisor 파트너는 파트너 테넌트의 각 사용자에게 MFA(Multi-Factor Authentication)를 적용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-111">All partners who are participating in the Cloud Solution Provider program, Control Panel Vendors, and Advisor partners are required to enforce Multi-Factor Authentication (MFA) for each user in their partner tenant.</span></span> <span data-ttu-id="726c9-112">이 적용 작업은 두 가지 [Azure Active Directory 기준 정책](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)을 사용하여 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-112">This enforcement can be done by enabling two [Azure Active Directory baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).</span></span> <span data-ttu-id="726c9-113">기준 정책은 여러 일반적인 공격으로부터 조직을 보호하는 데 도움이 되는 미리 정의된 정책 세트입니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-113">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="726c9-114">이러한 일반적인 공격은 암호 스프레이, 재생 및 피싱을 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-114">These common attacks can include password spray, replay, and phishing.</span></span> <span data-ttu-id="726c9-115">기준 정책은 모든 버전의 Azure Active Directory에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-115">Baseline policies are available in all editions of Azure Active Directory.</span></span> <span data-ttu-id="726c9-116">지난 몇 년 동안 ID 기반 공격이 증가해 왔기 때문에 Microsoft는 이러한 기준 보호 정책을 모든 사용자에게 제공하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-116">Microsoft is making these baseline protection policies available to everyone because identity-based attacks have been on the rise over the last few years.</span></span>

<span data-ttu-id="726c9-117">아래 절차는 두 가지 필수 기준 정책을 사용하도록 설정하는 프로세스를 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-117">The procedures below describe the process of enabling the two necessary baseline policies:</span></span>

- <span data-ttu-id="726c9-118">**관리자용 MFA 필요**  관리자용 MFA 필요 정책을 사용하도록 설정되면 관리자 역할의 사용자가 인증자 앱을 사용하여 MFA에 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-118">**Require MFA for admins**  Enabling the Require MFA for admins policy will require users in the administrator roles to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="726c9-119">MFA 등록이 완료되면 관리자가 로그인할 때마다 MFA를 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-119">Once MFA registration is complete, administrators will need to perform MFA every time they sign-in.</span></span>

- <span data-ttu-id="726c9-120">**최종 사용자 보호**  최종 사용자 보호는 디렉터리의 모든 사용자를 보호하는 위험 기반 MFA 기준 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-120">**End user protection**  End user protection is a risk-based MFA baseline policy that protects all users in a directory.</span></span> <span data-ttu-id="726c9-121">이 정책이 사용하도록 설정되면 모든 사용자가 인증자 앱을 사용하여 MFA에 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-121">Enabling this policy requires all users to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="726c9-122">사용자는 MFA 등록 프롬프트를 14일 동안 무시할 수 있으며 그 후에는 MFA에 등록하기 전까지 로그인이 차단됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-122">Users can ignore the MFA registration prompt for 14 days, after which they will be blocked from signing in until they register for MFA.</span></span> <span data-ttu-id="726c9-123">MFA에 등록된 사용자에게는 위험한 로그인 시도 중에만 MFA를 묻는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-123">Once registered for MFA, users will be prompted for MFA only during risky sign-in attempts.</span></span> <span data-ttu-id="726c9-124">손상된 사용자 계정은 해당 암호를 다시 설정하고 위험 이벤트를 해제할 때까지 차단됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-124">Compromised user accounts are blocked until their password is reset and risk events have been dismissed.</span></span>

<span data-ttu-id="726c9-125">이러한 정책을 사용하도록 설정되면 각 사용자는 추가 비용 없이 Azure MFA를 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-125">Once these policies are enabled, each user will be able to utilize Azure MFA at no additional cost.</span></span> <span data-ttu-id="726c9-126">타사 솔루션을 사용 중인 경우 Microsoft 상용 클라우드 서비스에 액세스할 때 각 사용자에게 MFA를 적용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-126">If you are using a third-party solution, then you are required to enforce MFA for each user when accessing Microsoft Commercial cloud services.</span></span>

>[!NOTE]
><span data-ttu-id="726c9-127">MFA는 파트너 디렉터리의 모든 사용자에게 적용되므로 사용자 자격 증명을 활용하는 모든 자동화 또는 통합에 영향을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-127">Since MFA will be enforced for every user in the partner directory, there will be an impact to any automation or integration that utilizes user credentials.</span></span> <span data-ttu-id="726c9-128">이러한 영향을 해결하려면 자동화 또는 통합을 Microsoft 상용 클라우드 서비스에 연결하는 방법을 수정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-128">To address this impact, you will need to modify the way your automation or integration connects to Microsoft commercial cloud services.</span></span> <span data-ttu-id="726c9-129">연결하는 서비스에서 토큰 기반 인증을 지원하는 경우 [보안 애플리케이션 모델 프레임워크](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)를 구현하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-129">If the service you are connecting to supports token-based authentication, then it is recommended that you implement the [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).</span></span>

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a><span data-ttu-id="726c9-130">1단계: 기존 레거시 인증 프로토콜 차단</span><span class="sxs-lookup"><span data-stu-id="726c9-130">Step one: Block any existing legacy authentication protocols</span></span>

<span data-ttu-id="726c9-131">관리자용 MFA 필요 및 최종 사용자 보호 정책을 사용하도록 설정하기 전에 사용자가 레거시 인증 프로토콜을 사용하고 있지 않은지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-131">Before you enable the Require MFA for admins and End user protection policies, ensure that your users are not using legacy authentication protocols.</span></span> <span data-ttu-id="726c9-132">자세한 내용은 [방법: 조건부 액세스를 사용하여 Azure AD에 대한 레거시 인증 차단](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="726c9-132">See the article [How to: Block legacy authentication to Azure AD with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) for more information.</span></span>

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a><span data-ttu-id="726c9-133">2단계: 관리자용 MFA 필요 기준 정책 사용</span><span class="sxs-lookup"><span data-stu-id="726c9-133">Step two: Enable the Require MFA for admins baseline policy</span></span>

<span data-ttu-id="726c9-134">관리자용 MFA 필요 기준 정책은 가장 높은 권한을 가진 Azure AD 역할로 간주되는 다음과 같은 디렉터리 역할에 MFA를 요구합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-134">The Require MFA for admin baseline policy requires MFA for the following directory roles, considered to be the most privileged Azure AD roles:</span></span>

- <span data-ttu-id="726c9-135">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-135">Global administrator</span></span>
- <span data-ttu-id="726c9-136">SharePoint 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-136">SharePoint administrator</span></span>
- <span data-ttu-id="726c9-137">Exchange 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-137">Exchange administrator</span></span>
- <span data-ttu-id="726c9-138">조건부 액세스 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-138">Conditional access administrator</span></span>
- <span data-ttu-id="726c9-139">보안 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-139">Security administrator</span></span>
- <span data-ttu-id="726c9-140">기술 지원팀 관리자/암호 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-140">Helpdesk administrator/Password administrator</span></span>
- <span data-ttu-id="726c9-141">대금 청구 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-141">Billing administrator</span></span>
- <span data-ttu-id="726c9-142">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="726c9-142">User administrator</span></span>

<span data-ttu-id="726c9-143">관리자용 MFA 필요 정책이 사용하도록 설정되면 위의 관리자 역할 9개가 인증자 앱을 사용하여 MFA에 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-143">Upon enabling the Require MFA for admins policy, the above nine administrator roles will be required to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="726c9-144">MFA 등록이 완료되면 관리자가 로그인할 때마다 MFA를 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-144">Once MFA registration is complete, administrators will need to perform MFA every single time they sign-in.</span></span>

<span data-ttu-id="726c9-145">조직에서 스크립트 또는 코드에 이러한 계정을 사용 중인 경우 이를  [관리 ID](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)로 바꾸는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-145">If your organization has these accounts in use in scripts or code, consider replacing them with [managed identities](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).</span></span>

<span data-ttu-id="726c9-146">이 정책을 사용하도록 설정하고 관리자를 보호하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-146">To enable this policy and protect your administrators:</span></span>

1. <span data-ttu-id="726c9-147">전역 관리자, 보안 관리자 또는 조건부 액세스 관리자로  **Azure Portal** 에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-147">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="726c9-148">**Azure Active Directory** > **조건부 액세스**로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-148">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="726c9-149">정책 목록에서 **기준 정책: 관리자용 MFA 필요**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-149">In the list of policies, select **Baseline policy: Require MFA for admins**.</span></span>

4. <span data-ttu-id="726c9-150">**정책 사용**을 **즉시 정책 사용**으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-150">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="726c9-151"> *\*저장*\*을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-151">Select **Save**.</span></span>

<span data-ttu-id="726c9-152">이러한 정책을 사용하도록 설정하면 위의 관리자 역할에 있는 사용자에게 추가 보안 정보를 제공하고 모바일 앱을 구성하기 위해 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-152">Once you’ve enabled this policy, users in the above administrator roles will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="726c9-153">이 작업이 완료되면 적절한 클라우드 서비스에 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-153">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a><span data-ttu-id="726c9-154">3단계: 최종 사용자 보호 기준 정책 사용</span><span class="sxs-lookup"><span data-stu-id="726c9-154">Step three: Enable the End user protection baseline policy</span></span>

<span data-ttu-id="726c9-155">최종 사용자 보호 기준 정책은 디렉터리의 모든 사용자를 보호합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-155">The End user protection baseline policy protects all users in a directory.</span></span> <span data-ttu-id="726c9-156">이 정책이 사용하도록 설정되면 모든 사용자가 14일 내에 Azure MFA에 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-156">Enabling this policy requires all users to register for Azure MFA within 14 days.</span></span> <span data-ttu-id="726c9-157">등록하면 위험한 로그인을 시도하는 동안에만 사용자에게 MFA를 요청하는 메시지가 표시되며, 이 동작은 나중에 파트너 테넌트에 적용되도록 변경될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-157">Once registered, users will be prompted for MFA only during risky sign-in attempts, this behavior will change for partner tenants in the future.</span></span> <span data-ttu-id="726c9-158">손상된 사용자 계정은 암호를 다시 설정하고 위험을 해제할 때까지 차단됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-158">Compromised user accounts are blocked until password reset and risk dismissal.</span></span>

<span data-ttu-id="726c9-159">기준 정책: 최종 사용자 보호 정책은 미리 구성된 상태로 제공되며 Azure Portal의 조건부 액세스 블레이드로 이동하면 위쪽에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-159">The policy Baseline policy: End user protection comes pre-configured and will show up at the top when you navigate to the Conditional Access blade in Azure portal.</span></span>

<span data-ttu-id="726c9-160">이 정책을 사용하도록 설정하고 사용자를 보호하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-160">To enable this policy and protect your users:</span></span>

1. <span data-ttu-id="726c9-161">전역 관리자, 보안 관리자 또는 조건부 액세스 관리자로  **Azure Portal** 에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-161">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="726c9-162">**Azure Active Directory** > **조건부 액세스**로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-162">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="726c9-163">정책 목록에서 **기준 정책: 최종 사용자 보호(미리 보기)** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-163">In the list of policies, select **Baseline policy: End user protection (preview)**.</span></span>

4. <span data-ttu-id="726c9-164">**정책 사용**을 **즉시 정책 사용**으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-164">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="726c9-165"> *\*저장*\*을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-165">Select **Save**.</span></span>

<span data-ttu-id="726c9-166">이러한 정책을 사용하도록 설정하면 모든 사용자에게 추가 보안 정보를 제공하고 모바일 앱을 구성하기 위해 로그인하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-166">Once you’ve enabled this policy, all users will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="726c9-167">이 작업이 완료되면 적절한 클라우드 서비스에 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-167">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

>[!NOTE]
><span data-ttu-id="726c9-168">파트너 보안 요구 사항이 적용되기 전에는, 관리자용 MFA 필요 기준 정책에 포함되지 않는 사용자에게 위험에 따라 MFA를 요청하는 메시지만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="726c9-168">Until the partner security requirements are enforced, users who are not covered by the Require MFA for admins baseline policy will only be prompted for MFA based on risk.</span></span>