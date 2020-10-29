---
title: 직접 청구 파트너를 간접 재판매인으로 전환
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 프로그램 파트너가 파트너 센터를 사용 하 여 직접 청구 파트너에서 간접 재판매인으로 전환 하는 방법을 알아봅니다.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795868"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="5523e-103">CSP(클라우드 솔루션 공급자) 직접 청구 파트너에서 CSP 간접 재판매인으로 전환</span><span class="sxs-lookup"><span data-stu-id="5523e-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="5523e-104">**적용 대상:**</span><span class="sxs-lookup"><span data-stu-id="5523e-104">**Applies to:**</span></span>
- <span data-ttu-id="5523e-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="5523e-105">Partner Center</span></span>

<span data-ttu-id="5523e-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="5523e-106">**Appropriate roles**</span></span>

- <span data-ttu-id="5523e-107">모든 CSP 직접 청구 파트너</span><span class="sxs-lookup"><span data-stu-id="5523e-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="5523e-108">이 문서는 간접 대리점으로 전환 하기로 결정 한 직접 청구 파트너를 위한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="5523e-109">그러나 간접 재판매인으로 등록 하는 것을 명시적으로 결정 하지 않은 경우에도 CSP 직접 청구 파트너 프로그램의 새 [요구 사항을](direct-partner-new-requirements.md) 충족 하지 않는 직접 청구 파트너는 [직접 청구 기능을 제한할](restricted-direct-bill-capabilities.md)때 Microsoft에서 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="5523e-110">2021 년 1 월부터 새 수익 요구 사항이 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="5523e-111">직접 청구 파트너로 등록 된 파트너는 이전 12 개월 동안 파트너 전역 계정 수준에서 클라우드 솔루션 공급자 프로그램 수익의 USD $ 제한은 30만 개의 이상 트랜잭션을 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="5523e-112">기존 직접 청구 테 넌 트를 사용 하 여 간접 재판매인 프로그램에 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="5523e-113">시작하기</span><span class="sxs-lookup"><span data-stu-id="5523e-113">Get started</span></span>

1. <span data-ttu-id="5523e-114">파트너 센터의 파트너 프로필 및 MPN ID가 최신 상태 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="5523e-115">간접 재판매인으로 전환 하려는 직접 청구 테 넌 트의 전역 관리자로 파트너 센터에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="개요":::

3. <span data-ttu-id="5523e-117">등록 양식에서 파트너 세부 정보를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="지금 등록":::

4. <span data-ttu-id="5523e-119">지금 등록을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-119">Select Enroll now.</span></span> <span data-ttu-id="5523e-120">간접 재판매인 비즈니스는 직접 비즈니스에 사용 하는 것과 동일한 AAD 테 넌 트를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5523e-121">처음에는 12 월부터 12 월 까지의 파트너에 게이 새로운 전환 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="5523e-122">9 월에서 12 월 사이에 기념일을 사용할 수 없는 경우에는 해당 기능이 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="5523e-123">12 월 2018 일 이후 기념일 날짜가 있는 파트너는 나중에 파트너에 대해 기능을 사용할 수 있게 되 면 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="5523e-124">등록이 승인 되 면 파트너 센터에 다시 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5523e-125">승인은 일반적으로 즉각적 이지만 최대 5 영업일까지 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="5523e-126">승인 되 면 등록 양식에서 기본 연락처 아래에 지정한 전자 메일 주소로 알림을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="5523e-127">**설정**  >  **파트너 설정**  >  **파트너 프로필** > 프로그램 정보에서 등록 상태를 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="5523e-128">**개요** 페이지에 간접 재판매인 규약이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="5523e-129">**수락 및 계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-129">Select **Accept and continue** .</span></span> <span data-ttu-id="5523e-130">이 작업을 통해 간접 재판매인 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="5523e-131">간접 재판매인 규약을 수락한 경우 파트너 프로필은 직접 청구 및 간접 재판매인 **모두** 를 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="간접 재판매인 규약":::

