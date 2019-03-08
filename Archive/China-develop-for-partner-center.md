---
title: 21Vianet에서 운영하는 파트너 센터 개발
ms.topic: article
ms.date: 10/29/2018
description: 21Vianet에서 운영 하는 파트너 센터에 대 한 개발 리소스
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 26b919459ea6e1c409d3f22aa324d0b877822e8c
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584286"
---
# <a name="develop-for-partner-center-operated-by-21-vianet"></a><span data-ttu-id="b9609-103">21 Vianet에서 운영 하는 파트너 센터에 대 한 개발</span><span class="sxs-lookup"><span data-stu-id="b9609-103">Develop for Partner Center operated by 21 Vianet</span></span>

<span data-ttu-id="b9609-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="b9609-104">**Applies to**</span></span>

-   <span data-ttu-id="b9609-105">21Vianet에서 운영하는 파트너 센터</span><span class="sxs-lookup"><span data-stu-id="b9609-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="b9609-106">소프트웨어 개발 키트를 사용 하 여 사용자 고유의 응용 프로그램을 사용 하 여 고객, 주문, 대금 청구 및 지원 시스템을 통합 합니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-106">Integrate your customer, orders, billing, and support systems with your own applications by using the software development kit.</span></span>

><span data-ttu-id="b9609-107">**참고**</span><span class="sxs-lookup"><span data-stu-id="b9609-107">**Note**</span></span><br> <span data-ttu-id="b9609-108">21Vianet에서 운영 하는 파트너 센터 SDK 설명서는 Microsoft Developer Network 웹 사이트 (MSDN)에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-108">The SDK documentation for Partner Center operated by 21Vianet is available on the Microsoft Developer Network website (MSDN).</span></span> <span data-ttu-id="b9609-109">가지 21vianet 파트너 센터에 대 한 SDK 및 파트너 센터 운영에 대 한 SDK 간의 일부 차이점이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-109">There are some differences between the SDK for Partner Center and the SDK for Partner Center Operated by 21Vianet.</span></span>
<span data-ttu-id="b9609-110">각 도움말 항목 멤버의 21Vianet에서 운영 하는 파트너 센터에 적용 되는 여부에 대해 설명 합니다 **적용할** 섹션.</span><span class="sxs-lookup"><span data-stu-id="b9609-110">Each help topic describes whether or not a member applies to Partner Center operated by 21Vianet in the **Applies to** section.</span></span> <span data-ttu-id="b9609-111">21Vianet에서 운영 하는 파트너 센터에 대 한 다른 REST 끝점이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-111">There are different REST endpoints for Partner Center operated by 21Vianet.</span></span> <span data-ttu-id="b9609-112">자세한 내용은 [파트너 센터 REST API 참조](https://msdn.microsoft.com/en-us/library/partnercenter/mt667943.aspx)합니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-112">For more information, see [Partner Center REST API reference](https://msdn.microsoft.com/en-us/library/partnercenter/mt667943.aspx).</span></span>


-   [<span data-ttu-id="b9609-113">SDK 다운로드</span><span class="sxs-lookup"><span data-stu-id="b9609-113">Get the SDK</span></span>](https://go.microsoft.com/fwlink/p/?LinkID=746681)

-   [<span data-ttu-id="b9609-114">샘플 다운로드</span><span class="sxs-lookup"><span data-stu-id="b9609-114">Download Samples</span></span>](https://msdn.microsoft.com/library/partnercenter/mt634711.aspx)

-   <span data-ttu-id="b9609-115">[개발자 계정을 구성할](https://msdn.microsoft.com/library/partnercenter/mt634709.aspx) 및 인증을 위해 Azure AD를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-115">[Configure your developer account](https://msdn.microsoft.com/library/partnercenter/mt634709.aspx) and set up Azure AD for authentication.</span></span> 

-   <span data-ttu-id="b9609-116">[테스트 및 디버그](https://msdn.microsoft.com/library/partnercenter/mt634717.aspx) 테스트-프로덕션 환경으로 통합 샌드박스를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-116">[Test and debug](https://msdn.microsoft.com/library/partnercenter/mt634717.aspx) using the integration sandbox as a test-in-production environment.</span></span>

## <a name="developer-help"></a><span data-ttu-id="b9609-117">개발자 도움말</span><span class="sxs-lookup"><span data-stu-id="b9609-117">Developer help</span></span>
<span data-ttu-id="b9609-118">일반적인 앱 시나리오 및 SDK의 사용 가능한 인터페이스에 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="b9609-118">Learn about common app scenarios and the available interfaces in the SDK:</span></span>

-   [<span data-ttu-id="b9609-119">SDK 시나리오</span><span class="sxs-lookup"><span data-stu-id="b9609-119">SDK scenarios</span></span>](https://msdn.microsoft.com/library/partnercenter/mt634715.aspx)

-   [<span data-ttu-id="b9609-120">관리 되는 API 참조</span><span class="sxs-lookup"><span data-stu-id="b9609-120">Managed API reference</span></span>](https://msdn.microsoft.com/library/partnercenter/mt635943.aspx)

-   [<span data-ttu-id="b9609-121">REST API 참조</span><span class="sxs-lookup"><span data-stu-id="b9609-121">REST API reference</span></span>](https://msdn.microsoft.com/library/partnercenter/mt667943.aspx)