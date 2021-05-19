---
title: 고객 계정에 대해 여러 사용자를 가져오는 .csv 파일의 필드
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객 계정에 여러 사용자를 추가하려면 적절한 필드가 있는 쉼표로 구분된 값(.csv) 파일을 만듭니다.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150984"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="8b0be-103">.csv 파일을 만들어 고객 계정에 여러 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="8b0be-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="8b0be-104">**적절한 역할**: 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="8b0be-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8b0be-105">쉼표로 구분된 값 파일 형식(.csv)으로 데이터 파일을 파트너 센터 업로드하여 한 번에 고객 계정에 여러 사용자를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="8b0be-106">파트너 센터 샘플 데이터 파일을 다운로드한 다음, 사용하기 위해 편집하거나 아래에 정의된 데이터 모델을 사용하여 새 데이터 파일을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="8b0be-107">데이터 파일 요구 사항</span><span class="sxs-lookup"><span data-stu-id="8b0be-107">Data file requirements</span></span>

<span data-ttu-id="8b0be-108">대량 업로드 프로세스를 사용하여 고객 계정에 여러 사용자를 추가하려면 다음 요구 사항을 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="8b0be-109">고객 계정에 대한 전역 관리자 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="8b0be-110">각 사용자에게는 고객의 이메일 도메인에 추가된 고유한 이메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="8b0be-111">한 번에 최대 100개 레코드를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="8b0be-112">100명 이상의 사용자를 추가해야 하는 경우 추가 데이터 파일을 만들고 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="8b0be-113">모든 사용자는 동일한 지리적 **위치** 에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="8b0be-114">아래에 설명된 데이터만 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-114">Enter only the data described below.</span></span> <span data-ttu-id="8b0be-115">데이터가 있으면 업로드가 실패합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="8b0be-116">데이터 파일에 다음 데이터를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="8b0be-117">**열 이름**</span><span class="sxs-lookup"><span data-stu-id="8b0be-117">**Column name**</span></span> | <span data-ttu-id="8b0be-118">**설명**</span><span class="sxs-lookup"><span data-stu-id="8b0be-118">**Description**</span></span>  | <span data-ttu-id="8b0be-119">**제한 사항**</span><span class="sxs-lookup"><span data-stu-id="8b0be-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="8b0be-120">이름</span><span class="sxs-lookup"><span data-stu-id="8b0be-120">First name</span></span>  | <span data-ttu-id="8b0be-121">사용자의 이름(선택적 필드)</span><span class="sxs-lookup"><span data-stu-id="8b0be-121">User's first name (optional field)</span></span>  | <span data-ttu-id="8b0be-122">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="8b0be-122">50-character limit</span></span>  |
| <span data-ttu-id="8b0be-123">성</span><span class="sxs-lookup"><span data-stu-id="8b0be-123">Last name</span></span>  | <span data-ttu-id="8b0be-124">사용자의 성(선택적 필드)</span><span class="sxs-lookup"><span data-stu-id="8b0be-124">User's last name (optional field)</span></span>  | <span data-ttu-id="8b0be-125">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="8b0be-125">50-character limit</span></span>  |
| <span data-ttu-id="8b0be-126">표시 이름</span><span class="sxs-lookup"><span data-stu-id="8b0be-126">Display name</span></span>    | <span data-ttu-id="8b0be-127">파트너 센터 표시되는 이름(필수 필드)</span><span class="sxs-lookup"><span data-stu-id="8b0be-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="8b0be-128">50자로 제한</span><span class="sxs-lookup"><span data-stu-id="8b0be-128">50-character limit</span></span>                         |
| <span data-ttu-id="8b0be-129">메일</span><span class="sxs-lookup"><span data-stu-id="8b0be-129">Email</span></span>   | <span data-ttu-id="8b0be-130">고객 회사의 사용자 비즈니스 이메일 주소(필수 필드)</span><span class="sxs-lookup"><span data-stu-id="8b0be-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="8b0be-131">각 사용자에게는 고유한 전자 메일 주소가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="8b0be-132">상태 업데이트</span><span class="sxs-lookup"><span data-stu-id="8b0be-132">Status update</span></span>   | <span data-ttu-id="8b0be-133">새 사용자 레코드가 성공적으로 만들어졌는지 여부를 나타내는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="8b0be-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="8b0be-134">\*\*비워 둠\*\*</span><span class="sxs-lookup"><span data-stu-id="8b0be-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="8b0be-135">다음 단계</span><span class="sxs-lookup"><span data-stu-id="8b0be-135">Next steps</span></span>

- [<span data-ttu-id="8b0be-136">고객에 대해 다수 사용자를 추가하는 방법</span><span class="sxs-lookup"><span data-stu-id="8b0be-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)