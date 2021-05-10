---
title: 파트너 센터 계정 설정 또는 MPN 갱신 문제 해결
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 파트너 센터 등록하려고 할 때의 문제를 해결합니다. 답변은 결제 방법, 암호 잊기 등의 문제를 해결합니다.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686265"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="53a58-104">계정 설정 또는 MPN 갱신 문제 해결</span><span class="sxs-lookup"><span data-stu-id="53a58-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="53a58-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="53a58-105">**Appropriate roles**</span></span>

- <span data-ttu-id="53a58-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="53a58-106">Global admin</span></span>
- <span data-ttu-id="53a58-107">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="53a58-107">MPN partner admin</span></span>
 
<span data-ttu-id="53a58-108">다음은 파트너 센터 계정을 설정하는 경우 발생하는 일반적인 문제를 해결하기 위한 몇 가지 제안 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="53a58-109">Partner Membership Center 마이그레이션하고 회사 정보 필드를 편집할 수 없는 경우 어떻게 되나요?</span><span class="sxs-lookup"><span data-stu-id="53a58-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="53a58-110">회사가 이미 파트너 센터 있는 경우(예: CSP 계정) 읽기 전용 화면이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="53a58-111">이 화면에는 회사에 대한 모든 정보가 파트너 센터 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="53a58-112">이 화면에서는 세부 정보를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-112">You can't change the details on this screen.</span></span> <span data-ttu-id="53a58-113">이는 오류가 아니라 의도적으로 한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-113">This is by design and not an error.</span></span>

<span data-ttu-id="53a58-114">**수락** 및 **계속을** 선택하여 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="53a58-115">IT 부서에서 **파트너 센터 등록을** 해제한 경우</span><span class="sxs-lookup"><span data-stu-id="53a58-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="53a58-116">바이럴 사용자가 비활성화되거나 Azure AD 테넌트에서 바이럴 등록이 비활성화되어 있으므로 이 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="53a58-117">Azure AD 계정의 전역 관리자는 다음 PowerShell 명령을 실행하여 필요한 기능을 사용하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="53a58-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="53a58-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="53a58-119">자세한 내용은 [셀프 서비스 등록을 읽어보십시오.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="53a58-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="53a58-120">암호를 잊어버렸습니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-120">You forgot your password</span></span>

<span data-ttu-id="53a58-121">암호를 잊어버린 경우 로그인 페이지에서 **계정에 액세스할 수 없나요?** 링크를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="53a58-122">이 옵션을 사용하면 암호를 재설정하거나 전역 관리자에게 새 자격 증명을 할당하도록 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="53a58-123">"회사에 대해 알려주세요" 화면에서 "문제가 발생했습니다." 오류가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="53a58-124">회사 전화 번호에서 특수 문자, 공백 또는 국가 코드를 실수로 사용 하는 경우이 오류 메시지는 일반적으로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="53a58-125">전화 번호 필드에 입력 한 값은 최대 10 자만 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="53a58-126">신용 카드 구입 시 "주문이 거부 되었습니다." 라는 오류 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="53a58-127">정보를 확인 하세요. "</span><span class="sxs-lookup"><span data-stu-id="53a58-127">Please verify your information”</span></span>


<span data-ttu-id="53a58-128">항상 법적 엔터티가 아닌 신용 카드에 해당 하는 주소를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="53a58-129">또한 우편 번호가 올바르고 사용 하는 주소에 해당 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="53a58-130">오프 라인 결제에서 온라인 지불 방법으로 전환 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="53a58-131">원래 주문을 취소 하 고 기본 결제 방법을 사용 하 여 다시 구매 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="53a58-132">주문을 취소 하려면:</span><span class="sxs-lookup"><span data-stu-id="53a58-132">To cancel an order:</span></span>

1. <span data-ttu-id="53a58-133">대시보드에서 **멤버 자격 제안** 탭을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="53a58-134">**취소 순서** 선택</span><span class="sxs-lookup"><span data-stu-id="53a58-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="53a58-135">확인 창이 표시 되 고 초기 주문을 취소 하기 위해 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a58-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="53a58-136">다음 단계</span><span class="sxs-lookup"><span data-stu-id="53a58-136">Next steps</span></span>

- [<span data-ttu-id="53a58-137">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="53a58-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="53a58-138">청구서 및 정찰 파일을 읽는 방법</span><span class="sxs-lookup"><span data-stu-id="53a58-138">How to read your bill and recon file</span></span>](read-your-bill.md)
