---
title: "CSP 지역 권한 설정 | 파트너 센터"
description: "이제 국제 비즈니스를 하는 파트너는 지역 권한 설정을 통해 전 세계 다양한 지역 및 국가에 있는 고객을 더 쉽게 관리할 수 있습니다."
ms.assetid: 22F9495E-E31A-41AE-BF51-3478AB2C8E78
author: MaggiePucciEvans
keywords: "Azure AD 테넌트, 사용자 테넌트 통합, CSP의 테넌트, CSP의 파트너 계정, CSP 시장 및 지역, CSP를 통해 어디에서 판매할 수 있나요?"
ms.openlocfilehash: 096f8421a9ccb95c00c79929124ed3c9adaf6933
ms.sourcegitcommit: e01a63d8b778668c560bc821275ddfcb0a6d4881
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2017
---
# <a name="tenant-consolidation-strategies-in-csp"></a><span data-ttu-id="f037a-104">CSP의 테넌트 통합 전략</span><span class="sxs-lookup"><span data-stu-id="f037a-104">Tenant consolidation strategies in CSP</span></span>


<span data-ttu-id="f037a-105">\[일부 정보는 상업용으로 출시되기 전에 상당 부분 수정될 수 있는 시험판 제품과 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-105">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="f037a-106">Microsoft는 여기에 제공된 정보에 대해 명시적 또는 묵시적 보증을 하지 않습니다.\]</span><span class="sxs-lookup"><span data-stu-id="f037a-106">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="f037a-107">이제 국제 비즈니스를 하는 파트너는 지역 권한 설정을 통해 전 세계 다양한 지역 및 국가에 있는 고객을 더 쉽게 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-107">With regional authorization, partners with international businesses can now more easily manage customers in different regions and countries around the world.</span></span> <span data-ttu-id="f037a-108">따라서 파트너가 관리해야 하는 테넌트 수가 줄어들고, 파트너가 처리해야 하는 청구 날짜가 줄어들며, 파트너가 영업에 대한 더 통합된 보기를 이용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-108">This reduces the number of tenants that partners need to manage, reduces the billing dates that partners have to handle, and gives partners a more consolidated view of their sales.</span></span>

<span data-ttu-id="f037a-109">과거에는 유럽 연합/EFTA를 제외하고는 파트너가 거래하기를 원하는 각 국가에 실제 업체가 있어야 했습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-109">In the past, with the exception of the European Union/EFTA, partners needed to have a physical entity in each country where they wanted to transact.</span></span> <span data-ttu-id="f037a-110">즉, 파트너가 파트너 센터에서 청구 날짜와 기타 설정이 여러 개인 다중 테넌트를 설정해야 했습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-110">This meant that partners needed to have multiple tenants set up in Partner Center, with multiple billing dates and other settings.</span></span> <span data-ttu-id="f037a-111">라틴 아메리카와 같은 지역에서는 파트너가 인접 지역 또는 국가에 있는 고객과 쉽게 작업할 수 없었으며, 일부 경우 완전히 제한되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-111">In regions such as Latin America, partners were not able to easily work with customers in a neighboring region or country, and in some cases, they were restricted completely.</span></span>

>**<span data-ttu-id="f037a-112">참고</span><span class="sxs-lookup"><span data-stu-id="f037a-112">Note</span></span>**<br> <span data-ttu-id="f037a-113">[Microsoft 클라우드 독일 CSP](partner-center-for-microsoft-cloud-germany.md)에 등록되어 있고 EU 및 EFTA 국가/지역의 고객에게 판매하는 경우 Microsoft 클라우드 독일 파트너 센터의 테넌트를 다른 테넌트와 통합할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-113">If you are enrolled in [CSP for Microsoft Cloud Germany](partner-center-for-microsoft-cloud-germany.md) and you sell to customers in the EU and EFTA countries/regions, you cannot consolidate your tenant for Partner Center for Microsoft Cloud Germany with your other tenants.</span></span>  

## <a name="planning"></a><span data-ttu-id="f037a-114">계획</span><span class="sxs-lookup"><span data-stu-id="f037a-114">Planning</span></span>

<span data-ttu-id="f037a-115">아래에 설명된 것처럼 파트너는 지역 테넌트를 통합하는 여러 옵션을 이용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-115">Partners have multiple options for consolidating their regional tenants, as outlined below.</span></span>

### <a name="separate-tenants-for-single-regions-or-countries"></a><span data-ttu-id="f037a-116">단일 지역 또는 국가에 대한 별도 테넌트</span><span class="sxs-lookup"><span data-stu-id="f037a-116">Separate tenants for single regions or countries</span></span>

<span data-ttu-id="f037a-117">테넌트 통합은 옵션입니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-117">Tenant consolidation is optional.</span></span> <span data-ttu-id="f037a-118">다음 표에 표시된 것처럼 파트너는 별도 테넌트가 있는 국제 고객을 계속 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-118">Partners can continue to manage their international customers with separate tenants, as shown in the following table.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f037a-119">파트너 위치</span><span class="sxs-lookup"><span data-stu-id="f037a-119">Partner location(s)</span></span></th>
<th><span data-ttu-id="f037a-120">청구 날짜</span><span class="sxs-lookup"><span data-stu-id="f037a-120">Billing Date(s)</span></span></th>
<th><span data-ttu-id="f037a-121">고객 위치</span><span class="sxs-lookup"><span data-stu-id="f037a-121">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="f037a-122">콜롬비아</span><span class="sxs-lookup"><span data-stu-id="f037a-122">Colombia</span></span></p></td>
<td><p><span data-ttu-id="f037a-123">청구 날짜 10일</span><span class="sxs-lookup"><span data-stu-id="f037a-123">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="f037a-124">콜롬비아</span><span class="sxs-lookup"><span data-stu-id="f037a-124">Colombia</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f037a-125">칠레</span><span class="sxs-lookup"><span data-stu-id="f037a-125">Chile</span></span></p></td>
<td><p><span data-ttu-id="f037a-126">청구 날짜 15일</span><span class="sxs-lookup"><span data-stu-id="f037a-126">Billing date 15th</span></span></p></td>
<td><p><span data-ttu-id="f037a-127">칠레</span><span class="sxs-lookup"><span data-stu-id="f037a-127">Chile</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="f037a-128">파라과이</span><span class="sxs-lookup"><span data-stu-id="f037a-128">Paraguay</span></span></p></td>
<td><p><span data-ttu-id="f037a-129">청구 날짜 5일</span><span class="sxs-lookup"><span data-stu-id="f037a-129">Billing date 5th</span></span></p></td>
<td><p><span data-ttu-id="f037a-130">파라과이</span><span class="sxs-lookup"><span data-stu-id="f037a-130">Paraguay</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f037a-131">페루</span><span class="sxs-lookup"><span data-stu-id="f037a-131">Peru</span></span></p></td>
<td><p><span data-ttu-id="f037a-132">청구 날짜 2일</span><span class="sxs-lookup"><span data-stu-id="f037a-132">Billing date 2nd</span></span></p></td>
<td><p><span data-ttu-id="f037a-133">페루</span><span class="sxs-lookup"><span data-stu-id="f037a-133">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="one-tenant-for-multiple-regions-or-countries"></a><span data-ttu-id="f037a-134">여러 지역 또는 국가 대한 하나의 테넌트</span><span class="sxs-lookup"><span data-stu-id="f037a-134">One tenant for multiple regions or countries</span></span>


<span data-ttu-id="f037a-135">파트너는 여러 CSP 테넌트에서 단일 CSP 테넌트로의 작업을 통합하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-135">Partners can choose to consolidate their operations from multiple CSP tenants into a single CSP tenant.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f037a-136">파트너 위치</span><span class="sxs-lookup"><span data-stu-id="f037a-136">Partner location</span></span></th>
<th><span data-ttu-id="f037a-137">청구 날짜</span><span class="sxs-lookup"><span data-stu-id="f037a-137">Billing Date</span></span></th>
<th><span data-ttu-id="f037a-138">고객 위치</span><span class="sxs-lookup"><span data-stu-id="f037a-138">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="f037a-139">콜롬비아</span><span class="sxs-lookup"><span data-stu-id="f037a-139">Colombia</span></span></p></td>
<td><p><span data-ttu-id="f037a-140">청구 날짜 10일</span><span class="sxs-lookup"><span data-stu-id="f037a-140">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="f037a-141">콜롬비아</span><span class="sxs-lookup"><span data-stu-id="f037a-141">Colombia</span></span></p>
<p><span data-ttu-id="f037a-142">칠레</span><span class="sxs-lookup"><span data-stu-id="f037a-142">Chile</span></span></p>
<p><span data-ttu-id="f037a-143">파라과이</span><span class="sxs-lookup"><span data-stu-id="f037a-143">Paraguay</span></span></p>
<p><span data-ttu-id="f037a-144">페루</span><span class="sxs-lookup"><span data-stu-id="f037a-144">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="some-tenants-for-some-regions-or-countries"></a><span data-ttu-id="f037a-145">일부 지역 또는 국가에 대한 일부 테넌트</span><span class="sxs-lookup"><span data-stu-id="f037a-145">Some tenants for some regions or countries</span></span>


<span data-ttu-id="f037a-146">파트너는 여러 CSP 테넌트에서 소수의 CSP 테넌트로의 작업을 통합하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-146">Partners can choose to consolidate their operations from multiple CSP tenants to fewer CSP tenants.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f037a-147">파트너 위치</span><span class="sxs-lookup"><span data-stu-id="f037a-147">Partner location(s)</span></span></th>
<th><span data-ttu-id="f037a-148">청구 날짜</span><span class="sxs-lookup"><span data-stu-id="f037a-148">Billing Date(s)</span></span></th>
<th><span data-ttu-id="f037a-149">고객 위치</span><span class="sxs-lookup"><span data-stu-id="f037a-149">Customer location(s)</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="f037a-150">콜롬비아</span><span class="sxs-lookup"><span data-stu-id="f037a-150">Colombia</span></span></p></td>
<td><p><span data-ttu-id="f037a-151">청구 날짜 10일</span><span class="sxs-lookup"><span data-stu-id="f037a-151">Billing date 10th</span></span></p></td>
<td><p><span data-ttu-id="f037a-152">콜롬비아</span><span class="sxs-lookup"><span data-stu-id="f037a-152">Colombia</span></span></p>
<p><span data-ttu-id="f037a-153">칠레</span><span class="sxs-lookup"><span data-stu-id="f037a-153">Chile</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f037a-154">파라과이</span><span class="sxs-lookup"><span data-stu-id="f037a-154">Paraguay</span></span></p></td>
<td><p><span data-ttu-id="f037a-155">청구 날짜 5일</span><span class="sxs-lookup"><span data-stu-id="f037a-155">Billing date 5th</span></span></p></td>
<td><p><span data-ttu-id="f037a-156">파라과이</span><span class="sxs-lookup"><span data-stu-id="f037a-156">Paraguay</span></span></p>
<p><span data-ttu-id="f037a-157">페루</span><span class="sxs-lookup"><span data-stu-id="f037a-157">Peru</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a name="consolidating-tenants"></a><span data-ttu-id="f037a-158">테넌트 통합</span><span class="sxs-lookup"><span data-stu-id="f037a-158">Consolidating tenants</span></span>


<span data-ttu-id="f037a-159">테넌트를 통합하려는 경우 다음과 같이 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-159">If you want to consolidate tenants, we recommend the following:</span></span>

-   <span data-ttu-id="f037a-160">**여러 지역/국가, 하나의 거래**.</span><span class="sxs-lookup"><span data-stu-id="f037a-160">**Multiple regions/countries but only one transacting**.</span></span> <span data-ttu-id="f037a-161">한 국가/지역에서만 거래하지만 설정된 다른 테넌트가 여러 개인 경우 거래 테넌트를 해당 지역에 대한 새 중앙 집중식 테넌트로 사용하고 다른 테넌트를 취소합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-161">If you are only transacting in one country/region, but have a number of other tenants set up, use the transacting tenant as your new centralized tenant for that region and cancel your other tenants.</span></span>

-   **<span data-ttu-id="f037a-162">여러 국가/지역, 하나의 거래.</span><span class="sxs-lookup"><span data-stu-id="f037a-162">Multiple countries/regions but only one Transacting.</span></span>** <span data-ttu-id="f037a-163">여러 국가/지역에서 거래하는 경우 최대 실제 사용자 수가 포함된 테넌트로 중앙 집중화하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-163">If you are transacting in a number of countries/regions, we recommend that you centralize to the tenant with the largest number of seats.</span></span> <span data-ttu-id="f037a-164">실제 사용자 수가 적은 국가/지역의 구독을 취소해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-164">You should cancel the subscriptions in the countries/regions where you have smaller amounts of seats.</span></span>


## <a name="countryregion-information"></a><span data-ttu-id="f037a-165">국가/지역 정보</span><span class="sxs-lookup"><span data-stu-id="f037a-165">Country/region information</span></span>


<span data-ttu-id="f037a-166">테넌트 통합을 시작하기 전에 다음을 고려하세요.</span><span class="sxs-lookup"><span data-stu-id="f037a-166">Consider the following before beginning consolidating tenants:</span></span>

-   <span data-ttu-id="f037a-167">**Microsoft 판매 대상 위치가 미국인 경우** 지역은 미국에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-167">**If your Microsoft sell-to location is the United States**, your Territory includes customers located in the United States.</span></span>

-   <span data-ttu-id="f037a-168">**Microsoft 판매 대상 위치가 캐나다인 경우** 지역은 캐나다에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-168">**If your Microsoft sell-to location is Canada**, your Territory includes customers located in Canada.</span></span>

-   <span data-ttu-id="f037a-169">**Microsoft 판매 대상 위치가 브라질인 경우** 지역은 브라질에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-169">**If your Microsoft sell-to location is Brazil**, your Territory includes customers located in Brazil.</span></span>

-   <span data-ttu-id="f037a-170">**Microsoft 판매 대상 위치가 다음 목록에 있는 국가/지역인 경우** 귀사의 지역에는 다음 목록에 있는 모든 국가/지역의 고객이 포함됩니다. 국가/지역: 앵귈라, 앤티가 바부다, 아르헨티나, 아루바, 바하마, 바베이도스, 벨리즈, 버뮤다, 볼리비아, 보네르, 사바 및 세인트외수타티우스, 케이맨 제도, 칠레, 콜롬비아, 코스타리카, 쿠라사오, 도미니카 공화국, 에콰도르, 엘살바도르, 프랑스령 기아나, 과들루프, 과테말라, 온두라스, 자메이카, 마르티니크, 멕시코, 니카라과, 파나마, 파라과이, 페루, 푸에르토리코, 세인트 크리스토퍼 네비스, 세인트 루시아, 생 마르탱, 세인트 빈센트 그레나딘, 신트마르텐, 수리남, 트리니다드 토바고, 터크스 케이커스 제도, 우루과이, 베네수엘라, 미국령 버전 아일랜드.</span><span class="sxs-lookup"><span data-stu-id="f037a-170">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Anguilla, Antigua and Barbuda, Argentina, Aruba, Bahamas, Barbados, Belize, Bermuda, Bolivia, Bonaire, Saba, and Sint Eustatius, Cayman Islands, Chile, Colombia, Costa Rica, Curacao, Dominican Republic, Ecuador, El Salvador, French Guiana, Guadeloupe, Guatemala, Honduras, Jamaica, Martinique, Mexico, Nicaragua, Panama, Paraguay, Peru, Puerto Rico, Saint Kitts and Nevis, Saint Lucia, Saint Martin, Saint Vincent and the Grenadines, Sint Maarten, Suriname, Trinidad and Tobago, Turks and Caicos Islands, Uruguay, Venezuela, U.S. Virgin Islands.</span></span>

-   <span data-ttu-id="f037a-171">**Microsoft 판매 대상 위치가 다음 목록에 있는 국가/지역인 경우** 귀사의 지역에는 다음 목록에 있는 모든 국가/지역의 고객이 포함됩니다. 국가/지역: 안도라, 오스트리아, 벨기에, 불가리아, 크로아티아, 키프로스, 체코 공화국, 덴마크, 에스토니아, 페로 제도, 핀란드, 프랑스, 독일, 그리스, 그린란드, 헝가리, 아이슬란드, 아일랜드, 맨 섬, 이탈리아, 저지, 라트비아, 리히텐슈타인, 리투아니아, 룩셈부르크, 마다가스카르, 말라위, 말리, 몰타, 마요트, 모나코, 네덜란드, 뉴칼레도니아, 노르웨이, 폴란드, 포르투갈, 루마니아, 산마리노, 슬로바키아, 슬로베니아, 스페인, 스웨덴, 스위스, 영국, 바티칸.</span><span class="sxs-lookup"><span data-stu-id="f037a-171">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Andorra, Austria, Belgium, Bulgaria, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Faroe Islands, Finland, France, Germany, Greece, Greenland, Hungary, Iceland, Ireland, Isle of Man, Italy, Jersey, Latvia, Liechtenstein, Lithuania, Luxembourg, Madagascar, Malawi, Mali, Malta, Mayotte, Monaco, Netherlands, New Caledonia, Norway, Poland, Portugal, Romania, San Marino, Slovakia, Slovenia, Spain, Sweden, Switzerland, United Kingdom, Vatican City.</span></span>

    >**<span data-ttu-id="f037a-172">참고</span><span class="sxs-lookup"><span data-stu-id="f037a-172">Note</span></span>**<br> <span data-ttu-id="f037a-173">[Microsoft 클라우드 독일 CSP](partner-center-for-microsoft-cloud-germany.md)에 등록되어 있고 EU 및 EFTA 국가/지역의 고객에게 판매하는 경우 Microsoft 클라우드 독일 파트너 센터의 테넌트를 다른 테넌트와 통합할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-173">If you are enrolled in [CSP for Microsoft Cloud Germany](partner-center-for-microsoft-cloud-germany.md) and you sell to customers in the EU and EFTA countries/regions, you cannot consolidate your tenant for Partner Center for Microsoft Cloud Germany with your other tenants.</span></span>  


-   <span data-ttu-id="f037a-174">**Microsoft 판매 대상 위치가 다음 목록에 있는 국가/지역인 경우** 귀사의 지역에는 다음 목록에 있는 모든 국가/지역의 고객이 포함됩니다. 국가/지역: 아프가니스탄, 알바니아, 알제리, 아르메니아, 아제르바이잔, 바레인, 벨라루스, 베냉, 보스니아 헤르체고비나, 부룬디, 코모로, 이집트, 프랑스령 폴리네시아, 조지아, 이라크, 이스라엘, 요르단, 카자흐스탄, 쿠웨이트, 키르기스스탄, 레바논, 리비아, 마케도니아(FYROM), 몰도바, 몽골, 몬테네그로, 모로코, 모잠비크, 오만, 파키스탄, 팔레스타인 자치 정부, 카타르, 리유니언, 사우디아라비아, 세르비아, 세이셸, 남아프리카 공화국, 타지키스탄, 토고, 튀니지, 터키, 투르크메니스탄, 우크라이나, 아랍에미리트연합국, 우즈베키스탄, 예멘, 짐바브웨.</span><span class="sxs-lookup"><span data-stu-id="f037a-174">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Afghanistan, Albania, Algeria, Armenia, Azerbaijan, Bahrain, Belarus, Benin, Bosnia and Herzegovina, Burundi, Comoros, Egypt, French Polynesia, Georgia, Iraq, Israel, Jordan, Kazakhstan, Kuwait, Kyrgyzstan, Lebanon, Libya, Republic of Macedonia (FYROM), Moldova, Mongolia, Montenegro, Morocco, Mozambique, Oman, Pakistan, Palestinian Authority, Qatar, Reunion, Saudi Arabia, Serbia, Seychelles, South Africa, Tajikistan, Togo, Tunisia, Turkey, Turkmenistan, Ukraine, United Arab Emirates, Uzbekistan, Yemen, Zimbabwe.</span></span>

-   <span data-ttu-id="f037a-175">**Microsoft 판매 대상 위치가 다음 목록에 있는 국가/지역인 경우** 귀사의 지역에는 다음 목록에 있는 모든 국가/지역의 고객이 포함됩니다. 국가/지역: 앙골라, 보츠와나, 카메룬, 카보베르데, 코트디부아르, 에티오피아, 가나, 케냐, 모리셔스, 나미비아, 나이지리아, 르완다, 세네갈, 탄자니아, 우간다, 잠비아.</span><span class="sxs-lookup"><span data-stu-id="f037a-175">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Angola, Botswana, Cameroon, Cabo Verde, Côte d'Ivoire, Ethiopia, Ghana, Kenya, Mauritius, Namibia, Nigeria, Rwanda, Senegal, Tanzania, Uganda, Zambia.</span></span>

-   <span data-ttu-id="f037a-176">**Microsoft 판매 대상 위치가 러시아인 경우** 지역은 러시아에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-176">**If your Microsoft sell-to location is Russia**, your Territory includes customers located in Russia.</span></span>

-   <span data-ttu-id="f037a-177">**Microsoft 판매 대상 위치가 다음 목록에 있는 국가/지역인 경우** 귀사의 지역에는 다음 목록에 있는 모든 국가/지역의 고객이 포함됩니다. 국가/지역: 방글라데시, 부탄, 브루나이, 캄보디아, 홍콩 특별 행정구, 인도네시아, 라오스, 마카오 특별 행정구, 말레이시아, 몰디브, 마샬 제도, 미얀마, 네팔, 파푸아뉴기니, 필리핀, 싱가포르, 스리랑카, 태국, 동티모르, 통가, 베트남.</span><span class="sxs-lookup"><span data-stu-id="f037a-177">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Bangladesh, Bhutan, Brunei Darussalam, Cambodia, Hong Kong SAR, Indonesia, Laos, Macao SAR, Malaysia, Maldives, Marshall Islands, Myanmar, Nepal, Papua New Guinea, Philippines, Singapore, Sri Lanka, Thailand, Timor-Leste, Tonga, Vietnam.</span></span>

-   <span data-ttu-id="f037a-178">**Microsoft 판매 대상 위치가 다음 목록에 있는 국가/지역인 경우** 귀사의 지역에는 다음 목록에 있는 모든 국가/지역의 고객이 포함됩니다. 국가/지역: 오스트레일리아 또는 피지.</span><span class="sxs-lookup"><span data-stu-id="f037a-178">**If your Microsoft sell-to location is a country/region on the following list**, your Territory includes customers located in any country/region in the following list: Australia or Fiji.</span></span>

-   <span data-ttu-id="f037a-179">**Microsoft 판매 대상 위치가 뉴질랜드인 경우** 지역은 뉴질랜드에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-179">**If your Microsoft sell-to location is New Zealand**, your Territory includes customers located in New Zealand.</span></span>

-   <span data-ttu-id="f037a-180">**Microsoft 판매 대상 위치가 인도인 경우** 지역은 인도에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-180">**If your Microsoft sell-to location is India**, your Territory includes customers located in India.</span></span>

-   <span data-ttu-id="f037a-181">**Microsoft 판매 대상 위치가 일본인 경우** 지역은 일본에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-181">**If your Microsoft sell-to location is Japan**, your Territory includes customers located in Japan.</span></span>

-   <span data-ttu-id="f037a-182">**Microsoft 판매 대상 위치가 한국인 경우** 지역은 한국에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-182">**If your Microsoft sell-to location is Korea**, your Territory includes customers located in Korea.</span></span>

-   <span data-ttu-id="f037a-183">**Microsoft 판매 대상 위치가 대만인 경우** 지역은 대만에 있는 고객을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-183">**If your Microsoft sell-to location is Taiwan**, your Territory includes customers located in Taiwan.</span></span>

## <a name="billing-currencies-by-country"></a><span data-ttu-id="f037a-184">국가별 청구 통화</span><span class="sxs-lookup"><span data-stu-id="f037a-184">Billing currencies by country</span></span>

<span data-ttu-id="f037a-185">다음 표와 같이 지리적 위치에 따라 청구 통화가 결정됩니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-185">Your geographic location determines the currency in which you are billed, as shown in the following table.</span></span> <span data-ttu-id="f037a-186">다른 청구 통화를 사용하려는 경우 세금 및 법적 책임 때문에 새로운 테넌트를 만들고 해당 통화를 지정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f037a-186">Note that due to tax and legal implications, if you want to use a different billing currency, you'll need to create a new tenant and specify that currency.</span></span> 

| <span data-ttu-id="f037a-187">통화</span><span class="sxs-lookup"><span data-stu-id="f037a-187">Currency</span></span> | <span data-ttu-id="f037a-188">국가</span><span class="sxs-lookup"><span data-stu-id="f037a-188">Country</span></span> |
| ---- | ---- |
| <span data-ttu-id="f037a-189">USD</span><span class="sxs-lookup"><span data-stu-id="f037a-189">USD</span></span> | <span data-ttu-id="f037a-190">알바니아, 앵귈라, 앤티가 바부다, 아르헨티나, 아르메니아, 아루바, 아제르바이잔, 바하마, 바레인, 방글라데시, 바베이도스, 벨로루시, 벨리즈, 베냉, 버뮤다, 볼리비아, 보네르, 사바 및 세인트외수타티우스, 브라질, 브루나이, 부룬디, 카메룬, 케이맨 제도, 칠레, 콜롬비아, 코모로, 코스타리카, 퀴라소, 도미니카 공화국, 에콰도르, 이집트, 엘살바도르, 프랑스령 기아나, 프랑스령 폴리네시아, 조지아, 가나, 과테말라, 온두라스, 홍콩 특별 행정구, 인도네시아, 이라크, 이스라엘, 자메이카, 카자흐스탄, 케냐, 쿠웨이트, 키르기스스탄, 레바논, 마카오 특별 행정구, 마다가스카르, 말라위, 말레이시아, 말리, 모리셔스, 마요트, 멕시코, 모로코, 나미비아, 뉴칼레도니아, 니카라과, 나이지리아, 오만, 파키스탄, 파나마, 파라과이, 페루, 필리핀, 푸에르토리코, 카타르, 리유니언, 르완다, 세인트 루시아, 생 마르탱, 세인트 빈센트 그레나딘, 사우디아라비아, 세르비아, 세이셸, 싱가포르, 신트마르텐, 남아프리카 공화국, 스리랑카, 수리남, 탄자니아, 태국, 동티모르, 토고, 트리니다드 토바고, 튀니지, 터키, 터크스 케이커스 제도, 미국령 버전 아일랜드, 우크라이나 아랍에미리트, 미국, 우루과이, 베네수엘라, 베트남</span><span class="sxs-lookup"><span data-stu-id="f037a-190">Albania, Anguilla, Antigua and Barbuda, Argentina, Armenia, Aruba, Azerbaijan, Bahamas, Bahrain, Bangladesh, Barbados, Belarus, Belize, Benin, Bermuda, Bolivia, Bonaire, Saba, and Sint Eustatius, Brazil, Brunei, Burundi, Cameroon, Cayman Islands, Chile, Colombia, Comoros, Costa Rica, Curaçao, Dominican Republic, Ecuador, Egypt, El Salvador, French Guiana, French Polynesia, Georgia, Ghana, Guatemala, Honduras, Hong Kong SAR, Indonesia, Iraq, Israel, Jamaica, Kazakhstan, Kenya, Kuwait, Kyrgyzstan, Lebanon, Macao SAR, Madagascar, Malawi, Malaysia, Mali, Mauritius, Mayotte, Mexico, Morocco, Namibia, New Caledonia, Nicaragua, Nigeria, Oman, Pakistan, Panama, Paraguay, Peru, Philippines, Puerto Rico, Qatar, Reunion, Rwanda, Saint Lucia, Saint Martin, Saint Vincent and the Grenadines, Saudi Arabia, Serbia, Seychelles, Singapore, Sint Maarten, South Africa, Sri Lanka, Suriname, Tanzania, Thailand, Timor-Leste, Togo, Trinidad and Tobago, Tunisia, Turkey, Turks and Caicos Islands, U.S. Virgin Islands, Ukraine, United Arab Emirates, United States, Uruguay, Venezuela, Vietnam</span></span>  | 
| <span data-ttu-id="f037a-191">TWD</span><span class="sxs-lookup"><span data-stu-id="f037a-191">TWD</span></span> | <span data-ttu-id="f037a-192">대만</span><span class="sxs-lookup"><span data-stu-id="f037a-192">Taiwan</span></span> |
| <span data-ttu-id="f037a-193">SEK</span><span class="sxs-lookup"><span data-stu-id="f037a-193">SEK</span></span> | <span data-ttu-id="f037a-194">스웨덴</span><span class="sxs-lookup"><span data-stu-id="f037a-194">Sweden</span></span> |
| <span data-ttu-id="f037a-195">INR</span><span class="sxs-lookup"><span data-stu-id="f037a-195">INR</span></span> | <span data-ttu-id="f037a-196">인도</span><span class="sxs-lookup"><span data-stu-id="f037a-196">India</span></span> |
| <span data-ttu-id="f037a-197">RUB</span><span class="sxs-lookup"><span data-stu-id="f037a-197">RUB</span></span> | <span data-ttu-id="f037a-198">러시아</span><span class="sxs-lookup"><span data-stu-id="f037a-198">Russia</span></span> |
| <span data-ttu-id="f037a-199">NZD</span><span class="sxs-lookup"><span data-stu-id="f037a-199">NZD</span></span> | <span data-ttu-id="f037a-200">뉴질랜드</span><span class="sxs-lookup"><span data-stu-id="f037a-200">New Zealand</span></span> |
| <span data-ttu-id="f037a-201">NOK</span><span class="sxs-lookup"><span data-stu-id="f037a-201">NOK</span></span> | <span data-ttu-id="f037a-202">노르웨이</span><span class="sxs-lookup"><span data-stu-id="f037a-202">Norway</span></span> |
| <span data-ttu-id="f037a-203">KRW</span><span class="sxs-lookup"><span data-stu-id="f037a-203">KRW</span></span> | <span data-ttu-id="f037a-204">한국</span><span class="sxs-lookup"><span data-stu-id="f037a-204">Korea</span></span> |
| <span data-ttu-id="f037a-205">JPY</span><span class="sxs-lookup"><span data-stu-id="f037a-205">JPY</span></span> | <span data-ttu-id="f037a-206">일본</span><span class="sxs-lookup"><span data-stu-id="f037a-206">Japan</span></span> |
| <span data-ttu-id="f037a-207">GBP</span><span class="sxs-lookup"><span data-stu-id="f037a-207">GBP</span></span> | <span data-ttu-id="f037a-208">맨 섬, 저지, 영국</span><span class="sxs-lookup"><span data-stu-id="f037a-208">Isle of Man, Jersey, United Kingdom</span></span> |
| <span data-ttu-id="f037a-209">EUR</span><span class="sxs-lookup"><span data-stu-id="f037a-209">EUR</span></span> | <span data-ttu-id="f037a-210">안도라, 오스트리아, 벨기에, 크로아티아, 체코 공화국, 에스토니아, 페로 제도, 핀란드, 프랑스, 독일, 그리스, 헝가리, 아이슬란드, 아일랜드, 이탈리아, 라트비아, 리히텐슈타인, 리투아니아, 룩셈부르크/벨기에, 네덜란드, 폴란드, 포르투갈, 루마니아, 산마리노, 슬로바키아, 슬로베니아, 스페인</span><span class="sxs-lookup"><span data-stu-id="f037a-210">Andorra, Austria, Belgium, Croatia, Czech Republic, Estonia, Faroe Islands, Finland, France, Germany, Greece, Hungary, Iceland, Ireland, Italy, Latvia, Liechtenstein, Lithuania, Luxembourg/Belgium, Netherlands, Poland, Portugal, Romania, San Marino, Slovakia, Slovenia, Spain</span></span> |
| <span data-ttu-id="f037a-211">DKK</span><span class="sxs-lookup"><span data-stu-id="f037a-211">DKK</span></span> | <span data-ttu-id="f037a-212">덴마크</span><span class="sxs-lookup"><span data-stu-id="f037a-212">Denmark</span></span> |
| <span data-ttu-id="f037a-213">CHF</span><span class="sxs-lookup"><span data-stu-id="f037a-213">CHF</span></span> | <span data-ttu-id="f037a-214">스위스</span><span class="sxs-lookup"><span data-stu-id="f037a-214">Switzerland</span></span> |
| <span data-ttu-id="f037a-215">CAD</span><span class="sxs-lookup"><span data-stu-id="f037a-215">CAD</span></span> | <span data-ttu-id="f037a-216">캐나다</span><span class="sxs-lookup"><span data-stu-id="f037a-216">Canada</span></span> |
| <span data-ttu-id="f037a-217">AUD</span><span class="sxs-lookup"><span data-stu-id="f037a-217">AUD</span></span> | <span data-ttu-id="f037a-218">오스트레일리아, 피지, 마샬 제도, 파푸아뉴기니, 통가</span><span class="sxs-lookup"><span data-stu-id="f037a-218">Australia, Fiji, Marshall Islands, Papua New Guinea, Tonga</span></span> |


 



