---
title: Azure 사용량 분석 | 파트너 센터
ms.date: 07/12/2018
Description: 파트너 센터를 사용 하 여 고객의 Azure 구독 사용에 대 한 데이터를 가져옵니다.
Author: Xansky
ms.author: mhopkins
ms.assetid: E7081190-C1FA-47C1-963B-6EBA1B33703B
ms.topic: article
keywords: 비즈니스 데이터
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 9bd76a51664b18a8b3cea1e4163415480186fd86
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62131874"
---
# <a name="get-data-about-the-usage-of-your-customers-azure-subscriptions"></a><span data-ttu-id="8aafb-104">고객의 Azure 구독 사용량에 대한 데이터 가져오기</span><span class="sxs-lookup"><span data-stu-id="8aafb-104">Get data about the usage of your customers' Azure subscriptions</span></span> 

<span data-ttu-id="8aafb-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="8aafb-105">**Applies to**</span></span>
- <span data-ttu-id="8aafb-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="8aafb-106">Partner Center</span></span>

<span data-ttu-id="8aafb-107">데이터는 비즈니스 결정을 주도합니다.</span><span class="sxs-lookup"><span data-stu-id="8aafb-107">Data drives business decisions.</span></span> <span data-ttu-id="8aafb-108">**Azure 사용량** 페이지의 메트릭을 사용하여 귀사의 성공 상태 및 더 많은 관심이 필요한 분야를 파악하세요.</span><span class="sxs-lookup"><span data-stu-id="8aafb-108">Use the metrics in the **Azure usage** page to identify your successes and areas that need more attention.</span></span> <span data-ttu-id="8aafb-109">이 정보를 사용하여 새로운 비즈니스 목표를 계획하세요.</span><span class="sxs-lookup"><span data-stu-id="8aafb-109">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="8aafb-110">Azure 사용량 분석은 클라우드 솔루션 공급자 프로그램의 파트너에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8aafb-110">Azure usage  analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="8aafb-111">다음과 같은 메트릭을 추적 중입니다.</span><span class="sxs-lookup"><span data-stu-id="8aafb-111">We are tracking the following metrics:</span></span>

<span data-ttu-id="8aafb-112">**요약**</span><span class="sxs-lookup"><span data-stu-id="8aafb-112">**Summary**</span></span>  
 - <span data-ttu-id="8aafb-113">**Azure 구독을 총 판매**: 지정된 된 기간 내에 판매 된 구독 수</span><span class="sxs-lookup"><span data-stu-id="8aafb-113">**Total Azure subscriptions sold**: Number of subscriptions sold in the specified time period</span></span>  
 - <span data-ttu-id="8aafb-114">**고객 사용량을**: 지정된 된 기간 내에 Azure 사용 고객의 수</span><span class="sxs-lookup"><span data-stu-id="8aafb-114">**Customers with usage**: Number of customers with Azure usage in the specified time period</span></span>  
 - <span data-ttu-id="8aafb-115">**사용 하지 않고 고객에 게**: 지정된 된 기간 내에 Azure 사용 하지 않고 고객의 수</span><span class="sxs-lookup"><span data-stu-id="8aafb-115">**Customers without usage**: Number of customers without Azure usage in the specified time period</span></span>  

<span data-ttu-id="8aafb-116">**상위 범주에서 5 대 고객**</span><span class="sxs-lookup"><span data-stu-id="8aafb-116">**Top 5 customers in category**</span></span>  
 -  <span data-ttu-id="8aafb-117">지정된 범주의 상위 5개 고객</span><span class="sxs-lookup"><span data-stu-id="8aafb-117">The top 5 customers for the specified category</span></span>  

<span data-ttu-id="8aafb-118">**사용 하지 않고 구독**</span><span class="sxs-lookup"><span data-stu-id="8aafb-118">**Subscriptions without usage**</span></span>  
 -  <span data-ttu-id="8aafb-119">지정된 기간에 Azure 사용량이 없는 특정 구독의 목록</span><span class="sxs-lookup"><span data-stu-id="8aafb-119">List of sepcific subscriptions without Azure usage in the specified time period</span></span>  

<span data-ttu-id="8aafb-120">**Azure 구독 변동**</span><span class="sxs-lookup"><span data-stu-id="8aafb-120">**Azure subscription churn**</span></span>  
 - <span data-ttu-id="8aafb-121">**활성 구독이**: 날짜별 활성 구독 수</span><span class="sxs-lookup"><span data-stu-id="8aafb-121">**Active subscriptions**: Count of active subscriptions by date</span></span>  
 - <span data-ttu-id="8aafb-122">**구독을 프로 비전 해제**: 프로 비전을 해제 하거나 날짜별 일시 중단 된 구독 수</span><span class="sxs-lookup"><span data-stu-id="8aafb-122">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="8aafb-123">**고객 수**</span><span class="sxs-lookup"><span data-stu-id="8aafb-123">**Customer count**</span></span>
 - <span data-ttu-id="8aafb-124">지정된 기간 동안 확보한 신규 고객</span><span class="sxs-lookup"><span data-stu-id="8aafb-124">New customers acquired during the specified time period</span></span>  

<span data-ttu-id="8aafb-125">**Azure 구독 보존**</span><span class="sxs-lookup"><span data-stu-id="8aafb-125">**Azure subscription retention**</span></span>  
 - <span data-ttu-id="8aafb-126">갱신된 구독의 수.</span><span class="sxs-lookup"><span data-stu-id="8aafb-126">The number of subscriptions that were renewed.</span></span>   
  