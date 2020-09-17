---
title: 인센티브 고객 제휴 문제
description: 요청 받은 레코드 파트너 (CPOR) 고객 연결을 사용할 때 발생 하는 문제를 해결 하는 방법을 알아봅니다.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: ab2c26cf097d6212375382cadd9ac5f4f80b5c2a
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/17/2020
ms.locfileid: "90714477"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a><span data-ttu-id="a9bb9-103">요청 받은 레코드 파트너 (CPOR) 고객 연결 문제</span><span class="sxs-lookup"><span data-stu-id="a9bb9-103">Issues with Claimed Partner of Record (CPOR) customer associations</span></span>

<span data-ttu-id="a9bb9-104">**적용 대상:**</span><span class="sxs-lookup"><span data-stu-id="a9bb9-104">**Applies to:**</span></span>

- <span data-ttu-id="a9bb9-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="a9bb9-105">Partner Center</span></span>

<span data-ttu-id="a9bb9-106">**적절한 역할:**</span><span class="sxs-lookup"><span data-stu-id="a9bb9-106">**Appropriate roles:**</span></span>

- <span data-ttu-id="a9bb9-107">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="a9bb9-107">Billing admin</span></span>
- <span data-ttu-id="a9bb9-108">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="a9bb9-108">Global admin</span></span>
- <span data-ttu-id="a9bb9-109">인센티브 관리자</span><span class="sxs-lookup"><span data-stu-id="a9bb9-109">Incentives admin</span></span>

<span data-ttu-id="a9bb9-110">아래 콘텐츠를 통해 고객 연결을 사용할 때 발생 하는 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-110">The content below will help you solve issues that can come up when you work with customer associations.</span></span>

## <a name="domain-tenant-mismatch"></a><span data-ttu-id="a9bb9-111">도메인-테 넌 트 불일치</span><span class="sxs-lookup"><span data-stu-id="a9bb9-111">Domain-tenant mismatch</span></span>

<span data-ttu-id="a9bb9-112">요청 받은 레코드 파트너 (CPOR) 연결 클레임 흐름에서 고객 테 넌 트 ID 및 하위 도메인을 제공 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-112">In the Claimed Partner of Record (CPOR) association claim flow, you will be asked to provide the customer tenant ID and subdomain.</span></span> <span data-ttu-id="a9bb9-113">일치 하지 않는다는 오류 메시지가 표시 되 면 고객에 게 문의 하 여 올바른 세부 정보를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-113">If you receive an error stating that they don’t match, contact your customer to ensure you have the correct details.</span></span>

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a><span data-ttu-id="a9bb9-114">CPOR association 클레임 흐름의 구독 오류</span><span class="sxs-lookup"><span data-stu-id="a9bb9-114">Subscription errors in the CPOR association claim flow</span></span>

<span data-ttu-id="a9bb9-115">CPOR association 클레임 흐름에서 Business Applications (Dynamics 365)를 통해 클레임 하려는 제품에 대 한 구독을 제공 하 라는 메시지가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-115">In the CPOR association claim flow, you may be asked to provide a subscription for a product that you're trying to claim via Business Applications (Dynamics 365).</span></span> <span data-ttu-id="a9bb9-116">제품 및 구독이에 대해 요청 되는 테 넌 트에 속하는지 여부를 동적으로 확인 하는 중 이므로 구독을 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-116">We ask for the subscription because we're dynamically checking that the product and subscription belong to the tenant being claimed for.</span></span> <span data-ttu-id="a9bb9-117">구독이 활성/유예 상태 인지 확인 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-117">We're also checking that the subscription is in active/in grace status.</span></span>

<span data-ttu-id="a9bb9-118">오류가 발생 하는 경우 다음과 같은 여러 가지 이유가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-118">If you receive the error, it could be for several reasons:</span></span>

