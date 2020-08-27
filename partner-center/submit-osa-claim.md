---
title: CPOR 모델을 통해 고객 연결 만들기
ms.topic: article
ms.date: 08/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: CPOR (레코드 파트너 클레임) 모델을 통해 고객 연결을 만듭니다. Microsoft 365 및 Dynamics 365 고객에 대 한 판매, 사용량 &의 성과급을 관리 하는 데 도움이 됩니다.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d5c71bf5c5461abaa7d86a19711ad941e0e8a4ff
ms.sourcegitcommit: 2d78a1a110a78c0997775f3613f1b08e333c546c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/26/2020
ms.locfileid: "88942555"
---
# <a name="create-a-customer-association-via-the-cpor-model--use-for-microsoft-365-and-dynamics-365-customers"></a><span data-ttu-id="42cc1-104">CPOR 모델을 통해 고객 연결 만들기 – Microsoft 365 및 Dynamics 365 고객에 사용</span><span class="sxs-lookup"><span data-stu-id="42cc1-104">Create a customer association via the CPOR model – use for Microsoft 365 and Dynamics 365 customers</span></span>

<span data-ttu-id="42cc1-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="42cc1-105">**Applies to**</span></span>

- <span data-ttu-id="42cc1-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="42cc1-106">Partner Center</span></span>

<span data-ttu-id="42cc1-107">2019 년 10 월 1 일부 터 Microsoft는 Microsoft에서 Microsoft의 Microsoft Microsoft 365 및 Dynamics 365 고객과의 연결을 관리 하기 위해 Microsoft의 OSA (온라인 서비스 자문) 판매, OSU (온라인 서비스 사용) Microsoft 365 및 OSU 비즈니스 응용 프로그램에 대 한 성과급을 관리 하기 시작 했습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

><span data-ttu-id="42cc1-108">[! 중요:] 고객 연결 (CPOR) 클레임은 OSA (Online services Advise) 판매, OSU (Online Services Usage) Microsoft 365 및 OSU 비즈니스 응용 프로그램 동기 프로그램에만 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-108">[!Important:] Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="42cc1-109">클라우드 솔루션 공급자, 관리 재판매인, 호스팅 또는 화면과 같은 다른 프로그램에 대 한 공동 작업 클레임을 제출 하는 경우 여기에 설명 된 Co op 클레임 프로세스를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="42cc1-109">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span>

