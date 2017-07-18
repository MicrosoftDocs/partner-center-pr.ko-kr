---
title: "Windows Autopilot으로 디바이스 설치 간소화 | 파트너 센터"
description: "파트너 센터에서 Windows AutoPilot 배포 프로필을 추가하여 Windows Autopilot으로 간단하게 디바이스 설치"
author: KPacquer
keywords: "autopilot, windows autopilot, microsoft autopilot, 제로 터치 배포, oobe, 로그인 화면"
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: aa650ee5f2848694fe44d4751d52f8014e0d22a8
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/01/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a><span data-ttu-id="36d13-104">Windows Autopilot으로 디바이스 설치 간소화</span><span class="sxs-lookup"><span data-stu-id="36d13-104">Simplify device setup with Windows Autopilot</span></span> 

<span data-ttu-id="36d13-105">Windows Autopilot은 몇 단계만 거치면 첫 번째 부팅에서 새 Windows 10 Pro 디바이스의 설치를 간소화하고 보호합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span></span> <span data-ttu-id="36d13-106">자세한 내용은 [Windows AutoPilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="36d13-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span>

## <a name="features"></a><span data-ttu-id="36d13-107">기능</span><span class="sxs-lookup"><span data-stu-id="36d13-107">Features</span></span>

*  <span data-ttu-id="36d13-108">디바이스를 설치하는 최종 사용자에 대해 **로컬 관리자 권한 해제**</span><span class="sxs-lookup"><span data-stu-id="36d13-108">**Disable local administrator permissions** for the end users setting up devices</span></span>
*  <span data-ttu-id="36d13-109">**조직의 로그인 페이지 표시**.</span><span class="sxs-lookup"><span data-stu-id="36d13-109">**Show an organization's login page**.</span></span> <span data-ttu-id="36d13-110">조직에서는 디바이스를 회사 디바이스로 추가하고 Azure Active Directory에 가입하는 로그온 페이지를 미리 정의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-110">The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span></span>
*  <span data-ttu-id="36d13-111">OOBE가 완료된 후 Microsoft Intune 같은 **MDM(Mobile Device Manager)에 디바이스 등록**.</span><span class="sxs-lookup"><span data-stu-id="36d13-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span></span>
*  <span data-ttu-id="36d13-112">꼭 필요한 단계와 의사 결정 항목만 사용하도록 Windows AutoPilot 배포 프로필을 사용하여 **OOBE(첫 실행 경험) 간소화**.</span><span class="sxs-lookup"><span data-stu-id="36d13-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span></span> 

## <a name="requirements"></a><span data-ttu-id="36d13-113">요구 사항</span><span class="sxs-lookup"><span data-stu-id="36d13-113">Requirements</span></span>

*  <span data-ttu-id="36d13-114">Windows 10 Pro 크리에이터스 업데이트(1703 이상)가 미리 설치된 디바이스</span><span class="sxs-lookup"><span data-stu-id="36d13-114">Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later)</span></span>
*  <span data-ttu-id="36d13-115">하드웨어 해시로 알려진 디바이스 식별자(128 HWH 또는 4k HWH). 일반적으로 OEM에서 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span></span> <span data-ttu-id="36d13-116">식별자를 사용하여 파트너 센터에서 조직 프로필을 할당할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-116">You'll use identifiers to assign organization profiles in Partner Center.</span></span> <span data-ttu-id="36d13-117">2017년 8월 이후부터는 더 이상 하드웨어 해시가 필요 없습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-117">After August 2017 you will no longer need the hardware hash.</span></span> 
*  <span data-ttu-id="36d13-118">디바이스가 인터넷에 액세스할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-118">The devices must have access to the internet.</span></span> <span data-ttu-id="36d13-119">디바이스를 연결할 수 없는 경우 기본 Windows OOBE(첫 실행 경험) 화면이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-119">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span></span>
*  <span data-ttu-id="36d13-120">디바이스를 MDM에 등록하려면 Azure Active Directory Premium이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-120">Enrolling the device into an MDM requires Azure Active Directory Premium.</span></span>

## <a name="add-organization-login-pages-to-oobe"></a><span data-ttu-id="36d13-121">OOBE에 조직 로그인 페이지 추가</span><span class="sxs-lookup"><span data-stu-id="36d13-121">Add organization login pages to OOBE</span></span>

