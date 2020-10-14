---
title: 공동 판매 추천 커넥터 문제 해결
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 공동 판매 커넥터 사용에 대 한 일반적인 질문에 대 한 대답을 알아봅니다. 공동 판매 커넥터 문제를 해결 하는 방법에 대 한 FAQ를 참조 하세요.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031266"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="e526e-104">공동 판매 추천 커넥터 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e526e-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="e526e-105">**적용 대상:**</span><span class="sxs-lookup"><span data-stu-id="e526e-105">**Applies to:**</span></span>

- <span data-ttu-id="e526e-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="e526e-106">Partner Center</span></span>
- <span data-ttu-id="e526e-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="e526e-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="e526e-108">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e526e-108">Salesforce CRM</span></span>

<span data-ttu-id="e526e-109">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="e526e-109">**Appropriate roles**</span></span>

- <span data-ttu-id="e526e-110">조회 관리자</span><span class="sxs-lookup"><span data-stu-id="e526e-110">Referrals admin</span></span>
- <span data-ttu-id="e526e-111">CRM에서 시스템 관리자 또는 시스템 사용자 지정자</span><span class="sxs-lookup"><span data-stu-id="e526e-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="e526e-112">필수 조건에 대 한 질문과 대답</span><span class="sxs-lookup"><span data-stu-id="e526e-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="e526e-113">사용자 환경에 대 한 평가판 공동 판매 조회 커넥터 솔루션을 사용할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="e526e-114">테스트/스테이징 환경을 사용할 경우 평가판 솔루션을 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="e526e-115">유료 버전의 커넥터는 AppSource에서 미국 $15/월에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="e526e-116">유료 연결을 사용 하면 하루에 10K API 호출을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="e526e-117">커넥터는 파트너 센터 조회 Api 위에 있는 래퍼입니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="e526e-118">커넥터 솔루션이 파트너 센터나 CRM 쪽의 기회에서 **만들기** 또는 **업데이트** 이벤트에 대해 실행 될 때마다 API 호출이 수행 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="e526e-119">CRM 환경에서 섹션을 만드는 데 필요한 역할은 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="e526e-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="e526e-120">시스템 관리자 또는 시스템 사용자 지정자 인 사용자는 모든 사용자에 대 한 변경 내용을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="e526e-121">그러나 모든 앱 사용자는 시스템을 개인 설정 하 고 일부 사용자 지정 항목을 다른 사용자와 공유할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="e526e-122">파트너 판매자는 파트너 센터에서 작업 하는 데 특별 한 역할이 필요 한가요?</span><span class="sxs-lookup"><span data-stu-id="e526e-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="e526e-123">파트너 판매자에 게는 "조회 관리자" 역할을 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="e526e-124">자세한 내용은 다음을 참조 하십시오. [사용 권한 개요) (사용자-계정 및 설정-권한)</span><span class="sxs-lookup"><span data-stu-id="e526e-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="e526e-125">CRM 환경에서 먼저 설정 해야 하는 필드는 무엇입니까?</span><span class="sxs-lookup"><span data-stu-id="e526e-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="e526e-126">• 통화가 사용자의 위치에 적합 하 고 CRM 환경에서 정확 하 게 사용 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="e526e-127">• 영업 팀이 crm 환경에 CRM 사용자로 나열 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="e526e-128">전원 자동화 환경 만들기에 필요한 필수 구성 요소는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="e526e-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="e526e-129">전원 자동화 환경을 사용 하려면 다음이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="e526e-130">전원 자동화 라이선스가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="e526e-131">최소 1gb의 저장소가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="e526e-132">Salesforce 커넥터 솔루션을 사용 하려면 Dynamics 365 구독이 필요 한가요?</span><span class="sxs-lookup"><span data-stu-id="e526e-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="e526e-133">Salesforce 커넥터 솔루션은 다른 CRM 시스템과의 동기화를 지 원하는 "Dynamics Flow" 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="e526e-134">이 솔루션에는 Dynamics 365 인스턴스 또는 구독이 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="e526e-135">Salesforce 솔루션을 설치 하는 동안 회사에서 기존 CD 환경을 사용한 드롭다운이 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="e526e-136">해당 환경을 선택 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-136">You need to select that environment.</span></span> <span data-ttu-id="e526e-137">또한 "로그인 한 사용자에 게 연결 된 Dynamics 365 조직을 찾을 수 없습니다." 라는 오류 메시지가 표시 되 면 커넥터에 대 한 새 환경을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="e526e-138">구성에 대 한 질문과 대답</span><span class="sxs-lookup"><span data-stu-id="e526e-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="e526e-139">전원 자동화 플랫폼에서 흐름을 활성화 하는 동안 다음 오류가 발생 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="e526e-140">오류: ' {"error": {"code": "WorkflowTriggerNotFound", "message": "workflow ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' 트리거 ' manual ' 트리거를 찾을 수 없습니다."}} ' 오류로 인해 Azure Resource Manager 요청이 실패 했습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="e526e-141">다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="e526e-142">CD 연결을 삭제 한 다음 CD 연결을 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="e526e-143">자식 흐름을 끄고 설정</span><span class="sxs-lookup"><span data-stu-id="e526e-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="e526e-144">솔루션을 삭제 한 다음 솔루션을 다시 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="e526e-145">전원 자동화 플랫폼에서 파트너 센터 커넥터를 추가 하는 동안 "로그인" 오류가 발생 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="로그인을 요구 하는 오류 메시지":::

