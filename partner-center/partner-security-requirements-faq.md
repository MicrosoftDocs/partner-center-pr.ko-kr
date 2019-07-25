---
title: 파트너 보안 요구 사항 FAQ | 파트너 센터
ms.topic: article
ms.date: 07/18/2019
description: 파트너 보안 요구 사항에 대 한 질문과 대답
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 클라우드 솔루션 공급자, 클라우드 솔루션 공급자 프로그램, CSP, 제어판 공급 업체, CPV, multi-factor authentication, MFA, 보안 응용 프로그램 모델, 보안 앱 모델, 보안
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315552"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a><span data-ttu-id="aac62-104">파트너 보안 요구 사항에 대 한 질문과 대답</span><span class="sxs-lookup"><span data-stu-id="aac62-104">Frequently asked questions about the partner security requirements</span></span>

<span data-ttu-id="aac62-105">이 문서에는 [파트너 보안 요구 사항](partner-security-requirements.md)에 대 한 몇 가지 질문과 대답이 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-105">This article contains some frequently asked questions for the [partner security requirements](partner-security-requirements.md).</span></span> <span data-ttu-id="aac62-106">[여기](http://assetsprod.microsoft.com/security-requirements-faq.pdf)에서 자주 묻는 질문의 포괄적인 목록을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-106">You can find a comprehensive list of frequently asked questions [here](http://assetsprod.microsoft.com/security-requirements-faq.pdf).</span></span>

## <a name="conditional-access"></a><span data-ttu-id="aac62-107">조건부 액세스</span><span class="sxs-lookup"><span data-stu-id="aac62-107">Conditional Access</span></span>

### <a name="can-conditional-access-be-used"></a><span data-ttu-id="aac62-108">조건부 액세스를 사용할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-108">Can conditional access be used?</span></span>

<span data-ttu-id="aac62-109">예, 조건부 액세스를 사용 하 여 파트너 테 넌 트에서 서비스 계정을 비롯 한 각 사용자에 대해 MFA를 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-109">Yes, you can use conditional access to enforce MFA for each user, including service accounts, in your partner tenant.</span></span> <span data-ttu-id="aac62-110">그러나 파트너의 매우 높은 권한이 있는 경우 각 사용자에 게 모든 단일 인증에 대 한 MFA 챌린지를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-110">However, given the highly privileged nature of being a partner we need to ensure that each user has an MFA challenge for every single authentication.</span></span> <span data-ttu-id="aac62-111">즉, MFA에 대 한 요구 사항을 회피 하는 조건부 액세스 기능을 활용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-111">This means you will not be able to leverage feature of conditional access that circumvent the requirement for MFA.</span></span>

## <a name="multi-factor-authentication"></a><span data-ttu-id="aac62-112">Multi-Factor Authentication</span><span class="sxs-lookup"><span data-stu-id="aac62-112">Multi-Factor Authentication</span></span>

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a><span data-ttu-id="aac62-113">고객은 파트너 보안 요구 사항을 적용 하나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-113">Are my customers subject to the partner security requirements?</span></span>

<span data-ttu-id="aac62-114">아니요, 고객의 Azure AD 테 넌 트의 각 사용자에 대해 MFA를 적용 해야 하는 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-114">No, it is not required that you enforce MFA for each user in your customer's Azure AD tenants.</span></span> <span data-ttu-id="aac62-115">그러나 각 고객을 사용 하 여 사용자를 보호 하는 최선의 방법을 결정 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-115">However, it is recommended that you work with each customer to determine how best to protect their users.</span></span>

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a><span data-ttu-id="aac62-116">앱 암호를 기준 보호 정책과 함께 사용할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-116">Can app passwords be used with the baseline protection policies?</span></span>

<span data-ttu-id="aac62-117">예, [앱 암호](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) 를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-117">Yes, [app passwords](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) can be used.</span></span> <span data-ttu-id="aac62-118">[여기](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) 에 설명 된 앱 암호 사용에 대 한 고려 사항을 검토 하 여 필요에 따라 지원 되는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-118">You should review the considerations for using app passwords documented [here](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) to determine if they are supported for your need.</span></span>

### <a name="can-any-user-be-excluded-from-this-requirement"></a><span data-ttu-id="aac62-119">이 요구 사항에서 사용자를 제외할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-119">Can any user be excluded from this requirement?</span></span> 

<span data-ttu-id="aac62-120">아니요. 파트너 테 넌 트에서 서비스 계정을 포함 한 각 사용자는 MFA를 사용 하 여 인증 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-120">No, each user, including service accounts, in your partner tenant will be required to authenticate using MFA.</span></span>

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a><span data-ttu-id="aac62-121">파트너 보안 요구 사항이 통합 샌드박스에 적용 되나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-121">Do the partner security requirements apply to the integration sandbox?</span></span>

<span data-ttu-id="aac62-122">예, 파트너 보안 요구 사항은 통합 샌드박스에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-122">Yes, the partner security requirements apply to the integration sandbox.</span></span> <span data-ttu-id="aac62-123">즉, integration sandbox 테 넌 트에서 사용자를 위한 적절 한 MFA 솔루션을 구현 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-123">This means you will need to implement the appropriate MFA solution for users in the integration sandbox tenant.</span></span> <span data-ttu-id="aac62-124">MFA를 제공 하는 기본 보호 정책을 구현 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-124">It is recommended that you implement the baseline protection policies to provide MFA.</span></span>

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a><span data-ttu-id="aac62-125">응급 액세스 (브레이크 유리) 계정을 구성 어떻게 할까요??</span><span class="sxs-lookup"><span data-stu-id="aac62-125">How do I configure an emergency access (break glass) account?</span></span>

<span data-ttu-id="aac62-126">Azure AD 테 넌 트에서 실수로 잠기는 것을 방지 하기 위해 하나 또는 두 개의 응급 액세스 계정을 만드는 것이 모범 사례로 간주 됩니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-126">It considered best practice to create one or two emergency access accounts to prevent being inadvertently locked out of your Azure AD tenant.</span></span> <span data-ttu-id="aac62-127">파트너 보안 요구 사항과 관련 하 여 각 사용자가 MFA를 사용 하 여 인증 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-127">With respect to the partner security requirements, it is required that each user authenticate using MFA.</span></span> <span data-ttu-id="aac62-128">따라서이는 응급 액세스 계정의 정의를 수정 해야 함을 의미 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-128">So, this means you will need to modify the definition of an emergency access account.</span></span> <span data-ttu-id="aac62-129">MFA에 타사 솔루션을 활용 하는 계정일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-129">It could be an account that is leveraging a third-party solution for MFA.</span></span>

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a><span data-ttu-id="aac62-130">게스트 사용자는 파트너 보안 요구 사항의 영향을 받는 방법</span><span class="sxs-lookup"><span data-stu-id="aac62-130">How will guest users be impacted by the partner security requirements?</span></span>

<span data-ttu-id="aac62-131">게스트 사용자는 파트너 테 넌 트의 리소스에 액세스할 때 MFA를 사용 하 여 인증 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-131">Guest users will be required to authenticate using MFA, when accessing resources in your partner tenant.</span></span> <span data-ttu-id="aac62-132">파트너 보안 요구 사항은 자체 테 넌 트의 리소스에 액세스 하는 게스트 사용자에 게 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-132">The partner security requirements will have no impact on the guest user will accessing resources in their own tenant.</span></span>

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a><span data-ttu-id="aac62-133">타사 솔루션을 사용 하는 경우 ADFS (Active Directory 페더레이션 서비스)가 필요 한가요?</span><span class="sxs-lookup"><span data-stu-id="aac62-133">If I am using a third-party solution is Active Directory Federation Service (ADFS) required?</span></span> 

<span data-ttu-id="aac62-134">아니요, 타사 솔루션을 사용 하는 경우에는 ADFS (Active Directory 페더레이션 서비스)를 사용할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-134">No, it is not required to have Active Directory Federation Service (ADFS) if you are using a third-party solution.</span></span> <span data-ttu-id="aac62-135">솔루션 공급 업체와 협력 하 여 솔루션에 대 한 요구 사항을 결정 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-135">It is recommended that you work with the vendor of the solution determine what the requirements for their solution are.</span></span>

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a><span data-ttu-id="aac62-136">기본 보호 정책을 사용 하도록 설정 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-136">Is it a requirement to enable the baseline protection policies?</span></span>

<span data-ttu-id="aac62-137">아니요, 기본 보호 정책을 사용 하도록 설정할 필요는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-137">No, it is not required that you enable the baseline protection policies.</span></span> <span data-ttu-id="aac62-138">유일한 요구 사항은 파트너 테 넌 트에서 서비스 계정을 포함 하 여 각 사용자에 대해 MFA를 적용 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-138">The only requirement is that you enforce MFA for each user, including service accounts, in your partner tenant.</span></span>

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a><span data-ttu-id="aac62-139">기준 보호 정책을 구현 하 여 제공 되는 확인 옵션은 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="aac62-139">What verification options are provided through the implementation of the baseline protection policies?</span></span> 

<span data-ttu-id="aac62-140">기본 보호 정책을 구현 하 여 사용할 수 있는 MFA 버전을 고려 하 여, 인증자 앱만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-140">With respect to the version of MFA that is available through the implementation of the baseline protection polices, the only verification option available is an authenticator app.</span></span> <span data-ttu-id="aac62-141">전화 통화 및 문자 메시지 메시지의 사용은 안전 하지 않은 것으로 간주 됩니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-141">The use of a phone call and text message message is considered less secure.</span></span> <span data-ttu-id="aac62-142">따라서 이러한 옵션은이 버전의 MFA를 통해 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-142">So, these options are not available through this version of MFA.</span></span>

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a><span data-ttu-id="aac62-143">에서 사용 하는 서비스 계정이 파트너 보안 요구 사항의 영향을 받을 Azure AD Connect 있나요?</span><span class="sxs-lookup"><span data-stu-id="aac62-143">Will the service account used by Azure AD Connect be impacted by the partner security requirements?</span></span>

<span data-ttu-id="aac62-144">아니요, Azure AD Connect에서 사용 하는 서비스 계정은 파트너 보안 요구 사항의 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="aac62-144">No, the service account used by Azure AD Connect will not be impacted by the partner security requirements.</span></span> <span data-ttu-id="aac62-145">MFA를 적용 한 결과로 Azure AD Connect에 문제가 발생 하는 경우 Microsoft 지원에 문의 하 여 기술 지원 요청을 여세요.</span><span class="sxs-lookup"><span data-stu-id="aac62-145">If you experience an issue with Azure AD Connect as result of enforcing MFA, then open a technical support request with Microsoft support.</span></span>
