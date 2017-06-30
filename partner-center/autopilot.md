---
title: "제로 터치 배포 프로필을 추가하여 Windows Autopilot으로 간단하게 디바이스 설치 | 파트너 센터"
description: "파트너 센터에서 제로 터치 배포 프로필을 추가하여 Windows Autopilot으로 간단하게 디바이스 설치"
author: KPacquer
keywords: "autopilot, windows autopilot, microsoft autopilot, 제로 터치, 제로 터치 배포, oobe, 로그인 화면"
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: c51d9204b352b548a4095e96944aacdbcde97fa2
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/19/2017
---
# <a name="add-a-zero-touch-deployment-profile-to-simplify-device-setup-with-windows-autopilot"></a>제로 터치 배포 프로필을 추가하여 Windows Autopilot으로 간단하게 디바이스 설치

Windows Autopilot은 몇 단계만 거치면 첫 번째 부팅에서 새 Windows 10 Pro 디바이스의 설치를 간소화하고 보호할 수 있습니다. 

## <a name="features"></a>기능

*  디바이스를 설치하는 최종 사용자에 대해 **로컬 관리자 권한 해제**
*  **조직의 로그인 페이지 표시**. 조직에서는 디바이스를 회사 디바이스로 추가하고 Azure Active Directory에 가입하는 로그온 페이지를 미리 정의할 수 있습니다.
*  OOBE가 완료된 후 Microsoft Intune 같은 **MDM에 디바이스 등록**.
*  꼭 필요한 단계와 의사 결정 항목만 사용하도록 ZTD(제로 터치 배포) 프로필을 사용하여 **OOBE(첫 실행 경험) 간소화**. 

## <a name="requirements"></a>요구 사항

*  Windows 10 Pro 크리에이터스 업데이트(1703 이상)가 미리 설치된 디바이스
*  하드웨어 해시로 알려진 디바이스 식별자(128 HWH 또는 4k HWH). 일반적으로 OEM에서 제공합니다. 식별자를 사용하여 파트너 센터에서 조직 프로필을 할당할 것입니다.
*  디바이스가 인터넷에 액세스할 수 있어야 합니다. 디바이스를 연결할 수 없는 경우 기본 Windows OOBE(첫 실행 경험) 화면이 표시됩니다.
*  디바이스를 MDM에 등록하려면 Azure Active Directory Premium이 필요합니다.

## <a name="add-organization-login-pages-to-oobe"></a>OOBE에 조직 로그인 페이지 추가

조직 관련 페이지를 추가하려면 디바이스를 조직의 [Azure AD 디렉터리](https://go.microsoft.com/fwlink/?linkid=848958)에 추가하고 로그인 페이지를 만듭니다.


## <a name="remove--windows-pages-from-oobe-with-a-zero-touch-deployment-ztd-profile"></a>ZTD(제로 터치 배포) 프로필을 사용하여 OOBE에서 Windows 페이지 제거

### <a name="examples-of-settings-in-a-ztd-profile"></a>ZTD 프로필의 설정 예
*  설치 시 개인 정보 설정 건너뛰기
*  설치 시 로컬 관리자 계정 비활성화
*  설치 시 자동으로 페이지 건너뛰기
   *  자동으로 회사 또는 학교 설치 선택
   *  Cortana, OneDrive 및 OEM 등록 설정 페이지 건너뛰기

### <a name="add-devices-and-apply-a-profile"></a>디바이스를 추가하고 프로필 적용

파트너 센터에서 ZTD 프로필을 만들어 디바이스 목록에 적용할 수 있습니다.

디바이스를 구성하려면 디바이스 목록을 파트너 센터에 업로드하고, 해당 디바이스에 적용되는 프로필을 만들어서 적용합니다.

1.  디바이스 목록을 파트너 센터에 추가합니다. (영업 에이전트와 관리자 에이전트는 디바이스 목록을 파트너 센터에 추가할 수 있는 권한을 갖습니다.)

    a.  새 디바이스를 보여주는 .csv 파일을 OEM에 요청합니다. 이 파일에는 일련 번호, 제품 ID, OEM Activation 3.0 도구에서 생성된 디바이스 식별자가 포함되어 있습니다. 

    b.  파트너 센터 대시보드에서 **고객** > select the customer that’s receiving the devices > **장치 > 장치 추가**로 이동합니다.

    c.  디바이스의 일괄 처리 이름을 지정합니다(예: “Contoso 영업 부서 PC – 2017년 4월 주문”). 

    d.  **찾아보기** > 장치 정보 파일 선택 > **유효성 검사**를 클릭합니다.

2.  디바이스에 적용할 수 있는 프로필을 만듭니다. (오직 관리자 에이전트만이 파트너 센터에서 프로필을 만들고 적용할 수 있습니다.)

    a.  **장치**에서 **새 프로필 추가**를 클릭합니다.

    b.  프로필 이름을 지정합니다(예: “Contoso 데스크톱 프로필 – 모든 OOBE 건너뛰기”).

    c.  OOBE 설정을 구성합니다. 예를 들어 **Skip Express Settings in setup**을 선택합니다.

    d.  **제출**을 클릭합니다.

3.  프로필을 적용합니다.

    a.  **장치**의 **장치 할당 및 삭제** 창에서 구성할 디바이스를 선택합니다. 일괄 처리 전체를 선택하려면 일괄 처리 이름(예: “Contoso 영업 부서 PC – 2017년 3월 주문”) 옆에 있는 확인란을 클릭합니다.

    b.  **프로필 적용**을 클릭하고 프로필(예: "Contoso 데스크톱 프로필 - 모든 OOBE 건너뛰기")을 선택합니다. 디바이스의 프로필 열에 프로필이 표시됩니다.

4.  선택 사항: 프로필이 정상적으로 작동하는지 테스트합니다.

    a.  디바이스를 네트워크에 연결하고 켭니다.

    b.  적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.

    c.  디바이스를 사용할 새 사용자를 위해 OOBE 환경을 완료한 다음 디바이스를 공장 기본 설정으로 초기화합니다.


## <a name="to-update-or-delete-a-profile"></a>프로필을 업데이트 또는 삭제하려면 

디바이스에 프로필을 할당했으면 디바이스를 업데이트할 수 있으며, 심지어 고객에게 디바이스를 건넨 후에도 업데이트할 수 있습니다. 디바이스가 인터넷에 연결되면 OOBE 프로세스가 진행되는 동안 최신 버전의 프로필이 디바이스로 다운로드됩니다. 고객이 디바이스를 공장 기본 설정으로 복원하는 경우 디바이스가 최신 업데이트를 다시 프로필로 다운로드합니다. 

###<a name="you-can-remove-a-profile-from-a-device"></a>디바이스에서 프로필을 제거할 수 있습니다.
1. 프로필을 제거할 디바이스(또는 디바이스의 일괄 처리)를 선택합니다. 

2. **디바이스 할당 및 삭제** 창에서 **프로필 제거**를 선택합니다.

3. 제거하려는 프로필로 이동하여 해당 프로필을 삭제합니다. 모든 디바이스에서 해당 프로필이 삭제됩니다.


**장치**에서 해당 프로필을 선택합니다. 여기서 기존 설정을 수정할 수 있습니다.