<span data-ttu-id="42cc1-110">클레임을 제출 하면 Microsoft에서 유효성을 검사 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-110">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="42cc1-111">이 시점에서 추가 정보를 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-111">We may ask you for more information at this point.</span></span> <span data-ttu-id="42cc1-112">또한 고객의 연결 요청에 대해 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-112">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="42cc1-113">고객은 옵트아웃 (opt out)을 5 영업일 이내에 사용할 수 있습니다. 옵트아웃 (opt out) 하지 않으면이 특정 테 넌 트 및 워크 로드와의 연결이 공식적으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-113">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="42cc1-114">이 시점에서 고객의 사용 현황 데이터에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-114">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="42cc1-115">클레임을 완료 하려면 다음 정보가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-115">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="42cc1-116">클레임을 만드는 엔터티의 **MPN ID**</span><span class="sxs-lookup"><span data-stu-id="42cc1-116">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="42cc1-117">고객의 **도메인 이름** [이를 찾습니다](find-domain-name.md) .</span><span class="sxs-lookup"><span data-stu-id="42cc1-117">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="42cc1-118">고객의 **디렉터리 id** 또는 **테 넌 트 id** 를 [찾습니다](find-domain-name.md) .</span><span class="sxs-lookup"><span data-stu-id="42cc1-118">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="42cc1-119">Business Applications 또는 Microsoft 365와 같은 **솔루션 영역**</span><span class="sxs-lookup"><span data-stu-id="42cc1-119">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="42cc1-120">수행 된 **작업** 및 수행 하려는 클레임 유형 (예: 판매 전, 사용량 또는 수입 연결)</span><span class="sxs-lookup"><span data-stu-id="42cc1-120">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="42cc1-121">고객의 **연락처 이름**, 제목 및 전자 메일 주소</span><span class="sxs-lookup"><span data-stu-id="42cc1-121">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="42cc1-122">Dynamics 365의 경우 고객의 **기술 담당자** 이름, 제목 및 전자 메일 주소도 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-122">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="42cc1-123">회사의 **연락처 이름** 및 전자 메일 주소</span><span class="sxs-lookup"><span data-stu-id="42cc1-123">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="42cc1-124">이 클레임에 대 한 **이름을** 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-124">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="42cc1-125">주장 하는 **제품** 또는 워크 로드</span><span class="sxs-lookup"><span data-stu-id="42cc1-125">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="42cc1-126">**POE (실행 증명) (** 예: 고객이 서명한 작업의 문)</span><span class="sxs-lookup"><span data-stu-id="42cc1-126">**Proof of execution (POE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="42cc1-127">POE 템플릿을 다운로드 하 여 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-127">You can also download a POE template to use.</span></span>

- <span data-ttu-id="42cc1-128">수익 연결만을 주장 하는 파트너의 경우: **Dynamics solution 판매자 이름**, **고객 이름**및 **ISV 제품/솔루션의 이름**입니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-128">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="42cc1-129">또한 다음 사항을 이해 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-129">You should also understand the following points:</span></span>

- <span data-ttu-id="42cc1-130">기존 Microsoft 365 고객이 있는 경우이 프로세스를 사용 하 여 계속 해 서 OSU의 성과급을 얻을 수 있도록 다시 연결 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-130">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="42cc1-131">Dynamics 365 또는 Power BI 고객에 대 한 기존 연결이 있는 경우 구독이 만료 될 때까지 이러한 연결은 유효한 상태로 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-131">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="42cc1-132">고객은 여러 파트너를 가질 수 있지만 각 워크 로드 (OSU Microsoft 365의 경우) 또는 구독 (OSA-판매 및 OSU-Business Applications)은 한 파트너에만 연결 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-132">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="42cc1-133">고객 연결 만들기</span><span class="sxs-lookup"><span data-stu-id="42cc1-133">Create a customer association</span></span>

1. <span data-ttu-id="42cc1-134">파트너 센터 대시보드의 **성과급**아래에서 **개요**를 선택한 다음, **고객 연결**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-134">In the Partner Center dashboard, under **Incentives**, select **Overview**, and then select **Customer associations**.</span></span> 

2. <span data-ttu-id="42cc1-135">고객 연결 페이지의 맨 위에서 **+ 고객 연결**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

3. <span data-ttu-id="42cc1-136">고객과 연결할 파트너 위치의 **MPN ID**를 선택한 다음 고객의 도메인 이름과 디렉터리 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="42cc1-137">찾을</span><span class="sxs-lookup"><span data-stu-id="42cc1-137">Find this</span></span>](find-domain-name.md)

4. <span data-ttu-id="42cc1-138">**계속**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-138">Select **Continue**.</span></span>

5. <span data-ttu-id="42cc1-139">**솔루션 영역** 및 **활동**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="42cc1-140">Business Applications를 선택 하는 경우 **사용량 및/또는 판매 전**또는 **수입 연결**중 하나를 선택한 다음 **계속**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 

   ><span data-ttu-id="42cc1-141">수익 연결을 선택하는 경우 아래 나열된 것과 약간 다른 정보를 묻는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

6. <span data-ttu-id="42cc1-142">**고객 연결** 페이지에 적절 한 정보를 입력 하 고 **클레임 만들기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

7. <span data-ttu-id="42cc1-143">이 고객 연결과 관련 된 제품을 선택 하 고 **계속**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

8. <span data-ttu-id="42cc1-144">고객 연락처 정보 및 회사의 연락처 정보 입력을 완료합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="42cc1-145">모든 필드는 필수입니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="42cc1-146">제품이 Dynamics 365이 고 선택한 제품에이 특정 고객에 대 한 구독이 여러 개 있는 경우 구독 ID도 입력 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

9. <span data-ttu-id="42cc1-147">POE(실행 증명)를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-147">Supply your proof of execution (POE).</span></span> <span data-ttu-id="42cc1-148">이를 상자로 끌거나, 고유한 지원 설명서를 찾아보거나, **템플릿 다운로드**를 선택하여 템플릿을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

10. <span data-ttu-id="42cc1-149">원하는 경우 설명을 추가하여 저장한 다음 **클레임 제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="42cc1-150">고객 연결에 대한 승인을 요청하는 고객에게 이메일이 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="42cc1-151">고객 연결을 제출한 후에는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="42cc1-152">고객 연결의 상태가 **상태** 필드에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="42cc1-153">**기록**을 선택하여 고객 연결 기록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="42cc1-153">Select **History** to view the history of a customer association.</span></span>
