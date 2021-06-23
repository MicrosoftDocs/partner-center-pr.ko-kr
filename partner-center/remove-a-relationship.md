---
title: 고객과의 대리점 관계 제거
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft 직접 파트너가 목록에서 고객을 제거하고, 위임된 관리자 권한을 제거하고, 고객에 대한 지원 또는 구매를 중지하는 방법을 알아보세요.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551472"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="f9bdb-103">파트너 센터에서 고객과 재판매인 관계를 제거하는 방법</span><span class="sxs-lookup"><span data-stu-id="f9bdb-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="f9bdb-104">**적절한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="f9bdb-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="f9bdb-105">이 문서에서는 파트너 센터 고객과의 대리점 관계를 제거하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="f9bdb-106">직접 파트너 또는 간접 공급자: 고객과 더 이상 거래하지 않는 경우 파트너 센터 관계를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="f9bdb-107">관계를 제거하면 다음과 같은 결과가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="f9bdb-108">파트너 센터의 고객 목록에서 고객 제거</span><span class="sxs-lookup"><span data-stu-id="f9bdb-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="f9bdb-109">고객에 대해 [사용 가능한 지원 연락처 목록에서 제거합니다.](assign-support-contacts.md)</span><span class="sxs-lookup"><span data-stu-id="f9bdb-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="f9bdb-110">고객에 대한 위임 관리자 권한 제거</span><span class="sxs-lookup"><span data-stu-id="f9bdb-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="f9bdb-111">고객에 대한 향후 구매 방지</span><span class="sxs-lookup"><span data-stu-id="f9bdb-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="f9bdb-112">관계를 제거하는 방법</span><span class="sxs-lookup"><span data-stu-id="f9bdb-112">How to remove a relationship</span></span>

<span data-ttu-id="f9bdb-113">관계를 제거하려면 먼저 Azure RI(예약 인스턴스) 예약을 취소하고, 소프트웨어 구매를 취소하고, 나머지 활성 구독을 일시 중단해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="f9bdb-114">**활성 구독을 일시 중단합니다.**</span><span class="sxs-lookup"><span data-stu-id="f9bdb-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="f9bdb-115">파트너 센터 **고객으로** 이동하여 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="f9bdb-116">**구독에서 구독을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="f9bdb-117">**일시 중단 선택**</span><span class="sxs-lookup"><span data-stu-id="f9bdb-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="f9bdb-118">각 활성 구독에 대해 이러한 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="f9bdb-119">**파트너 센터 관계를 제거합니다.**</span><span class="sxs-lookup"><span data-stu-id="f9bdb-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="f9bdb-120">a.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-120">a.</span></span> <span data-ttu-id="f9bdb-121">파트너 센터 **고객으로** 이동하여 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="f9bdb-122">b.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-122">b.</span></span> <span data-ttu-id="f9bdb-123">**계정** 을 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-123">Select the **Account**.</span></span>

   <span data-ttu-id="f9bdb-124">다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-124">c.</span></span> <span data-ttu-id="f9bdb-125">**대리점 관계 제거를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="f9bdb-126">구독이 여전히 활성 상태이면 **대리점 관계 제거** 링크가 비활성 상태가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f9bdb-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9bdb-127">다음 단계</span><span class="sxs-lookup"><span data-stu-id="f9bdb-127">Next steps</span></span>

- [<span data-ttu-id="f9bdb-128">고객과의 관계 요청 또는 다시 설정</span><span class="sxs-lookup"><span data-stu-id="f9bdb-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
