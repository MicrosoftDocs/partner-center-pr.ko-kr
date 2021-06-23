---
title: 제한된 직접 청구 기능
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP(클라우드 솔루션 공급자) 직접 청구 파트너 요구 사항 및 기능이 제한되지 않도록 하기 위해 수행할 작업을 알아봅니다. 기능이 제한되었는지 확인합니다.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551421"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a><span data-ttu-id="8ee7b-104">제한된 직접 청구 기능 및 CSP 직접 청구 파트너에 필요한 요구 사항</span><span class="sxs-lookup"><span data-stu-id="8ee7b-104">Restricted direct bill capabilities and the requirements needed for CSP direct bill partners</span></span>

<span data-ttu-id="8ee7b-105">**적절한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="8ee7b-105">**Appropriate roles**: Global admin</span></span>

## <a name="overview"></a><span data-ttu-id="8ee7b-106">개요</span><span class="sxs-lookup"><span data-stu-id="8ee7b-106">Overview</span></span>

<span data-ttu-id="8ee7b-107">직접 청구 파트너는 CSP(클라우드 솔루션 공급자) 직접 청구 파트너 프로그램에 남아 있는 새로운 [요구 사항을](direct-partner-new-requirements.md) 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-107">Direct bill partners must meet the new [requirements](direct-partner-new-requirements.md) to remain in the Cloud Solution Provider (CSP) direct bill partner program.</span></span> <span data-ttu-id="8ee7b-108">충족하지 못하면 직접 청구 기능에 대한 액세스 권한이 제한되며 고객의 신규 구매와 같은 특정 작업을 더 이상 수행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-108">Otherwise, their access to direct bill capabilities will eventually be restricted and can longer perform specific tasks, such as making new purchases for their customers.</span></span>

> [!Note]
> <span data-ttu-id="8ee7b-109">CSP 직접 청구 파트너 프로그램에 대한 새로운 요구 사항을 충족하지 않는 직접 청구 파트너는 직접 청구 기능이 제한될 때 Microsoft에서 알 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-109">Direct bill partners who do not meet the new requirements for CSP direct bill partner program will be informed by Microsoft when their direct bill capabilities will be restricted.</span></span> <span data-ttu-id="8ee7b-110">이는 직접 청구 파트너에서 간접 대리점으로의 전환을 선택했는지 여부에 관계없이 모든 [직접 청구 파트너에게 적용됩니다.](transition-direct-to-indirect.md)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-110">This applies to all direct bill partners, whether they have opted for [transition from direct bill partner to indirect resellers](transition-direct-to-indirect.md) or not.</span></span>  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a><span data-ttu-id="8ee7b-111">직접 청구 기능이 제한되었는지를 알려주는 방법</span><span class="sxs-lookup"><span data-stu-id="8ee7b-111">How to tell if your direct bill capabilities has been restricted</span></span>

<span data-ttu-id="8ee7b-112">직접 청구 파트너 테넌트에서 직접 청구 기능으로의 액세스가 제한되었는지 확인하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-112">To confirm whether access from the direct bill partner tenant to direct bill capabilities has been restricted, follow these steps.</span></span>

