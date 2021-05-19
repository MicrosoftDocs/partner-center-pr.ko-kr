---
title: 다중 파트너 지원
ms.topic: article
ms.date: 11/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객은 클라우드 솔루션 공급자 프로그램에서 서로 다른 서비스를 전문화한 여러 파트너와 함께 작업하기를 원할 수 있습니다.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b41d3ee33b789c8f839ff1b3b5f5d8fd27c23f02
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151154"
---
# <a name="multi-partner-support-for-customers-who-want-to-work-with-more-than-one-partner"></a><span data-ttu-id="78ace-103">두 개 이상의 파트너와 함께 작업하려는 고객을 위한 다중 파트너 지원</span><span class="sxs-lookup"><span data-stu-id="78ace-103">Multi-partner support for customers who want to work with more than one partner</span></span>

<span data-ttu-id="78ace-104">**적용된 내용:** 파트너 센터 | Microsoft Cloud for US Government 대한 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="78ace-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="78ace-105">**적절한 역할:** 전역 관리자 | 사용자 관리 관리자 | 판매 에이전트</span><span class="sxs-lookup"><span data-stu-id="78ace-105">**Appropriate roles**: Global admin | User management admin | Sales agent</span></span>

<span data-ttu-id="78ace-106">파트너 센터 다중 파트너 기능은 고객이 두 개 이상의 파트너와 함께 작업하려는 시나리오를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-106">The Partner Center's multi-partner feature supports scenarios when a customer wants to work with more than one partner.</span></span> <span data-ttu-id="78ace-107">예를 들어 고객은 Office 365의 전문 지식을 위해 한 파트너를 고용하되 Microsoft Azure 전문 분야의 다른 파트너를 고용하려고 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-107">For example, a customer may want to hire one partner for their expertise in Office 365, but hire a different partner who specializes in Microsoft Azure.</span></span>

<span data-ttu-id="78ace-108">Azure CSP 테넌트는 다른 CSP 파트너의 추가 Azure 구독을 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-108">An Azure CSP tenant can include an additional Azure subscription from a different CSP partner.</span></span>

<span data-ttu-id="78ace-109">파트너 센터 다중 파트너 기능을 사용하려면 위임된 관리 권한을 부여하도록 고객을 초대합니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-109">To use the multi-partner feature in the Partner Center, invite the customer to give you delegated administration privileges.</span></span> <span data-ttu-id="78ace-110">이미 파트너와 작업 중인 고객과 관계를 설정하는 방법에 대한 자세한 내용은 [고객과의](request-a-relationship-with-a-customer.md) 관계 요청을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="78ace-110">See [Request a relationship with a customer](request-a-relationship-with-a-customer.md) for information about how to establish a relationship with a customer who is already working with a partner.</span></span>

<span data-ttu-id="78ace-111">다중 파트너 기능은 다음을 수행하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-111">Multi-partner functionality does not:</span></span>

- <span data-ttu-id="78ace-112">고객의 기존 구독 변경</span><span class="sxs-lookup"><span data-stu-id="78ace-112">Change any of the customer's existing subscriptions</span></span>

- <span data-ttu-id="78ace-113">고객의 기존 구독 또는 계정 소유권 전환</span><span class="sxs-lookup"><span data-stu-id="78ace-113">Transition the customer's existing subscriptions or account ownership</span></span>

- <span data-ttu-id="78ace-114">기존 구독에 대한 약관 또는 고객의 의무 변경</span><span class="sxs-lookup"><span data-stu-id="78ace-114">Change the terms or customer's obligations for any of their existing subscriptions</span></span>

- <span data-ttu-id="78ace-115">구독에 대한 레코드 파트너 변경</span><span class="sxs-lookup"><span data-stu-id="78ace-115">Change the partner of record for a subscription</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="78ace-116">현재 CSP 프로그램의 파트너는 CSP 프로그램의 다른 파트너에게 온라인 서비스를 재판매할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-116">A partner in the CSP program cannot resell online services to another partner in the CSP program currently.</span></span> <span data-ttu-id="78ace-117">이 제한은 CSP 거래 수행에 사용되는 테넌트에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-117">This restriction only applies to the tenant used for conducting CSP transactions.</span></span> <span data-ttu-id="78ace-118">회사용으로 CSP가 아닌 테넌트를 사용하는 CSP 파트너는 다른 CSP 파트너에게서 온라인 서비스를 구입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-118">CSP partners who use a non-CSP tenant for their corporate usage can purchase online services from another CSP partner.</span></span> <span data-ttu-id="78ace-119">Microsoft에서는 모든 프로그램의 정책과 기능을 지속적으로 검토하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-119">Microsoft continuously reviews the policies and capabilities of all programs.</span></span> <span data-ttu-id="78ace-120">기능 릴리스 또는 정책 변경에 대한 뉴스는 [파트너 센터 발표](announcements/index.md)를 포함한 일반적인 통신 채널을 통해 발표될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="78ace-120">Any news about feature releases or policy changes will be announced through the usual communications channels, including [Partner Center announcements](announcements/index.md).</span></span>
