---
title: 고객 제휴 만들기
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: CPOR(Claiming Partner of Record) 모델을 사용하여 고객 연결을 만듭니다. Microsoft 365 & Dynamics 365 고객에 대한 판매, 사용량, 인센티브 관리를 지원합니다.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489954"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="608db-104">Microsoft 365 및 Dynamics 365에 대해 CPOR(클레임된 파트너) 모델을 통한 고객 연결</span><span class="sxs-lookup"><span data-stu-id="608db-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="608db-105">**적절한 역할:** 인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="608db-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="608db-106">2019년 10월 1일에 Microsoft는 CPOR(Claiming Partner of Record) 모델을 사용하여 OSA(온라인 서비스 권고) 판매, OSU(온라인 서비스 사용) Microsoft 365 및 OSU-Business 애플리케이션 인센티브와 관련하여 Microsoft 365 및 Dynamics 365 고객과의 관계를 관리하기 시작했습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="608db-107">CPOR(고객 연결) 클레임은 OSA(Online Services Advisory) 판매, OSU(온라인 서비스 사용) Microsoft 365 및 OSU-Business 애플리케이션 인센티브 프로그램에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="608db-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="608db-108">CSP(클라우드 솔루션 공급자), Managed Reseller, 호스팅 또는 Surface와 같은 다른 프로그램에 대한 공동 클레임을 제출하는 경우 여기에 설명된 공동 클레임 프로세스를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="608db-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="608db-109">클레임을 제출하면 Microsoft에서 유효성을 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="608db-110">이 시점에서 자세한 정보를 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="608db-111">또한 고객에게 연결 요청을 알립니다.</span><span class="sxs-lookup"><span data-stu-id="608db-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="608db-112">고객은 영업일 5일 동안 옵트아웃해야 합니다. 옵트아웃하지 않으면 이 특정 테넌트 및 워크로드와의 연결이 공식이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="608db-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="608db-113">이 시점에서 고객의 사용량 현황 데이터에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="608db-114">클레임을 완료하려면 다음 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="608db-115">클레임을 만드는 엔터티의 **MPN ID(Microsoft 파트너 네트워크** ID)</span><span class="sxs-lookup"><span data-stu-id="608db-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="608db-116">고객의 **도메인 이름(자세한** 내용은 [테넌트 ID 찾기, 도메인 이름, 사용자 개체 ID](find-ids-and-domain-names.md)참조)</span><span class="sxs-lookup"><span data-stu-id="608db-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="608db-117">고객의 **디렉터리 ID** 또는 **테넌트 ID(자세한** 내용은 [테넌트 ID 찾기, 도메인 이름, 사용자 개체 ID](find-ids-and-domain-names.md)참조)</span><span class="sxs-lookup"><span data-stu-id="608db-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="608db-118">**솔루션** 영역(예: Business Applications 또는 Microsoft 365)</span><span class="sxs-lookup"><span data-stu-id="608db-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="608db-119">수행한 **활동** 및 수행하려는 클레임 유형(예: 판매 전, 사용량 또는 수익 연결)</span><span class="sxs-lookup"><span data-stu-id="608db-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="608db-120">고객의 연락처 **이름,** 제목 및 이메일 주소</span><span class="sxs-lookup"><span data-stu-id="608db-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="608db-121">Dynamics 365의 경우 고객의 **기술 연락처** 이름, 직위 및 이메일 주소도 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="608db-122">회사의 **연락처 이름** 및 이메일 주소</span><span class="sxs-lookup"><span data-stu-id="608db-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="608db-123">이 클레임에 대한 **이름을** 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="608db-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="608db-124">클레임하는 **제품** 또는 워크로드</span><span class="sxs-lookup"><span data-stu-id="608db-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="608db-125">**PoE(실행 증명)(예:** 고객이 서명한 작업 명세서)</span><span class="sxs-lookup"><span data-stu-id="608db-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="608db-126">사용할 PoE 템플릿을 다운로드할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="608db-127">수익 연결을 클레임하는 파트너의 **경우: Dynamics 솔루션 판매자 이름,** **고객 이름** 및 **ISV 제품/솔루션의 이름입니다.**</span><span class="sxs-lookup"><span data-stu-id="608db-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="608db-128">또한 다음 사항을 이해해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-128">You should also understand the following points:</span></span>

- <span data-ttu-id="608db-129">기존 Microsoft 365 고객이 있는 경우 이 프로세스를 사용하여 OSU 인센티브 획득을 계속하려는 고객과 다시 연결을 끊어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="608db-130">Dynamics 365 또는 Power BI 고객과 기존 연결이 있는 경우 구독이 만료될 때까지 이러한 연결은 유효한 상태로 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="608db-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="608db-131">고객은 여러 파트너를 가질 수 있지만 각 워크로드(OSU-Microsoft 365용) 또는 구독(OSA-Sell 및 OSU-Business 애플리케이션의 경우)은 한 파트너와만 연결될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="608db-132">고객 제휴 만들기</span><span class="sxs-lookup"><span data-stu-id="608db-132">Create a customer association</span></span>

1. <span data-ttu-id="608db-133">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="608db-134">**인센티브** 탭을 선택하고 **개요** 를 선택한 **다음, 고객 연결을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="608db-135">고객 연결 페이지의 맨 위에서 **+ 고객 연결** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="608db-136">고객과 연결할 파트너 위치의 **MPN ID** 를 선택한 다음 고객의 도메인 이름과 디렉터리 ID를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="608db-137">다음을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="608db-138">**계속** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-138">Select **Continue**.</span></span>

6. <span data-ttu-id="608db-139">솔루션 **영역** 및 **작업 을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="608db-140">Business Applications 선택하는 경우 **사용량 및/또는 판매 전** 또는 **수익 연결** 를 선택한 **다음, 계속을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="608db-141">수익 연결을 선택하는 경우 아래 나열된 것과 약간 다른 정보를 묻는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="608db-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="608db-142">**고객 연결** 페이지에서 적절한 정보를 입력한 다음 클레임 **만들기를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="608db-143">이 고객 연결과 연결된 제품을 선택한 다음, **계속을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="608db-144">고객 연락처 정보 및 회사의 연락처 정보 입력을 완료합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="608db-145">모든 필드는 필수입니다.</span><span class="sxs-lookup"><span data-stu-id="608db-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="608db-146">제품이 Dynamics 365이고 선택한 제품에 이 특정 고객에 대한 여러 구독이 있는 경우 구독 ID도 입력해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="608db-147">PoE를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-147">Supply your PoE.</span></span> <span data-ttu-id="608db-148">이를 상자로 끌거나, 고유한 지원 설명서를 찾아보거나, **템플릿 다운로드** 를 선택하여 템플릿을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="608db-149">원하는 경우 설명을 추가하여 저장한 다음 **클레임 제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="608db-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="608db-150">고객 연결에 대한 승인을 요청하는 고객에게 이메일이 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="608db-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="608db-151">고객 연결을 제출한 후에는 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="608db-152">고객 연결의 상태가 **상태** 필드에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="608db-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="608db-153">**기록** 을 선택하여 고객 연결 기록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="608db-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="608db-154">다음 단계</span><span class="sxs-lookup"><span data-stu-id="608db-154">Next steps</span></span>

- [<span data-ttu-id="608db-155">고객 제휴 보기</span><span class="sxs-lookup"><span data-stu-id="608db-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)