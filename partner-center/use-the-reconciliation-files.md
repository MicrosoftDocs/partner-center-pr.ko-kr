---
title: 조정 파일 사용
ms.topic: article
ms.date: 03/26/2021
description: 파트너 센터의 조정 파일에 대해 알아보고, 지정 된 청구 주기에 대 한 자세한 라인 항목 항목 보기를 해석 하는 방법에 대해 알아봅니다.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633899"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="3f7f9-103">파트너 센터 조정 파일의 품목을 읽는 방법에 대해 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="3f7f9-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="3f7f9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3f7f9-105">청구 관리자</span><span class="sxs-lookup"><span data-stu-id="3f7f9-105">Billing admin</span></span>
- <span data-ttu-id="3f7f9-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="3f7f9-106">Global admin</span></span>

<span data-ttu-id="3f7f9-107">청구 주기에서 각 요금에 대 한 자세한 라인 항목 보기를 위해 파트너 센터에서 조정 파일을 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="3f7f9-108">품목 세부 정보에는 각 고객의 구독에 대 한 요금 및 자세한 이벤트 (예: 구독에 대 한 라이선스 추가)가 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="3f7f9-109">**청구서** 를 읽는 방법에 대 한 자세한 내용은 [청구서 읽기](read-your-bill.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="3f7f9-110">조정 파일 필드 이해</span><span class="sxs-lookup"><span data-stu-id="3f7f9-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="3f7f9-111">라이선스 기반 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="3f7f9-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="3f7f9-112">사용량 기반 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="3f7f9-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="3f7f9-113">일일 요금 지정 사용량 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="3f7f9-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="3f7f9-114">일회성 구매 CSP 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="3f7f9-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="3f7f9-115">조정 파일의 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="3f7f9-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="3f7f9-116">조정 파일 ( **Chargetype** 열)의 요금 유형을 이해 하려면 [조정 파일 요금 유형](recon-file-charge-types.md)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="3f7f9-117">서식 지정 문제 해결</span><span class="sxs-lookup"><span data-stu-id="3f7f9-117">Fix formatting issues</span></span>

<span data-ttu-id="3f7f9-118">경우에 따라 조정 파일에 서식 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="3f7f9-119">예를 들어 en-us 로캘이 사용 되지 않는 경우이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="3f7f9-120">조정 파일에서 서식 지정 문제를 해결 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="3f7f9-121">Microsoft Excel에서 조정 파일 (.csv 형식)을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="3f7f9-122">파일의 첫 번째 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="3f7f9-123">**텍스트를 열로 변환 마법사** 를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="3f7f9-124">리본 메뉴에서 **데이터** 를 선택 **하 고 열 텍스트를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="3f7f9-125">마법사에서 **구분 기호로 분리 된 파일 형식** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="3f7f9-126">그다음에 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="3f7f9-127">**구분 기호** 필드에서 **쉼표** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="3f7f9-128">**탭** 이 이미 선택 되어 있으면이 옵션을 선택 된 상태로 둘 수 있습니다. 그런 후 **다음** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="3f7f9-129">**열 데이터 형식** 필드에서 **날짜: MDY** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="3f7f9-130">그다음에 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="3f7f9-131">**열 데이터 형식** 필드에서 모든 금액 열에 대해 **텍스트** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="3f7f9-132">**마침** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="3f7f9-133">프로그래밍 방식으로 조정 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="3f7f9-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="3f7f9-134">조정 파일은 매우 클 수 있으며 다운로드 하기 어려울 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="3f7f9-135">프로그래밍 방식으로 조정 파일을 다운로드 하려면 [청구서 품목 가져오기 항목](/partner-center/develop/get-invoiceline-items)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="3f7f9-136">파일이 Excel에서 행 제한을 초과 하는 경우</span><span class="sxs-lookup"><span data-stu-id="3f7f9-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="3f7f9-137">Microsoft Excel에서 조정 파일을 다운로드할 수 있지만 파일을 열 수 없는 경우에는 파일에 Excel에서 허용 하는 것 보다 많은 행이 포함 되어 있는 것을 의미 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="3f7f9-138">이 경우 아래 절차 중 하나를 사용 하 여 파일을 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="3f7f9-139">Power BI에서 정찰 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="3f7f9-140">일반적으로 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="3f7f9-141">Power BI 인스턴스를 다운로드 하 여 설치 하 고 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="3f7f9-142">Power BI **홈** 탭에서 **데이터 가져오기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="3f7f9-143">**일반 데이터 원본** 목록에서 **Text/CSV** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="3f7f9-144">메시지가 표시 되 면 정찰 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="3f7f9-145">Excel 피벗 테이블에서 정찰 파일 열기</span><span class="sxs-lookup"><span data-stu-id="3f7f9-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="3f7f9-146">일반적으로 조정 파일을 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="3f7f9-147">Microsoft Excel에서 새 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="3f7f9-148">**데이터** 탭에서 **데이터 가져오기** 를 선택 하 고, **파일에서** 를 선택한 다음, **텍스트/CSV** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="3f7f9-149">메시지가 표시 되 면 정찰 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-149">When prompted, open your recon file.</span></span> <span data-ttu-id="3f7f9-150">데이터가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-150">Your data will appear.</span></span>
5. <span data-ttu-id="3f7f9-151">**로드** 드롭다운 메뉴에서 **로드 대상** 을 선택 하 고 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="3f7f9-152">**데이터 가져오기** 대화 상자에서 **피벗 테이블 보고서** 를 선택 하 여 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="3f7f9-153">세금 또는 VAT 지도</span><span class="sxs-lookup"><span data-stu-id="3f7f9-153">Map taxes or VAT</span></span>

<span data-ttu-id="3f7f9-154">청구서에 세금 또는 부가 액 (VAT)을 매핑하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="3f7f9-155">라이선스 기반 파일에서 **세금** 열 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="3f7f9-156">사용량 기반 파일에서 **taxationitem.taxamount** 열의 합계를 계산 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="3f7f9-157">파트너 별로 조정 파일 정리</span><span class="sxs-lookup"><span data-stu-id="3f7f9-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="3f7f9-158">**간접 모델** 의 파트너는 라이선스 기반 조정 파일의 이러한 추가 필드를 사용 하 여 재판매인의 파일을 정리 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="3f7f9-159">MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f7f9-159">MPN ID</span></span> | <span data-ttu-id="3f7f9-160">설명</span><span class="sxs-lookup"><span data-stu-id="3f7f9-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="3f7f9-161">MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f7f9-161">MPN ID</span></span> | <span data-ttu-id="3f7f9-162">CSP (클라우드 솔루션 공급자) 파트너 (직접 또는 간접)의 Microsoft 파트너 네트워크 (MPN) 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="3f7f9-163">대리점 MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f7f9-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="3f7f9-164">[구독에 대 한 레코드 대리점의 MPN 식별자](#reseller-mpn-id)입니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="3f7f9-165">이 필드는 파트너 센터의 특정 구독에 대해 나열 된 재판매인 ID에 해당 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="3f7f9-166">간접 모델의 파트너에 대 한 조정 파일에만 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="3f7f9-167">대리점 MPN ID</span><span class="sxs-lookup"><span data-stu-id="3f7f9-167">Reseller MPN ID</span></span>

<span data-ttu-id="3f7f9-168">CSP 파트너가 직접 구독을 고객에 게 판매 하는 경우 **MPN id** 는 **MPN ID** 와 **재판매인 MPN id** 로 두 번 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="3f7f9-169">CSP 파트너에 **MPN ID** 가 없는 재판매인이 있는 경우이 값은 파트너의 **MPN id** 로 대신 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="3f7f9-170">CSP 파트너가 **재판매인 MPN ID** 를 제거 하는 경우이 값은 *-1* 로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="3f7f9-171">**재판매인 MPN ID** 를 보거나 업데이트 하려면:</span><span class="sxs-lookup"><span data-stu-id="3f7f9-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="3f7f9-172">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="3f7f9-173">파트너 센터 메뉴에서 **고객** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="3f7f9-174">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="3f7f9-175">고객 메뉴에서 **구독** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="3f7f9-176">목록에서 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="3f7f9-177">**업데이트** 를 선택 하 여 **재판매인 (MPN ID)** 을 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f7f9-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3f7f9-178">다음 단계</span><span class="sxs-lookup"><span data-stu-id="3f7f9-178">Next steps</span></span>

- [<span data-ttu-id="3f7f9-179">청구서 & 정찰 파일을 읽는 방법</span><span class="sxs-lookup"><span data-stu-id="3f7f9-179">How to read your bill & recon file</span></span>](read-your-bill.md) 