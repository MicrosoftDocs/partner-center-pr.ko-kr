---
title: 파트너 센터에 액세스하기 위해 회사 계정 연결
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 회사를 파트너 센터 계정에 연결하는 회사 계정을 만듭니다. 이렇게 하면 회사 직원이 파트너 센터에 액세스할 수 있습니다.
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: 회사 계정, 이메일, 테넌트, Azure 테넌트, 계정 만들기, 도메인 이름
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: e46be80cb39233e7632a97fd511232d5ff762499
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394213"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>회사를 파트너 센터 계정에 연결하는 회사 계정 만들기

**적용 대상**

- 파트너 센터

**적절한 역할**

- 글로벌 관리자
- 사용자 관리 담당자

## <a name="why-you-need-a-work-account"></a>회사 계정이 필요한 이유

Microsoft에서는 회사 계정을 새 파트너 센터 계정에 연결하도록 요구하고 있습니다. 이 링크를 통해 계정 사용자는 회사 계정 사용자 이름과 암호를 사용하여 파트너 센터에 로그인할 수 있습니다.

## <a name="the-work-account-email-address"></a>회사 계정 이메일 주소

회사 계정이나 업무용 메일은 회사에서 제공하는 이메일 주소입니다. 회사 계정 이메일은 대해 `you@yourcompany.com` 형식입니다. Hotmail, Gmail 또는 Yahoo의 개인 이메일 주소는 업무용 메일이 아니며 파트너 센터 계정에 사용할 수 없습니다.

유효한 업무용 메일 주소가 여러 개 있는 경우 지역 부서가 아닌 본사에 연결된 메일 주소를 사용합니다. 예를 들어 `contoso.uk` 주소가 아닌 `contoso.com` 이메일을 사용합니다.

> [!NOTE]  
> 기존 회사 계정을 사용하기로 결정하기 전에 계정의 사용자 중 파트너 센터에서 작업해야 하는 인원이 몇 명인지 생각해 보세요. 파트너 센터에서 작업할 필요가 없는 사용자가 계정에 포함된 경우 파트너 센터에서 작업해야 하는 사용자만을 위한 새 계정을 만드는 방안을 고려해 볼 수 있습니다.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>회사 계정이 있는지 확실하지 않은가요?

회사 계정이 있는지 확실하지 않은 경우 다음 단계에 따라 확인할 수 있습니다. Microsoft Azure 또는 Office 365에 대한 활성 구독이 있는 경우 회사 계정이 이미 있는 것입니다.

1. [Azure Portal](https://portal.azure.com)에 로그인합니다.

2. 메뉴에서 Azure Active Directory를 선택하고 도메인 이름을 선택합니다.

3. 이미 회사 계정이 있는 경우 도메인 이름이 나열됩니다.

회사 계정이 아직 없는 경우 등록 과정에서 회사 계정을 만들 수 있습니다.

아래 다이어그램에서는 몇 가지 일반적인 시나리오에 대한 단계를 제공합니다.

- 회사 계정이 있는지 확인
- 회사 계정에 로그인하는 방법 확인
- 새 회사 계정을 만들어야 하는지 확인

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="회사 계정이 있나요, 아니면 회사 계정을 만들어야 하나요?":::

Azure AD에서 도메인 추가에 대한 자세한 내용은 [Azure AD에서 도메인 추가 또는 연결](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)을 참조하세요.

## <a name="about-microsoft-azure"></a>Microsoft Azure 정보

Microsoft Azure는 Microsoft에서 관리하는 글로벌 데이터 센터 네트워크에서 애플리케이션을 빌드, 구축 및 관리하는 데 사용할 수 있는 퍼블릭 클라우드 플랫폼입니다. 회사에서는 Azure를 사용하여 실제 컴퓨터 대신 가상 기능 또는 서비스를 통해 가상 IT 인프라를 구축할 수 있습니다.

Azure 구독을 구입한다는 것은 근본적으로 Azure 퍼블릭 클라우드 내에 안전한 전용 공간을 임대한다는 의미입니다. 회사의 물리적 비즈니스를 수용하기 위해 사무용 건물의 한 층을 임대하는 것과 크게 다르지 않습니다. 사무용 건물의 소유자 입장에서 볼 때 회사는 임차인입니다.

어떤 회사에서 Azure, Microsoft Intune, Office 365 등의 Microsoft 클라우드 서비스를 구독하면 Azure 퍼블릭 클라우드에 그 회사만을 위한 격리된 전용 가상 공간이 생성되는데, 이것이 바로 Azure 회사 계정입니다.

회사 계정은 Azure AD 사용자 및 사용자에 대한 정보(암호, 프로필 데이터, 권한 등)를 호스팅합니다. 또한 회사 계정에는 그룹, 애플리케이션, 회사 및 보안에 관련된 기타 정보가 포함되어 있습니다.
