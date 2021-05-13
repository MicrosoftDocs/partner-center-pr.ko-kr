---
title: 신용 한도 적용
ms.topic: how-to
ms.date: 05/11/2021
description: 신용 한도 및 계산 방법에 대해 알아보세요. FAQ를 포함 합니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819215"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="c2ec4-104">신용 한도 적용 (CLE)</span><span class="sxs-lookup"><span data-stu-id="c2ec4-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="c2ec4-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="c2ec4-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c2ec4-106">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="c2ec4-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="c2ec4-107">신용 한도 및 작동 방식</span><span class="sxs-lookup"><span data-stu-id="c2ec4-107">Your credit limit and how it works</span></span>

<span data-ttu-id="c2ec4-108">신용 한도는 파트너 센터에서 제품이 나 구독을 구매 하는 데 사용할 수 있는 최대 금액 (미국 달러)입니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="c2ec4-109">신용 한도를 초과 하는 경우에는 충분 한 지불이 완료 될 때까지 새로운 구매를 수행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="c2ec4-110">기존 구독은 중단 없이 계속 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="c2ec4-111">크레딧 제한은 Azure 계획, Azure 예약, 소프트웨어, Marketplace, Azure 145 P, Office 및 Dynamics 제품의 제안에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="c2ec4-112">신용 한도는 갱신 및 진행 중인 소비에는 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="c2ec4-113">온 보 딩 기간 동안에는 테 넌 트 수준에서 신용 한도를 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="c2ec4-114">예측 수익, 구매 prowess 및 지불 기록을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="c2ec4-115">그런 다음, 다음 수식을 사용 하 여 사용 가능한 잔액을 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="c2ec4-116">**[크레딧 한도 – (수신 구매 + 미결 미지불 청구서 + 청구 되지 않은 요금-과잉 지불)]**</span><span class="sxs-lookup"><span data-stu-id="c2ec4-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="c2ec4-117">질문과 대답</span><span class="sxs-lookup"><span data-stu-id="c2ec4-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="c2ec4-118">내 크레딧 한도가 테 넌 트 또는 글로벌 수준에서 설정 되나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="c2ec4-119">테 넌 트 수준입니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-119">The tenant level.</span></span> <span data-ttu-id="c2ec4-120">예를 들어 미국, 캐나다 및 일본에서 작업 한다고 가정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="c2ec4-121">캐나다 테 넌 트가 신용 한도에 도달 하면 파트너 센터에서 구매 하려고 할 때 해당 테 넌 트가 알림을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="c2ec4-122">다른 테 넌 트는 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="c2ec4-123">내 신용 한도를 초과 하는 경우 모든 권한으로 기존 고객 및 구독 서비스를 계속 제공할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="c2ec4-124">예.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-124">Yes.</span></span> <span data-ttu-id="c2ec4-125">고객의 기존 구독은 중단 없이 계속 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="c2ec4-126">그러나 고객에 대 한 새 구독은 구매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="c2ec4-127">CLE는 직접 청구 파트너와 간접 공급자 모두에 적용 되나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="c2ec4-128">예, 둘 다에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="c2ec4-129">내 계정 복원에 대 한 지불을 제출한 후 추가 구독을 언제 구매할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="c2ec4-130">Microsoft에서 신용 확인 프로세스를 계속 하기 위한 모든 요구 사항을 받은 경우 지불의 24 시간 이내에 구매를 재개할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="c2ec4-131">내 크레딧 한도를 확인 하려면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-131">How can I check my credit limit?</span></span>

<span data-ttu-id="c2ec4-132">에 연락 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 하 여 신용 한도를 확인 하 고 최근 구매에 대 한 정보를 받으세요.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="c2ec4-133">크레딧 한도에 대해 분쟁 수가 있는 청구서를 하나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="c2ec4-134">예.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-134">Yes.</span></span> <span data-ttu-id="c2ec4-135">그러나 Microsoft에 문의 하 여 문제를 해결할 수 있습니다 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) .</span><span class="sxs-lookup"><span data-stu-id="c2ec4-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="c2ec4-136">에 기록 하는 경우 잠시 후에 다시 말 ucmwrcsp@microsoft.com 까 요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="c2ec4-137">24 시간 이내에 응답이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="c2ec4-138">Microsoft에서 파트너의 신용 한도를 설정 하는 데 사용 하는 기준은 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="c2ec4-139">예측 수익, 구매 prowess 및 지불 내역에 따라 신용 한도를 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="c2ec4-140">현재 신용 한도가 새 상거래 환경에 적용 되나요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="c2ec4-141">예.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-141">Yes.</span></span> <span data-ttu-id="c2ec4-142">신용 한도는 파트너 센터의 모든 CSP 프로그램 및 제품에 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="c2ec4-143">조직에서 신용 한도에 근접 한 경우 알림을 받는 사람은 누구 인가요?</span><span class="sxs-lookup"><span data-stu-id="c2ec4-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="c2ec4-144">조직의 재무 계좌 매입금 담당자가 알림을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c2ec4-145">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c2ec4-145">Next steps</span></span>

[<span data-ttu-id="c2ec4-146">청구 기본 사항</span><span class="sxs-lookup"><span data-stu-id="c2ec4-146">Billing basics</span></span>](./billing-basics.md)
