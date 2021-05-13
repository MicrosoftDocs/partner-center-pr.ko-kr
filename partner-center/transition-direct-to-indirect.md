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
ms.openlocfilehash: e57ae5a30e3ee4331ae509a0650d09baf4a82590
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854896"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="73b29-103">CSP(클라우드 솔루션 공급자) 직접 청구 파트너에서 CSP 간접 재판매인으로 전환</span><span class="sxs-lookup"><span data-stu-id="73b29-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="73b29-104">**적절 한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="73b29-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="73b29-105">이 문서는 간접 대리점으로 전환 하기로 결정 한 직접 청구 파트너를 위한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="73b29-106">그러나 간접 재판매인으로 등록 하는 것을 명시적으로 결정 하지 않은 경우에도 CSP 직접 청구 파트너 프로그램의 새 [요구 사항을](direct-partner-new-requirements.md) 충족 하지 않는 직접 청구 파트너는 [직접 청구 기능을 제한할](restricted-direct-bill-capabilities.md)때 Microsoft에서 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="73b29-107">2021 년 1 월부터 새 수익 요구 사항이 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="73b29-108">직접 청구 파트너로 등록 된 파트너는 이전 12 개월 동안 파트너 전역 계정 수준에서 클라우드 솔루션 공급자 프로그램 수익의 USD $ 제한은 30만 개의 이상 트랜잭션을 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="73b29-109">기존 직접 청구 테 넌 트를 사용 하 여 간접 재판매인 프로그램에 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="73b29-110">시작하기</span><span class="sxs-lookup"><span data-stu-id="73b29-110">Get started</span></span>

1. <span data-ttu-id="73b29-111">파트너 센터의 파트너 프로필 및 MPN ID가 최신 상태 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="73b29-112">간접 재판매인으로 전환 하려는 직접 청구 테 넌 트의 전역 관리자로 파트너 센터에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="개요":::

3. <span data-ttu-id="73b29-114">등록 양식에서 파트너 세부 정보를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="지금 등록":::

4. <span data-ttu-id="73b29-116">지금 등록을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-116">Select Enroll now.</span></span> <span data-ttu-id="73b29-117">간접 재판매인 비즈니스는 직접 비즈니스에 사용 하는 것과 동일한 AAD 테 넌 트를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="73b29-118">처음에는 12 월부터 12 월 까지의 파트너에 게이 새로운 전환 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="73b29-119">9 월에서 12 월 사이에 기념일을 사용할 수 없는 경우에는 해당 기능이 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="73b29-120">12 월 2018 일 이후 기념일 날짜가 있는 파트너는 나중에 파트너에 대해 기능을 사용할 수 있게 되 면 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="73b29-121">등록이 승인 되 면 파트너 센터에 다시 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="73b29-122">승인은 일반적으로 즉각적 이지만 최대 5 영업일까지 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="73b29-123">승인 되 면 등록 양식에서 기본 연락처 아래에 지정한 전자 메일 주소로 알림을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="73b29-124">**설정**  >  **계정 설정**  >  **파트너 프로필** > 프로그램 정보에서 등록 상태를 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="73b29-125">**개요** 페이지에 간접 재판매인 규약이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="73b29-126">**수락 및 계속** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-126">Select **Accept and continue**.</span></span> <span data-ttu-id="73b29-127">이 작업을 통해 간접 재판매인 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="73b29-128">간접 재판매인 규약을 수락한 경우 파트너 프로필은 직접 청구 및 간접 재판매인 **모두** 를 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="간접 재판매인 규약":::

> [!IMPORTANT]
> <span data-ttu-id="73b29-130">새 기능을 사용 하 여 간접 재판매인로 등록 한 후에는 직접 청구 전용 테 넌 트로 롤백할 수 있는 옵션이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="73b29-131">간접 재판매인으로 등록 하려면 먼저 비즈니스 요구 사항을 완전히 평가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="73b29-132">직접에서 간접 재판매인으로 전환 하는 동안</span><span class="sxs-lookup"><span data-stu-id="73b29-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="73b29-133">이 단계에서 청구 프로세스를 포함 하 여 직접 고객의 구독 요구 사항을 계속 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="73b29-134">간접 공급자에서 고객을 수락 하 고 간접 재판매인으로 작동할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="직접 청구 및 간접 재판매인 모두":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="73b29-136">간접 공급자 찾기</span><span class="sxs-lookup"><span data-stu-id="73b29-136">Find an indirect provider</span></span>

