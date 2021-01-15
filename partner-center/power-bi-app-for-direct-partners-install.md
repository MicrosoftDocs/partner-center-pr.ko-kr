---
title: Power BI에 대 한 파트너 센터 분석 설치
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 문서의 단계를 수행 하 여 Power BI에 대 한 파트너 센터 분석 앱 (CSP의 직접 파트너)을 설치 하 고 미리 봅니다.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215852"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="01ef7-103">Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기</span><span class="sxs-lookup"><span data-stu-id="01ef7-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="01ef7-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="01ef7-104">**Appropriate roles**</span></span>
-   <span data-ttu-id="01ef7-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="01ef7-105">Global admin</span></span>
-   <span data-ttu-id="01ef7-106">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="01ef7-106">User admin</span></span>
-   <span data-ttu-id="01ef7-107">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="01ef7-107">Sales agent</span></span>
-   <span data-ttu-id="01ef7-108">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="01ef7-108">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="01ef7-109">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="01ef7-109">Before you begin</span></span>

<span data-ttu-id="01ef7-110">사용 가능한 Power BI 앱의 다음 목록에서 비즈니스에 가장 적합 한 응용 프로그램을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-110">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="01ef7-111">직접 공급자</span><span class="sxs-lookup"><span data-stu-id="01ef7-111">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="01ef7-112">간접 공급자</span><span class="sxs-lookup"><span data-stu-id="01ef7-112">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="01ef7-113">간접 재판매인</span><span class="sxs-lookup"><span data-stu-id="01ef7-113">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="01ef7-114">파트너 센터 분석 앱 미리 보기 버전을 설치 하기 전에 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-114">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="01ef7-115">비즈니스에 적합 한 Power BI 앱을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-115">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="01ef7-116">Power BI pro 라이선스가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-116">You have a Power BI pro license.</span></span>

- <span data-ttu-id="01ef7-117">테 넌 트에서 템플릿 앱을 설치할 수 있는 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-117">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="01ef7-118">Power BI에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-118">You can sign in to Power BI.</span></span>

- <span data-ttu-id="01ef7-119">전역 관리자, 관리 에이전트 또는 청구 관리자로 [회사의 Azure Active Directory (AZURE AD) 테 넌 트](azure-active-directory-tenants-and-partner-center.md)에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-119">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="01ef7-120">앱을 설치 하려면</span><span class="sxs-lookup"><span data-stu-id="01ef7-120">To install the app</span></span>

1. <span data-ttu-id="01ef7-121">위의 섹션에서 제공 된 앱 소스 링크 (Direct Provider/간접 공급자/i a t e r/간접 재판매인)를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-121">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="01ef7-122">**지금 가져오기** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-122">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="01ef7-123">**계속** 을 클릭 하 여 사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-123">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="01ef7-124">에 이미 계정이 있나요? **로그인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-124">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="01ef7-125">다음 페이지에서 Power BI 사용자 이름 및 암호를 입력 한 다음 로그인을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-125">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="01ef7-126">작업 영역 이름을 제공 하 여 작업 영역을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-126">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="01ef7-127">앱 섹션 아래에 설치 된 템플릿 앱을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-127">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="01ef7-128">앱을 클릭 하 고 설치 된 앱을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-128">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="01ef7-129">새 앱 시작 화면이 열립니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-129">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="01ef7-130">데이터에 연결 하려면 **연결** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-130">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="01ef7-131">**파트너 센터 분석에 연결** 팝업 창에서 **인증 방법이** **oAuth2** 으로 설정 되어 있는지 확인 하 고 그렇지 않은 경우 목록에서 **oAuth2** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-131">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="01ef7-132">이 창을 표시 하는 데 몇 분 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-132">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="01ef7-133">**파트너 센터 분석 커넥터** 페이지에서 회사의 Azure AD 테 넌 트에 대 한 전역 관리자, 관리 에이전트 또는 청구 관리자 자격 증명을 사용 하 여 로그인 한 다음 **로그인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-133">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="01ef7-134">액세스를 요청 하는 메시지가 표시 되 면 **동의** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-134">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="01ef7-135">파트너 센터 분석 서비스가 Power BI에 연결 되 면 데이터가 로드 되기 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-135">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="01ef7-136">데이터 양에 따라 최대 10 분이 소요 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-136">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="01ef7-137">데이터가 로드를 완료 한 후 Power BI에서 파트너 센터 분석 앱 대시보드 및 보고서를 사용 하 여 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ef7-137">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="01ef7-138">다음 단계</span><span class="sxs-lookup"><span data-stu-id="01ef7-138">Next steps</span></span>

[<span data-ttu-id="01ef7-139">Microsoft Power BI 파트너 센터 분석 앱을 사용 하 여 비즈니스 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="01ef7-139">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
