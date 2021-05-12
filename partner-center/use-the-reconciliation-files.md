---
title: 조정 파일 사용
ms.topic: article
ms.date: 03/26/2021
description: 파트너 센터 조정 파일 및 지정된 청구 주기에 대한 요금의 자세한 품목 보기를 해석하는 방법에 대해 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794958"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="15220-103">파트너 센터 조정 파일에서 품목을 읽는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="15220-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="15220-104">**적절한 역할:** 청구 관리자 | 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="15220-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="15220-105">청구 주기의 각 요금에 대한 자세한 품목 보기를 보려면 파트너 센터 조정 파일을 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="15220-106">품목 세부 정보는 각 고객의 구독에 대한 요금 및 자세한 이벤트(예: 구독에 대한 라이선스의 중간 기간 추가)를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="15220-107">**청구서를** 읽는 방법에 대한 자세한 내용은 [청구서 읽기를 참조하세요.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="15220-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="15220-108">조정 파일 필드 이해</span><span class="sxs-lookup"><span data-stu-id="15220-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="15220-109">라이선스 기반 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="15220-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="15220-110">사용량 기반 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="15220-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="15220-111">일일 요금 지정 사용량 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="15220-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="15220-112">일회성 구매 CSP 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="15220-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="15220-113">조정 파일의 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="15220-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="15220-114">조정 파일의 요금 **유형(ChargeType** 열)을 이해하려면 [조정 파일 요금 유형을 참조하세요.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="15220-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="15220-115">서식 지정 문제 해결</span><span class="sxs-lookup"><span data-stu-id="15220-115">Fix formatting issues</span></span>

<span data-ttu-id="15220-116">경우에 따라 조정 파일에 서식 문제가 포함될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="15220-117">예를 들어 en-US 로케일을 사용하지 않는 경우 이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="15220-118">조정 파일의 서식 문제를 해결하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="15220-119">Microsoft Excel에서 조정 파일(.csv 형식)을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="15220-120">파일의 첫 번째 열을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="15220-121">텍스트를 **열로 변환 마법사 를 엽니다.**</span><span class="sxs-lookup"><span data-stu-id="15220-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="15220-122">리본에서 **데이터** 를 선택한 다음, **텍스트에서 열로를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="15220-123">마법사에서 구분 **기호로 분리된 파일 형식 을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="15220-124">그다음에 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="15220-125">**구분 기호** 필드에서 **쉼표** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="15220-126">**탭** 이 이미 선택 되어 있으면이 옵션을 선택 된 상태로 둘 수 있습니다. 그런 후 **다음** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="15220-127">**열 데이터 형식** 필드에서 **날짜: MDY** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="15220-128">그다음에 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="15220-129">**열 데이터 형식** 필드에서 모든 금액 열에 대해 **텍스트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="15220-130">**마침** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="15220-131">프로그래밍 방식으로 조정 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="15220-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="15220-132">조정 파일은 매우 클 수 있으며 다운로드 하기 어려울 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="15220-133">프로그래밍 방식으로 조정 파일을 다운로드 하려면 [청구서 품목 가져오기 항목](/partner-center/develop/get-invoiceline-items)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="15220-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="15220-134">파일이 Excel에서 행 제한을 초과 하는 경우</span><span class="sxs-lookup"><span data-stu-id="15220-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="15220-135">Microsoft Excel에서 조정 파일을 다운로드할 수 있지만 파일을 열 수 없는 경우에는 파일에 Excel에서 허용 하는 것 보다 많은 행이 포함 되어 있는 것을 의미 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="15220-136">이 경우 아래 절차 중 하나를 사용 하 여 파일을 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="15220-137">Power BI에서 정찰 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="15220-138">일반적으로 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="15220-139">Power BI 인스턴스를 다운로드 하 여 설치 하 고 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="15220-140">Power BI **홈** 탭에서 **데이터 가져오기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="15220-141">**일반 데이터 원본** 목록에서 **Text/CSV** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="15220-142">메시지가 표시 되 면 정찰 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="15220-143">Excel 피벗 테이블에서 정찰 파일 열기</span><span class="sxs-lookup"><span data-stu-id="15220-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="15220-144">일반적으로 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="15220-145">Microsoft Excel에서 새 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="15220-146">**데이터** 탭에서 **데이터 가져오기** 를 선택 하 고, **파일에서** 를 선택한 다음, **텍스트/CSV** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="15220-147">메시지가 표시되면 recon 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-147">When prompted, open your recon file.</span></span> <span data-ttu-id="15220-148">데이터가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="15220-148">Your data will appear.</span></span>
5. <span data-ttu-id="15220-149">**로드** 드롭다운 메뉴에서 **로 로드를** 선택한 **다음, 확인을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="15220-150">데이터 **가져오기** 대화 상자에서 **피벗 테이블 보고서를** 선택하여 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="15220-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="15220-151">음수 양 표시</span><span class="sxs-lookup"><span data-stu-id="15220-151">Negative amount displayed</span></span>

<span data-ttu-id="15220-152">조정 파일에 음수 금액이 표시되었을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="15220-153">이는 다음 중 하나에 의해 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="15220-154">최근에 라이선스 수를 취소하거나 줄임</span><span class="sxs-lookup"><span data-stu-id="15220-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="15220-155">SLA(서비스 사용권 계약) 또는 Azure 사용량에 대한 크레딧을 받았습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="15220-156">이 트랜잭션에 대한 자세한 정보를 보려면 조정 파일에서 해당 청구 유형 특성을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="15220-157">세금 또는 VAT 매핑</span><span class="sxs-lookup"><span data-stu-id="15220-157">Map taxes or VAT</span></span>

<span data-ttu-id="15220-158">세금 또는 VAT(부가가치세)를 청구서에 매핑하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="15220-159">라이선스 기반 파일에서 **Tax** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="15220-160">사용량 기반 파일에서 **TaxAmount** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="15220-161">파트너별 조정 파일 항목화</span><span class="sxs-lookup"><span data-stu-id="15220-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="15220-162">**간접 모델의** 파트너는 라이선스 기반 및 사용량 기반 조정 파일 모두에서 이러한 추가 필드를 사용하여 대리점별로 파일을 항목화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="15220-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="15220-163">MPN ID</span><span class="sxs-lookup"><span data-stu-id="15220-163">MPN ID</span></span> | <span data-ttu-id="15220-164">Description</span><span class="sxs-lookup"><span data-stu-id="15220-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="15220-165">MPN ID</span><span class="sxs-lookup"><span data-stu-id="15220-165">MPN ID</span></span> | <span data-ttu-id="15220-166">CSP(클라우드 솔루션 공급자) 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="15220-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="15220-167">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="15220-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="15220-168">[구독에 대한 레코드의 대리점 MPN 식별자입니다.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="15220-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="15220-169">이 필드는 파트너 센터 특정 구독에 대해 나열된 대리점 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="15220-170">간접 모델의 파트너에 대한 조정 파일에만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="15220-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="15220-171">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="15220-171">Reseller MPN ID</span></span>

<span data-ttu-id="15220-172">CSP 파트너가 직접 구독을 고객에 게 판매 하는 경우 **MPN id** 는 **MPN ID** 와 **재판매인 MPN id** 로 두 번 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="15220-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="15220-173">CSP 파트너에 **MPN ID** 가 없는 재판매인이 있는 경우이 값은 파트너의 **MPN id** 로 대신 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="15220-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="15220-174">CSP 파트너가 **재판매인 MPN ID** 를 제거 하는 경우이 값은 *-1* 로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="15220-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="15220-175">**재판매인 MPN ID** 를 보거나 업데이트 하려면:</span><span class="sxs-lookup"><span data-stu-id="15220-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="15220-176">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="15220-177">파트너 센터 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="15220-178">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="15220-179">고객 메뉴에서 **구독** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="15220-180">목록에서 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="15220-181">**업데이트** 를 선택 하 여 **재판매인 (MPN ID)** 을 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="15220-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="15220-182">다음 단계</span><span class="sxs-lookup"><span data-stu-id="15220-182">Next steps</span></span>

- [<span data-ttu-id="15220-183">청구서 & 정찰 파일을 읽는 방법</span><span class="sxs-lookup"><span data-stu-id="15220-183">How to read your bill & recon file</span></span>](read-your-bill.md) 