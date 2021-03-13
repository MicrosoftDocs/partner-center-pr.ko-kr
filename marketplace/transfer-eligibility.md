---
title: 전송 자격 – 청구 계정 간에 구독을 전송 하기 위한 지침 Azure Marketplace
description: Azure Portal에서 청구 계정 간에 구독을 전송 하기 전에 상업적 검사에 대 한 지침입니다.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412559"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="3777f-103">청구 계정 간 구독에 대 한 자격 전송</span><span class="sxs-lookup"><span data-stu-id="3777f-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="3777f-104">Azure Portal의 청구 섹션에서 한 청구 계정에서 다른 계정으로 [구독을 전송할](/azure/cost-management-billing/understand/subscription-transfer) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="3777f-105">전송 전에는 타사 제품에 대 한 구독이 검색 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="3777f-106">전송은 *모든* 제품을 이전에 삭제 한 경우에만 허용 됩니다 (아래 [조건을](#criteria-for-transfer-approval-or-denial) 참조).</span><span class="sxs-lookup"><span data-stu-id="3777f-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="3777f-107">시스템은 다음 단계를 결정 하는 데 도움이 되도록 지우지 못한 앱에 대 한 관련 오류 메시지를 생성 합니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="3777f-108">SaaS 리소스는 구독이 아닌 테 넌 트에 연결 되어 있으므로이 문서는 SaaS 제품에는 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="3777f-109">SaaS 리소스는 한 청구 계정에서 다른 요금으로 전송할 수 있지만이는 리소스 및 Azure 지원에서 지원 요청으로 수행 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="3777f-110">전송 승인 또는 거부 조건</span><span class="sxs-lookup"><span data-stu-id="3777f-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="3777f-111">다음 조건 중 하나를 충족 하는 타사 앱이 있으면 구독을 전송할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="3777f-112">대상 계정은 상업적 이며 앱은 파트너를 통해 판매 되도록 옵트아웃 (opt out) 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="3777f-113">앱이 선택한 파트너에 대해 옵트인 (opt in) 되 고 대상 계정이 허용 목록에 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="3777f-114">제품은 이전에 선택한 구독에 대 한 미리 보기 제품 이거나 비공개 제품 이며 구독은 더 이상 허용 목록에 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="3777f-115">새 청구 계정은 제품이 판매 되는 위치와 다른 지역에 있으며 제품을 해당 지역에서 판매 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="3777f-116">차단 된 전송은 구독에서 리소스를 제거할 때까지 계속 적용 되며, 그 후에는 전송을 다시 시도할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3777f-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3777f-117">다음 단계</span><span class="sxs-lookup"><span data-stu-id="3777f-117">Next steps</span></span>

[<span data-ttu-id="3777f-118">Microsoft AppSource 및 Azure Marketplace에 대 한 지원 받기</span><span class="sxs-lookup"><span data-stu-id="3777f-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

