---
title: CSP를 통해 소프트웨어 구독 판매
ms.topic: how-to
ms.date: 03/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP 프로그램의 파트너가 파트너 센터를 사용하여 고객의 Azure 예약 인스턴스 및 서버 구독을 구매, 관리, 판매 및 취소하는 방법을 알아봅니다.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ac6169ea6680ea0b36cd5caa3f3e8276f557bea2
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502555"
---
# <a name="sell-software-subscriptions-through-the-cloud-solution-provider-csp-program"></a><span data-ttu-id="ae4da-103">CSP(클라우드 솔루션 공급자) 프로그램을 통해 소프트웨어 구독 판매</span><span class="sxs-lookup"><span data-stu-id="ae4da-103">Sell software subscriptions through the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="ae4da-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="ae4da-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ae4da-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="ae4da-105">Admin agent</span></span>
- <span data-ttu-id="ae4da-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="ae4da-106">Global admin</span></span>

<span data-ttu-id="ae4da-107">Azure 예약 및 Server 구독(Windows Server 및 SQL Server 구독)이 있으면 CSP 프로그램의 파트너는 예측성이 뛰어난 영구적인 클라우드 워크로드를 지원할 수 있는 비용 효과적인 솔루션에 대한 고객의 급증하는 요구를 보다 잘 충족할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-107">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="ae4da-108">이제 파트너는 파트너 센터 및 Azure Portal을 통해 Azure 하이브리드 혜택을 활용하여 상업 고객 대신 Azure 예약 및 Server 구독을 획득하고, 프로비저닝하고, 관리할 수 있게 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-108">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="ae4da-109">Azure 하이브리드 혜택은 Windows Server 라이선스에서 더 많은 가치를 창출하고 가상 머신에서 최대 40%의 비용을 절감할 수 있도록 도와줍니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-109">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="ae4da-110">Software Assurance에서 적용되는 Windows Server Datacenter 및 Standard 버전 라이선스를 통해 이 혜택을 이용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-110">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="ae4da-111">버전에 따라 라이선스를 변환하거나 재사용하여 Azure에서 더 낮은 기본 컴퓨팅 요금(예: Linux 가상 머신 요금)으로 Windows Server 가상 머신을 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-111">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, for example).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="ae4da-112">Azure 예약을 사용할 수 없는 지역/국가</span><span class="sxs-lookup"><span data-stu-id="ae4da-112">Azure reservations unavailable markets</span></span>

