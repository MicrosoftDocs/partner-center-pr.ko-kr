---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. 새 제품의 일부로 Microsoft에서는 2016년 11월 1일 고객을 위한 새로운 Microsoft Dynamics 구독 계획을 소개합니다. 이 계획은 현재 계획과 유사하지만 같지는 않습니다.

이 문서의 지침에서는 간접 공급자가 고객의 기존 Microsoft Dynamics AX 구독 및 Microsoft Dymanics CRM Online 구독을 새 Microsoft Dynamics 365로 전환하는 방법을 설명합니다. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

Microsoft Dynamics CRM Online 및 AX 계획은 사용 중지되었습니다.  2017년 7월 1일부터 더 이상 예전 계획으로 갱신할 수 없으며 기존 E4 구독은 만료될 때 자동으로 갱신되지 않습니다.

CRM Online 및 AX 구독은 종료 시 취소됩니다. 고객에게 연속성을 보장하기 위해 구독이 곧 만료되는 고객을 아래에 나열된 지원되는 SKU 옵션으로 전환해야 합니다. 고객 서비스가 중단되는 일이 없도록 구독의 만료 날짜 전에 고객을 새 구독으로 이동하는 것이 좋습니다. 

구독의 세부 정보 페이지에서 만료되는 구독에 대한 구독 상태가 "[날짜]에 자동 갱신"에서 "[날짜]에 만료"로 변경된 것을 볼 수 있습니다. 

API(CREST 또는 파트너 센터)를 사용하는 경우 auto renew = False 속성과 함께 구독의 종료 날짜를 확인하여 곧 만료되는 구독을 검색할 수 있습니다. 언제든지 고객을 새 요금제로 이동할 수 있습니다. 

**Microsoft Dynamics AX 라이선싱 변경**

Microsoft Dynamics AX 제품군은 2016년 11월 1일부터 사용 중지됩니다. Dynamics 365의 새 라이선싱 옵션에 대한 자세한 내용을 알아보려면 [라이선싱 가이드](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)를 검토하세요.

 라이선스 매핑에 대한 자세한 내용은 다음 표를 참조하세요.

|**사용 중지된 SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Microsoft Dynamics 365 for Unified Operations 또는 Microsoft Dynamics 365 계획 |
|작업|Microsoft Dynamics 365 for Activity
|작업/셀프 서비스|Microsoft Dynamics 365 for Team Members|
|장치|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Microsoft Dynamics CRM Online 라이선싱 변경 

**Microsoft Dynamics CRM Online**

현재 Microsoft Dynamics CRM Online 계획은 2016년 11월 1일부터 사용 중지되었습니다. Microsoft Dynamics 365의 새 라이선싱 옵션에 대한 자세한 내용을 알아보려면 [라이선싱 가이드](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)를 검토하세요. 새 라이선싱 옵션에 대한 자세한 내용은 [Important information for CRM Online customers](https://go.microsoft.com/fwlink/?linkid=831667)(CRM Online 고객에 대한 중요 정보)를 참조하세요.

라이선스 매핑에 대한 자세한 내용은 다음 표를 참조하세요.

|**사용 중지된 SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Dynamics 365 엔터프라이즈 고객 참여 계획 |
|Professional|Dynamics 365 엔터프라이즈 고객 참여 계획, Dynamics 365 for Sales 또는 Dynamics 365 for Customer Service|
|Basic|Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service 또는 Dynamics 365 엔터프라이즈 고객 참여 계획|
|Essential|Dynamics 365 for Team Members|
|Field Service 추가 기능|Dynamics 365 엔터프라이즈 고객 참여 계획 또는 Dynamics 365 for Field Service|
|Project Service Authomation 추가 기능|Dynamics 365 엔터프라이즈 고객 참여 계획 또는 Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>새 제품 요금제로 고객 전환


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [이전 구독 취소](#manual-subscription-migration-cancelsubscriptions).

다음 절차에서는 Microsoft Dynamics AX 또는 CRM Online에서 Dynamics 365로 고객을 이동합니다.

재판매인은 Dynamics AX Enterprise에 대한 기존 구독이 있는 고객을 Dynamics 365 for Operations로 이동해야 합니다. 첫 번째 단계는 Dynamics 365 for Operations를 구매하는 것입니다.  Microsoft Dynamics 365로 이동하는 CRM Online 고객에 대해 이러한 단계를 반복합니다.

<a href="" id="purchasenewsubsc"></a>

**새 구독 구매**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



