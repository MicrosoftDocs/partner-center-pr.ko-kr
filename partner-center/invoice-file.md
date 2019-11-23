---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389841"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| 필드 | 정의 |
| ----- | ---------- |
| US FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| 고객 번호 | 고객 번호입니다. |
| 청구지 | 송장을 보내는 주소입니다. You can change your company name and/or address in your Partner Center billing profile. |
| 라이선스 기반 요금 | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| 사용량 기반 청구 | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| 할인 | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| 크레딧 | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| Subtotal | 세금 및 세금이 포함되지 않은 요금 및 크레딧 이전의 총계입니다. |
| Tax | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| 다른 크레딧 | 세금이 포함되지 않은 크레딧입니다. |
| 현재 총 요금 | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| 결제 관련 지침 | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| 송장 번호 | 송장의 번호입니다. |
| 청구 기간 | The monthly period leading up to the invoice date. This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count. |
| 송장 날짜 | The billing date or anniversary date on which your invoice is generated each month. |
| 지급 조건 | The payment term. 일회성 구매에 대해서는 항상 60일 이내입니다. |
| 결제 기한 | The date by which your payment must be received. |
| 고객 PO | Your purchase number order. |
| 고객 서비스 | The website address where you can access customer service. |
| 서비스 수령인 | The address where the service is being used. (This is the legal company address associated with company vetting.) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| 필드 | 정의 |
| ----- | ---------- |
| 날짜 | 구매 날짜입니다. |
| 설명 | 제품 이름입니다. |
| Quantity | The number of products (such as reservations) purchased. |
| 단가 | Price per product (such as a reservation). |
| 할인 | 적용 가능한 모든 할인 혜택입니다. |
| 세전 금액 | 세금 부과 전 구입액의 소계입니다. |
| 판매세 | 세금 액수입니다. |
| 총액 | Total amount to be paid. |
