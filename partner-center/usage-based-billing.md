---
title: 사용량 기반 청구
ms.topic: article
ms.date: 06/05/2020
Description: 월별 사용 요금에 대 한 요금이 청구 되는 파트너 센터의 사용량 기반 요금 청구에 대해 자세히 알아보세요.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4b3c3626bea685a8751ffcc5aa877fd95824e693
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436462"
---
# <a name="understand-usage-based-billing-for-monthly-pay-as-you-go-consumption-of-services"></a><span data-ttu-id="53a40-103">월간 종 량 제 사용량에 대 한 사용량 기반 청구 이해</span><span class="sxs-lookup"><span data-stu-id="53a40-103">Understand usage-based billing for monthly, pay-as-you-go consumption of services</span></span>

- <span data-ttu-id="53a40-104">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="53a40-104">Partner Center</span></span>
- <span data-ttu-id="53a40-105">CSP 프로그램의 파트너</span><span class="sxs-lookup"><span data-stu-id="53a40-105">Partners in the CSP program</span></span>

<span data-ttu-id="53a40-106">Azure 구독과 같은 온라인 서비스를 구매 하는 경우 월간 사용 요금에 대 한 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-106">When you buy online services such as Azure subscriptions, you're billed for monthly usage rates.</span></span> <span data-ttu-id="53a40-107">Azure와 같은 사용량 기반 서비스는 사용량을 기준으로 계량 요금에 따라 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-107">Usage-based services, such as Azure, are billed according to metered rates, based on consumption.</span></span>

<span data-ttu-id="53a40-108">일부 Microsoft 제품 및 서비스에서는 사용 되는 서비스에 대해서만 요금이 청구 되는 "종 량 제" 청구 모델을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-108">Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used.</span></span> <span data-ttu-id="53a40-109">예를 들어 Microsoft Azure은이 모델을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-109">For example, Microsoft Azure uses this model.</span></span> 

## <a name="usage-billing-frequency"></a><span data-ttu-id="53a40-110">사용량 청구 빈도</span><span class="sxs-lookup"><span data-stu-id="53a40-110">Usage billing frequency</span></span>

<span data-ttu-id="53a40-111">**월간 청구** 는 사용량 기반 제품에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-111">Only **monthly billing** is available for usage-based products.</span></span> <span data-ttu-id="53a40-112">월간 요금 청구에 대 한 자세한 내용은 [월별 및 연간 청구 차이점](billing-annual-monthly.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="53a40-112">For more information on monthly billing, see [Monthly and annual billing differences](billing-annual-monthly.md).</span></span>

<span data-ttu-id="53a40-113">사용량 기반 구독은 체납의 **구독 기념일 날짜**에 매월 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-113">Usage-based subscriptions are billed monthly, in arrears, on the **subscription anniversary date**.</span></span> <span data-ttu-id="53a40-114">예를 들어 구독 예정일 날짜가 15 인 경우 서비스 기간으로 1 월 15 일에서 1 월 14 일에 대 한 요금이 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-114">For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period of December 15 to January 14.</span></span> <span data-ttu-id="53a40-115">1 월 15 일에서 2 월 14 일의 서비스 기간에 대해 2 월 15 일에 다시 청구 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-115">You will be charged again on February 15 for the service period of January 15 to February 14.</span></span>

## <a name="usage-charges"></a><span data-ttu-id="53a40-116">사용 요금</span><span class="sxs-lookup"><span data-stu-id="53a40-116">Usage charges</span></span>

<span data-ttu-id="53a40-117">구독 기념일 날짜에 생성 되는 요금은 다음 청구서 및 [조정 파일](usage-based-recon-files.md)에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-117">The charges that are generated on the subscription anniversary date will appear on the following invoice and [reconciliation file](usage-based-recon-files.md).</span></span>

<span data-ttu-id="53a40-118">청구서에서 사용 요금이 누락 되거나 이전 달의 사용량이 현재 월의 청구서에 부과 되는 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-118">You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice.</span></span> <span data-ttu-id="53a40-119">이는 오류가 아닙니다. 서비스가 발생 한 후 서비스가 타임 스탬프 되었음을 의미 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-119">This is not an error; it simply means that the service was timestamped after the services occurred.</span></span> <span data-ttu-id="53a40-120">청구 주기가 끝날 때 24 시간 이내에 보고 된 사용량은 다음 달의 청구서에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-120">Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill.</span></span>

## <a name="cancelling-usage-based-subscriptions"></a><span data-ttu-id="53a40-121">사용 빈도 기반 구독 취소</span><span class="sxs-lookup"><span data-stu-id="53a40-121">Cancelling usage-based subscriptions</span></span>

<span data-ttu-id="53a40-122">언제 든 지 사용 빈도 기반 구독을 일시 중단할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-122">You can suspend usage-based subscriptions at any time.</span></span>

## <a name="pricing-for-usage"></a><span data-ttu-id="53a40-123">사용량 가격</span><span class="sxs-lookup"><span data-stu-id="53a40-123">Pricing for usage</span></span>

<span data-ttu-id="53a40-124">Azure CSP 가격 목록은 매월 게시 되며 파트너 센터 판매->가격 책정 및 제품 페이지에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-124">The Azure CSP Price List is published monthly and can be found on the Partner Center Sell->Pricing and Offers page.</span></span> <span data-ttu-id="53a40-125">가격은 매일 변경 될 수 있으며 가격 목록의 변경 내용 탭에 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-125">Please note prices can change daily and are reflected on the Change History tab of the Price List.</span></span>

<span data-ttu-id="53a40-126">사용량 요금은 일일 가격을 기준으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-126">Usage charges are based on daily prices.</span></span> <span data-ttu-id="53a40-127">서비스 기간 동안 가격이 변경 되 면 비례 하는 각 서비스 기간 및 해당 가격에 대 한 청구 줄이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="53a40-127">If the price changes during the service period you will see a billing line for each prorated service period and applicable price.</span></span>
