---
title: 2021년 3월 공지
description: 새로운 기능, 프로모션, 제품, 시장 또는 기존 제품의 변경 사항 등 Microsoft 파트너 센터에 대한 2021년 3월 공지입니다.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374393"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="85230-103">2021년 3월 공지</span><span class="sxs-lookup"><span data-stu-id="85230-103">March 2021 announcements</span></span>

<span data-ttu-id="85230-104">이 페이지에서는 2021년 3월 Microsoft 파트너 센터에 대한 공지를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="85230-105">이제 업데이트된 CSP 고객 주소 유효성 검사 API를 테스트에 사용 가능</span><span class="sxs-lookup"><span data-stu-id="85230-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="85230-106">범주</span><span class="sxs-lookup"><span data-stu-id="85230-106">Categories</span></span>

- <span data-ttu-id="85230-107">날짜: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="85230-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="85230-108">기능</span><span class="sxs-lookup"><span data-stu-id="85230-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-109">요약</span><span class="sxs-lookup"><span data-stu-id="85230-109">Summary</span></span>

<span data-ttu-id="85230-110">파트너와 고객이 신뢰를 바탕으로 사업을 영위하도록 도와주기 위한 노력의 일환으로, ValidateAddress API 변경 내용을 테스트하는 자리에 전 세계의 파트너를 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-111">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-111">Impacted audience</span></span>

<span data-ttu-id="85230-112">새 고객 주소 정보를 만들거나 기존 고객 주소 정보를 업데이트하는 모든 CSP 직접 청구 파트너 및 간접 공급자</span><span class="sxs-lookup"><span data-stu-id="85230-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="85230-113">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-113">Details</span></span>

<span data-ttu-id="85230-114">Microsoft는 신뢰할 수 있는 방식으로 운영되며,</span><span class="sxs-lookup"><span data-stu-id="85230-114">Microsoft runs on trust.</span></span> <span data-ttu-id="85230-115">규정을 준수하고 안전하며 보안이 유지되는 고객 주소 유효성 검사 제출 방법을 제공하여 CSP 프로그램에서 고객 구독을 거래할 수 있도록 최선을 다하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="85230-116">2021년 3월 31일에 ValidateAddress API가 변경되었습니다. 2021년 6월에 변경 내용을 적용하기에 앞서 변경 내용을 테스트하는 자리에 여러분을 초대하려 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="85230-117">이번 변경 내용은 ValidateAddress API에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="85230-118">CreateCustomer 및 UpdateBillingProfile API는 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="85230-119">응답에서 다음 상태 메시지 중 하나를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="85230-120">상태</span><span class="sxs-lookup"><span data-stu-id="85230-120">Status</span></span> | <span data-ttu-id="85230-121">Description</span><span class="sxs-lookup"><span data-stu-id="85230-121">Description</span></span> | <span data-ttu-id="85230-122">반환되는 추천 주소 수</span><span class="sxs-lookup"><span data-stu-id="85230-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="85230-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="85230-123">VerifiedShippable</span></span> | <span data-ttu-id="85230-124">주소가 확인되어 제품을 배송할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="85230-125">Single</span><span class="sxs-lookup"><span data-stu-id="85230-125">Single</span></span> |
| <span data-ttu-id="85230-126">Verified</span><span class="sxs-lookup"><span data-stu-id="85230-126">Verified</span></span> | <span data-ttu-id="85230-127">주소가 확인되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-127">Address is verified.</span></span> | <span data-ttu-id="85230-128">Single</span><span class="sxs-lookup"><span data-stu-id="85230-128">Single</span></span> |
| <span data-ttu-id="85230-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="85230-129">InteractionRequired</span></span> | <span data-ttu-id="85230-130">추천 주소가 많이 변경되어 사용자 확인이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="85230-131">Single</span><span class="sxs-lookup"><span data-stu-id="85230-131">Single</span></span> |
| <span data-ttu-id="85230-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="85230-132">StreetPartial</span></span> | <span data-ttu-id="85230-133">주소에 입력된 거리명이 완전하지 않아 추가 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="85230-134">여러 개(최대 3개)</span><span class="sxs-lookup"><span data-stu-id="85230-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="85230-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="85230-135">PremisesPartial</span></span> | <span data-ttu-id="85230-136">입력된 부지(건물 번호, 다세대 동호수 등)가 완전하지 않아 추가 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="85230-137">여러 개(최대 3개)</span><span class="sxs-lookup"><span data-stu-id="85230-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="85230-138">여러</span><span class="sxs-lookup"><span data-stu-id="85230-138">Multiple</span></span> | <span data-ttu-id="85230-139">주소에서 완전하지 않은 필드가 여러 개 있습니다(StreetPartial 및 PremisesPartial이 포함될 가능성도 있음).</span><span class="sxs-lookup"><span data-stu-id="85230-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="85230-140">여러 개(최대 3개)</span><span class="sxs-lookup"><span data-stu-id="85230-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="85230-141">없음</span><span class="sxs-lookup"><span data-stu-id="85230-141">None</span></span> | <span data-ttu-id="85230-142">주소가 올바르지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-142">Address is incorrect.</span></span> | <span data-ttu-id="85230-143">없음</span><span class="sxs-lookup"><span data-stu-id="85230-143">None</span></span> |
| <span data-ttu-id="85230-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="85230-144">NotValidated</span></span> | <span data-ttu-id="85230-145">유효성 검사 프로세스를 통해 주소를 보낼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="85230-146">없음</span><span class="sxs-lookup"><span data-stu-id="85230-146">None</span></span> |

<span data-ttu-id="85230-147">주소를 확인하기 위해 ValidateAddress API를 통해 주소를 제출하면 다음과 같은 응답 스키마가 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="85230-148">이 샘플 응답을 잘 보세요.</span><span class="sxs-lookup"><span data-stu-id="85230-148">Take a look at this sample response.</span></span> <span data-ttu-id="85230-149">미국의 경우 우편 번호에 5자리 숫자만 입력하면 우편 번호 줄에 4자리 숫자 접미사가 추가된 응답이 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="85230-150">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-150">Next steps</span></span>

- <span data-ttu-id="85230-151">업데이트 준비를 시작할 수 있도록, 테스트에 참가하는 SME(실무 전문가) Ali Khaki 씨와 샌드박스 테넌트 ID를 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="85230-152">CPV(제어판 공급업체) 솔루션을 사용하는 경우 CPV에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-153">질문이 있으신가요?</span><span class="sxs-lookup"><span data-stu-id="85230-153">Questions?</span></span>

<span data-ttu-id="85230-154">Microsoft 제품을 사용한 작업에 대해 질문이 있거나 지원이 필요한 경우 파트너 지원 Yammer 그룹에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="85230-155">새 EAC(Exchange 관리 센터) 환경</span><span class="sxs-lookup"><span data-stu-id="85230-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="85230-156">범주</span><span class="sxs-lookup"><span data-stu-id="85230-156">Categories</span></span>

- <span data-ttu-id="85230-157">날짜: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="85230-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="85230-158">기능</span><span class="sxs-lookup"><span data-stu-id="85230-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-159">요약</span><span class="sxs-lookup"><span data-stu-id="85230-159">Summary</span></span>

<span data-ttu-id="85230-160">2021년 4월 27일부터 EAC(Exchange 관리 센터)는 사용자의 일상적인 효율성을 개선하는 새로운 환경을 도입합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-161">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-161">Impacted audience</span></span>

<span data-ttu-id="85230-162">파트너 센터를 통해 Exchange에 액세스하는 위임된 관리자</span><span class="sxs-lookup"><span data-stu-id="85230-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="85230-163">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-163">Details</span></span>

