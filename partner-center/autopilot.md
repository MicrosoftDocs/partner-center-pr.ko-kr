---
title: Windows Autopilot 프로필을 사용 하 여 디바이스의 기본 제공 환경을 사용자 지정 | 파트너 센터
description: Autopilot 프로필을 사용 하 여 디바이스의 기본 제공 경험 미리 구성 합니다.
author: maggiepuccievans
keywords: autopilot, windows autopilot, microsoft autopilot, 제로 터치 배포, oobe, 로그인 화면, 기본 제공
ms.localizationpriority: medium
ms.openlocfilehash: 70740212f433ad6eb4f2f04d63708fff436024ad
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995937"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Windows Autopilot 프로필을 사용 하 여 디바이스의 기본 제공 환경을 사용자 지정

**적용 대상**

- CSP 직접 청구서 파트너, 간접 공급자와 간접 재판매인

고객 장치를 관리 하는 경우 고객의 사용자에 대 한 기본 제공 경험 (OOBE)을 사용자 지정 해야 합니다. 고객에 게 장치를 전달 하기 전에 Windows Autopilot 프로필을 사용 하 여 새 장치를 미리 구성 하 고 이미 구매한 고객 장치에 새 프로필을 적용할 수 있습니다. 이 문서에서는 만들고 파트너 센터에서 장치에 Autopilot 프로필을 적용 하는 방법을 설명 합니다.

수 없는 경우 이미 익숙한 autopilot,이 문서의 정보를 검토:

