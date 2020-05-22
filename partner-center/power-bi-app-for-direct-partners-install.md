---
title: Power BI에 대 한 파트너 센터 분석 설치
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 이 문서의 단계를 수행 하 여 Power BI에 대 한 파트너 센터 분석 앱 (CSP의 직접 파트너)을 설치 하 고 미리 봅니다.
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795870"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="5e865-103">Microsoft Power BI용 파트너 센터 분석 앱 설치 및 미리 보기</span><span class="sxs-lookup"><span data-stu-id="5e865-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="5e865-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="5e865-104">**Applies to**</span></span>

- <span data-ttu-id="5e865-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="5e865-105">Partner Center</span></span>

<span data-ttu-id="5e865-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="5e865-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="5e865-107">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="5e865-107">Global admin</span></span>
-   <span data-ttu-id="5e865-108">사용자 관리자</span><span class="sxs-lookup"><span data-stu-id="5e865-108">User admin</span></span>
-   <span data-ttu-id="5e865-109">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="5e865-109">Sales agent</span></span>
-   <span data-ttu-id="5e865-110">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="5e865-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="5e865-111">시작하기 전에</span><span class="sxs-lookup"><span data-stu-id="5e865-111">Before you begin</span></span>

<span data-ttu-id="5e865-112">사용 가능한 Power BI 앱의 다음 목록에서 비즈니스에 가장 적합 한 응용 프로그램을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="5e865-113">직접 파트너</span><span class="sxs-lookup"><span data-stu-id="5e865-113">Direct Partner</span></span>](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [<span data-ttu-id="5e865-114">간접 파트너</span><span class="sxs-lookup"><span data-stu-id="5e865-114">Indirect Partner</span></span>](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [<span data-ttu-id="5e865-115">간접 재판매인</span><span class="sxs-lookup"><span data-stu-id="5e865-115">Indirect Reseller</span></span>](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

<span data-ttu-id="5e865-116">파트너 센터 분석 앱 미리 보기 버전을 설치 하기 전에 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="5e865-117">비즈니스에 적합 한 Power BI 앱을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="5e865-118">Microsoft Power BI Professional 또는 Microsoft Power BI Premium에 대 한 활성 구독이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-118">You have an active subscription to either Microsoft Power BI Professional or Microsoft Power BI Premium.</span></span>

- <span data-ttu-id="5e865-119">Power BI에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-119">You can sign in to Power BI.</span></span>

- <span data-ttu-id="5e865-120">전역 관리자, 관리 에이전트 또는 청구 관리자로 [회사의 Azure Active Directory (AZURE AD) 테 넌 트](azure-active-directory-tenants-and-partner-center.md)에 로그인 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-120">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="5e865-121">앱을 설치 하려면</span><span class="sxs-lookup"><span data-stu-id="5e865-121">To install the app</span></span>

1. <span data-ttu-id="5e865-122">[설치 프로세스를](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-122">Kick off [the installation process](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).</span></span>

2. <span data-ttu-id="5e865-123">**이미 계정이 있나요?** 에서 **로그인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-123">Under **Already have an account?** select **Sign In**.</span></span> 

3. <span data-ttu-id="5e865-124">다음 페이지에서 Power BI 사용자 이름 및 암호를 입력 한 다음 **로그인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-124">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span> 

4. <span data-ttu-id="5e865-125">**파트너 센터 분석에 연결** 팝업 창에서 **인증 방법이** **oAuth2** 으로 설정 되어 있는지 확인 하 고 그렇지 않은 경우 목록에서 **oAuth2** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-125">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="5e865-126">이 창을 표시 하는 데 몇 분 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-126">This window may take a few minutes to appear.</span></span>

5. <span data-ttu-id="5e865-127">**파트너 센터 분석 커넥터** 페이지에서 회사의 Azure AD 테 넌 트에 대 한 전역 관리자, 관리 에이전트 또는 청구 관리자 자격 증명을 사용 하 여 로그인 한 다음 **로그인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-127">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
6. <span data-ttu-id="5e865-128">액세스를 요청 하는 메시지가 표시 되 면 **동의**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-128">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="5e865-129">파트너 센터 분석 서비스가 Power BI에 연결 되 면 데이터가 로드 되기 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-129">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="5e865-130">데이터 양에 따라 최대 10 분이 소요 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-130">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="5e865-131">데이터가 로드를 완료 한 후 Power BI에서 파트너 센터 분석 앱 대시보드 및 보고서를 사용 하 여 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5e865-131">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5e865-132">다음 단계</span><span class="sxs-lookup"><span data-stu-id="5e865-132">Next steps</span></span>

[<span data-ttu-id="5e865-133">Microsoft Power BI 파트너 센터 분석 앱을 사용 하 여 비즈니스 데이터 보기</span><span class="sxs-lookup"><span data-stu-id="5e865-133">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
