---
title: Windows Autopilot으로 디바이스 설치 간소화 | 파트너 센터
ms.topic: article
ms.date: 10/29/2018
description: 파트너 센터에서 Windows AutoPilot 배포 프로필을 추가하여 Windows Autopilot으로 간단하게 디바이스 설치
author: KPacquer
ms.author: kenpacq
keywords: autopilot, windows autopilot, microsoft autopilot, 제로 터치 배포, oobe, 로그인 화면
ms.localizationpriority: medium
ms.openlocfilehash: 3d6e6e015424eb8be83bae21b2e15bdc072e480b
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917565"
---
<!--Maggie, 12/7/18 - removed line telling indirect resellers to go through their indirect providers for autopilot stuff as per Bhavya Chopra in bug 19841770.-->

# <a name="simplify-device-setup-with-windows-autopilot"></a><span data-ttu-id="ad58d-104">Windows Autopilot으로 디바이스 설치 간소화</span><span class="sxs-lookup"><span data-stu-id="ad58d-104">Simplify device setup with Windows Autopilot</span></span> 

<span data-ttu-id="ad58d-105">Windows Autopilot은 몇 단계만 거치면 첫 번째 부팅에서 새 Windows 10 Pro 디바이스의 설치를 간소화하고 보호합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span></span> <span data-ttu-id="ad58d-106">자세한 내용은 [Windows AutoPilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ad58d-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span>

## <a name="features"></a><span data-ttu-id="ad58d-107">기능</span><span class="sxs-lookup"><span data-stu-id="ad58d-107">Features</span></span>

- <span data-ttu-id="ad58d-108">디바이스를 설치하는 최종 사용자에 대해 **로컬 관리자 권한 해제**</span><span class="sxs-lookup"><span data-stu-id="ad58d-108">**Disable local administrator permissions** for the end users setting up devices</span></span>
- <span data-ttu-id="ad58d-109">**조직의 로그인 페이지 표시**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-109">**Show an organization's login page**.</span></span> <span data-ttu-id="ad58d-110">조직에서 작업으로 장치를 추가 하 고 Azure Active Directory를 사용 하 여 장치를 연결 하는 로그온 페이지를 정의할 미리 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-110">The organization can pre-define a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span></span>
- <span data-ttu-id="ad58d-111">OOBE가 완료된 후 Microsoft Intune 같은 **MDM(Mobile Device Manager)에 디바이스 등록**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span></span>
- <span data-ttu-id="ad58d-112">꼭 필요한 단계와 의사 결정 항목만 사용하도록 Windows AutoPilot 배포 프로필을 사용하여 **OOBE(첫 실행 경험) 간소화**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span></span>

## <a name="requirements"></a><span data-ttu-id="ad58d-113">요구 사항</span><span class="sxs-lookup"><span data-stu-id="ad58d-113">Requirements</span></span>

- <span data-ttu-id="ad58d-114">Windows 10 Pro 크리에이터스 업데이트(버전 1703 이상) 또는 Windows 10 Pro for Advanced PC가 미리 설치된 디바이스.</span><span class="sxs-lookup"><span data-stu-id="ad58d-114">Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later) or Windows 10 Pro for Advanced PCs.</span></span>
- <span data-ttu-id="ad58d-115">하드웨어 해시로 알려진 디바이스 식별자(128 HWH 또는 4k HWH). 일반적으로 OEM에서 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span></span> <span data-ttu-id="ad58d-116">식별자를 사용 하 여 파트너 센터에서 조직 프로필을 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-116">You'll use identifiers to assign organization profiles in the Partner Center.</span></span>
- <span data-ttu-id="ad58d-117">디바이스가 인터넷에 액세스할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-117">The devices must have access to the internet.</span></span> <span data-ttu-id="ad58d-118">디바이스를 연결할 수 없는 경우 기본 Windows OOBE(첫 실행 경험) 화면이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-118">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span></span>
- <span data-ttu-id="ad58d-119">디바이스를 MDM에 등록하려면 Azure Active Directory Premium이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-119">Enrolling the device into an MDM requires Azure Active Directory Premium.</span></span>

## <a name="add-company-branded-sign-in-pages-to-oobe"></a><span data-ttu-id="ad58d-120">OOBE에 회사 브랜드의 로그인 페이지 추가</span><span class="sxs-lookup"><span data-stu-id="ad58d-120">Add company-branded sign-in pages to OOBE</span></span>

