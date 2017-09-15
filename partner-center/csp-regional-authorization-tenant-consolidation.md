---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>CSP regional authorization tenant consolidation

**Applies to**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

\[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.\]

Use these instructions to consolidate tenants for different country/regions.

**참고** 고객이 전환 계정에서 프로비전한 모든 구독 및 실제 사용자 수를 알고 있어야 합니다. Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process. Use the export list feature to help create a list of customers to move over to the centralized tenant. Partners choose to consolidate their tenants. Once consolidation is complete, Partners cannot revert to their previous state. Note that customer action is also be required.

 

## <a name="prepare-for-migration"></a>Prepare for migration


-   Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Migrate customer accounts


1.  전환(새) 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 파트너 센터 대시보드에서 고객 목록으로 이동합니다.

2.  Select Customer.

3.  **재판매인 관계 요청**을 클릭합니다. You are presented with a default email message to present to your customers. This message contains a URL with the org ID unique to your new Partner Center account.

4.  **고객 작업:** 마이그레이션할 각 활성 고객이 이 URL을 방문하도록 합니다. When opening the URL, the customer is prompted to sign in to the Office 365 portal. The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.

5.  After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account. If they agree, the customer selects the checkbox and agrees to authorize the relationship.

The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrating Office 365 and non-Azure usage-based subscriptions


1.  Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.

2.  파트너 센터 대시보드의 왼쪽 탐색에서 **고객**을 클릭합니다.

3.  Open the company name for the customer you want to migrate.

4.  **구독 추가**를 클릭합니다.

5.  Add the correct subscriptions and seat counts from the catalog. **전환 원본** 파트너 계정에 제공된 정보로 확인합니다.

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  **제출**을 클릭합니다.

이제 서비스가 **전환 대상** 파트너 계정의 고객에게 제공됩니다.

Repeat these steps to migrate subscriptions for all additional customers.

Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.

**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabling the Office 365 subscriptions under the Transitioning From partner account


**전환 원본** 파트너 계정에서 CSP 구독을 사용하지 않도록 설정하면 이후 청구가 중지됩니다. You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.

1.  **전환 원본** CSP 계정으로 <https://partnercenter.microsoft.com>에 로그온하고 고객 목록으로 이동합니다.

2.  Open the customer with subscriptions to disable, and then select the first offer to disable.
3.  구독을 **일시 중단됨**으로 설정한 다음 **제출**을 클릭합니다.

    **참고** 구독을 일시 중단하면 이중 청구가 발생하지 않습니다.

     

    구독이 구독 목록에서 **일시 중단됨**으로 표시됩니다.

4.  Repeat these steps for all subscriptions under the customer. 모든 구독이 **일시 중단됨**으로 표시되는지 확인합니다.

5.  Select the next customer on the list and repeat the process of disabling all subscriptions.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrating Azure usage-based subscriptions


Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions. Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account. There will be no disruption of service to the customer during this transition.

1.  Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.
2.  Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.
3.  Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.
4.  The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.
5.  The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.

    **참고** 고객의 구독을 사용하지 않도록 설정해도 고객 목록에서 고객의 모양이 변경되지는 않습니다. There is currently no option to remove customers from the list. 파트너는 나중에 **전환 원본** 계정에서 이러한 고객에 구독을 다시 추가하지 않아야 합니다.

     

6.  모든 고객의 모든 구독에 대해 이러한 단계를 반복하여 이후 **전환 원본** 계정에 요금이 청구되지 않도록 합니다. The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period. No future invoices will generate after that final billing period.

### <a name="notes"></a>Notes

-   Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.

-   Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.

-   There is currently no way to remove a customer from the Customers list completely.

-   **Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.

     

### <a name="simplify-migration-using-export"></a>Simplify migration using Export

**내보내기 기능**을 사용하여 새 통합 구조에서 사용해야 하는 구독을 캡처할 수 있습니다.

1.  대시보드에서 **고객**을 클릭하여 기존 구조에서 고객 목록을 표시합니다.

2.  Open the desired customer name.

3.  **구독** 페이지에서 **구독 내보내기**를 클릭하여 구독 세부 정보를 Excel 파일로 내보냅니다.

4.  Use this list to recreate the subscriptions in your new consolidated tenant.

### <a name="api-registration"></a>API registration

API 등록에 대한 자세한 내용은 [이 페이지를 참조](https://go.microsoft.com/fwlink/?linkid=847990)하세요.

## <a name="partner-center-activity-log"></a>Partner Center Activity log


With the Activity log, partners can view a record of all customer-affecting changes made on their tenant. This helps partners track changes on a customer tenant.

**View the Activity log**

1.  파트너 센터 대시보드에서 **활동 로그** 링크를 클릭합니다.
2.  **활동 로그** 페이지에서 고객 계정에 수행된 변경 내용을 확인합니다. 날짜를 기준으로 활동 로그를 필터링하려면 **시작일** 및 **종료일**을 선택하여 로그에서 선택되는 레코드 범위를 좁힙니다. **활동 로그**에서 고객을 기준으로 필터링하려면 검색 상자를 사용합니다.

**Export the Activity log**

-   **로그 내보내기**를 클릭하여 활동 로그 데이터를 CSV 파일로 내보냅니다.

    You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).

 

 



