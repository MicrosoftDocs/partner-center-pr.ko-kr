---
title: Windows Autopilot 프로필을 사용 하 여 장치의 기본 제공 환경을 사용자 지정 | 파트너 센터
description: Autopilot 프로필을 사용 하 여 장치의 기본 제공 환경을 미리 구성 합니다.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot, windows autopilot, microsoft autopilot, 제로 터치 배포, oobe, 로그인 화면, 기본 제공
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162223"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Windows Autopilot 프로필을 사용 하 여 장치의 기본 제공 환경을 사용자 지정

**적용 대상**

- CSP 직접 청구 파트너, 간접 공급자 및 간접 대리점

고객의 장치를 관리 하는 경우에 고객의 사용자에 대 한 기본 제공 환경 (OOBE) 사용자 지정 해야 합니다. 고객에 게 장치를 제공 하기 전에 Windows Autopilot 프로필을 사용 하 여 새 장치를 미리 구성할 수 있으며 고객이 이미 구입한 장치에 새 프로필을 적용할 수 있습니다. 이 문서에서는 만들고 파트너 센터에서 장치에 Autopilot 프로필을 적용 하는 방법을 설명 합니다.

아직 수행 하지 않은 Autopilot을 사용 하 여 친숙 한,이 문서의 정보를 검토:

