---
title: Azure AD 서비스 사용자
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD 테넌트에 서비스 사용자를 추가하는 방법을 알아봅니다. 이렇게 하면 파트너 센터에서 Azure AD 애플리케이션(서비스 사용자)을 추가하는 것을 의미합니다.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure 플랜, 서비스 사용자, Azure AD 애플리케이션
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 76a65cd824c7c1af5242bea3af6069a466c9fa1c
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2020
ms.locfileid: "84426002"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>파트너 센터에서 Azure AD 애플리케이션(서비스 사용자) 추가

파트너 센터의 상용 마켓플레이스 프로그램에서 이제 Azure AD 애플리케이션(서비스 사용자)을 파트너 센터 계정의 사용자로 추가할 수 있습니다. (이전에 Cloud 파트너 포털 또는 CPP 계정에서 이 작업을 수행할 수 있었습니다. 파트너 센터로 마이그레이션되었으므로 CPP 계정은 읽기 전용입니다.) 서비스 사용자는 Azure AD 애플리케이션과 동의어입니다.

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD 애플리케이션(서비스 사용자) 추가

1. 파트너 센터 대시보드에서 **설정**을 선택한 다음, **개발자 설정**을 선택합니다.

2. **사용자**를 선택한 다음, **Azure AD 애플리케이션 추가**를 선택합니다.

3. 기존 Azure AD 애플리케이션을 선택하거나 새로 만듭니다.

4. 새 Azure AD 애플리케이션을 만드는 경우 다음 정보를 포함시킵니다.  

   - **회신 URL**: 사용자가 Azure AD 애플리케이션을 사용하기 위해 로그인할 수 있는 URL입니다.

   - **앱 ID URI**: Azure AD에 Single Sign-On 요청을 보낼 때 제공되는 Azure AD 애플리케이션의 논리적 식별자입니다.

   - **보안 역할**: **관리자** 역할(CPP의 '소유자' 역할과 동일) 및 **개발자** 역할(CPP의 '기여자' 역할과 동일)은 파트너 센터의 상업용 마켓플레이스 프로그램에 적용되며, 이 Azure AD 애플리케이션과 연결될 수 있습니다.  
