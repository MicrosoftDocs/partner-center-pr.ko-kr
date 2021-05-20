---
title: 고객 계정에 대 한 여러 사용자 추가
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객의 계정에 여러 사용자를 추가 하려면 쉼표로 구분 된 값 (.csv) 파일 형식을 사용 하 여 파트너 센터에 데이터 파일을 업로드 합니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150474"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="e545e-103">고객의 계정에 사용자의 .csv 파일 업로드</span><span class="sxs-lookup"><span data-stu-id="e545e-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="e545e-104">**적절한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="e545e-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e545e-105">쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="e545e-106">고객 사용자의 파일을 만들고 고객 계정에 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="e545e-107">위에서 설명한 데이터를 사용 하 여 쉼표로 구분 된 값 (.csv) 데이터 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="e545e-108">이후 단계에서 찾아볼 수 있도록 파일을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="e545e-109">[고객 계정에 대 한 여러 사용자를 가져오려면 .csv 파일의 필드](file-customer-users.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e545e-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="e545e-110">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="e545e-111">파트너 센터 메뉴에서 **고객** 을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="e545e-112">고객의 **사용자 및 라이선스** 탭을 선택 하 고 **사용자 업로드** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="e545e-113">**사용자 정보 업로드** 에서 **찾아보기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="e545e-114">파일 선택기에서 데이터 파일을 선택한 다음 **열기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="e545e-115">**유효성 검사** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-115">Select **Validate**.</span></span>

    <span data-ttu-id="e545e-116">**참고**  대부분의 계정 생성 오류는 누락 된 정보, 형식이 잘못 되었거나 중복 된 전자 메일 주소를 포함 하거나 파일에 너무 많은 레코드를 포함 하 여 데이터 파일 문제로 인해 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="e545e-117">파트너 센터가 파일의 유효성을 검사 한 후 새 사용자의 지리적 **위치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="e545e-118">**저장** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-118">Select **Save**.</span></span>
10. <span data-ttu-id="e545e-119">사용자에 대한 임시 암호 정보를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="e545e-120">나중에이 작업을 수행할 수 없으므로 임시 암호를 사용 하 여 파일을 다운로드 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="e545e-121">새 사용자는 새 계정에 대 한 임시 암호를 사용 하 여 새 계정에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="e545e-122">새 사용자에 게 **라이선스 및 서비스를 사용할 수 있는** 권한이 자동으로 할당 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e545e-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e545e-123">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e545e-123">Next steps</span></span>

- [<span data-ttu-id="e545e-124">파트너 센터에서 고객에 게 자신의 제품 또는 서비스를 구매할 수 있는 권한 부여</span><span class="sxs-lookup"><span data-stu-id="e545e-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
