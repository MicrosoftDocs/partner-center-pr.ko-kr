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
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302330"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="d306b-103">Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기</span><span class="sxs-lookup"><span data-stu-id="d306b-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="d306b-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="d306b-104">**Applies to**</span></span>

- <span data-ttu-id="d306b-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="d306b-105">Partner Center</span></span>

<span data-ttu-id="d306b-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="d306b-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="d306b-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="d306b-107">Global admin</span></span>
-   <span data-ttu-id="d306b-108">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="d306b-108">User admin</span></span>
-   <span data-ttu-id="d306b-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="d306b-109">Sales agent</span></span>
-   <span data-ttu-id="d306b-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="d306b-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="d306b-111">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="d306b-111">Before you begin</span></span>

<span data-ttu-id="d306b-112">사용 가능한 Power BI 앱의 다음 목록에서 비즈니스에 가장 적합 한 응용 프로그램을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="d306b-113">직접 공급자</span><span class="sxs-lookup"><span data-stu-id="d306b-113">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="d306b-114">간접 공급자</span><span class="sxs-lookup"><span data-stu-id="d306b-114">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="d306b-115">간접 재판매인</span><span class="sxs-lookup"><span data-stu-id="d306b-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="d306b-116">파트너 센터 분석 앱 미리 보기 버전을 설치 하기 전에 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="d306b-117">비즈니스에 적합 한 Power BI 앱을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="d306b-118">Power BI pro 라이선스가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="d306b-119">테 넌 트에서 템플릿 앱을 설치할 수 있는 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="d306b-120">Power BI에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="d306b-121">전역 관리자, 관리 에이전트 또는 청구 관리자로 [회사의 Azure Active Directory (AZURE AD) 테 넌 트](azure-active-directory-tenants-and-partner-center.md)에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="d306b-122">앱을 설치 하려면</span><span class="sxs-lookup"><span data-stu-id="d306b-122">To install the app</span></span>

1. <span data-ttu-id="d306b-123">위의 섹션에서 제공 된 앱 소스 링크 (Direct Provider/간접 공급자/i a t e r/간접 재판매인)를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="d306b-124">**지금 가져오기**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-124">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="d306b-125">**계속**을 클릭 하 여 사용 약관에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-125">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="d306b-126">에 이미 계정이 있나요? **로그인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-126">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="d306b-127">다음 페이지에서 Power BI 사용자 이름 및 암호를 입력 한 다음 로그인을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="d306b-128">작업 영역 이름을 제공 하 여 작업 영역을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-128">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="d306b-129">앱 섹션 아래에 설치 된 템플릿 앱을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="d306b-130">앱을 클릭 하 고 설치 된 앱을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="d306b-131">새 앱 시작 화면이 열립니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="d306b-132">데이터에 연결 하려면 **연결**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-132">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="d306b-133">**파트너 센터 분석에 연결** 팝업 창에서 **인증 방법이** **oAuth2** 으로 설정 되어 있는지 확인 하 고 그렇지 않은 경우 목록에서 **oAuth2** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="d306b-134">이 창을 표시 하는 데 몇 분 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="d306b-135">**파트너 센터 분석 커넥터** 페이지에서 회사의 Azure AD 테 넌 트에 대 한 전역 관리자, 관리 에이전트 또는 청구 관리자 자격 증명을 사용 하 여 로그인 한 다음 **로그인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="d306b-136">액세스를 요청 하는 메시지가 표시 되 면 **동의**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-136">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="d306b-137">파트너 센터 분석 서비스가 Power BI에 연결 되 면 데이터가 로드 되기 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="d306b-138">데이터 양에 따라 최대 10 분이 소요 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="d306b-139">데이터가 로드를 완료 한 후 Power BI에서 파트너 센터 분석 앱 대시보드 및 보고서를 사용 하 여 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d306b-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d306b-140">다음 단계</span><span class="sxs-lookup"><span data-stu-id="d306b-140">Next steps</span></span>

[<span data-ttu-id="d306b-141">Microsoft Power BI 파트너 센터 분석 앱을 사용 하 여 비즈니스 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="d306b-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