> [!IMPORTANT]
> <span data-ttu-id="5523e-133">새 기능을 사용 하 여 간접 재판매인로 등록 한 후에는 직접 청구 전용 테 넌 트로 롤백할 수 있는 옵션이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="5523e-134">간접 재판매인으로 등록 하려면 먼저 비즈니스 요구 사항을 완전히 평가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="5523e-135">직접에서 간접 재판매인으로 전환 하는 동안</span><span class="sxs-lookup"><span data-stu-id="5523e-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="5523e-136">이 단계에서 청구 프로세스를 포함 하 여 직접 고객의 구독 요구 사항을 계속 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="5523e-137">간접 공급자에서 고객을 수락 하 고 간접 재판매인으로 작동할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="직접 청구 및 간접 재판매인 모두":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="5523e-139">간접 공급자 찾기</span><span class="sxs-lookup"><span data-stu-id="5523e-139">Find an indirect provider</span></span>

<span data-ttu-id="5523e-140">등록 후 간접 공급자에 대 한 링크가 왼쪽 탐색 창에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="5523e-141">간접 재판매인은 대금 청구를 처리 하 고, 고객을 위한 제품을 구매 하 고, 인프라를 지원할 수 있는 간접 공급자와의 관계를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="5523e-142">다양한 간접 공급자가 다양한 지원과 서비스를 제공하므로 간접 재판매인은 해당 지역의 공급자를 평가하여 요구 사항을 가장 잘 만족하는 공급자를 선정하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="5523e-143">일반적으로 대부분 공급자는 다음과 같은 일을 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-143">Generally, most providers will:</span></span>

- <span data-ttu-id="5523e-144">간접 재판매인에게 기술 지원 제공</span><span class="sxs-lookup"><span data-stu-id="5523e-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="5523e-145">제품 및 서비스 마케팅 지원</span><span class="sxs-lookup"><span data-stu-id="5523e-145">Help you market your products and services</span></span>
- <span data-ttu-id="5523e-146">금융 및 신용 사용 약관 관리</span><span class="sxs-lookup"><span data-stu-id="5523e-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="5523e-147">공식 [Microsoft 간접 공급자](https://partnercenter.microsoft.com/partner/find-a-provider)목록을 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="5523e-148">자세한 정보, [간접 공급자가 있는 파트너](indirect-reseller-tasks-in-partner-center.md) 읽기</span><span class="sxs-lookup"><span data-stu-id="5523e-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="5523e-149">간접 공급자의 파트너 관계 초대 수락</span><span class="sxs-lookup"><span data-stu-id="5523e-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="5523e-150">파트너와 협력 하는 간접 공급자를 찾았으면 파트너 센터에서 간접 공급자와 파트너 관계를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="5523e-151">선택한 간접 공급자는 파트너 센터의 초대로 이동 하는 파트너 관계 초대 링크를 전자 메일로 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="5523e-152">전역 관리자가 파트너 센터에 로그인 하 고 초대 링크를 따르는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="5523e-153">초대를 수락 하면 해당 공급자의 이름이 간접 공급자 목록에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="5523e-154">새 고객을 간접 재판매인으로 획득</span><span class="sxs-lookup"><span data-stu-id="5523e-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="5523e-155">사용자와 사용자의 간접 공급자는 모두 재판매인과 고객과의 관계를가지고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="5523e-156">이러한 재판매인 관계를 통해 고객의 구독과 서비스를 대신 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="5523e-157">기존 Azure AD 테 넌 트를 보유 한 새 고객을 확보 하기 위해 고객에 게 초대 하 여 사용자와 공급자 모두와 동시에 재판매인 관계를 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="5523e-158">간접 재판매인 초대를 만들려면:</span><span class="sxs-lookup"><span data-stu-id="5523e-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="5523e-159">파트너 센터 왼쪽 탐색에서 **간접 공급자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="5523e-160">**새 고객 초대** 를 선택하여 귀사 및 간접 공급자와 동시에 재판매인 관계를 맺도록 고객을 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="5523e-161">공급자는 고객에 게 대리점 관계가 있어야 하므로 고객이 새 구독을 구입 하거나 기존 구독에 새 라이선스를 추가 하려는 경우 고객을 대신 하 여 주문을 제출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="5523e-162">다음 페이지에서 초안 이메일 메시지를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="5523e-163">전자 메일로 초안 메시지를 열거나, 메시지를 클립보드에 복사 하 여 전자 메일에 붙여 넣을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="5523e-164">전자 메일의 텍스트를 편집 하 여 필요한 항목을 표시 하 고, 사용자의 계정 및 공급자 계정 모두에 직접 고객을 연결 하도록 개인 설정 된 링크를 포함 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="5523e-165">그런 후 **완료** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-165">Then select **Done** .</span></span>