- <span data-ttu-id="a9bb9-119">선택한 제품이 고객의 테넌트에 없음</span><span class="sxs-lookup"><span data-stu-id="a9bb9-119">The product selected doesn’t exist on the customer’s tenant</span></span>
- <span data-ttu-id="a9bb9-120">제공 된 구독은 Dynamics에 대해 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-120">The subscription provided isn't for Dynamics</span></span>
- <span data-ttu-id="a9bb9-121">제공된 구독이 CSP용임</span><span class="sxs-lookup"><span data-stu-id="a9bb9-121">The subscription provided is for CSP</span></span>
- <span data-ttu-id="a9bb9-122">고객은 해당 구독에 대 한 제품을 아직 활성화/프로 비전 하지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-122">The customer hasn't yet activated/provisioned the products for that subscription</span></span>
- <span data-ttu-id="a9bb9-123">구독이 이미 클레임됨</span><span class="sxs-lookup"><span data-stu-id="a9bb9-123">The subscription has already been claimed</span></span>
- <span data-ttu-id="a9bb9-124">제공 된 식별자가 구독 ID가 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-124">The identifier provided isn't a subscription ID</span></span>

<span data-ttu-id="a9bb9-125">구독의 정확성에 대 한 질문이 있는 경우 고객과 협력 하 여 구독이 올바르고 올바른 테 넌 트 ID를 사용 하 고 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-125">If you have a question about the accuracy of your subscription, work with your customer to ensure the subscription is correct and that you're using the correct tenant ID.</span></span>

<span data-ttu-id="a9bb9-126">이 경로에서 문제가 해결 되지 않으면 [지원](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)담당자에 게 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-126">If this route hasn't resolved your issue, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="when-subscriptions-will-be-available-to-claim"></a><span data-ttu-id="a9bb9-127">구독을 클레임에 사용할 수 있는 경우</span><span class="sxs-lookup"><span data-stu-id="a9bb9-127">When subscriptions will be available to claim</span></span>

<span data-ttu-id="a9bb9-128">구독을 요청 하는 경우 구독이 아직 프로 비전 되지 않은 경우 오류를 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-128">When claiming for a subscription, you will receive an error if the subscription hasn't been provisioned yet.</span></span> <span data-ttu-id="a9bb9-129">CPOR 플랫폼에서 구독을 선택 하 고 클레임을 제공 하는 데 사용할 수 있도록 고객이 수행 해야 하는 몇 가지 단계가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-129">There are several steps the customer needs to take for the subscription to become available for the CPOR platform to pick it up and make it available to claim.</span></span> <span data-ttu-id="a9bb9-130">구독을 요청 하는 동안 오류가 발생 하는 경우 고객에 게 연락 하 여 프로 비전 되었으며 주장 하는 구독이 올바른지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-130">If you're receiving an error when trying to claim a subscription, contact your customer to ensure that it has been provisioned and the subscription you're claiming is correct.</span></span> <span data-ttu-id="a9bb9-131">이 경로를 이미 만든 경우 [지원](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)담당자에 게 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-131">If you have taken this route already, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="which-activity-do-i-choose"></a><span data-ttu-id="a9bb9-132">어떤 작업을 선택 해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="a9bb9-132">Which activity do I choose?</span></span>

<span data-ttu-id="a9bb9-133">CPOR 클레임 플랫폼은 Business Applications 및 Microsoft 365 솔루션 영역과 관련 된 CPOR association 클레임을 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-133">The CPOR claiming platform allows for CPOR association claims related to Business Applications and Microsoft 365 solution areas.</span></span> <span data-ttu-id="a9bb9-134">각 솔루션 영역에 적용할 수 있는 작업은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-134">The activities that are applicable to each solution area are below.</span></span> <span data-ttu-id="a9bb9-135">설명에 따라 올바른 활동을 선택 하 여 나중에 회수할 필요가 없도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-135">Select the correct activity based on the descriptions to avoid having to reclaim in the future.</span></span> <span data-ttu-id="a9bb9-136">잘못 된 작업으로 주장 하면 자격 및 동기 소득이 누락 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-136">Claiming with an incorrect activity may result in missed eligibility and incentive earnings.</span></span>