>[!IMPORTANT]
><span data-ttu-id="ae4da-113">Azure 예약은 다음과 같은 지역/국가에서는 사용할 수 **없습니다**.</span><span class="sxs-lookup"><span data-stu-id="ae4da-113">Azure reservations **are not** available in the following markets:</span></span>  
>  
> <span data-ttu-id="ae4da-114">**사용할 수 없는 시장(사전순)**</span><span class="sxs-lookup"><span data-stu-id="ae4da-114">**Unavailable markets (in alphabetical order)**</span></span>
>
> |<span data-ttu-id="ae4da-115">A부터 Gi까지</span><span class="sxs-lookup"><span data-stu-id="ae4da-115">A to Gi</span></span>   | <span data-ttu-id="ae4da-116">Gr부터 Pal까지</span><span class="sxs-lookup"><span data-stu-id="ae4da-116">Gr to Pal</span></span>  | <span data-ttu-id="ae4da-117">Pap부터 Z까지</span><span class="sxs-lookup"><span data-stu-id="ae4da-117">Pap to Z</span></span> |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="ae4da-118">올란드 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-118">Aland Islands</span></span>     | <span data-ttu-id="ae4da-119">그린란드</span><span class="sxs-lookup"><span data-stu-id="ae4da-119">Greenland</span></span>     | <span data-ttu-id="ae4da-120">파푸아뉴기니</span><span class="sxs-lookup"><span data-stu-id="ae4da-120">Papua New Guinea</span></span>     |
> | <span data-ttu-id="ae4da-121">미국령 사모아</span><span class="sxs-lookup"><span data-stu-id="ae4da-121">American Samoa</span></span>     | <span data-ttu-id="ae4da-122">그레나다</span><span class="sxs-lookup"><span data-stu-id="ae4da-122">Grenada</span></span>     | <span data-ttu-id="ae4da-123">핏케언 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-123">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="ae4da-124">안도라</span><span class="sxs-lookup"><span data-stu-id="ae4da-124">Andorra</span></span>     | <span data-ttu-id="ae4da-125">과들루프</span><span class="sxs-lookup"><span data-stu-id="ae4da-125">Guadeloupe</span></span>     | <span data-ttu-id="ae4da-126">리유니언</span><span class="sxs-lookup"><span data-stu-id="ae4da-126">Reunion</span></span>     |
> | <span data-ttu-id="ae4da-127">앵귈라</span><span class="sxs-lookup"><span data-stu-id="ae4da-127">Anguilla</span></span>     | <span data-ttu-id="ae4da-128">괌</span><span class="sxs-lookup"><span data-stu-id="ae4da-128">Guam</span></span>     | <span data-ttu-id="ae4da-129">사바</span><span class="sxs-lookup"><span data-stu-id="ae4da-129">Saba</span></span>   |
> | <span data-ttu-id="ae4da-130">남극</span><span class="sxs-lookup"><span data-stu-id="ae4da-130">Antarctica</span></span>     | <span data-ttu-id="ae4da-131">건지</span><span class="sxs-lookup"><span data-stu-id="ae4da-131">Guernsey</span></span>     | <span data-ttu-id="ae4da-132">세인트 바르텔레미</span><span class="sxs-lookup"><span data-stu-id="ae4da-132">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="ae4da-133">앤티가 바부다</span><span class="sxs-lookup"><span data-stu-id="ae4da-133">Antigua and Barbuda</span></span>       | <span data-ttu-id="ae4da-134">기니</span><span class="sxs-lookup"><span data-stu-id="ae4da-134">Guinea</span></span>     | <span data-ttu-id="ae4da-135">세인트 루시아</span><span class="sxs-lookup"><span data-stu-id="ae4da-135">Saint Lucia</span></span>   |
> | <span data-ttu-id="ae4da-136">아루바</span><span class="sxs-lookup"><span data-stu-id="ae4da-136">Aruba</span></span>       | <span data-ttu-id="ae4da-137">기니비사우</span><span class="sxs-lookup"><span data-stu-id="ae4da-137">Guinea-Bissau</span></span>     | <span data-ttu-id="ae4da-138">세인트 마틴</span><span class="sxs-lookup"><span data-stu-id="ae4da-138">Saint Martin</span></span>   |
> | <span data-ttu-id="ae4da-139">아제르바이잔</span><span class="sxs-lookup"><span data-stu-id="ae4da-139">Azerbaijan</span></span>       | <span data-ttu-id="ae4da-140">가이아나</span><span class="sxs-lookup"><span data-stu-id="ae4da-140">Guyana</span></span>     | <span data-ttu-id="ae4da-141">생피에르앤드미클롱</span><span class="sxs-lookup"><span data-stu-id="ae4da-141">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="ae4da-142">베냉</span><span class="sxs-lookup"><span data-stu-id="ae4da-142">Benin</span></span>     | <span data-ttu-id="ae4da-143">아이티</span><span class="sxs-lookup"><span data-stu-id="ae4da-143">Haiti</span></span>       | <span data-ttu-id="ae4da-144">세인트 빈센트 그레나딘</span><span class="sxs-lookup"><span data-stu-id="ae4da-144">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="ae4da-145">부탄</span><span class="sxs-lookup"><span data-stu-id="ae4da-145">Bhutan</span></span>     | <span data-ttu-id="ae4da-146">허드 섬 및 맥도널드 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-146">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="ae4da-147">사모아</span><span class="sxs-lookup"><span data-stu-id="ae4da-147">Samoa</span></span>     |
> | <span data-ttu-id="ae4da-148">보네르</span><span class="sxs-lookup"><span data-stu-id="ae4da-148">Bonaire</span></span>     | <span data-ttu-id="ae4da-149">맨 섬</span><span class="sxs-lookup"><span data-stu-id="ae4da-149">Isle of Man</span></span>     | <span data-ttu-id="ae4da-150">산마리노</span><span class="sxs-lookup"><span data-stu-id="ae4da-150">San Marino</span></span>     |
> | <span data-ttu-id="ae4da-151">부베이 섬</span><span class="sxs-lookup"><span data-stu-id="ae4da-151">Bouvet Island</span></span>     | <span data-ttu-id="ae4da-152">얀마웬</span><span class="sxs-lookup"><span data-stu-id="ae4da-152">Jan Mayen</span></span>     | <span data-ttu-id="ae4da-153">상투메 프린시페</span><span class="sxs-lookup"><span data-stu-id="ae4da-153">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="ae4da-154">영국령 인도양 식민지</span><span class="sxs-lookup"><span data-stu-id="ae4da-154">British Indian Ocean Territory</span></span>       | <span data-ttu-id="ae4da-155">저지</span><span class="sxs-lookup"><span data-stu-id="ae4da-155">Jersey</span></span>     | <span data-ttu-id="ae4da-156">세이셸</span><span class="sxs-lookup"><span data-stu-id="ae4da-156">Seychelles</span></span>   |
> | <span data-ttu-id="ae4da-157">영국령 버전 아일랜드</span><span class="sxs-lookup"><span data-stu-id="ae4da-157">British Virgin Islands</span></span>     | <span data-ttu-id="ae4da-158">키리바시</span><span class="sxs-lookup"><span data-stu-id="ae4da-158">Kiribati</span></span>       | <span data-ttu-id="ae4da-159">시에라리온</span><span class="sxs-lookup"><span data-stu-id="ae4da-159">Sierra Leone</span></span>   |
> | <span data-ttu-id="ae4da-160">부르키나파소</span><span class="sxs-lookup"><span data-stu-id="ae4da-160">Burkina Faso</span></span>     | <span data-ttu-id="ae4da-161">코소보</span><span class="sxs-lookup"><span data-stu-id="ae4da-161">Kosovo</span></span>     | <span data-ttu-id="ae4da-162">신트외스타티위스</span><span class="sxs-lookup"><span data-stu-id="ae4da-162">Sint Eustatius</span></span>     |
> | <span data-ttu-id="ae4da-163">부룬디</span><span class="sxs-lookup"><span data-stu-id="ae4da-163">Burundi</span></span>     | <span data-ttu-id="ae4da-164">라오스</span><span class="sxs-lookup"><span data-stu-id="ae4da-164">Laos</span></span>     | <span data-ttu-id="ae4da-165">신트마르텐</span><span class="sxs-lookup"><span data-stu-id="ae4da-165">Sint Maarten</span></span>     |
> | <span data-ttu-id="ae4da-166">캄보디아</span><span class="sxs-lookup"><span data-stu-id="ae4da-166">Cambodia</span></span>     | <span data-ttu-id="ae4da-167">레소토</span><span class="sxs-lookup"><span data-stu-id="ae4da-167">Lesotho</span></span>     | <span data-ttu-id="ae4da-168">솔로몬 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-168">Solomon Islands</span></span>     |
> | <span data-ttu-id="ae4da-169">중앙 아프리카 공화국</span><span class="sxs-lookup"><span data-stu-id="ae4da-169">Central African Republic</span></span>     | <span data-ttu-id="ae4da-170">라이베리아</span><span class="sxs-lookup"><span data-stu-id="ae4da-170">Liberia</span></span>     | <span data-ttu-id="ae4da-171">소말리아</span><span class="sxs-lookup"><span data-stu-id="ae4da-171">Somalia</span></span>     |
> | <span data-ttu-id="ae4da-172">차드</span><span class="sxs-lookup"><span data-stu-id="ae4da-172">Chad</span></span>     | <span data-ttu-id="ae4da-173">마다가스카르</span><span class="sxs-lookup"><span data-stu-id="ae4da-173">Madagascar</span></span>     | <span data-ttu-id="ae4da-174">사우스 조지아 및 사우스 샌드위치 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-174">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="ae4da-175">중국</span><span class="sxs-lookup"><span data-stu-id="ae4da-175">China</span></span>     | <span data-ttu-id="ae4da-176">말라위</span><span class="sxs-lookup"><span data-stu-id="ae4da-176">Malawi</span></span>     | <span data-ttu-id="ae4da-177">남수단</span><span class="sxs-lookup"><span data-stu-id="ae4da-177">South Sudan</span></span>     |
> | <span data-ttu-id="ae4da-178">크리스마스 섬</span><span class="sxs-lookup"><span data-stu-id="ae4da-178">Christmas Island</span></span>     | <span data-ttu-id="ae4da-179">몰디브</span><span class="sxs-lookup"><span data-stu-id="ae4da-179">Maldives</span></span>     | <span data-ttu-id="ae4da-180">세인트 헬레나, 어센션, 트리스탄 다 쿠나</span><span class="sxs-lookup"><span data-stu-id="ae4da-180">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="ae4da-181">코코스 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-181">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="ae4da-182">말리</span><span class="sxs-lookup"><span data-stu-id="ae4da-182">Mali</span></span>     | <span data-ttu-id="ae4da-183">수리남</span><span class="sxs-lookup"><span data-stu-id="ae4da-183">Suriname</span></span>     |
> | <span data-ttu-id="ae4da-184">코모로</span><span class="sxs-lookup"><span data-stu-id="ae4da-184">Comoros</span></span>     | <span data-ttu-id="ae4da-185">마셜 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-185">Marshall Islands</span></span>     | <span data-ttu-id="ae4da-186">스발바르</span><span class="sxs-lookup"><span data-stu-id="ae4da-186">Svalbard</span></span>     |
> | <span data-ttu-id="ae4da-187">콩고</span><span class="sxs-lookup"><span data-stu-id="ae4da-187">Congo</span></span>     | <span data-ttu-id="ae4da-188">마르티니크</span><span class="sxs-lookup"><span data-stu-id="ae4da-188">Martinique</span></span>     | <span data-ttu-id="ae4da-189">스와질란드</span><span class="sxs-lookup"><span data-stu-id="ae4da-189">Swaziland</span></span>     |
> | <span data-ttu-id="ae4da-190">콩고 민주 공화국</span><span class="sxs-lookup"><span data-stu-id="ae4da-190">Congo (DRC)</span></span>     | <span data-ttu-id="ae4da-191">모리타니</span><span class="sxs-lookup"><span data-stu-id="ae4da-191">Mauritania</span></span>     | <span data-ttu-id="ae4da-192">동티모르</span><span class="sxs-lookup"><span data-stu-id="ae4da-192">Timor-Leste</span></span>   |
> | <span data-ttu-id="ae4da-193">쿡 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-193">Cook Islands</span></span>     | <span data-ttu-id="ae4da-194">마요트</span><span class="sxs-lookup"><span data-stu-id="ae4da-194">Mayotte</span></span>     | <span data-ttu-id="ae4da-195">토고</span><span class="sxs-lookup"><span data-stu-id="ae4da-195">Togo</span></span>   |
> | <span data-ttu-id="ae4da-196">지부티</span><span class="sxs-lookup"><span data-stu-id="ae4da-196">Djibouti</span></span>     | <span data-ttu-id="ae4da-197">미크로네시아</span><span class="sxs-lookup"><span data-stu-id="ae4da-197">Micronesia</span></span>     | <span data-ttu-id="ae4da-198">토켈라우</span><span class="sxs-lookup"><span data-stu-id="ae4da-198">Tokelau</span></span>   |
> | <span data-ttu-id="ae4da-199">도미니카</span><span class="sxs-lookup"><span data-stu-id="ae4da-199">Dominica</span></span>     | <span data-ttu-id="ae4da-200">몬트세라트</span><span class="sxs-lookup"><span data-stu-id="ae4da-200">Montserrat</span></span>     | <span data-ttu-id="ae4da-201">통가</span><span class="sxs-lookup"><span data-stu-id="ae4da-201">Tonga</span></span>   |
> | <span data-ttu-id="ae4da-202">적도 기니</span><span class="sxs-lookup"><span data-stu-id="ae4da-202">Equatorial Guinea</span></span>     | <span data-ttu-id="ae4da-203">모잠비크</span><span class="sxs-lookup"><span data-stu-id="ae4da-203">Mozambique</span></span>     | <span data-ttu-id="ae4da-204">터크스 케이커스 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-204">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="ae4da-205">에리트레아</span><span class="sxs-lookup"><span data-stu-id="ae4da-205">Eritrea</span></span>     | <span data-ttu-id="ae4da-206">미얀마</span><span class="sxs-lookup"><span data-stu-id="ae4da-206">Myanmar</span></span>     | <span data-ttu-id="ae4da-207">투발루</span><span class="sxs-lookup"><span data-stu-id="ae4da-207">Tuvalu</span></span>   |
> | <span data-ttu-id="ae4da-208">포클랜드 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-208">Falkland Islands</span></span>     | <span data-ttu-id="ae4da-209">나우루</span><span class="sxs-lookup"><span data-stu-id="ae4da-209">Nauru</span></span>     | <span data-ttu-id="ae4da-210">미국령 해외 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-210">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="ae4da-211">프랑스령 기아나</span><span class="sxs-lookup"><span data-stu-id="ae4da-211">French Guiana</span></span>     | <span data-ttu-id="ae4da-212">뉴칼레도니아</span><span class="sxs-lookup"><span data-stu-id="ae4da-212">New Caledonia</span></span>     | <span data-ttu-id="ae4da-213">바누아투</span><span class="sxs-lookup"><span data-stu-id="ae4da-213">Vanuatu</span></span>   |
> | <span data-ttu-id="ae4da-214">프랑스령 폴리네시아</span><span class="sxs-lookup"><span data-stu-id="ae4da-214">French Polynesia</span></span>     | <span data-ttu-id="ae4da-215">니제르</span><span class="sxs-lookup"><span data-stu-id="ae4da-215">Niger</span></span>     | <span data-ttu-id="ae4da-216">바티칸 시국</span><span class="sxs-lookup"><span data-stu-id="ae4da-216">Vatican City</span></span>   |
> | <span data-ttu-id="ae4da-217">프랑스 남부 지방</span><span class="sxs-lookup"><span data-stu-id="ae4da-217">French Southern Territories</span></span>     | <span data-ttu-id="ae4da-218">니우에</span><span class="sxs-lookup"><span data-stu-id="ae4da-218">Niue</span></span>     | <span data-ttu-id="ae4da-219">월리스 푸투나</span><span class="sxs-lookup"><span data-stu-id="ae4da-219">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="ae4da-220">가봉</span><span class="sxs-lookup"><span data-stu-id="ae4da-220">Gabon</span></span>     | <span data-ttu-id="ae4da-221">노퍽 섬</span><span class="sxs-lookup"><span data-stu-id="ae4da-221">Norfolk Island</span></span>     | <span data-ttu-id="ae4da-222">예멘</span><span class="sxs-lookup"><span data-stu-id="ae4da-222">Yemen</span></span>   |
> | <span data-ttu-id="ae4da-223">감비아</span><span class="sxs-lookup"><span data-stu-id="ae4da-223">Gambia</span></span>     | <span data-ttu-id="ae4da-224">북마리아나 제도</span><span class="sxs-lookup"><span data-stu-id="ae4da-224">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="ae4da-225">지브롤터</span><span class="sxs-lookup"><span data-stu-id="ae4da-225">Gibraltar</span></span>     | <span data-ttu-id="ae4da-226">팔라우</span><span class="sxs-lookup"><span data-stu-id="ae4da-226">Palau</span></span>       |    |

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="ae4da-227">고객을 대신하여 소프트웨어 구독 구입</span><span class="sxs-lookup"><span data-stu-id="ae4da-227">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="ae4da-228">고객을 대신하여 소프트웨어 구독을 구입하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-228">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="ae4da-229">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-229">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ae4da-230">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-230">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ae4da-231">고객의 세부 정보 페이지에서 **제품 추가** 를 선택한 다음, 화면의 지침에 따라 주문을 생성하고 결제합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-231">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="ae4da-232">오스트레일리아와 브라질을 제외한 나머지 국가에서는 모든 상용 가격에 세금이 포함되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-232">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="ae4da-233">오스트레일리아와 브라질은 가격에 세금이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-233">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="ae4da-234">소프트웨어 구독 활성화 및 관리</span><span class="sxs-lookup"><span data-stu-id="ae4da-234">Activate and manage software subscriptions</span></span>

