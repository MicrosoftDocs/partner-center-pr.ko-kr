---
title: Office 365 Partner Advisory - Microsoft 365 Voice in CSP | Partner Center
description: PSTN services in some countries may be subject to special tax and regulatory requirements that may affect partner order and invoicing.
ms.topic: article
ms.date: 11/04/2019
author: maggiepuccievans
ms.author: evansma
keywords: Office, O365, PSTN services, taxes, requirements, invoice, invoicing
ms.localizationpriority: medium
ms.openlocfilehash: b6359a49503237e72c8cffdb5758bdd418910306
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384810"
---
# <a name="office-365-partner-advisory-microsoft-365-voice-in-csp"></a>Office 365 Partner Advisory: Microsoft 365 Voice in CSP

**적용 대상**

- 파트너 센터  

Public Switched Telephone Network (PSTN) services in some countries may be subject to special tax and regulatory requirements that may affect partner order and invoicing.  In the United States, Puerto Rico, and Canada, Skype for Business PSTN and Microsoft 365 Voice services are subject to special tax and regulatory requirements. In the United States and Puerto Rico, Microsoft prices PSTN services as tax-inclusive.  Unique PSTN taxes and regulations will affect Office 365 partners transacting Microsoft 365 Voice products.  파트너가 Microsoft PSTN 서비스의 가격을 올리는 경우 PSTN 세금 및 수수료를 계산하고 송금하는 작업을 담당해야 할 수 있습니다.

## <a name="partner-recommendations"></a>Partner Recommendations

세금 및 법률 변호인에게 상담하여 PSTN 서비스 규제, 세금 및 수수료 및 기타 잠재적 책임과 관련한 조직의 책임을 이해합니다.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Invoice Presentation and Partner Reconciliation File

CSP invoices and CSP reconciliation files in the United States, Puerto Rico and Canada which include Skype for Business PSTN and Microsoft 365 Voice services will provide separate line items for the PSTN and non-PSTN components.

Additionally, CSP invoices will display the following footnote:

* The price displayed is a charge for Audio Conferencing and Calling Plan Services.  Any applicable transactional taxes are charged exclusively of the amount shown except for sales made within the United States.  In the U.S., the price displayed is tax inclusive as it includes a charge for the Calling Plan and Audio Conferencing Services and a charge for the taxes and fees we are required to charge.  Audio Conferencing and Calling Plan Services are serviced by the Microsoft Affiliate authorized to provide them.  See [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) for details.

## <a name="reconciliation-file-example"></a>Reconciliation File Example

Office 365 Enterprise E5 presents on reconciliation file as two line items with identical names and identical IDs, but each line item has a unique unit price (example: $28.40 and $2.00). 따라서 Office 365 제품의 비즈니스용 Skype PSTN 회의 구성 요소가 분리되므로 세금을 올바르게 적용할 수 있습니다.

**Partner Reconciliation example #1 (select columns):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |주기 수수료   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |주기 수수료   |2.00   |

**Partner Reconciliation example #2**

Microsoft 365 Business Voice available in Canada has additional PSTN taxable components that are consolidated on CSP Invoice (similar to Office 365 E5, two line items are presented, one for PSTN components and the other for non-PSTN components).  The CSP Reconciliation file for Microsoft 365 Business Voice will display all PSTN taxable components individually (individual PSTN components will not be consolidated in .CSV or API tool).  The summation of order details and billed amounts for customers found in the reconciliation file will match the CSP Invoice.

## <a name="additional-resources"></a>추가 리소스
For more details, visit the [Microsoft 365 for Partners](https://drumbeat.office.com/Pages/home2016.aspx) site.

