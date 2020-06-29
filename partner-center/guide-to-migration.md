---
title: PMC에서 파트너 센터로 마이그레이션
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 회사를 PMC(Partner Membership Center)에서 파트너 센터로 마이그레이션하는 방법에 대해 알아봅니다.
author: LauraBrenner
ms.author: labrenne
keywords: PMC, 마이그레이션, 파트너 센터로 이동
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 773466a1c7bfb8a091be11f8e825dae6cc90b765
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679090"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>PMC에서 파트너 센터로 마이그레이션에 대한 가이드

**적절한 역할**

- 글로벌 관리자

partner.microsoft.com의 Microsoft 파트너 웹 사이트는 파트너를 위한 통합 디지털 환경입니다. 파트너 웹 사이트에서 기회를 살펴보고 회사에서 Microsoft와 앱 및 서비스를 빌드하고 판매하는 데 도움이 되는 안내 환경에 참여할 수 있습니다. Microsoft 파트너 네트워크의 구성원은 파트너 웹 사이트에서 사용 가능한 대시보드 링크를 통해 Microsoft와의 관계를 관리하고 프로그램과 제품에 가입할 수 있는 파트너 센터에 로그인할 수 있습니다.

PMC(Partner Membership Center)는 서비스 해제 중입니다. 귀사는 Microsoft 파트너 네트워크 멤버십 관리를 파트너 센터로 전환하도록 초대되셨습니다. 이 가이드를 통해 PMC에서 파트너 센터로 이동할 때 예상되는 결과에 대해 알 수 있습니다.

>[!NOTE]
>회사에 계정이나 위치가 둘 이상 있는 경우에도 파트너 센터로 이동은 (첫 번째) 계정을 파트너 센터로 이동하는 것으로 시작합니다.

## <a name="get-started"></a>시작

PMC에서 이동이 시작됩니다. 글로벌 관리자가 이동을 시작하라는 초대를 받게 됩니다.

### <a name="prepare-in-pmc"></a>PMC에서 준비할 사항

- 회사 정보 확인
- 주 프로그램 담당자 확인
- 비즈니스 확인
- 승인된 사용자 업데이트

### <a name="when-youre-ready"></a>준비 후 진행할 사항

초대에서 **시작하기**를 선택합니다. 파트너 센터 로그인 페이지로 이동됩니다.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="시작":::

## <a name="start-with-your-work-email"></a>업무용 메일로 시작

회사에 업무용 이메일과 AAD 테넌트가 없는 경우 파트너 센터 로그인 프로세스 중 업무용 이메일과 AAD 테넌트를 설정하도록 도와드릴 수 있습니다. 개인 계정과 같은 업무용 메일이 아닌 이메일 계정으로 로그인하려고 하면 AAD 테넌트와 업무용 메일을 설정할 수 있게 회사에 대한 정보를 제공하라는 메시지가 나타납니다. 이러한 회사 정보는 파트너 센터에서 계정 등록을 마무리하는 데 사용되므로 정보가 정확한지 확인합니다.

>[!NOTE]
>중국의 파트너이며 Microsoft 파트너 네트워크와 CSP(클라우드 솔루션 공급자) 프로그램 모두에 등록되어 있는 경우 각 계정에 대해 별도의 테넌트가 제공됩니다. 클라우드 솔루션 공급자 프로그램 계정은 국가 클라우드에서 관리되고 Microsoft 파트너 네트워크 계정은 글로벌 클라우드에서 관리됩니다. 두 계정을 연결할 수 없습니다.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="회사에 대한 정보 제공":::

정보를 확인하거나 업데이트한 후 **동의 후 계속**을 선택합니다.
이 페이지의 계약조건은 회사가 PMC에서 이미 서명한 계약과 **똑같습니다**.  
이 단계는 Azure AD 테넌트의 생성을 시작하고 회사 계정이 제공됩니다.

**동의 후 계속**을 선택하면 다음 작업도 수행됩니다.

- 계정이 모든 해당 위치와 함께 파트너 센터로 마이그레이션됩니다.

- PMC에서 구매한 역량이나 MAP가 마이그레이션됩니다.

- PMC에 있는 모든 마케팅 리소스, 제품 및 프로그램(MAP, 실버, 골드)을 마이그레이션합니다.

## <a name="invite-employees-to-join-you"></a>참가하도록 직원 초대

새 Azure AD 테넌트가 생성되면 파트너 센터에 로그인하도록 직원들을 초대할 수 있습니다.

:::image type="content" source="images/migration/invite.png" alt-text="직원 초대":::

기존 AAD 테넌트로 로그인하면 직원이 귀사와 함께 이동합니다. 이 경우 파트너 센터에서 수행할 수 있는 작업을 결정하는 역할을 직원에게 할당합니다. 

>[!NOTE] 
>파트너 센터의 역할은 PMC의 역할과 다릅니다. 자세한 내용은 [PMC에서 파트너 센터로 이동](move-pmc-pc-map.md)을 참조하세요.

## <a name="verify-your-domain-and-become-a-global-admin"></a>도메인을 확인하고 글로벌 관리자가 됩니다.  

AAD 테넌트가 새로 생성된 경우 아무에게도 글로벌 관리자의 역할이 할당되지 않습니다. 글로벌 관리자가 되려면 도메인 소유권을 확인해야 합니다. 이를 위해 도메인 관리자가 필요할 수 있습니다.

이미 구매한 제품을 사용할 수 있지만 전역 관리자를 할당하는 단계를 완료할 때까지 새 제품을 구매할 수 없습니다.

:::image type="content" source="images/migration/takecontrol.png" alt-text="제어":::

시작하기를 선택하면 다음 화면이 나타납니다.

:::image type="content" source="images/migration/verifytxt.png" alt-text="도메인 소유권 확인":::

도메인 등록 기관은 이미 입력되어 있습니다. 도메인 소유자만 DNS 파일을 업데이트할 수 있으므로 텍스트 파일을 복사하고 DNS 레코드에 추가하여 자신이 소유자인지 확인할 수 있습니다. 업데이트가 수행되는 데 몇 분 정도 걸릴 수 있습니다. 파트너 센터에서 로그아웃했다가 다시 로그인해야 합니다. 역할이 글로벌 관리자로 변경됩니다.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>대시보드 및 파트너 센터에 대해 알아보기

대시보드를 둘러봅니다. 여기에서 멤버십을 관리하고, 조회를 위한 비즈니스 프로필을 추가하고, 클라우드 솔루션 공급자 프로그램에 등록하고, **대시보드**를 선택하여 언제든지 비즈니스에 관련된 알림과 제품을 확인할 수 있습니다. 또한 인센티브를 관리하고, 마켓플레이스에서 구매하고, 출시 서비스에 가입하는 등의 작업을 수행할 수 있습니다.  

:::image type="content" source="images/migration/fre.png" alt-text="둘러보기":::

## <a name="next-steps"></a>다음 단계

- [사용자 계정 만들기](create-user-accounts-and-set-permissions.md)

- [사용자 역할 및 권한 할당](permissions-overview.md)

- [멤버십 프로그램 관리](renew-mpn-offers.md)

- [회사의 비즈니스 프로필 만들기](create-a-marketing-profile.md)

- [추천을 통해 고객과 연결](responding-to-referrals.md)

- [PMC에서 파트너 센터로 여러 회사 마이그레이션에 대한 가이드](move-multiple-companies.md)