| <span data-ttu-id="a9bb9-137">솔루션 영역</span><span class="sxs-lookup"><span data-stu-id="a9bb9-137">Solution area</span></span> | <span data-ttu-id="a9bb9-138">활동</span><span class="sxs-lookup"><span data-stu-id="a9bb9-138">Activity</span></span> | <span data-ttu-id="a9bb9-139">적용 가능</span><span class="sxs-lookup"><span data-stu-id="a9bb9-139">Applicable for</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="a9bb9-140">비즈니스 애플리케이션</span><span class="sxs-lookup"><span data-stu-id="a9bb9-140">Business applications</span></span>      | <span data-ttu-id="a9bb9-141">예약 판매</span><span class="sxs-lookup"><span data-stu-id="a9bb9-141">Presales</span></span>   | <span data-ttu-id="a9bb9-142">적격 제품의 구매에 영향을 준 경우 사전 판매 성과급을 적용 하려는 경우에 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-142">Select if you influenced their purchase of an eligible product, and want to apply for pre-sale incentives.</span></span> <span data-ttu-id="a9bb9-143">이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-143">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    |  <span data-ttu-id="a9bb9-144">사용량</span><span class="sxs-lookup"><span data-stu-id="a9bb9-144">Usage</span></span>  | <span data-ttu-id="a9bb9-145">적합 한 워크 로드의 도입 및 사용을 추진 하 고 사용 성과급을 적용 하려는 경우에 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-145">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> <span data-ttu-id="a9bb9-146">이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-146">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    | <span data-ttu-id="a9bb9-147">수익 연결</span><span class="sxs-lookup"><span data-stu-id="a9bb9-147">Revenue association</span></span>   | <span data-ttu-id="a9bb9-148">적격 제품의 선택에 영향을 주는 비즈니스 주는 요인은 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-148">Select if you influenced their selection of an eligible product as a Business Influencer.</span></span> <span data-ttu-id="a9bb9-149">이 옵션은 동기 지불액이 아닌 수익 연결에만 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-149">This option is for revenue association only, not for incentive payments.</span></span> <span data-ttu-id="a9bb9-150">이 옵션은 고객이 볼륨 라이선싱 계약 또는 웹 다이렉트를 통해 이러한 제품을 구매한 경우에만 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-150">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span>   |
| <span data-ttu-id="a9bb9-151">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a9bb9-151">Microsoft 365</span></span>   | <span data-ttu-id="a9bb9-152">사용량</span><span class="sxs-lookup"><span data-stu-id="a9bb9-152">Usage</span></span>   | <span data-ttu-id="a9bb9-153">적합 한 워크 로드의 도입 및 사용을 추진 하 고 사용 성과급을 적용 하려는 경우에 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-153">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> |

## <a name="which-mpn-do-i-choose"></a><span data-ttu-id="a9bb9-154">어떤 MPN를 선택 하나요?</span><span class="sxs-lookup"><span data-stu-id="a9bb9-154">Which MPN do I choose?</span></span>

<span data-ttu-id="a9bb9-155">CPOR association 클레임 흐름에서 최종 고객에 게 요청 하는 작업에 연결 해야 하는 회사 MPN을 선택 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-155">In the CPOR association claim flow, you will be asked to choose a company MPN that should be associated to the work you're claiming for at the end customer.</span></span> <span data-ttu-id="a9bb9-156">회사에는 여러 MPNs가 있을 수 있으며, 그 중 일부는 동기 프로그램에 등록 될 수 있으며, 다른 일부는 FRP FastTrack 같은 파트너 유형과 연결 되어 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-156">Your company may have many MPNs, some of which may be enrolled in incentive programs, and others associated with a partner type such as FRP FastTrack.</span></span> <span data-ttu-id="a9bb9-157">CPOR association 클레임 흐름은 동기 프로그램에 등록 된 MPNs를 식별 하지만 MPN 특정 파트너 유형인 경우에는 알 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-157">The CPOR association claim flow will identify which MPNs are enrolled in an incentive program, but it will not tell you if it is a specific partner type MPN.</span></span> <span data-ttu-id="a9bb9-158">나중에 회수할 필요가 없도록 올바른 MPN를 선택 하는 것이 중요 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-158">It’s important to select the correct MPN, to avoid having to reclaim in the future.</span></span> <span data-ttu-id="a9bb9-159">잘못 된 MPN를 사용 하 여 주장 하면 자격 및 동기 소득이 누락 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-159">Claiming with an incorrect MPN may result in missed eligibility and incentive earnings.</span></span>

<span data-ttu-id="a9bb9-160">사용할 MPN를 모르는 경우 전역 관리자에 게 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-160">If you do not know which MPN to use, contact your global admin.</span></span>