<span data-ttu-id="85230-164">2021년 4월 27일부터 파트너 센터를 통해 Exchange로 이동하는 파트너는 새 EAC로 리디렉션됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="85230-165">이 새로운 환경은 현재 미리 보기로 제공되며, 관리자는 기존 EAC 내에서 오른쪽 위 모서리의 토글을 선택하여 이 환경을 활성화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="85230-166">모든 페이지에 표시되는 "지금 사용해 보기" 배너를 선택하여 새 EAC로 이동할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="85230-167">새 EAC의 이점은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="85230-168">메일 흐름 관련 문제에 대한 인사이트, 보고서 및 경고 메커니즘이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="85230-169">맞춤형 대시보드로 생산성을 향상할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="85230-170">새 환경을 탐색하는 방법을 안내하기 위해 새 EAC 환경의 **학습 및 가이드** 섹션에 비디오가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="85230-171">새 포털을 최대로 활용하는 방법을 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="85230-172">이 변경 내용이 적용되면 기존 EAC 환경은 더 이상 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="85230-173">변경 내용이 구현되기 전에 미리 통보됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-174">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-174">Next steps</span></span>

- <span data-ttu-id="85230-175">새 환경의 스크린샷을 볼 수 있는 [이 토픽에 대한 리소스](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="85230-176">이 정보를 조직의 적절한 관련자와 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="85230-177">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-177">Questions?</span></span>

<span data-ttu-id="85230-178">이 변경 내용에 대해 궁금한 점이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="85230-179">Microsoft Operations: 제품 출시 일정 소개</span><span class="sxs-lookup"><span data-stu-id="85230-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="85230-180">범주</span><span class="sxs-lookup"><span data-stu-id="85230-180">Categories</span></span>

- <span data-ttu-id="85230-181">날짜: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="85230-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="85230-182">제품 | 최신 작업 공간</span><span class="sxs-lookup"><span data-stu-id="85230-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="85230-183">요약</span><span class="sxs-lookup"><span data-stu-id="85230-183">Summary</span></span>

<span data-ttu-id="85230-184">파트너 피드백에 대응하기 위한 조치로 Microsoft Operations에서는 제품 출시에 대한 통신문을 간소화할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-185">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-185">Impacted audience</span></span>

<span data-ttu-id="85230-186">CSP(클라우드 솔루션 공급자) 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="85230-187">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-187">Details</span></span>

<span data-ttu-id="85230-188">Microsoft는 파트너 환경을 지속적으로 개선하기 위해 최선을 다하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="85230-189">제품 출시에 대한 중복 공지를 포함하여 Microsoft에서 보내는 통신문이 너무 많다는 피드백을 받았습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="85230-190">이러한 피드백에 대응하기 위해 Microsoft는 새 제품과 기존 제품의 제품 출시를 위한 준비 환경을 간소화했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="85230-191">이제 제품 출시 정보 보기가 한 달에 한 번만 제공되며, Operations 준비 리소스 갤러리에 게시됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="85230-192">이 월간 [제품 출시 일정 보기](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)는 Operations 준비 리소스 갤러리와 파트너 센터 공지의 개별 제품 출시 통신문을 대체합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="85230-193">[커뮤니티 컬렉션](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [일정 보기](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)및 [CSP 뉴스레터](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)에서도 이 [제품 출시 일정](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="85230-194">매월 제품 출시 일정을 게시할 때 Operations 준비 리소스 갤러리에 공지를 올려 소식을 알려 드리겠습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="85230-195">가격표 미리 보기 및 가격표 변경 로그뿐 아니라 제품 블로그, 라이선스 가이드 및 제품 마케팅 페이지에서 신제품과 기존 제품에 대한 정보를 계속 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="85230-196">변경 내용은 다음 제품이 출시될 때 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="85230-197">Dynamics 온-프레미스</span><span class="sxs-lookup"><span data-stu-id="85230-197">Dynamics on-premises</span></span>
- <span data-ttu-id="85230-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="85230-198">Microsoft 365</span></span>
- <span data-ttu-id="85230-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="85230-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="85230-200">Windows</span><span class="sxs-lookup"><span data-stu-id="85230-200">Windows</span></span>
- <span data-ttu-id="85230-201">서버</span><span class="sxs-lookup"><span data-stu-id="85230-201">Server</span></span>  
- <span data-ttu-id="85230-202">도구</span><span class="sxs-lookup"><span data-stu-id="85230-202">Tools</span></span>
- <span data-ttu-id="85230-203">Teams 및 Telco</span><span class="sxs-lookup"><span data-stu-id="85230-203">Teams and Telco</span></span>

<span data-ttu-id="85230-204">Operations 준비 정보가 필요한 제품 출시에 대한 공지를 계속 보내 드립니다.</span><span class="sxs-lookup"><span data-stu-id="85230-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-205">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-205">Next steps</span></span>

<span data-ttu-id="85230-206">이 토픽에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관련자와 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-207">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-207">Questions?</span></span>

<span data-ttu-id="85230-208">이러한 제품에 대한 추가 질문은 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="85230-209">CSP 고객 등록 요구 사항에 대한 변경 내용</span><span class="sxs-lookup"><span data-stu-id="85230-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="85230-210">범주</span><span class="sxs-lookup"><span data-stu-id="85230-210">Categories</span></span>

- <span data-ttu-id="85230-211">날짜: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="85230-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="85230-212">기능</span><span class="sxs-lookup"><span data-stu-id="85230-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-213">요약</span><span class="sxs-lookup"><span data-stu-id="85230-213">Summary</span></span>

<span data-ttu-id="85230-214">파트너와 고객이 신뢰를 바탕으로 비즈니스를 운영할 수 있도록 지원하기 위한 노력의 일환으로 Microsoft는 2021년 3월 25일부터 추가 고객 정보를 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-215">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-215">Impacted audience</span></span>

<span data-ttu-id="85230-216">다음 섹션에 나열된 국가에 신규 또는 기존 고객이 있는 CSP(클라우드 솔루션 공급자) 직접 청구 파트너 및 간접 공급자</span><span class="sxs-lookup"><span data-stu-id="85230-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="85230-217">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-217">Details</span></span>

<span data-ttu-id="85230-218">Microsoft는 신뢰할 수 있는 방식으로 운영되며,</span><span class="sxs-lookup"><span data-stu-id="85230-218">Microsoft runs on trust.</span></span> <span data-ttu-id="85230-219">규정을 준수하고 안전하며 보안이 유지되는 고객 유효성 검사 방법을 제공하여 CSP 프로그램에서 고객 구독을 거래할 수 있도록 최선을 다하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="85230-220">2021년 3월 25일에 다음 조건을 모두 충족하는 파트너에게 영향을 주는 파트너 센터 API 및 UI(사용자 인터페이스)의 향상된 기능이 도입됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="85230-221">파트너는 Microsoft와 직접 청구 관계를 맺고 있습니다(즉, 파트너가 직접 청구 파트너 또는 간접 공급자임).</span><span class="sxs-lookup"><span data-stu-id="85230-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="85230-222">파트너가 다음 국가의 신규 또는 기존 고객과 함께 비즈니스를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="85230-223">태국</span><span class="sxs-lookup"><span data-stu-id="85230-223">Thailand</span></span>
    - <span data-ttu-id="85230-224">베트남</span><span class="sxs-lookup"><span data-stu-id="85230-224">Vietnam</span></span>
    - <span data-ttu-id="85230-225">터키</span><span class="sxs-lookup"><span data-stu-id="85230-225">Turkey</span></span>
    - <span data-ttu-id="85230-226">폴란드</span><span class="sxs-lookup"><span data-stu-id="85230-226">Poland</span></span>
    - <span data-ttu-id="85230-227">남아프리카</span><span class="sxs-lookup"><span data-stu-id="85230-227">South Africa</span></span>
    - <span data-ttu-id="85230-228">인도</span><span class="sxs-lookup"><span data-stu-id="85230-228">India</span></span>
    - <span data-ttu-id="85230-229">브라질</span><span class="sxs-lookup"><span data-stu-id="85230-229">Brazil</span></span>
    - <span data-ttu-id="85230-230">이라크</span><span class="sxs-lookup"><span data-stu-id="85230-230">Iraq</span></span>
    - <span data-ttu-id="85230-231">미얀마</span><span class="sxs-lookup"><span data-stu-id="85230-231">Myanmar</span></span>
    - <span data-ttu-id="85230-232">남수단</span><span class="sxs-lookup"><span data-stu-id="85230-232">South Sudan</span></span>
    - <span data-ttu-id="85230-233">사우디아라비아</span><span class="sxs-lookup"><span data-stu-id="85230-233">Saudi Arabia</span></span>
    - <span data-ttu-id="85230-234">아랍에미리트연합국</span><span class="sxs-lookup"><span data-stu-id="85230-234">United Arab Emirates</span></span>
    - <span data-ttu-id="85230-235">베네수엘라</span><span class="sxs-lookup"><span data-stu-id="85230-235">Venezuela</span></span>

<span data-ttu-id="85230-236">조건을 충족하는 파트너는 신규 고객을 등록하거나 기존 고객의 세부 정보를 수정할 때 고객의 **회사 등록 ID**(고객의 **조직 INN** 이라고도 함) 및 **전화 번호** 를 제출해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="85230-237">이러한 파트너는 고객에 대한 선택적 **중간 이름** 을 입력할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="85230-238">회사 등록 ID를 추가할 때 고객 개인 ID가 아닌 회사 납세자 식별 번호를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="85230-239">다음 국가에서 신규 또는 기존 고객과 거래하는 파트너는 이미 2020년 11월의 이전 릴리스에 등록되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="85230-240">아르메니아</span><span class="sxs-lookup"><span data-stu-id="85230-240">Armenia</span></span>
- <span data-ttu-id="85230-241">아제르바이잔</span><span class="sxs-lookup"><span data-stu-id="85230-241">Azerbaijan</span></span>
- <span data-ttu-id="85230-242">벨라루스</span><span class="sxs-lookup"><span data-stu-id="85230-242">Belarus</span></span>
- <span data-ttu-id="85230-243">헝가리</span><span class="sxs-lookup"><span data-stu-id="85230-243">Hungary</span></span>
- <span data-ttu-id="85230-244">카자흐스탄</span><span class="sxs-lookup"><span data-stu-id="85230-244">Kazakhstan</span></span>
- <span data-ttu-id="85230-245">키르기스스탄</span><span class="sxs-lookup"><span data-stu-id="85230-245">Kyrgyzstan</span></span>
- <span data-ttu-id="85230-246">몰도바</span><span class="sxs-lookup"><span data-stu-id="85230-246">Moldova</span></span>
- <span data-ttu-id="85230-247">러시아</span><span class="sxs-lookup"><span data-stu-id="85230-247">Russia</span></span>
- <span data-ttu-id="85230-248">타지키스탄</span><span class="sxs-lookup"><span data-stu-id="85230-248">Tajikistan</span></span>
- <span data-ttu-id="85230-249">우크라이나</span><span class="sxs-lookup"><span data-stu-id="85230-249">Ukraine</span></span>
- <span data-ttu-id="85230-250">우즈베키스탄</span><span class="sxs-lookup"><span data-stu-id="85230-250">Uzbekistan</span></span>

<span data-ttu-id="85230-251">전 세계의 나머지 지역에 있는 고객을 대상으로 하는 파트너는 2021년 3월 25일에 고객의 **회사 등록 ID**, **전화 번호** 및 **중간 이름** 을 선택적 세부 정보로 입력할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-252">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-252">Next steps</span></span>

- <span data-ttu-id="85230-253">[전용 파트너 컬렉션](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)에서 기술 설명서 및 질문과 대답을 검토하여 자세한 지침을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="85230-254">파트너 센터 API 및 웹 사용자 환경을 사용하여 변경 내용을 통합할 준비를 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="85230-255">API/SDK는 테스트에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="85230-256">신규 고객을 등록하거나 기존 고객 세부 정보를 수정하는 경우 추가 데이터를 제출해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="85230-257">CPV(제어판 공급업체) 솔루션을 사용하는 경우 CPV에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-258">질문이 있으신가요?</span><span class="sxs-lookup"><span data-stu-id="85230-258">Questions?</span></span>

<span data-ttu-id="85230-259">법인 식별자(INN 또는 TIN이라고도 함)와 관련된 질문이 있는 경우 세무 고문 또는 지역 세무서에 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="85230-260">Microsoft는 세금 문제에 대한 지침을 제공할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="85230-261">Microsoft와의 작업에 대한 지원이 필요한 경우 [서비스 요청을 여세요](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="85230-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="85230-262">2021년 3월 1일 영구 소프트웨어 가격표 수정</span><span class="sxs-lookup"><span data-stu-id="85230-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="85230-263">범주</span><span class="sxs-lookup"><span data-stu-id="85230-263">Categories</span></span>

- <span data-ttu-id="85230-264">날짜: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="85230-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="85230-265">제품/시장</span><span class="sxs-lookup"><span data-stu-id="85230-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-266">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-266">Impacted audience</span></span>

<span data-ttu-id="85230-267">클라우드 솔루션 공급자 프로그램에서 영구 소프트웨어를 거래하는 간접 공급자 및 직접 청구 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="85230-268">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-268">Details</span></span>

<span data-ttu-id="85230-269">2021년 3월 1일에 게시된 영구 소프트웨어의 가격표에 잘못된 시장이 포함되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="85230-270">2021년 3월 17일에 영구 소프트웨어 가격표에 수정 사항이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="85230-271">이러한 수정 사항은 다음에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="85230-272">제품 ID: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="85230-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="85230-273">제품 이름: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="85230-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="85230-274">제거되었거나 지원되지 않는 시장: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="85230-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="85230-275">이러한 변경 내용은 위의 제품에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-275">These changes only apply to the above product.</span></span> <span data-ttu-id="85230-276">다른 제품은 수정되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="85230-277">다음 단계 및 리소스</span><span class="sxs-lookup"><span data-stu-id="85230-277">Next steps and resources</span></span>

- <span data-ttu-id="85230-278">영구 소프트웨어를 거래하는 파트너는 최신 소프트웨어 가격표를 다운로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="85230-279">두 글자로 된 약어와 해당 국가의 간편한 대응표는 [지역 국가 번호](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a><span data-ttu-id="85230-280">.NET Standard(v1.17.0)의 SDK 릴리스</span><span class="sxs-lookup"><span data-stu-id="85230-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="85230-281">범주</span><span class="sxs-lookup"><span data-stu-id="85230-281">Categories</span></span>

- <span data-ttu-id="85230-282">날짜: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="85230-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="85230-283">기능</span><span class="sxs-lookup"><span data-stu-id="85230-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="85230-284">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-284">Impacted audience</span></span>

<span data-ttu-id="85230-285">파트너 센터 .NET SDK를 사용하는 CSP 프로그램에 참여하는 Direct Bill 파트너 및 간접 공급자</span><span class="sxs-lookup"><span data-stu-id="85230-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="85230-286">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-286">Details</span></span>

<span data-ttu-id="85230-287">2020년 3월 23일부터 파트너는 업데이트된 퍼블릭 파트너 센터 SDK [GitHub 샘플](https://github.com/Microsoft/Partner-Center-DotNet-Samples)과 함께 [MicrosoftPartnerCenter.NETSDK(NuGet 갤러리 | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)를 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="85230-288">이 버전에는 다음 방법에 대한 업데이트가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="85230-289">감사 업데이트: 새 작업 유형</span><span class="sxs-lookup"><span data-stu-id="85230-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="85230-290">고객이 DAP를 승인하고 종료한 시점을 파악하기 위한 새 [작업 유형](https://docs.microsoft.com/partner-center/develop/auditing-resources)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="85230-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="85230-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="85230-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="85230-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="85230-293">감사 업데이트: 새 리소스 및 작업 유형</span><span class="sxs-lookup"><span data-stu-id="85230-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="85230-294">고객 디렉터리 역할 시나리오를 지원하기 위한 새 [리소스 및 작업 유형](https://docs.microsoft.com/partner-center/develop/auditing-resources)이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="85230-295">새 리소스 유형 "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="85230-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="85230-296">작업 유형 "AddUserMember" 및 "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="85230-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="85230-297">고객 계정에 대한 SDK 업데이트</span><span class="sxs-lookup"><span data-stu-id="85230-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="85230-298">GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus 지원</span><span class="sxs-lookup"><span data-stu-id="85230-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="85230-299">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="85230-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="85230-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="85230-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="85230-301">추가 변경 내용</span><span class="sxs-lookup"><span data-stu-id="85230-301">Additional changes</span></span>

<span data-ttu-id="85230-302">다음 변경 내용은 새 상거래의 일부로 도입되었으며 현재 M365/D365 새 상거래 환경 기술 미리 보기에 속하는 파트너에게만 초대를 통해 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="85230-303">새 상거래 기술 미리 보기에 속하지 않는 파트너는 영향을 인지할 수 없으며 이전 버전과 호환되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="85230-304">카탈로그 변경:</span><span class="sxs-lookup"><span data-stu-id="85230-304">Catalog Changes:</span></span>

  - <span data-ttu-id="85230-305">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="85230-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="85230-306">구매 및 관리:</span><span class="sxs-lookup"><span data-stu-id="85230-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="85230-307">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="85230-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="85230-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="85230-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="85230-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="85230-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="85230-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="85230-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="85230-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="85230-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="85230-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="85230-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-313">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-313">Next Steps</span></span>

- <span data-ttu-id="85230-314">최신 버전의 [MicrosoftPartnerCenter.NETSDK(NuGet 갤러리 | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) 다운로드</span><span class="sxs-lookup"><span data-stu-id="85230-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="85230-315">[GitHub 샘플](https://github.com/Microsoft/Partner-Center-DotNet-Samples) 다운로드 및 검토</span><span class="sxs-lookup"><span data-stu-id="85230-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="85230-316">CSP 상업용 Marketplace 제품 및 적격 제품에 대한 FY21 CSP 인센티브</span><span class="sxs-lookup"><span data-stu-id="85230-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="85230-317">범주</span><span class="sxs-lookup"><span data-stu-id="85230-317">Categories</span></span>

- <span data-ttu-id="85230-318">날짜: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="85230-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="85230-319">기능</span><span class="sxs-lookup"><span data-stu-id="85230-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-320">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-320">Impacted audience</span></span>

<span data-ttu-id="85230-321">클라우드 솔루션 공급자 프로그램의 간접 공급자 및 직접 청구 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="85230-322">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-322">Details</span></span>

<span data-ttu-id="85230-323">클라우드 솔루션 공급자 프로그램의 간접 공급자 및 직접 청구 파트너는 타사 제품을 판매하고, 파트너 센터 또는 Azure Portal에서 거래한 각 적격 타사 제품에 대한 리베이트 인센티브를 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="85230-324">이 인센티브는 적격 제품에 청구된 매출에 대한 리베이트 형태로 **2021년 6월 30일까지 제공** 됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="85230-325">아래에서 이 CSP 상업용 Marketplace 제품 인센티브에 대해 계속 알아보고, 오늘 고객에게 연락하여 지속적인 성공 및 디지털 변환을 가능하게 해주는 올바른 제품을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="85230-326">Microsoft는 ISV(독립 소프트웨어 공급업체)와 협력하여 Microsoft 고객을 위한 최신 IaaS 및 SaaS 솔루션을 출시했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="85230-327">ISV 게시자는 Microsoft 파트너 채널을 통해 제품 판매를 가능하게 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="85230-328">Microsoft의 인센티브 지급 대상 제품은 다음과 같은 두 가지 범주로 나뉩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="85230-329">Azure IP 공동 판매 인센티브화 상태의 SaaS 및 IaaS 타사 제품을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="85230-330">PowerPoint, Word, Excel, Outlook 또는 SharePoint 같은 Microsoft 365 생산성 앱 2개 이상 또는 Teams가 통합된 SaaS 애플리케이션</span><span class="sxs-lookup"><span data-stu-id="85230-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="85230-331">다음 단계 및 리소스</span><span class="sxs-lookup"><span data-stu-id="85230-331">Next steps and resources</span></span>

- <span data-ttu-id="85230-332">인센티브 지급 대상 Marketplace 앱을 판매한 후 [파트너 인센티브](https://partner.microsoft.com/membership/partner-incentives)를 획득하는 방법에 대해 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="85230-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="85230-333">새 제품은 매월 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="85230-334">클라우드 솔루션 공급자 직접 청구 파트너 인센티브 리소스</span><span class="sxs-lookup"><span data-stu-id="85230-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="85230-335">클라우드 솔루션 공급자 간접 공급자 인센티브 리소스</span><span class="sxs-lookup"><span data-stu-id="85230-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="85230-336">이 [프레젠테이션](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)을 검토하여 상업용 Marketplace 앱을 판매하는 방법에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="85230-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="85230-337">[여기](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)에서 추가 리소스를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="85230-338">[파트너 센터](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) 또는 [Azure Portal](https://ms.portal.azure.com/#home)에서 상업용 Marketplace 카탈로그 살펴보기</span><span class="sxs-lookup"><span data-stu-id="85230-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="85230-339">[API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)를 사용하여 회사의 Marketplace에 앱 통합</span><span class="sxs-lookup"><span data-stu-id="85230-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="85230-340">함께 비즈니스를 수행하고 싶은 ISV에게 연락하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="85230-341">간접 공급자는 API 사용을 통합하고 판매할 앱을 재판매인에게 안내해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="85230-342">질문이 있으세요?</span><span class="sxs-lookup"><span data-stu-id="85230-342">Questions?</span></span>  

<span data-ttu-id="85230-343">파트너 센터의 상업용 Marketplace에 대한 개요는 [이 문서](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="85230-344">추가 지원이 필요한 경우 파트너 센터에서 지원 요청을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="85230-345">[https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1)에서 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="85230-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="85230-346">Power BI Premium 제품 이름 지정 및 필수 구성 요소 업데이트</span><span class="sxs-lookup"><span data-stu-id="85230-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="85230-347">범주</span><span class="sxs-lookup"><span data-stu-id="85230-347">Categories</span></span>

- <span data-ttu-id="85230-348">날짜: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="85230-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="85230-349">기능</span><span class="sxs-lookup"><span data-stu-id="85230-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-350">요약</span><span class="sxs-lookup"><span data-stu-id="85230-350">Summary</span></span>

<span data-ttu-id="85230-351">Power BI Premium Per User 제품의 명명 및/또는 필수 구성 요소 정보를 명확히 하기 위해 2021년 4월 1일에 최종 가격표가 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-352">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-352">Impacted audience</span></span>

<span data-ttu-id="85230-353">CSP(클라우드 솔루션 공급자) 직접 및 간접 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="85230-354">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-354">Details</span></span>

<span data-ttu-id="85230-355">Power BI Premium Per User 제품의 명명 및/또는 필수 구성 요소 정보를 명확히 하기 위해 2021년 4월 1일에 최종 가격표가 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="85230-356">최종 가격표가 업데이트될 때까지 이 섹션의 정보를 사용하여 올바른 제품을 주문하도록 하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="85230-357">다음 세부 정보는 영향을 받는 SKU 및 필수 구성 요소를 자세히 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="85230-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="85230-358">3월 1일 가격표 미리 보기의 제품 표시 이름</span><span class="sxs-lookup"><span data-stu-id="85230-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="85230-359">4월 1일 최종 가격표에서 업데이트된 제품 표시 이름</span><span class="sxs-lookup"><span data-stu-id="85230-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="85230-360">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="85230-361">Power BI Premium Per User Add-On(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="85230-362">Power BI Premium Per User 추가 기능 **(Office)** (비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="85230-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="85230-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="85230-364">이 제품을 구매하려는 고객은 다음 필수 구성 요소 중 하나가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="85230-365">제품 표시 이름</span><span class="sxs-lookup"><span data-stu-id="85230-365">Offer display name</span></span> | <span data-ttu-id="85230-366">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="85230-367">Microsoft 365 E5(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="85230-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="85230-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="85230-369">오디오 회의 제외 Microsoft 365 E5(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="85230-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="85230-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="85230-371">Office 365 E5(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="85230-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="85230-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="85230-373">Office 365 E5(비영리 직원 가격) 평가판</span><span class="sxs-lookup"><span data-stu-id="85230-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="85230-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="85230-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="85230-375">오디오 회의 제외 Office 365 E5(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="85230-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="85230-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="85230-377">다음 Power BI Premium 제품을 구매하려면 필수 구성 요소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="85230-378">제품 표시 이름</span><span class="sxs-lookup"><span data-stu-id="85230-378">Offer display name</span></span> | <span data-ttu-id="85230-379">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="85230-380">Power BI Premium Per User Add-On(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="85230-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="85230-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="85230-382">이 제품을 구매하려는 고객은 이러한 필수 구성 요소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="85230-383">제품 표시 이름</span><span class="sxs-lookup"><span data-stu-id="85230-383">Offer display name</span></span> | <span data-ttu-id="85230-384">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="85230-385">Power BI Pro(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="85230-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="85230-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="85230-387">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-387">Next steps</span></span>

<span data-ttu-id="85230-388">이 항목에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관련자와 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="85230-389">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-389">Questions?</span></span>

<span data-ttu-id="85230-390">이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="85230-391">Microsoft 365 F3의 3월 가격 업데이트</span><span class="sxs-lookup"><span data-stu-id="85230-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="85230-392">범주</span><span class="sxs-lookup"><span data-stu-id="85230-392">Categories</span></span>

- <span data-ttu-id="85230-393">날짜: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="85230-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="85230-394">제품/시장</span><span class="sxs-lookup"><span data-stu-id="85230-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="85230-395">요약</span><span class="sxs-lookup"><span data-stu-id="85230-395">Summary</span></span>

<span data-ttu-id="85230-396">2021년 3월 가격표에서 Microsoft 365 F3 영국 파운드(GBP) 및 유로(EUR)의 잘못된 가격이 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-397">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-397">Impacted audience</span></span>

<span data-ttu-id="85230-398">2021년 3월 1일과 3월 17일 사이에 CSP(클라우드 솔루션 공급자) 프로그램을 통해 GBP 또는 EUR로 Microsoft 365 F3을 구매한 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="85230-399">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-399">Details</span></span>

<span data-ttu-id="85230-400">Microsoft에서 Microsoft 365 F3의 잘못된 가격을 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="85230-401">잘못된 가격은 2021년 3월 1일과 3월 17일 사이에 GBP 및 EUR로 구매한 제품에만 해당됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="85230-402">영향을 받는 제품과 통화는 아래에 나와 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="85230-403">Offer name</span><span class="sxs-lookup"><span data-stu-id="85230-403">Offer name</span></span> | <span data-ttu-id="85230-404">통화</span><span class="sxs-lookup"><span data-stu-id="85230-404">Currency</span></span> | <span data-ttu-id="85230-405">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-405">Offer ID</span></span> | <span data-ttu-id="85230-406">소재 ID</span><span class="sxs-lookup"><span data-stu-id="85230-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="85230-407">Microsoft 365 F3(자선)</span><span class="sxs-lookup"><span data-stu-id="85230-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="85230-408">GBP</span><span class="sxs-lookup"><span data-stu-id="85230-408">GBP</span></span> | <span data-ttu-id="85230-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="85230-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="85230-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="85230-410">AAD-11626</span></span> |
| <span data-ttu-id="85230-411">Microsoft 365 F3(상업용)</span><span class="sxs-lookup"><span data-stu-id="85230-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="85230-412">EUR</span><span class="sxs-lookup"><span data-stu-id="85230-412">EUR</span></span>| <span data-ttu-id="85230-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="85230-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="85230-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="85230-414">AAA-89898</span></span> |
 
<span data-ttu-id="85230-415">3월 및 4월 미리 보기 라이선스 기반 가격표는 태평양 표준시를 기준으로 3월 16일 오후 5시에 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-416">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-416">Next steps</span></span>

- <span data-ttu-id="85230-417">파트너는 해당하는 경우 이러한 가격 수정 사항이 포함된 최신 라이선스 기반 가격표(3월 및 4월 미리 보기 모두)를 다시 다운로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="85230-418">Microsoft는 앞으로 몇 주간 이메일을 통해 영향을 받는 파트너에게 연락하여 관련 거래 시정과 관련된 다음 조치를 알려 드릴 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-419">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-419">Questions?</span></span>

<span data-ttu-id="85230-420">추가 질문은 관련 CSP Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a><span data-ttu-id="85230-421">파트너 센터를 통해 법적 회사 이름 업데이트</span><span class="sxs-lookup"><span data-stu-id="85230-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="85230-422">범주</span><span class="sxs-lookup"><span data-stu-id="85230-422">Categories</span></span>

- <span data-ttu-id="85230-423">날짜: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="85230-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="85230-424">효율성 및 스케일링 향상</span><span class="sxs-lookup"><span data-stu-id="85230-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="85230-425">요약</span><span class="sxs-lookup"><span data-stu-id="85230-425">Summary</span></span>

<span data-ttu-id="85230-426">2021년 3월부터 MPN(Microsoft Partner Network) 파트너와 CSP(Cloud Solution Provider) 간접 재판매인은 파트너 센터를 통해 법적 회사 이름을 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-427">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-427">Impacted audience</span></span>

<span data-ttu-id="85230-428">MPN 파트너 및 CSP 간접 재판매인(CSP 다이렉트 청구 파트너에게는 적용되지 않음)</span><span class="sxs-lookup"><span data-stu-id="85230-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="85230-429">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-429">Details</span></span>

<span data-ttu-id="85230-430">2021년 3월부터 MPN 파트너 및 CSP 간접 재판매인은 규정을 준수하는 셀프 서비스 방식으로 파트너 센터를 통해 법적 회사 이름을 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="85230-431">이 새로운 기능을 통해 파트너는 더 이상 회사 이름을 업데이트하기 위해 파트너 센터 지원 티켓을 제출할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="85230-432">따라서 파트너는 이 작업을 수행할 때 상당한 시간을 절약할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="85230-433">자세히 알아보려면 [법적 비즈니스 프로필 업데이트](../update-your-partner-profile.md#update-your-legal-business-profile)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="85230-434">법적 비즈니스 프로필에 있는 회사 이름에 철자 오류와 약어가 없으며 정식 회사 비즈니스 등록 기록과 정확히 일치하는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="85230-435">조직 프로필을 업데이트하는 방법에 대한 자세한 내용은 [조직 프로필 확인](../update-your-partner-profile.md#update-your-legal-business-profile)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-436">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-436">Next steps</span></span>

<span data-ttu-id="85230-437">적절한 팀이 프로세스를 검토하고 업데이트할 수 있도록 조직 내에서 이 정보를 공유하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-438">질문이 있으세요?</span><span class="sxs-lookup"><span data-stu-id="85230-438">Questions?</span></span>

<span data-ttu-id="85230-439">추가 질문은 관련 CSP Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a><span data-ttu-id="85230-440">CSP(클라우드 솔루션 공급자) 프로그램 진화 및 오픈 라이선스 프로그램 변경 사항에 대한 업데이트</span><span class="sxs-lookup"><span data-stu-id="85230-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="85230-441">범주</span><span class="sxs-lookup"><span data-stu-id="85230-441">Categories</span></span>

- <span data-ttu-id="85230-442">날짜: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="85230-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="85230-443">기능</span><span class="sxs-lookup"><span data-stu-id="85230-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-444">요약</span><span class="sxs-lookup"><span data-stu-id="85230-444">Summary</span></span>

<span data-ttu-id="85230-445">새로운 상용 및 공공 부문 영구 소프트웨어 제품이 오픈 라이선스 프로그램의 변경 사항과 함께 CSP(클라우드 솔루션 공급자) 프로그램에 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-446">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-446">Impacted audience</span></span>

<span data-ttu-id="85230-447">오픈 라이선스 프로그램뿐만 아니라 모든 CSP 파트너 거래 영구 소프트웨어를 통해 판매되는 상업적 배포자 및 관리 재판매인</span><span class="sxs-lookup"><span data-stu-id="85230-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="85230-448">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-448">Details</span></span>

<span data-ttu-id="85230-449">2020년 9월 Microsoft는 파트너를 위한 온-프레미스 소프트웨어의 가용성을 포함하여 CSP 프로그램의 파트너에 대한 기회를 확장하는 디지털 변환 과정에서 일련의 단계를 [발표](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="85230-450">이러한 변화를 통해 파트너는 CSP의 소프트웨어 라이선스를 활용하여 비즈니스를 성장시키고 범위를 확장하여 오늘날의 클라우드 우선 세계에서 성공을 거둘 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="85230-451">또한 고객의 클라우드 전환을 지원하고 파트너에게 고객 하이브리드 클라우드 환경에 필요한 유연성을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="85230-452">이와 같은 디지털 전환 과정을 계속 진행하면서 다음과 같은 변경 사항을 발표합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="85230-453">2021년 7월 1일: 오픈 라이선스 프로그램 가격 목록에 새 SKU, 제품 또는 프로모션이 추가되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="85230-454">2021년 7월 7일: 두 개의 상용 제품인 Get Genuine Windows 및 Visual Studio Professional과 공공 부문 제품(정부, 교육 및 비영리 – [공지](./2020-december.md#9) 참조)이 CSP 영구 소프트웨어 가격표에 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="85230-455">가격 목록은 파트너 센터의 [판매 > 가격 및 제안](https://partnercenter.microsoft.com/pcv/sales) 페이지에 있는 소프트웨어 섹션에서 찾을 수 있으며 이 날짜에 다시 게시됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="85230-456">CSP 프로그램 발전 및 Open License 프로그램 변경에 대한 자세한 내용은 아래 **다음 단계** 를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-457">다음 단계:</span><span class="sxs-lookup"><span data-stu-id="85230-457">Next Steps:</span></span>

- <span data-ttu-id="85230-458">CSP 프로그램 진화: [클라우드 솔루션 공급자 프로그램의 영구 소프트웨어](https://partner.microsoft.com/resources/collection/software-in-csp#/) 준비 자료를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="85230-459">이 [준비 맵](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)을 사용하여 역할에 필요한 정보를 신속하게 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="85230-460">오픈 라이선스 프로그램 변경: [CSP 프로그램 진화 및 오픈 라이선스 프로그램 변경](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) 준비 자료를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="85230-461">이 [준비 맵](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)을 사용하여 역할에 필요한 정보를 신속하게 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-462">질문</span><span class="sxs-lookup"><span data-stu-id="85230-462">Questions</span></span>

<span data-ttu-id="85230-463">추가 질문은 관련 CSP Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="85230-464">이전 공지에 대한 업데이트: Compliance Manager의 추가 기능인 프리미엄 평가</span><span class="sxs-lookup"><span data-stu-id="85230-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="85230-465">범주</span><span class="sxs-lookup"><span data-stu-id="85230-465">Categories</span></span>

- <span data-ttu-id="85230-466">날짜: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="85230-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="85230-467">비즈니스 성장</span><span class="sxs-lookup"><span data-stu-id="85230-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="85230-468">요약</span><span class="sxs-lookup"><span data-stu-id="85230-468">Summary</span></span>

<span data-ttu-id="85230-469">평가판 제품은 가격 목록에 나열되지 않으며 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-470">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-470">Impacted audience</span></span>

<span data-ttu-id="85230-471">클라우드 솔루션 공급자를 통해 거래하는 모든 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="85230-472">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-472">Details</span></span>

<span data-ttu-id="85230-473">평가판 제품은 가격 목록에 포함되지 않았어야 했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="85230-474">이들 제품은 2021년 5월 1일 가격 목록에서 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="85230-475">원래 공지는 [여기](./2021-february.md#4)에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="85230-476">추가 자료</span><span class="sxs-lookup"><span data-stu-id="85230-476">Additional resources</span></span>

- [<span data-ttu-id="85230-477">Microsoft 365 E5 보안 및 규정 준수</span><span class="sxs-lookup"><span data-stu-id="85230-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="85230-478">Microsoft Compliance Manager에서 평가 빌드 및 관리 - Microsoft 365 Compliance</span><span class="sxs-lookup"><span data-stu-id="85230-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="85230-479">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-479">Next steps</span></span>

<span data-ttu-id="85230-480">이 항목에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관련자와 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-481">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-481">Questions?</span></span>

<span data-ttu-id="85230-482">이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a><span data-ttu-id="85230-483">OCP(One Commercial Partner) GTM(Go-to Market)에서 Microsoft 상업용 Marketplace로 솔루션 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="85230-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="85230-484">범주</span><span class="sxs-lookup"><span data-stu-id="85230-484">Categories</span></span>

- <span data-ttu-id="85230-485">날짜: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="85230-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="85230-486">기능</span><span class="sxs-lookup"><span data-stu-id="85230-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-487">요약</span><span class="sxs-lookup"><span data-stu-id="85230-487">Summary</span></span>

<span data-ttu-id="85230-488">2021년 3월 29일부터 OCP(One Commercial Partner) GTM(Go-to Market) 기능을 제한하는 것으로 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="85230-489">파트너 센터에서 상업용 Marketplace로 솔루션을 마이그레이션하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-490">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-490">Impacted audience</span></span>

<span data-ttu-id="85230-491">OCP GTM에서 솔루션과 공동 판매하는 조직</span><span class="sxs-lookup"><span data-stu-id="85230-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="85230-492">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-492">Details</span></span>

<span data-ttu-id="85230-493">2020년 12월에 Microsoft OCP GTM 도구에서 파트너 센터의 Microsoft 상업 시장으로 이동하기 시작했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="85230-494">이러한 전환은 수백만 고객에게 솔루션을 선보이고 다른 Microsoft 및 파트너 판매자와 양방향으로 기회를 공유하며 혁신적인 솔루션을 공동 판매할 수 있는 상용 시장의 기능을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="85230-495">전환의 다음 마일스톤은 2021년 3월 29일에 진행됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="85230-496">이때 일부 필드가 읽기 전용으로 되는 제한된 OCP GTM 기능을 경험하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="85230-497">현재 OCP GTM의 솔루션과 공동 판매 중인 경우 솔루션을 상용 시장으로 마이그레이션하여 기능을 활용하고 게시 환경을 단순화하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="85230-498">상업용 Marketplace로 전환하면 파트너 센터가 공동 판매 게시 환경의 주 대상이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="85230-499">Microsoft 제품에 사용되는 것과 동일한 채널 및 제품 내 환경을 통해 솔루션을 공유 고객과 연결하여 비즈니스를 계속 성장시킬 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="85230-500">[상업용 Marketplace에 대해 자세히 알아보세요](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="85230-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-501">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-501">Next steps</span></span>

- <span data-ttu-id="85230-502">솔루션을 아직 이동하지 않은 경우 [전환 가이드](/azure/marketplace/co-sell-solution-migration)에 설명된 지침을 따르거나 [단계별 비디오 자습서](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)를 참조하여 모든 마이그레이션 작업을 완료하고 상업용 Marketplace에 솔루션을 게시하기 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="85230-503">OCP GTM의 제한된 기능 환경과 관련된 질문은 [Microsoft 상업용 Marketplace FAQ에서 게시하기 위한 공동 판매 요구 사항](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="85230-504">("2021년 3월 29일부터 시작되는 OCP GTM 제한된 기능" 섹션을 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="85230-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="85230-505">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-505">Questions?</span></span>

<span data-ttu-id="85230-506">궁금한 사항이 있거나 추가 정보가 필요한 경우 [지원 팀](https://partner.microsoft.com/support/?stage=1)에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="85230-507">Azure용 CSP(클라우드 솔루션 공급자) 프로그램의 새로운 상거래 경험을 러시아로 확장</span><span class="sxs-lookup"><span data-stu-id="85230-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="85230-508">범주</span><span class="sxs-lookup"><span data-stu-id="85230-508">Categories</span></span>

- <span data-ttu-id="85230-509">날짜: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="85230-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="85230-510">기능</span><span class="sxs-lookup"><span data-stu-id="85230-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-511">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-511">Impacted audience</span></span>

<span data-ttu-id="85230-512">CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 러시아의 모든 파트너.</span><span class="sxs-lookup"><span data-stu-id="85230-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="85230-513">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-513">Details</span></span>

<span data-ttu-id="85230-514">2021년 3월 10일부터 **러시아 Azure용 CSP의 새로운 상거래 환경** 을 사용할 수 있게 되어 기쁘게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="85230-515">이 경험은 고객이 Azure 서비스를 구매하고 사용하는 방식을 간소화하고 개선합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="85230-516">또한 CSP 프로그램의 파트너에게 판매 활동 전반에 걸친 Azure 가격 책정, 글로벌 일관성을 위한 USD 가격 책정, 청구 날짜 조정 및 Azure Cost Management에 대한 액세스를 일관된 보기로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-517">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-517">Next steps</span></span>

<span data-ttu-id="85230-518">새로운 Azure 상거래 경험을 소개하고 추가 정보를 제공할 수 있는 몇 가지 리소스가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="85230-519">[CSP 프로그램 업데이트 리소스 갤러리](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)에서 최신 FAQ, 데크, 비디오 등을 찾아보세요.</span><span class="sxs-lookup"><span data-stu-id="85230-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="85230-520">파트너 센터 소프트웨어 라이선스 키 및 다운로드 이행</span><span class="sxs-lookup"><span data-stu-id="85230-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="85230-521">범주</span><span class="sxs-lookup"><span data-stu-id="85230-521">Categories</span></span>

- <span data-ttu-id="85230-522">날짜: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="85230-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="85230-523">기능</span><span class="sxs-lookup"><span data-stu-id="85230-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-524">요약</span><span class="sxs-lookup"><span data-stu-id="85230-524">Summary</span></span>

<span data-ttu-id="85230-525">파트너 센터 소프트웨어 다운로드 및 라이선스 키 이행 기능이 복구되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-526">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-526">Impacted audience</span></span>

<span data-ttu-id="85230-527">파트너 센터를 통해 정품 및 서버 구독 소프트웨어 주문을 거래하는 모든 CSP(클라우드 솔루션 공급자) 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="85230-528">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-528">Details</span></span>

<span data-ttu-id="85230-529">파트너의 피드백에 따라 파트너 센터에서 영구적인 서버 구독 소프트웨어 주문의 소프트웨어 및 라이선스 키를 얻을 수 있도록 파트너 센터 이행 기능을 복원 중입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="85230-530">이 기능은 2021년 1월 19일에 제거되기 이전 상태로 복원됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="85230-531">([공지](2020-september.md#17)를 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="85230-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="85230-532">소프트웨어 라이선스 키와 다운로드 링크는 매우 소중하고 인기가 많은 지적 자산입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="85230-533">유출될 경우 활성화 제한이 빠르게 삭제되어 고객 및 파트너 환경에 부정적인 영향을 미칠 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-534">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-534">Next steps</span></span>

<span data-ttu-id="85230-535">소프트웨어 키 사용 및 배포에 대한 다음 리소스와 중요 지침을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="85230-536">CSP 프로그램을 통해 온-프레미스 소프트웨어 판매</span><span class="sxs-lookup"><span data-stu-id="85230-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="85230-537">[파트너 센터 새 상거래 운영 가이드](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)(**소프트웨어 키 배포에 대한 지침** 섹션 참조)</span><span class="sxs-lookup"><span data-stu-id="85230-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="85230-538">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-538">Questions?</span></span>

<span data-ttu-id="85230-539">이 공지에 대한 추가 질문은 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><span data-ttu-id="85230-540"><a name="3">PSC(Partner Sales Connect)에서 파트너 센터로 거래 마이그레이션</a></span><span class="sxs-lookup"><span data-stu-id="85230-540"><a name="3"></a>Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="85230-541">범주</span><span class="sxs-lookup"><span data-stu-id="85230-541">Categories</span></span>

- <span data-ttu-id="85230-542">날짜: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="85230-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="85230-543">기능</span><span class="sxs-lookup"><span data-stu-id="85230-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-544">요약</span><span class="sxs-lookup"><span data-stu-id="85230-544">Summary</span></span>

<span data-ttu-id="85230-545">2021년 3월 31일부터 PSC(Partner Sales Connect)가 읽기 전용 액세스로 전환되므로 PSC의 거래를 파트너 센터로 마이그레이션하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-546">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-546">Impacted audience</span></span>

<span data-ttu-id="85230-547">PSC에서 거래하는 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="85230-548">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-548">Details</span></span>

<span data-ttu-id="85230-549">동반 성장이라는 약속을 지키기 위한 방편 중 하나인 **Microsoft와 공동 판매** 는 파트너가 **검색되고, 전문 지식을 제공하고, 고객 범위를 확장** 하여 긍정적인 고객 결과를 얻을 수 있는 경로입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="85230-550">평균 거래 속도가 일반 판매보다 **3.5배 빠르기 때문에** 파트너 센터에서 공동 판매 환경을 관리하면 직접 고객, 파트너 및 Microsoft 판매자 채널을 통해 판매하고 전체 추천 파이프라인을 한 곳에서 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="85230-551">**2021년 3월 31일** 부터 **PSC** 가 **읽기 전용 액세스** 로 전환되므로 파트너 센터로 이동하여 개선된 기능을 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="85230-552">필요한 지원의 종류에 따라 Microsoft와 공유하는 거래를 적절한 판매자에게 **보다 정확하게 라우팅** 합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="85230-553">인센티브 대상 솔루션을 결정하고 ISV Connect 프로그램 조건을 충족하기 위한 **거래 자격 사전 평가** 를 도입했으며, 승인 프로세스 및 POE(최종 실행 증명서) 입증이 간소화될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="85230-554">공동 판매 기회와 영업부에서 확인한 잠재 고객을 모두 한 곳에서 관리하는 **원활한 사용자 환경** 을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="85230-555">또한 최근에는 파트너의 전환을 도와주기 위해 파트너 센터에 새로운 기능을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="85230-556">공동 판매 기회를 대량으로 작업</span><span class="sxs-lookup"><span data-stu-id="85230-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="85230-557">[거래 마이그레이션 기능](../psc-to-pc.md)(**PSC 거래 마이그레이션** 섹션 참조)</span><span class="sxs-lookup"><span data-stu-id="85230-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="85230-558">파트너 센터에서 공동 판매 환경을 사용하면 영업 팀은 잠재 고객 및 기회를 창출하고, 거래를 완료하고, 지속적인 고객 관계를 만드는 데 더 많은 시간을 투자할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="85230-559">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-559">Next steps</span></span>

<span data-ttu-id="85230-560">파트너 센터 [전환 가이드](../psc-to-pc.md)를 사용하여 PSC의 거래를 파트너 센터로 마이그레이션하는 단계를 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="85230-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-561">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-561">Questions?</span></span>

<span data-ttu-id="85230-562">추가 질문은 [고객 지원](https://partner.microsoft.com/support/?stage=1)으로 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="85230-563">2021년 4월 1일에 사용 가능한 새로운 Microsoft Dynamics 365 제품 및 제안</span><span class="sxs-lookup"><span data-stu-id="85230-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="85230-564">범주</span><span class="sxs-lookup"><span data-stu-id="85230-564">Categories</span></span>

- <span data-ttu-id="85230-565">날짜: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="85230-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="85230-566">기능</span><span class="sxs-lookup"><span data-stu-id="85230-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-567">요약</span><span class="sxs-lookup"><span data-stu-id="85230-567">Summary</span></span>

<span data-ttu-id="85230-568">2021년 4월 1일에 Microsoft는 CSP(클라우드 솔루션 공급자) 프로그램에 대한 여러 가지 신제품을 출시할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-569">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-569">Impacted audience</span></span>

<span data-ttu-id="85230-570">CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 모든 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="85230-571">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-571">Details</span></span>

<span data-ttu-id="85230-572">2021년 4월 1일에 Microsoft는 다음과 같은 신제품을 출시할 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="85230-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="85230-573">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="85230-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="85230-574">Customer Voice and Marketing USL 지역 및 세그먼트 확장</span><span class="sxs-lookup"><span data-stu-id="85230-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="85230-575">**Power BI Premium Per User**</span><span class="sxs-lookup"><span data-stu-id="85230-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="85230-576">Microsoft 최초의 사용자 단위 Power BI Premium 제품이 곧 출시됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="85230-577">Power BI Premium은 현재 용량 구성으로만 판매됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="85230-578">Power BI Premium Per User는 엔터프라이즈 BI(비즈니스 인텔리전스) 및 분석 기능에 대한 액세스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="85230-579">유연한 개별 사용자 단위 라이선스는 중소기업에 적합합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="85230-580">이 제품에 대한 자세한 내용은 [Power BI 릴리스 정보](/power-platform-release-plan/2020wave2/power-bi/planned-features)를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="85230-581">**솔루션 세부 정보**</span><span class="sxs-lookup"><span data-stu-id="85230-581">**Offer details**</span></span>

<span data-ttu-id="85230-582">제품 이름은 가격표 미리 보기와 약간 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="85230-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="85230-583">Offer name</span><span class="sxs-lookup"><span data-stu-id="85230-583">Offer name</span></span> | <span data-ttu-id="85230-584">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="85230-585">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="85230-585">Power BI Premium Per User</span></span> | <span data-ttu-id="85230-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="85230-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="85230-587">Power BI Premium Per User for Faculty</span><span class="sxs-lookup"><span data-stu-id="85230-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="85230-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="85230-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="85230-589">Power BI Premium Per User for Students</span><span class="sxs-lookup"><span data-stu-id="85230-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="85230-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="85230-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="85230-591">Power BI Premium Per User(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="85230-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="85230-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="85230-593">Power BI Premium Per User Add-On</span><span class="sxs-lookup"><span data-stu-id="85230-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="85230-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="85230-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="85230-595">Power BI Premium Per User Add-On for Faculty</span><span class="sxs-lookup"><span data-stu-id="85230-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="85230-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="85230-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="85230-597">Power BI Premium Per User Add-On for Students</span><span class="sxs-lookup"><span data-stu-id="85230-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="85230-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="85230-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="85230-599">Power BI Premium Per User Add-On(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="85230-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="85230-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="85230-601">**Customer Voice and Marketing USL 지역 및 세그먼트 확장**</span><span class="sxs-lookup"><span data-stu-id="85230-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="85230-602">2020년 12월 출시의 후속 작업으로 Dynamics 365 Customer Voice and Marketing USL 제품이 새로운 국가와 비영리 및 교육 SKU를 추가하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="85230-603">Offer name</span><span class="sxs-lookup"><span data-stu-id="85230-603">Offer name</span></span> | <span data-ttu-id="85230-604">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="85230-605">Dynamics 365 Customer Voice USL(비영리 직원 가격)</span><span class="sxs-lookup"><span data-stu-id="85230-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="85230-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="85230-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="85230-607">Dynamics 365 Customer Voice USL for Faculty</span><span class="sxs-lookup"><span data-stu-id="85230-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="85230-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="85230-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="85230-609">이 제품에 대해 자세히 알아보려면 다음 페이지를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="85230-610">Dynamics 365 Customer Service Voice 홈 페이지</span><span class="sxs-lookup"><span data-stu-id="85230-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="85230-611">Dynamics 365 Marketing 홈 페이지</span><span class="sxs-lookup"><span data-stu-id="85230-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="85230-612">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-612">Next steps</span></span>

<span data-ttu-id="85230-613">이 토픽에 대한 리소스를 검토하고, 이 정보를 조직 내의 적절한 관계자와 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="85230-614">궁금한 점이 더 있나요?</span><span class="sxs-lookup"><span data-stu-id="85230-614">Questions?</span></span>

<span data-ttu-id="85230-615">이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a><span data-ttu-id="85230-616">현재 일부 제품군에서 Microsoft 유니버설 인쇄 사용 가능</span><span class="sxs-lookup"><span data-stu-id="85230-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="85230-617">범주</span><span class="sxs-lookup"><span data-stu-id="85230-617">Categories</span></span>

- <span data-ttu-id="85230-618">날짜: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="85230-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="85230-619">기능</span><span class="sxs-lookup"><span data-stu-id="85230-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="85230-620">요약</span><span class="sxs-lookup"><span data-stu-id="85230-620">Summary</span></span>

<span data-ttu-id="85230-621">Microsoft 유니버설 인쇄는 2021년 3월 1일부터 일부 Microsoft 365 제품군 내에서 독립 실행형 추가 기능으로 거래에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="85230-622">영향을 받는 대상</span><span class="sxs-lookup"><span data-stu-id="85230-622">Impacted audience</span></span>

<span data-ttu-id="85230-623">CSP(클라우드 솔루션 공급자) 프로그램을 통해 거래하는 모든 파트너</span><span class="sxs-lookup"><span data-stu-id="85230-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="85230-624">세부 정보</span><span class="sxs-lookup"><span data-stu-id="85230-624">Details</span></span>

<span data-ttu-id="85230-625">[유니버설 인쇄](https://aka.ms/universalprint)는 Windows 디바이스에서 Azure에 등록된 프린터로 인쇄할 수 있게 해주는 Microsoft 365 인쇄 서비스이며, 온-프레미스 인쇄 서버가 필요 없습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="85230-626">2021년 3월 1일부터 거래에 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="85230-627">작업자는 드라이버 없는 인쇄, 간소화된 위치 기반 프린터 검색, 오랜 학습 기간이 필요 없는 직관적인 인쇄 환경이라는 장점을 누릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="85230-628">Azure AD(Azure Active Directory)에 조인된 디바이스는 기존 Azure AD 자격 증명을 사용하여 안전하게 인쇄합니다.</span><span class="sxs-lookup"><span data-stu-id="85230-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="85230-629">관리자는 Azure Portal에서 인쇄를 관리하며, 유니버설 인쇄가 기본 지원되므로 프린터를 쉽게 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="85230-630">유니버설 인쇄는 유니버설 인쇄 커넥터 소프트웨어를 사용하여 호환되지 않는 프린터와 함께 배포할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85230-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="85230-631">유니버설 인쇄는 출시 시 Windows E3, A3, E5, A5 및 Microsoft 365 BP, F3, E3, A3, E5, A5에 백필됩니다.</span><span class="sxs-lookup"><span data-stu-id="85230-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="85230-632">**솔루션 세부 정보**</span><span class="sxs-lookup"><span data-stu-id="85230-632">**Offer details**</span></span>

<span data-ttu-id="85230-633">제품 이름은 가격표 미리 보기와 약간 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="85230-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="85230-634">Offer name</span><span class="sxs-lookup"><span data-stu-id="85230-634">Offer name</span></span> | <span data-ttu-id="85230-635">제품 ID</span><span class="sxs-lookup"><span data-stu-id="85230-635">Offer ID</span></span> | <span data-ttu-id="85230-636">소재 ID</span><span class="sxs-lookup"><span data-stu-id="85230-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="85230-637">유니버설 인쇄 볼륨 추가(작업 500개) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="85230-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="85230-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="85230-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="85230-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="85230-639">9BI-00004</span></span>   |
| <span data-ttu-id="85230-640">교직원용 유니버설 인쇄 볼륨 추가(작업 500개) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="85230-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="85230-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="85230-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="85230-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="85230-642">9BK-00004</span></span>   |
| <span data-ttu-id="85230-643">유니버설 인쇄 볼륨 추가(작업 500개) - Windows</span><span class="sxs-lookup"><span data-stu-id="85230-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="85230-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="85230-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="85230-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="85230-645">9BI-00002</span></span>   |
| <span data-ttu-id="85230-646">교직원용 유니버설 인쇄 볼륨 추가(작업 500개) - Windows</span><span class="sxs-lookup"><span data-stu-id="85230-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="85230-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="85230-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="85230-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="85230-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="85230-649">다음 단계</span><span class="sxs-lookup"><span data-stu-id="85230-649">Next steps</span></span>

<span data-ttu-id="85230-650">가격표와 [유니버설 인쇄 개요](/universal-print/fundamentals/universal-print-whatis)를 숙지하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="85230-651">이 정보를 조직 내의 모든 해당 담당자와 공유하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="85230-652">질문이 있으세요?</span><span class="sxs-lookup"><span data-stu-id="85230-652">Questions?</span></span>

<span data-ttu-id="85230-653">이 제품에 대한 질문이 있는 경우 관련 Yammer 커뮤니티를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="85230-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