<span data-ttu-id="ae4da-235">소프트웨어를 구매한 후에는 파트너 또는 파트너의 고객이 소프트웨어를 다운로드해야 합니다(파트너 센터를 사용하는 파트너, Microsoft 365 관리 센터를 사용하는 고객).</span><span class="sxs-lookup"><span data-stu-id="ae4da-235">Once you've purchased your software, you or your customers need to download it (partners using Partner Center; customers using the Microsoft 365 Admin Center).</span></span> <span data-ttu-id="ae4da-236">다음 절차를 사용 하 여이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-236">Use the following procedure to do this.</span></span> <span data-ttu-id="ae4da-237">링크 복사 및 소프트웨어 다운로드와 관련된 위험을 이해하는 것이 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-237">It’s important to understand the risks associated with copying links and downloading software.</span></span> <span data-ttu-id="ae4da-238">자세한 내용은 [파트너 센터 새 상거래 운영 가이드](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)의 **파트너 센터를 사용하여 고객 소프트웨어 다운로드 및 라이선스 키 가져오기** 를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ae4da-238">For more information, see **Using Partner Center to obtain customer software downloads and license keys** in the [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

>[!NOTE]
><span data-ttu-id="ae4da-239">키 및 다운로드의 링크를 얻으려면 파트너 센터에서 관리자 에이전트여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-239">You must be an Admin agent in Partner Center to obtain the link to keys and downloads.</span></span>

