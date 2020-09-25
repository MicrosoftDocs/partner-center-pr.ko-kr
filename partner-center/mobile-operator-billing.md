---
title: 모바일 운영자 대금 청구-Microsoft Store
description: Microsoft Store는이 기능을 지 원하는 모바일 운영자를 위한 지불 방법으로 모바일 운영자 요금 청구 기능을 제공 합니다.
ms.date: 05/29/2020
ms.service: partner-dashboard
ms.topic: article
ms.author: hickeys
author: hickeys
keywords: windows 10, uwp, 모바일 운영자, 모바일 청구, 모바일 운영자 요금 청구
ms.localizationpriority: medium
ms.openlocfilehash: 010451506df0d6115a8e1b4781e6fb40ab8853bb
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335755"
---
# <a name="mobile-operator-billing"></a><span data-ttu-id="c71b7-104">통신사 청구</span><span class="sxs-lookup"><span data-stu-id="c71b7-104">Mobile operator billing</span></span>

> [!NOTE]
> <span data-ttu-id="c71b7-105">지급 계정 구성, 지급 누락, 지급 보류 등을 포함하여 지급과 관련된 지원이 필요한 경우 [여기](https://developer.microsoft.com/windows/support)의 지원에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="c71b7-105">If you're looking for support regarding payouts, including configuring payout accounts, missing payouts, putting payouts on hold, or anything else, contact support [here](https://developer.microsoft.com/windows/support).</span></span>

<span data-ttu-id="c71b7-106">Microsoft Store은 Windows 10을 실행 하는 장치, Windows 10 Mobile을 실행 하는 휴대폰 및 Xbox One 콘솔에 대 한 지불 방법으로 모바일 운영자 요금 청구를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c71b7-106">The Microsoft Store offers Mobile Operator Billing as a payment method for devices running Windows 10, phones running Windows 10 Mobile, and Xbox One consoles.</span></span> <span data-ttu-id="c71b7-107">고객의 모바일 운영자가이 기능을 지 원하는 경우 고객은 지불 방법으로 모바일 운영자 대금 청구를 추가 하 고 모바일 계정을 사용 하 여 스토어 구매를 수행 하는 데 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c71b7-107">If a customer’s mobile operator supports this capability, the customer can add Mobile Operator Billing as a payment method and use it to make Store purchases using their mobile account.</span></span>

> [!TIP]
>  <span data-ttu-id="c71b7-108">고객의 모바일 운영자가 모바일 운영자 요금 청구 기능을 제공 하지만 고객이 장치에서이 옵션을 찾을 수 없는 경우 다음 [단계](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f)를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="c71b7-108">If a customer’s mobile operator offers Mobile Operator Billing, but the customer can't find this option on their device, review these [steps](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f).</span></span>

<span data-ttu-id="c71b7-109">정기적으로 모바일 운영자와 협력 하 여이 지불 방법의 가용성을 확장 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c71b7-109">We are regularly working with mobile operators to expand the availability of this payment method.</span></span> <span data-ttu-id="c71b7-110">아래에 표시 되지 않는 모바일 운영자를 제안 하려면 해당 모바일 운영자에 게 연락 하 여이 지불 방법을 추가 하도록 요청 하세요.</span><span class="sxs-lookup"><span data-stu-id="c71b7-110">If you’d like to suggest a mobile operator that you don’t see listed below, contact that mobile operator and request that they add this payment method.</span></span>

<span data-ttu-id="c71b7-111">다음 모바일 운영자는 현재 모바일 운영자 대금 청구를 지원 합니다.</span><span class="sxs-lookup"><span data-stu-id="c71b7-111">The following mobile operators currently support Mobile Operator Billing.</span></span>

| <span data-ttu-id="c71b7-112">국가/지역</span><span class="sxs-lookup"><span data-stu-id="c71b7-112">Country/region</span></span>       | <span data-ttu-id="c71b7-113">통신사</span><span class="sxs-lookup"><span data-stu-id="c71b7-113">Mobile operators</span></span>                                        |
|----------------------|---------------------------------------------------------|
| <span data-ttu-id="c71b7-114">오스트레일리아</span><span class="sxs-lookup"><span data-stu-id="c71b7-114">Australia</span></span>            | <span data-ttu-id="c71b7-115">Optus</span><span class="sxs-lookup"><span data-stu-id="c71b7-115">Optus</span></span>                                                   |
| <span data-ttu-id="c71b7-116">오스트리아</span><span class="sxs-lookup"><span data-stu-id="c71b7-116">Austria</span></span>              | <span data-ttu-id="c71b7-117">A1 Telekom, Hutchison 3G 오스트리아, T-모바일/tele-transmission</span><span class="sxs-lookup"><span data-stu-id="c71b7-117">A1 Telekom, Hutchison 3G Austria, T-Mobile / tele.ring</span></span>  |
| <span data-ttu-id="c71b7-118">벨기에</span><span class="sxs-lookup"><span data-stu-id="c71b7-118">Belgium</span></span>              | <span data-ttu-id="c71b7-119">기본, Proximus</span><span class="sxs-lookup"><span data-stu-id="c71b7-119">Base, Proximus</span></span>                                          |
| <span data-ttu-id="c71b7-120">Canada</span><span class="sxs-lookup"><span data-stu-id="c71b7-120">Canada</span></span>               | <span data-ttu-id="c71b7-121">Telus</span><span class="sxs-lookup"><span data-stu-id="c71b7-121">Telus</span></span>                                                   |
| <span data-ttu-id="c71b7-122">체코</span><span class="sxs-lookup"><span data-stu-id="c71b7-122">Czechia</span></span>              | <span data-ttu-id="c71b7-123">T-모바일</span><span class="sxs-lookup"><span data-stu-id="c71b7-123">T-Mobile</span></span>                                                |
| <span data-ttu-id="c71b7-124">덴마크</span><span class="sxs-lookup"><span data-stu-id="c71b7-124">Denmark</span></span>              | <span data-ttu-id="c71b7-125">3, TDC/., Telenor, Telia</span><span class="sxs-lookup"><span data-stu-id="c71b7-125">3, TDC / YouSee, Telenor, Telia</span></span>                         |
| <span data-ttu-id="c71b7-126">핀란드</span><span class="sxs-lookup"><span data-stu-id="c71b7-126">Finland</span></span>              | <span data-ttu-id="c71b7-127">DNA, Elisa</span><span class="sxs-lookup"><span data-stu-id="c71b7-127">DNA, Elisa</span></span>                                              |
| <span data-ttu-id="c71b7-128">프랑스</span><span class="sxs-lookup"><span data-stu-id="c71b7-128">France</span></span>               | <span data-ttu-id="c71b7-129">Orange</span><span class="sxs-lookup"><span data-stu-id="c71b7-129">Orange</span></span>                                                  |
| <span data-ttu-id="c71b7-130">독일</span><span class="sxs-lookup"><span data-stu-id="c71b7-130">Germany</span></span>              | <span data-ttu-id="c71b7-131">O2, Telekom Deutschland, Vodafone</span><span class="sxs-lookup"><span data-stu-id="c71b7-131">O2, Telekom Deutschland, Vodafone</span></span>                       |
| <span data-ttu-id="c71b7-132">헝가리</span><span class="sxs-lookup"><span data-stu-id="c71b7-132">Hungary</span></span>              | <span data-ttu-id="c71b7-133">Telenor</span><span class="sxs-lookup"><span data-stu-id="c71b7-133">Telenor</span></span>                                                 |
| <span data-ttu-id="c71b7-134">이탈리아</span><span class="sxs-lookup"><span data-stu-id="c71b7-134">Italy</span></span>                | <span data-ttu-id="c71b7-135">Tre, 바람</span><span class="sxs-lookup"><span data-stu-id="c71b7-135">Tre, Wind</span></span>                                               |
| <span data-ttu-id="c71b7-136">말레이시아</span><span class="sxs-lookup"><span data-stu-id="c71b7-136">Malaysia</span></span>             | <span data-ttu-id="c71b7-137">에서 digi</span><span class="sxs-lookup"><span data-stu-id="c71b7-137">Digi</span></span>                                                    |
| <span data-ttu-id="c71b7-138">네덜란드</span><span class="sxs-lookup"><span data-stu-id="c71b7-138">Netherlands</span></span>          | <span data-ttu-id="c71b7-139">KPN/통신 요새</span><span class="sxs-lookup"><span data-stu-id="c71b7-139">KPN / Telfort</span></span>                                           |
| <span data-ttu-id="c71b7-140">노르웨이</span><span class="sxs-lookup"><span data-stu-id="c71b7-140">Norway</span></span>               | <span data-ttu-id="c71b7-141">Telenor/Talkmore, Telia/OneCall</span><span class="sxs-lookup"><span data-stu-id="c71b7-141">Telenor / Talkmore, Telia / OneCall</span></span>                     |
| <span data-ttu-id="c71b7-142">폴란드</span><span class="sxs-lookup"><span data-stu-id="c71b7-142">Poland</span></span>               | <span data-ttu-id="c71b7-143">주황, 재생</span><span class="sxs-lookup"><span data-stu-id="c71b7-143">Orange, Play</span></span>                                            |
| <span data-ttu-id="c71b7-144">싱가포르</span><span class="sxs-lookup"><span data-stu-id="c71b7-144">Singapore</span></span>            | <span data-ttu-id="c71b7-145">M1 제한 된 StarHub</span><span class="sxs-lookup"><span data-stu-id="c71b7-145">M1 Limited, StarHub</span></span>                                     |
| <span data-ttu-id="c71b7-146">슬로바키아</span><span class="sxs-lookup"><span data-stu-id="c71b7-146">Slovakia</span></span>             | <span data-ttu-id="c71b7-147">슬로바키아어 Telekom</span><span class="sxs-lookup"><span data-stu-id="c71b7-147">Slovak Telekom</span></span>                                          |
| <span data-ttu-id="c71b7-148">남아프리카 공화국</span><span class="sxs-lookup"><span data-stu-id="c71b7-148">South Africa</span></span>         | <span data-ttu-id="c71b7-149">Vodacom</span><span class="sxs-lookup"><span data-stu-id="c71b7-149">Vodacom</span></span>                                                 |
| <span data-ttu-id="c71b7-150">스페인</span><span class="sxs-lookup"><span data-stu-id="c71b7-150">Spain</span></span>                | <span data-ttu-id="c71b7-151">Orange</span><span class="sxs-lookup"><span data-stu-id="c71b7-151">Orange</span></span>                                                  |
| <span data-ttu-id="c71b7-152">스웨덴</span><span class="sxs-lookup"><span data-stu-id="c71b7-152">Sweden</span></span>               | <span data-ttu-id="c71b7-153">3, 통신 또는</span><span class="sxs-lookup"><span data-stu-id="c71b7-153">3, Telenor</span></span>                                              |
| <span data-ttu-id="c71b7-154">스위스</span><span class="sxs-lookup"><span data-stu-id="c71b7-154">Switzerland</span></span>          | <span data-ttu-id="c71b7-155">일출, Swisscom</span><span class="sxs-lookup"><span data-stu-id="c71b7-155">Sunrise, Swisscom</span></span>                                       |
| <span data-ttu-id="c71b7-156">대만</span><span class="sxs-lookup"><span data-stu-id="c71b7-156">Taiwan</span></span>               | <span data-ttu-id="c71b7-157">FarEasTone</span><span class="sxs-lookup"><span data-stu-id="c71b7-157">FarEasTone</span></span>                                              |
| <span data-ttu-id="c71b7-158">터키</span><span class="sxs-lookup"><span data-stu-id="c71b7-158">Turkey</span></span>               | <span data-ttu-id="c71b7-159">Turkcell</span><span class="sxs-lookup"><span data-stu-id="c71b7-159">Turkcell</span></span>                                                |
| <span data-ttu-id="c71b7-160">아랍에미리트연합국</span><span class="sxs-lookup"><span data-stu-id="c71b7-160">United Arab Emirates</span></span> | <span data-ttu-id="c71b7-161">Etisalat</span><span class="sxs-lookup"><span data-stu-id="c71b7-161">Etisalat</span></span>                                                |
| <span data-ttu-id="c71b7-162">미국</span><span class="sxs-lookup"><span data-stu-id="c71b7-162">United States</span></span>        | <span data-ttu-id="c71b7-163">스 프린트, Verizon</span><span class="sxs-lookup"><span data-stu-id="c71b7-163">Sprint, Verizon</span></span>                                         |
| <span data-ttu-id="c71b7-164">영국</span><span class="sxs-lookup"><span data-stu-id="c71b7-164">United Kingdom</span></span>       | <span data-ttu-id="c71b7-165">3 영국, EE, O2, Vodaphone</span><span class="sxs-lookup"><span data-stu-id="c71b7-165">3 UK, EE, O2, Vodaphone</span></span>                                 |
