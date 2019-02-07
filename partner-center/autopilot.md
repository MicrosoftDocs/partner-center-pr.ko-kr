---
title: Windows Autopilot 프로필을 사용 하 여 디바이스의 기본 제공 환경을 사용자 지정 | 파트너 센터
description: Autopilot 프로필을 사용 하 여 디바이스의 기본 제공 경험 미리 구성 합니다.
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot, windows autopilot, microsoft autopilot, 제로 터치 배포, oobe, 로그인 화면, 기본 제공
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062281"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="0e374-104">Windows Autopilot 프로필을 사용 하 여 디바이스의 기본 제공 환경을 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="0e374-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="0e374-105">적용 대상</span><span class="sxs-lookup"><span data-stu-id="0e374-105">Applies to</span></span>**

- <span data-ttu-id="0e374-106">CSP 직접 청구서 파트너, 간접 공급자와 간접 재판매인</span><span class="sxs-lookup"><span data-stu-id="0e374-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="0e374-107">고객 장치를 관리 하는 경우 고객의 사용자에 대 한 기본 제공 경험 (OOBE)을 사용자 지정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="0e374-108">고객에 게 장치를 전달 하기 전에 Windows Autopilot 프로필을 사용 하 여 새 장치를 미리 구성 하 고 이미 구매한 고객 장치에 새 프로필을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="0e374-109">이 문서에서는 만들고 파트너 센터에서 장치에 Autopilot 프로필을 적용 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="0e374-110">수 없는 경우 이미 익숙한 autopilot,이 문서의 정보를 검토:</span><span class="sxs-lookup"><span data-stu-id="0e374-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="0e374-111">Windows Autopilot 개요</span><span class="sxs-lookup"><span data-stu-id="0e374-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="0e374-112">Autopilot 배포 참조 가이드</span><span class="sxs-lookup"><span data-stu-id="0e374-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="0e374-113">개요</span><span class="sxs-lookup"><span data-stu-id="0e374-113">Overview</span></span>

