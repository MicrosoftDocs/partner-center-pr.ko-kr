---
title: 고객 활동 로그를 사용 하 여 통찰력 얻기
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 활동 로그를 보거나 내보내 고객 계정 트랜잭션 및 기타 고객 관련 파트너 관리 활동에 대 한 통찰력을 얻는 방법에 대해 알아봅니다.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150593"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="958f8-103">고객 거래에 대 한 자세한 정보를 보려면 고객 활동 로그 보기 또는 내보내기</span><span class="sxs-lookup"><span data-stu-id="958f8-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="958f8-104">**적절 한 역할**: 전역 관리자 | 청구 관리자 | 사용자 관리 관리자 | 관리 에이전트 | 판매 에이전트 | 기술 지원팀 에이전트</span><span class="sxs-lookup"><span data-stu-id="958f8-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="958f8-105">활동 로그는 거래에 대 한 정보 및 고객에 대 한 파트너 관리 작업을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="958f8-106">트랜잭션에 대 한 로그는 구매한 구독을 포함 하 여 트랜잭션에 대 한 자세한 정보를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="958f8-107">활동 로그를 Excel과 호환 되는 쉼표로 구분 된 값 파일 형식 (.csv)으로 내보낼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="958f8-108">활동 로그는 고객 계정 및 제품 트랜잭션에 대 한 파트너 작업 레코드를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="958f8-109">활동 로그를 .csv 파일로 내보낼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="958f8-110">활동 로그 보기 및 내보내기</span><span class="sxs-lookup"><span data-stu-id="958f8-110">View and export activity logs</span></span>

1. <span data-ttu-id="958f8-111">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="958f8-112">**계정 설정** 메뉴에서 **활동 로그** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="958f8-113">**시작** 및 **대상** 필드에서 활동 로그 기간을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="958f8-114">활동 로그 내보내기는 가장 최근 달로 기본 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="958f8-115">각 활동 로그는 나열 된 고객의 **구독** 페이지에 대 한 링크를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="958f8-116">활동 로그에 대 한 아래쪽 화살표를 선택 하 여 기록 된 액션에 대 한 세부 정보를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="958f8-117">단일 활동 로그에는 여러 제품의 정렬과 같은 상당한 양의 데이터가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="958f8-118">로그의 데이터 열에는 다음 정보가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="958f8-119">**날짜-시간**-작업의 날짜 및 시간</span><span class="sxs-lookup"><span data-stu-id="958f8-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="958f8-120">**영향을 받는 고객**-고객의 회사 이름</span><span class="sxs-lookup"><span data-stu-id="958f8-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="958f8-121">**작업**—고객이 수행한 작업(예: “조회 생성”)</span><span class="sxs-lookup"><span data-stu-id="958f8-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="958f8-122">**파트너 사용자**—활동과 연관된 파트너.</span><span class="sxs-lookup"><span data-stu-id="958f8-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="958f8-123">**로그 내보내기** 를 선택하여 고객의 구독 데이터를 .csv 파일에 복사하고 이를 컴퓨터의 기본 다운로드 폴더에 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="958f8-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="958f8-124">다음 단계</span><span class="sxs-lookup"><span data-stu-id="958f8-124">Next steps</span></span>

- [<span data-ttu-id="958f8-125">비즈니스 의사 결정을 내리는 데 도움이 되는 구독 및 라이선스 분석</span><span class="sxs-lookup"><span data-stu-id="958f8-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
