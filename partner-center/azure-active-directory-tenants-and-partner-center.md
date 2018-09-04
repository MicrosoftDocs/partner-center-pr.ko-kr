---
title: 회사 계정 및 파트너 센터 | 파트너 센터
description: 파트너 센터 계정을 만들려면 회사 계정이 있어야 합니다.
author: labrenne
Keywords: work account, email, tenant, Azure tenant, create account, domain name
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 2ebc5490d724b49836b0051802038c4ba4c86e20
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876083"
---
# <a name="your-company-work-account-and-the-partner-dashboard"></a>조직의 회사 계정 및 파트너 대시보드  

**적용 대상**

-  파트너 센터

## <a name="why-you-need-a-work-account"></a>회사 계정이 필요한 이유

계정 사용자가 자신의 회사 계정 사용자 이름 및 암호를 사용하여 파트너 대시보드에 로그인할 수 있도록 조직의 회사 계정을 새 파트너 대시보드에 연결해야 합니다.

조직에 이미 회사 계정이 있는 경우 이를 파트너 대시보드 계정에 연결할 수 있습니다. 

>**참고** 기존 회사 계정을 사용하기로 결정하기 전에 계정의 사용자 중 파트너 대시보드에서 작업해야 하는 인원이 몇 명인지 생각해 보세요. 파트너 대시보드에서 작업할 필요가 없는 사용자가 계정에 포함된 경우 파트너 대시보드에서 작업해야 하는 사용자만을 위한 새 계정을 만드는 방안을 고려해 볼 수 있습니다.

회사에 아직 회사 계정이 없는 경우 등록 과정에서 테넌트를 만들 수 있습니다. 

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>회사에 회사 계정이 있는지 확실하지 않은가요?

회사에 회사 계정이 있는지 확실하지 않은 경우, 다음 단계에 따라 확인할 수 있습니다. Microsoft Azure 또는 Office 365의 활성 구독이 있는 회사는 이미 회사 계정을 갖고 있습니다.
1.  https://ms.portal.azure.com에서 Azure 포털에 로그인합니다.
2.  메뉴에서 Azure Active Directory를 선택한 다음 도메인 이름을 선택합니다.
3.  이미 회사 계정이 있는 경우 도메인 이름이 나열됩니다.

## <a name="using-an-existing-work-account"></a>기존 회사 계정 사용

기존 회사 계정을 사용하고 싶지만 로그인하는 데 문제가 있는 경우 아래 다이어그램에서 현재 상황과 가장 잘 맞는 시나리오를 찾아 권장 단계를 수행합니다. 

![회사 계정이 있나요 아니면 새로 만들어야 하나요?](images/onboardingAADFlow.png)

Azure AD에서 도메인 추가에 대한 자세한 내용은 [Azure Active Directory에 사용자 지정 도메인 이름 추가](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)를 참조하세요.

# <a name="about-microsoft-azure"></a>Microsoft Azure에 대한 정보

Microsoft Azure는 Microsoft에서 관리하는 전체 데이터 센터 네트워크에서 응용 프로그램을 빌드, 구축 및 관리하는 데 사용할 수 있는 공개 클라우드 플랫폼입니다. 회사에서는 Azure를 사용하여 실제 컴퓨터 대신 가상 기능 또는 서비스를 통해 가상 IT 인프라를 구축할 수 있습니다. 

Azure 구독을 구입한다는 것은 근본적으로 Azure 공용 클라우드 내에 안전한 전용 공간을 임대한다는 의미입니다. 회사의 물리적 비즈니스를 수용하기 위해 사무용 건물의 한 층을 임대하는 것과 크게 다르지 않습니다. 사무용 건물의 소유자 입장에서 볼 때 회사는 임차인입니다. 

어떤 회사에서 Azure, Microsoft Intune, Office 365 같은 Microsoft 클라우드 서비스를 구독하면 Azure 공용 클라우드에 그 회사만을 위해 격리된 전용 가상 공간이 생성되는데, 이것이 바로 Azure 회사 계정입니다. 

회사 계정은 Azure AD 사용자 및 사용자에 대한 정보(암호, 프로필 데이터, 권한 등)를 호스팅합니다. 또한 회사 계정에는 그룹, 응용 프로그램, 회사 및 보안에 관련된 기타 정보가 포함되어 있습니다. 
