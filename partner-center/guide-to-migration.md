---
title: PMC에서 파트너 센터로의 마이그레이션 가이드 | 파트너 센터
ms.topic: article
ms.date: 04/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: PMC에서 파트너 센터로 회사를 마이그레이션할 때 알아야 할 사항
author: LauraBrenner
ms.author: labrenne
keywords: PMC, 마이그레이션, 파트너 센터로 이동
ms.localizationpriority: medium
ms.openlocfilehash: a39c4114758004ff4291bc577182fd8ba469149b
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653095"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>PMC에서 파트너 센터로의 마이그레이션 가이드

Partner.microsoft.com의 Microsoft 파트너 웹 사이트는 파트너를 위한 통합 디지털 환경입니다. 파트너 웹 사이트에서 사용자의 기회를 살펴보고 회사에서 Microsoft와 앱 및 서비스를 구축 하 고 판매 하는 데 도움이 되는 안내가 제공 되는 환경을 사용할 수 있습니다. 파트너 웹 사이트에서 사용할 수 있는 대시보드 링크를 사용 하면 Microsoft 파트너 네트워크의 구성원이 Microsoft와의 관계를 관리 하는 파트너 센터에 로그인 하 고, 프로그램에 등록 하 고, 제품에 등록할 수 있습니다. 

PMC (파트너 구성원 센터)를 서비스 해제 하 고 있습니다. 회사는 Microsoft 파트너 네트워크 멤버 관리를 파트너 센터로 전환 하도록 초대 되었습니다. 이 가이드는 PMC에서 파트너 센터로 이동 하는 것 처럼 예측할 수 있는 것을 준비 합니다.

>[!Note]
>회사에 계정이 나 위치가 둘 이상 있는 경우에도 파트너 센터로 이동은 먼저 (첫 번째) 계정을 파트너 센터로 이동 하 여 시작 합니다.

## <a name="get-started"></a>시작하기

PMC에서 이동이 시작 됩니다. 전역 관리자는 이동을 시작 하 라는 초대를 받게 됩니다. 

**PMC에서 준비**
- 회사 세부 정보 확인 
- 기본 프로그램 연결 확인 
- 비즈니스 위치 확인
- 승인 된 사용자 업데이트

**준비가 되 면**

초대에서 **시작** 을 선택 합니다. 파트너 센터 로그인 페이지로 이동 됩니다.

![시작하기](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>회사 전자 메일을 사용 하 여 시작

회사에 업무용 메일 및 AAD 테 넌 트가 없는 경우 파트너 센터 로그인 프로세스 중에 설정 하는 것이 도움이 될 수 있습니다. 개인 계정과 같은 업무용 메일이 아닌 전자 메일 계정을 사용 하 여 로그인을 시도 하면 AAD 테 넌 트 및 직장 메일을 설정할 수 있도록 회사에 대 한 정보를 제공 하는 것으로 리디렉션됩니다.
이러한 회사 세부 정보는 파트너 센터에서 계정을 마무리 하는 데 사용 되므로 정확한 지 확인 합니다.

>[!Note]
>중국의 파트너 이며 Microsoft 파트너 네트워크 및 CSP (클라우드 솔루션 공급자) 프로그램 모두에 등록 되어 있는 경우 각 계정에 대해 별도의 테 넌 트가 제공 됩니다. 클라우드 솔루션 공급자 프로그램을 사용 하는 계정은 국가별 클라우드에서 관리 되 고 Microsoft 파트너 네트워크 계정은 글로벌 클라우드에서 관리 됩니다. 두 계정을 연결할 수 없습니다.

![회사에 대해 알려주세요.](images/migration/newtellusabout.png)

정보를 확인 하거나 업데이트 했으면 **동의 후 계속**을 선택 합니다.
이 페이지의 사용 약관은 회사에서 이미 PMC 로그인 한 계약과 **정확히 동일 합니다** .  
그러면 Azure AD 테 넌 트의 생성이 시작 되 고가 회사 계정으로 제공 됩니다.

**수락 및 계속을** 선택 하면 다음 작업도 수행 됩니다.

• 계정을 파트너 센터에 모든 위치와 함께 마이그레이션합니다.

• PMC에서 구매한 역량 또는 지도를 마이그레이션합니다.

• PMC에서 제공 하는 모든 혜택 (지도, 실버, 골드)을 마이그레이션합니다.

## <a name="invite-employees-to-join-you"></a>참가할 직원 초대

새 Azure AD 테 넌 트가 만들어지면 직원이 파트너 센터에 로그인 하도록 초대할 수 있습니다.

![직원 초대](images/migration/invite.png)


기존 AAD 테 넌 트를 사용 하 여 로그인 한 경우 직원은 사용자와 함께 이동 됩니다. 이 경우 파트너 센터에서 수행할 수 있는 작업을 결정 하는 직원 역할을 할당 합니다. 참고: 파트너 센터의 역할은 PMC의 역할과 다릅니다. 자세한 내용은 [PMC에서 파트너 센터로 이동을](move-pmc-pc-map.md)참조 하세요.

## <a name="verify-your-domain-and-become-a-global-admin"></a>도메인을 확인 하 고 전역 관리자가 됩니다.  

AAD 테 넌 트가 새로운 경우 전역 관리자의 역할이 할당 되지 않습니다. 전역 관리자가 되 면 도메인 소유권을 확인 해야 합니다. 이를 위해 도메인 관리자가 필요할 수 있습니다. 이미 구매한 제품을 사용할 수 있지만 전역 관리자를 가져오는 단계를 완료할 때까지 새 제품을 구매할 수 없습니다. 

![컨트롤 사용](images/migration/takecontrol.png)

시작을 선택 하면 다음 화면이 표시 됩니다.

![도메인 소유권 확인](images/migration/verifytxt.png)

도메인 등록자는 이미 입력 되어 있습니다. 도메인 소유자만 dns 파일을 업데이트할 수 있으므로, 텍스트 파일을 복사 하 여 DNS 레코드에 추가 하면 소유자 인지 확인할 수 있습니다. 업데이트가 발생 하는 데 몇 분 정도 걸릴 수 있습니다. 파트너 센터에서 로그 아웃 한 후 다시 로그인 해야 합니다. 사용자의 역할은 전역 관리자로 변경 됩니다. 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>대시보드 및 파트너 센터에 대해 알아봅니다.

대시보드 둘러보기를 살펴보겠습니다. 여기에서 구성원 자격을 관리 하 고, 조회에 대 한 비즈니스 프로필을 추가 하 고, 클라우드 솔루션 공급자 프로그램에 등록 하 고, 언제 든 지 **대시보드**를 선택 하 여 비즈니스와 관련 된 알림 및 제안을 확인할 수 있습니다. 또한 성과급을 관리 하 고, marketplace에서 구매 하 고, 시장 출시 서비스에 등록 하는 등의 작업을 수행할 수 있습니다.  

![둘러보기](images/migration/fre.png)

## <a name="next-steps"></a>다음 단계

- [사용자 계정 만들기](create-user-accounts-and-set-permissions.md)
- [사용자 역할 및 권한 할당](permissions-overview.md)
- [멤버십 프로그램 관리](renew-mpn-offers.md)
- [회사의 비즈니스 프로필 만들기](create-a-marketing-profile.md)
- [추천을 통해 고객과 연결](responding-to-referrals.md)

## <a name="see-also"></a>참고 항목

- [PMC에서 파트너 센터로 여러 회사를 마이그레이션하는 방법에 대 한 가이드](move-multiple-companies.md)