<span data-ttu-id="73b29-137">등록 후 간접 공급자에 대 한 링크가 왼쪽 탐색 창에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="73b29-138">간접 재판매인은 대금 청구를 처리 하 고, 고객을 위한 제품을 구매 하 고, 인프라를 지원할 수 있는 간접 공급자와의 관계를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="73b29-139">다양한 간접 공급자가 다양한 지원과 서비스를 제공하므로 간접 재판매인은 해당 지역의 공급자를 평가하여 요구 사항을 가장 잘 만족하는 공급자를 선정하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="73b29-140">일반적으로 대부분 공급자는 다음과 같은 일을 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-140">Generally, most providers will:</span></span>

- <span data-ttu-id="73b29-141">간접 재판매인에게 기술 지원 제공</span><span class="sxs-lookup"><span data-stu-id="73b29-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="73b29-142">제품 및 서비스 마케팅 지원</span><span class="sxs-lookup"><span data-stu-id="73b29-142">Help you market your products and services</span></span>
- <span data-ttu-id="73b29-143">금융 및 신용 사용 약관 관리</span><span class="sxs-lookup"><span data-stu-id="73b29-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="73b29-144">공식 [Microsoft 간접 공급자](https://partnercenter.microsoft.com/partner/find-a-provider)목록을 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="73b29-145">자세한 정보, [간접 공급자가 있는 파트너](indirect-reseller-tasks-in-partner-center.md) 읽기</span><span class="sxs-lookup"><span data-stu-id="73b29-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="73b29-146">간접 공급자의 파트너 관계 초대 수락</span><span class="sxs-lookup"><span data-stu-id="73b29-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="73b29-147">파트너와 협력 하는 간접 공급자를 찾았으면 파트너 센터에서 간접 공급자와 파트너 관계를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="73b29-148">선택한 간접 공급자는 파트너 센터의 초대로 이동 하는 파트너 관계 초대 링크를 전자 메일로 보냅니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="73b29-149">전역 관리자가 파트너 센터에 로그인 하 고 초대 링크를 따르는지를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="73b29-150">초대를 수락 하면 해당 공급자의 이름이 간접 공급자 목록에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="73b29-151">새 고객을 간접 재판매인으로 획득</span><span class="sxs-lookup"><span data-stu-id="73b29-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="73b29-152">사용자와 사용자의 간접 공급자는 모두 재판매인과 고객과의 관계를가지고 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="73b29-153">이러한 재판매인 관계를 통해 고객의 구독과 서비스를 대신 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="73b29-154">기존 Azure AD 테 넌 트를 보유 한 새 고객을 확보 하기 위해 고객에 게 초대 하 여 사용자와 공급자 모두와 동시에 재판매인 관계를 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="73b29-155">간접 재판매인 초대를 만들려면:</span><span class="sxs-lookup"><span data-stu-id="73b29-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="73b29-156">파트너 센터 왼쪽 탐색에서 **간접 공급자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="73b29-157">**새 고객 초대** 를 선택하여 귀사 및 간접 공급자와 동시에 재판매인 관계를 맺도록 고객을 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="73b29-158">공급자는 고객에 게 대리점 관계가 있어야 하므로 고객이 새 구독을 구입 하거나 기존 구독에 새 라이선스를 추가 하려는 경우 고객을 대신 하 여 주문을 제출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="73b29-159">다음 페이지에서 임시 이메일 메시지를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="73b29-160">전자 메일로 초안 메시지를 열거나, 메시지를 클립보드에 복사 하 여 전자 메일에 붙여 넣을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="73b29-161">전자 메일의 텍스트를 편집 하 여 필요한 항목을 표시 하 고, 사용자의 계정 및 공급자 계정 모두에 직접 고객을 연결 하도록 개인 설정 된 링크를 포함 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="73b29-162">그런 후 **완료** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-162">Then select **Done**.</span></span>