<span data-ttu-id="ad58d-121">회사에 특정 페이지를 추가 하려면 회사의 [Azure AD 디렉터리](https://go.microsoft.com/fwlink/?linkid=848958) 에 디바이스를 추가 하 고 로그인 페이지를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-121">To add company-specific pages, add the devices into your company's [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span></span>

## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="ad58d-122">Windows AutoPilot 배포 프로필을 사용하여 OOBE에서 Windows 페이지 제거</span><span class="sxs-lookup"><span data-stu-id="ad58d-122">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span></span>

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="ad58d-123">Windows AutoPilot 배포 프로필의 설정 예</span><span class="sxs-lookup"><span data-stu-id="ad58d-123">Examples of settings in a Windows AutoPilot deployment profile</span></span>

- <span data-ttu-id="ad58d-124">설치 시 개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="ad58d-124">Skip Privacy Settings in setup</span></span>
- <span data-ttu-id="ad58d-125">설치 시 로컬 관리자 계정 비활성화</span><span class="sxs-lookup"><span data-stu-id="ad58d-125">Disable local admin account in setup</span></span>
- <span data-ttu-id="ad58d-126">설치 시 자동으로 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="ad58d-126">Automatically skip pages in setup</span></span>
  - <span data-ttu-id="ad58d-127">자동으로 회사 또는 학교 설치 선택</span><span class="sxs-lookup"><span data-stu-id="ad58d-127">Automatically select setup for work or school</span></span>
  - <span data-ttu-id="ad58d-128">Cortana, OneDrive 및 OEM 등록 설정 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="ad58d-128">Skip Cortana, OneDrive, and OEM registration setup pages</span></span>

### <a name="add-devices-and-apply-a-profile"></a><span data-ttu-id="ad58d-129">디바이스를 추가하고 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="ad58d-129">Add devices and apply a profile</span></span>

<span data-ttu-id="ad58d-130">파트너 센터에서 Windows AutoPilot 배포 프로필을 만들고 디바이스의 목록에 적용 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-130">From Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span></span>

<span data-ttu-id="ad58d-131">디바이스를 구성하려면 디바이스 목록을 업로드하고, 해당 디바이스에 적용되는 프로필을 만들어서 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-131">To configure devices, upload a list of the devices, create a profile that applies to the devices, and apply it.</span></span>

1.  <span data-ttu-id="ad58d-132">디바이스 목록을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-132">Add the list of devices.</span></span>

    <span data-ttu-id="ad58d-133">(영업 에이전트와 관리자 에이전트는 디바이스 목록을 파트너 센터에 추가할 수 있는 권한을 갖습니다.)</span><span class="sxs-lookup"><span data-stu-id="ad58d-133">Sales agents and admin agents have access to add the list of devices into Partner Center.</span></span>

    <span data-ttu-id="ad58d-134">a.</span><span class="sxs-lookup"><span data-stu-id="ad58d-134">a.</span></span> <span data-ttu-id="ad58d-135">[Windows AutoPilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)항목의 PowerShell 스크립트를 사용 하 여.csv 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-135">Create a .csv file using the PowerShell script from the topic [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span> <span data-ttu-id="ad58d-136">이 .csv 파일에는 일련 번호, OEM 이름, 모델 이름, 제품 ID, 디바이스 식별자를 포함한 디바이스 정보가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-136">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span></span> 

    <span data-ttu-id="ad58d-137">b.</span><span class="sxs-lookup"><span data-stu-id="ad58d-137">b.</span></span> <span data-ttu-id="ad58d-138">파트너 센터에서 **고객** 에 게 이동 > 장치를 수신 하는 고객을 선택 > **장치 > 장치 추가**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-138">From Partner Center, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span></span>

    <span data-ttu-id="ad58d-139">c.</span><span class="sxs-lookup"><span data-stu-id="ad58d-139">c.</span></span> <span data-ttu-id="ad58d-140">디바이스의 일괄 처리 이름을 지정합니다(예: “Contoso 영업 부서 PC – 2017년 4월 주문”).</span><span class="sxs-lookup"><span data-stu-id="ad58d-140">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span></span> 

    <span data-ttu-id="ad58d-141">d.</span><span class="sxs-lookup"><span data-stu-id="ad58d-141">d.</span></span> <span data-ttu-id="ad58d-142">**찾아보기** 선택 > 장치 정보 파일 선택 > **유효성 검사**합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-142">Select **Browse** > select the device info file > **Validate**.</span></span>

    <span data-ttu-id="ad58d-143">**참고:** .csv 파일을 업로드한 후 오류 메시지가 나타나면 파일 형식을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-143">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="ad58d-144">8월 이후에는 하드웨어 해시만 사용하거나 OEM 이름, 일련 번호 및 모델을 해당 열의 순서대로 사용하거나 Windows 제품 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-144">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span></span> <span data-ttu-id="ad58d-145">**장치 추가** 옆에 있는 링크에서 제공하는 샘플 .csv 파일을 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-145">You can also use the sample .csv file provided from the link next to **Add devices**.</span></span>

2.  <span data-ttu-id="ad58d-146">디바이스에 적용할 수 있는 프로필을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-146">Create a profile that you can apply to the devices.</span></span> <span data-ttu-id="ad58d-147">(오직 관리자 에이전트만 만들어 파트너 센터에서 프로필을 적용 하.)</span><span class="sxs-lookup"><span data-stu-id="ad58d-147">(Only admin agents have access to create and apply profiles in the Partner Center.)</span></span>

    <span data-ttu-id="ad58d-148">a.</span><span class="sxs-lookup"><span data-stu-id="ad58d-148">a.</span></span>  <span data-ttu-id="ad58d-149">**장치** **새 프로필 추가**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-149">From **Devices**, select **Add new profile**.</span></span>

    <span data-ttu-id="ad58d-150">b.</span><span class="sxs-lookup"><span data-stu-id="ad58d-150">b.</span></span>  <span data-ttu-id="ad58d-151">프로필 이름을 지정합니다(예: “Contoso 데스크톱 프로필 – 모든 OOBE 건너뛰기”).</span><span class="sxs-lookup"><span data-stu-id="ad58d-151">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span></span>

    <span data-ttu-id="ad58d-152">c.</span><span class="sxs-lookup"><span data-stu-id="ad58d-152">c.</span></span>  <span data-ttu-id="ad58d-153">OOBE 설정을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-153">Configure the OOBE settings.</span></span> <span data-ttu-id="ad58d-154">예를 들어 **Skip Express Settings in setup**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-154">For example, check **Skip Express Settings in setup**.</span></span>

    <span data-ttu-id="ad58d-155">d.</span><span class="sxs-lookup"><span data-stu-id="ad58d-155">d.</span></span>  <span data-ttu-id="ad58d-156">**제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-156">Select **Submit**.</span></span>

3.  <span data-ttu-id="ad58d-157">프로필을 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-157">Apply the profile.</span></span>

    <span data-ttu-id="ad58d-158">a.</span><span class="sxs-lookup"><span data-stu-id="ad58d-158">a.</span></span>  <span data-ttu-id="ad58d-159">**장치**의 **장치 할당 및 삭제** 창에서 구성할 디바이스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-159">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span></span> <span data-ttu-id="ad58d-160">일괄 처리 전체를 선택하려면 일괄 처리 이름(예: “Contoso 영업 부서 PC – 2017년 3월 주문”) 옆에 있는 확인란을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-160">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span></span>

    <span data-ttu-id="ad58d-161">b.</span><span class="sxs-lookup"><span data-stu-id="ad58d-161">b.</span></span>  <span data-ttu-id="ad58d-162">**적용 프로필**을 선택 하 고 프로필 (예를 들어 "Contoso 데스크톱 프로필 – 모든 OOBE 건너뛰기")를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-162">Select **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span></span> <span data-ttu-id="ad58d-163">디바이스의 프로필 열에 프로필이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-163">The devices will show the profile in the Profile column.</span></span>

4.  <span data-ttu-id="ad58d-164">선택 사항: 프로필이 정상적으로 작동하는지 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-164">Optional: Test to see that your profile works.</span></span>

    <span data-ttu-id="ad58d-165">a.</span><span class="sxs-lookup"><span data-stu-id="ad58d-165">a.</span></span>  <span data-ttu-id="ad58d-166">장치 네트워크에 연결한 다음 켭니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-166">Connect a device to the network and then turn it on.</span></span>

    <span data-ttu-id="ad58d-167">b.</span><span class="sxs-lookup"><span data-stu-id="ad58d-167">b.</span></span>  <span data-ttu-id="ad58d-168">적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-168">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="ad58d-169">c.</span><span class="sxs-lookup"><span data-stu-id="ad58d-169">c.</span></span>  <span data-ttu-id="ad58d-170">디바이스를 사용할 새 사용자를 위해 OOBE 환경을 완료한 다음 디바이스를 공장 기본 설정으로 초기화합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-170">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span></span>

## <a name="to-update-or-delete-a-profile"></a><span data-ttu-id="ad58d-171">프로필을 업데이트 또는 삭제하려면</span><span class="sxs-lookup"><span data-stu-id="ad58d-171">To update or delete a profile</span></span> 

<span data-ttu-id="ad58d-172">프로필을 장치에 할당 한 후 고객에 게 장치를 이미 제공한 경우에를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-172">After you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span></span> <span data-ttu-id="ad58d-173">디바이스가 인터넷에 연결되면 OOBE 프로세스가 진행되는 동안 최신 버전의 프로필이 디바이스로 다운로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-173">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span></span> <span data-ttu-id="ad58d-174">고객이 디바이스를 공장 기본 설정으로 복원하는 경우 디바이스가 최신 업데이트를 다시 프로필로 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-174">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 

### <a name="remove-a-profile-from-a-device"></a><span data-ttu-id="ad58d-175">장치에서 프로필 제거</span><span class="sxs-lookup"><span data-stu-id="ad58d-175">Remove a profile from a device</span></span>

1. <span data-ttu-id="ad58d-176">프로필을 제거할 디바이스(또는 디바이스의 일괄 처리)를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-176">Select the device (or batch of devices) you want to remove the profile from.</span></span> 

2. <span data-ttu-id="ad58d-177">**디바이스 할당 및 삭제** 창에서 **프로필 제거**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-177">In **Assign and delete devices** pane, select **Remove profile**.</span></span>

3. <span data-ttu-id="ad58d-178">제거하려는 프로필로 이동하여 해당 프로필을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-178">Go to the profile you want to remove and delete it.</span></span> <span data-ttu-id="ad58d-179">모든 디바이스에서 해당 프로필이 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-179">The profile will be deleted from all devices.</span></span>

<span data-ttu-id="ad58d-180">**장치**에서 해당 프로필을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-180">From **Devices**, select the profile.</span></span> <span data-ttu-id="ad58d-181">여기서 기존 설정을 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-181">From here, you can modify the existing settings.</span></span>

## <a name="windows-autopilot-eula-dismissal--important-information"></a><span data-ttu-id="ad58d-182">Windows Autopilot EULA 철회 – 중요한 정보</span><span class="sxs-lookup"><span data-stu-id="ad58d-182">Windows Autopilot EULA dismissal – important information</span></span>

<span data-ttu-id="ad58d-183">이 도구를 사용하면 고객을 위해 관리하는 장치에서 Windows 개별 설치를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-183">Using this tool allows you to configure individual installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="ad58d-184">고객이 승인한 경우 EULA 동의 화면 등 Windows를 설정할 때 일반적으로 사용자에게 제시되는 일부 설정 화면을 표시하지 않거나 숨길 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-184">If authorized to do so by the customer, you may choose to suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA acceptance screen.</span></span> 

<span data-ttu-id="ad58d-185">이 기능을 사용함으로써 귀하는 약관의 고지 또는 동의를 사용자에게 제공하도록 고안된 화면을 표시하지 않거나 숨기는 데 동의합니다. 이는 약관을 숨기기 위해 고객으로부터 충분한 동의와 승인을 얻었으며 고객(경우에 따라 조직 또는 개별 사용자)을 대신하여 고지에 동의하고 고객에게 적용되는 약관에 동의함을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-185">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="ad58d-186">여기에는 이 도구를 사용하여 표시하거나 숨기지 않는 경우, 사용자에게 제시되는 라이선스 약관 또는 고지에 대한 동의가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-186">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="ad58d-187">귀하의 고객이 Microsoft 또는 사용권이 허용된 배포자로부터 유효하게 소프트웨어 라이선스를 취득하지 않은 경우, 고객은 이러한 장치에서 Windows 소프트웨어를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ad58d-187">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>