1. <span data-ttu-id="ae4da-240">고객의 세부 정보 페이지로 이동하여 **소프트웨어** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-240">Go to your customer's detail page, and then select **Software**.</span></span> <span data-ttu-id="ae4da-241">고객을 대신하여 구입한 모든 소프트웨어 목록이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-241">You'll see a list of all the software you've purchased on behalf of the customer.</span></span>

2. <span data-ttu-id="ae4da-242">제품 **버전**, **언어**, **비트** 를 선택하고 **키 및 다운로드 받기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-242">Choose product **version**, **language**, **bit**, and select **Get keys and downloads**.</span></span> 

3. <span data-ttu-id="ae4da-243">**키 받기** 를 선택하면 팝업 대화 상자에 32자리 제품 키가 표시되는데, 이 키를 복사하여 고객에게 전달하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-243">Choose **Get Key** to display the 32-digit product in a pop-up dialog box which you can copy and send to the customer.</span></span> 

4. <span data-ttu-id="ae4da-244">**다운로드** 를 선택하여 비트를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-244">Choose **Download** to download the bits.</span></span> 

5. <span data-ttu-id="ae4da-245">고객에게 비트 다운로드 링크를 보내려면 **링크 복사** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-245">Choose **Copy Link** if you want to send the customer the link to the bits download.</span></span> 

