---
title: 고객 계정에 대한 다수의 사용자 만들기 | 파트너 센터
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가 하는 방법에 대해 알아봅니다.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: 대량 업로드, 고객 계정에 여러 사용자 추가, 고객의 사용자 추가, 고객 사용자 대량 업로드, 고객 계정, 고객 사용자, 사용자
ms.localizationpriority: medium
ms.openlocfilehash: 2195d23074a3e7c397b5f557fd3bed9ec0cc518e
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721993"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="ea019-104">고객 계정에 여러 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="ea019-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="ea019-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="ea019-105">**Applies to**</span></span>

- <span data-ttu-id="ea019-106">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="ea019-106">Partner Center</span></span>

<span data-ttu-id="ea019-107">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="ea019-107">**Appropriate roles**</span></span>

- <span data-ttu-id="ea019-108">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="ea019-108">Global admin</span></span>

<span data-ttu-id="ea019-109">쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="ea019-110">파트너 센터에서 샘플 데이터 파일을 다운로드 한 다음 사용자가 사용할 수 있도록 편집 하거나 아래에 정의 된 데이터 모델을 사용 하 여 새 데이터 파일을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="ea019-111">데이터 파일 요구 사항</span><span class="sxs-lookup"><span data-stu-id="ea019-111">Data file requirements</span></span>

<span data-ttu-id="ea019-112">대량 업로드 프로세스를 사용 하 여 고객의 계정에 여러 사용자를 추가 하려면 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="ea019-113">고객 계정에 대한 전역 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="ea019-114">각 사용자는 고객의 메일 도메인에 추가된 고유한 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="ea019-115">한 번에 최대 100개의 레코드를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="ea019-116">100명이 넘는 사용자를 추가해야 할 경우 추가 데이터 파일을 만들어 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="ea019-117">모든 사용자가 같은 지리적 **위치**에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="ea019-118">아래에 설명된 데이터만 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-118">Enter only the data described below.</span></span> <span data-ttu-id="ea019-119">관련 없는 데이터를 입력하면 업로드에 실패하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="ea019-120">데이터 파일에 다음 데이터를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="ea019-121">**열 이름**</span><span class="sxs-lookup"><span data-stu-id="ea019-121">**Column name**</span></span> | <span data-ttu-id="ea019-122">**설명**</span><span class="sxs-lookup"><span data-stu-id="ea019-122">**Description**</span></span>                                                              | <span data-ttu-id="ea019-123">**있다는**</span><span class="sxs-lookup"><span data-stu-id="ea019-123">**Limitation**</span></span>                             |
| <span data-ttu-id="ea019-124">이름</span><span class="sxs-lookup"><span data-stu-id="ea019-124">First name</span></span>      | <span data-ttu-id="ea019-125">사용자의 이름 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="ea019-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="ea019-126">50자 제한</span><span class="sxs-lookup"><span data-stu-id="ea019-126">50-character limit</span></span>                         |
| <span data-ttu-id="ea019-127">성</span><span class="sxs-lookup"><span data-stu-id="ea019-127">Last name</span></span>       | <span data-ttu-id="ea019-128">사용자의 성(선택적 필드)</span><span class="sxs-lookup"><span data-stu-id="ea019-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="ea019-129">50자 제한</span><span class="sxs-lookup"><span data-stu-id="ea019-129">50-character limit</span></span>                         |
| <span data-ttu-id="ea019-130">표시 이름</span><span class="sxs-lookup"><span data-stu-id="ea019-130">Display name</span></span>    | <span data-ttu-id="ea019-131">파트너 센터 (필수 필드)에 표시 되는 이름</span><span class="sxs-lookup"><span data-stu-id="ea019-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="ea019-132">50자 제한</span><span class="sxs-lookup"><span data-stu-id="ea019-132">50-character limit</span></span>                         |
| <span data-ttu-id="ea019-133">이메일</span><span class="sxs-lookup"><span data-stu-id="ea019-133">Email</span></span>           | <span data-ttu-id="ea019-134">고객 회사의 사용자 회사 전자 메일 주소 (필수 필드)</span><span class="sxs-lookup"><span data-stu-id="ea019-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="ea019-135">각 사용자는 고유한 메일 주소가 있어야 함</span><span class="sxs-lookup"><span data-stu-id="ea019-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="ea019-136">상태 업데이트</span><span class="sxs-lookup"><span data-stu-id="ea019-136">Status update</span></span>   | <span data-ttu-id="ea019-137">새 사용자 레코드가 만들어졌는지를 나타내는 데 사용됨</span><span class="sxs-lookup"><span data-stu-id="ea019-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="ea019-138">\*빈\*\*남겨 둡니다 \*</span><span class="sxs-lookup"><span data-stu-id="ea019-138">\*\*Leave empty\*\*</span></span>                        |

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="ea019-139">여러 사용자 계정을 만들려면</span><span class="sxs-lookup"><span data-stu-id="ea019-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="ea019-140">위에서 설명한 데이터로 쉼표로 구분된 값(.csv) 데이터 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="ea019-141">이후 단계에서 찾아볼 수 있도록 이 파일을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="ea019-142">파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="ea019-143">파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="ea019-144">고객의 **사용자 및 라이선스** 탭을 선택 하 고 **사용자 업로드**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="ea019-145">**사용자 정보 업로드**에서 **찾아보기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="ea019-146">파일 선택기에서 데이터 파일을 선택한 다음 **열기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="ea019-147">**유효성 검사**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-147">Select **Validate**.</span></span>

    <span data-ttu-id="ea019-148">**참고**  대부분의 계정 생성 오류는 누락 된 정보, 형식이 잘못 되었거나 중복 된 전자 메일 주소를 포함 하거나 파일에 너무 많은 레코드를 포함 하 여 데이터 파일 문제로 인해 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="ea019-149">파트너 센터가 파일의 유효성을 검사 한 후 새 사용자의 지리적 **위치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="ea019-150">**저장**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-150">Select **Save**.</span></span>
10. <span data-ttu-id="ea019-151">사용자의 임시 암호 정보를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="ea019-152">**중요:** 나중에는 할 수 없으므로 지금 임시 암호를 사용하여 파일을 다운로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="ea019-153">새 사용자는 새 계정의 임시 암호를 사용하여 새 계정에 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="ea019-154">새 사용자에게 **라이선스 및 서비스를 사용할 수 있는** 권한이 자동으로 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="ea019-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



