---
title: 공동 판매 추천 커넥터 문제 해결
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 공동 판매 커넥터 사용에 대한 일반적인 질문에 대한 답변을 알아봅니다. 공동 판매 커넥터 문제를 해결하는 방법에 대한 이 FAQ를 참조합니다.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148349"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="7e7db-104">공동 판매 추천 커넥터 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7e7db-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="7e7db-105">**적용 내용:** Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="7e7db-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="7e7db-106">**적절한 역할:** 조회 관리자 | CRM의 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="7e7db-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="7e7db-107">필수 구성요소에 대한 질문 및 답변</span><span class="sxs-lookup"><span data-stu-id="7e7db-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="7e7db-108">환경에 대한 평가판 공동 판매 추천 커넥터 솔루션을 사용할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="7e7db-109">테스트/스테이징 환경에 있는 경우 평가판 솔루션을 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="7e7db-110">유료 버전의 커넥터는 AppSource에서 US$ 15/월로 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="7e7db-111">유료 연결을 사용하면 하루에 10K API 호출을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="7e7db-112">커넥터는 파트너 센터 조회 API를 기반으로 하는 래퍼입니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="7e7db-113">커넥터 솔루션이 파트너 센터 또는 CRM 쪽의 기회에서 **Create** 또는 **Update** 이벤트에 대해 실행되면 API 호출이 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="7e7db-114">CRM 환경에서 섹션을 만드는 데 필요한 역할은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="7e7db-115">시스템 관리자 또는 시스템 사용자 지정자는 모든 사용자에게 변경 내용을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="7e7db-116">그러나 모든 앱 사용자는 시스템을 개인 설정할 수 있으며 일부 사용자 지정을 다른 사용자와 공유할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="7e7db-117">파트너 판매자가 파트너 센터 작업하기 위해 특별한 역할이 필요한가요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="7e7db-118">파트너 판매자에게 "조회 관리자" 역할이 할당되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="7e7db-119">자세한 내용은 [사용 권한 개요를 참조하세요.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="7e7db-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="7e7db-120">CRM 환경에서 먼저 설정해야 하는 필드는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="7e7db-121">• 통화가 사용자의 위치에 적합하고 CRM 환경에 정확하게 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="7e7db-122">• 영업 팀이 CRM 환경에 CRM 사용자로 나열되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="7e7db-123">전원 자동화 환경 만들기에 필요한 필수 구성 요소는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="7e7db-124">전원 자동화 환경을 사용 하려면 다음이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="7e7db-125">전원 자동화 라이선스가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="7e7db-126">최소 1gb의 저장소가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="7e7db-127">Salesforce 커넥터 솔루션을 사용 하려면 Dynamics 365 구독이 필요 한가요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="7e7db-128">Salesforce 커넥터 솔루션은 다른 CRM 시스템과의 동기화를 지 원하는 "Dynamics Flow" 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="7e7db-129">이 솔루션에는 Dynamics 365 인스턴스 또는 구독이 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="7e7db-130">Salesforce 솔루션을 설치 하는 동안 회사에서 기존 CD 환경을 사용한 드롭다운이 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="7e7db-131">해당 환경을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-131">You need to select that environment.</span></span> <span data-ttu-id="7e7db-132">또한 "로그인 한 사용자에 게 연결 된 Dynamics 365 조직을 찾을 수 없습니다." 라는 오류 메시지가 표시 되 면 커넥터에 대 한 새 환경을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="7e7db-133">구성에 대 한 질문과 대답</span><span class="sxs-lookup"><span data-stu-id="7e7db-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="7e7db-134">전원 자동화 플랫폼에서 흐름을 활성화 하는 동안 다음 오류가 발생 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="7e7db-135">오류: ' {"error": {"code": "WorkflowTriggerNotFound", "message": "workflow ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' 트리거 ' manual ' 트리거를 찾을 수 없습니다."}} ' 오류로 인해 Azure Resource Manager 요청이 실패 했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="7e7db-136">다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="7e7db-137">CD 연결을 삭제 한 다음 CD 연결을 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="7e7db-138">자식 흐름을 끄고 설정</span><span class="sxs-lookup"><span data-stu-id="7e7db-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="7e7db-139">솔루션을 삭제 한 다음 솔루션을 다시 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="7e7db-140">전원 자동화 플랫폼에서 파트너 센터 커넥터를 추가 하는 동안 "로그인" 오류가 발생 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="로그인을 요구 하는 오류 메시지":::

<span data-ttu-id="7e7db-142">다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="7e7db-143">파트너 센터 자격 증명을 사용 하 여 흐름 환경에 한 번 로그인 합니다 (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="7e7db-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="7e7db-144">전원 자동화 플랫폼에서 파트너 센터를 CRM 흐름으로 활성화 하는 동안 다음과 같은 오류가 표시 되 면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="업데이트 해야 하는 오류 메시지":::

<span data-ttu-id="7e7db-146">다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="7e7db-147">파트너 센터를 CRM flow로 활성화 하기 전에 먼저 다음 두 자식 흐름을 활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="7e7db-148">파트너 센터-CRM-도우미 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="7e7db-149">파트너 센터 Microsoft에서 CRM (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="7e7db-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="7e7db-150">흐름을 편집 하려고 할 때 흐름에 대 한 연결을 추가할 수 없는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="7e7db-151">흐름이 실행 되는 동안 흐름에 연결을 추가 하 고 각 흐름에 개별적으로 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="7e7db-152">흐름을 편집 하는 동안 연결을 추가 하는 대화 상자가 자동으로 열리지 않는 경우 흐름의 각 단계와 하위 단계를 개별적으로 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="7e7db-153">각 흐름을 선택 하 고 개별적으로 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="7e7db-154">흐름의 모든 단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="연결 해야 하는 단계":::

- <span data-ttu-id="7e7db-156">연결을 연결 하 고 연결을 추가 하 라는 경고 아이콘이 표시 되는 단계를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="흐름 단계별 편집":::


5. <span data-ttu-id="7e7db-158">공동 판매 된 조회 커넥터 솔루션의 흐름이 켜지 지 않으면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="7e7db-159">A.</span><span class="sxs-lookup"><span data-stu-id="7e7db-159">A.</span></span> <span data-ttu-id="7e7db-160">전원 자동화에서 다음과 같은 순서로 흐름을 편집 하 고 올바른 연결을 사용 하도록 업데이트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="7e7db-161">파트너 센터 Webhook 등록 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="7e7db-162">공동 판매 참조-Salesforce를 파트너 센터 (Insider Preview)에 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7e7db-163">파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="7e7db-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="7e7db-164">Salesforce에 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="7e7db-165">Salesforce에서 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7e7db-166">Salesforce 파트너 센터 기회(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7e7db-167">파트너 센터 Salesforce Microsoft 솔루션(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="7e7db-168">B.</span><span class="sxs-lookup"><span data-stu-id="7e7db-168">B.</span></span> <span data-ttu-id="7e7db-169">각 흐름에 대해 **사용자만 실행** 옵션을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="7e7db-170">실행 전용 사용자가 **제공하는** 대신 **연결 사용을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="흐름을 활성화하려면":::


<span data-ttu-id="7e7db-172">C.</span><span class="sxs-lookup"><span data-stu-id="7e7db-172">C.</span></span> <span data-ttu-id="7e7db-173">아래에 언급된 흐름을 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="7e7db-174">Salesforce에 대한 Microsoft 공동 판매 조회 업데이트 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="7e7db-175">Salesforce에서 파트너 센터(Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7e7db-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="7e7db-176">D.</span><span class="sxs-lookup"><span data-stu-id="7e7db-176">D.</span></span> <span data-ttu-id="7e7db-177">나머지 흐름을 모두 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="7e7db-178">E.</span><span class="sxs-lookup"><span data-stu-id="7e7db-178">E.</span></span> <span data-ttu-id="7e7db-179">흐름 파트너 센터 Webhook 등록에서 **실행을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="7e7db-180">파트너 센터 첫 번째 작업에서 **Salesforce 흐름으로** **http url을** 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="7e7db-181">이벤트 아래에서 네 가지 옵션을 Select all **등록하고** 덮어쓰기에서 **예를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="7e7db-182">실행/유지 관리와 대한 질문 및 답변</span><span class="sxs-lookup"><span data-stu-id="7e7db-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="7e7db-183">Power Automate 흐름 실행 중 오류를 해결하려면 어떻게 해야 할까요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="7e7db-184">Power Automate 흐름이 예상대로 실행되도록 하고 실행 중에 오류를 해결하려면 흐름 [오류 해결을 참조하세요.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="7e7db-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="7e7db-185">파트너 센터 또는 CRM 환경에서 제대로 동기화되지 않은 조회가 표시되면 어떻게 해야 할까요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="7e7db-186">조회 동기화의 상태를 확인하려면 **감사를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="조회를 동기화하는 방법":::

<span data-ttu-id="7e7db-188">다음 조건이 충족 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="7e7db-189">솔루션 ID는 기회의 일부로 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="7e7db-190">두 자로 된 국가 코드가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-190">Two letter country code is required.</span></span>

- <span data-ttu-id="7e7db-191">Microsoft의 도움을 기회에 대해 선택 하는 경우 고객 연락처 정보가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="7e7db-192">조회가 양방향를 동기화 하는지 확인 하는 방법</span><span class="sxs-lookup"><span data-stu-id="7e7db-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="7e7db-193">다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-193">Do the following steps:</span></span>

- <span data-ttu-id="7e7db-194">파트너 판매자는 CRM 섹션에서 **파트너 센터와 동기화** 를 사용 하도록 설정 했는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="동기화를 사용 하도록 설정 했는지 확인":::

- <span data-ttu-id="7e7db-196">판매자는 잠재 고객을 한 정하는 경우 수익 및 마감 날짜를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="7e7db-197">공동 판매 기회의 **만들기** 또는 **업데이트** 단계에서 crm ID를 제공 하지만 crm에서 해당 id를 가진 잠재 고객을 찾을 수 없는 경우 업데이트 또는 만들기는 무시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="7e7db-198">Salesforce 환경에서 조회 통화 필드가 구성 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="7e7db-199">커넥터의 연결을 끊고 조회 동기화를 누락 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="7e7db-200">시험해 볼 수 있는 몇 가지 옵션은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="7e7db-201">조회 관리자 역할이 있는 파트너 센터 사용자에 대 한 사용자 이름 또는 암호가 만료 되었는지 여부를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="7e7db-202">동기화 되지 않은 기회로 이동 하 고, 사소한 업데이트를 수행 하 고, 조회가 동기화 되었는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="7e7db-203">흐름이 실행 되 고 실패 한 경우 흐름을 선택 하 고 실패 한 실행을 다시 제출 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="7e7db-204">액세스 거부 오류가 발생 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="7e7db-205">적절 한 역할이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="7e7db-206">파트너 센터 판매자에 대 한 조회 관리자 역할</span><span class="sxs-lookup"><span data-stu-id="7e7db-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="7e7db-207">CRM 인스턴스의 시스템 관리자 또는 시스템 사용자 지정자 역할</span><span class="sxs-lookup"><span data-stu-id="7e7db-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="7e7db-208">Power 자동화 흐름 계정 사용자가 https://flow.microsoft.com 사전에 한 번 이상 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="7e7db-209">공동 판매 기회를 만드는 동안 **고객 계정 국가 코드가** 누락된 경우 어떻게 해야 할까요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="7e7db-210">CRM의 고객 계정에 ISO 2자로 된 국가 코드를 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="7e7db-211">공동 판매 기회를 만드는 동안 **솔루션 ID가 필요하다는** 오류가 표시되면 어떻게 해야 할까요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="7e7db-212">공동 판매 추천을 만들려면 Microsoft 공동 판매 준비 솔루션이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="7e7db-213">흐름 오류가 없는 경우에도 CRM에 동기화되지 않는 파트너 센터 생성된 공동 판매 기회가 표시되면 어떻게 해야 할까요?</span><span class="sxs-lookup"><span data-stu-id="7e7db-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="7e7db-214">다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-214">Do the following:</span></span>

- <span data-ttu-id="7e7db-215">파트너 센터 새 공동 판매 거래를 만든 후 Dynamics 365 흐름에 대한 파트너 센터 호출되는지 확인합니다(여러 번 호출될 수 있습니다).</span><span class="sxs-lookup"><span data-stu-id="7e7db-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="7e7db-216">흐름이 호출되면 호출된 모든 흐름을 확인하고 CRM을 업데이트할 흐름 실행을 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="7e7db-217">작업을 따르고 CRM을 업데이트했는지 또는 문제가 발생했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="7e7db-218">파트너 센터 **새 거래를** 확인하여 CRM ID로 채워지는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7e7db-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="7e7db-219">파트너 센터 실수로 거래를 **종료하지** 않았는지 확인합니다. </span><span class="sxs-lookup"><span data-stu-id="7e7db-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7e7db-220">다음 단계</span><span class="sxs-lookup"><span data-stu-id="7e7db-220">Next steps</span></span>

- [<span data-ttu-id="7e7db-221">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="7e7db-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="7e7db-222">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="7e7db-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