6. <span data-ttu-id="ae4da-246">소프트웨어 주문을 **취소** 하고 크레딧을 100% 받을 수도 있습니다(60일 취소 정책 기간 내에 취소하는 경우).</span><span class="sxs-lookup"><span data-stu-id="ae4da-246">You can also **Cancel** the software order and receive 100% credit (if done within the 60 days cancellation policy period).</span></span>

>[!NOTE]
><span data-ttu-id="ae4da-247">오직 고객만이 Microsoft 365 관리 센터에서 제품 키와 다운로드 정보를 볼 수 있습니다(전역 관리자 역할 필요).</span><span class="sxs-lookup"><span data-stu-id="ae4da-247">Only customers have access to see the product keys and download information in the Microsoft 365 Admin Center (Global Admin role required).</span></span> <span data-ttu-id="ae4da-248">파트너는 파트너 센터를 사용하여 이 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-248">Partners must use Partner Center to see this information.</span></span>

## <a name="server-subscription-download-and-license-keys-available-through-microsoft-365-admin-center-for-customers"></a><span data-ttu-id="ae4da-249">서버 구독 다운로드 및 라이선스 키는 Microsoft 365 관리 센터를 통해 고객에게 제공</span><span class="sxs-lookup"><span data-stu-id="ae4da-249">Server subscription download and license keys available through Microsoft 365 Admin Center for customers</span></span> 

