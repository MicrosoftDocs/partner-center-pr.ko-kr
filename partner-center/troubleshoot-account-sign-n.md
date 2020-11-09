---
title: 파트너 센터 계정 설정 또는 MPN 갱신 문제 해결
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 파트너 센터에 등록 하려고 할 때 발생 하는 문제를 해결 합니다. 지불 방법, 잊어버린 암호 등을 사용 하 여 문제를 해결 합니다.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381412"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="20010-104">계정 설정 또는 MPN 갱신 문제 해결</span><span class="sxs-lookup"><span data-stu-id="20010-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="20010-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="20010-105">**Applies to**</span></span>

- <span data-ttu-id="20010-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="20010-106">Partner Center</span></span>
 
<span data-ttu-id="20010-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="20010-107">**Appropriate roles**</span></span>

- <span data-ttu-id="20010-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="20010-108">Global admin</span></span>
- <span data-ttu-id="20010-109">MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="20010-109">MPN partner admin</span></span> 
 
<span data-ttu-id="20010-110">파트너 센터 계정을 설정할 때 발생 하는 일반적인 문제를 해결 하기 위한 몇 가지 제안 사항은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="20010-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="20010-111">파트너 구성원 센터에서 마이그레이션하는 경우에는 어떻게 되나요? 회사 정보 필드는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="20010-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="20010-112">파트너가 파트너 센터에 이미 존재 하 고 있는 경우 (예를 들어 CSP 계정) 읽기 전용 화면이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="20010-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="20010-113">이 화면에는 파트너 센터에 존재 하는 회사에 대 한 모든 정보가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="20010-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="20010-114">이 화면에서는 세부 정보를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="20010-114">You can't change the details on this screen.</span></span> <span data-ttu-id="20010-115">이것은 의도적 이며 오류가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="20010-115">This is by design and not an error.</span></span>

<span data-ttu-id="20010-116">**수락** 을 선택 하 고 **계속** 진행 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="20010-117">IT 부서가 **파트너 센터 등록을 해제 한** 경우</span><span class="sxs-lookup"><span data-stu-id="20010-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="20010-118">바 이럴 사용자를 사용할 수 없거나 Azure AD 테 넌 트에서 바 이럴 등록을 사용할 수 없기 때문에이 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="20010-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="20010-119">Azure AD 계정에 대 한 전역 관리자는 다음 PowerShell 명령을 실행 하 여 필요한 기능을 사용 하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="20010-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="20010-120">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="20010-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="20010-121">자세한 내용은 [셀프 서비스 등록](/azure/active-directory/users-groups-roles/directory-self-service-signup) 을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="20010-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="20010-122">암호를 잊은 경우</span><span class="sxs-lookup"><span data-stu-id="20010-122">You forgot your password</span></span>

<span data-ttu-id="20010-123">암호를 잊은 경우 로그인 페이지에서 계정에 **액세스할 수 없습니까?** 링크를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="20010-124">이 옵션을 사용 하면 암호를 재설정 하거나 전역 관리자에 게 새 자격 증명을 할당 하도록 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="20010-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="20010-125">"회사에 대해 알려주세요." 화면에서 "오류가 발생 했습니다." 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="20010-125">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="20010-126">회사 전화 번호에서 특수 문자, 공백 또는 국가 코드를 실수로 사용 하는 경우이 오류 메시지는 일반적으로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="20010-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="20010-127">전화 번호 필드에 입력 한 값은 최대 10 자만 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="20010-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="20010-128">신용 카드 구입 시 "주문이 거부 되었습니다." 라는 오류 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="20010-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="20010-129">정보를 확인 하세요. "</span><span class="sxs-lookup"><span data-stu-id="20010-129">Please verify your information”</span></span>


<span data-ttu-id="20010-130">항상 법적 엔터티가 아닌 신용 카드에 해당 하는 주소를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="20010-131">또한 우편 번호가 올바르고 사용 하는 주소에 해당 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="20010-132">오프 라인 결제에서 온라인 지불 방법으로 전환 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="20010-133">원래 주문을 취소 하 고 기본 결제 방법을 사용 하 여 다시 구매 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="20010-134">주문을 취소 하려면:</span><span class="sxs-lookup"><span data-stu-id="20010-134">To cancel an order:</span></span>

1. <span data-ttu-id="20010-135">대시보드에서 **멤버 자격 제안** 탭을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="20010-136">**취소 순서** 선택</span><span class="sxs-lookup"><span data-stu-id="20010-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="20010-137">확인 창이 표시 되 고 초기 주문을 취소 하기 위해 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="20010-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20010-138">다음 단계</span><span class="sxs-lookup"><span data-stu-id="20010-138">Next steps</span></span>

- [<span data-ttu-id="20010-139">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="20010-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="20010-140">청구서 및 정찰 파일을 읽는 방법</span><span class="sxs-lookup"><span data-stu-id="20010-140">How to read your bill and recon file</span></span>](read-your-bill.md)
