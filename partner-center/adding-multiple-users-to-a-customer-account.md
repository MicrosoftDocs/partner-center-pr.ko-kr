---
title: 고객 계정에 대 한 여러 사용자 추가
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 한 번에 여러 사용자를 고객 계정에 추가 하는 방법을 알아봅니다. 쉼표로 구분 된 값 (.csv) 파일 형식을 사용 하 여 파트너 센터에 데이터 파일을 업로드 합니다.
author: parthpandyaMSFT
ms.author: parthp
keywords: 대량 업로드, 고객의 계정에 여러 사용자 추가, 고객의 사용자 추가, 고객 계정, 고객 사용자, 사용자에 대 한 대량 업로드
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 72a1bf634950ac5a445dca894e3925abcae5f645
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377277"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="dba6e-105">고객 계정에 여러 사용자 추가-파트너 센터에 데이터 파일 업로드</span><span class="sxs-lookup"><span data-stu-id="dba6e-105">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="dba6e-106">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="dba6e-106">**Applies to**</span></span>

- <span data-ttu-id="dba6e-107">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="dba6e-107">Partner Center</span></span>

<span data-ttu-id="dba6e-108">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="dba6e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="dba6e-109">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="dba6e-109">Global admin</span></span>

<span data-ttu-id="dba6e-110">쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-110">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="dba6e-111">파트너 센터에서 샘플 데이터 파일을 다운로드 한 다음 사용자가 사용할 수 있도록 편집 하거나 아래에 정의 된 데이터 모델을 사용 하 여 새 데이터 파일을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-111">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="dba6e-112">데이터 파일 요구 사항</span><span class="sxs-lookup"><span data-stu-id="dba6e-112">Data file requirements</span></span>

<span data-ttu-id="dba6e-113">대량 업로드 프로세스를 사용 하 여 고객의 계정에 여러 사용자를 추가 하려면 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-113">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="dba6e-114">고객 계정에 대 한 전역 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-114">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="dba6e-115">각 사용자에 게는 고객의 메일 도메인에 추가 된 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-115">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="dba6e-116">한 번에 최대 100 개의 레코드를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-116">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="dba6e-117">100 명 이상의 사용자를 추가 해야 하는 경우 추가 데이터 파일을 만들고 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-117">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="dba6e-118">모든 사용자는 동일한 지리적 **위치**에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-118">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="dba6e-119">아래에 설명 된 데이터만 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-119">Enter only the data described below.</span></span> <span data-ttu-id="dba6e-120">불필요 한 데이터를 업로드 하면 업로드가 실패 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-120">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="dba6e-121">데이터 파일에 다음 데이터를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-121">Enter the following data in the data file:</span></span>

| <span data-ttu-id="dba6e-122">**열 이름**</span><span class="sxs-lookup"><span data-stu-id="dba6e-122">**Column name**</span></span> | <span data-ttu-id="dba6e-123">**설명**</span><span class="sxs-lookup"><span data-stu-id="dba6e-123">**Description**</span></span>  | <span data-ttu-id="dba6e-124">**제한 사항**</span><span class="sxs-lookup"><span data-stu-id="dba6e-124">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="dba6e-125">이름</span><span class="sxs-lookup"><span data-stu-id="dba6e-125">First name</span></span>  | <span data-ttu-id="dba6e-126">사용자의 이름 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="dba6e-126">User's first name (optional field)</span></span>  | <span data-ttu-id="dba6e-127">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="dba6e-127">50-character limit</span></span>  |
| <span data-ttu-id="dba6e-128">성</span><span class="sxs-lookup"><span data-stu-id="dba6e-128">Last name</span></span>  | <span data-ttu-id="dba6e-129">사용자의 성 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="dba6e-129">User's last name (optional field)</span></span>  | <span data-ttu-id="dba6e-130">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="dba6e-130">50-character limit</span></span>  |
| <span data-ttu-id="dba6e-131">표시 이름</span><span class="sxs-lookup"><span data-stu-id="dba6e-131">Display name</span></span>    | <span data-ttu-id="dba6e-132">파트너 센터 (필수 필드)에 표시 되는 이름</span><span class="sxs-lookup"><span data-stu-id="dba6e-132">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="dba6e-133">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="dba6e-133">50-character limit</span></span>                         |
| <span data-ttu-id="dba6e-134">메일</span><span class="sxs-lookup"><span data-stu-id="dba6e-134">Email</span></span>   | <span data-ttu-id="dba6e-135">고객 회사의 사용자 회사 전자 메일 주소 (필수 필드)</span><span class="sxs-lookup"><span data-stu-id="dba6e-135">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="dba6e-136">각 사용자에게는 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-136">Each user must have a unique email address</span></span> |
| <span data-ttu-id="dba6e-137">상태 업데이트</span><span class="sxs-lookup"><span data-stu-id="dba6e-137">Status update</span></span>   | <span data-ttu-id="dba6e-138">새 사용자 레코드가 성공적으로 만들어졌는지 여부를 나타내는 데 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-138">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="dba6e-139">\*\*비워 둠\*\*</span><span class="sxs-lookup"><span data-stu-id="dba6e-139">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="dba6e-140">여러 사용자 계정을 만들려면</span><span class="sxs-lookup"><span data-stu-id="dba6e-140">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="dba6e-141">위에서 설명한 데이터를 사용 하 여 쉼표로 구분 된 값 (.csv) 데이터 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-141">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="dba6e-142">이후 단계에서 찾아볼 수 있도록 파일을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-142">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="dba6e-143">파트너 센터 [대시보드](https://partner.microsoft.com/dashboard)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="dba6e-144">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-144">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="dba6e-145">고객의 **사용자 및 라이선스** 탭을 선택 하 고 **사용자 업로드**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-145">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="dba6e-146">**사용자 정보 업로드**에서 **찾아보기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-146">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="dba6e-147">파일 선택기에서 데이터 파일을 선택한 다음 **열기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-147">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="dba6e-148">**유효성 검사**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-148">Select **Validate**.</span></span>

    <span data-ttu-id="dba6e-149">**참고**    대부분의 계정 생성 오류는 누락 된 정보, 형식이 잘못 되었거나 중복 된 전자 메일 주소를 포함 하거나 파일에 너무 많은 레코드를 포함 하 여 데이터 파일 문제로 인해 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-149">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="dba6e-150">파트너 센터가 파일의 유효성을 검사 한 후 새 사용자의 지리적 **위치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-150">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="dba6e-151">**저장**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-151">Select **Save**.</span></span>
10. <span data-ttu-id="dba6e-152">사용자에 대한 임시 암호 정보를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-152">Download the temporary password information for the users.</span></span>

<span data-ttu-id="dba6e-153">**중요:** 나중에이 작업을 수행할 수 없으므로 임시 암호를 사용 하 여 파일을 다운로드 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-153">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="dba6e-154">새 사용자는 새 계정에 대 한 임시 암호를 사용 하 여 새 계정에 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-154">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="dba6e-155">새 사용자에 게 **라이선스 및 서비스를 사용할 수 있는** 권한이 자동으로 할당 됩니다.</span><span class="sxs-lookup"><span data-stu-id="dba6e-155">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