<span data-ttu-id="ae4da-250">고객은 Microsoft 365 관리 센터에서 CSP 서버 구독 라이선스 키 및 다운로드를 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-250">Your customers will be able to get CSP server subscription license keys and downloads from Microsoft 365 Admin Center.</span></span> <span data-ttu-id="ae4da-251">CSP 서버 구독 라이선스 키 및 다운로드를 보려면 고객은 Microsoft 365 관리 센터 > **청구 > 제품 > 소프트웨어 탭** 으로 이동해야 합니다. 자세한 내용은 [청구에 있는 소프트웨어 탭](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ae4da-251">To see their CSP server subscription license keys and downloads, customer must go to Microsoft 365 Admin Center > **Billing > Your products > Software tab**. For more details, see [Software Tab under Billing](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions).</span></span>  

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="ae4da-252">소프트웨어 키 액세스 및 소프트웨어 다운로드에 대한 작업 보기</span><span class="sxs-lookup"><span data-stu-id="ae4da-252">View activity for software key access and software downloads</span></span>

<span data-ttu-id="ae4da-253">감사 또는 규정 준수를 위해, Server 구독 소프트웨어 키에 액세스하거나 Server 구독 소프트웨어를 다운로드한 사용자 목록을 확인해야 할 때가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-253">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="ae4da-254">아래 절차에 따라 이 정보를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-254">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="ae4da-255">이러한 활동 로그를 보려면 글로벌 관리자, 계정 관리자, 추천 관리자 또는 마케팅 콘텐츠 관리자여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-255">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="ae4da-256">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-256">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ae4da-257">오른쪽 위 모서리에서 기어 아이콘을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-257">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="ae4da-258">메뉴에서 **활동 로그** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-258">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="ae4da-259">보고 싶은 활동의 날짜 범위를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-259">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="ae4da-260">활동 로그에는 관리자가 지정한 시간 동안 소프트웨어 키에 액세스했거나 소프트웨어를 다운로드한 사용자 목록이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-260">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="ae4da-261">구입 취소</span><span class="sxs-lookup"><span data-stu-id="ae4da-261">Cancel a purchase</span></span>

