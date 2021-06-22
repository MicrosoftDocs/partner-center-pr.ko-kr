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
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431760"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="e896c-104">계정 설정 또는 MPN 갱신 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e896c-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="e896c-105">**적절 한 역할**: 전역 관리자 | MPN 파트너 관리자</span><span class="sxs-lookup"><span data-stu-id="e896c-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="e896c-106">파트너 센터 계정을 설정할 때 발생 하는 일반적인 문제를 해결 하기 위한 몇 가지 제안 사항은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="e896c-107">파트너 구성원 센터에서 마이그레이션하는 경우에는 어떻게 되나요? 회사 정보 필드는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="e896c-108">회사에 파트너 센터 (예: CSP (클라우드 솔루션 공급자) 계정)가 이미 있는 경우에는 읽기 전용 화면이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="e896c-109">이 화면에는 파트너 센터에 존재 하는 회사에 대 한 모든 정보가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="e896c-110">이 화면에서는 세부 정보를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-110">You can't change the details on this screen.</span></span> <span data-ttu-id="e896c-111">이것은 의도적 이며 오류가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-111">This is by design and not an error.</span></span>

<span data-ttu-id="e896c-112">계속 하려면 **동의** 를 선택 하 고 **계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="e896c-113">IT 부서가 **파트너 센터 등록을 해제 한** 경우</span><span class="sxs-lookup"><span data-stu-id="e896c-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="e896c-114">바 이럴 사용자를 사용할 수 없거나 AD (Azure Active Directory) 테 넌 트에서 바 이럴 등록을 사용할 수 없기 때문에이 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="e896c-115">Azure AD 계정에 대 한 전역 관리자는 다음 PowerShell 명령을 실행 하 여 필요한 기능을 사용 하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="e896c-116">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="e896c-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="e896c-117">자세한 내용은 [셀프 서비스 등록](/azure/active-directory/users-groups-roles/directory-self-service-signup)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e896c-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="e896c-118">암호를 잊은 경우</span><span class="sxs-lookup"><span data-stu-id="e896c-118">You forgot your password</span></span>

<span data-ttu-id="e896c-119">암호를 잊은 경우 로그인 페이지에서 **계정에 액세스할 수 없습니까?** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="e896c-120">이 옵션을 사용 하면 암호를 재설정 하거나 전역 관리자에 게 새 자격 증명을 할당 하도록 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="e896c-121">"회사에 대해 알려주세요." 화면에서 "오류가 발생 했습니다." 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="e896c-122">회사 전화 번호에서 특수 문자, 공백 또는 국가 코드를 실수로 사용 하는 경우이 오류 메시지는 일반적으로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="e896c-123">전화 번호 필드에 입력 한 값은 최대 10 자만 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="e896c-124">신용 카드 구입 시 "주문이 거부 되었습니다." 라는 오류 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="e896c-125">정보를 확인 하세요. "</span><span class="sxs-lookup"><span data-stu-id="e896c-125">Please verify your information”</span></span>


<span data-ttu-id="e896c-126">항상 법적 엔터티가 아닌 신용 카드에 해당 하는 주소를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="e896c-127">또한 우편 번호가 올바르고 사용 하는 주소에 해당 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="e896c-128">오프 라인 결제에서 온라인 지불 방법으로 전환 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="e896c-129">원래 주문을 취소 하 고 기본 결제 방법을 사용 하 여 다시 구매 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="e896c-130">주문을 취소 하려면:</span><span class="sxs-lookup"><span data-stu-id="e896c-130">To cancel an order:</span></span>

1. <span data-ttu-id="e896c-131">파트너 센터 대시보드에서 **멤버 자격 제안** 탭을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="e896c-132">**취소 순서** 선택</span><span class="sxs-lookup"><span data-stu-id="e896c-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="e896c-133">확인 창이 표시 되 고 초기 주문을 취소 하기 위해 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e896c-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e896c-134">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e896c-134">Next steps</span></span>

- [<span data-ttu-id="e896c-135">파트너 센터 계정 관리</span><span class="sxs-lookup"><span data-stu-id="e896c-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="e896c-136">청구서 및 정찰 파일을 읽는 방법</span><span class="sxs-lookup"><span data-stu-id="e896c-136">How to read your bill and recon file</span></span>](read-your-bill.md)
