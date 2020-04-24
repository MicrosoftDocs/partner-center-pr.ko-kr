---
title: 고객의 Microsoft 고객 계약 동의 확인 | 파트너 센터
ms.topic: article
ms.date: 04/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft 고객 계약에 대한 고객의 동의 여부를 확인하는 방법을 알아봅니다. 이는 고객을 위해 Microsoft 제품 및 서비스를 주문하는 데 필요할 수 있습니다.
author: LauraBrenner
ms.author: labrenne
keywords: 고객, 고객들, 동의, MCA, Microsoft 고객 계약, 고객 계약 템플릿
ms.localizationpriority: high
ms.openlocfilehash: 2223a8e05a9df4c2d6ac377fc6f6b5a06944adc9
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2020
ms.locfileid: "81123323"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="b3210-105">Microsoft 고객 계약에 대한 고객의 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b3210-105">Confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="b3210-106">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="b3210-106">**Applies to**</span></span>
-  <span data-ttu-id="b3210-107">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b3210-107">Partner Center</span></span>

<span data-ttu-id="b3210-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="b3210-108">**Appropriate roles**</span></span>

- <span data-ttu-id="b3210-109">관리자 에이전트</span><span class="sxs-lookup"><span data-stu-id="b3210-109">Admin agent</span></span>
- <span data-ttu-id="b3210-110">영업 에이전트</span><span class="sxs-lookup"><span data-stu-id="b3210-110">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="b3210-111">계약 리소스는 현재 Microsoft 퍼블릭 클라우드의 파트너 센터에서만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-111">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="b3210-112">다음 센터에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-112">It is not applicable to:</span></span>
> * <span data-ttu-id="b3210-113">21Vianet에서 운영하는 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b3210-113">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="b3210-114">Microsoft 클라우드 독일 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b3210-114">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="b3210-115">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b3210-115">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="b3210-116">2020년 1월 31일부로 모든 기존 고객과 신규 고객은 새로운 Microsoft 고객 계약에 서명해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-116">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="b3210-117">자세한 내용은 [Microsoft 고객 계약에 대한 고객 동의 확인](confirm-customer-agreement.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3210-117">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="b3210-118">파트너는 고객 대신 Microsoft 제품 및 서비스를 주문하려면 Microsoft 고객 계약에 대한 고객 동의를 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-118">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="b3210-119">파트너가 규정을 잘 준수할 수 있도록, Microsoft는 계약에 동의한 사람과 관련해 다음과 같은 세부 정보를 제공함으로써 파트너에게 동의 여부를 확인하도록 요구하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-119">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="b3210-120">이름</span><span class="sxs-lookup"><span data-stu-id="b3210-120">First name</span></span>

- <span data-ttu-id="b3210-121">성</span><span class="sxs-lookup"><span data-stu-id="b3210-121">Last name</span></span>

- <span data-ttu-id="b3210-122">메일 주소</span><span class="sxs-lookup"><span data-stu-id="b3210-122">Email address</span></span>

- <span data-ttu-id="b3210-123">전화 번호(선택 사항)</span><span class="sxs-lookup"><span data-stu-id="b3210-123">Phone number (optional)</span></span>

- <span data-ttu-id="b3210-124">동의 날짜</span><span class="sxs-lookup"><span data-stu-id="b3210-124">Date of acceptance</span></span>

<span data-ttu-id="b3210-125">직접 청구 파트너 및 간접 공급자는 파트너 센터 또는 파트너 센터 API를 통해 거래할 때 고객의 Microsoft 고객 계약 동의 여부를 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-125">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="b3210-126">확인은 *필수 사항*입니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-126">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="b3210-127">고객이 계약에 동의한 것으로 확인되지 않으면 다음과 같은 결과가 초래됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-127">If confirmation is not provided for a given customer:</span></span>

-    <span data-ttu-id="b3210-128">해당 고객의 신규 주문을 작성할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-128">You won't be able to create new orders for this customer.</span></span>

-    <span data-ttu-id="b3210-129">해당 고객의 기존 사용자 수 기준 구독의 사용자 수를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-129">You won't be able to change the seat count of existing seat-based subscriptions for this customer.</span></span>

<span data-ttu-id="b3210-130">파트너 센터 또는 파트너 센터 API를 통해 고객 동의 여부를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-130">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="b3210-131">파트너 센터 API를 통해 확인하려면 다음 토픽을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b3210-131">To do this through the Partner Center API, see the following topics:</span></span> 

-   [<span data-ttu-id="b3210-132">고객 동의 확인 정보 가져오기</span><span class="sxs-lookup"><span data-stu-id="b3210-132">Get confirmation of customer consent</span></span>](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [<span data-ttu-id="b3210-133">계약 메타데이터 가져오기</span><span class="sxs-lookup"><span data-stu-id="b3210-133">Get agreement metadata</span></span>](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [<span data-ttu-id="b3210-134">고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b3210-134">Confirm customer consent</span></span>](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


<span data-ttu-id="b3210-135">프로덕션 환경과 샌드박스 환경에 모두 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-135">This applies to both production and sandbox environments.</span></span>

## <a name="confirming-customer-acceptance-in-partner-center"></a><span data-ttu-id="b3210-136">파트너 센터에서 고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b3210-136">Confirming customer acceptance in Partner Center</span></span>

### <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="b3210-137">신규 고객의 고객 동의 확인</span><span class="sxs-lookup"><span data-stu-id="b3210-137">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="b3210-138">파트너 센터에서 신규 고객 테넌트를 생성하는 동안 다음 절차에 따라 고객의 동의 여부를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-138">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="b3210-139">고객의 동의 여부를 확인하려면 관리자 에이전트 또는 판매 에이전트여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-139">Note that you must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b3210-140">**고객**, **새 고객**, **계정 정보**를 차례로 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-140">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>
2. <span data-ttu-id="b3210-141">**회사** 및 **기본 연락처** 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-141">Enter the information about the **Company** and **Primary contact**.</span></span>

![회사 정보](images/mca/mca1.png)

3. <span data-ttu-id="b3210-143">**Microsoft 고객 계약**에서 **고객이 최신 Microsoft 고객 계약에 동의했음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-143">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>
4. <span data-ttu-id="b3210-144">**계약 동의 날짜**에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-144">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b3210-145">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-145">You cannot set this to a future date.</span></span>
5. <span data-ttu-id="b3210-146">동의를 표한 사용자의 세부 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-146">Enter the details of the user who provided the acceptance.</span></span>

![동의 날짜 추가](images/mca/MCA3.png)

<span data-ttu-id="b3210-148">기본적으로 사용자의 기본 연락처 정보가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-148">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="b3210-149">이 정보가 틀린 경우에는 **업데이트**를 선택하고, 계약에 동의한 사람의 **이름**, **성**, **이메일 주소** 및 \**전화 번호*(선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-149">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="b3210-150">고객 테넌트를 생성하기 위한 나머지 단계를 계속하려면 **다음**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-150">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="b3210-151">기존 고객의 동의 여부 확인</span><span class="sxs-lookup"><span data-stu-id="b3210-151">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="b3210-152">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-152">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b3210-153">**고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-153">Select **Customers**, and then find and select the customer you want to see.</span></span>
2. <span data-ttu-id="b3210-154">**계정 정보**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-154">Select **Account info**.</span></span>
3. <span data-ttu-id="b3210-155">**Microsoft 고객 계약**에서 **업데이트**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-155">Under **Microsoft customer agreement**, select **Update**.</span></span>

![업데이트](images/mca/mca4.png)

4. <span data-ttu-id="b3210-157">계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-157">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>
5. <span data-ttu-id="b3210-158">**계약 동의 날짜**에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-158">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b3210-159">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-159">You cannot set this to a future date.</span></span>
6. <span data-ttu-id="b3210-160">**저장하고 계속**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-160">Select **Save and continue**.</span></span>

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="b3210-161">기존 고객의 신규 주문을 작성할 때 고객의 동의 여부 확인</span><span class="sxs-lookup"><span data-stu-id="b3210-161">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="b3210-162">앞서 동의 여부를 확인하지 않은 기존 고객의 신규 주문을 작성하려고 시도하면 확인을 완료하라는 메시지를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-162">If you try to create a new order for an existing customer which you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="b3210-163">다음 절차를 사용 하 여이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-163">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="b3210-164">계약에 동의한 사용자의 **이름**, **성**, **이메일 주소** 및 **전화 번호**(선택 사항)를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-164">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>
2. <span data-ttu-id="b3210-165">**계약 동의 날짜**에 해당 날짜를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-165">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="b3210-166">이 날짜는 미래의 날짜로 설정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-166">You cannot set this to a future date.</span></span>
3. <span data-ttu-id="b3210-167">**저장하고 계속**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-167">Select **Save and continue**.</span></span>

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="b3210-168">기존 고객의 동의 여부 검색</span><span class="sxs-lookup"><span data-stu-id="b3210-168">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="b3210-169">아래 절차에 따라 이전에 제공한 기존 고객의 동의 여부를 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-169">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="b3210-170">관리 담당자 또는 판매 담당자만 이러한 확인이 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-170">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="b3210-171">**고객**을 선택한 다음, 확인하려는 고객을 찾아서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-171">Select **Customers**, and then find and select the customer you want to see.</span></span>
2. <span data-ttu-id="b3210-172">**계정 정보**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-172">Select **Account info**.</span></span>
3. <span data-ttu-id="b3210-173">**Microsoft 고객 계약**에서 이 고객의 확인 여부를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3210-173">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>