5. <span data-ttu-id="73b29-163">고객이 귀사와 공급자를 공식 재판매인으로 승인하면 귀사에는 고객을 대신하여 고객의 구독, 라이선스 및 사용자를 관리할 관리자 권한이 부여되고 간접 공급자는 고객을 대신하여 주문을 제출할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="73b29-164">고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="73b29-165">직접 청구 파트너와 달리 간접 재판매인은 파트너 센터에서 새 고객을 위해 Azure AD 테 넌 트를 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="73b29-166">공급자는 테 넌 트를 만들고이 고객에 대 한 간접 재판매인으로 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="73b29-167">이렇게 하면 고객이 파트너 센터의 고객 목록에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="73b29-168">직접 청구 기능을 사용 하 여 간접 재판매인으로 얻은 고객에 대 한 구매를 만들 수는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="73b29-169">직접 청구 고객 및 간접 재판매인 고객 관리</span><span class="sxs-lookup"><span data-stu-id="73b29-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="73b29-170">직접 청구 고객 및 간접 재판매인 고객을 다르게 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="73b29-171">직접 청구 고객 (간접 재판매인으로 수행 하지 않는 작업)</span><span class="sxs-lookup"><span data-stu-id="73b29-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="73b29-172">제품에 대 한 주문 만들기</span><span class="sxs-lookup"><span data-stu-id="73b29-172">Create orders for products</span></span>
- <span data-ttu-id="73b29-173">Azure 예약 관리</span><span class="sxs-lookup"><span data-stu-id="73b29-173">Manage Azure reservations</span></span>
- <span data-ttu-id="73b29-174">주문 기록 관리</span><span class="sxs-lookup"><span data-stu-id="73b29-174">Manage their order history</span></span>
- <span data-ttu-id="73b29-175">소프트웨어 구매</span><span class="sxs-lookup"><span data-stu-id="73b29-175">Purchase software</span></span>
- <span data-ttu-id="73b29-176">고객에게 직접 청구</span><span class="sxs-lookup"><span data-stu-id="73b29-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="73b29-177">간접 대리점 고객</span><span class="sxs-lookup"><span data-stu-id="73b29-177">Indirect reseller customers</span></span>

- <span data-ttu-id="73b29-178">간접 공급자가 고객을 위해 제품을 주문합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="73b29-179">고객의 라이선스 및 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="73b29-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="73b29-180">구독 갱신 처리</span><span class="sxs-lookup"><span data-stu-id="73b29-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="73b29-181">직접 청구 파트너로 획득한 고객을 식별하려면</span><span class="sxs-lookup"><span data-stu-id="73b29-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="73b29-182">**고객** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-182">Select **Customers**.</span></span>

2. <span data-ttu-id="73b29-183">세부 정보를 볼 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="73b29-184">이 고객이 직접 청구 파트너로 획득한 고객인 경우 제품을 **추가하거나** **보는** 옵션이 표시되고 해당 구독이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="73b29-185">고객이 귀하와 간접 대리점 관계를 맺은 경우 해당 옵션을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="73b29-186">직접 청구 고객을 간접 공급자로 이동</span><span class="sxs-lookup"><span data-stu-id="73b29-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="73b29-187">간접 공급자는 기존 직접 청구 고객에 대한 주문 또는 기존 구독 양도를 대리점과 관계를 맺을 때까지 제출할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="73b29-188">간접 공급자와 기존 직접 청구 고객 간에 대리점 관계를 설정하려면 다음 방법 중 하나를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="73b29-189">Reseller 관계 확장</span><span class="sxs-lookup"><span data-stu-id="73b29-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="73b29-190">고객에게 간접 대리점 초대 보내기</span><span class="sxs-lookup"><span data-stu-id="73b29-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="73b29-191">[직접-간접 전환 문서에서](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/) 단계별 프로세스에 대한 자세한 개요를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="73b29-192">Reseller 관계 확장</span><span class="sxs-lookup"><span data-stu-id="73b29-192">Reseller relationship extension</span></span>

