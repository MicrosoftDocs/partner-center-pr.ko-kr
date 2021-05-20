---
title: 디바이스의 첫 번째 환경 사용자 지정
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객의 새 디바이스를 제공하기 전에 Windows Autopilot 프로필을 사용하여 디바이스의 OOBE(첫 번째 환경)를 사용자 지정하거나 미리 구성할 수 있습니다.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149828"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="111b7-103">새 디바이스에서 Windows Autopilot 프로필을 사용하여 고객의 기본 환경을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="111b7-104">**적절한 역할:** 관리 에이전트 | 전역 관리자 | 영업 에이전트 | 사용자 관리 관리자</span><span class="sxs-lookup"><span data-stu-id="111b7-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="111b7-105">고객 디바이스를 관리하는 경우 고객 사용자를 위해 OOBE(첫 경험)를 사용자 지정해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="111b7-106">고객에게 디바이스를 전달하기 전에 Windows Autopilot 프로필을 사용하여 새 디바이스를 미리 구성하고 고객이 이미 구매한 디바이스에 새 프로필을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="111b7-107">OEM은 디바이스의 **PKID(제품 키 ID)를** 표시하는 Autopilot 디바이스 상자 외부에 배송 레이블을 포함하기 시작했습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="111b7-108">이 1차원 읽을 수 있는 바코드는 다운스트림 파트너에게 디바이스의 unbox를 해제하고 대체 방법으로 디바이스 ID를 수집하지 않고도 Autopilot에 디바이스를 등록하는 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="111b7-109">이 문서에서는 파트너 센터 디바이스에 Autopilot 프로필을 만들고 적용하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="111b7-110">Autopilot에 익숙하지 않은 경우 다음 문서의 정보를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="111b7-111">Windows Autopilot 개요</span><span class="sxs-lookup"><span data-stu-id="111b7-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="111b7-112">Autopilot 배포 참조 가이드</span><span class="sxs-lookup"><span data-stu-id="111b7-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="111b7-113">개요</span><span class="sxs-lookup"><span data-stu-id="111b7-113">Overview</span></span>

