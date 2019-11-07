---
title: Microsoft에서 SLA 크레딧 요청 | 파트너 센터
ms.topic: article
ms.date: 06/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 서비스에서 가동 중단이 발생 하는 경우 고객에 대 한 SLA 크레딧을 요청할 수 있습니다.
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6a04d8e179f48f60c71b2e0e5c723c9d821de797
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651695"
---
# <a name="request-an-sla-credit-from-microsoft"></a><span data-ttu-id="c7413-103">Microsoft에서 SLA 크레딧 요청</span><span class="sxs-lookup"><span data-stu-id="c7413-103">Request an SLA credit from Microsoft</span></span> 

<span data-ttu-id="c7413-104">고객을 위해 제공 하는 서비스의 작동이 중단 되는 경우 Microsoft에서 크레딧을 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-104">If a service you are providing for your customers has an outage, you are able to request a credit from Microsoft.</span></span> <span data-ttu-id="c7413-105">SLA (Service Level Agreement(서비스 수준 약정)) 크레딧을 영향을 받는 서비스에 따라 결정 됩니다. 즉, 고객이 O365 제품군을 보유 하 고 있고 SharePoint만 다운 된 경우에는 전체 계획이 아닌 SharePoint에 대해서만 SLA 크레딧을 승인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-105">Service Level Agreement (SLA) credits are determined based on which service was impacted (i.e. if the customer has an O365 suite and only SharePoint was down, the SLA credit is approved for SharePoint only, not for the entire plan).</span></span>

<span data-ttu-id="c7413-106">크레딧은 영향을 받는 서비스 및 가동 중단 기간을 기준으로 비례 배분 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-106">Credits are pro-rated based on the service affected and the duration of the outage.</span></span> <span data-ttu-id="c7413-107">SLA 크레딧을 충족 하는 시나리오의 유형을 확인 하려면 [온라인 서비스 통합 SLA 문서](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c7413-107">To see the types of scenarios that qualify for SLA credits, read the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="c7413-108">이 정보는 클라우드 솔루션 공급자 프로그램을 통해 판매 되는 서비스에도 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-108">This information applies to services sold through the Cloud Solution Provider program, too.</span></span>

>[!Note]
><span data-ttu-id="c7413-109">**매우 중요 합니다.**</span><span class="sxs-lookup"><span data-stu-id="c7413-109">**VERY IMPORTANT!**</span></span> <span data-ttu-id="c7413-110">CSP 파트너 (간접 공급자 또는 직접 청구 파트너 (최종 고객 또는 간접 재판매인 아님))는 인시던트가 발생 한 월 뒤의 월 끝에 클레임 및 모든 필수 정보를 제출 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-110">The CSP partner, either the indirect provider or the direct bill partner, (not the end customer or the indirect reseller) must submit a claim and all required information by the end of the calendar month following the month in which the incident occurred.</span></span> <span data-ttu-id="c7413-111">예를 들어 인시던트가 2 월 15 일에 발생 한 경우 클레임 및 모든 필수 정보를 3 월 31 일까 지 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-111">For example, if the incident occurred on February 15, we must receive the claim and all required information by March 31.</span></span> 

## <a name="required-information"></a><span data-ttu-id="c7413-112">필요한 정보</span><span class="sxs-lookup"><span data-stu-id="c7413-112">Required information</span></span>


<span data-ttu-id="c7413-113">SLA 크레딧을 요청 하려면 다음 정보를 제공 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-113">To request an SLA credit, you need to provide the following information:</span></span> 

- <span data-ttu-id="c7413-114">고객 테 넌 트 GUID:</span><span class="sxs-lookup"><span data-stu-id="c7413-114">Customer tenant GUID:</span></span> 

- <span data-ttu-id="c7413-115">중단 인시던트 #: (아래 참조)</span><span class="sxs-lookup"><span data-stu-id="c7413-115">Outage Incident#: (see below)</span></span>

- <span data-ttu-id="c7413-116">CSP를 통해 구매한 영향을 받는 구독이 있나요?</span><span class="sxs-lookup"><span data-stu-id="c7413-116">Were the impacted subscriptions purchased via CSP?</span></span> <span data-ttu-id="c7413-117">예/아니요</span><span class="sxs-lookup"><span data-stu-id="c7413-117">Yes/No</span></span>

<span data-ttu-id="c7413-118">중단 인시던트 ID (예: EX25194)는 Microsoft 365 관리 센터의 Service Health 페이지에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-118">The Outage Incident ID (such as EX25194) is found on the Service Health page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="c7413-119">인시던트 번호 앞에는 다음의 영향을 받는 서비스를 나타내는 2 자로 된 약어가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-119">Incident numbers are preceded with a 2-letter abbreviation that indicates the service affected, such as:</span></span>

<span data-ttu-id="c7413-120">예: Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c7413-120">EX - Exchange Online</span></span>

<span data-ttu-id="c7413-121">Exchange Online 보호</span><span class="sxs-lookup"><span data-stu-id="c7413-121">FO - Exchange Online Protection</span></span>

<span data-ttu-id="c7413-122">SB-비즈니스용 Skype Online (공식 Lync Online)</span><span class="sxs-lookup"><span data-stu-id="c7413-122">SB - Skype for Business Online (formally Lync Online)</span></span>

<span data-ttu-id="c7413-123">OS-Office 구독</span><span class="sxs-lookup"><span data-stu-id="c7413-123">OS - Office Subscription</span></span>

<span data-ttu-id="c7413-124">PB-Office 365용 Power BI</span><span class="sxs-lookup"><span data-stu-id="c7413-124">PB -Power BI for Office 365</span></span>

<span data-ttu-id="c7413-125">SP-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c7413-125">SP - SharePoint Online</span></span>

<span data-ttu-id="c7413-126">인 Yammer 엔터프라이즈</span><span class="sxs-lookup"><span data-stu-id="c7413-126">YA - Yammer Enterprise</span></span>

<span data-ttu-id="c7413-127">MO-포털 오류</span><span class="sxs-lookup"><span data-stu-id="c7413-127">MO - Portal Error</span></span>

## <a name="submit-a-request"></a><span data-ttu-id="c7413-128">요청 제출</span><span class="sxs-lookup"><span data-stu-id="c7413-128">Submit a request</span></span>

<span data-ttu-id="c7413-129">파트너 센터에서 신용 요청을 제출 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-129">Submit your credit request on Partner Center.</span></span>

1. <span data-ttu-id="c7413-130">파트너 센터 대시보드의 왼쪽 탐색 창에서 **지원** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-130">From your Partner Center dashboard, select **Support** from the left nav.</span></span>

2. <span data-ttu-id="c7413-131">**파트너 지원 요청** 을 선택한 다음 **CSP-고객, 주문 및 구독/고객 서비스 신용 요청**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-131">Select **Partner support requests** and then select **CSP - customers, orders, and subscriptions/Customer services credit requests**.</span></span>

3. <span data-ttu-id="c7413-132">SLA 신용 요청을 제출 합니다.</span><span class="sxs-lookup"><span data-stu-id="c7413-132">Submit your SLA credit request.</span></span>