- [Windows Autopilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 배포 참조 가이드](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>개요

파트너 센터에서 Windows Autopilot 기능을 사용 하 여 고객의 장치에 적용할 사용자 지정 프로필을 만들 수 있습니다. 이 문서는 게시 시점에 다음 프로필 설정을 사용할 수 없었습니다.

- 개인 정보 설정을 건너뜁니다. 이 선택적 Autopilot 프로필 설정은 조직을 OOBE 과정에서 개인 정보 설정에 대 한 표시를 수 있습니다.

- 장치의 로컬 관리자 계정 만들기를 사용 하지 않도록 설정 합니다. 조직에서는 프로세스가 완료 되 면 사용자 장치 설정에서 관리자 액세스할 수 있어야 하는지 여부를 결정할 수 있습니다.

- 회사 또는 학교에 대 한 장치를 자동으로 설정 합니다. Autopilot을 사용 하 여 등록 된 모든 장치 작업 자동으로 간주 됩니다 또는 OOBE 과정에서이 질문 확인 하도록 장치를 학교입니다.

- Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다. Autopilot을 사용 하 여 등록 된 모든 장치에서 기본 제공 환경 (OOBE) 프로세스 중에 자동으로 이러한 페이지를 건너뜁니다.

- 최종 사용자 사용권 계약 (EULA)을 건너뜁니다. Windows 10 버전 1709부터 조직 EULA 페이지 OOBE 프로세스 중에 표시 하지 않으려면 결정할 수 있습니다. 참조 [Windows Autopilot EULA 사건의](#windows-autopilot-eula-dismissal) 아래 Windows 중 EULA 페이지 건너뛰기에 대 한 고려해 야 할 중요 한 정보를 설정 합니다.

다음 프로필 및 장치 관리 권한 및 제한 사항이 적용 됩니다.

- CSP 파트너 계속 고객은 파트너의 위임 된 관리 권한을 제거 하는 경우에 기존 고객에 게 부여한를 사용 하 여 대리점 관계를 갖습니다 Autopilot 프로필을 관리할 수 있습니다.

- 추가한 고객에 게 기존 장치를 관리할 수 있습니다.

- 고객에 게는 비즈니스용 Microsoft Store 또는 Microsoft Intune 포털에 업로드 하는 장치를 관리할 수 없습니다.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>파트너 센터에서 Autopilot 프로필을 만들고 설정 합니다.

파트너 센터에서 Windows Autopilot 배포 프로필 만들기 및 장치에 적용할 수 있습니다.

>[!NOTE]
>관리 에이전트 에서만 만들고 프로필을 적용할 수 있습니다.

### <a name="create-a-new-autopilot-profile"></a>새 Autopilot 프로필 만들기

1. 선택 **고객** 파트너 센터 메뉴 선택에서 고객 만들 Autopilot 프로필에 대 한 합니다.

2. 고객의 세부 정보 페이지에서 선택 **장치**합니다.

3. 아래 **Windows Autopilot 프로필** 선택 **새 프로필 추가**합니다.

4. 프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다. 선택 합니다.  

   - 설치 프로그램에서 개인 정보 설정 건너뛰기

   - 설치 시 로컬 관리자 계정 비활성화
  
   - 설치 시 자동으로 페이지 건너뛰기<br>
        (포함 *직장 이나 학교 선택 자동으로 설치* 하 고 *건너뛰기 Cortana, OneDrive 및 OEM 등록 설정 페이지*)
  
   - 최종 사용자 사용권 계약 (EULA) 건너뛰기<br> 
       >[!IMPORTANT] 
       >참조 [Windows Autopilot EULA 사건의](#windows-autopilot-eula-dismissal) 아래 Windows 중 EULA 페이지 건너뛰기에 대 한 고려해 야 할 중요 한 정보를 설정 합니다.

5. 작업을 마쳤으면 **제출**을 선택합니다.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>고객의 장치에 Autopilot 프로필 적용

>[!NOTE]
>아래 지침에 따라 사용자가 이미 추가한 고객의 장치 파트너 센터 및 장치 목록에 액세스할 수 있는지를 가정 합니다. 고객의 장치를 추가 하지 않은 경우의 지침을 따릅니다 [고객의 계정에 장치 추가](#add-devices-to-a-customers-account) 아래 단계를 따릅니다.

고객에 대 한 Autopilot 프로필을 만든 후에 고객의 장치에 적용할 수 있습니다.

1. 선택 **고객** 파트너 센터 메뉴 선택에서 고객이 만든 Autopilot 프로필에 대 한 합니다.

2. 고객의 세부 정보 페이지에서 선택 **장치**합니다.

3. 아래 **장치에 프로필을 적용할** 장치 또는 프로필을 추가 하 고 선택한 장치 그룹 선택 **프로필을 적용**합니다. 방금 적용 프로필이 나타나고 합니다 **프로필** 열입니다.

4. 장치에 프로필을 성공적으로 적용할 수 있는지 확인 하려면 다음 단계를 수행 합니다.

    a.  네트워크 장치를 연결 하 고 전원을 켭니다.

    b.  적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.

    다.  OOBE 프로세스가 중지 되 면 새 사용자에 대 한 준비를 공장 기본 설정으로 장치를 재설정 합니다.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>고객의 장치에서 Autopilot 프로필을 제거 합니다.

1. 선택 **고객** 파트너 센터 메뉴 선택에서 고객이 만든 Autopilot 프로필에 대 한 합니다.

2. 고객의 세부 정보 페이지에서 선택 **장치**합니다.

3. 아래 **프로필을 장치에 적용할** 에서 프로필을 제거 하 고 선택 하려는 장치를 선택 **프로필을 제거**합니다.

   >[!NOTE]
   >장치에서 프로필을 제거 해도 프로필 목록에서 삭제 되지 않습니다. 프로필을 삭제 하려는 경우의 지침을 따릅니다 [Update 또는 delete Autopilot 프로필](#update-or-delete-an-autopilot-profile)합니다.

### <a name="update-or-delete-an-autopilot-profile"></a>Autopilot 프로필을 삭제 또는 업데이트

고객이 장치에 배송 한 후 기본 제공 환경을 변경 하는 경우에 파트너 센터에서 해당 프로필을 변경할 수 있습니다.

고객의 장치가 인터넷에 연결할 때 프로필이 최신 OOBE 과정에서 다운로드 됩니다. 또한 고객은 장치가 공장 기본 설정으로 복원 하 든 지 장치는 다시 최신 버전을 다운로드 프로필 OOBE 과정입니다.

1. 선택 **고객** 파트너 센터 메뉴와 Autopilot 프로필을 변경 하도록 요구 하는 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 선택 **장치**합니다.

3. 아래 **Windows Autopilot 프로필** 업데이트 해야 하는 프로필을 선택 합니다. 필요한 변경을 수행 하 고 선택한 **제출**합니다.

이 프로필을 삭제 하려면 선택 **프로필을 삭제** 페이지의 오른쪽 위 모서리에서.

### <a name="add-devices-to-a-customers-account"></a>고객의 계정에 장치 추가

>[!NOTE]
>영업 에이전트와 관리 에이전트 고객 계정에 장치를 추가할 수 있습니다.

고객의 장치에 사용자 지정 Autopilot 프로필을 적용할 수 있습니다, 전에 고객의 장치 목록에 액세스할 수 있어야 합니다.

OEM 이름, 일련 번호 및 모델 조합 사용 하려는 경우 이러한 제한 사항을 고려해 야 합니다.

- 최신 장치 (4 k 해시, 예를 들어)에 대해서만이 튜플 작동 128b 해시 (RS2 및 이전 장치)에 대 한 지원 되지 않습니다.

- 파일의 데이터 모델과 제조업체 이름과 일치 해야 하므로 튜플 등록은 대 소문자를 구분 ***정확 하 게*** OEM 공급자 (하드웨어 공급자)에서 제공 합니다.

파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따릅니다.

1. 선택 **고객** 파트너 센터 메뉴와 해당 장치를 관리 하려는 고객을 선택 합니다.

2. 고객의 세부 정보 페이지에서 선택 **장치**합니다.

3. 아래 **프로필을 장치에 적용할** 선택 **장치 추가**합니다.

4. 장치 목록에 대 한 이름을 입력 하 고 선택한 **찾아보기** 파트너 센터 고객 목록 (.csv 파일 형식)를 업로드할 수 있습니다.

    >[!NOTE]
    >장치 구매를 사용 하 여이.csv 파일을 받아야 합니다. .Csv 파일을 받지 않은 경우 만들면 직접의 단계를 수행 하 여 [Windows Autopilot 장치 추가](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)합니다.  

5. .Csv 파일을 업로드 하 고 선택한 **저장할**합니다.

.Csv 파일을 업로드 하는 동안 오류 메시지를 받게 되 면 파일의 형식을 확인 합니다. 전용 하드웨어 해시 또는 OEM 이름, 일련 번호 및 순서로 해당 열을 모델 또는 Windows 제품 ID를 사용할 수 있습니다. 옆의 링크에서 제공 된 샘플.csv 파일을 사용할 수도 있습니다 **장치 추가** 장치 목록을 만듭니다.

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 사건

### <a name="important-information"></a>중요 한 정보

Windows Autopilot을 사용 하면 고객에 게 관리 하는 장치에서 Windows의 사용자 지정된 설치를 구성할 수 있습니다. 이렇게 하려면 고객에 의해 권한이 부여 된, 표시 하지 않을 수도 있고 EULA (최종 사용자 사용권 계약) 동의 화면을 포함 하 여 Windows를 설정할 때 사용자에 게 일반적으로 표시 되는 특정 설정 화면을 숨길 수 있습니다.

이 함수를 사용 하 여 한다는 데 동의 억제 또는 공지 또는 충분 한 동 및 권한 부여 대신 용어 및 해당 사용자를 숨기려면 고객 으로부터 얻은 용어 의미에 대 한 동의 사용 하 여 사용자에 게 제공 하도록 설계 된 모든 화면 숨기기 (여부 조직 또는 개별 사용자의 경우 일 수 있음)를 고객은 알림 메시지에 동의 받고 모든 고객에 게 적용 되는 용어입니다. 여기에는 이 도구를 사용하여 표시하거나 숨기지 않는 경우, 사용자에게 제시되는 라이선스 약관 또는 고지에 대한 동의가 포함됩니다. 귀하의 고객이 Microsoft 또는 사용권이 허용된 배포자로부터 유효하게 소프트웨어 라이선스를 취득하지 않은 경우, 고객은 이러한 장치에서 Windows 소프트웨어를 사용할 수 없습니다.