<span data-ttu-id="111b7-114">파트너 센터 Windows Autopilot 기능을 사용하면 고객 디바이스에 적용할 사용자 지정 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="111b7-115">이 문서가 게시되었을 때 사용할 수 있는 프로필 설정은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="111b7-116">개인 정보 설정을 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-116">Skip privacy settings.</span></span> <span data-ttu-id="111b7-117">이 선택적 Autopilot 프로필 설정을 사용하면 조직에서 OOBE 프로세스 중에 개인 정보 설정에 대해 묻지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="111b7-118">디바이스에서 로컬 관리자 계정 만들기를 사용하지 않도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="111b7-119">조직은 프로세스가 완료되면 디바이스를 설정하는 사용자에게 관리자 액세스 권한이 있어야 하는지 여부를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="111b7-120">직장 또는 학교용 디바이스를 자동으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="111b7-121">Autopilot에 등록된 모든 디바이스는 자동으로 직장 또는 학교 디바이스로 간주되므로 OOBE 프로세스 중에 이 질문을 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="111b7-122">Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="111b7-123">Autopilot에 등록 된 모든 장치는 OOBE (기본 경험) 프로세스 중에 이러한 페이지를 자동으로 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="111b7-124">EULA (최종 사용자 사용권 계약)를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="111b7-125">Windows 10 버전 1709부터 조직은 OOBE 프로세스 중에 제공 된 EULA 페이지를 건너뛰도록 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="111b7-126">Windows 설치 중에 EULA 페이지를 건너뛰는 방법에 대해 고려해 야 하는 중요 한 정보는 [Windows AUTOPILOT EULA 해제](#windows-autopilot-eula-dismissal) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="111b7-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="111b7-127">다음 프로필 및 디바이스 관리 사용 권한 및 제한이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="111b7-128">CSP 파트너는 고객이 파트너의 위임된 관리 권한을 제거한 경우에도 재판매인 관계가 있는 기존 고객에 대해 Autopilot 프로필을 계속 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="111b7-129">추가한 고객에 대한 기존 디바이스를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="111b7-130">고객이 비즈니스용 Microsoft Store 또는 Microsoft Intune 포털에 업로드한 디바이스를 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="111b7-131">파트너 센터에서 Autopilot 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="111b7-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="111b7-132">파트너 센터에서 Windows Autopilot 배포 프로필을 만들어 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="111b7-133">관리자 에이전트만 프로필을 만들고 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="111b7-134">새 Autopilot 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="111b7-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="111b7-135">파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만들 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="111b7-136">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="111b7-137">**Windows Autopilot 프로필** 에서 **추가 새 프로필** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="111b7-138">프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="111b7-139">다음 중에서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-139">Choose from:</span></span>  

   - <span data-ttu-id="111b7-140">설치에서 개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="111b7-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="111b7-141">설치 프로그램에서 로컬 관리자 계정 사용 안 함</span><span class="sxs-lookup"><span data-stu-id="111b7-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="111b7-142">설치 프로그램에서 자동으로 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="111b7-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="111b7-143">( *회사 또는 학교에 대 한 설치를 자동으로 선택* 하 고 *Cortana, OneDrive 및 OEM 등록 설정 페이지 건너뛰기*)</span><span class="sxs-lookup"><span data-stu-id="111b7-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="111b7-144">EULA (최종 사용자 사용권 계약) 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="111b7-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="111b7-145">Windows 설치 중에 EULA 페이지를 건너뛰는 방법에 대해 고려해 야 하는 중요 한 정보는 [Windows AUTOPILOT EULA 해제](#windows-autopilot-eula-dismissal) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="111b7-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="111b7-146">완료 되 면 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="111b7-147">고객 장치에 Autopilot 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="111b7-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="111b7-148">아래 지침에서는 파트너 센터 고객의 디바이스를 이미 추가했으며 해당 디바이스 목록에 액세스할 수 있다고 가정합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="111b7-149">고객의 디바이스를 아직 추가하지 않은 경우 고객 계정에 [디바이스 추가의 지침에](#add-devices-to-a-customers-account) 따라 아래 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="111b7-150">고객에 대한 Autopilot 프로필을 만든 후 고객의 디바이스에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="111b7-151">파트너 센터 메뉴에서 **고객을** 선택한 다음, Autopilot 프로필을 만든 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="111b7-152">고객의 세부 정보 페이지에서 **디바이스를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="111b7-153">**디바이스에 프로필 적용에서 프로필을** 추가할 디바이스 또는 디바이스 그룹을 선택한 **다음, 프로필 적용을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="111b7-154">방금 적용한 프로필이 **프로필** 열에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="111b7-155">아래 단계에 따라 프로필이 디바이스에 성공적으로 적용되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="111b7-156">a.</span><span class="sxs-lookup"><span data-stu-id="111b7-156">a.</span></span>  <span data-ttu-id="111b7-157">디바이스를 네트워크에 연결하고 켭니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="111b7-158">b.</span><span class="sxs-lookup"><span data-stu-id="111b7-158">b.</span></span>  <span data-ttu-id="111b7-159">적절한 OOBE 화면(있는 경우)이 표시되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="111b7-160">다.</span><span class="sxs-lookup"><span data-stu-id="111b7-160">c.</span></span>  <span data-ttu-id="111b7-161">OOBE 프로세스가 중지되면 디바이스를 공장 기본 설정으로 다시 설정하여 새 사용자를 위해 준비합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="111b7-162">고객의 디바이스에서 Autopilot 프로필 제거</span><span class="sxs-lookup"><span data-stu-id="111b7-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="111b7-163">파트너 센터 메뉴에서 **고객을** 선택한 다음, Autopilot 프로필을 만든 고객을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="111b7-164">고객의 세부 정보 페이지에서 **디바이스를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="111b7-165">**디바이스에 프로필 적용에서 프로필을** 제거할 디바이스를 선택한 다음 **프로필 제거를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="111b7-166">디바이스에서 프로필을 제거해도 목록에서 프로필이 삭제되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="111b7-167">프로필을 삭제하려면 Autopilot 프로필 업데이트 [또는 삭제의](#update-or-delete-an-autopilot-profile)지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="111b7-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="111b7-168">Autopilot 프로필 업데이트 또는 삭제</span><span class="sxs-lookup"><span data-stu-id="111b7-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="111b7-169">디바이스를 배송한 후 고객이 첫 번째 환경을 변경하려는 경우 파트너 센터 프로필을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="111b7-170">고객의 디바이스가 인터넷에 연결되면 OOBE 프로세스 중에 최신 프로필 버전을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="111b7-171">또한 고객이 공장 기본 설정으로 장치를 복원할 때마다 장치는 OOBE 프로세스 중에 최신 프로필 버전을 다시 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="111b7-172">파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 변경 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="111b7-173">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="111b7-174">**Windows Autopilot 프로필** 아래에서 업데이트 해야 하는 프로필을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="111b7-175">필요한 변경 작업을 수행한 다음 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="111b7-176">이 프로필을 삭제 하려면 페이지의 오른쪽 위 모서리에서 **프로필 삭제** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="111b7-177">고객 계정에 디바이스 추가</span><span class="sxs-lookup"><span data-stu-id="111b7-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="111b7-178">판매 에이전트 및 관리 에이전트는 고객의 계정에 장치를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="111b7-179">사용자 지정 Autopilot 프로필을 고객 장치에 적용 하려면 먼저 고객의 장치 목록에 액세스할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="111b7-180">OEM 이름, 일련 번호 및 모델 조합을 사용할 계획인 경우 다음 제한 사항에 유의 하세요.</span><span class="sxs-lookup"><span data-stu-id="111b7-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="111b7-181">이 튜플은 최신 장치 (예: 4k 해시)에 대해서만 작동 하며, 128b 해시 (RS2 및 이전 장치)에 대해서는 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="111b7-182">튜플 등록은 대/소문자를 구분 하므로 파일의 데이터는 OEM 공급자 (하드웨어 공급자)에서 제공 하는 것과 ***정확 하 게*** 모델 및 제조업체 이름과 일치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="111b7-183">파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="111b7-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="111b7-184">파트너 센터 메뉴에서 **고객** 을 선택 하 고 관리할 장치를 포함 하는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="111b7-185">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="111b7-186">**장치에 프로필 적용** 에서 **장치 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="111b7-187">장치 목록에 대 한 이름을 입력 하 고 **찾아보기** 를 선택 하 여 고객 목록 (.csv 파일 형식)을 파트너 센터에 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="111b7-188">장치를 구입 하 여이 .csv 파일을 수신 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="111b7-189">.Csv 파일을 받지 못한 경우 [Windows Autopilot에 장치 추가](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)의 단계를 수행 하 여 직접 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="111b7-190">.Csv 파일을 업로드 하 고 **저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="111b7-191">.csv 파일을 업로드하는 동안 오류 메시지가 나타나면 파일의 형식을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="111b7-192">하드웨어 해시만 사용하거나 OEM 이름, 일련 번호 및 모델(해당 열 순서로) 또는 Windows 제품 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="111b7-193">**디바이스 추가** 옆에 있는 링크에서 제공된 샘플 .csv 파일을 사용하여 디바이스 목록을 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="111b7-194">.csv 파일은 다음과 같이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="111b7-195">**디바이스 일련 번호, Windows 제품 ID, 하드웨어 해시, 제조업체 이름, 디바이스 모델**</span><span class="sxs-lookup"><span data-stu-id="111b7-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="111b7-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="111b7-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="111b7-197">"제조업체 이름" 및 "디바이스 모델"은 대/소문자 구분입니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="111b7-198">제조업체 이름 및 디바이스 모델에 대해 어떤 값을 입력할지 모르는 경우 디바이스에서 이 값을 실행하여 올바른 값을 수집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="111b7-199">EULA Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="111b7-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="111b7-200">중요 정보</span><span class="sxs-lookup"><span data-stu-id="111b7-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="111b7-201">Windows Autopilot 사용하면 고객을 위해 관리하는 디바이스에서 사용자 지정된 Windows 설치를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="111b7-202">고객이 이 작업을 수행할 수 있는 권한이 있는 경우 EULA(최종 사용자 사용권 계약) 동의 화면을 포함하여 Windows를 설정할 때 일반적으로 사용자에게 제공된 특정 설정 화면을 표시하지 않거나 숨길 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="111b7-203">이 기능을 사용하면 사용자에게 약관에 대한 통지 또는 동의를 제공하도록 설계된 화면을 표시하지 않거나 숨기지 않는 것은 사용자가 약관을 숨기도록 고객으로부터 충분한 동의와 권한을 획득했으며, 귀하는 고객(조직 또는 개별 사용자와 관계없이)을 대신하여 통지에 동의하고 고객에게 적용되는 모든 약관에 동의한다는 데 동의합니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="111b7-204">여기에는 이 도구를 사용하여 표시하거나 숨기지 않은 경우 사용자에게 제공될 라이선스 사용 약관 또는 통지에 대한 계약이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="111b7-205">고객이 Microsoft 또는 사용이 허가된 배포자로부터 소프트웨어에 대한 라이선스를 유효하게 획득하지 않은 경우 고객은 해당 디바이스에서 Windows 소프트웨어를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="111b7-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>