<span data-ttu-id="ae4da-262">소프트웨어를 구매한 날짜로부터 60일 이내에 구매를 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-262">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="ae4da-263">60일 이내에 구매를 취소하면 조기 해지 수수료가 부과되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-263">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="ae4da-264">60일이 지나면 더 이상 구매를 취소할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-264">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="ae4da-265">(이 취소 규칙에 대한 주요 제한 사항을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ae4da-265">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="ae4da-266">소프트웨어 구매를 취소한 이후의 과정에 대한 자세한 내용은 다음 단계를 수행한 후 나오는 중요 메모를 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="ae4da-266">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="ae4da-267">구매를 취소하는 다음 단계는 구매 후 60일 이내처럼 특정 취소 기간 내에 취소된 소프트웨어에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-267">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="ae4da-268">Azure의 SUSE Linux 또는 RedHat 소프트웨어플랜에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-268">These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="ae4da-269">현재는 SUSE 또는 RedHat 소프트웨어 플랜을 취소하거나 교환할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-269">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="ae4da-270">SUSE Linux 또는 RedHat 플랜 사용에 대한 [자세한 정보](/azure/virtual-machines/linux/prepay-suse-software-charges)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="ae4da-270">[Learn more](/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="ae4da-271">구매를 취소하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-271">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="ae4da-272">구매를 취소하려면 관리 에이전트여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-272">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="ae4da-273">다음 단계에서는 파트너 센터 대시보드에서 구매를 취소하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-273">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="ae4da-274">[파트너 센터 API](/partner-center/develop/cancel-software-purchases)를 사용하여 취소할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-274">You can also do this using the [Partner Center API](/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="ae4da-275">취소 프로세스를 시작하기 전에, 먼저 다음 사항을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-275">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="ae4da-276">고객의 이름, 테넌트 GUID 또는 도메인 이름</span><span class="sxs-lookup"><span data-stu-id="ae4da-276">The customer's name, tenant GUID, or domain name</span></span>

    - <span data-ttu-id="ae4da-277">취소하려는 제품의 이름</span><span class="sxs-lookup"><span data-stu-id="ae4da-277">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="ae4da-278">주문 ID</span><span class="sxs-lookup"><span data-stu-id="ae4da-278">The Order ID</span></span>

2. <span data-ttu-id="ae4da-279">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-279">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="ae4da-280">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-280">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="ae4da-281">고객의 세부 정보 페이지에서 **소프트웨어** 를 선택하여 고객 대신 구매한 소프트웨어 목록을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-281">On the customer's details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="ae4da-282">취소하려는 소프트웨어 구매를 찾아서 **취소** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-282">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="ae4da-283">대화 상자가 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-283">A dialog box will appear.</span></span>

6. <span data-ttu-id="ae4da-284">주문 번호 드롭다운 목록에서 취소하려는 주문 ID 번호를 정확하게 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-284">From the Order number drop-down list, select the correct order ID number you want to cancel.</span></span> <span data-ttu-id="ae4da-285">(고객의 **주문 기록** 페이지에서 주문 또는 주문 ID 번호에 대한 자세한 내용을 확인할 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="ae4da-285">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

7. <span data-ttu-id="ae4da-286">구매 취소와 관련된 **중요한** 메시지를 읽었다는 확인란을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-286">Select the checkbox to acknowledge that you have read the **Important** message concerning cancellation.</span></span> <span data-ttu-id="ae4da-287">(구매를 취소한 이후의 과정에 대한 자세한 내용은 아래의 **중요** 메모를 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="ae4da-287">(Refer to the **Important** note below to learn more about what happens after you cancel a purchase.)</span></span>

8. <span data-ttu-id="ae4da-288">**제출** 을 선택하여 구매를 취소합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-288">Select **Submit** to cancel your purchase.</span></span> <span data-ttu-id="ae4da-289">고객의 여러 주문을 취소하려면 고유한 주문 ID 번호마다 4~6단계를 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-289">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span>

<span data-ttu-id="ae4da-290">주문을 취소하려고 시도할 때 파트너 센터에서 다른 정보를 제공할 수도 있습니다(주문 번호 드롭다운 목록 아래에 표시됨).</span><span class="sxs-lookup"><span data-stu-id="ae4da-290">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="ae4da-291">이 정보에는 다음 내용이 포함될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-291">This information can include:</span></span>

- <span data-ttu-id="ae4da-292">해당 주문을 취소할 수 있는 남은 일 수</span><span class="sxs-lookup"><span data-stu-id="ae4da-292">How many days remain for you to cancel that particular order</span></span>

- <span data-ttu-id="ae4da-293">취소 기간이 이미 지나 더 이상 주문을 취소할 수 없는지 여부</span><span class="sxs-lookup"><span data-stu-id="ae4da-293">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

- <span data-ttu-id="ae4da-294">파트너의 취소 요청에 대한 자세한 정보가 필요한 경우 Microsoft에서 파트너에게 **고객 지원 요청** 양식의 링크를 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-294">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="ae4da-295">주문을 취소하면 취소를 확인하는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-295">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="ae4da-296">하지만 파트너 센터 대시보드에 취소가 표시될 때까지 최대 15분이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-296">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> 

