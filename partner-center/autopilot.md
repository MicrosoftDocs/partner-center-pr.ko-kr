---
title: 장치의 기본 제공 환경 사용자 지정
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객의 새 장치를 제공 하기 전에 Windows Autopilot 프로필을 사용 하 여 장치의 OOBE (기본 제공 경험)를 사용자 지정 하거나 미리 구성할 수 있습니다.
author: LauraBrenner
ms.author: labrenne
keywords: autopilot, windows autopilot, microsoft autopilot, zero touch 배포, oobe, 로그인 화면, 기본
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a3067b674b7784df34fba3de9cfaa5b44349b8c4
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679190"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>새 장치에서 Windows Autopilot 프로필을 사용 하 여 고객의 기본 환경을 사용자 지정 합니다.

**적용 대상**

- CSP 직접-청구서 파트너, 간접 공급자 및 간접 대리점

**적절한 역할**

- 관리 에이전트
- 글로벌 관리자
- 영업 상담원
- 사용자 관리 담당자

고객 장치를 관리 하는 경우 고객의 사용자에 대 한 OOBE (기본 경험)를 사용자 지정 해야 할 수 있습니다. 장치를 고객에 게 배달 하기 전에 Windows Autopilot 프로필을 사용 하 여 새 장치를 미리 구성 하 고 고객이 이미 구매한 장치에 새 프로필을 적용할 수 있습니다. 

Oem은 장치의 **제품 키 id (pkid)** 를 표시 하는 Autopilot 장치 상자 외부에 배송 레이블을 포함 하기 시작 했습니다.  이 1 차원, 읽을 수 있는 바코드는 장치를 unbox 하 고 다른 방법으로 장치 ID를 수집 하지 않고도 Autopilot에 대 한 장치를 등록 하는 방법을 제공 하는 다운스트림 파트너를 제공 합니다.

이 문서에서는 파트너 센터에서 장치에 Autopilot 프로필을 만들고 적용 하는 방법을 설명 합니다.

Autopilot에 익숙하지 않은 경우 다음 문서의 정보를 검토 하세요.

