---
title: Windows Autopilot 프로필을 사용 하 여 장치의 기본 제공 환경을 사용자 지정 | 파트너 센터
description: Autopilot 프로필을 사용 하 여 장치의 기본 제공 환경을 미리 구성 합니다.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot, windows autopilot, microsoft autopilot, 제로 터치 배포, oobe, 로그인 화면, 기본 제공
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586916"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="0b58e-104">Windows Autopilot 프로필을 사용 하 여 장치의 기본 제공 환경을 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="0b58e-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="0b58e-105">**적용 대상**</span><span class="sxs-lookup"><span data-stu-id="0b58e-105">**Applies to**</span></span>

- <span data-ttu-id="0b58e-106">CSP 직접 청구 파트너, 간접 공급자 및 간접 대리점</span><span class="sxs-lookup"><span data-stu-id="0b58e-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="0b58e-107">고객의 장치를 관리 하는 경우에 고객의 사용자에 대 한 기본 제공 환경 (OOBE) 사용자 지정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="0b58e-108">고객에 게 장치를 제공 하기 전에 Windows Autopilot 프로필을 사용 하 여 새 장치를 미리 구성할 수 있으며 고객이 이미 구입한 장치에 새 프로필을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="0b58e-109">이 문서에서는 만들고 파트너 센터에서 장치에 Autopilot 프로필을 적용 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="0b58e-110">아직 수행 하지 않은 Autopilot을 사용 하 여 친숙 한,이 문서의 정보를 검토:</span><span class="sxs-lookup"><span data-stu-id="0b58e-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="0b58e-111">Windows Autopilot 개요</span><span class="sxs-lookup"><span data-stu-id="0b58e-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="0b58e-112">Autopilot 배포 참조 가이드</span><span class="sxs-lookup"><span data-stu-id="0b58e-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="0b58e-113">개요</span><span class="sxs-lookup"><span data-stu-id="0b58e-113">Overview</span></span>