5. <span data-ttu-id="5523e-166">고객이 귀사와 공급자를 공식 재판매인으로 승인하면 귀사에는 고객을 대신하여 고객의 구독, 라이선스 및 사용자를 관리할 관리자 권한이 부여되고 간접 공급자는 고객을 대신하여 주문을 제출할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="5523e-167">고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="5523e-168">직접 청구 파트너와 달리 간접 재판매인은 파트너 센터에서 새 고객을 위해 Azure AD 테 넌 트를 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="5523e-169">공급자는 테 넌 트를 만들고이 고객에 대 한 간접 재판매인으로 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="5523e-170">이렇게 하면 고객이 파트너 센터의 고객 목록에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="5523e-171">직접 청구 기능을 사용 하 여 간접 재판매인으로 얻은 고객에 대 한 구매를 만들 수는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="5523e-172">직접 청구 고객 및 간접 재판매인 고객 관리</span><span class="sxs-lookup"><span data-stu-id="5523e-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="5523e-173">직접 청구 고객 및 간접 재판매인 고객을 다르게 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="5523e-174">직접 청구 고객 (간접 재판매인으로 수행 하지 않는 작업)</span><span class="sxs-lookup"><span data-stu-id="5523e-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="5523e-175">제품에 대 한 주문 만들기</span><span class="sxs-lookup"><span data-stu-id="5523e-175">Create orders for products</span></span>
- <span data-ttu-id="5523e-176">Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="5523e-176">Manage Azure reservations</span></span>
- <span data-ttu-id="5523e-177">주문 기록 관리</span><span class="sxs-lookup"><span data-stu-id="5523e-177">Manage their order history</span></span>
- <span data-ttu-id="5523e-178">소프트웨어 구입</span><span class="sxs-lookup"><span data-stu-id="5523e-178">Purchase software</span></span>
- <span data-ttu-id="5523e-179">고객에 게 직접 청구</span><span class="sxs-lookup"><span data-stu-id="5523e-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="5523e-180">간접 재판매인 고객</span><span class="sxs-lookup"><span data-stu-id="5523e-180">Indirect reseller customers</span></span>

- <span data-ttu-id="5523e-181">고객을 위한 간접 공급자 주문 제품</span><span class="sxs-lookup"><span data-stu-id="5523e-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="5523e-182">고객의 라이선스 및 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="5523e-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="5523e-183">구독 갱신 처리</span><span class="sxs-lookup"><span data-stu-id="5523e-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="5523e-184">직접 청구 파트너로 구매한 고객을 확인 하려면</span><span class="sxs-lookup"><span data-stu-id="5523e-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="5523e-185">**고객** 선택</span><span class="sxs-lookup"><span data-stu-id="5523e-185">Select **Customers**</span></span>

2. <span data-ttu-id="5523e-186">세부 정보를 볼 고객 선택</span><span class="sxs-lookup"><span data-stu-id="5523e-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="5523e-187">이 고객이 직접 청구 파트너로 구매한 경우 제품을 **추가** 하거나 **볼** 수 있는 옵션이 표시 되 고 해당 구독이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="5523e-188">고객에 게 간접 대리점 관계가 있는 경우 해당 옵션을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="5523e-189">직접 청구 고객을 간접 공급자로 이동</span><span class="sxs-lookup"><span data-stu-id="5523e-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="5523e-190">간접 공급자는 대리점 관계에 도달할 때까지 기존 직접 청구 고객에 대 한 주문 또는 기존 구독 전송을 제출할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="5523e-191">간접 공급자와 기존 직접 청구 고객 간에 재판매인 관계를 설정 하려면 다음 방법 중 하나를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="5523e-192">대리점 관계 확장</span><span class="sxs-lookup"><span data-stu-id="5523e-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="5523e-193">간접 재판매인 초대를 고객에 게 보내기</span><span class="sxs-lookup"><span data-stu-id="5523e-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="5523e-194">[간접 전환 직접 전환 문서](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) 에서 단계별 프로세스에 대 한 자세한 개요를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="5523e-195">대리점 관계 확장</span><span class="sxs-lookup"><span data-stu-id="5523e-195">Reseller relationship extension</span></span>

