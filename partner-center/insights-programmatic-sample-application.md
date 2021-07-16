---
title: 예제 응용 프로그램
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 샘플 애플리케이션을 사용하여 프로그래밍 방식으로 파트너 인사이트 데이터에 액세스하는 고유한 애플리케이션을 빌드합니다.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375856"
---
# <a name="sample-application"></a><span data-ttu-id="9cd2f-103">예제 응용 프로그램</span><span class="sxs-lookup"><span data-stu-id="9cd2f-103">Sample Application</span></span>

<span data-ttu-id="9cd2f-104">샘플 애플리케이션은 C# 및 JAVA 언어로 만들어지고 [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="9cd2f-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="9cd2f-105">C# 샘플 애플리케이션</span><span class="sxs-lookup"><span data-stu-id="9cd2f-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="9cd2f-106">JAVA 샘플 애플리케이션</span><span class="sxs-lookup"><span data-stu-id="9cd2f-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="9cd2f-107">샘플 애플리케이션에서 아이디어를 얻어 원하는 언어로 자체 애플리케이션을 빌드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="9cd2f-108">샘플 애플리케이션은 다음 목표를 달성합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="9cd2f-109">Azure AD(Azure Active Directory) 토큰을 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="9cd2f-110">사용 가능한 데이터 세트를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-110">Gets available datasets.</span></span>
- <span data-ttu-id="9cd2f-111">사용자 정의 쿼리를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-111">Creates user defined queries.</span></span>
- <span data-ttu-id="9cd2f-112">사용자 정의 및 시스템 쿼리를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="9cd2f-113">보고서를 예약합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-113">Schedules a report.</span></span>

<span data-ttu-id="9cd2f-114">샘플 애플리케이션은 다른 기능에 대해 API를 호출하는 방법을 다루지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="9cd2f-115">그러나 다른 API를 호출하는 프로세스는 위에 설명된 것과 동일하게 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="9cd2f-116">애플리케이션을 실행하는 방법</span><span class="sxs-lookup"><span data-stu-id="9cd2f-116">How to run the application</span></span>

- <span data-ttu-id="9cd2f-117">다음 명령을 사용하여 로컬 시스템에 리포지토리를 복제합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="9cd2f-118">자세한 내용은 GitHub [리포지토리의](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)ProgrammaticExportSampleAppMPN/README.md 파일을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="9cd2f-119">앱을 신속하게 실행하려면appsettings.Development.js클라이언트 ID 및 클라이언트 비밀을 **업데이트합니다.**</span><span class="sxs-lookup"><span data-stu-id="9cd2f-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="앱설정 개발 json 설명":::

<span data-ttu-id="9cd2f-121">앱을 실행하면 로컬 웹 서버가 시작되고 페이지가 열립니다(`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span><span class="sxs-lookup"><span data-stu-id="9cd2f-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="샘플 애플리케이션의 UI 설명":::

<span data-ttu-id="9cd2f-123">이 페이지는 로컬 머신에서 실행되는 웹 서버에 대한 API 호출을 수행합니다. 이에 따라 실제 프로그래밍 방식 액세스 API 호출을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="9cd2f-124">코드 조각</span><span class="sxs-lookup"><span data-stu-id="9cd2f-124">Code Snippets</span></span>

<span data-ttu-id="9cd2f-125">프로그래밍 방식 액세스 API 호출을 수행하는 C# 코드의 기본 구조는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd2f-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="코드 조각 설명":::

## <a name="next-steps"></a><span data-ttu-id="9cd2f-127">다음 단계</span><span class="sxs-lookup"><span data-stu-id="9cd2f-127">Next steps</span></span>

[<span data-ttu-id="9cd2f-128">파트너 인사이트 분석 데이터에 액세스하기 위한 API</span><span class="sxs-lookup"><span data-stu-id="9cd2f-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
