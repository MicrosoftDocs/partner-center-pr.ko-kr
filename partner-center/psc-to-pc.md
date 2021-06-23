---
title: PSC(Partner Sales Connect)에서 마이그레이션
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft 파트너가 PSC(Partner Sales Connect)에서 microsoft 판매자가 보낸 거래를 파트너 센터 만들거나 관리하는 방법을 알아봅니다.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 5be1c09a26cfcc0d038663e5814ccda7e535d4d1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551438"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>PSC(파트너 판매 연결)에서 마이그레이션하는 파트너를 위한 PC(파트너 센터 공동 판매 가이드)

**적절한 역할:** 계정 관리자 | 조회 관리자 | PSC(파트너 판매 연결) 판매자 | PSC(파트너 판매 연결) 관리자 | PSC(파트너 판매 연결) 거래 관리자

이 문서에서는 PSC(파트너 판매 연결)에서 PC(파트너 센터)로 마이그레이션하는 파트너가 파트너 센터 공동 판매 거래를 계속 만들고 관리할 수 있도록 지침을 제공합니다.

>[!Note]
> 마이그레이션에 대한 배너가 PSC에 있으므로 여기 있는 경우 올바른 위치에 있습니다. 이 가이드는 PSC에서 거래를 관리하는 SA(솔루션 평가) 및 OEM 라이선스 비즈니스 파트너에게는 적용되지 않습니다.