<span data-ttu-id="0b58e-114">파트너 센터에서 Windows Autopilot 기능을 사용 하 여 고객의 장치에 적용할 사용자 지정 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="0b58e-115">이 문서는 게시 시점에 다음 프로필 설정을 사용할 수 없었습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="0b58e-116">개인 정보 설정을 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-116">Skip privacy settings.</span></span> <span data-ttu-id="0b58e-117">이 선택적 Autopilot 프로필 설정은 조직을 OOBE 과정에서 개인 정보 설정에 대 한 표시를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="0b58e-118">장치의 로컬 관리자 계정 만들기를 사용 하지 않도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="0b58e-119">조직에서는 프로세스가 완료 되 면 사용자 장치 설정에서 관리자 액세스할 수 있어야 하는지 여부를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="0b58e-120">회사 또는 학교에 대 한 장치를 자동으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="0b58e-121">Autopilot을 사용 하 여 등록 된 모든 장치 작업 자동으로 간주 됩니다 또는 OOBE 과정에서이 질문 확인 하도록 장치를 학교입니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="0b58e-122">Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="0b58e-123">Autopilot을 사용 하 여 등록 된 모든 장치에서 기본 제공 환경 (OOBE) 프로세스 중에 자동으로 이러한 페이지를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="0b58e-124">최종 사용자 사용권 계약 (EULA)을 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="0b58e-125">Windows 10 버전 1709부터 조직 EULA 페이지 OOBE 프로세스 중에 표시 하지 않으려면 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="0b58e-126">참조 [Windows Autopilot EULA 사건의](#windows-autopilot-eula-dismissal) 아래 Windows 중 EULA 페이지 건너뛰기에 대 한 고려해 야 할 중요 한 정보를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="0b58e-127">다음 프로필 및 장치 관리 권한 및 제한 사항이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="0b58e-128">CSP 파트너 계속 고객은 파트너의 위임 된 관리 권한을 제거 하는 경우에 기존 고객에 게 부여한를 사용 하 여 대리점 관계를 갖습니다 Autopilot 프로필을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="0b58e-129">추가한 사용자 또는 다른 CSP 파트너가 고객에 게 기존 장치를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="0b58e-130">고객에 게는 비즈니스용 Microsoft Store 또는 Microsoft Intune 포털에 업로드 하는 장치를 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="0b58e-131">파트너 센터에서 Autopilot 프로필을 만들고 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="0b58e-132">파트너 센터에서 Windows Autopilot 배포 프로필 만들기 및 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="0b58e-133">관리 에이전트 에서만 만들고 프로필을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="0b58e-134">새 Autopilot 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="0b58e-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="0b58e-135">선택 **고객** 파트너 센터 메뉴 선택에서 고객 만들 Autopilot 프로필에 대 한 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="0b58e-136">고객의 세부 정보 페이지에서 선택 **장치**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0b58e-137">아래 **Windows Autopilot 프로필** 선택 **새 프로필 추가**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="0b58e-138">프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="0b58e-139">선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-139">Choose from:</span></span>  

   - <span data-ttu-id="0b58e-140">설치 프로그램에서 개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0b58e-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="0b58e-141">설치 시 로컬 관리자 계정 비활성화</span><span class="sxs-lookup"><span data-stu-id="0b58e-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="0b58e-142">설치 시 자동으로 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0b58e-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="0b58e-143">(포함 *직장 이나 학교 선택 자동으로 설치* 하 고 *건너뛰기 Cortana, OneDrive 및 OEM 등록 설정 페이지*)</span><span class="sxs-lookup"><span data-stu-id="0b58e-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="0b58e-144">최종 사용자 사용권 계약 (EULA) 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0b58e-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="0b58e-145">참조 [Windows Autopilot EULA 사건의](#windows-autopilot-eula-dismissal) 아래 Windows 중 EULA 페이지 건너뛰기에 대 한 고려해 야 할 중요 한 정보를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="0b58e-146">작업을 마쳤으면 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="0b58e-147">고객의 장치에 Autopilot 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="0b58e-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="0b58e-148">아래 지침에 따라 사용자가 이미 추가한 고객의 장치 파트너 센터 및 장치 목록에 액세스할 수 있는지를 가정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="0b58e-149">고객의 장치를 추가 하지 않은 경우의 지침을 따릅니다 [고객의 계정에 장치 추가](#add-devices-to-a-customers-account) 아래 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="0b58e-150">고객에 대 한 Autopilot 프로필을 만든 후에 고객의 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="0b58e-151">선택 **고객** 파트너 센터 메뉴 선택에서 고객이 만든 Autopilot 프로필에 대 한 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="0b58e-152">고객의 세부 정보 페이지에서 선택 **장치**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0b58e-153">아래 **장치에 프로필을 적용할** 장치 또는 프로필을 추가 하 고 선택한 장치 그룹 선택 **프로필을 적용**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="0b58e-154">방금 적용 프로필이 나타나고 합니다 **프로필** 열입니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="0b58e-155">장치에 프로필을 성공적으로 적용할 수 있는지 확인 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="0b58e-156">a.</span><span class="sxs-lookup"><span data-stu-id="0b58e-156">a.</span></span>  <span data-ttu-id="0b58e-157">네트워크 장치를 연결 하 고 전원을 켭니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="0b58e-158">b.</span><span class="sxs-lookup"><span data-stu-id="0b58e-158">b.</span></span>  <span data-ttu-id="0b58e-159">적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="0b58e-160">c.</span><span class="sxs-lookup"><span data-stu-id="0b58e-160">c.</span></span>  <span data-ttu-id="0b58e-161">OOBE 프로세스가 중지 되 면 새 사용자에 대 한 준비를 공장 기본 설정으로 장치를 재설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="0b58e-162">고객의 장치에서 Autopilot 프로필을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="0b58e-163">선택 **고객** 파트너 센터 메뉴 선택에서 고객이 만든 Autopilot 프로필에 대 한 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="0b58e-164">고객의 세부 정보 페이지에서 선택 **장치**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0b58e-165">아래 **프로필을 장치에 적용할** 에서 프로필을 제거 하 고 선택 하려는 장치를 선택 **프로필을 제거**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="0b58e-166">장치에서 프로필을 제거 해도 프로필 목록에서 삭제 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="0b58e-167">프로필을 삭제 하려는 경우의 지침을 따릅니다 [Update 또는 delete Autopilot 프로필](#update-or-delete-an-autopilot-profile)합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="0b58e-168">Autopilot 프로필을 삭제 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="0b58e-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="0b58e-169">고객이 장치에 배송 한 후 기본 제공 환경을 변경 하는 경우에 파트너 센터에서 해당 프로필을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="0b58e-170">고객의 장치가 인터넷에 연결할 때 프로필이 최신 OOBE 과정에서 다운로드 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="0b58e-171">또한 고객은 장치가 공장 기본 설정으로 복원 하 든 지 장치는 다시 최신 버전을 다운로드 프로필 OOBE 과정입니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="0b58e-172">선택 **고객** 파트너 센터 메뉴와 Autopilot 프로필을 변경 하도록 요구 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="0b58e-173">고객의 세부 정보 페이지에서 선택 **장치**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0b58e-174">아래 **Windows Autopilot 프로필** 업데이트 해야 하는 프로필을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="0b58e-175">필요한 변경을 수행 하 고 선택한 **제출**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="0b58e-176">이 프로필을 삭제 하려면 선택 **프로필을 삭제** 페이지의 오른쪽 위 모서리에서.</span><span class="sxs-lookup"><span data-stu-id="0b58e-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="0b58e-177">고객의 계정에 장치 추가</span><span class="sxs-lookup"><span data-stu-id="0b58e-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="0b58e-178">영업 에이전트와 관리 에이전트 고객 계정에 장치를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="0b58e-179">고객의 장치에 사용자 지정 Autopilot 프로필을 적용할 수 있습니다, 전에 고객의 장치 목록에 액세스할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="0b58e-180">OEM 이름, 일련 번호 및 모델 조합 사용 하려는 경우 이러한 제한 사항을 고려해 야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="0b58e-181">최신 장치 (4 k 해시, 예를 들어)에 대해서만이 튜플 작동 128b 해시 (RS2 및 이전 장치)에 대 한 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="0b58e-182">파일의 데이터 모델과 제조업체 이름과 일치 해야 하므로 튜플 등록은 대 소문자를 구분 ***정확 하 게*** OEM 공급자 (하드웨어 공급자)에서 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="0b58e-183">파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="0b58e-184">선택 **고객** 파트너 센터 메뉴와 해당 장치를 관리 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="0b58e-185">고객의 세부 정보 페이지에서 선택 **장치**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0b58e-186">아래 **프로필을 장치에 적용할** 선택 **장치 추가**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="0b58e-187">장치 목록에 대 한 이름을 입력 하 고 선택한 **찾아보기** 파트너 센터 고객 목록 (.csv 파일 형식)를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="0b58e-188">장치 구매를 사용 하 여이.csv 파일을 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="0b58e-189">.Csv 파일을 받지 않은 경우 만들면 직접의 단계를 수행 하 여 [Windows Autopilot 장치 추가](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="0b58e-190">.Csv 파일을 업로드 하 고 선택한 **저장할**합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="0b58e-191">.Csv 파일을 업로드 하는 동안 오류 메시지를 받게 되 면 파일의 형식을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="0b58e-192">전용 하드웨어 해시 또는 OEM 이름, 일련 번호 및 순서로 해당 열을 모델 또는 Windows 제품 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="0b58e-193">옆의 링크에서 제공 된 샘플.csv 파일을 사용할 수도 있습니다 **장치 추가** 장치 목록을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="0b58e-194">Windows Autopilot EULA 사건</span><span class="sxs-lookup"><span data-stu-id="0b58e-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="0b58e-195">중요 한 정보</span><span class="sxs-lookup"><span data-stu-id="0b58e-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="0b58e-196">Windows Autopilot을 사용 하면 고객에 게 관리 하는 장치에서 Windows의 사용자 지정된 설치를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="0b58e-197">이렇게 하려면 고객에 의해 권한이 부여 된, 표시 하지 않을 수도 있고 EULA (최종 사용자 사용권 계약) 동의 화면을 포함 하 여 Windows를 설정할 때 사용자에 게 일반적으로 표시 되는 특정 설정 화면을 숨길 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="0b58e-198">이 함수를 사용 하 여 한다는 데 동의 억제 또는 공지 또는 충분 한 동 및 권한 부여 대신 용어 및 해당 사용자를 숨기려면 고객 으로부터 얻은 용어 의미에 대 한 동의 사용 하 여 사용자에 게 제공 하도록 설계 된 모든 화면 숨기기 (여부 조직 또는 개별 사용자의 경우 일 수 있음)를 고객은 알림 메시지에 동의 받고 모든 고객에 게 적용 되는 용어입니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="0b58e-199">여기에는 이 도구를 사용하여 표시하거나 숨기지 않는 경우, 사용자에게 제시되는 라이선스 약관 또는 고지에 대한 동의가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="0b58e-200">귀하의 고객이 Microsoft 또는 사용권이 허용된 배포자로부터 유효하게 소프트웨어 라이선스를 취득하지 않은 경우, 고객은 이러한 장치에서 Windows 소프트웨어를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0b58e-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>