1. <span data-ttu-id="8ee7b-113">[파트너 센터 대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-113">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8ee7b-114">계정 **설정** 법적 프로필 로  >  이동합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-114">Go to **Account settings** > **Legal Profile**.</span></span>

3. <span data-ttu-id="8ee7b-115">**프로그램 정보** 에서 **Microsoft 클라우드 솔루션 공급자 상태를** 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-115">Under **Program info**, look for **Microsoft Cloud Solution Provider status**.</span></span>

4. <span data-ttu-id="8ee7b-116">프로그램 상태에 값이 **제한된** 경우 직접 청구 파트너 테넌트의 직접 청구 기능에 대한 액세스가 제한되었습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-116">If the program status has value **restricted**, it means that your direct bill partner tenant's access to direct bill capabilities has been restricted.</span></span>

## <a name="affected-direct-bill-capabilities"></a><span data-ttu-id="8ee7b-117">영향을 받는 직접 청구 기능</span><span class="sxs-lookup"><span data-stu-id="8ee7b-117">Affected direct bill capabilities</span></span>

<span data-ttu-id="8ee7b-118">직접 청구 기능이 제한된 경우 더 이상 파트너 센터 고객을 위해 새 구매를 할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-118">If your direct bill capabilities have been restricted, you can no longer make new purchases for your customers in Partner Center.</span></span> <span data-ttu-id="8ee7b-119">이 제한에는 다음이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-119">This restriction includes:</span></span>

- <span data-ttu-id="8ee7b-120">Azure 구독</span><span class="sxs-lookup"><span data-stu-id="8ee7b-120">Azure subscriptions</span></span>

- <span data-ttu-id="8ee7b-121">라이선스 기반 구독</span><span class="sxs-lookup"><span data-stu-id="8ee7b-121">License-based subscriptions</span></span>

- <span data-ttu-id="8ee7b-122">기존 라이선스 기반 구독에 새 추가 기능 추가</span><span class="sxs-lookup"><span data-stu-id="8ee7b-122">Add new add-ons to existing license-based subscriptions.</span></span>

- <span data-ttu-id="8ee7b-123">소프트웨어 및 예약 제품(예: 소프트웨어 구독, 영구 소프트웨어 및 Azure Reserved Virtual Machine 인스턴스)을 한 번 구매합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-123">Make one-time purchases of software and reservation products (for example, software subscriptions, perpetual software, and Azure Reserved Virtual Machine instances).</span></span>

<span data-ttu-id="8ee7b-124">또한 CSP 프로그램에서 [Azure 파트너 공유 서비스 제안을](shared-services.md) 사용하여 사용자 고유의 용도로 새 Azure 구독을 구매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-124">You also cannot use the [Azure partner shared services offer](shared-services.md) under the CSP program to purchase new Azure subscriptions for your own use.</span></span>

<span data-ttu-id="8ee7b-125">기존 직접 청구 구독은 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-125">Existing direct bill subscriptions are not affected.</span></span> <span data-ttu-id="8ee7b-126">유효한 상태로 유지되고 자동 새로 고침됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-126">They remain valid and are autorenewed.</span></span> <span data-ttu-id="8ee7b-127">취소될 때까지 Microsoft에서 직접 요금이 계속 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-127">You will continue to be billed directly by Microsoft until they are canceled.</span></span> <span data-ttu-id="8ee7b-128">다음과 같은 방법으로 기존 구독을 계속 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-128">You can still manage existing subscriptions in the following ways:</span></span>

- <span data-ttu-id="8ee7b-129">기존 구독 일시 중단</span><span class="sxs-lookup"><span data-stu-id="8ee7b-129">Suspend existing subscriptions</span></span>

- <span data-ttu-id="8ee7b-130">기존 라이선스 기반 구독의 라이선스 수 조정</span><span class="sxs-lookup"><span data-stu-id="8ee7b-130">Adjust license count of existing license-based subscriptions</span></span>

- <span data-ttu-id="8ee7b-131">구독에 대한 기존 추가 기능의 라이선스 수를 조정합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-131">Adjust license count of existing add-ons to a subscription.</span></span> 

    >[!Note]
    ><span data-ttu-id="8ee7b-132">새 구매로 처리되는 기존 구독에는 새 추가 기능 을 추가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-132">You cannot add new add-ons to existing subscriptions as it is treated as new purchase.</span></span>

- <span data-ttu-id="8ee7b-133">새 Azure 리소스를 배포하고 기존 Azure 구독에서 기존 Azure 리소스를 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-133">Deploy new Azure resources and manage existing Azure resources under existing Azure subscriptions.</span></span> <span data-ttu-id="8ee7b-134">여기에는 Azure Marketplace 및 Visual Studio 구독을 통해 사용할 수 있는 리소스가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-134">This includes resources, which are available through Azure Marketplace and Visual Studio subscriptions.</span></span>

<span data-ttu-id="8ee7b-135">새 구매 외에도 파트너 센터 다음과 같은 직접 청구 기능에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-135">In addition to new purchases, you cannot access the following direct bill capabilities in Partner Center:</span></span>

- <span data-ttu-id="8ee7b-136">새 고객 테넌트는 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-136">You cannot create new customer tenants.</span></span> <span data-ttu-id="8ee7b-137">파트너 센터 **고객** 페이지에서 **고객 만들기** 옵션을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-137">The **Create customer** option under **Customers** page in Partner Center will not be available.</span></span>

- <span data-ttu-id="8ee7b-138">직접 대리점 관계를 요청하는 고객에게 초대를 생성할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-138">You cannot generate invitation to customer requesting for direct reseller relationship.</span></span> <span data-ttu-id="8ee7b-139">파트너 센터 **고객** 페이지의 **대리점 관계 요청** 옵션을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-139">The **Request a reseller relationship** option under **Customers** page in Partner Center will not be available.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8ee7b-140">직접 청구 파트너에서 간접 대리점으로 전환하는 과정의 일환으로 직접 청구 파트너 테넌트를 간접 대리점으로 이미 등록한 경우 간접 대리점 관계를 요청하는 고객에게 초대를 대신 생성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-140">As part of transitioning from direct bill partner to indirect reseller, if you have already enrolled your direct bill partner tenant as indirect reseller, you can generate invitation to customer requesting for indirect reseller relationship instead.</span></span>

- <span data-ttu-id="8ee7b-141">새 샌드박스 테넌트는 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-141">You cannot create new sandbox tenant.</span></span> <span data-ttu-id="8ee7b-142">각 직접 청구 파트너 테넌트는 직접 청구 API 통합을 위해 하나의 샌드박스 테넌트만 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-142">Each direct bill partner tenant can create one sandbox tenant for direct bill API integration.</span></span> <span data-ttu-id="8ee7b-143">이전에 만들지 않은 경우 직접 청구 파트너 기능이 제한된 후에는 만들 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-143">If you haven't created one previously, you are not allowed to do so after your direct bill partner capability has been restricted.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="8ee7b-144">다음 단계</span><span class="sxs-lookup"><span data-stu-id="8ee7b-144">Next steps</span></span>

- [<span data-ttu-id="8ee7b-145">간접 재판매인이 되기 위한 추가 정보</span><span class="sxs-lookup"><span data-stu-id="8ee7b-145">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [<span data-ttu-id="8ee7b-146">CSP 직접 파트너 새로운 요구 사항</span><span class="sxs-lookup"><span data-stu-id="8ee7b-146">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