<span data-ttu-id="5523e-196">대리점 관계 확장 기능을 사용 하 여 파트너 센터 대시보드를 사용 하 여 기존 직접 청구 고객 및 간접 공급자 간에 재판매인 관계를 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="5523e-197">기능을 사용 하기 전에 다음에 유의 하십시오.</span><span class="sxs-lookup"><span data-stu-id="5523e-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="5523e-198">이 기능은 간접 재판매인이 [간접 재판매인 등록](#get-started)을 완료 하는 것으로 전환 중인 직접 청구 파트너 에게만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="5523e-199">기존 직접 청구 고객 에게만이 기능을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="5523e-200">[간접 재판매인 고객](#acquire-new-customers-as-indirect-reseller)에 게는 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="5523e-201">[간접 공급자의 파트너 초대를 수락한](#accept-a-partnership-invitation-from-your-indirect-provider)간접 공급자만 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="5523e-202">이 고객에 대 한 청구 정보의 복사본은 간접 공급자가 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="5523e-203">파트너 센터 대시보드에서이 고객의 계정 페이지에 액세스 하 여 청구 정보에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5523e-204">재판매인 관계 확장 기능을 사용 하 여이 고객에 대 한 청구 정보를 간접 공급자와 공유 하는 데 동의 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="5523e-205">간접 공급자는 고객 테 넌 트에 [위임 된 관리 권한이](customers-revoke-admin-privileges.md) 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="5523e-206">간접 공급자에 게 위임 된 관리 권한이 필요한 경우 대신 간접 재판매인 초대를 고객에 게 보내야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="5523e-207">대리점 관계가 설정 되 면 간접 공급자는 [M365 관리 센터](https://admin.microsoft.com/AdminPortal/Home#/partners) 의 파트너 관계 페이지에서 고객에 게 CSP 파트너로 표시 되 고 [비즈니스에 대 한 Microsoft Store](/microsoft-store/work-with-partner-microsoft-store-business)됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="5523e-208">혼동 및 있다면 오해을 방지 하기 위해 관계 확장 기능을 사용 하 여 기존 다이렉트 청구서 고객과 간접 공급자 간의 재판매인 관계를 설정 하기 전에 파트너 계약에 따라 직접 청구 고객 으로부터 동의 하 고 동의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="5523e-209">기존 고객 테 넌 트에서이 기능을 사용 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="5523e-210">파트너 센터에 **관리 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="5523e-211">**고객 페이지** 에서 기존 고객을 선택 하 고 **빠른 링크** 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5523e-212">**간접 공급자** 에서 **간접 공급자에 대해 고객 전송** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="간접 공급자로 고객 전송":::

4. <span data-ttu-id="5523e-214">팝업 대화 상자에서 고객과의 대리점 관계를 설정할 **간접 공급자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="5523e-215">**저장 후 계속** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="5523e-216">선택한 간접 공급자가 **간접 공급자** 아래에 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="간접 공급자 나열":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="5523e-218">간접 재판매인 초대를 고객에 게 보내기</span><span class="sxs-lookup"><span data-stu-id="5523e-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="5523e-219">간접 공급자는 대리점 관계에 도달할 때까지 기존 직접 청구 고객에 대 한 주문을 제출할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="5523e-220">기존 고객과 간접 공급자 간의 재판매인 관계를 설정 하려면 간접 재판매인 초대를 사용 하 여 고객을 초대 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="5523e-221">파트너 센터 왼쪽 탐색에서 **간접 공급자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="5523e-222">**새 고객 초대** 를 선택하여 귀사 및 간접 공급자와 동시에 재판매인 관계를 맺도록 고객을 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="5523e-223">공급자는 고객에 게 대리점 관계가 있어야 하므로 고객이 새 구독을 구입 하거나 기존 구독에 새 라이선스를 추가 하려는 경우 고객을 대신 하 여 주문을 제출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="새 고객 초대":::

3. <span data-ttu-id="5523e-225">다음 페이지에서 초안 이메일 메시지를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="5523e-226">전자 메일로 초안 메시지를 열거나, 메시지를 클립보드에 복사 하 여 전자 메일에 붙여 넣을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="5523e-227">전자 메일의 텍스트를 편집 하 여 필요한 항목을 표시 하 고, 사용자의 계정 및 공급자 계정 모두에 직접 고객을 연결 하도록 개인 설정 된 링크를 포함 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="5523e-228">그런 후 **완료** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-228">Then select **Done** .</span></span>

5. <span data-ttu-id="5523e-229">고객이 귀사와 공급자를 공식 재판매인으로 승인하면 귀사에는 고객을 대신하여 고객의 구독, 라이선스 및 사용자를 관리할 관리자 권한이 부여되고 간접 공급자는 고객을 대신하여 주문을 제출할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="5523e-230">고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="5523e-231">Microsoft 고객 계약 승인</span><span class="sxs-lookup"><span data-stu-id="5523e-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="5523e-232">Microsoft 클라우드 계약은 2020 년 1 월 31 일까 지 유효 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="5523e-233">이 날짜 이후에는 모든 고객 (기존 및 신규)이 새 [Microsoft 고객 계약](confirm-customer-agreement.md)에 서명 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="5523e-234">고객을 전환 하는 경우에는 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="5523e-235">**고객이 Microsoft 고객 계약을 아직 수락 하지 않았습니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="5523e-236">간접 공급자와 협력 하 여 고객이 [Microsoft 고객 계약에 동의](confirm-customer-agreement.md)하도록 하세요.</span><span class="sxs-lookup"><span data-stu-id="5523e-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="5523e-237">**고객이 Microsoft 365 관리 센터를 통해 Microsoft 고객 계약에 동의 했습니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="5523e-238">이는 간접 공급자를 사용 하 여 재판매인 관계가 설정 된 후에 보존 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="5523e-239">수행 해야 할 작업이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="5523e-240">**고객이 파트너 증명을 통해 Microsoft 고객 계약에 동의 함**</span><span class="sxs-lookup"><span data-stu-id="5523e-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="5523e-241">수락은 유지 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-241">The acceptance will not be retained.</span></span> <span data-ttu-id="5523e-242">간접 공급자와 협력 하 여 [파트너 센터에서 고객의 동의를 업데이트](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)하세요.</span><span class="sxs-lookup"><span data-stu-id="5523e-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="5523e-243">간접 공급자에 게 기존 직접 청구 구독 이전</span><span class="sxs-lookup"><span data-stu-id="5523e-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="5523e-244">CSP 간접 모델에서 간접 대리점은 Microsoft와 청구 관계를 갖지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="5523e-245">대신 간접 대리점은 간접 공급자를 통해 고객에 대 한 구독을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="5523e-246">직접 청구 파트너에서 간접 재판매인으로 전환 하는 동안 직접 청구 파트너 인 기존 구독을 간접 공급자에 게 양도 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="5523e-247">파트너 센터 대시보드에서 자체 제공 되는 구독 전송 기능을 사용 하 여이 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="5523e-248">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="5523e-248">Pre-requisites</span></span>

- <span data-ttu-id="5523e-249">이 기능은 기존 직접 청구 파트너 테 넌 트를 사용 하 여 간접 재판매인 등록을 완료 한 파트너를 전환 하는 경우에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="5523e-250">지정 된 고객과 연결 된 구독을 전송 하기 전에 전환 파트너가 고객을 간접 공급자로 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="5523e-251">고객은 [간접 공급자를 통해 Microsoft 고객 계약에 동의](#microsoft-customer-agreement-acceptance)해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="5523e-252">간접 재판매인 상태로 전환 하는 방법</span><span class="sxs-lookup"><span data-stu-id="5523e-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="5523e-253">이 기능은 다음과 같은 4 단계 프로세스입니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="5523e-254">전환 파트너는 구독 전송 요청을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="5523e-255">이 요청에는 동일한 고객과 연결 된 기존 구독이 하나 이상 포함 되어 있으며 간접 공급자로 주소가 지정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="5523e-256">간접 공급자는 전송 요청을 검토 하 고 수락 (또는 거부) 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="5523e-257">간접 공급자는 전송 요청이 완료 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="5523e-258">전환 파트너가 전송 요청이 완료 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="5523e-259">파트너 전환</span><span class="sxs-lookup"><span data-stu-id="5523e-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="5523e-260">[파트너 센터 API/SDK](/partner-center/develop/manage-customers) 를 사용 하 여 기존 구독을 간접 공급자로 전송할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="5523e-261">고객의 구독 이전 자격 가져오기</span><span class="sxs-lookup"><span data-stu-id="5523e-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="5523e-262">고객의 이전 만들기</span><span class="sxs-lookup"><span data-stu-id="5523e-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="5523e-263">고객의 이전 철회</span><span class="sxs-lookup"><span data-stu-id="5523e-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="5523e-264">고객의 이전 수락</span><span class="sxs-lookup"><span data-stu-id="5523e-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="5523e-265">고객의 전송 거부</span><span class="sxs-lookup"><span data-stu-id="5523e-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="5523e-266">고객의 이전 가져오기</span><span class="sxs-lookup"><span data-stu-id="5523e-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="5523e-267">Id로 전송 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="5523e-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="5523e-268">파트너 전환-전송 요청 만들기</span><span class="sxs-lookup"><span data-stu-id="5523e-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="5523e-269">전환 파트너로 전송 요청을 만들려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="5523e-270">파트너 센터에 **관리 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="5523e-271">**고객** 페이지에서 원하는 고객을 선택 하 고 빠른 링크 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5523e-272">**간접 공급자** 에서 의도 한 간접 공급자가 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="5523e-273">**구독 보기** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="5523e-274">**구독** 페이지에서 **구독 이전** 을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="5523e-275">**구독 전송** 에서 **구독 전송 요청** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="구독 전송 요청":::

7. <span data-ttu-id="5523e-277">요청 전송 대화 상자에서 전송할 구독을 하나 이상 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="전송 요청 만들기":::

8. <span data-ttu-id="5523e-279">**만들기** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-279">Click **Create** .</span></span>

9. <span data-ttu-id="5523e-280">활성 구독 전송 요청은 **구독 이전** 에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="전송 요청 목록":::

10. <span data-ttu-id="5523e-282">사용자가 구독 전송 요청을 만들었음을 간접 공급자에 게 알립니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="5523e-283">간접 공급자-전송 요청 수락</span><span class="sxs-lookup"><span data-stu-id="5523e-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="5523e-284">간접 공급자로 전송 요청을 검토 하 고 수락 하려면:</span><span class="sxs-lookup"><span data-stu-id="5523e-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="5523e-285">파트너 센터에 **관리** 에이전트 또는 **영업 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="5523e-286">**고객 페이지에서** 원하는 고객을 선택 하 고 빠른 링크 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5523e-287">**간접 재판매인** 에서 전환 파트너가 나열 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="5523e-288">**구독 보기** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="5523e-289">**구독** 페이지에서 **구독 이전** 을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="전송 요청 보기":::

6. <span data-ttu-id="5523e-291">**구독 전송** 에서 검토할 전송 요청을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="5523e-292">적절 한 **수락** (또는 **거부** )을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="전송 요청 수락":::

8. <span data-ttu-id="5523e-294">전송 요청이 완료 될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="5523e-295">간접 공급자-전송 요청이 완료 되었는지 확인</span><span class="sxs-lookup"><span data-stu-id="5523e-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="5523e-296">전송 요청이 성공적으로 완료 되 면 구독이 **구독** 아래에 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="5523e-297">전환 파트너에 게 알립니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="5523e-298">파트너 전환-전송 요청 확인이 완료 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="5523e-299">전환 파트너는 다음을 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="5523e-300">파트너 센터에 **관리 에이전트** 또는 **영업 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="5523e-301">**고객** 페이지에서 원하는 고객을 선택 하 고 **빠른 링크** 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5523e-302">**구독 보기** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="5523e-303">**구독** 페이지에서 **구독 이전** 을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="5523e-304">전송 요청이 **완료** 로 표시 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="5523e-305">구독 페이지에서 구독이 더 이상 활성으로 표시 되지 않는지 **확인 합니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="5523e-306">Azure 구독 (MS MS-AZR-0017P-0145P) 인 경우 더 이상 나열 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="5523e-307">라이선스 기반 구독 (Office 365, Dynamics, Intune) 인 경우 **일시 중단** 됨 상태로 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="구독 일시 중단 됨":::

### <a name="considerations"></a><span data-ttu-id="5523e-309">고려 사항</span><span class="sxs-lookup"><span data-stu-id="5523e-309">Considerations</span></span>

- <span data-ttu-id="5523e-310">**전송 후에는 구독 ID가 다릅니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="5523e-311">Azure 구독 (MS-AZR-0017P-0145P) 인 경우에는 이전 소유자 로부터 유지 되 고 Azure 관리 포털에 표시 되는 Azure 구독 ID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="5523e-312">**여러 전송 요청에서 동일한 구독을 참조할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="5523e-313">기존 구독이 포함 된 전송 요청을 만든 후에는 첫 번째 전송 요청이 취소 될 때까지 동일한 구독을 포함 한 추가 전송 요청을 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="5523e-314">**라이선스 기반 구독의 추가 기능은 해당 기본 구독과 함께 전송 되어야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="5523e-315">전송 요청을 만들 때 하나 이상의 추가 기능이 있는 기존 구독을 선택 하면 해당 추가 기능이 전송 요청에 자동으로 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="5523e-316">**구독에 대 한 라이선스 수 변경 내용은 기존 전송 요청에 반영 되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="5523e-317">기존 구독이 포함 된 전송 요청을 만든 후에는 구독 (또는 연결 된 addons)의 라이선스 수량을 업데이트 하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="5523e-318">이렇게 하면 새 수량이 전송 요청에 반영 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="5523e-319">간접 공급자가 전송 요청을 수락 하면 결과 구독은 이전 수량을 갖게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="5523e-320">간접 공급자로 새 수량을 전송 하려는 경우 기존 전송 요청을 취소 하 고 새 전송 요청을 다시 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="5523e-321">**모든 구매는 자체 제공 구독 전송을 사용 하 여 전송할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="5523e-322">현재이 기능을 사용 하 여 O365 구독과 Azure PAYG subscription (MS-MS-AZR-0017P-0145P)만 전송할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="5523e-323">Azure Marketplace에 대 한 Azure 계획, Azure Reserved Instances, Term 기반 구독 및 SaaS 구독을 비롯 한 다른 구매는 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="5523e-324">전송 요청 제출 페이지에서 구독을 전송할 수 없는 이유가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="5523e-325">이러한 구독을 전송 하려면 [기존 구독을 취소](create-a-new-subscription.md#suspend-or-cancel-a-subscription) 하 고 간접 공급자를 통해 고객에 대 한 새 제품을 구매 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="5523e-326">**샌드박스 환경을 사용 하 여 테스트할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="5523e-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="5523e-327">간접 재판매인 성과급 등록</span><span class="sxs-lookup"><span data-stu-id="5523e-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="5523e-328">기존 직접 청구 파트너 테 넌 트에 간접 재판매인로 등록 한 후에는 30 일 이내에 간접 대리점에 등록 하 라는 초대를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="5523e-329">초대는 현재 CSP 파트너 테 넌 트와 연결 된 partner MPN 계정을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="5523e-330">초대가 partner MPN 계정과 연결 된 전자 메일 주소로 전송 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="5523e-331">또한 동일한 파트너 테 넌 트를 사용 하 여 직접 청구 동기 프로그램에 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="5523e-332">프로그램은 개별적으로 관리 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5523e-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5523e-333">다음 단계</span><span class="sxs-lookup"><span data-stu-id="5523e-333">Next steps</span></span>

- [<span data-ttu-id="5523e-334">간접 재판매인이 되기 위한 추가 정보</span><span class="sxs-lookup"><span data-stu-id="5523e-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="5523e-335">CSP 직접 파트너 새로운 요구 사항</span><span class="sxs-lookup"><span data-stu-id="5523e-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="5523e-336">제한된 직접 청구 기능</span><span class="sxs-lookup"><span data-stu-id="5523e-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)