<span data-ttu-id="e526e-147">다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="e526e-148">파트너 센터 자격 증명을 사용 하 여 흐름 환경에 한 번 로그인 합니다 (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="e526e-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="e526e-149">전원 자동화 플랫폼에서 파트너 센터를 CRM 흐름으로 활성화 하는 동안 다음과 같은 오류가 표시 되 면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="로그인을 요구 하는 오류 메시지":::

<span data-ttu-id="e526e-151">다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="e526e-152">파트너 센터를 CRM flow로 활성화 하기 전에 먼저 다음 두 자식 흐름을 활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="e526e-153">파트너 센터-CRM-도우미 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e526e-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="e526e-154">파트너 센터 Microsoft에서 CRM (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="e526e-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="e526e-155">흐름을 편집 하려고 할 때 흐름에 대 한 연결을 추가할 수 없는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="e526e-156">흐름이 실행 되는 동안 흐름에 연결을 추가 하 고 각 흐름에 개별적으로 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="e526e-157">흐름을 편집 하는 동안 연결을 추가 하는 대화 상자가 자동으로 열리지 않는 경우 흐름의 각 단계와 하위 단계를 개별적으로 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="e526e-158">각 흐름을 선택 하 고 개별적으로 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="e526e-159">흐름의 모든 단계를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="로그인을 요구 하는 오류 메시지":::

- <span data-ttu-id="e526e-161">연결을 연결 하 고 연결을 추가 하 라는 경고 아이콘이 표시 되는 단계를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="로그인을 요구 하는 오류 메시지":::


5. <span data-ttu-id="e526e-163">공동 판매 된 조회 커넥터 솔루션의 흐름이 켜지 지 않으면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="e526e-164">A.</span><span class="sxs-lookup"><span data-stu-id="e526e-164">A.</span></span> <span data-ttu-id="e526e-165">전원 자동화에서 다음과 같은 순서로 흐름을 편집 하 고 올바른 연결을 사용 하도록 업데이트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="e526e-166">파트너 센터 Webhook 등록 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e526e-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="e526e-167">공동 판매 참조-Salesforce를 파트너 센터 (Insider Preview)에 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e526e-168">파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="e526e-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e526e-169">파트너 센터를 Salesforce로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e526e-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e526e-170">Salesforce에서 파트너 센터로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e526e-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e526e-171">Salesforce 기회와 파트너 센터 간 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e526e-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e526e-172">파트너 센터 (Insider Preview)에 대 한 Salesforce Microsoft 솔루션</span><span class="sxs-lookup"><span data-stu-id="e526e-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="e526e-173">B.</span><span class="sxs-lookup"><span data-stu-id="e526e-173">B.</span></span> <span data-ttu-id="e526e-174">각 흐름에 대해 **실행만 사용자** 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="e526e-175">**실행 전용 사용자가 제공 하**는 대신 **연결 사용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-175">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="로그인을 요구 하는 오류 메시지":::


<span data-ttu-id="e526e-177">C.</span><span class="sxs-lookup"><span data-stu-id="e526e-177">C.</span></span> <span data-ttu-id="e526e-178">아래에서 언급 한 흐름을 활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="e526e-179">파트너 센터 Microsoft가 Salesforce (Insider Preview)에 대 한 조회 업데이트를 공동 판매</span><span class="sxs-lookup"><span data-stu-id="e526e-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="e526e-180">Salesforce에서 파트너 센터로 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e526e-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="e526e-181">D.</span><span class="sxs-lookup"><span data-stu-id="e526e-181">D.</span></span> <span data-ttu-id="e526e-182">나머지 흐름을 모두 활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="e526e-183">E.</span><span class="sxs-lookup"><span data-stu-id="e526e-183">E.</span></span> <span data-ttu-id="e526e-184">Flow 파트너 센터 Webhook 등록에서 **실행**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-184">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="e526e-185">**파트너 센터** 의 첫 번째 작업에서 Salesforce 흐름으로의 **http url** 을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="e526e-186">**등록할 이벤트** 에서 네 가지 옵션을 모두 선택 하 고 덮어쓰기에 대해 **예** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="e526e-187">실행/유지 관리에 대 한 질문과 대답</span><span class="sxs-lookup"><span data-stu-id="e526e-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="e526e-188">전원 자동화 흐름을 실행 하는 동안 오류가 발생 하는 경우 문제를 어떻게 해결 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="e526e-189">전원 자동화 흐름이 기대한 대로 실행 되도록 하 고 실행 중에 오류를 해결 하려면 [흐름 오류 수정](/power-automate/fix-flow-failures)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e526e-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="e526e-190">파트너 센터 또는 CRM 환경에서 제대로 동기화 되지 않는 조회가 표시 되는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="e526e-191">조회 동기화 상태를 확인 하려면 **감사**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-191">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="로그인을 요구 하는 오류 메시지":::

<span data-ttu-id="e526e-193">다음 조건이 충족 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="e526e-194">솔루션 id는 기회의 일부로 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="e526e-195">두 자로 된 국가 코드가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-195">Two letter country code is required.</span></span>

- <span data-ttu-id="e526e-196">Microsoft의 도움을 기회에 대해 선택 하는 경우 고객 연락처 정보가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="e526e-197">조회가 양방향를 동기화 하는지 확인 하는 방법</span><span class="sxs-lookup"><span data-stu-id="e526e-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="e526e-198">다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-198">Do the following steps:</span></span>

- <span data-ttu-id="e526e-199">파트너 판매자는 CRM 섹션에서 **파트너 센터와 동기화** 를 사용 하도록 설정 했는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="로그인을 요구 하는 오류 메시지":::

- <span data-ttu-id="e526e-201">판매자는 잠재 고객을 한 정하는 경우 수익 및 마감 날짜를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="e526e-202">공동 판매 기회의 **만들기** 또는 **업데이트** 단계에서 crm ID를 제공 하지만 crm에서 해당 id를 가진 잠재 고객을 찾을 수 없는 경우 업데이트 또는 만들기는 무시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="e526e-203">Salesforce 환경에서 조회 통화 필드가 구성 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="e526e-204">커넥터의 연결을 끊고 조회 동기화를 누락 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="e526e-205">시험해 볼 수 있는 몇 가지 옵션은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="e526e-206">조회 관리자 역할이 있는 파트너 센터 사용자에 대 한 사용자 이름 또는 암호가 만료 되었는지 여부를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="e526e-207">동기화 되지 않은 기회로 이동 하 고, 사소한 업데이트를 수행 하 고, 조회가 동기화 되었는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="e526e-208">흐름이 실행 되 고 실패 한 경우 흐름을 선택 하 고 실패 한 실행을 다시 제출 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="e526e-209">액세스 거부 오류가 발생 하는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="e526e-210">적절 한 역할이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="e526e-211">파트너 센터 판매자에 대 한 조회 관리자 역할</span><span class="sxs-lookup"><span data-stu-id="e526e-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="e526e-212">CRM 인스턴스의 시스템 관리자 또는 시스템 사용자 지정자 역할</span><span class="sxs-lookup"><span data-stu-id="e526e-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="e526e-213">Power 자동화 흐름 계정 사용자가 https://flow.microsoft.com 사전에 한 번 이상 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="e526e-214">공동 판매 기회를 만드는 동안 **고객 계정 국가 코드가** 누락 되는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="e526e-215">CRM의 고객 계정에 ISO 2 자로 된 국가 번호를 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="e526e-216">공동 판매 기회를 만드는 동안 **솔루션 ID가 필요** 하다는 오류가 표시 되 면 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="e526e-217">공동 판매 조회를 만들려면 Microsoft 공동 판매 준비 솔루션이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="e526e-218">흐름 오류가 없더라도 CRM에 동기화 되지 않은 파트너 센터에서 만든 공동 판매 기회가 표시 되는 경우 어떻게 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="e526e-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="e526e-219">다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-219">Do the following:</span></span>

- <span data-ttu-id="e526e-220">파트너 센터에서 새 공동 판매 거래를 만든 후에는 파트너 센터가 Dynamics 365 flow를 호출 하는지 확인 합니다 (여러 번 호출 될 수 있음).</span><span class="sxs-lookup"><span data-stu-id="e526e-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="e526e-221">흐름이 호출 되 면 호출 된 모든 흐름을 확인 하 고 CRM을 업데이트 하는 흐름 실행을 식별 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="e526e-222">작업을 수행 하 여 CRM을 업데이트 했거나 문제가 발생 했는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="e526e-223">파트너 센터에서 \*새 거래\*\*를 확인 하 여 CRM ID로 채워져 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-223">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="e526e-224">거래 센터에서 "성공" 또는 "손실"로 인해 실수로 닫히지 않았는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e526e-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e526e-225">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e526e-225">Next steps</span></span>

- [<span data-ttu-id="e526e-226">잠재 고객 관리</span><span class="sxs-lookup"><span data-stu-id="e526e-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="e526e-227">공동 판매 기회 관리</span><span class="sxs-lookup"><span data-stu-id="e526e-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)