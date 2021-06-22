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
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431567"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="e4da0-103">파트너 센터 조정 파일에서 품목을 읽는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="e4da0-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="e4da0-104">**적절한 역할:** 청구 관리자 | 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="e4da0-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="e4da0-105">청구 주기의 각 요금에 대한 자세한 품목 보기를 보려면 파트너 센터 조정 파일을 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="e4da0-106">품목 세부 정보는 각 고객의 구독에 대한 요금 및 자세한 이벤트(예: 구독에 대한 라이선스의 중간 기간 추가)를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="e4da0-107">**청구서를** 읽는 방법에 대한 자세한 내용은 [청구서 읽기를 참조하세요.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="e4da0-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="e4da0-108">조정 파일 필드 이해</span><span class="sxs-lookup"><span data-stu-id="e4da0-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="e4da0-109">라이선스 기반 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="e4da0-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="e4da0-110">사용량 기반 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="e4da0-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="e4da0-111">일일 요금 지정 사용량 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="e4da0-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="e4da0-112">일회성 구매 CSP 조정 파일 필드</span><span class="sxs-lookup"><span data-stu-id="e4da0-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="e4da0-113">조정 파일의 요금 유형 이해</span><span class="sxs-lookup"><span data-stu-id="e4da0-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="e4da0-114">조정 파일의 요금 **유형(ChargeType** 열)을 이해하려면 [조정 파일 요금 유형을 참조하세요.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="e4da0-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="e4da0-115">서식 지정 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e4da0-115">Fix formatting issues</span></span>

<span data-ttu-id="e4da0-116">경우에 따라 조정 파일에 서식 문제가 포함될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="e4da0-117">예를 들어 en-US 로케일을 사용하지 않는 경우 이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="e4da0-118">조정 파일의 서식 문제를 해결하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="e4da0-119">Microsoft Excel에서 조정 파일(.csv 형식)을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="e4da0-120">파일의 첫 번째 열을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="e4da0-121">텍스트를 **열로 변환 마법사 를 엽니다.**</span><span class="sxs-lookup"><span data-stu-id="e4da0-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="e4da0-122">리본에서 **데이터** 를 선택한 다음, **텍스트에서 열로를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="e4da0-123">마법사에서 구분 **기호로 분리된 파일 형식 을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="e4da0-124">그다음에 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="e4da0-125">구분 **기호** 필드에서 **쉼표** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="e4da0-126">**(탭이** 이미 선택된 경우 이 옵션을 선택한 상태로 둘 수 있습니다.) 그런 다음, **다음을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="e4da0-127">열 **데이터 형식** 필드에서 **날짜:MDY** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="e4da0-128">그다음에 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="e4da0-129">열 **데이터 형식** 필드에서 모든 양 열에 대해 **텍스트를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="e4da0-130">**마침** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="e4da0-131">프로그래밍 방식으로 조정 파일 다운로드</span><span class="sxs-lookup"><span data-stu-id="e4da0-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="e4da0-132">조정 파일은 매우 클 수 있으며 다운로드하기 어려운 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="e4da0-133">조정 파일을 프로그래밍 방식으로 다운로드하려면 [청구서 품목 받기를 참조하세요.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="e4da0-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="e4da0-134">파일이 Excel의 행 제한을 초과하는 경우</span><span class="sxs-lookup"><span data-stu-id="e4da0-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="e4da0-135">조정 파일을 다운로드할 수 있지만 Microsoft Excel에서 열 수 없는 경우 파일에 Excel에서 허용하는 것보다 더 많은 행이 포함되어 있는 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="e4da0-136">이 경우 아래 절차 중 하나를 사용하여 파일을 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="e4da0-137">Power BI 정찰 파일 열기</span><span class="sxs-lookup"><span data-stu-id="e4da0-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="e4da0-138">정상적으로 조정 파일을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="e4da0-139">Microsoft Power BI 인스턴스를 다운로드, 설치 및 엽니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="e4da0-140">Power BI **홈** 탭에서 **데이터 받기를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="e4da0-141">일반 데이터 **원본** 목록에서 **Text/CSV를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="e4da0-142">메시지가 표시되면 recon 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="e4da0-143">Excel 피벗 테이블에서 recon 파일 열기</span><span class="sxs-lookup"><span data-stu-id="e4da0-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="e4da0-144">정상적으로 조정 파일을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="e4da0-145">Microsoft Excel에서 새 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="e4da0-146">**데이터** 탭에서 **데이터 받기를** 선택하고 **파일에서** 를 선택한 **다음, Text/CSV** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="e4da0-147">메시지가 표시되면 recon 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-147">When prompted, open your recon file.</span></span> <span data-ttu-id="e4da0-148">데이터가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-148">Your data will appear.</span></span>
5. <span data-ttu-id="e4da0-149">**로드** 드롭다운 메뉴에서 **로 로드를** 선택한 **다음, 확인을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="e4da0-150">데이터 **가져오기** 대화 상자에서 **피벗 테이블 보고서를** 선택하여 파일을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="e4da0-151">음수 양 표시</span><span class="sxs-lookup"><span data-stu-id="e4da0-151">Negative amount displayed</span></span>

<span data-ttu-id="e4da0-152">조정 파일에 음수 금액이 표시되었을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="e4da0-153">이는 다음 중 하나에 의해 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="e4da0-154">최근에 라이선스 수를 취소하거나 줄임</span><span class="sxs-lookup"><span data-stu-id="e4da0-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="e4da0-155">SLA(서비스 사용권 계약) 또는 Azure 사용량에 대한 크레딧을 받았습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="e4da0-156">이 트랜잭션에 대한 자세한 정보를 보려면 조정 파일에서 해당 청구 유형 특성을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="e4da0-157">세금 또는 VAT 매핑</span><span class="sxs-lookup"><span data-stu-id="e4da0-157">Map taxes or VAT</span></span>

<span data-ttu-id="e4da0-158">세금 또는 VAT(부가가치세)를 청구서에 매핑하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="e4da0-159">라이선스 기반 파일에서 **Tax** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="e4da0-160">사용량 기반 파일에서 **TaxAmount** 열의 합계를 계산합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="e4da0-161">파트너별 조정 파일 항목화</span><span class="sxs-lookup"><span data-stu-id="e4da0-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="e4da0-162">**간접 모델의** 파트너는 라이선스 기반 및 사용량 기반 조정 파일 모두에서 이러한 추가 필드를 사용하여 대리점별로 파일을 항목화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="e4da0-163">MPN ID</span><span class="sxs-lookup"><span data-stu-id="e4da0-163">MPN ID</span></span> | <span data-ttu-id="e4da0-164">설명</span><span class="sxs-lookup"><span data-stu-id="e4da0-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="e4da0-165">MPN ID</span><span class="sxs-lookup"><span data-stu-id="e4da0-165">MPN ID</span></span> | <span data-ttu-id="e4da0-166">CSP(클라우드 솔루션 공급자) 파트너(직접 또는 간접)의 MPN(Microsoft 파트너 네트워크) 식별자입니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="e4da0-167">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="e4da0-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="e4da0-168">[구독에 대한 레코드의 대리점 MPN 식별자입니다.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="e4da0-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="e4da0-169">이 필드는 파트너 센터 특정 구독에 대해 나열된 대리점 ID에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="e4da0-170">간접 모델의 파트너에 대한 조정 파일에만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="e4da0-171">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="e4da0-171">Reseller MPN ID</span></span>

<span data-ttu-id="e4da0-172">CSP 파트너가 구독을 고객에게 직접 판매한 경우 **MPN ID는 MPN ID와** Reseller **MPN ID** 둘 다로 두 번 **나열됩니다.**</span><span class="sxs-lookup"><span data-stu-id="e4da0-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="e4da0-173">CSP 파트너에 **MPN ID가** 없는 대리점이 있는 경우 이 값은 대신 파트너의 **MPN ID로** 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="e4da0-174">CSP 파트너가 **Reseller MPN ID** 를 제거하는 경우 이 값은 *-1로* 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="e4da0-175">**Reseller MPN ID** 를 보거나 업데이트하려면:</span><span class="sxs-lookup"><span data-stu-id="e4da0-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="e4da0-176">파트너 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="e4da0-177">파트너 센터 메뉴에서 **고객을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="e4da0-178">목록에서 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="e4da0-179">고객 메뉴에서 **구독을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e4da0-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="e4da0-180">목록에서 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e4da0-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="e4da0-181">**업데이트를** 선택하여 **Reseller(MPN ID) 를 변경합니다.**</span><span class="sxs-lookup"><span data-stu-id="e4da0-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e4da0-182">다음 단계</span><span class="sxs-lookup"><span data-stu-id="e4da0-182">Next steps</span></span>

- [<span data-ttu-id="e4da0-183">청구 & 재구성 파일을 읽는 방법</span><span class="sxs-lookup"><span data-stu-id="e4da0-183">How to read your bill & recon file</span></span>](read-your-bill.md) 