- [Windows Autopilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 배포 참조 가이드](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>개요

파트너 센터의 Windows Autopilot 기능을 사용 하면 고객 장치에 적용할 사용자 지정 프로필을 만들 수 있습니다. 이 문서를 게시할 때 다음 프로필 설정을 사용할 수 있습니다.

- 개인 정보 설정 건너뛰기 이 선택적 Autopilot 프로필 설정을 사용 하면 조직에서 OOBE 프로세스 중 개인 정보 설정에 대해 질문할 수 있습니다.

- 장치에서 로컬 관리자 계정 만들기를 사용 하지 않도록 설정 합니다. 조직에서는 프로세스가 완료 된 후 장치를 설정 하는 사용자에 게 관리자 권한이 있는지 여부를 결정할 수 있습니다.

- 회사 또는 학교에 대 한 장치를 자동으로 설정 합니다. Autopilot에 등록 된 모든 장치는 회사 또는 학교 장치로 자동으로 간주 되므로이 질문은 OOBE 프로세스 중에 묻지 않습니다.

- Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다. Autopilot에 등록 된 모든 장치는 OOBE (기본 경험) 프로세스 중에 이러한 페이지를 자동으로 건너뜁니다.

- EULA (최종 사용자 사용권 계약)를 건너뜁니다. Windows 10 버전 1709부터 조직은 OOBE 프로세스 중에 제공 된 EULA 페이지를 건너뛰도록 결정할 수 있습니다. Windows 설치 중에 EULA 페이지를 건너뛰는 방법에 대해 고려해 야 하는 중요 한 정보는 [Windows AUTOPILOT EULA 해제](#windows-autopilot-eula-dismissal) 를 참조 하세요.

다음 프로필 및 장치 관리 권한 및 제한이 적용 됩니다.

- CSP 파트너는 고객이 파트너의 위임 된 관리 권한을 제거한 경우에도 재판매인 관계가 있는 기존 고객에 대해 Autopilot 프로필을 계속 관리할 수 있습니다.

- 추가한 고객에 대 한 기존 장치를 관리할 수 있습니다.

- 고객이 비즈니스용 Microsoft Store 또는 Microsoft Intune 포털에 업로드 한 장치를 관리할 수 없습니다.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>파트너 센터에서 Autopilot 프로필 만들기 및 관리

파트너 센터에서 Windows Autopilot 배포 프로필을 만들어 장치에 적용할 수 있습니다.

>[!NOTE]
>관리자 에이전트만 프로필을 만들고 적용할 수 있습니다.

### <a name="create-a-new-autopilot-profile"></a>새 Autopilot 프로필 만들기

1. 파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만들 고객을 선택 합니다.

2. 고객 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **Windows Autopilot 프로필** 에서 **추가 새 프로필**을 선택 합니다.

4. 프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다. 다음 중에서 선택합니다.  

   - 설치에서 개인 정보 설정 건너뛰기

   - 설치 프로그램에서 로컬 관리자 계정 사용 안 함
  
   - 설치 프로그램에서 자동으로 페이지 건너뛰기<br>
        ( *회사 또는 학교에 대 한 설치를 자동으로 선택* 하 고 *Cortana, OneDrive 및 OEM 등록 설정 페이지 건너뛰기*)
  
   - EULA (최종 사용자 사용권 계약) 건너뛰기<br> 
       >[!IMPORTANT] 
       >Windows 설치 중에 EULA 페이지를 건너뛰는 방법에 대해 고려해 야 하는 중요 한 정보는 [Windows AUTOPILOT EULA 해제](#windows-autopilot-eula-dismissal) 를 참조 하세요.

5. 완료 되 면 **제출** 을 선택 합니다.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>고객 장치에 Autopilot 프로필 적용

>[!NOTE]
>아래 지침에서는 고객의 장치를 파트너 센터에 이미 추가 했 고 해당 장치 목록에 액세스할 수 있다고 가정 합니다. 고객의 장치를 아직 추가 하지 않은 경우 [고객 계정에 장치 추가](#add-devices-to-a-customers-account) 의 지침에 따라 다음 단계를 수행 합니다.

고객에 대 한 Autopilot 프로필을 만든 후 고객의 장치에 적용할 수 있습니다.

1. 파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만든 고객을 선택 합니다.

2. 고객 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **장치에 프로필 적용** 에서 프로필을 추가할 장치 또는 장치 그룹을 선택 하 고 **프로필 적용**을 선택 합니다. 방금 적용 한 프로필이 **프로필** 열에 표시 됩니다.

4. 아래 단계에 따라 프로필이 장치에 성공적으로 적용 되는지 확인 합니다.

    a.  장치를 네트워크에 연결 하 고 설정 합니다.

    b.  적절 한 OOBE 화면 (있는 경우)이 표시 되는지 확인 합니다.

    다.  OOBE 프로세스가 중지 되 면 장치를 공장 기본 설정으로 다시 설정 하 여 새 사용자에 대해 준비 합니다.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>고객의 장치에서 Autopilot 프로필 제거

1. 파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만든 고객을 선택 합니다.

2. 고객 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **장치에 프로필 적용** 에서 프로필을 제거 하려는 장치를 선택 하 고 **프로필 제거**를 선택 합니다.

   >[!NOTE]
   >장치에서 프로필을 제거 해도 해당 프로필은 목록에서 삭제 되지 않습니다. 프로필을 삭제 하려면 [Autopilot 프로필 업데이트 또는 삭제](#update-or-delete-an-autopilot-profile)의 지침을 따르세요.

### <a name="update-or-delete-an-autopilot-profile"></a>Autopilot 프로필 업데이트 또는 삭제

고객이 장치를 배송 한 후 기본 경험을 변경 하려는 경우 파트너 센터에서 프로필을 변경할 수 있습니다.

고객의 장치가 인터넷에 연결 되 면 OOBE 프로세스 중에 최신 프로필 버전이 다운로드 됩니다. 또한 고객이 공장 기본 설정으로 장치를 복원할 때마다 장치는 OOBE 프로세스 중에 최신 프로필 버전을 다시 다운로드 합니다.

1. 파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 변경 하려는 고객을 선택 합니다.

2. 고객 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **Windows Autopilot 프로필** 아래에서 업데이트 해야 하는 프로필을 선택 합니다. 필요한 변경 작업을 수행한 다음 **제출**을 선택 합니다.

이 프로필을 삭제 하려면 페이지의 오른쪽 위 모서리에서 **프로필 삭제** 를 선택 합니다.

### <a name="add-devices-to-a-customers-account"></a>고객 계정에 장치 추가

>[!NOTE]
>판매 에이전트 및 관리 에이전트는 고객의 계정에 장치를 추가할 수 있습니다.

사용자 지정 Autopilot 프로필을 고객 장치에 적용 하려면 먼저 고객의 장치 목록에 액세스할 수 있어야 합니다.

OEM 이름, 일련 번호 및 모델 조합을 사용할 계획인 경우 다음 제한 사항에 유의 하세요.

- 이 튜플은 최신 장치 (예: 4k 해시)에 대해서만 작동 하며, 128b 해시 (RS2 및 이전 장치)에 대해서는 지원 되지 않습니다.

- 튜플 등록은 대/소문자를 구분 하므로 파일의 데이터는 OEM 공급자 (하드웨어 공급자)에서 제공 하는 것과 ***정확 하 게*** 모델 및 제조업체 이름과 일치 해야 합니다.

파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따르세요.

1. 파트너 센터 메뉴에서 **고객** 을 선택 하 고 관리할 장치를 포함 하는 고객을 선택 합니다.

2. 고객 세부 정보 페이지에서 **장치**를 선택 합니다.

3. **장치에 프로필 적용** 에서 **장치 추가**를 선택 합니다.

4. 장치 목록에 대 한 이름을 입력 하 고 **찾아보기** 를 선택 하 여 고객 목록 (.csv 파일 형식)을 파트너 센터에 업로드 합니다.

    >[!NOTE]
    >장치를 구입 하 여이 .csv 파일을 수신 해야 합니다. .Csv 파일을 받지 못한 경우 [Windows Autopilot에 장치 추가](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)의 단계를 수행 하 여 직접 만들 수 있습니다.  

5. .Csv 파일을 업로드 하 고 **저장**을 선택 합니다.

.Csv 파일을 업로드 하는 동안 오류 메시지가 나타나면 파일의 형식을 확인 합니다. 하드웨어 해시만 또는 OEM 이름, 일련 번호 및 모델 (해당 열 순서 대로) 또는 Windows 제품 ID를 사용할 수 있습니다. 장치 **추가** 옆에 있는 링크에서 제공 된 샘플 .csv 파일을 사용 하 여 장치 목록을 만들 수도 있습니다.

.Csv 파일의 모양은 다음과 같습니다.

> **장치 일련 번호, Windows 제품 ID, 하드웨어 해시, 제조업체 이름, 장치 모델**

> **{,,,) Microsoft Corporation, Surface 노트북**

>[!NOTE]
> "제조업체 이름" 및 "장치 모델"은 대/소문자를 구분 합니다.

제조업체 이름 및 장치 모델에 넣을 값을 모르는 경우 장치에서이를 실행 하 여 올바른 값을 수집할 수 있습니다.

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 해제

### <a name="important-information"></a>중요 정보

Windows Autopilot를 사용 하면 고객을 위해 관리 하는 장치에서 Windows의 사용자 지정 설치를 구성할 수 있습니다. 고객이이 작업을 수행할 수 있는 권한이 있는 경우 EULA (최종 사용자 사용권 계약) 승인 화면을 비롯 한 Windows를 설정할 때 일반적으로 사용자에 게 표시 되는 특정 설정 화면을 표시 하거나 숨길 수 있습니다.

이 함수를 사용 하 여 사용자에 게 통지를 제공 하거나 약관에 동의 하도록 디자인 된 화면을 표시 하거나 숨기는 것은 사용자에 게 약관을 숨길 수 있는 충분 한 동의 및 권한 부여를 제공 하는 것을 의미 하 고, 고객을 대신 하 여 (조직이 나 개별 사용자가 될 수 있는지 여부에 관계 없이) 고객에 게 동의 하 고 고객에 게 적용 되는 모든 약관을 수락 여기에는이 도구를 사용 하 여 표시 하거나 숨기는 경우 사용자에 게 표시 되는 사용권 계약 조건에 대 한 계약이 포함 됩니다. 고객이 Microsoft 또는 라이선스 대리점에서 소프트웨어에 대 한 라이선스를 합법적으로 취득 하지 않은 경우 고객이 해당 장치에서 Windows 소프트웨어를 사용 하지 못할 수 있습니다.
