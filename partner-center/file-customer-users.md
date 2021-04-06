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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441424"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="65745-103">.Csv 파일을 만들어 여러 사용자를 고객 계정에 추가</span><span class="sxs-lookup"><span data-stu-id="65745-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="65745-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="65745-104">**Appropriate roles**</span></span>

- <span data-ttu-id="65745-105">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="65745-105">Global admin</span></span>

<span data-ttu-id="65745-106">쉼표로 구분 된 값 파일 형식 (.csv)의 데이터 파일을 파트너 센터에 업로드 하 여 한 번에 여러 사용자를 고객 계정에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="65745-107">파트너 센터에서 샘플 데이터 파일을 다운로드 한 다음 사용자가 사용할 수 있도록 편집 하거나 아래에 정의 된 데이터 모델을 사용 하 여 새 데이터 파일을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65745-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="65745-108">데이터 파일 요구 사항</span><span class="sxs-lookup"><span data-stu-id="65745-108">Data file requirements</span></span>

<span data-ttu-id="65745-109">대량 업로드 프로세스를 사용 하 여 고객의 계정에 여러 사용자를 추가 하려면 다음 요구 사항을 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="65745-110">고객 계정에 대 한 전역 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="65745-111">각 사용자에 게는 고객의 메일 도메인에 추가 된 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="65745-112">한 번에 최대 100 개의 레코드를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65745-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="65745-113">100 명 이상의 사용자를 추가 해야 하는 경우 추가 데이터 파일을 만들고 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="65745-114">모든 사용자는 동일한 지리적 **위치** 에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="65745-115">아래에 설명 된 데이터만 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-115">Enter only the data described below.</span></span> <span data-ttu-id="65745-116">불필요 한 데이터를 업로드 하면 업로드가 실패 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="65745-117">데이터 파일에 다음 데이터를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="65745-118">**열 이름**</span><span class="sxs-lookup"><span data-stu-id="65745-118">**Column name**</span></span> | <span data-ttu-id="65745-119">**설명**</span><span class="sxs-lookup"><span data-stu-id="65745-119">**Description**</span></span>  | <span data-ttu-id="65745-120">**제한 사항**</span><span class="sxs-lookup"><span data-stu-id="65745-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="65745-121">이름</span><span class="sxs-lookup"><span data-stu-id="65745-121">First name</span></span>  | <span data-ttu-id="65745-122">사용자의 이름 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="65745-122">User's first name (optional field)</span></span>  | <span data-ttu-id="65745-123">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="65745-123">50-character limit</span></span>  |
| <span data-ttu-id="65745-124">성</span><span class="sxs-lookup"><span data-stu-id="65745-124">Last name</span></span>  | <span data-ttu-id="65745-125">사용자의 성 (선택 필드)</span><span class="sxs-lookup"><span data-stu-id="65745-125">User's last name (optional field)</span></span>  | <span data-ttu-id="65745-126">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="65745-126">50-character limit</span></span>  |
| <span data-ttu-id="65745-127">표시 이름</span><span class="sxs-lookup"><span data-stu-id="65745-127">Display name</span></span>    | <span data-ttu-id="65745-128">파트너 센터 (필수 필드)에 표시 되는 이름</span><span class="sxs-lookup"><span data-stu-id="65745-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="65745-129">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="65745-129">50-character limit</span></span>                         |
| <span data-ttu-id="65745-130">Email</span><span class="sxs-lookup"><span data-stu-id="65745-130">Email</span></span>   | <span data-ttu-id="65745-131">고객 회사의 사용자 회사 전자 메일 주소 (필수 필드)</span><span class="sxs-lookup"><span data-stu-id="65745-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="65745-132">각 사용자에게는 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="65745-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="65745-133">상태 업데이트</span><span class="sxs-lookup"><span data-stu-id="65745-133">Status update</span></span>   | <span data-ttu-id="65745-134">새 사용자 레코드가 성공적으로 만들어졌는지 여부를 나타내는 데 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="65745-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="65745-135">\*\*비워 둠\*\*</span><span class="sxs-lookup"><span data-stu-id="65745-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="65745-136">다음 단계</span><span class="sxs-lookup"><span data-stu-id="65745-136">Next steps</span></span>

- [<span data-ttu-id="65745-137">고객에 대해 다수 사용자를 추가하는 방법</span><span class="sxs-lookup"><span data-stu-id="65745-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)