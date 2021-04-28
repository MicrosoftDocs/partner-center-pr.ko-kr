---
title: 모바일 운영자 대금 청구-Microsoft Store
description: Microsoft Store는이 기능을 지 원하는 모바일 운영자를 위한 지불 방법으로 모바일 운영자 요금 청구 기능을 제공 합니다.
ms.date: 04/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.topic: article
ms.author: hickeys
author: hickeys
keywords: windows 10, uwp, 모바일 운영자, 모바일 청구, 모바일 운영자 요금 청구
ms.localizationpriority: medium
ms.openlocfilehash: 20ce286814682277e375894e99f947d084206246
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172390"
---
# <a name="mobile-operator-billing"></a><span data-ttu-id="17d84-104">통신사 청구</span><span class="sxs-lookup"><span data-stu-id="17d84-104">Mobile operator billing</span></span>

<span data-ttu-id="17d84-105">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="17d84-105">**Appropriate roles**</span></span>

- <span data-ttu-id="17d84-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="17d84-106">Global admin</span></span>

> [!NOTE]
> <span data-ttu-id="17d84-107">지급 계정 구성, 지급 누락, 지급 보류 등을 포함하여 지급과 관련된 지원이 필요한 경우 [여기](https://developer.microsoft.com/windows/support)의 지원에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="17d84-107">If you're looking for support regarding payouts, including configuring payout accounts, missing payouts, putting payouts on hold, or anything else, contact support [here](https://developer.microsoft.com/windows/support).</span></span>

<span data-ttu-id="17d84-108">Microsoft Store은 Windows 10을 실행 하는 장치, Windows 10 Mobile을 실행 하는 휴대폰 및 Xbox One 콘솔에 대 한 지불 방법으로 모바일 운영자 요금 청구를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="17d84-108">The Microsoft Store offers mobile operator billing as a payment method for devices running Windows 10, phones running Windows 10 Mobile, and Xbox One consoles.</span></span> <span data-ttu-id="17d84-109">고객의 모바일 운영자가이 기능을 지 원하는 경우 고객은 지불 방법으로 모바일 운영자 대금 청구를 추가 하 고 모바일 계정을 사용 하 여 스토어 구매를 수행 하는 데 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d84-109">If a customer’s mobile operator supports this capability, the customer can add mobile operator billing as a payment method and use it to make Store purchases using their mobile account.</span></span>

> [!TIP]
> <span data-ttu-id="17d84-110">고객의 모바일 운영자가 모바일 운영자 요금 청구 기능을 제공 하지만 고객이 장치에서이 옵션을 찾을 수 없는 경우 다음 [단계](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f)를 검토 합니다.</span><span class="sxs-lookup"><span data-stu-id="17d84-110">If a customer’s mobile operator offers mobile operator billing, but the customer can't find this option on their device, review these [steps](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f).</span></span>

<span data-ttu-id="17d84-111">정기적으로 모바일 운영자와 협력 하 여이 지불 방법의 가용성을 확장 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d84-111">We are regularly working with mobile operators to expand the availability of this payment method.</span></span> <span data-ttu-id="17d84-112">아래에 표시 되지 않는 모바일 운영자를 제안 하려면 해당 모바일 운영자에 게 연락 하 여이 지불 방법을 추가 하도록 요청 하세요.</span><span class="sxs-lookup"><span data-stu-id="17d84-112">If you’d like to suggest a mobile operator that you don’t see listed below, contact that mobile operator and request that they add this payment method.</span></span>

## <a name="operators-that-support-mobile-operator-billing"></a><span data-ttu-id="17d84-113">모바일 운영자 요금 청구를 지 원하는 운영자</span><span class="sxs-lookup"><span data-stu-id="17d84-113">Operators that support mobile operator billing</span></span>

<span data-ttu-id="17d84-114">다음 모바일 운영자는 현재 모바일 운영자 대금 청구를 지원 합니다.</span><span class="sxs-lookup"><span data-stu-id="17d84-114">The following mobile operators currently support mobile operator billing.</span></span>

| <span data-ttu-id="17d84-115">국가/지역</span><span class="sxs-lookup"><span data-stu-id="17d84-115">Country/region</span></span>       | <span data-ttu-id="17d84-116">통신사</span><span class="sxs-lookup"><span data-stu-id="17d84-116">Mobile operators</span></span>                                        |
|----------------------|---------------------------------------------------------|
| <span data-ttu-id="17d84-117">오스트레일리아</span><span class="sxs-lookup"><span data-stu-id="17d84-117">Australia</span></span>            | <span data-ttu-id="17d84-118">Optus</span><span class="sxs-lookup"><span data-stu-id="17d84-118">Optus</span></span>                                                   |
| <span data-ttu-id="17d84-119">오스트리아</span><span class="sxs-lookup"><span data-stu-id="17d84-119">Austria</span></span>              | <span data-ttu-id="17d84-120">A1 Telekom, Hutchison 3G 오스트리아, T-모바일/tele-transmission</span><span class="sxs-lookup"><span data-stu-id="17d84-120">A1 Telekom, Hutchison 3G Austria, T-Mobile / tele.ring</span></span>  |
| <span data-ttu-id="17d84-121">벨기에</span><span class="sxs-lookup"><span data-stu-id="17d84-121">Belgium</span></span>              | <span data-ttu-id="17d84-122">기본, Proximus</span><span class="sxs-lookup"><span data-stu-id="17d84-122">Base, Proximus</span></span>                                          |
| <span data-ttu-id="17d84-123">캐나다</span><span class="sxs-lookup"><span data-stu-id="17d84-123">Canada</span></span>               | <span data-ttu-id="17d84-124">Telus</span><span class="sxs-lookup"><span data-stu-id="17d84-124">Telus</span></span>                                                   |
| <span data-ttu-id="17d84-125">체코</span><span class="sxs-lookup"><span data-stu-id="17d84-125">Czechia</span></span>              | <span data-ttu-id="17d84-126">T-모바일, Vodafone, O2</span><span class="sxs-lookup"><span data-stu-id="17d84-126">T-Mobile, Vodafone, O2</span></span>                                  |
| <span data-ttu-id="17d84-127">덴마크</span><span class="sxs-lookup"><span data-stu-id="17d84-127">Denmark</span></span>              | <span data-ttu-id="17d84-128">3, TDC/., Telenor, Telia</span><span class="sxs-lookup"><span data-stu-id="17d84-128">3, TDC / YouSee, Telenor, Telia</span></span>                         |
| <span data-ttu-id="17d84-129">핀란드</span><span class="sxs-lookup"><span data-stu-id="17d84-129">Finland</span></span>              | <span data-ttu-id="17d84-130">DNA, Elisa</span><span class="sxs-lookup"><span data-stu-id="17d84-130">DNA, Elisa</span></span>                                              |
| <span data-ttu-id="17d84-131">프랑스</span><span class="sxs-lookup"><span data-stu-id="17d84-131">France</span></span>               | <span data-ttu-id="17d84-132">Orange</span><span class="sxs-lookup"><span data-stu-id="17d84-132">Orange</span></span>                                                  |
| <span data-ttu-id="17d84-133">독일</span><span class="sxs-lookup"><span data-stu-id="17d84-133">Germany</span></span>              | <span data-ttu-id="17d84-134">O2, Telekom Deutschland, Vodafone</span><span class="sxs-lookup"><span data-stu-id="17d84-134">O2, Telekom Deutschland, Vodafone</span></span>                       |
| <span data-ttu-id="17d84-135">헝가리</span><span class="sxs-lookup"><span data-stu-id="17d84-135">Hungary</span></span>              | <span data-ttu-id="17d84-136">Telenor</span><span class="sxs-lookup"><span data-stu-id="17d84-136">Telenor</span></span>                                                 |
| <span data-ttu-id="17d84-137">이탈리아</span><span class="sxs-lookup"><span data-stu-id="17d84-137">Italy</span></span>                | <span data-ttu-id="17d84-138">Tre, 바람, Vodafone</span><span class="sxs-lookup"><span data-stu-id="17d84-138">Tre, Wind, Vodafone</span></span>                                     |
| <span data-ttu-id="17d84-139">한국</span><span class="sxs-lookup"><span data-stu-id="17d84-139">Korea</span></span>                | <span data-ttu-id="17d84-140">가 나 통신</span><span class="sxs-lookup"><span data-stu-id="17d84-140">SK Telecom</span></span>                                              |
| <span data-ttu-id="17d84-141">말레이시아</span><span class="sxs-lookup"><span data-stu-id="17d84-141">Malaysia</span></span>             | <span data-ttu-id="17d84-142">에서 digi</span><span class="sxs-lookup"><span data-stu-id="17d84-142">Digi</span></span>                                                    |
| <span data-ttu-id="17d84-143">네덜란드</span><span class="sxs-lookup"><span data-stu-id="17d84-143">Netherlands</span></span>          | <span data-ttu-id="17d84-144">KPN/통신 요새, Vodafone</span><span class="sxs-lookup"><span data-stu-id="17d84-144">KPN / Telfort, Vodafone</span></span>                                 |
| <span data-ttu-id="17d84-145">노르웨이</span><span class="sxs-lookup"><span data-stu-id="17d84-145">Norway</span></span>               | <span data-ttu-id="17d84-146">Telenor/Talkmore, Telia/OneCall</span><span class="sxs-lookup"><span data-stu-id="17d84-146">Telenor / Talkmore, Telia / OneCall</span></span>                     |
| <span data-ttu-id="17d84-147">폴란드</span><span class="sxs-lookup"><span data-stu-id="17d84-147">Poland</span></span>               | <span data-ttu-id="17d84-148">주황색, 재생, T-모바일</span><span class="sxs-lookup"><span data-stu-id="17d84-148">Orange, Play, T-Mobile</span></span>                                  |
| <span data-ttu-id="17d84-149">사우디아라비아</span><span class="sxs-lookup"><span data-stu-id="17d84-149">Saudi Arabia</span></span>         | <span data-ttu-id="17d84-150">STC</span><span class="sxs-lookup"><span data-stu-id="17d84-150">STC</span></span>                                                     |
| <span data-ttu-id="17d84-151">싱가포르</span><span class="sxs-lookup"><span data-stu-id="17d84-151">Singapore</span></span>            | <span data-ttu-id="17d84-152">M1 제한 된 StarHub</span><span class="sxs-lookup"><span data-stu-id="17d84-152">M1 Limited, StarHub</span></span>                                     |
| <span data-ttu-id="17d84-153">슬로바키아</span><span class="sxs-lookup"><span data-stu-id="17d84-153">Slovakia</span></span>             | <span data-ttu-id="17d84-154">슬로바키아어 Telekom</span><span class="sxs-lookup"><span data-stu-id="17d84-154">Slovak Telekom</span></span>                                          |
| <span data-ttu-id="17d84-155">남아프리카 공화국</span><span class="sxs-lookup"><span data-stu-id="17d84-155">South Africa</span></span>         | <span data-ttu-id="17d84-156">Vodacom</span><span class="sxs-lookup"><span data-stu-id="17d84-156">Vodacom</span></span>                                                 |
| <span data-ttu-id="17d84-157">스페인</span><span class="sxs-lookup"><span data-stu-id="17d84-157">Spain</span></span>                | <span data-ttu-id="17d84-158">Orange</span><span class="sxs-lookup"><span data-stu-id="17d84-158">Orange</span></span>                                                  |
| <span data-ttu-id="17d84-159">스웨덴</span><span class="sxs-lookup"><span data-stu-id="17d84-159">Sweden</span></span>               | <span data-ttu-id="17d84-160">3, 통신 또는</span><span class="sxs-lookup"><span data-stu-id="17d84-160">3, Telenor</span></span>                                              |
| <span data-ttu-id="17d84-161">스위스</span><span class="sxs-lookup"><span data-stu-id="17d84-161">Switzerland</span></span>          | <span data-ttu-id="17d84-162">일출, Swisscom</span><span class="sxs-lookup"><span data-stu-id="17d84-162">Sunrise, Swisscom</span></span>                                       |
| <span data-ttu-id="17d84-163">대만</span><span class="sxs-lookup"><span data-stu-id="17d84-163">Taiwan</span></span>               | <span data-ttu-id="17d84-164">FarEasTone</span><span class="sxs-lookup"><span data-stu-id="17d84-164">FarEasTone</span></span>                                              |
| <span data-ttu-id="17d84-165">터키</span><span class="sxs-lookup"><span data-stu-id="17d84-165">Turkey</span></span>               | <span data-ttu-id="17d84-166">Turkcell</span><span class="sxs-lookup"><span data-stu-id="17d84-166">Turkcell</span></span>                                                |
| <span data-ttu-id="17d84-167">아랍에미리트연합국</span><span class="sxs-lookup"><span data-stu-id="17d84-167">United Arab Emirates</span></span> | <span data-ttu-id="17d84-168">Etisalat</span><span class="sxs-lookup"><span data-stu-id="17d84-168">Etisalat</span></span>                                                |
| <span data-ttu-id="17d84-169">미국</span><span class="sxs-lookup"><span data-stu-id="17d84-169">United States</span></span>        | <span data-ttu-id="17d84-170">스 프린트, Verizon</span><span class="sxs-lookup"><span data-stu-id="17d84-170">Sprint, Verizon</span></span>                                         |
| <span data-ttu-id="17d84-171">영국</span><span class="sxs-lookup"><span data-stu-id="17d84-171">United Kingdom</span></span>       | <span data-ttu-id="17d84-172">3 영국, EE, O2, Vodafone</span><span class="sxs-lookup"><span data-stu-id="17d84-172">3 UK, EE, O2, Vodafone</span></span>                                 |