>[!Important]
> 2021년 4월 1일부터 회사는 PSC에서 거래를 만들거나 편집할 수 없습니다. **PSC의 대량 내보내기 기능을 사용하여 기존 거래 데이터를 다운로드할 수 있습니다. 또한 이 날짜 이후에 PSC에서 파트너 센터 [열린 거래를 마이그레이션할](psc-to-pc.md#psc-deals-migration) 수 있습니다.** <br><br> IP 공동 판매 인센티브 적격 솔루션을 포함하는 적극적으로 작업 중인 거래가 있는 경우 다음 두 가지 옵션이 있습니다. <br><br> 1. 2021년 3월 31일 이전에 PSC에서 거래를 획득으로 표시하고 거래 등록을 완료합니다. <br> 2. 거래를 처리하고 거래 등록을 시작하는 데 더 많은 시간을 할애할 수 있도록 거래를 파트너 센터 [마이그레이션합니다.](psc-to-pc.md#psc-deals-migration)

알고 있듯이 **회사는 2021년 4월 30일 이후에 PSC에 액세스할 수 없게 됩니다.** 그러나 공동 판매 거래 만들기, 거래 관리 및 Microsoft 판매자가 보낸 거래와 같이 파트너 센터 수행하려는 모든 작업을 찾을 수 있습니다.

그러나 차이점이 있습니다. 다음 지침은 파트너 센터 더 원활하고 간단하게 전환하는 데 도움이 될 수 있습니다.

## <a name="before-you-move-things-you-need-to-know"></a>이동하기 전에 알아야 할 사항

### <a name="if-you-are-a-psc-admin"></a>PSC 관리자인 경우

- [파트너 센터](https://partner.microsoft.com/)로그인하려면 업무 메일이 필요합니다.
- 파트너 센터 계정 [관리자의](permissions-overview.md)도움을 받아 계정을 설정합니다.
- 이 문서를 읽어 파트너 센터 공동 판매 방법을 알아봅니다.
- 모든 PSC 사용자(관리자, 거래 관리자 및 판매자 역할)에 대해 파트너 센터 사용자 계정을 설정하고 [조회 관리자 역할을](permissions-overview.md)할당합니다.

>[!IMPORTANT]
> PSC 배너에 표시된 MPN(Microsoft 파트너 네트워크) ID를 파트너 센터 MPN 위치 목록에서 사용할 수 있는지 확인합니다.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="파트너가 MPN ID를 찾을 수 있는 PSC 배너를 보여주는 이미지.":::

 MPN ID가 파트너 센터 MPN 위치로 표시되는지 확인하려면 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인한 다음, 화면 오른쪽 위에 있는 **설정(기어** 아이콘)을 선택한 다음 계정 **설정** 을 선택합니다. 두 번째 수준의 왼쪽 탐색 메뉴에서 **위치를** 선택하여 파트너 센터 계정과 연결된 모든 MPN ID 및 위치 목록을 확인합니다.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>PSC 거래 관리자 또는 판매자인 경우

- 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard)로그인하려면 업무 메일이 필요합니다.
- PSC에서 회사 이외의 계정을 사용 중이거나 회사 메일이 파트너 회사와 다른 회사에 대한 경우 계정 설정 도움말을 PSC 관리자에게 문의하세요.
- PSC에 로그인하는 데 사용하는 계정에 관계없이 파트너 센터 계정 설정이 완료되었는지 PSC 관리자에게 확인합니다.
- 파트너 센터 및 조회 섹션에 액세스할 수 있는지 확인합니다.
- 워크플로 및 파트너 센터 변경 내용을 이해하려면 이 문서를 참조합니다.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC의 관리자는 다음 단계를 수행합니다.

파트너 센터 왼쪽 탐색 메뉴에서 **조회** 옵션을 선택합니다. 조회 페이지에 액세스할 수 있는지 확인합니다.

  >[!Note]
  > 파트너 센터 로그아웃했다가 다시 로그인하여 조회 페이지에 액세스하기 위해 자격 증명을 새로 고쳐야 할 수 있습니다.

파트너 센터 메뉴 또는 조회 관련 페이지에 **조회** 옵션이 표시되지 않으면 회사의 [계정 관리자에게](permissions-overview.md) 문의하여 **조회** 옵션 및 관련 영역에 대한 액세스 권한을 부여해 달라고 요청합니다.

회사의 계정 관리자를 찾으려면 다음을 수행합니다.

1. 파트너 센터 대시보드의 오른쪽 위에 있는 기어 아이콘에서 **계정 설정을** 선택합니다.

1. 두 번째 수준의 왼쪽 탐색 메뉴에서 **사용자 관리를** 선택합니다.

1. 사용자 목록의 맨 위에서 **필터** 드롭다운 메뉴를 선택합니다. 옵션을 계정 관리자 로 **변경합니다.**

   페이지에는 해당 이메일 주소가 있는 모든 계정 관리자가 표시됩니다. 그 중 하나에 이메일을 보내서 업무 계정에 대한 조회 관리자 역할을 할당하도록 요청합니다.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="파트너 설정 사용자 관리 페이지의 계정 관리자를 보여주는 이미지.":::

>[!Important]
>- 사용자 역할이 PSC의 사용자 관리만 포함하는 경우 회사의 계정 관리자에게 파트너 센터 [계정 관리자](permissions-overview.md#manage-mpn-membership-and-your-company) 역할을 할당하도록 요청합니다. 
>- 공동 판매 기회 관리도 역할에 포함되는 경우 추천 관리자 역할을 할당하도록 [요청합니다.](permissions-overview.md#manage-referrals)
> - 또한 PSC 관리자 중 하나의 변경 관리 리더를 지정하는 것이 좋습니다. 이렇게 하면 모든 PSC 관리자가 파트너 센터 계정 관리자에게 개별적으로 연락할 필요가 없습니다. 대신 변경 관리 책임자는 파트너 센터 계정 관리자로 작업하는 기본 사람이 될 수 있습니다.

## <a name="user-migration"></a>사용자 마이그레이션

파트너 센터 계정을 설정한 후 공동 판매 기회 페이지의 사용자 마이그레이션 마법사를 사용하여 회사 직원에게 파트너 센터 역할을 자동으로 할당합니다.

>[!Note]
> 사용자 마이그레이션은 회사의 [계정 관리자만](permissions-overview.md#manage-mpn-membership-and-your-company) 수행할 수 있습니다. 계정 관리자 역할이 없는 경우 사용자 마이그레이션 마법사의 도움을 받아 사용자 계정을 설정할 수 있는 계정 관리자를 찾습니다.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="사용자 마이그레이션 마법사를 보여주는 이미지.":::

계정 관리자는 추천 가이드 옆에 있는 공동 판매 기회 페이지에 PSC 사용자 마이그레이션 마법사 링크가 표시됩니다. 링크를 선택하여 사용자 마이그레이션을 시작할 수 있습니다. 사용자 마이그레이션을 시작하려면 관리자가 링크를 선택할 수 있습니다. 모든 사용자에게 파트너 센터 적절한 역할이 할당될 때까지 이 사용자 마이그레이션 단계를 여러 번 수행할 수 있습니다.

사용자 마이그레이션 테이블에는 다음과 같은 세부 정보가 있습니다.

- 사용자 계정 - 직원의 이메일 ID
- PSC 파트너 계정 - PSC에서 직원이 연결된 계정
- PSC 사용자 역할 - PSC에서 에 할당된 세 가지 역할 중 하나입니다.
- PC MPN 위치 - 사용자에게 PC(관련 파트너 센터) 역할을 부여할 위치입니다. PSC 파트너 계정 MPN은 파트너 센터 권한을 할당할 동등한 MPN 위치를 찾는 데 사용됩니다. 전체 조직은 vOrg MPN ID를 표시합니다.
- PC 사용자 역할 - 직원에게는 PSC 사용자 역할에 따라 역할이 할당됩니다. PSC의 관리자는 파트너 센터 조회 관리자 역할이 할당됩니다. 판매자에게 파트너 센터 추천 사용자 역할이 할당됩니다. 파트너 센터 역할에 대해 자세히 알아보고 이러한 역할을 가진 사용자가 여기에서 파트너 센터 수행할 수 있는 작업을 [알아봅니다.](permissions-overview.md#manage-referrals)
- PC AAD 테넌트 - 파트너 센터 사용자가 할당된 Microsoft Azure Active Directory(Azure AD) 테넌트
- 상태 - 마이그레이션 상태에 대한 세 가지 가능한 상태가 있습니다.
    - **마이그레이션되지 않음** - 사용자에게 할당된 파트너 센터 조회 역할이 없습니다.
    - **마이그레이션됨** - 표에 표시된 대로 관련 역할이 할당된 사용자가 성공적으로 마이그레이션되었습니다.
    - **오류** - 일부 오류로 인해 마이그레이션을 완료할 수 없음

경우에 따라 마이그레이션이 실패하고 오류가 발생할 수 있습니다. 다음은 마이그레이션으로 인해 오류가 발생할 수 있는 몇 가지 이유와 문제를 해결하는 몇 가지 방법입니다.

1. PSC 사용자가 비작업 계정을 사용하고 있을 수 있습니다.

2. PSC 사용자는 파트너 센터 사용하는 도메인과 다른 도메인의 계정을 사용하고 있을 수 있습니다.

   시나리오 1 및 2와 관련된 오류를 해결하려면 Azure AD 테넌트에서 연결된 작업 계정을 사용하여 파트너 센터 로그인하도록 사용자에게 요청합니다. [전역 관리자가](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) 도움을 줄 수 있습니다.
   
   전역 관리자를 찾으려면 다음을 수행합니다. 
   - 파트너 센터 [대시보드에](https://partner.microsoft.com/dashboard) 로그인하고 오른쪽 위에 있는 기어 아이콘에서 **계정 설정을** 선택합니다.
   - 두 번째 수준의 왼쪽 탐색 모음에서 **사용자 관리를** 선택합니다.
   - 사용자 목록 맨 위에서 **필터** 드롭다운 메뉴를 선택하고 옵션을 **전역 관리자** 로 변경합니다. 그러면 페이지에 해당 이메일 주소가 있는 모든 전역 관리자가 표시됩니다. 그 중 한에게 작업 계정에 대한 조회 관리자 역할을 할당하도록 요청합니다.
   
      전역 관리자는 Azure AD 테넌트에서 새 사용자 계정을 만들거나 게스트 사용자 액세스 권한을 다른 도메인 계정 사용자에게 할당할 수 있습니다. 모든 PSC 거래 관리자 및 사용자에 대해 계정이 설정되면 파트너 센터 로그인하고, 왼쪽 탐색 메뉴에서 **조회를** 선택하고, 조회 페이지를 볼 수 있는지 확인해야 합니다.

3. 사용자에게 파트너 센터 할당된 조회 역할이 이미 있습니다.
    - 사용자의 기존 역할을 확인할 수 있습니다. 파트너 센터 오른쪽 위 모서리에서 **설정(기어** 아이콘), **계정 설정을** 선택합니다. 두 번째 왼쪽 탐색 메뉴가 표시되면 **사용자 관리를** 선택하고 사용자를 검색합니다.

## <a name="psc-deals-migration"></a>PSC 거래 마이그레이션

사용자 마이그레이션을 완료한 후 공동 판매 기회 페이지의 거래 마이그레이션 마법사를 사용하여 PSC에서 파트너 센터 모든 적격 오픈 거래를 가져옵니다. **거래 마이그레이션 링크는 파트너 센터 전체 조직 범위를 가진 추천 관리자만 볼 수 있습니다.** 공동 판매 기회 페이지의 오른쪽 위에 **"PSC 거래 마이그레이션"이라는** 링크가 표시되어 거래 마이그레이션 마법사가 열립니다.

거래 마이그레이션을 시작하기 전에 이 섹션을 읽습니다.

**마이그레이션에 적격**

일부 거래만 PSC에서 파트너 센터 마이그레이션할 수 있습니다. 이 마이그레이션 마법사는 파트너가 거래를 성사시키기 위해 고객과 적극적으로 협력하는 파트너 센터 거래를 할 수 있도록 돕기 위해 빌드되었습니다. **올바른 파트너 계정 세부 정보 (올바른 MPN ID)를 사용 하 여 1 월 1 2020 일에 생성 된 미해결 상태의 거래만 마이그레이션에 적합 합니다.**

**마이그레이션에 적합 하지 않음**

- 솔루션 평가 거래는 거래 마이그레이션에 적합 하지 않습니다.
- OEM 라이선스 비즈니스 거래는 거래 마이그레이션에 적합 하지 않습니다.
- PSC에서 성공으로 표시 된 모든 거래는 마이그레이션에 적합 하지 않습니다. 성공으로 표시 된 거래에 적격 한 경우에는 PSC에서 완료 해야 합니다.

## <a name="pre-requisites-for-deal-migration"></a>거래 마이그레이션에 대 한 필수 구성 요소

파트너 센터에서의 마이그레이션 처리를 시작 하기 전에 다음 지침에 따라 성공적인 마이그레이션에 대 한 PSC의 거래를 설정 합니다.

1. 회사에서 오픈 거래에 대해 작업 하는 모든 영업 팀 구성원은이 마이그레이션에 대 한 정보를 받습니다.
2. 영업 팀 멤버는 거래 센터를 사용 하 여 거래 관리를 위해 교육을 받습니다.
3. 거래에는 아래에 설명 된 대로 필요한 모든 정보가 포함 되어 있습니다.
    - 이름 및 주소를 포함 한 고객 회사 세부 정보
    - 공동 판매 거래 인 경우 고객 연락처 세부 정보
    - 하나 이상의 솔루션
    - 모든 세부 정보 (이름, 성, 전자 메일 ID 및 전화 번호)가 있는 팀 구성원 하나 이상
    - 거래 값
    - 예상 되는 종료 날짜
    - 파트너 정보

PSC에서 대량 다운로드 및 업로드 기능을 사용 하 여 모든 적격 거래에 대 한 거래에 누락 된 세부 정보를 모두 추가할 수 있습니다.

>[!Note]
> 위의 필수 구성 요소가 충족 되지 않더라도 마이그레이션에 성공 합니다. 그러나 파트너 센터에서 위에 언급 된 필수 필드를 사용할 수 없는 경우에는 거래 상태를 변경할 수 없습니다. 그런 다음 파트너 센터의 거래 센터에서 누락 된 모든 필수 정보를 입력 하 여 작업을 시작 해야 합니다. **파트너 센터로 마이그레이션하기 전에 PSC에서 적격 거래를 정리 하는 것이 좋습니다.**

파트너 센터의 거래 마이그레이션은 한 번의 클릭 환경으로 빌드됩니다. 회사에서 적격 거래를 마이그레이션할 준비가 되 면 **"거래 마이그레이션"** 단추를 선택 하기만 하면 됩니다. **PSC에서 마이그레이션하려는 거래를 선택할 수 없습니다. 파트너 센터에 대 한 거래를 마이그레이션하지 않으려는 경우 마이그레이션을 시작 하기 전에 PSC에서 closed 상태로 전환 합니다.**

>[!Note]
> 마이그레이션을 시작한 후에 **는 해당 거래를 마이그레이션하는 데 최대 24 시간이 걸릴 수 있습니다**.

마이그레이션이 완료 되 면 배너 메시지의 상태가 마이그레이션 보고서에 대 한 링크를 사용 하 여 완료로 변경 됩니다. 보고서를 다운로드 하 여 PSC에서 파트너 센터로 마이그레이션한 거래의 세부 정보를 확인 합니다.

이 보고서에는 다음과 같은 세부 정보가 포함 되어 있습니다.

1. **파트너 센터 ENGAGEMENT ID** -engagement의 모든 거래에 대 한 파트너 센터의 고유 식별자입니다. 파트너에 대 한 두 가지 거래와 파트너 센터의 공동 판매 참여에 Microsoft 용 거래가 있습니다.
2. 파트너 **센터 조회 ID** -파트너에 속하는 거래의 파트너 센터에서 고유한 식별자입니다.
3. **거래 이름** -PSC의 거래에 지정 된 식별자입니다.
4. **Psc 거래 ID** -거래의 psc에서 고유 식별자입니다.
5. **오류** -특정 거래를 마이그레이션하는 동안 오류가 있는지 여부를 표시 합니다.

성공적으로 마이그레이션된 모든 거래는 PSC에 표시 되지 않습니다. 파트너 센터에서의 거래 등록 완료를 포함 하 여 파트너 센터의 마이그레이션된 거래에 대해 계속 작업할 수 있습니다. 공동 판매 거래의 경우 Microsoft 판매자와의 상호 작용은 변경 되지 않습니다.

PSC에서 마이그레이션한 거래는 거래의 원본에 따라 인바운드 및 아웃 바운드 탭에서 사용할 수 있습니다. 회사에서 공유 하는 모든 거래는 아웃 바운드 탭에서 사용할 수 있으며, Microsoft에서 시작한 거래는 파트너 센터의 인바운드 탭에서 제공 됩니다. 마이그레이션 후에는 두 가지 유형의 거래를 만들 수 있습니다.

1. **공동 판매 거래** -PSC에서 공동 판매로 표시 되는 거래는 파트너 센터에서 공동 판매 거래로 생성 됩니다.
2. 공동 판매로 표시 되지 않은 **파트너 주도** 거래 사항은 파트너 센터에서 파트너 주도 거래로 생성 됩니다. 파트너 주도 거래는 Microsoft 판매자에 게 표시 되며, 터미널 상태 (성공, 손실)에 도달 하기 전에 공동 판매 거래로 업그레이드할 수 있습니다. 또한 거래에 적합 한 솔루션이 있는 경우 파트너 주도 거래는 거래를 등록 하는 데 적합 합니다.

>[!Important]
> 일부 거래를 마이그레이션할 수 없기 때문에 오류가 발생 하는 경우 **"거래 마이그레이션" 단추를 클릭 하 여 거래 마이그레이션을 다시 시작할 수** 있습니다. 아직 마이그레이션해야 하는 적격 거래가 있는 경우에만 사용할 수 있습니다. 이는 초기 마이그레이션을 시작한 후 PSC에서 몇 가지 새로운 거래를 만드는 전환 단계에 있는 경우에도 유용 합니다.

모든 거래를 성공적으로 마이그레이션한 후에는 " **거래** **하지 않음** " 단추를 **사용 하지 않도록 설정** 하는 배너를 표시 합니다.

사용자 마이그레이션 및/또는 마이그레이션 작업을 완료 한 후에는 다음 지침을 사용 하 여 마이그레이션 전략을 결정 합니다.

회사에 PDM (파트너 개발 관리자)이 있는 경우-파트너 센터 계정이 설정 되 고 사용자가 이동 하 여 역할 및 권한이 있는 경우 공동 판매 작업을 파트너 센터로 이동할 수 있습니다. 마이그레이션이 완료 될 때까지 기다리지 않고 스위치를 설정 하 여 모든 새 거래를 파트너 센터로 이동 하 게 하는 것을 PDM에 알립니다.

>[!Note]
>이 스위치를 만든 후에는 PSC의 기존 활성 거래에 대해서만 작업을 수행할 수 있습니다. 새 거래를 만들거나 PSC의 Microsoft 판매자 로부터 거래를 받을 수 없습니다.

회사에서 PDM을 사용 하지 않는 경우 모든 사용자 계정이 설정 되 고 모든 사용자가 확인 하는지 확인 합니다. 파트너 센터에서 공동 판매를 시작할 수 있는 정확한 날짜와 관련 하 여 PSC의 전자 메일과 배너를 통해 알림이 제공 됩니다. PSC에서 기존 활성 거래를 관리 해야 한다는 점에 주의 해야 합니다.

>[!Important]
> 2021 년 4 월 30 일까 지 성공으로 표시 되는 거래를 등록할 수 있습니다.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC 관리자, PSC 거래 관리자 및 PSC 판매자를 위한 다음 단계

파트너 센터에 공동 판매 하는 방법에 대해 알아봅니다.
이는 파트너 센터에서 공동 판매를 위해 준비 하는 데 도움이 되는 중요 한 단계입니다. 파트너 센터의 워크플로와 변경 사항을 이해 하 여 효과적으로 공동 판매할 수 있도록 합니다. 이 문서를 완전히 읽고 시작 합니다. [공동 판매 환경 갤러리](https://aka.ms/cosellexperience)에서도 적절 한 리소스 집합을 사용할 수 있습니다.

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>PSC와 파트너 센터 워크플로 간의 주요 차이점

|**시나리오**|**파트너 판매 연결**|**파트너 센터**|
|-----|:-----|:-----|
|사용자 역할|PSC에는 관리자, 거래 관리자 및 판매자 역할이 있습니다.|파트너 센터에는 모든 거래에 대해 읽기 및 쓰기 권한을 모두 제공 하는 [조회 관리자](permissions-overview.md#manage-referrals) 역할만 있습니다.|
|공동 판매 거래에 Microsoft 초대|Microsoft 판매자에 의해 시작 된 파트너에 게는 명시적으로 묻지 않습니다.|파트너는 Microsoft 판매자 도움말이 거래에 필요한 경우 [명시적 요청](manage-co-sell-opportunities.md#add-solutions) 을 해야 합니다. Microsoft 판매자에 게 요청을 거부 하는 옵션이 있습니다.|
|만료|거래 만료 라는 개념은 없습니다.|파트너 인바운드 거래는 파트너에 의해 허용 되지 않는 경우 14 일 후에 만료 됩니다. Microsoft 판매자가 14 일 내에 작업 하지 않는 경우 만료 된 상태로 전환할 수 있는 파트너 아웃 바운드 거래의 경우에도 마찬가지입니다.|
|Microsoft 판매자 세부 정보|거래를 만드는 즉시 표시 됩니다.|판매자가 파트너의 공동 판매 초대를 명시적으로 수락 하는 경우에만 Microsoft 판매자 세부 정보가 파트너와 공유 됩니다.|
|[개인 파이프라인](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|사용할 수 없습니다.|파트너는 Microsoft 판매자에 게 가시성을 제공 하지 않고 파이프라인을 공유할 수 있습니다.|
|솔루션|하나 이상의 가격 목록에 속한 솔루션도 거래에 추가할 수 있습니다.|파트너는 다음 목록을 포함 하는 [솔루션](manage-co-sell-opportunities.md#add-solutions) 을 추가할 수 있습니다. a) 자사 솔루션 b) Microsoft 자사 카탈로그 (PSC의 트랜잭션 거래 역할과 비슷함) 및 c) 다른 타사 파트너의 공동 판매 솔루션 (PSC의 ISV 거래 역할과 비슷함)|
|거래 과제|할당 된 판매자만 거래를 보고 작업할 수 있습니다.|팀 멤버를 거래에 추가 하 여 거래를 담당 하는 사용자를 지정할 수 있으며, 다른 조회 관리자가 해당 거래를 보거나 작업을 수행할 수 없도록 차단 되지 않습니다.|
|고객 조직|자유 형식 텍스트 항목입니다.|몇 자만 입력 하면 [D&B 데이터베이스](https://www.dnb.com/) 에 대해 [고객 조직을](manage-co-sell-opportunities.md#select-your-customer) 검색할 수 있습니다. 올바른 이름 및 주소는 선택에 따라 자동으로 채워집니다.|
|고객 연락처|필수가 아닙니다.|개인 파이프라인 공유의 경우 필수 항목이 아닙니다. Microsoft 판매자가 공동 판매 요청에 참여하도록 초대된 경우 필요합니다.|
|공용 API|사용할 수 없습니다.|프로그래밍 방식으로 파트너 센터 조회를 관리하는 [공용 API입니다.](/partner/develop/referrals)|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>PSC의 필드를 의 해당 필드에 매핑합니다파트너 센터

이 섹션에서는 PSC에 대해 선택한 스크린샷(또는 "지도")을 파트너 센터 공동 판매 기회 섹션의 해당 보기와 비교합니다.

각 스크린샷 쌍에 번호가 매겨진, 노란색 또는 빨간색 원이 표시됩니다.

- **노란색 원의 의미는 무엇인가요?** 번호가 매겨진 노란색 원은 각 PSC 스크린샷에 먼저 표시됩니다. 그런 다음, 동일한 숫자가 많이 있는 도우미 파트너 센터 스크린샷을 찾을 수 있습니다.

   PSC의 각 필드 또는 특성이 파트너 센터 해당 필드와 매핑되는 방식을 확인하려면 두 개의 관련 스크린샷에서 번호가 매겨진 원과 일치합니다. 예를 들어 첫 번째 PSC 스크린샷의 번호가 매겨진 노란색 "1"을 두 번째의 번호가 매겨진 노란색 "1"과 파트너 센터 그 아래 스크린샷과 일치합니다.

- **빨간색 원은 무엇을 의미하나요?** 한 스크린샷에 빨간색 원이 표시되면 파트너 센터 PSC 필드를 사용할 수 없다는 것을 나타냅니다.

PSC-파트너 센터 필드 매핑은 다음 영역에 대해 표시됩니다.

1. 파트너 센터 공동 판매 기회 기본 보기에 매핑된 PSC 홈페이지
1. 파트너 센터 거래 보기에 매핑된 PSC 그리드 보기
1. 파트너 센터 거래 세부 정보 보기에 매핑된 PSC 거래 세부 정보 보기
1. 파트너 센터 솔루션 추가 보기에 매핑된 PSC 제품 추가 보기
1. 파트너 센터 사용자 관리 뷰에 매핑된 PSC 사용자 관리 뷰
1. 파트너 센터 역할 할당 보기에 매핑된 PSC 사용자 역할 할당 보기
1. 파트너 센터 알림 보기에 매핑된 PSC 알림 보기

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - 파트너 센터 공동 판매 기회 기본 보기에 매핑된 PSC 홈페이지

맨 위 PSC 스크린샷과 그 아래의 파트너 센터 스크린샷 간에 일치하는 번호가 매겨진 원을 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 일치하는 파트너 센터 필드가 없음을 나타냅니다.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Partner Sales Connect의 홈페이지와 파트너 센터 공동 판매 기회의 기본 보기 간의 필드 매핑을 보여주는 이미지." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - 파트너 센터 거래 보기에 매핑된 PSC 그리드 보기

맨 위 PSC 스크린샷과 그 아래의 파트너 센터 스크린샷 간에 일치하는 번호가 매겨진 원을 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 일치하는 파트너 센터 필드가 없음을 나타냅니다.  

> [!NOTE]
> 스크린샷 아래에 다른 고려 사항이 표시됩니다.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="PSC(Partner Sales Connect) 그리드 보기와 파트너 센터 거래 보기 간의 필드 매핑을 보여주는 이미지" lightbox="images/pscmigration/grid-view-expanded.png":::

**특별 고려 사항:**

- 파트너 센터 PSC와 같은 목록 보기가 없습니다.  모든 계약은 고객 정보 및 거래 유형과 함께 수신되거나 생성된 최신 날짜를 기준으로 나열됩니다. 보기의 첫 번째 계약은 기본적으로 선택됩니다. PSC 테이블 형식으로 표시되는 대부분의 값은 파트너 센터 거래 세부 정보 보기에서 사용할 수 있습니다.
- 거래 역할은 파트너 센터 필수 필드가 아닙니다. 워크플로에는 표시되지 않거나 캡처되지 않습니다. 이 솔루션은 거래로 추가된 솔루션에 따라 Microsoft 판매자 쪽에서 자동으로 파생됩니다.
- 마지막으로 수정한 날짜는 파트너 센터 조회 세부 정보 페이지에 표시되지 않습니다. 파트너는 정렬 기능을 사용하여 마지막 업데이트 날짜를 기준으로 거래를 정렬할 수 있습니다.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - 파트너 센터 매핑된 PSC 거래 세부 정보 보기

맨 위(PSC) 스크린샷의 일치하는 번호가 매겨진 원을 아래의 파트너 센터 스크린샷과 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 파트너 센터 일치하는 필드 또는 영역이 없음을 나타냅니다.

> [!NOTE]
> 스크린샷 아래에 다른 고려 사항이 표시됩니다.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="PSC(파트너 판매 연결) 거래 세부 정보 보기와 파트너 센터 거래 세부 정보 보기 간의 필드 매핑을 보여주는 이미지." lightbox="images/pscmigration/deal-details-expanded.png":::

**특별 고려 사항:**

- 파트너는 파트너 거래 세부 정보 보기에서 편집 단추를 선택하여 거래를 편집할 수 있습니다(6). 편집 단추를 선택하면 모든 필드를 편집할 수 있습니다. 그런 다음, 거래 편집을 저장하거나 취소할 수 있는 옵션이 있습니다.
- 파트너 센터 거래를 중복으로 닫을 수 있는 옵션은 없습니다.
- 고객 결과는 파트너 센터 사용할 수 없습니다. 고객 상호 작용과 관련된 모든 세부 정보는 파트너 센터 Notes 섹션에서 업데이트할 수 있습니다.
- 예상 솔루션 종료 날짜는 파트너 센터 OEM IOT 거래에만 사용할 수 있습니다. 이 정보는 다른 거래 유형에 대해서는 표시되지 않습니다.
- 파트너 센터 라이선스 프로그램은 필요하지 않습니다. 이 정보는 거래 시 선택한 솔루션에 따라 자동으로 유추됩니다.

>[!Note]
>획득 또는 손실로 표시된 모든 거래를 나중에 편집할 수 없습니다. 이러한 터미널 상태 중 하나로 거래를 이동하는 동안 주의해야 합니다.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - 파트너 센터 '솔루션 추가' 보기에 매핑된 PSC '제품 추가' 보기

맨 위(PSC) 스크린샷의 일치하는 번호가 매겨진 원을 아래의 파트너 센터 스크린샷과 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 파트너 센터 일치하는 필드 또는 영역이 없음을 나타냅니다.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="PSC(Partner Sales Connect) 제품 추가 보기와 솔루션 추가 보기 간의 필드 매핑을 보여 파트너 센터 이미지." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - PSC 및 파트너 센터 사용자 관리

맨 위(PSC) 스크린샷의 일치하는 번호가 매겨진 원을 아래의 파트너 센터 스크린샷과 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 파트너 센터 일치하는 필드 또는 영역이 없음을 나타냅니다.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="계정 설정 영역 내의 PSC(Partner Sales Connect) 사용자 관리 홈과 파트너 센터 사용자 관리 페이지 보기 간의 필드 매핑을 보여 주는 이미지."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - PSC 및 파트너 센터 사용자 역할 할당

맨 위(PSC) 스크린샷의 일치하는 번호가 매겨진 원을 아래의 파트너 센터 스크린샷과 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 파트너 센터 일치하는 필드 또는 영역이 없음을 나타냅니다.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="PSC(파트너 판매 연결) 역할 할당 보기와 파트너 센터 역할 할당 보기 간의 필드 매핑을 보여 지는 이미지" lightbox="images/pscmigration/roles-expanded.png":::

**특별 고려 사항:**

- PSC 관리자에 해당하는 역할은 파트너 센터 계정 관리자 역할입니다.
- 공동 판매 거래 관리에 대한 파트너 센터 역할은 하나뿐입니다. 이 역할은 조회 관리자 역할입니다.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - PSC 및 파트너 센터 알림

맨 위(PSC) 스크린샷의 일치하는 번호가 매겨진 원을 아래의 파트너 센터 스크린샷과 비교합니다. 일치하는 숫자는 파트너 센터 PSC 관련 기능 또는 특성을 찾을 수 있는 위치를 표시합니다. 빨간색 원은 파트너 센터 일치하는 필드 또는 영역이 없음을 나타냅니다.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="PSC(Partner Sales Connect) 알림과 파트너 센터 알림 보기 간의 매핑을 보여주는 이미지"  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC에서 파트너 센터 이동 - 질문과 대답

다음 섹션에서는 마이그레이션에 대한 질문과 대답을 자주 합니다.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - 파트너 센터 액세스할 수 없는 경우 어떻게 해야 합니까?

"액세스 권한 없음" 페이지에 나열된 관리자에게 문의하여 역할을 할당받을 수 있습니다. 조회 섹션에서 읽기 및 쓰기 권한에 대한 조회 [관리자](permissions-overview.md#manage-referrals) 역할이 필요합니다. 비즈니스 프로필만 관리하는 경우 파트너 센터에서 비즈니스 프로필 관리자 역할이 필요합니다.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="파트너 센터 액세스 없음 환경을 보여주는 이미지.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - 파트너 센터 조회 섹션에 대한 액세스 권한을 부여할 수 있는 사람은 누구인가요?

[계정 관리자는](permissions-overview.md#manage-mpn-membership-and-your-company) 조회 탭에 대한 액세스 권한을 부여할 수 있습니다. 계정 관리자를 찾으려면 파트너 센터 [대시보드의](https://partner.microsoft.com/dashboard)오른쪽 위에 있는 기어 아이콘에서 **계정 설정을** 선택합니다. 그런 다음, 두 번째 수준의 왼쪽 탐색 모음에서 **사용자 관리를** 선택합니다. 사용자 목록 맨 위에서 **필터** 드롭다운 메뉴를 선택하고 옵션을 **계정 관리자** 로 변경합니다. 페이지에는 해당 이메일 주소가 있는 모든 계정 관리자가 표시됩니다. 그 중 한에게 작업 계정에 대한 조회 관리자 역할을 할당하도록 요청합니다.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - 계정에 대해 +새 거래 단추가 회색으로 표시됩니다. 거래 만들기를 시작하려면 어떻게 해야 합니까?

파트너 센터에서 사용 하는 MPN 조직에 연결 된 공동 판매 준비 솔루션이 없는 경우에만이 문제가 발생 합니다. PDM에 문의 하 여 해결 된 솔루션의 MPN ID를 확인 하거나 문제를 언급 하는 지원 티켓을 만드세요. "새 거래 단추는 PSC 마이그레이션 후 회색으로 표시 됩니다."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-PSC와 같은 조직의 특정 사용자에 게 거래를 할당할 수 있나요?

팀 멤버를 특정 거래에 할당할 수 있습니다. 다른 조회 관리자가 해당 거래를 보거나 동작 하는 것을 차단 하지 않습니다.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-내게 할당 된 모든 거래의 뷰가 있나요?

사용자 수준 탭 인 즐겨찾기 기능을 사용할 수 있습니다. 자신에 게 할당 된 모든 거래를 즐겨찾기로 표시 하 여 거래에 빠르게 액세스할 수 있습니다.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-거래에 대 한 읽기 전용 보기가 있나요?

아니요, 조회 섹션에는 거래에 대 한 읽기 전용 보기가 없습니다. 모든 조회 관리자는 모든 거래에 대해 모든 읽기 및 쓰기 권한을 갖습니다.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-성공으로 표시 한 후에 어떻게 등록할 수 있나요?

이러한 조건이 아래 조건을 충족 하는 경우 [등록](./register-deals.md)을 시작 하는 팝업이 표시 됩니다.

- 거래에 연결 된 동기 솔루션이 있습니다.
- Microsoft 판매자는 거래에 참여 하거나 거래에 초대 합니다.
- Microsoft 카드는 파트너 센터의 수락 또는 성공 상태에 있습니다.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-[거래 등록] 섹션에서 "+ 새 거래 등록" 단추를 선택 하면 오류 메시지가 표시 됩니다. 내 거래를 등록 하려면 어떻게 해야 하나요?

**+ 새 거래 등록** 단추는 ISV connect 프로그램에 등록 되어 있는 파트너가 파트너 센터에서 해당 하는 공동 판매 기회를 갖지 않도록 등록 하는 경우에만 사용 됩니다. 공동 판매 기회를 사용 하 여 거래를 등록 하는 경우에는 거래가 성공으로 표시 되 고 등록을 위한 조건을 충족 하는 경우 팝업이 표시 됩니다.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-고객 조직을 필수로 추가 하 고 있습니까?

예, [고객 조직](./manage-co-sell-opportunities.md#select-your-customer) 추가는 파트너 센터에서 필수입니다. 먼저 고객이 위치한 위치를 검색 합니다. 사용자의 세부 정보를 기반으로 합니다. 정확한 빌드 이름을 포함 하거나 도시 세부 정보를 제공할 수 있습니다. 조직 검색은 사용자가 입력 한 이름과 일치 하는 모든 법률 엔터티를 인출 하므로 주소 정보를 입력할 필요가 없습니다. 모든 세부 정보는 선택한 조직에 따라 자동으로 채워집니다.

### <a name="10---are-customer-contact-details-mandatory"></a>10-고객 연락처 세부 정보는 필수 인가요?

만들고 있는 [거래 유형에](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) 따라 달라 집니다. 파이프라인을 공유 하 고 Microsoft 판매 조직의 도움을 요구 하지 않는 경우 고객 연락처 세부 정보를 제공 하지 않도록 선택할 수 있습니다. Microsoft 판매자의 도움을 받을 수 있는 공동 판매 인 경우 고객 연락처 세부 정보를 제공 해야 합니다. 파트너 센터에서 공동 판매 요청을 만들기 전에 고객 으로부터 명시적 동의를 받아야 합니다.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-거래에 추가할 수 있는 솔루션은 몇 개입니까?

최대 50 솔루션 (PSC의 ' 제품 '과 유사)을 거래에 추가할 수 있습니다. PSC와 달리 공동 판매 적격 솔루션, Microsoft 자사 Sku 및 기타 타사 공동 판매 솔루션의 솔루션을 혼합할 수 있습니다. 파트너 센터에서 선택 하거나 사용할 수 있는 거래 역할이 없습니다. Microsoft Sku의 경우 거래에 추가 된 각 SKU에 대 한 수량 및 가격을 선택적으로 추가할 수 있습니다.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-거래를 만든 후 Microsoft 판매자 세부 정보를 어떻게 알 수 있나요?

Microsoft 판매자는 Microsoft 쪽에서 관련 판매자 가상 사용자와 거래 하는 과정을 만드는 동안 명시 된 정확한 도움말 요구 사항을 충족 하는 경우에만 할당 됩니다. 할당 후에도 Microsoft 판매자는 공동 판매 초대를 수락 하거나 거부 하는 옵션을 사용할 수 있습니다. 판매자가 공동 판매 초대를 수락 하는 경우에만 Microsoft 판매자 연락처 세부 정보를 사용 하 여 해당 거래를 업데이트 합니다. Microsoft 판매자에 대 한 SLA는 14 일입니다. 파트너가 만료 된 상태로 전환 되기 전에 처리 해야 하는 SLA와 동일 합니다.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-기회 ID는 어디서 찾을 수 있나요?

PSC의 기회 ID는 파트너 센터의 거래 ID와 동일 합니다. 거래를 열 때 거래 이름 옆의 거래 ID를 찾을 수 있습니다.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14-PDM에서 파트너 센터에 액세스 하는 방법

파트너 센터는 PSC와는 달리 사용자의 사용자가 직접 액세스할 수 없습니다. 이 기능을 사용 하도록 설정 하는 여러 옵션이 있습니다. 이러한 기능은 아래에 설명 되어 있습니다.

- OCP 정보-사용자가 관련 된 거래 및 진행 상황을 확인 하는 경우에는 단일 상업용 파트너 (OCP) Insights 포털을 사용 하 여 조직 보기를 가져올 수 있습니다. 이는 내부 도구 이며,이 도구는 사용 가능한 경우에만 사용할 수 있습니다. 사용자의 회사 사용자에 게는 OCP 정보를 사용할 수 없습니다.
- 파트너 센터의 게스트 사용자- @microsoft.com 거래 센터에서 PDM 계정을 게스트 사용자로 추가 하 고 조회를 보고 작업을 수행할 수 있도록 해당 사용자에 게 조회 관리자 역할을 할당할 수 있습니다.
- 테 넌 트에 [새 사용자](./create-user-accounts-and-set-permissions.md#add-a-new-user) 만들기-사용자의 테 넌 트에 새 사용자를 만들고 해당 세부 정보를 PDM과 공유 하 여 계정의 다른 참조 사용자와 비슷한 조회를 보고 작업할 수 있습니다.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>PSC의 계정이 유효한 MPN와 연결 되지 않은 경우 올바른 MPN ID 찾기

여기에 있는 경우 ' PSC 잘못 된 MPN ID 연결 문제 '를 언급 하는에 대 한 배너를 확인 했으므로 올바른 위치에 있습니다. 다음 이유로 인해 계정이 잘못 된 MPN ID에 연결 되었을 수 있습니다.

- 회사에 파트너 센터 계정이 없습니다.
- 사용자의 계정 ID를 파트너 센터 계정 (MPN ID)에 연결 하는 내부 시스템에서 계정 MPN ID를 입력 하는 동안 PDM에서 실수를 했습니다.
- 회사에서 파트너 구성원 센터 (PMC)에서 파트너 센터로의 마이그레이션을 완료 하지 못했습니다.

먼저 아래 단계에 따라 올바른 MPN ID를 찾습니다.

- 파트너 센터 계정에 로그인 합니다.
- [계정 설정 설명서](./partner-center-account-setup.md#locate-your-mpn-id) 에 제공 된 지침을 사용 하 여 MPN ID를 찾습니다.

다음은 파트너 센터 MPN ID를 찾을 수 있는 정확한 위치를 보여 주는 스크린샷입니다.

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="파트너가 MPN ID를 찾을 수 있는 계정 설정을 보여 주는 이미지입니다."  lightbox="images/pscmigration/findingMPNID.png":::

다음으로,

- PDM이 있는 경우 파트너 센터 계정의 올바른 MPN ID로 수정 된 MPN ID를 가져오도록 요청 하세요.
- PDM이 없으면 psc 배너에 표시 된 PSC 계정 정보와 파트너 센터 계정에서 올바른 MPN ID를 모두 사용 하 여 PSC 배너에 지정 된 주소로 전자 메일을 보냅니다.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>파트너 센터에서 거래를 만들고 관리 하는 데 도움이 되는 리소스

공동 판매 도움말 항목을 아직 읽지 않은 경우 다음 리소스는 파트너 센터에서 거래를 관리 하는 데 도움이 됩니다.

|**수행할 작업**   |**이 글 읽기**   |
|-----------------------|:-----------------------|
|공동 판매 기회 페이지에서 탭 및 탐색 이해|[공동 판매 섹션 탐색](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|D&B 목록에서 고객 조직 선택 |[고객 선택](./manage-co-sell-opportunities.md#select-your-customer)|
|거래 정보 섹션에서 필드 수정|[거래 정보](./manage-co-sell-opportunities.md#deal-details)|
|팀 멤버를 거래 팀에 추가|[직원 추가](./manage-co-sell-opportunities.md#add-team-members)|
|공동 판매 거래에 대응|[공동 판매 거래 관리](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|파트너 센터에서 승리한 거래 등록 |[새 거래 등록](./register-deals.md)
|조회 정보를 얻고 조회를 수행 하는 방법 알아보기 |[참조 인사이트](./referral-insights.md)
|비즈니스 프로필 만들기 및 관리|[비즈니스 프로필 관리](./create-a-marketing-profile.md)
|비즈니스 프로필에 대 한 잠재 고객 관리 |[잠재 고객 관리](./manage-leads.md)|

## <a name="next-steps"></a>다음 단계


- 파트너 [판매 파트너 센터 통합 문서에 연결](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -파트너 센터 및 파트너 판매 연결을 통해 파트너의 판매 프로세스 및 역할을 새 판매 프로세스와 맞춥니다.
- [파트너 센터 공동 판매 운영 가이드](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -파트너 센터를 통해 운영 모델을 식별 하 여 잠재 고객 또는 공동 판매 기회를 관리 하 고 거래를 등록 하는 지침을 제공 합니다.
- [조회 관리 데크](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -파트너 센터를 통해 잠재 고객과 공동 판매 기회를 관리 하는 단계별 지침을 시각화 합니다.
- [상업적 marketplace에서 게시 및 관리](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -상업적 Marketplace에서 파트너 센터를 통해 제품을 만들고, 관리 하 고, 게시 하는 단계별 지침을 제공 합니다.