### <a name="post-cancellation-details"></a><span data-ttu-id="ae4da-297">사후 취소 세부 정보</span><span class="sxs-lookup"><span data-stu-id="ae4da-297">Post-cancellation details</span></span>

<span data-ttu-id="ae4da-298">구매를 취소한 이후의 과정:</span><span class="sxs-lookup"><span data-stu-id="ae4da-298">After you cancel a purchase:</span></span>

- <span data-ttu-id="ae4da-299">모든 관련 소프트웨어 키와 다운로드 링크가 해지됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-299">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="ae4da-300">즉, 파트너와 파트너의 고객은 해당 구매와 관련된 소프트웨어 키 및 다운로드 링크를 더 이상 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-300">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="ae4da-301">파트너와 파트너의 고객에게는 취소된 모든 소프트웨어의 사용 중단에 대한 책임이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-301">You and your customer are responsible for discontinuing the use of all canceled software.</span></span> <span data-ttu-id="ae4da-302">또한 파트너에게는 취소된 소프트웨어를 제거하고 관련 소프트웨어 다운로드 및 링크를 제거할 책임이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-302">You are also responsible for uninstalling the canceled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="ae4da-303">취소된 항목은 고객의 소프트웨어 세부 정보 페이지에 계속 표시되지만 활성화 키를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-303">The canceled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="ae4da-304">취소된 주문의 크레딧은 다음 달 청구서에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-304">A credit for the canceled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="ae4da-305">영구 소프트웨어는 크레딧을 100% 받고 소프트웨어 구독은 비례 배분 방식으로 계산된 크레딧을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-305">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="ae4da-306">구매를 취소해 달라는 고객 지원 요청 제출</span><span class="sxs-lookup"><span data-stu-id="ae4da-306">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="ae4da-307">파트너 센터를 통해 소프트웨어 구매를 취소하려고 했지만 추가 정보를 제공하고 고객 지원 요청 양식을 작성하라는 요청을 받은 경우 다음 단계를 수행하는 것이 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-307">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="ae4da-308">구입 취소 창에서 **고객 지원 요청** 링크를 선택하면 **파트너 센터에 문제 보고** 페이지가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-308">When you select the **customer support request** link from the Cancel purchase window, the **Report a problem with Partner Center** page will open.</span></span>

2. <span data-ttu-id="ae4da-309">**세부 정보** 의 문제 유형 목록에서 **고객을 대신하여 CSP 구입/환불** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-309">Under **Details**, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="ae4da-310">[영향] 및 [제목] 필드에 내용을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-310">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="ae4da-311">[설명] 필드에 다음 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-311">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="ae4da-312">고객 테넌트 GUID 또는 도메인 이름</span><span class="sxs-lookup"><span data-stu-id="ae4da-312">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="ae4da-313">주문 ID 또는 구독 ID</span><span class="sxs-lookup"><span data-stu-id="ae4da-313">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="ae4da-314">환불 이유</span><span class="sxs-lookup"><span data-stu-id="ae4da-314">Refund reason</span></span>

    - <span data-ttu-id="ae4da-315">요청된 금액</span><span class="sxs-lookup"><span data-stu-id="ae4da-315">Amount requested</span></span>

5. <span data-ttu-id="ae4da-316">[연락처] 필드에 이름, 이메일 주소 및 전화 번호를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-316">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="ae4da-317">어떤 이유로 파일을 첨부해야 하는 경우에는 **파일 추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-317">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="ae4da-318">이 단계는 선택 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-318">This step is optional.</span></span>

7. <span data-ttu-id="ae4da-319">모두 마쳤으면 **제출** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ae4da-319">When you're finished, select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae4da-320">다음 단계</span><span class="sxs-lookup"><span data-stu-id="ae4da-320">Next steps</span></span>

- [<span data-ttu-id="ae4da-321">파트너 센터를 사용하여 상용 마켓플레이스 제품에 대한 고객 구독 판매</span><span class="sxs-lookup"><span data-stu-id="ae4da-321">Use Partner Center to sell customers subscriptions to commercial marketplace products</span></span>](sell-marketplace-products.md)
 
- [<span data-ttu-id="ae4da-322">파트너 센터의 고객에게 Azure 구독 할당</span><span class="sxs-lookup"><span data-stu-id="ae4da-322">Assigning Azure subscriptions to customers in Partner Center</span></span>](assign-azure-subscriptions.md)