<span data-ttu-id="0e374-114">파트너 센터에서 Windows Autopilot 기능을 사용 하 여 고객 장치에 적용할 사용자 지정 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="0e374-115">이 문서가 게시 시간에 다음 프로필 설정을 사용할 수 있게 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="0e374-116">개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0e374-116">Skip privacy settings.</span></span> <span data-ttu-id="0e374-117">이 선택적 Autopilot 프로필 설정을 통해 조직은 않을 OOBE 프로세스 동안 개인 정보 설정에 대 한 요청 하지 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="0e374-118">장치에 로컬 관리자 계정 만들기를 사용 하지 않도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="0e374-119">조직은은 프로세스가 완료 되 면 장치를 설정 하는 사용자 관리자 액세스를 가져야 할지 여부를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="0e374-120">회사 또는 학교에 대 한 장치를 자동으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="0e374-121">Autopilot을 사용 하 여 등록 된 모든 장치 작업 자동으로 간주 됩니다 또는 학교 장치, 하므로 OOBE 프로세스 동안이 질문을 요청 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="0e374-122">Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="0e374-123">Autopilot을 사용 하 여 등록 된 모든 장치는 자동으로 아웃-첫 실행 경험 (OOBE) 동안 이러한 페이지를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="0e374-124">최종 사용자 사용권 계약 (EULA) 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0e374-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="0e374-125">Windows 10 버전 1709부터 조직은 OOBE 프로세스 도중 EULA 페이지를 건너뛸 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="0e374-126">[Windows Autopilot EULA 철회](#windows-autopilot-eula-dismissal) 아래 중요 한 정보에 대 한 Windows 설치 시 EULA 페이지 건너뛰기에 대 한 고려를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="0e374-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="0e374-127">다음 프로필 및 장치 관리 권한 및 제한 사항이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="0e374-128">CSP 파트너 계속 파트너의 위임 된 관리 권한을 제거한 경우에 재판매인 관계에 있는 기존 고객을 위해 Autopilot 프로필을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="0e374-129">사용자 또는 다른 CSP 파트너가 추가한 고객을 위해 기존 장치를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="0e374-130">고객은 비즈니스용 Microsoft 스토어 또는 Microsoft Intune 포털에 업로드 한 장치를 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="0e374-131">만들기 및 파트너 센터에서 Autopilot 프로필 관리</span><span class="sxs-lookup"><span data-stu-id="0e374-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="0e374-132">파트너 센터에서 Windows Autopilot 배포 프로필을 만들 수 있으며 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="0e374-133">관리자 에이전트만 만들고 프로필을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="0e374-134">새 Autopilot 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="0e374-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="0e374-135">파트너 센터 메뉴에서 **고객** 을 선택 하 고 Autopilot 프로필을 만드는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="0e374-136">고객의 세부 정보 페이지에서 **장치**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0e374-137">**Windows Autopilot 프로필** 에서 **새 프로필 추가**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="0e374-138">프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="0e374-139">선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-139">Choose from:</span></span>  

   - <span data-ttu-id="0e374-140">설정의 개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0e374-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="0e374-141">설치 시 로컬 관리자 계정 비활성화</span><span class="sxs-lookup"><span data-stu-id="0e374-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="0e374-142">설치 시 자동으로 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0e374-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="0e374-143">( *자동으로 회사 또는 학교 설치 선택* 및 *건너뛰기 Cortana, OneDrive 및 OEM 등록 설정 페이지*포함)</span><span class="sxs-lookup"><span data-stu-id="0e374-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="0e374-144">최종 사용자 사용권 계약 (EULA) 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="0e374-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="0e374-145">[Windows Autopilot EULA 철회](#windows-autopilot-eula-dismissal) 아래 중요 한 정보에 대 한 Windows 설치 시 EULA 페이지 건너뛰기에 대 한 고려를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="0e374-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="0e374-146">작업을 마쳤으면 **제출**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="0e374-147">고객 장치에 Autopilot 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="0e374-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="0e374-148">다음 지침을 이미 추가한 고객의 디바이스 파트너 센터로 자신의 장치 목록에 액세스할 수 있는지 가정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="0e374-149">고객의 장치를 추가 하지 않은 경우 [고객의 계정에 추가 디바이스](#add-devices-to-a-customers-account) 의 지침에 따라 한 다음 아래 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="0e374-150">고객의 Autopilot 프로필을 만든 후에 고객의 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="0e374-151">파트너 센터 메뉴에서 **고객** 을 선택 하 고 만든 Autopilot 프로필에 대 한 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="0e374-152">고객의 세부 정보 페이지에서 **장치**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0e374-153">**장치에 적용 프로필** 에서 장치나 프로필을 추가 하 고 다음 **적용 프로필**을 선택 하 고 싶은 장치 그룹을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="0e374-154">방금 적용 프로필 **프로필** 열에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="0e374-155">프로필 적용 됨을 성공적으로 장치를 확인 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="0e374-156">a.</span><span class="sxs-lookup"><span data-stu-id="0e374-156">a.</span></span>  <span data-ttu-id="0e374-157">네트워크에 장치를 연결 하 고 켭니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="0e374-158">b.</span><span class="sxs-lookup"><span data-stu-id="0e374-158">b.</span></span>  <span data-ttu-id="0e374-159">적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="0e374-160">c.</span><span class="sxs-lookup"><span data-stu-id="0e374-160">c.</span></span>  <span data-ttu-id="0e374-161">OOBE 프로세스를 중지 하면 새 사용자를 위한 준비를 공장 기본 설정에 디바이스를 초기화 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="0e374-162">고객의 장치에서 Autopilot 프로필 제거</span><span class="sxs-lookup"><span data-stu-id="0e374-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="0e374-163">파트너 센터 메뉴에서 **고객** 을 선택 하 고 만든 Autopilot 프로필에 대 한 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="0e374-164">고객의 세부 정보 페이지에서 **장치**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0e374-165">**장치에 적용 프로필** 에서 프로필을 제거 하 고 선택한 다음 **프로필 제거**하려는 디바이스를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="0e374-166">장치에서 프로필을 제거 해도 목록에서 프로필을 삭제 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="0e374-167">프로필을 삭제 하려는 경우 [업데이트 또는 삭제 Autopilot 프로필의](#update-or-delete-an-autopilot-profile)지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="0e374-168">업데이트 또는 Autopilot 프로필을 삭제 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="0e374-169">고객이 장치에 제공한 후 기본 제공 경험을 변경 하는 경우 파트너 센터에서 프로필을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="0e374-170">고객의 장치가 인터넷에 연결 하는 경우 OOBE 프로세스 동안 최신 프로필 버전을 다운로드 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="0e374-171">또한 고객이 디바이스를 공장 기본 설정, 복원 언제 든 지 장치를 다시 최신 버전을 다운로드 프로필 OOBE 프로세스 동안 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="0e374-172">파트너 센터 메뉴에서 **고객** 을 선택 하 고 Autopilot 프로필을 변경할 수를 원하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="0e374-173">고객의 세부 정보 페이지에서 **장치**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0e374-174">**Windows Autopilot 프로필** 에서 업데이트 해야 하는 프로필을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="0e374-175">필요한 사항을 변경 하 고 **제출**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="0e374-176">이 프로필을 삭제 하려면 페이지의 오른쪽 위 모서리에서 **프로필 삭제** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="0e374-177">고객의 계정에 장치를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="0e374-178">영업 에이전트와 관리자 에이전트는 고객의 계정에 디바이스를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="0e374-179">고객 장치에 사용자 지정 Autopilot 프로필을 적용 하려면, 먼저 고객의 장치 목록에 액세스할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="0e374-180">OEM 이름, 일련 번호 및 모델 조합을 사용 하려는 경우 이러한 제한 사항을 고려해 야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="0e374-181">최신 장치 (4 k 해시, 예:)에 대해서만이 튜플 작동 128b 해시 (RS2 및 이전 장치)에 대 한 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="0e374-182">튜플 등록 대/소문자를 구분 이므로 OEM 공급자 (하드웨어 공급자)가 제공한 파일의 데이터는 제조업체 및 모델 이름을 ***정확히*** 일치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="0e374-183">파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="0e374-184">파트너 센터 메뉴에서 **고객** 을 선택 하 고 해당 장치를 관리 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="0e374-185">고객의 세부 정보 페이지에서 **장치**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0e374-186">**장치에 적용 프로필** 에서 **추가 장치**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="0e374-187">장치 목록에 대 한 이름을 입력 하 고 (.csv 파일 형식)의 고객의 목록을 파트너 센터에 업로드할 **찾아보기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="0e374-188">장치 구입이.csv 파일을 받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="0e374-189">.Csv 파일을 받은 후 하지 않은 경우에 [추가 Windows Autopilot 장치](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)에 단계에 따라 직접 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="0e374-190">.Csv 파일을 업로드 하 고 **저장**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="0e374-191">.Csv 파일을 업로드 하는 동안 오류 메시지가 나타나면 파일 형식을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="0e374-192">하드웨어 해시만 또는 OEM 이름, 일련 번호 및 모델 (순서로 열) 또는 Windows 제품 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="0e374-193">또한 장치 목록을 만드는 **추가 장치** 옆에 있는 링크에서 제공 되는 샘플.csv 파일을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="0e374-194">Windows Autopilot EULA 철회</span><span class="sxs-lookup"><span data-stu-id="0e374-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="0e374-195">중요 한 정보</span><span class="sxs-lookup"><span data-stu-id="0e374-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="0e374-196">Windows Autopilot을 사용 하면 고객에 게 관리 하는 장치에서 Windows의 사용자 지정 된 설치를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="0e374-197">고객이 이렇게 하려면 권한이 있으면 표시 안 함 하거나 일반적으로 EULA (최종 사용자 사용권 계약) 동의 화면 등 Windows를 설정할 때 사용자에 게 제시 되는 일부 설정 화면을 숨길 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="0e374-198">이 기능을 사용 함으로써 귀하는 표시 하지 않거나 숨기 고 지 또는 동의 용어 의미를 갖고 있는 충분 한 동 및 권한 부여 대신, 약관을 숨기기 고객 으로부터 사용자를 제공 하도록 고안 된 화면 (여부는 조직 또는 개별 사용자 경우에 따라 수 있음), 고객 지에 동의 하 고 수락 모든 고객에 게 적용 되는 약관 합니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="0e374-199">여기에는 이 도구를 사용하여 표시하거나 숨기지 않는 경우, 사용자에게 제시되는 라이선스 약관 또는 고지에 대한 동의가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="0e374-200">귀하의 고객이 Microsoft 또는 사용권이 허용된 배포자로부터 유효하게 소프트웨어 라이선스를 취득하지 않은 경우, 고객은 이러한 장치에서 Windows 소프트웨어를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0e374-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>