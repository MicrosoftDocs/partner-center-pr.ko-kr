---
title: Azure Marketplace 프라이빗 제안
description: Azure Marketplace 프라이빗 제안에 대해 알아봅니다.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534146"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="eaec5-103">Azure Marketplace 프라이빗 계획</span><span class="sxs-lookup"><span data-stu-id="eaec5-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="eaec5-104">프라이빗 플랜은 게시자가 특정 고객에게 사용자 지정 플랜을 제공하는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="eaec5-105">프라이빗 플랜은 Azure Portal 구매하여 직접 설치할 수 있는 유료 제안에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="eaec5-106">게시자는 포털에서 설치할 수 있는지 여부에 관계없이  컨설팅 서비스, 연락처를 호출로 연락하는 서비스 또는 무료 서비스에 대한 프라이빗 플랜을 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="eaec5-107">Azure Portal 프라이빗 플랜 찾기</span><span class="sxs-lookup"><span data-stu-id="eaec5-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="eaec5-108">파트너가 프라이빗 플랜을 게시하면 Azure Portal **Marketplace** 섹션에서 적격 사용자에게만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="eaec5-109">이러한 사용자는 제품 유형에 따라 구독 ID 또는 테넌트 ID로 정의됩니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="eaec5-110">프라이빗 플랜에 적합한 경우 포털에서 두 가지 방법으로 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="eaec5-111">프라이빗 플랜은 검색할 수 있지만 Azure Portal 필터링할 수 없습니다(범주별).</span><span class="sxs-lookup"><span data-stu-id="eaec5-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="eaec5-112">Azure Portal **+ 리소스 만들기를** 선택하거나 "마켓플레이스"를 검색하여 **Marketplace** 페이지로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="eaec5-113">프라이빗 플랜을 사용할 수 있는 경우 페이지 맨 위에 **프라이빗 플랜 사용 가능** 배너가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="eaec5-114">**프라이빗 제안 보기 + 플랜을** 선택하여 프라이빗 플랜 페이지로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="프라이빗 플랜을 사용할 수 있는 경우 표시되는 배너입니다.":::

## <a name="review-private-plans"></a><span data-ttu-id="eaec5-116">프라이빗 플랜 검토</span><span class="sxs-lookup"><span data-stu-id="eaec5-116">Review private plans</span></span>

<span data-ttu-id="eaec5-117">프라이빗 플랜은 제안의 여러 계획에 속합니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="eaec5-118">각 제안에는 여러 플랜(퍼블릭 및 프라이빗)이 있을 수 있지만 프라이빗 플랜은 퍼블릭 플랜과 별도의 목록에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="eaec5-119">고유한 프라이빗 배지로 표시된 계획 탭에서 사용 가능한 **프라이빗** **플랜을** 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="프라이빗으로 표시된 계획의 페이지입니다.":::

<span data-ttu-id="eaec5-121">구독이 두 개 이상인 경우 모든 구독에 사용할 수 있는 모든 프라이빗 플랜이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="eaec5-122">**만들기를** 선택하면 리소스 만들기 페이지로 라우팅되어 리소스 구성을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="eaec5-123">**만들기를** 선택하고 여러 구독이 있지만 모두 프라이빗 플랜에 추가되는 것은 아닌 경우 기본 구독이 이 프라이빗 플랜에 적합한 구독이 아닐 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="eaec5-124">이 경우 올바른 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="eaec5-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="더 많은 프라이빗 플랜을 사용할 수 있음을 보여주는 링크입니다.":::

## <a name="next-steps"></a><span data-ttu-id="eaec5-126">다음 단계</span><span class="sxs-lookup"><span data-stu-id="eaec5-126">Next steps</span></span>

- [<span data-ttu-id="eaec5-127">Azure Marketplace란 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="eaec5-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
