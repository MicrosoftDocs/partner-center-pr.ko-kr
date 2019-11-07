---
title: 고객을 위한 Azure 지출 예산 설정 | 파트너 센터
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 파트너 센터에서 고객 당 월별 예산을 설정 하 여 해당 월의 끝에 Azure 청구서가 예기치 않은 상태가 되도록 할 수 있습니다.
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 03901b4b17c744c0c91d732331842f6cb579bf88
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73654065"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="213e6-103">고객을 위한 Azure 지출 예산 설정</span><span class="sxs-lookup"><span data-stu-id="213e6-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="213e6-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="213e6-104">**Applies to**</span></span>

-  <span data-ttu-id="213e6-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="213e6-105">Partner Center</span></span>
-  <span data-ttu-id="213e6-106">Microsoft Cloud for US Government 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="213e6-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="213e6-107">고객이 Azure 비용을 관리 하는 데 도움이 되도록 매월 지출 예산을 설정 하 여 Azure 청구서가 예상 보다 더 이상 표시 되지 않도록 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn't higher than they anticipated.</span></span> <span data-ttu-id="213e6-108">Azure 지출을 예산을 설정하면 해당 달 동안 고객의 Azure 지출을 예산과 비교할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="213e6-109">이 기능을 사용하면 다음을 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="213e6-110">고객이 예산 한도에 도달할 정보로 지출한 경우 전자 메일로 알림 받기</span><span class="sxs-lookup"><span data-stu-id="213e6-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="213e6-111">매월 고객의 예상 Azure 비용 검토</span><span class="sxs-lookup"><span data-stu-id="213e6-111">Review your customers' estimated Azure costs per month</span></span>
-   <span data-ttu-id="213e6-112">잘못 구성된 서비스나 사기로 추정할 수 있는 비정상적인 사용 추세 확인</span><span class="sxs-lookup"><span data-stu-id="213e6-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="213e6-113">고객과 협력하여 근본 문제를 식별하고 비용을 관리</span><span class="sxs-lookup"><span data-stu-id="213e6-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="213e6-114">귀하와 귀하의 고객이 필요하다고 생각하는 경우 예산을 더 큰 금액으로 변경</span><span class="sxs-lookup"><span data-stu-id="213e6-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="213e6-115">Azure 지출 데이터는 예상 수치이며 실제 청구 금액은 이와 다를 수 있습니다. 세금, 크레딧, 조정 또는 적용될 수 있는 기타 요금은 이 값에 반영되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="213e6-116">지출 데이터는 하루에 한 번 새로 고쳐집니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="213e6-117">귀하가 Azure Portal에서 고객의 계정 설정을 변경하지 않으면 고객은 Azure 서비스와 리소스를 계속 사용하게 되며 해당 사용 요금이 부과됩니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="213e6-118">이 기능은 샌드박스 또는 프로덕션 (TIP) 계정의 테스트에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="213e6-119">**전자 메일 알림 설정**</span><span class="sxs-lookup"><span data-stu-id="213e6-119">**Turn on email notifications**</span></span>
1.  <span data-ttu-id="213e6-120">파트너 센터 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="213e6-121">**전자 메일 받기** 옵션을 설정하여 고객이 해당 예산 중 80% 이상을 사용하는 경우 알림을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="213e6-122">그러면 Azure 청구서를 주시하는 데 도움을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="213e6-123">알림을 받을 개인의 기본 전자 메일 주소 또는 다른 전자 메일을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="213e6-124">**예산 설정**</span><span class="sxs-lookup"><span data-stu-id="213e6-124">**Set a budget**</span></span>
1.  <span data-ttu-id="213e6-125">파트너 센터 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="213e6-126">예산을 설정하려는 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="213e6-127">**월별 예산** 상자에 값을 입력하고 **적용**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="213e6-128">현재 지출을 확인하려면 이 페이지로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="213e6-129">고객 관리 페이지의 **사용량 기준 구독** 아래에서 개별 예산을 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="213e6-130">**예산 제거**</span><span class="sxs-lookup"><span data-stu-id="213e6-130">**Remove a budget**</span></span>
1.  <span data-ttu-id="213e6-131">파트너 센터 메뉴에서 **Azure 지출**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="213e6-132">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="213e6-133">**예산 제거**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-133">Select **Remove budget**.</span></span>

<span data-ttu-id="213e6-134">**항목별 비용 보기**</span><span class="sxs-lookup"><span data-stu-id="213e6-134">**See itemized costs**</span></span>
1.  <span data-ttu-id="213e6-135">파트너 센터 메뉴에서 **고객**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="213e6-136">고객 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="213e6-137">해당 고객 관리 페이지의 **사용량 기준 구독** 아래에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="213e6-138">현재 예상 사용량 및 서비스 항목별로 구분한 비용 목록을 봅니다.</span><span class="sxs-lookup"><span data-stu-id="213e6-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



