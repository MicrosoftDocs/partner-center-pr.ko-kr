---
title: 고객 계정에 대한 다수의 사용자 만들기 | 파트너 센터
ms.topic: article
ms.date: 03/15/2019
description: 쉼표로 구분된 값 파일 형식(.csv)의 데이터 파일을 파트너 센터에 업로드하여 한 번에 고객 계정에 다수의 사용자를 추가할 수 있습니다.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: 대량 업로드, 고객 계정에 여러 사용자 추가, 고객의 사용자 추가, 고객 사용자 대량 업로드, 고객 계정, 고객 사용자, 사용자
ms.localizationpriority: medium
ms.openlocfilehash: b113736330b201ed6a4d1c6b8915e844b80fe5d5
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134533"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="4e82a-104">고객 계정에 여러 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="4e82a-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="4e82a-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="4e82a-105">**Applies to**</span></span>

-  <span data-ttu-id="4e82a-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="4e82a-106">Partner Center</span></span>

<span data-ttu-id="4e82a-107">추가할 수 있습니다 여러 사용자가 고객의 계정에 한 번에 모든 파트너 센터를 쉼표로 구분 된 값 파일 (.csv) 형식으로 데이터 파일을 업로드 하 여.</span><span class="sxs-lookup"><span data-stu-id="4e82a-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="4e82a-108">파트너 센터에서 샘플 데이터 파일을 다운로드 하 고 사용에 대 한 편집 하거나 아래에 정의 된 데이터 모델을 사용 하 여 새 데이터 파일을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="4e82a-109">데이터 파일 요구 사항</span><span class="sxs-lookup"><span data-stu-id="4e82a-109">Data file requirements</span></span>


<span data-ttu-id="4e82a-110">대량 업로드 프로세스를 사용하여 고객 계정에 다수의 사용자를 추가하려면 다음 요구 사항을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="4e82a-111">고객 계정에 대한 전역 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="4e82a-112">각 사용자는 고객의 메일 도메인에 추가된 고유한 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="4e82a-113">한 번에 최대 100개의 레코드를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="4e82a-114">100명이 넘는 사용자를 추가해야 할 경우 추가 데이터 파일을 만들어 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="4e82a-115">모든 사용자가 같은 지리적 **위치**에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="4e82a-116">아래에 설명된 데이터만 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-116">Enter only the data described below.</span></span> <span data-ttu-id="4e82a-117">관련 없는 데이터를 입력하면 업로드에 실패하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="4e82a-118">데이터 파일에 다음 데이터를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="4e82a-119">**열 이름**</span><span class="sxs-lookup"><span data-stu-id="4e82a-119">**Column name**</span></span> | <span data-ttu-id="4e82a-120">**설명**</span><span class="sxs-lookup"><span data-stu-id="4e82a-120">**Description**</span></span>                                                              | <span data-ttu-id="4e82a-121">**제한 사항**</span><span class="sxs-lookup"><span data-stu-id="4e82a-121">**Limitation**</span></span>                             |
| <span data-ttu-id="4e82a-122">이름</span><span class="sxs-lookup"><span data-stu-id="4e82a-122">First name</span></span>      | <span data-ttu-id="4e82a-123">사용자의 이름(선택적 필드)</span><span class="sxs-lookup"><span data-stu-id="4e82a-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="4e82a-124">50자 제한</span><span class="sxs-lookup"><span data-stu-id="4e82a-124">50-character limit</span></span>                         |
| <span data-ttu-id="4e82a-125">성</span><span class="sxs-lookup"><span data-stu-id="4e82a-125">Last name</span></span>       | <span data-ttu-id="4e82a-126">사용자의 성(선택적 필드)</span><span class="sxs-lookup"><span data-stu-id="4e82a-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="4e82a-127">50자 제한</span><span class="sxs-lookup"><span data-stu-id="4e82a-127">50-character limit</span></span>                         |
| <span data-ttu-id="4e82a-128">표시 이름</span><span class="sxs-lookup"><span data-stu-id="4e82a-128">Display name</span></span>    | <span data-ttu-id="4e82a-129">파트너 센터 (필수 필드)에 표시 된 이름</span><span class="sxs-lookup"><span data-stu-id="4e82a-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="4e82a-130">50자 제한</span><span class="sxs-lookup"><span data-stu-id="4e82a-130">50-character limit</span></span>                         |
| <span data-ttu-id="4e82a-131">EMail</span><span class="sxs-lookup"><span data-stu-id="4e82a-131">Email</span></span>           | <span data-ttu-id="4e82a-132">고객 회사의 사용자 회사 메일 주소(필수 필드)</span><span class="sxs-lookup"><span data-stu-id="4e82a-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="4e82a-133">각 사용자는 고유한 메일 주소가 있어야 함</span><span class="sxs-lookup"><span data-stu-id="4e82a-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="4e82a-134">상태 업데이트</span><span class="sxs-lookup"><span data-stu-id="4e82a-134">Status update</span></span>   | <span data-ttu-id="4e82a-135">새 사용자 레코드가 만들어졌는지를 나타내는 데 사용됨</span><span class="sxs-lookup"><span data-stu-id="4e82a-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="4e82a-136">\*\*비워 둡니다\*\*</span><span class="sxs-lookup"><span data-stu-id="4e82a-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="4e82a-137">여러 사용자 계정을 만들려면</span><span class="sxs-lookup"><span data-stu-id="4e82a-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="4e82a-138">위에서 설명한 데이터로 쉼표로 구분된 값(.csv) 데이터 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="4e82a-139">이후 단계에서 찾아볼 수 있도록 이 파일을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="4e82a-140">**파트너 센터** 메뉴에서 **고객**를 목록에서 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="4e82a-141">**사용자 업로드**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="4e82a-142">**사용자 정보 업로드**에서 **찾아보기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="4e82a-143">파일 선택기에서 데이터 파일을 선택한 다음 **열기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="4e82a-144">**유효성 검사**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-144">Select **Validate**.</span></span>

    <span data-ttu-id="4e82a-145">**참고**  대부분 계정 만들기 오류는 누락 된 정보, 형식이 잘못 되었거나 중복 된 전자 메일 주소 또는 파일에서 너무 많은 레코드를 포함 하 여, 데이터 파일 문제로 인해 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="4e82a-146">파트너 센터 파일 유효성을 검사 한 후 선택 지리적 **위치** 새 사용자에 대 한 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="4e82a-147">**저장**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-147">Select **Save**.</span></span>
9.  <span data-ttu-id="4e82a-148">사용자의 임시 암호 정보를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="4e82a-149">**중요:** 임시 암호를 사용 하 여 파일을 다운로드 해야 합니다. 이제이 작업을 나중에 수행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="4e82a-150">새 사용자는 새 계정의 임시 암호를 사용하여 새 계정에 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="4e82a-151">새 사용자에게 **라이선스 및 서비스를 사용할 수 있는** 권한이 자동으로 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="4e82a-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



