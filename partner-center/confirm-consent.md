---
title: Microsoft 고객 계약에 대한 고객의 동의 확인
description: Microsoft 고객 계약에 대한 고객의 동의 여부를 확인하는 방법을 알아봅니다. 이는 고객을 위해 Microsoft 제품 및 서비스를 주문하는 데 필요할 수 있습니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354613"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="b99d4-104">Microsoft 고객 계약에 대한 고객의 동의 여부를 확인하는 방법이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="b99d4-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="b99d4-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="b99d4-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b99d4-106">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="b99d4-106">Admin agent</span></span>
- <span data-ttu-id="b99d4-107">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="b99d4-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="b99d4-108">계약 리소스는 현재 Microsoft 퍼블릭 클라우드의 파트너 센터에서만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="b99d4-109">다음 센터에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-109">It is not applicable to:</span></span>
> * <span data-ttu-id="b99d4-110">21Vianet에서 운영하는 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b99d4-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="b99d4-111">Microsoft 클라우드 독일 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b99d4-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="b99d4-112">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b99d4-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="b99d4-113">2020년 1월 31일부로 모든 기존 고객과 신규 고객은 새로운 Microsoft 고객 계약에 서명해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="b99d4-114">자세한 내용은 [Microsoft 고객 계약에 대한 고객 동의 확인](confirm-customer-agreement.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b99d4-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="b99d4-115">파트너는 고객 대신 Microsoft 제품 및 서비스를 주문하려면 Microsoft 고객 계약에 대한 고객 동의를 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="b99d4-116">파트너가 규정을 잘 준수할 수 있도록, Microsoft는 계약에 동의한 사람과 관련해 다음과 같은 세부 정보를 제공함으로써 파트너에게 동의 여부를 확인하도록 요구하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="b99d4-117">이름</span><span class="sxs-lookup"><span data-stu-id="b99d4-117">First name</span></span>

- <span data-ttu-id="b99d4-118">성</span><span class="sxs-lookup"><span data-stu-id="b99d4-118">Last name</span></span>

- <span data-ttu-id="b99d4-119">메일 주소</span><span class="sxs-lookup"><span data-stu-id="b99d4-119">Email address</span></span>

- <span data-ttu-id="b99d4-120">전화 번호(선택 사항)</span><span class="sxs-lookup"><span data-stu-id="b99d4-120">Phone number (optional)</span></span>

- <span data-ttu-id="b99d4-121">동의 날짜</span><span class="sxs-lookup"><span data-stu-id="b99d4-121">Date of acceptance</span></span>

<span data-ttu-id="b99d4-122">직접 청구 파트너 및 간접 공급자는 파트너 센터 또는 파트너 센터 API를 통해 거래할 때 고객의 Microsoft 고객 계약 동의 여부를 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="b99d4-123">확인은 *필수 사항* 입니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="b99d4-124">고객이 계약에 동의한 것으로 확인되지 않으면 다음과 같은 결과가 초래됩니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="b99d4-125">해당 고객의 신규 주문을 작성할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="b99d4-126">해당 고객의 기존 라이선스 기반 구독의 라이선스 수를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="b99d4-127">파트너 센터 또는 파트너 센터 API를 통해 고객 동의 여부를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="b99d4-128">파트너 센터 API를 통해 확인하려면 다음 토픽을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b99d4-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="b99d4-129">고객 동의 확인 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="b99d4-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="b99d4-130">계약 메타데이터 가져오기</span><span class="sxs-lookup"><span data-stu-id="b99d4-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="b99d4-131">고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b99d4-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="b99d4-132">프로덕션 환경과 샌드박스 환경에 모두 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="b99d4-133">신규 고객의 고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b99d4-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="b99d4-134">파트너 센터에서 신규 고객 테넌트를 생성하는 동안 다음 절차에 따라 고객의 동의 여부를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="b99d4-135">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b99d4-136">**고객**, **새 고객**, **계정 정보** 를 차례로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="b99d4-137">**회사** 및 **기본 연락처** 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="회사 정보":::

3. <span data-ttu-id="b99d4-139">**Microsoft 고객 계약** 에서 **고객이 최신 Microsoft 고객 계약에 동의했음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="b99d4-140">**계약 동의 날짜** 에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b99d4-141">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="b99d4-142">동의를 표한 사용자의 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="동의 날짜 추가":::

   <span data-ttu-id="b99d4-144">기본적으로 사용자의 기본 연락처 정보가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="b99d4-145">이 정보가 틀린 경우에는 **업데이트** 를 선택하고, 계약에 동의한 사람의 **이름**, **성**, **이메일 주소** 및 \**전화 번호*(선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="b99d4-146">고객 테넌트를 생성하기 위한 나머지 단계를 계속하려면 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="b99d4-147">기존 고객의 동의 여부 확인</span><span class="sxs-lookup"><span data-stu-id="b99d4-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="b99d4-148">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b99d4-149">**고객** 을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="b99d4-150">**계정 정보** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-150">Select **Account info**.</span></span>

3. <span data-ttu-id="b99d4-151">**Microsoft 고객 계약** 에서 **업데이트** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Update":::

4. <span data-ttu-id="b99d4-153">계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="b99d4-154">**계약 동의 날짜** 에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b99d4-155">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="b99d4-156">**저장하고 계속** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="b99d4-157">기존 고객의 신규 주문을 작성할 때 고객의 동의 여부 확인</span><span class="sxs-lookup"><span data-stu-id="b99d4-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="b99d4-158">앞서 동의 여부를 확인하지 않은 기존 고객의 신규 주문을 작성하려고 시도하면 확인을 완료하라는 메시지를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="b99d4-159">다음 절차를 사용 하 여이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="b99d4-160">계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="b99d4-161">**계약 동의 날짜** 에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b99d4-162">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="b99d4-163">**저장하고 계속** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="b99d4-164">기존 고객의 동의 여부 검색</span><span class="sxs-lookup"><span data-stu-id="b99d4-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="b99d4-165">아래 절차에 따라 이전에 제공한 기존 고객의 동의 여부를 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="b99d4-166">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b99d4-167">**고객** 을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="b99d4-168">**계정 정보** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-168">Select **Account info**.</span></span>

3. <span data-ttu-id="b99d4-169">**Microsoft 고객 계약** 에서 이 고객의 확인 여부를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b99d4-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b99d4-170">다음 단계</span><span class="sxs-lookup"><span data-stu-id="b99d4-170">Next steps</span></span>

- [<span data-ttu-id="b99d4-171">CSP 파트너 프로그램에서 고객의 Microsoft 고객 계약 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b99d4-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="b99d4-172">고객을 대신하여 Microsoft 고객 계약 동의 증명</span><span class="sxs-lookup"><span data-stu-id="b99d4-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)