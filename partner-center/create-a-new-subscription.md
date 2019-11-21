---
title: 고객 구독 만들기, 일시 중단, 또는 취소 | 파트너 센터
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to sell your customers subscriptions to products in the catalog after you have created a customer record in Partner Center.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
Keywords: subscription, create new, add subscription, suspend, cancel, suspension, suspend, SaaS, license, ISV, third party
ms.localizationpriority: medium
ms.openlocfilehash: d829ba7ee520cab42ec5985ac2156ddff60d8e99
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253455"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>고객 구독 만들기, 일시 중단 또는 취소

**적용 대상**

-  파트너 센터
-  Microsoft Cloud for US Government 파트너 센터
-  CSP 파트너

**Appropriate roles**

- 전역 관리자
- 관리자 에이전트

파트너 센터에서 고객 기록을 만들면 카탈로그에서 제품의 구독을 판매할 수 있습니다. This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace). 

일부 제품은 고객당 구독 하나로 제한됩니다. 제한되는 제품 목록을 보려면 파트너 센터 가격 책정 및 제품 페이지를 방문하세요.

>[!IMPORTANT]
As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center. This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access. To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/). For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>새 구독 만들기

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. **구독 추가**를 선택합니다. The **Online Services** tab will show all available Marketplace SaaS offers.

4. 특정 유형의 구독만 표시하려면 사용 가능한 필터 중에서 원하는 필터를 선택합니다.
   - **Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.
   - **Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**. 월간 청구 주기와 연간 청구 주기 중 어떤 것을 선택할지 결정할 때 도움이 되는 정보는 [새 청구 기능에 대한 FAQ](faq-about-new-billing-features.md)를 참조하세요.
   - **Category**: Choose **Enterprise**, **Small business**, or **Trial**. 평가판 구독에 대한 자세한 내용은 [고객에게 Microsoft 제품의 평가판 제공](offer-your-customers-trials-of-microsoft-products.md)을 참조하세요.

5. Select the product subscriptions you want to purchase for your customer. The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied. Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner. This can be because:

    - The customer already has a subscription to that product and is only allowed one

    - The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)
    
    - For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners. The ISV offer may also not be transactable through the Partner Center (e.g. containers or some usage-based offers).  

6. For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.

7. When you are finished adding subscriptions, select **Review** and review your order.

8. Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.

9. After you buy a subscription for a customer, the following will occur:

    - You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page. 여기에서 사용 가능한 경우 추가 기능 라이선스를 선택하거나, 라이선스 수를 변경하거나, 구독을 일시 중단할 수 있습니다.

    **For ISV SaaS (license-based) subscriptions:**
    - You will receive a link to the ISV publisher's site. This link should help you complete the deployment or account setup of the customer's subscription. (Note that neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)
    
    - If your subscription comes with a 30-day free trial, the free trial period will be applied automatically. As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers. Once the free trial period ends, the subscription term will begin and the subscription will convert to paid. The subscription will then auto-renew according to the same schedule.

## <a name="suspend-or-cancel-a-subscription"></a>구독 일시 중단 또는 취소

고객의 요청이 있거나 사기 또는 미결제 발생 시 파트너는 구독을 일시 중단하거나 취소할 수 있습니다.

### <a name="suspend-a-subscription"></a>구독 일시 중단

구독 상태를 **일시 중단됨**으로 변경하면 사용자가 로그인하거나 서비스에 액세스할 수 없습니다.

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. 관리할 구독을 선택합니다.

4. **상태** 섹션에서 **일시 중단**을 선택합니다. 그런 다음 변경 내용을 **제출**합니다.

5. 90일 이내에 또는 90일에 계정이 개설된 시간과 첫 번째 청구 기간 사이의 일 수를 더한 기간(최대 120일) 이내에 구독을 다시 활성화하지 않으면 모든 데이터가 삭제됩니다.

구독을 일시 중단할 경우, **일시 중단** 버튼 아래에 표시된 날짜는 구독을 다시 활성화하지 않을 경우 자동으로 구독이 만료되는 시점을 나타냅니다. For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).

### <a name="cancel-a-subscription"></a>구독 취소

You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md). As long as you cancel within the cancellation period, you will receive a full refund.

For ISV offers billed monthly:

- If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.

- If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.

For offers billed annually:

- If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.

- If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.

After these periods are over, you will no longer see the option to cancel the subscription.

> [!NOTE]
> Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return. Usage-based services can be de-provisioned as a cancellation method. Since charges are billed after use, these services are not eligible for a refund.

To cancel a license-based SaaS subscription from an ISV publisher, do the following:

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3. Locate the subscription you want to cancel.

4. In the **Status** column, select **Cancel**. 그런 다음 변경 내용을 **제출**합니다.

5. If a dialog box appears, fill out any relevant details then select **Submit**.

6. To confirm the cancellation, select **Yes, cancel**.

> [!NOTE]
> You can also choose to cancel an Azure Marketplace subscription using APIs. To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>상업용 마켓플레이스 구독을 자동으로 갱신할지 선택

기본적으로 활성 구독은 구독 기간이 만료되면 자동으로 갱신되도록 설정됩니다. [상업용 마켓플레이스 제품 구독](csp-commercial-marketplace-overview.md)의 경우 필요에 따라 구독을 자동으로 갱신하지 않도록 선택할 수 있습니다.

To stop an active commercial marketplace subscription from automatically renewing:

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. 파트너 센터 메뉴에서 **고객**을 선택한 다음, 목록에서 고객을 선택합니다.

3.  Select **Subscriptions**. This lists any license-based subscriptions you have purchased for the customer.

4.  In the **Subscription** column, select the subscription you want to modify.

5. In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box. 

6. **제출**을 선택합니다.

## <a name="see-also"></a>참고 항목

- [Purchase commercial marketplace products for your customers](csp-commercial-marketplace-purchase.md)
- [Manage commercial marketplace products for your customers](csp-commercial-marketplace-manage.md)
- [Commercial marketplace overview](csp-commercial-marketplace-overview.md)


