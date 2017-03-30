---
title: "Dynamics AX 구독을 Dynamics 365로 마이그레이션 | 파트너 센터"
description: "Microsoft에서는 조직이 성장, 발전 및 변혁을 통해 고객의 요구 사항을 충족하고 새로운 기회를 포착할 수 있게 해주는 차세대 지능형 비즈니스 응용 프로그램인 Dynamics 365를 소개합니다."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: f19e46da31a7e479ebd3b1cd368ca7646c3c55b7
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Dynamics AX 구독을 Dynamics 365로 마이그레이션

**적용 대상**

-  파트너 센터

Microsoft에서는 조직이 성장, 발전 및 변혁을 통해 고객의 요구 사항을 충족하고 새로운 기회를 포착할 수 있게 해주는 차세대 지능형 비즈니스 응용 프로그램인 Dynamics 365를 소개합니다. 새 제품의 일부로 Microsoft에서는 2016년 11월 1일 고객을 위한 새로운 Microsoft Dynamics 구독 계획을 소개합니다. 이 계획은 현재 계획과 유사하지만 같지는 않습니다.

이 문서의 지침에서는 간접 공급자가 고객의 기존 Microsoft Dynamics AX 구독을 새 Microsoft Dynamics 365로 전환하는 방법을 설명합니다. 이 지침은 공급자가 고객의 구독을 새 SKU로 마이그레이션해야 하는 새 버전으로 업데이트하는 다른 Microsoft 제품에도 적용됩니다.

**Microsoft Dynamics AX 라이선싱 변경**

Microsoft Dynamics AX 제품군은 2016년 11월 1일부터 사용 중지됩니다. Dynamics 365의 새 라이선싱 옵션에 대한 자세한 내용을 알아보려면 곧 게시될 향후 라이선싱 가이드를 검토하세요. 라이선스 매핑에 대한 자세한 내용은 다음 표를 참조하세요.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>사용 중지된 Dynamics AX 라이선스</strong></p></td>
<td><p><strong>Dynamics 365 라이선스</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Dynamics 365 Enterprise Edition Plan 2</p>
<p>또는 Dynamics 365 for Operations</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Task</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Functional</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Device</p></td>
<td><p>Dynamics 365 for Operations Device</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

현재 Microsoft Dynamics CRM Online 계획은 2016년 11월 1일부터 사용 중지될 예정입니다. 새 라이선싱 옵션에 대한 자세한 내용은 [Important information for CRM Online customers](https://go.microsoft.com/fwlink/?linkid=831667)(CRM Online 고객에 대한 중요 정보)를 참조하세요.

## <a name="transition-customers-to-new-product-plans"></a>새 제품 계획으로 고객 전환


Microsoft는 지속적으로 재판매인 및 공급자에 새 제품 및 서비스를 제공합니다. 이러한 경우 재판매인은 고객을 새 서비스로 업그레이드하거나 결국 종료될 SKU의 구독을 마이그레이션해야 할 수 있습니다. 이전 SKU에서 새 SKU로 고객을 마이그레이션하려면 다음 순서가 필요합니다.

-   [새 구독 구매](#manual-subscription-migration-purchasenewsubsc)
-   [현재 사용자 라이선스 다시 할당](#manual-subscription-migration-reassignlicenses)
-   [이전 구독 취소](#manual-subscription-migration-cancelsubscriptions)

다음 절차에서는 Dynamics AX7 Enterprise에서 Dynamics 365 for Operations로 고객을 이동합니다.

<a href="" id="purchasenewsubsc"></a>재판매인은 Dynamics AX Enterprise에 대한 기존 구독이 있는 고객을 Dynamics 365 for Operations로 이동해야 합니다. 첫 번째 단계는 Dynamics 365 for Operations를 구매하는 것입니다.

**새 구독 구매**

1.  **대시보드** 메뉴에서 **고객**을 선택하고 이동하려는 고객을 선택한 다음 **구독 추가**를 선택합니다.
2.  카탈로그에서 구매할 구독을 선택하고(이 경우 Dynamics 365 for Operations, Enterprise Edition) 라이선스 수를 입력한 다음 **제출**을 선택합니다.

    이제 고객은 이전 구독과 새 구독이 둘 다 있어야 합니다. 이 예제에서는 이전 Dynamics AX Enterprise와 새 '대상' 구독인 Dynamics 365 for Operations, Enterprise Edition이 있습니다.

<a href="" id="reassignlicenses"></a> 다음 단계는 새 구독에 모든 기존 사용자 라이선스를 다시 할당하는 것입니다.

**사용자 라이선스 다시 할당**

1.  **대시보드** 메뉴에서 **고객**을 선택하고 이동하려는 고객을 선택한 다음 **사용자 및 라이선스**를 선택합니다. 고객의 사용자 및 라이선스 페이지가 열립니다.
2.  사용자 라이선스를 다시 할당하려면 다시 할당할 사용자를 선택한 다음 **라이선스 관리**를 선택합니다.
3.  **라이선스 관리** 페이지에서 **Dynamics AX Enterprise** 라이선스 확인란을 선택 취소하고 **Dynamics 365 for Operations** 라이선스를 선택합니다.
4.  **제출**을 선택합니다. 확인 페이지에 새 라이선스 할당이 나열됩니다.
5.  라이선스 다시 할당이 필요한 다른 모든 고객 사용자에 대해 같은 단계를 계속합니다.

<a href="" id="cancelsubscriptions"></a> 사용자 라이선스를 새 서비스로 이동한 후 최상위 고객 수준에서 이전 구독을 안전하게 취소할 수 있습니다.

**이전 구독 취소**

1.  **대시보드** 메뉴에서 **고객**을 선택하고 이동하려는 고객을 선택한 다음 취소할 구독을 선택합니다.
2.  구독 세부 정보 페이지에서 구독 **상태**를 **일시 중단됨**으로 설정합니다.
3.  **제출**을 선택합니다.

이전 구독이 일시 중단되고 새 구독이 활성화됩니다. 일시 중단된 구독은 자동으로 120일 후 프로비전이 해제됩니다. 이전 구독에 대해서는 고객에게 추가 비용이 발생하지 않습니다.

## <a name="additional-considerations"></a>추가 고려 사항


이후 구독 프로비전을 위해 고객이 개방형 채널에서 클라우드 서비스 프로그램으로 이전하는 경우 기존 구독도 마이그레이션해야 합니다.

-   고객이 개방형 채널을 통해 이전 구독을 받은 경우 새 SKU의 CSP로 이동하는 작업은 간단합니다.
-   고객이 귀하의 고객으로 아직 설정되지 않은 경우 고객을 초대할 수 있습니다. 자세한 내용은 [고객과의 관계 요청](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) 도움말 항목을 참조하세요.

고객이 귀하를 간접 공급자로 수락한 후 프로비전 단계는 대개 위에 설명된 내용과 같습니다. 즉, 새 구독을 구매한 다음 사용자 라이선스를 할당합니다. 유일한 차이점은 이전 구독 취소가 수반된다는 점입니다. 새 공급자는 다른 채널을 통해 취득한 구독을 일시 중단/취소할 수 없습니다. 고객이 다른 판매 채널(예: 개방형 채널)을 통해 이전 구독을 취득한 경우 고객은 해당 채널을 통해 이전 구독을 직접 취소해야 합니다.

 

 



