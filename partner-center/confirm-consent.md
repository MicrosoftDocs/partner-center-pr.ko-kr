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
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333922"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="224f2-104">Microsoft 고객 계약에 대한 고객의 동의 여부를 확인하는 방법이 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="224f2-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="224f2-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="224f2-105">**Applies to**</span></span>

-  <span data-ttu-id="224f2-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="224f2-106">Partner Center</span></span>

<span data-ttu-id="224f2-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="224f2-107">**Appropriate roles**</span></span>

- <span data-ttu-id="224f2-108">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="224f2-108">Admin agent</span></span>
- <span data-ttu-id="224f2-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="224f2-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="224f2-110">계약 리소스는 현재 Microsoft 퍼블릭 클라우드의 파트너 센터에서만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="224f2-111">다음 센터에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-111">It is not applicable to:</span></span>
> * <span data-ttu-id="224f2-112">21Vianet에서 운영하는 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="224f2-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="224f2-113">Microsoft 클라우드 독일 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="224f2-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="224f2-114">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="224f2-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="224f2-115">2020년 1월 31일부로 모든 기존 고객과 신규 고객은 새로운 Microsoft 고객 계약에 서명해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="224f2-116">자세한 내용은 [Microsoft 고객 계약에 대한 고객 동의 확인](confirm-customer-agreement.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="224f2-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="224f2-117">파트너는 고객 대신 Microsoft 제품 및 서비스를 주문하려면 Microsoft 고객 계약에 대한 고객 동의를 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="224f2-118">파트너가 규정을 잘 준수할 수 있도록, Microsoft는 계약에 동의한 사람과 관련해 다음과 같은 세부 정보를 제공함으로써 파트너에게 동의 여부를 확인하도록 요구하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="224f2-119">이름</span><span class="sxs-lookup"><span data-stu-id="224f2-119">First name</span></span>

- <span data-ttu-id="224f2-120">성</span><span class="sxs-lookup"><span data-stu-id="224f2-120">Last name</span></span>

- <span data-ttu-id="224f2-121">메일 주소</span><span class="sxs-lookup"><span data-stu-id="224f2-121">Email address</span></span>

- <span data-ttu-id="224f2-122">전화 번호(선택 사항)</span><span class="sxs-lookup"><span data-stu-id="224f2-122">Phone number (optional)</span></span>

- <span data-ttu-id="224f2-123">동의 날짜</span><span class="sxs-lookup"><span data-stu-id="224f2-123">Date of acceptance</span></span>

<span data-ttu-id="224f2-124">직접 청구 파트너 및 간접 공급자는 파트너 센터 또는 파트너 센터 API를 통해 거래할 때 고객의 Microsoft 고객 계약 동의 여부를 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="224f2-125">확인은 *필수 사항* 입니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="224f2-126">고객이 계약에 동의한 것으로 확인되지 않으면 다음과 같은 결과가 초래됩니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="224f2-127">해당 고객의 신규 주문을 작성할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="224f2-128">해당 고객의 기존 라이선스 기반 구독의 라이선스 수를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="224f2-129">파트너 센터 또는 파트너 센터 API를 통해 고객 동의 여부를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="224f2-130">파트너 센터 API를 통해 확인하려면 다음 토픽을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="224f2-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="224f2-131">고객 동의 확인 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="224f2-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="224f2-132">계약 메타데이터 가져오기</span><span class="sxs-lookup"><span data-stu-id="224f2-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="224f2-133">고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="224f2-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="224f2-134">프로덕션 환경과 샌드박스 환경에 모두 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="224f2-135">신규 고객의 고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="224f2-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="224f2-136">파트너 센터에서 신규 고객 테넌트를 생성하는 동안 다음 절차에 따라 고객의 동의 여부를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="224f2-137">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="224f2-138">**고객** , **새 고객** , **계정 정보** 를 차례로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="224f2-139">**회사** 및 **기본 연락처** 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="회사 정보":::

3. <span data-ttu-id="224f2-141">**Microsoft 고객 계약** 에서 **고객이 최신 Microsoft 고객 계약에 동의했음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="224f2-142">**계약 동의 날짜** 에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="224f2-143">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="224f2-144">동의를 표한 사용자의 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="동의 날짜 추가":::

   <span data-ttu-id="224f2-146">기본적으로 사용자의 기본 연락처 정보가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="224f2-147">이 정보가 틀린 경우에는 **업데이트** 를 선택하고, 계약에 동의한 사람의 **이름** , **성** , **이메일 주소** 및 \* *전화 번호* (선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="224f2-148">고객 테넌트를 생성하기 위한 나머지 단계를 계속하려면 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="224f2-149">기존 고객의 동의 여부 확인</span><span class="sxs-lookup"><span data-stu-id="224f2-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="224f2-150">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="224f2-151">**고객** 을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="224f2-152">**계정 정보** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-152">Select **Account info** .</span></span>

3. <span data-ttu-id="224f2-153">**Microsoft 고객 계약** 에서 **업데이트** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Update":::

4. <span data-ttu-id="224f2-155">계약에 동의한 사용자의 **이름** , **성** , **이메일 주소** 및 **전화 번호** (선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="224f2-156">**계약 동의 날짜** 에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="224f2-157">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="224f2-158">**저장하고 계속** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="224f2-159">기존 고객의 신규 주문을 작성할 때 고객의 동의 여부 확인</span><span class="sxs-lookup"><span data-stu-id="224f2-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="224f2-160">앞서 동의 여부를 확인하지 않은 기존 고객의 신규 주문을 작성하려고 시도하면 확인을 완료하라는 메시지를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="224f2-161">다음 절차를 사용 하 여이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="224f2-162">계약에 동의한 사용자의 **이름** , **성** , **이메일 주소** 및 **전화 번호** (선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="224f2-163">**계약 동의 날짜** 에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="224f2-164">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="224f2-165">**저장하고 계속** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="224f2-166">기존 고객의 동의 여부 검색</span><span class="sxs-lookup"><span data-stu-id="224f2-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="224f2-167">아래 절차에 따라 이전에 제공한 기존 고객의 동의 여부를 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="224f2-168">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="224f2-169">**고객** 을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="224f2-170">**계정 정보** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-170">Select **Account info** .</span></span>

3. <span data-ttu-id="224f2-171">**Microsoft 고객 계약** 에서 이 고객의 확인 여부를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="224f2-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="224f2-172">다음 단계</span><span class="sxs-lookup"><span data-stu-id="224f2-172">Next steps</span></span>

- [<span data-ttu-id="224f2-173">CSP 파트너 프로그램에서 고객의 Microsoft 고객 계약 동의 확인</span><span class="sxs-lookup"><span data-stu-id="224f2-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="224f2-174">고객을 대신하여 Microsoft 고객 계약 동의 증명</span><span class="sxs-lookup"><span data-stu-id="224f2-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)