<span data-ttu-id="36d13-122">조직 관련 페이지를 추가하려면 디바이스를 조직의 [Azure AD 디렉터리](https://go.microsoft.com/fwlink/?linkid=848958)에 추가하고 로그인 페이지를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-122">To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span></span>


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="36d13-123">Windows AutoPilot 배포 프로필을 사용하여 OOBE에서 Windows 페이지 제거</span><span class="sxs-lookup"><span data-stu-id="36d13-123">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span></span>

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="36d13-124">Windows AutoPilot 배포 프로필의 설정 예</span><span class="sxs-lookup"><span data-stu-id="36d13-124">Examples of settings in a Windows AutoPilot deployment profile</span></span>
*  <span data-ttu-id="36d13-125">설치 시 개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="36d13-125">Skip Privacy Settings in setup</span></span>
*  <span data-ttu-id="36d13-126">설치 시 로컬 관리자 계정 비활성화</span><span class="sxs-lookup"><span data-stu-id="36d13-126">Disable local admin account in setup</span></span>
*  <span data-ttu-id="36d13-127">설치 시 자동으로 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="36d13-127">Automatically skip pages in setup</span></span>
   *  <span data-ttu-id="36d13-128">자동으로 회사 또는 학교 설치 선택</span><span class="sxs-lookup"><span data-stu-id="36d13-128">Automatically select setup for work or school</span></span>
   *  <span data-ttu-id="36d13-129">Cortana, OneDrive 및 OEM 등록 설정 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="36d13-129">Skip Cortana, OneDrive, and OEM registration setup pages</span></span>

### <a name="add-devices-and-apply-a-profile"></a><span data-ttu-id="36d13-130">디바이스를 추가하고 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="36d13-130">Add devices and apply a profile</span></span>

<span data-ttu-id="36d13-131">파트너 센터에서 Windows AutoPilot 배포 프로필을 만들어 디바이스 목록에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-131">In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span></span>

<span data-ttu-id="36d13-132">디바이스를 구성하려면 디바이스 목록을 파트너 센터에 업로드하고, 해당 디바이스에 적용되는 프로필을 만들어서 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-132">To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.</span></span>

1.  <span data-ttu-id="36d13-133">디바이스 목록을 파트너 센터에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-133">Add the list of devices into Partner Center.</span></span> <span data-ttu-id="36d13-134">(영업 에이전트와 관리자 에이전트는 디바이스 목록을 파트너 센터에 추가할 수 있는 권한을 갖습니다.)</span><span class="sxs-lookup"><span data-stu-id="36d13-134">(Sales agents and admin agents have access to add the list of devices into Partner Center.)</span></span>

    <span data-ttu-id="36d13-135">a.</span><span class="sxs-lookup"><span data-stu-id="36d13-135">a.</span></span>  <span data-ttu-id="36d13-136">[Windows AutoPilot 개요](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot) 항목의 PowerShell 스크립트를 사용하여 .csv 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-136">Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span> <span data-ttu-id="36d13-137">이 .csv 파일에는 일련 번호, OEM 이름, 모델 이름, 제품 ID, 디바이스 식별자를 포함한 디바이스 정보가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-137">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span></span> 

    <span data-ttu-id="36d13-138">b.</span><span class="sxs-lookup"><span data-stu-id="36d13-138">b.</span></span>  <span data-ttu-id="36d13-139">파트너 센터 대시보드에서 **고객** > select the customer that’s receiving the devices > **장치 > 장치 추가**로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-139">From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span></span>

    <span data-ttu-id="36d13-140">c.</span><span class="sxs-lookup"><span data-stu-id="36d13-140">c.</span></span>  <span data-ttu-id="36d13-141">디바이스의 일괄 처리 이름을 지정합니다(예: “Contoso 영업 부서 PC – 2017년 4월 주문”).</span><span class="sxs-lookup"><span data-stu-id="36d13-141">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span></span> 

    <span data-ttu-id="36d13-142">d.</span><span class="sxs-lookup"><span data-stu-id="36d13-142">d.</span></span>  <span data-ttu-id="36d13-143">**찾아보기** > 장치 정보 파일 선택 > **유효성 검사**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-143">Click **Browse** > select the device info file > **Validate**.</span></span>

    <span data-ttu-id="36d13-144">**참고:** .csv 파일을 업로드한 후 오류 메시지가 나타나면 파일 형식을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-144">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="36d13-145">8월 이후에는 하드웨어 해시만 사용하거나 OEM 이름, 일련 번호 및 모델을 해당 열의 순서대로 사용하거나 Windows 제품 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-145">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span></span> <span data-ttu-id="36d13-146">**장치 추가** 옆에 있는 링크에서 제공하는 샘플 .csv 파일을 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-146">You can also use the sample .csv file provided from the link next to **Add devices**.</span></span>

2.  <span data-ttu-id="36d13-147">디바이스에 적용할 수 있는 프로필을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-147">Create a profile that you can apply to the devices.</span></span> <span data-ttu-id="36d13-148">(오직 관리자 에이전트만이 파트너 센터에서 프로필을 만들고 적용할 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="36d13-148">(Only admin agents have access to create and apply profiles in Partner Center.)</span></span>

    <span data-ttu-id="36d13-149">a.</span><span class="sxs-lookup"><span data-stu-id="36d13-149">a.</span></span>  <span data-ttu-id="36d13-150">**장치**에서 **새 프로필 추가**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-150">From **Devices**, click **Add new profile**.</span></span>

    <span data-ttu-id="36d13-151">b.</span><span class="sxs-lookup"><span data-stu-id="36d13-151">b.</span></span>  <span data-ttu-id="36d13-152">프로필 이름을 지정합니다(예: “Contoso 데스크톱 프로필 – 모든 OOBE 건너뛰기”).</span><span class="sxs-lookup"><span data-stu-id="36d13-152">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span></span>

    <span data-ttu-id="36d13-153">c.</span><span class="sxs-lookup"><span data-stu-id="36d13-153">c.</span></span>  <span data-ttu-id="36d13-154">OOBE 설정을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-154">Configure the OOBE settings.</span></span> <span data-ttu-id="36d13-155">예를 들어 **Skip Express Settings in setup**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-155">For example, check **Skip Express Settings in setup**.</span></span>

    <span data-ttu-id="36d13-156">d.</span><span class="sxs-lookup"><span data-stu-id="36d13-156">d.</span></span>  <span data-ttu-id="36d13-157">**제출**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-157">Click **Submit**.</span></span>

3.  <span data-ttu-id="36d13-158">프로필을 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-158">Apply the profile.</span></span>

    <span data-ttu-id="36d13-159">a.</span><span class="sxs-lookup"><span data-stu-id="36d13-159">a.</span></span>  <span data-ttu-id="36d13-160">**장치**의 **장치 할당 및 삭제** 창에서 구성할 디바이스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-160">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span></span> <span data-ttu-id="36d13-161">일괄 처리 전체를 선택하려면 일괄 처리 이름(예: “Contoso 영업 부서 PC – 2017년 3월 주문”) 옆에 있는 확인란을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-161">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span></span>

    <span data-ttu-id="36d13-162">b.</span><span class="sxs-lookup"><span data-stu-id="36d13-162">b.</span></span>  <span data-ttu-id="36d13-163">**프로필 적용**을 클릭하고 프로필(예: "Contoso 데스크톱 프로필 - 모든 OOBE 건너뛰기")을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-163">Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span></span> <span data-ttu-id="36d13-164">디바이스의 프로필 열에 프로필이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-164">The devices will show the profile in the Profile column.</span></span>

4.  <span data-ttu-id="36d13-165">선택 사항: 프로필이 정상적으로 작동하는지 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-165">Optional: Test to see that your profile works.</span></span>

    <span data-ttu-id="36d13-166">a.</span><span class="sxs-lookup"><span data-stu-id="36d13-166">a.</span></span>  <span data-ttu-id="36d13-167">디바이스를 네트워크에 연결하고 켭니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-167">Connect a device to the network, and turn it on.</span></span>

    <span data-ttu-id="36d13-168">b.</span><span class="sxs-lookup"><span data-stu-id="36d13-168">b.</span></span>  <span data-ttu-id="36d13-169">적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-169">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="36d13-170">c.</span><span class="sxs-lookup"><span data-stu-id="36d13-170">c.</span></span>  <span data-ttu-id="36d13-171">디바이스를 사용할 새 사용자를 위해 OOBE 환경을 완료한 다음 디바이스를 공장 기본 설정으로 초기화합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-171">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span></span>


## <a name="to-update-or-delete-a-profile"></a><span data-ttu-id="36d13-172">프로필을 업데이트 또는 삭제하려면</span><span class="sxs-lookup"><span data-stu-id="36d13-172">To update or delete a profile</span></span> 

<span data-ttu-id="36d13-173">디바이스에 프로필을 할당했으면 디바이스를 업데이트할 수 있으며, 심지어 고객에게 디바이스를 건넨 후에도 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-173">Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span></span> <span data-ttu-id="36d13-174">디바이스가 인터넷에 연결되면 OOBE 프로세스가 진행되는 동안 최신 버전의 프로필이 디바이스로 다운로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-174">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span></span> <span data-ttu-id="36d13-175">고객이 디바이스를 공장 기본 설정으로 복원하는 경우 디바이스가 최신 업데이트를 다시 프로필로 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-175">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 

###<a name="you-can-remove-a-profile-from-a-device"></a><span data-ttu-id="36d13-176">디바이스에서 프로필을 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-176">You can remove a profile from a device</span></span>
1. <span data-ttu-id="36d13-177">프로필을 제거할 디바이스(또는 디바이스의 일괄 처리)를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-177">Select the device (or batch of devices) you want to remove the profile from.</span></span> 

2. <span data-ttu-id="36d13-178">**디바이스 할당 및 삭제** 창에서 **프로필 제거**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-178">In **Assign and delete devices** pane, select **Remove profile**.</span></span>

3. <span data-ttu-id="36d13-179">제거하려는 프로필로 이동하여 해당 프로필을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-179">Go to the profile you want to remove and delete it.</span></span> <span data-ttu-id="36d13-180">모든 디바이스에서 해당 프로필이 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-180">The profile will be deleted from all devices.</span></span>

<span data-ttu-id="36d13-181">**장치**에서 해당 프로필을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-181">From **Devices**, select the profile.</span></span> <span data-ttu-id="36d13-182">여기서 기존 설정을 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36d13-182">From here, you can modify the existing settings.</span></span>