<span data-ttu-id="a9bb9-161">사용 하려는 MPN이 등록 되지 않은 경우에는 [성과급 개요 탭](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (로그인 필요)에서 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-161">If the MPN you're wanting to use isn't enrolled, you can manage that in the [Incentives overview tab](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (sign-in required).</span></span>

## <a name="choosing-a-product-vs-entering-a-subscription"></a><span data-ttu-id="a9bb9-162">제품 선택 및 구독 입력</span><span class="sxs-lookup"><span data-stu-id="a9bb9-162">Choosing a product vs entering a subscription</span></span>

<span data-ttu-id="a9bb9-163">Dynamics 제품이 요청 및 승인 되 면 파트너는 CPOR association 클레임 자체에서 구독 ID를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-163">When a Dynamics product is claimed and approved, the partner can view the subscription ID in the CPOR association claim itself.</span></span> <span data-ttu-id="a9bb9-164">이 구독을 요청 하면 활성 또는 유예 상태 이지만 구독이 종료 되는 시간이 있을 수 있으며 새 구독은 별도의 CPOR 연결 클레임에서 요청 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-164">When this subscription is claimed, it is in active or in grace status, but there may be a time when the subscription ends, and the new subscriptions will need to be claimed in a separate CPOR association claim.</span></span>

## <a name="competing-claims"></a><span data-ttu-id="a9bb9-165">경쟁 하는 클레임</span><span class="sxs-lookup"><span data-stu-id="a9bb9-165">Competing claims</span></span>

<span data-ttu-id="a9bb9-166">다른 파트너와 이미 연결 되어 있는 고객 및 해당 제품에 대 한 CPOR association 클레임을 만드는 경우 클레임은 중재를 통해 수행 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-166">If you're creating a CPOR association claim for a customer and their product(s) that is already associated with another partner, your claim will go through arbitration:</span></span>

1. <span data-ttu-id="a9bb9-167">파트너가 새 고객 연결을 만들면 Microsoft가 정확성을 보장하기 위해 제공된 연결 및 실행 증명의 세부 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-167">After you create a new customer association, Microsoft will verify the details of the association and proof of execution provided to ensure its accuracy.</span></span>

2. <span data-ttu-id="a9bb9-168">사용자와 다른 파트너가 동일한 고객 및 제품/작업을 클레임 하는 경우 Microsoft는 각 파트너의 실행 설명서를 검토 하 여 승인할 파트너를 결정 합니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-168">If you and another partner claim the same customer and product/workload, Microsoft will review each partner's proof of execution documentation to determine which partner to approve.</span></span>

3. <span data-ttu-id="a9bb9-169">두 파트너 모두에서 추가 정보를 요청할 수 있으며,이로 인해 연결 요청 처리가 지연 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-169">Additional information might be requested from both partners, which could cause delays in processing your association request.</span></span>

4. <span data-ttu-id="a9bb9-170">CPOR association 클레임은 계속 해 서 5 영업일 이내에 검토 됩니다. 단, 그 상태는 더 오랜 기간 동안 _검토_ 하는 것으로 유지 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-170">Your CPOR association claim will still be reviewed within five business days, although its status may stay as _Under Review_ for a longer period of time.</span></span> <span data-ttu-id="a9bb9-171">이 시나리오는 Microsoft가 현재 제품/워크 로드를 소유 하 고 있는 파트너와 함께 작업 하는 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-171">This scenario can happen when Microsoft works with the partner currently owning the product/workload.</span></span> <span data-ttu-id="a9bb9-172">해당 하는 경우에는 클레임의 설명 섹션에서 알림이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-172">You will be notified within the comments section of your claim if that is the case.</span></span> 

>[!IMPORTANT]
><span data-ttu-id="a9bb9-173">CPOR 연결 실행 증명 (PoE)을 확인 하는 데 추가 정보가 필요한 경우 CPOR association 클레임 설명 섹션을 통해 연락 드리겠습니다.</span><span class="sxs-lookup"><span data-stu-id="a9bb9-173">If we require additional information to verify your CPOR association proof of execution (PoE), we'll contact you via the CPOR association claim comments section.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a9bb9-174">다음 단계</span><span class="sxs-lookup"><span data-stu-id="a9bb9-174">Next steps</span></span>

- [<span data-ttu-id="a9bb9-175">인센티브 시작</span><span class="sxs-lookup"><span data-stu-id="a9bb9-175">Getting started with incentives</span></span>](incentives-get-started-intro.md)
