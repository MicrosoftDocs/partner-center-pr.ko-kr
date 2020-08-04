---
title: 고객 계정에 대 한 여러 사용자를 가져오기 위한 .csv 파일 필드
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객 계정에 여러 사용자를 추가 하려면 적절 한 필드를 사용 하 여 쉼표로 구분 된 값 (.csv) 파일을 만듭니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528187"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="c321c-103">.Csv 파일을 만들어 여러 사용자를 고객 계정에 추가</span><span class="sxs-lookup"><span data-stu-id="c321c-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="c321c-104">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="c321c-104">**Applies to**</span></span>

- <span data-ttu-id="c321c-105">파트너 센터</span><span class="sxs-lookup"><span data-stu-id="c321c-105">Partner Center</span></span>

<span data-ttu-id="c321c-106">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="c321c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="c321c-107">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="c321c-107">Global admin</span></span>

<span data-ttu-id="c321c-108">쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="c321c-109">파트너 센터에서 샘플 데이터 파일을 다운로드 한 다음 사용자가 사용할 수 있도록 편집 하거나 아래에 정의 된 데이터 모델을 사용 하 여 새 데이터 파일을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="c321c-110">데이터 파일 요구 사항</span><span class="sxs-lookup"><span data-stu-id="c321c-110">Data file requirements</span></span>

<span data-ttu-id="c321c-111">대량 업로드 프로세스를 사용 하 여 고객의 계정에 여러 사용자를 추가 하려면 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="c321c-112">고객 계정에 대 한 전역 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="c321c-113">각 사용자에 게는 고객의 메일 도메인에 추가 된 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="c321c-114">한 번에 최대 100 개의 레코드를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="c321c-115">100 명 이상의 사용자를 추가 해야 하는 경우 추가 데이터 파일을 만들고 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="c321c-116">모든 사용자는 동일한 지리적 **위치**에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="c321c-117">아래에 설명 된 데이터만 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-117">Enter only the data described below.</span></span> <span data-ttu-id="c321c-118">불필요 한 데이터를 업로드 하면 업로드가 실패 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="c321c-119">데이터 파일에 다음 데이터를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="c321c-120">**열 이름**</span><span class="sxs-lookup"><span data-stu-id="c321c-120">**Column name**</span></span> | <span data-ttu-id="c321c-121">**설명**</span><span class="sxs-lookup"><span data-stu-id="c321c-121">**Description**</span></span>  | <span data-ttu-id="c321c-122">**제한 사항**</span><span class="sxs-lookup"><span data-stu-id="c321c-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="c321c-123">이름</span><span class="sxs-lookup"><span data-stu-id="c321c-123">First name</span></span>  | <span data-ttu-id="c321c-124">사용자의 이름 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="c321c-124">User's first name (optional field)</span></span>  | <span data-ttu-id="c321c-125">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="c321c-125">50-character limit</span></span>  |
| <span data-ttu-id="c321c-126">성</span><span class="sxs-lookup"><span data-stu-id="c321c-126">Last name</span></span>  | <span data-ttu-id="c321c-127">사용자의 성 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="c321c-127">User's last name (optional field)</span></span>  | <span data-ttu-id="c321c-128">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="c321c-128">50-character limit</span></span>  |
| <span data-ttu-id="c321c-129">표시 이름</span><span class="sxs-lookup"><span data-stu-id="c321c-129">Display name</span></span>    | <span data-ttu-id="c321c-130">파트너 센터 (필수 필드)에 표시 되는 이름</span><span class="sxs-lookup"><span data-stu-id="c321c-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="c321c-131">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="c321c-131">50-character limit</span></span>                         |
| <span data-ttu-id="c321c-132">Email</span><span class="sxs-lookup"><span data-stu-id="c321c-132">Email</span></span>   | <span data-ttu-id="c321c-133">고객 회사의 사용자 회사 전자 메일 주소 (필수 필드)</span><span class="sxs-lookup"><span data-stu-id="c321c-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="c321c-134">각 사용자에게는 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="c321c-135">상태 업데이트</span><span class="sxs-lookup"><span data-stu-id="c321c-135">Status update</span></span>   | <span data-ttu-id="c321c-136">새 사용자 레코드가 성공적으로 만들어졌는지 여부를 나타내는 데 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c321c-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="c321c-137">\*\*비워 둠\*\*</span><span class="sxs-lookup"><span data-stu-id="c321c-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="c321c-138">다음 단계</span><span class="sxs-lookup"><span data-stu-id="c321c-138">Next steps</span></span>

- [<span data-ttu-id="c321c-139">고객에 대해 여러 사용자를 추가 하는 방법</span><span class="sxs-lookup"><span data-stu-id="c321c-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)