- [Windows Autopilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 배포 참조 가이드](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>개요

파트너 센터에서 Windows Autopilot 기능을 사용 하 여 고객 장치에 적용할 사용자 지정 프로필을 만들 수 있습니다. 이 문서가 게시 시간에 다음 프로필 설정을 사용할 수 있게 합니다.

- 개인 정보 설정 건너뛰기 이 선택적 Autopilot 프로필 설정을 통해 조직은 않을 OOBE 프로세스 동안 개인 정보 설정에 대 한 요청 하지 수 있습니다.

- 장치에 로컬 관리자 계정 만들기를 사용 하지 않도록 설정 합니다. 조직은은 프로세스가 완료 되 면 장치를 설정 하는 사용자 관리자 액세스를 가져야 할지 여부를 결정할 수 있습니다.

- 회사 또는 학교에 대 한 장치를 자동으로 설정 합니다. Autopilot을 사용 하 여 등록 된 모든 장치 작업 자동으로 간주 됩니다 또는 학교 장치, 하므로 OOBE 프로세스 동안이 질문을 요청 하지 않습니다.

- Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다. Autopilot을 사용 하 여 등록 된 모든 장치는 자동으로 아웃-첫 실행 경험 (OOBE) 동안 이러한 페이지를 건너뜁니다.

- 최종 사용자 사용권 계약 (EULA) 건너뛰기 Windows 10 버전 1709부터 조직은 OOBE 프로세스 도중 EULA 페이지를 건너뛸 결정할 수 있습니다. [Windows Autopilot EULA 철회](#windows-autopilot-eula-dismissal) 아래 중요 한 정보에 대 한 Windows 설치 시 EULA 페이지 건너뛰기에 대 한 고려를 참조 하세요.

다음 프로필 및 장치 관리 권한 및 제한 사항이 적용 됩니다.

- CSP 파트너 계속 파트너의 위임 된 관리 권한을 제거한 경우에 재판매인 관계에 있는 기존 고객을 위해 Autopilot 프로필을 관리할 수 있습니다.

- 사용자 또는 다른 CSP 파트너가 추가한 고객을 위해 기존 장치를 관리할 수 있습니다.

- 고객은 비즈니스용 Microsoft 스토어 또는 Microsoft Intune 포털에 업로드 한 장치를 관리할 수 없습니다.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>만들기 및 파트너 센터에서 Autopilot 프로필 관리

파트너 센터에서 Windows Autopilot 배포 프로필을 만들 수 있으며 장치에 적용할 수 있습니다.

>[!NOTE]
>관리자 에이전트만 만들고 프로필을 적용할 수 있습니다.

### <a name="create-a-new-autopilot-profile"></a>새 Autopilot 프로필 만들기

1. 파트너 센터 메뉴에서 **고객** 을 선택 하 고 Autopilot 프로필을 만드는 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **Windows Autopilot 프로필** 에서 **새 프로필 추가**선택 합니다.

4. 프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다. 선택 합니다.  

   - 설정의 개인 정보 설정 건너뛰기

   - 설치 시 로컬 관리자 계정 비활성화
  
   - 설치 시 자동으로 페이지 건너뛰기<br>
        ( *자동으로 회사 또는 학교 설치 선택* 및 *건너뛰기 Cortana, OneDrive 및 OEM 등록 설정 페이지*포함)
  
   - 최종 사용자 사용권 계약 (EULA) 건너뛰기<br> 
       >[!IMPORTANT] 
       >[Windows Autopilot EULA 철회](#windows-autopilot-eula-dismissal) 아래 중요 한 정보에 대 한 Windows 설치 시 EULA 페이지 건너뛰기에 대 한 고려를 참조 하세요.

5. 작업을 마쳤으면 **제출**을 선택합니다.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>고객 장치에 Autopilot 프로필 적용

>[!NOTE]
>다음 지침을 이미 추가한 고객의 디바이스 파트너 센터로 자신의 장치 목록에 액세스할 수 있는지 가정 합니다. 고객의 장치를 추가 하지 않은 경우 [고객의 계정에 추가 디바이스](#add-devices-to-a-customers-account) 의 지침에 따라 한 다음 아래 단계를 따릅니다.

고객의 Autopilot 프로필을 만든 후에 고객의 장치에 적용할 수 있습니다.

1. 파트너 센터 메뉴에서 **고객** 을 선택 하 고 만든 Autopilot 프로필에 대 한 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **장치에 적용 프로필** 에서 장치나 프로필을 추가 하 고 다음 **적용 프로필**을 선택 하 고 싶은 장치 그룹을 선택 합니다. 방금 적용 프로필 **프로필** 열에 표시 됩니다.

4. 프로필 적용 됨을 성공적으로 장치를 확인 하려면 다음 단계를 수행 합니다.

    a.  네트워크에 장치를 연결 하 고 켭니다.

    b.  적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.

    c.  OOBE 프로세스를 중지 하면 새 사용자를 위한 준비를 공장 기본 설정에 디바이스를 초기화 합니다.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>고객의 장치에서 Autopilot 프로필 제거

1. 파트너 센터 메뉴에서 **고객** 을 선택 하 고 만든 Autopilot 프로필에 대 한 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **장치에 적용 프로필** 에서 프로필을 제거 하 고 선택한 다음 **프로필 제거**하려는 디바이스를 선택 합니다.

   >[!NOTE]
   >장치에서 프로필을 제거 해도 목록에서 프로필을 삭제 되지 않습니다. 프로필을 삭제 하려는 경우 [업데이트 또는 삭제 Autopilot 프로필의](#update-or-delete-an-autopilot-profile)지침을 따릅니다.

### <a name="update-or-delete-an-autopilot-profile"></a>업데이트 또는 Autopilot 프로필을 삭제 합니다.

고객이 장치에 제공한 후 기본 제공 경험을 변경 하는 경우 파트너 센터에서 프로필을 변경할 수 있습니다.

고객의 장치가 인터넷에 연결 하는 경우 OOBE 프로세스 동안 최신 프로필 버전을 다운로드 됩니다. 또한 고객이 디바이스를 공장 기본 설정, 복원 언제 든 지 장치를 다시 최신 버전을 다운로드 프로필 OOBE 프로세스 동안 합니다.

1. 파트너 센터 메뉴에서 **고객** 을 선택 하 고 Autopilot 프로필을 변경할 수를 원하는 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **Windows Autopilot 프로필** 에서 업데이트 해야 하는 프로필을 선택 합니다. 필요한 사항을 변경 하 고 **제출**를 선택 합니다.

이 프로필을 삭제 하려면 페이지의 오른쪽 위 모서리에서 **프로필 삭제** 를 선택 합니다.

### <a name="add-devices-to-a-customers-account"></a>고객의 계정에 장치를 추가 합니다.

>[!NOTE]
>영업 에이전트와 관리자 에이전트는 고객의 계정에 디바이스를 추가할 수 있습니다.

고객 장치에 사용자 지정 Autopilot 프로필을 적용 하려면, 먼저 고객의 장치 목록에 액세스할 수 있어야 합니다.

OEM 이름, 일련 번호 및 모델 조합을 사용 하려는 경우 이러한 제한 사항을 고려해 야 합니다.

- 최신 장치 (4 k 해시, 예:)에 대해서만이 튜플 작동 128b 해시 (RS2 및 이전 장치)에 대 한 지원 되지 않습니다.

- 튜플 등록 대/소문자를 구분 이므로 OEM 공급자 (하드웨어 공급자)가 제공한 파일의 데이터는 제조업체 및 모델 이름을 ***정확히*** 일치 해야 합니다.

파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따릅니다.

1. 파트너 센터 메뉴에서 **고객** 을 선택 하 고 해당 장치를 관리 하려는 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **장치에 적용 프로필** 에서 **추가 장치**를 선택 합니다.

4. 장치 목록에 대 한 이름을 입력 하 고 (.csv 파일 형식)의 고객의 목록을 파트너 센터에 업로드할 **찾아보기** 를 선택 합니다.

    >[!NOTE]
    >장치 구입이.csv 파일을 받아야 합니다. .Csv 파일을 받은 후 하지 않은 경우에 [추가 Windows Autopilot 장치](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)에 단계에 따라 직접 만들 수 있습니다.  

5. .Csv 파일을 업로드 하 고 **저장**을 선택 합니다.

.Csv 파일을 업로드 하는 동안 오류 메시지가 나타나면 파일 형식을 확인 합니다. 하드웨어 해시만 또는 OEM 이름, 일련 번호 및 모델 (순서로 열) 또는 Windows 제품 ID를 사용할 수 있습니다. 또한 장치 목록을 만드는 **추가 장치** 옆에 있는 링크에서 제공 되는 샘플.csv 파일을 사용할 수 있습니다.

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 철회

### <a name="important-information"></a>중요 한 정보

Windows Autopilot을 사용 하면 고객에 게 관리 하는 장치에서 Windows의 사용자 지정 된 설치를 구성할 수 있습니다. 고객이 이렇게 하려면 권한이 있으면 표시 안 함 하거나 일반적으로 EULA (최종 사용자 사용권 계약) 동의 화면 등 Windows를 설정할 때 사용자에 게 제시 되는 일부 설정 화면을 숨길 수 있습니다.

이 기능을 사용 함으로써 귀하는 표시 하지 않거나 숨기 고 지 또는 동의 용어 의미를 갖고 있는 충분 한 동 및 권한 부여 대신, 약관을 숨기기 고객 으로부터 사용자를 제공 하도록 고안 된 화면 (여부는 조직 또는 개별 사용자 경우에 따라 수 있음), 고객 지에 동의 하 고 수락 모든 고객에 게 적용 되는 약관 합니다. 여기에는 이 도구를 사용하여 표시하거나 숨기지 않는 경우, 사용자에게 제시되는 라이선스 약관 또는 고지에 대한 동의가 포함됩니다. 귀하의 고객이 Microsoft 또는 사용권이 허용된 배포자로부터 유효하게 소프트웨어 라이선스를 취득하지 않은 경우, 고객은 이러한 장치에서 Windows 소프트웨어를 사용할 수 없습니다.