<span data-ttu-id="73b29-193">파트너 센터 대시보드를 사용하여 기존 직접 청구 고객과 간접 공급자 간에 대리점 관계를 설정하려면 대리점 관계 확장 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="73b29-194">이 기능을 사용하기 전에 다음을 참고하세요.</span><span class="sxs-lookup"><span data-stu-id="73b29-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="73b29-195">이 기능은 간접 대리점으로 전환하는 직접 청구 파트너가 간접 대리점 등록을 완료한 경우에만 사용할 수 [있습니다.](#get-started)</span><span class="sxs-lookup"><span data-stu-id="73b29-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="73b29-196">기존 직접 청구 고객 에게만이 기능을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="73b29-197">[간접 재판매인 고객](#acquire-new-customers-as-indirect-reseller)에 게는 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="73b29-198">[간접 공급자의 파트너 초대를 수락한](#accept-a-partnership-invitation-from-your-indirect-provider)간접 공급자만 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="73b29-199">이 고객에 대 한 청구 정보의 복사본은 간접 공급자가 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="73b29-200">파트너 센터 대시보드에서이 고객의 계정 페이지에 액세스 하 여 청구 정보에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="73b29-201">재판매인 관계 확장 기능을 사용 하 여이 고객에 대 한 청구 정보를 간접 공급자와 공유 하는 데 동의 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="73b29-202">간접 공급자는 고객 테 넌 트에 [위임 된 관리 권한이](customers-revoke-admin-privileges.md) 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="73b29-203">간접 공급자에 게 위임 된 관리 권한이 필요한 경우 대신 간접 재판매인 초대를 고객에 게 보내야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="73b29-204">대리점 관계가 설정 되 면 간접 공급자가 [Microsoft 365 관리 센터](https://admin.microsoft.com/AdminPortal/Home#/partners) 및 [Microsoft Store](/microsoft-store/work-with-partner-microsoft-store-business)의 파트너 관계 페이지에서 고객에 게 CSP 파트너로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="73b29-205">혼동 및 있다면 오해을 방지 하기 위해 관계 확장 기능을 사용 하 여 기존 다이렉트 청구서 고객과 간접 공급자 간의 재판매인 관계를 설정 하기 전에 파트너 계약에 따라 직접 청구 고객 으로부터 동의 하 고 동의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="73b29-206">기존 고객 테 넌 트에서이 기능을 사용 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="73b29-207">파트너 센터에 **관리 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="73b29-208">**고객 페이지** 에서 기존 고객을 선택 하 고 **빠른 링크** 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="73b29-209">**간접 공급자** 에서 **간접 공급자에 대해 고객 전송** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="간접 공급자로 고객 전송":::

4. <span data-ttu-id="73b29-211">팝업 대화 상자에서 고객과의 대리점 관계를 설정할 **간접 공급자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="73b29-212">**저장 후 계속** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="73b29-213">선택한 간접 공급자가 간접 공급자 아래에 **표시되는지 확인합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="간접 공급자 나열":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="73b29-215">고객에게 간접 대리점 초대 보내기</span><span class="sxs-lookup"><span data-stu-id="73b29-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="73b29-216">간접 공급자는 기존 직접 청구 고객과 대리점 관계를 맺을 때까지 주문을 제출할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="73b29-217">기존 고객과 간접 공급자 간에 대리점 관계를 설정하려면 간접 대리점 초대를 사용하여 고객을 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="73b29-218">파트너 센터 왼쪽 탐색에서 **간접 공급자를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="73b29-219">**새 고객 초대** 를 선택하여 귀사 및 간접 공급자와 동시에 재판매인 관계를 맺도록 고객을 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="73b29-220">공급자는 고객과 대리점 관계를 맺어야 하므로 고객이 새 구독을 구입하거나 기존 구독에 새 라이선스를 추가하려는 경우 고객을 대신하여 주문을 제출할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="새 고객 초대":::

3. <span data-ttu-id="73b29-222">다음 페이지에서 임시 이메일 메시지를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="73b29-223">전자 메일로 초안 메시지를 열거나 클립보드에 메시지를 복사하여 메일에 붙여넣을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="73b29-224">이메일의 텍스트를 편집하여 필요한 내용을 말하지만 고객을 계정과 공급자 계정 모두에 직접 연결하도록 개인 설정될 때 링크를 포함해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="73b29-225">그런 후 **완료** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-225">Then select **Done**.</span></span>

5. <span data-ttu-id="73b29-226">고객이 귀사와 공급자를 공식 재판매인으로 승인하면 귀사에는 고객을 대신하여 고객의 구독, 라이선스 및 사용자를 관리할 관리자 권한이 부여되고 간접 공급자는 고객을 대신하여 주문을 제출할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="73b29-227">고객의 계정, 서비스, 사용자 및 라이선스를 관리하려면 고객 이름 옆에 있는 아래쪽 화살표를 선택하여 고객의 기록을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="73b29-228">Microsoft 고객 계약 동의</span><span class="sxs-lookup"><span data-stu-id="73b29-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="73b29-229">Microsoft 클라우드 계약 2020년 1월 31일까지 유효합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="73b29-230">해당 날짜 이후에는 기존 및 신규 고객인 모든 고객이 새 [Microsoft 고객 계약](confirm-customer-agreement.md)서명해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="73b29-231">고객 전환의 경우 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="73b29-232">**고객이 아직 Microsoft 고객 계약 수락하지 않았습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="73b29-233">간접 공급자와 협력하여 고객이 [Microsoft 고객 계약 수락하도록](confirm-customer-agreement.md)하세요.</span><span class="sxs-lookup"><span data-stu-id="73b29-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="73b29-234">**고객이 Microsoft 365 관리 센터를 통해 사용자와 Microsoft 고객 계약 수락했습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="73b29-235">간접 공급자와 대리점 관계가 설정되면 동의가 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="73b29-236">수행할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="73b29-237">**고객이 파트너 증명을 통해 사용자와 Microsoft 고객 계약 수락했습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="73b29-238">수락은 유지 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-238">The acceptance will not be retained.</span></span> <span data-ttu-id="73b29-239">간접 공급자와 협력 하 여 [파트너 센터에서 고객의 동의를 업데이트](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)하세요.</span><span class="sxs-lookup"><span data-stu-id="73b29-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="73b29-240">간접 공급자에 게 기존 직접 청구 구독 이전</span><span class="sxs-lookup"><span data-stu-id="73b29-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="73b29-241">CSP 간접 모델에서 간접 대리점은 Microsoft와 청구 관계를 갖지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="73b29-242">대신 간접 대리점은 간접 공급자를 통해 고객에 대 한 구독을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="73b29-243">직접 청구 파트너에서 간접 재판매인으로 전환 하는 동안 직접 청구 파트너 인 기존 구독을 간접 공급자에 게 양도 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="73b29-244">파트너 센터 대시보드에서 자체 제공 되는 구독 전송 기능을 사용 하 여이 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="73b29-245">필수 조건</span><span class="sxs-lookup"><span data-stu-id="73b29-245">Prerequisites</span></span>

- <span data-ttu-id="73b29-246">이 기능은 기존 직접 청구 파트너 테 넌 트를 사용 하 여 간접 재판매인 등록을 완료 한 파트너를 전환 하는 경우에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="73b29-247">지정 된 고객과 연결 된 구독을 전송 하기 전에 전환 파트너가 고객을 간접 공급자로 이동 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="73b29-248">고객은 [간접 공급자를 통해 Microsoft 고객 계약에 동의](#microsoft-customer-agreement-acceptance)해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="73b29-249">간접 재판매인 상태로 전환 하는 방법</span><span class="sxs-lookup"><span data-stu-id="73b29-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="73b29-250">이 기능은 다음과 같은 4 단계 프로세스입니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="73b29-251">전환 파트너는 구독 전송 요청을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="73b29-252">이 요청에는 동일한 고객과 연결 된 기존 구독이 하나 이상 포함 되어 있으며 간접 공급자로 주소가 지정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="73b29-253">간접 공급자는 전송 요청을 검토 하 고 수락 (또는 거부) 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="73b29-254">간접 공급자는 전송 요청이 완료 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="73b29-255">전환 파트너가 전송 요청이 완료 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="73b29-256">파트너 전환</span><span class="sxs-lookup"><span data-stu-id="73b29-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="73b29-257">[파트너 센터 API/SDK](/partner-center/develop/manage-customers) 를 사용 하 여 기존 구독을 간접 공급자로 전송할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="73b29-258">고객의 구독 이전 자격 가져오기</span><span class="sxs-lookup"><span data-stu-id="73b29-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="73b29-259">고객의 이전 만들기</span><span class="sxs-lookup"><span data-stu-id="73b29-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="73b29-260">고객의 이전 철회</span><span class="sxs-lookup"><span data-stu-id="73b29-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="73b29-261">고객의 이전 수락</span><span class="sxs-lookup"><span data-stu-id="73b29-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="73b29-262">고객의 전송 거부</span><span class="sxs-lookup"><span data-stu-id="73b29-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="73b29-263">고객의 이전 가져오기</span><span class="sxs-lookup"><span data-stu-id="73b29-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="73b29-264">Id로 전송 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="73b29-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="73b29-265">파트너 전환-전송 요청 만들기</span><span class="sxs-lookup"><span data-stu-id="73b29-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="73b29-266">전환 파트너로 전송 요청을 만들려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="73b29-267">파트너 센터에 **관리 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="73b29-268">**고객** 페이지에서 원하는 고객을 선택 하 고 빠른 링크 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="73b29-269">**간접 공급자** 에서 의도 한 간접 공급자가 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="73b29-270">**구독 보기** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="73b29-271">**구독** 페이지에서 **구독 이전** 을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="73b29-272">**구독 전송** 에서 **구독 전송 요청** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="구독 전송 요청":::

7. <span data-ttu-id="73b29-274">요청 전송 대화 상자에서 전송할 구독을 하나 이상 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="전송 요청 만들기":::

8. <span data-ttu-id="73b29-276">**만들기** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-276">Click **Create**.</span></span>

9. <span data-ttu-id="73b29-277">활성 구독 전송 요청은 **구독 이전** 에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="전송 요청 목록":::

10. <span data-ttu-id="73b29-279">사용자가 구독 전송 요청을 만들었음을 간접 공급자에 게 알립니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="73b29-280">간접 공급자-전송 요청 수락</span><span class="sxs-lookup"><span data-stu-id="73b29-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="73b29-281">간접 공급자로 전송 요청을 검토 하 고 수락 하려면:</span><span class="sxs-lookup"><span data-stu-id="73b29-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="73b29-282">파트너 센터에 **관리** 에이전트 또는 **영업 에이전트로** 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="73b29-283">**고객 페이지에서** 원하는 고객을 선택 하 고 빠른 링크 아이콘을 클릭 하 여 고객의 요약 뷰를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="73b29-284">**간접 재판매인** 에서 전환 파트너가 나열 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="73b29-285">**구독 보기를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="73b29-286">구독 페이지에서 **구독** **이전** 을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="전송 요청 보기":::

6. <span data-ttu-id="73b29-288">**구독 전송** 에서 검토할 전송 요청을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="73b29-289">**적절하게 수락(또는** **거부)을** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="전송 요청 수락":::

8. <span data-ttu-id="73b29-291">전송 요청이 완료되기를 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="73b29-292">간접 공급자 - 전송 요청이 완료되었는지 확인</span><span class="sxs-lookup"><span data-stu-id="73b29-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="73b29-293">전송 요청이 성공적으로 완료되면 구독 아래에 구독이 표시되는지 **확인합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="73b29-294">전환 파트너에게 알릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="73b29-295">전환 파트너 - 전송 요청이 완료되었는지 확인</span><span class="sxs-lookup"><span data-stu-id="73b29-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="73b29-296">전환 파트너는 다음을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="73b29-297">관리 에이전트 또는 **판매 에이전트로** 파트너 센터 로그인합니다. </span><span class="sxs-lookup"><span data-stu-id="73b29-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="73b29-298">**고객** 페이지에서 원하는 고객을 선택하고 **빠른 링크** 아이콘을 클릭하여 고객의 요약 보기를 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="73b29-299">**구독 보기를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="73b29-300">구독 페이지에서 **구독** **이전** 을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="73b29-301">전송 요청이 완료 로 표시되는지 **확인합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="73b29-302">구독 페이지에서 구독이 더 이상 활성으로 표시되지 않는지 **확인합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="73b29-303">Azure 구독(MS-AZR-0145P)인 경우 더 이상 나열되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="73b29-304">라이선스 기반 구독(Office 365, Dynamics, Intune)이면 상태가 **일시 중단으로 나열됩니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="구독 일시 중단 됨":::

### <a name="considerations"></a><span data-ttu-id="73b29-306">고려 사항</span><span class="sxs-lookup"><span data-stu-id="73b29-306">Considerations</span></span>

- <span data-ttu-id="73b29-307">**전송 후에는 구독 ID가 다릅니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="73b29-308">Azure 구독 (MS-AZR-0017P-0145P) 인 경우에는 이전 소유자 로부터 유지 되 고 Azure 관리 포털에 표시 되는 Azure 구독 ID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="73b29-309">**여러 전송 요청에서 동일한 구독을 참조할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="73b29-310">기존 구독이 포함 된 전송 요청을 만든 후에는 첫 번째 전송 요청이 취소 될 때까지 동일한 구독을 포함 한 추가 전송 요청을 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="73b29-311">**라이선스 기반 구독의 추가 기능은 해당 기본 구독과 함께 전송 되어야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="73b29-312">전송 요청을 만들 때 하나 이상의 추가 기능이 있는 기존 구독을 선택 하면 해당 추가 기능이 전송 요청에 자동으로 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="73b29-313">**구독에 대 한 라이선스 수 변경 내용은 기존 전송 요청에 반영 되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="73b29-314">기존 구독이 포함 된 전송 요청을 만든 후에는 구독 (또는 연결 된 addons)의 라이선스 수량을 업데이트 하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="73b29-315">이렇게 하면 새 수량이 전송 요청에 반영 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="73b29-316">간접 공급자가 전송 요청을 수락 하면 결과 구독은 이전 수량을 갖게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="73b29-317">간접 공급자로 새 수량을 전송 하려는 경우 기존 전송 요청을 취소 하 고 새 전송 요청을 다시 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="73b29-318">**모든 구매는 자체 제공 구독 전송을 사용 하 여 전송할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="73b29-319">현재이 기능을 사용 하 여 O365 구독과 Azure PAYG subscription (MS-MS-AZR-0017P-0145P)만 전송할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="73b29-320">Azure Marketplace에 대 한 Azure 계획, Azure Reserved Instances, Term 기반 구독 및 SaaS 구독을 비롯 한 다른 구매는 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="73b29-321">전송 요청 제출 페이지에서 구독을 전송할 수 없는 이유가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="73b29-322">이러한 구독을 양도하려면 간접 공급자를 통해 [기존 구독을 취소하고](create-a-new-subscription.md#suspend-or-cancel-a-subscription) 고객을 위한 새 제안을 구매해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="73b29-323">**샌드박스 환경을 사용하여 테스트할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="73b29-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="73b29-324">간접 대리점 인센티브 등록</span><span class="sxs-lookup"><span data-stu-id="73b29-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="73b29-325">기존 직접 청구 파트너 테넌트에서 간접 대리점으로 성공적으로 등록한 후에는 30일 이내에 간접 대리점 인센티브에 등록하라는 초대를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="73b29-326">초대는 현재 CSP 파트너 테넌트와 연결된 파트너 MPN 계정을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="73b29-327">파트너 MPN 계정과 연결된 이메일 주소로 초대가 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="73b29-328">또한 동일한 파트너 테넌트에서 직접 청구 인센티브 프로그램에 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="73b29-329">프로그램을 별도로 관리해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="73b29-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="73b29-330">다음 단계</span><span class="sxs-lookup"><span data-stu-id="73b29-330">Next steps</span></span>

- [<span data-ttu-id="73b29-331">간접 재판매인이 되기 위한 추가 정보</span><span class="sxs-lookup"><span data-stu-id="73b29-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="73b29-332">CSP 직접 파트너 새로운 요구 사항</span><span class="sxs-lookup"><span data-stu-id="73b29-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="73b29-333">제한된 직접 청구 기능</span><span class="sxs-lookup"><span data-stu-id="73b29-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
