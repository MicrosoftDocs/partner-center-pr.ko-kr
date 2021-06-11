---
title: Microsoft AppSource의 비공개 요금제
description: Microsoft AppSource (Azure Marketplace)에서 전용 요금제를 설정 합니다.
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008551"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="8ff49-103">Microsoft AppSource의 비공개 요금제</span><span class="sxs-lookup"><span data-stu-id="8ff49-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="8ff49-104">개인 계획은 게시자가 특정 고객에 게 사용자 지정 계획을 제공 하는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="8ff49-105">이 옵션은 현재 Microsoft AppSource에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="8ff49-106">비공개 요금제는 **이제 Get** 을 사용 하 여 작업을 호출할 수 있는 SaaS (software as a service) 제품에 대 한 appsource에서 판매 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="8ff49-107">ISV에 게 개인 요금제 요청</span><span class="sxs-lookup"><span data-stu-id="8ff49-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="8ff49-108">비공개 요금제를 AppSource에서 사용할 수 있도록 하려면 ISV에 직접 문의 하 고 사용자 지정 가격 및 기술 사양을 협상 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="8ff49-109">비공개 요금제의 조건에 동의한 후에는 ISV가 계획을 만들어 조직의 테 넌 트 ID (제공 해야 함)에 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="8ff49-110">테 넌 트 ID 찾기</span><span class="sxs-lookup"><span data-stu-id="8ff49-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="8ff49-111">AppSource의 오른쪽 위 모서리에서 계정 프로필 아이콘을 선택 하 고 **테 넌 트를 봅니다**.</span><span class="sxs-lookup"><span data-stu-id="8ff49-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="8ff49-112">테 넌 트 ID를 복사 하 여 ISV에 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="테 넌 트 ID를 찾는 방법을 보여 줍니다.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="8ff49-114">AppSource에서 비공개 요금제 찾기</span><span class="sxs-lookup"><span data-stu-id="8ff49-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="8ff49-115">ISV가 AppSource에 표시 되기 전에 새 개인 계획을 게시 한 후 최대 48 시간까지 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="8ff49-116">테 넌 트 ID와 연결 된 개인 계획을 찾으려면 AppSource의 오른쪽 위에서 **비공개 계획** (잠금 아이콘)을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="위쪽 도구 모음에서 자물쇠 아이콘 (자물쇠)을 표시 합니다.":::

<span data-ttu-id="8ff49-118">로그인 하지 않은 경우 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="8ff49-119">그런 다음 **요금제 + 가격 책정** 탭에서 테 넌 트 ID와 연결 된 비공개 요금제를 구입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="요금제 및 가격 책정 탭에서 비공개 제품을 표시 합니다.":::

<span data-ttu-id="8ff49-121">테 넌 트에 대해 비공개 요금제를 사용할 수 없는 경우 개인 계획 또는 제안이 없다는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="8ff49-122">비공개 요금제 구매</span><span class="sxs-lookup"><span data-stu-id="8ff49-122">Purchase a private plan</span></span>

<span data-ttu-id="8ff49-123">ISV는 제품 내에서 하나 이상의 비공개 계획을 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="8ff49-124">각 제품에는 공용 및 비공개 요금제가 모두 포함 될 수 있지만 비공개 요금제는 페이지의 오른쪽 위에 있는 개인 제안 아이콘 (자물쇠)에서 액세스 하는 별도의 제안 목록 페이지 아래에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="8ff49-125">**요금제 + 가격 책정** 탭에 사용 가능한 비공개 요금제가 표시 됩니다. 비공개 요금제에는 독특한 파란색 배지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="개인 제안 옆에 파란색 개인 제품 배지를 표시 합니다.":::

<span data-ttu-id="8ff49-127">선택한 계획을 구매 하려면 **지금 가져오기** 를 선택 하 고 제공 된 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="8ff49-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8ff49-128">다음 단계</span><span class="sxs-lookup"><span data-stu-id="8ff49-128">Next steps</span></span>

- [<span data-ttu-id="8ff49-129">Microsoft AppSource란?</span><span class="sxs-lookup"><span data-stu-id="8ff49-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
