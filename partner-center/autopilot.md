---
title: 장치의 기본 제공 환경 사용자 지정
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 고객의 새 장치를 제공 하기 전에 Windows Autopilot 프로필을 사용 하 여 장치의 OOBE (기본 제공 경험)를 사용자 지정 하거나 미리 구성할 수 있습니다.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534995"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="2d797-103">새 디바이스에서 Windows Autopilot 프로필을 사용하여 고객의 기본 환경을 사용자 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="2d797-104">**적절한 역할**</span><span class="sxs-lookup"><span data-stu-id="2d797-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2d797-105">관리 에이전트</span><span class="sxs-lookup"><span data-stu-id="2d797-105">Admin agent</span></span>
- <span data-ttu-id="2d797-106">글로벌 관리자</span><span class="sxs-lookup"><span data-stu-id="2d797-106">Global admin</span></span>
- <span data-ttu-id="2d797-107">영업 상담원</span><span class="sxs-lookup"><span data-stu-id="2d797-107">Sales agent</span></span>
- <span data-ttu-id="2d797-108">사용자 관리 담당자</span><span class="sxs-lookup"><span data-stu-id="2d797-108">User management admin</span></span>

<span data-ttu-id="2d797-109">고객 장치를 관리 하는 경우 고객의 사용자에 대 한 OOBE (기본 경험)를 사용자 지정 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="2d797-110">장치를 고객에 게 배달 하기 전에 Windows Autopilot 프로필을 사용 하 여 새 장치를 미리 구성 하 고 고객이 이미 구매한 장치에 새 프로필을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="2d797-111">Oem은 장치의 **제품 키 id (pkid)** 를 표시 하는 Autopilot 장치 상자 외부에 배송 레이블을 포함 하기 시작 했습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="2d797-112">이 1 차원, 읽을 수 있는 바코드는 장치를 unbox 하 고 다른 방법으로 장치 ID를 수집 하지 않고도 Autopilot에 대 한 장치를 등록 하는 방법을 제공 하는 다운스트림 파트너를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="2d797-113">이 문서에서는 파트너 센터에서 장치에 Autopilot 프로필을 만들고 적용 하는 방법을 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="2d797-114">Autopilot에 익숙하지 않은 경우 다음 문서의 정보를 검토 하세요.</span><span class="sxs-lookup"><span data-stu-id="2d797-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="2d797-115">Windows Autopilot 개요</span><span class="sxs-lookup"><span data-stu-id="2d797-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="2d797-116">Autopilot 배포 참조 가이드</span><span class="sxs-lookup"><span data-stu-id="2d797-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="2d797-117">개요</span><span class="sxs-lookup"><span data-stu-id="2d797-117">Overview</span></span>

<span data-ttu-id="2d797-118">파트너 센터의 Windows Autopilot 기능을 사용 하면 고객 장치에 적용할 사용자 지정 프로필을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="2d797-119">이 문서를 게시할 때 다음 프로필 설정을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="2d797-120">개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="2d797-120">Skip privacy settings.</span></span> <span data-ttu-id="2d797-121">이 선택적 Autopilot 프로필 설정을 사용 하면 조직에서 OOBE 프로세스 중 개인 정보 설정에 대해 질문할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="2d797-122">장치에서 로컬 관리자 계정 만들기를 사용 하지 않도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="2d797-123">조직에서는 프로세스가 완료 된 후 장치를 설정 하는 사용자에 게 관리자 권한이 있는지 여부를 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="2d797-124">회사 또는 학교에 대 한 장치를 자동으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="2d797-125">Autopilot에 등록 된 모든 장치는 회사 또는 학교 장치로 자동으로 간주 되므로이 질문은 OOBE 프로세스 중에 묻지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="2d797-126">Cortana, OneDrive 및 OEM 등록 설정 페이지를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="2d797-127">Autopilot에 등록 된 모든 장치는 OOBE (기본 경험) 프로세스 중에 이러한 페이지를 자동으로 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="2d797-128">EULA (최종 사용자 사용권 계약)를 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="2d797-129">Windows 10 버전 1709부터 조직은 OOBE 프로세스 중에 제공 된 EULA 페이지를 건너뛰도록 결정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="2d797-130">Windows 설치 중에 EULA 페이지를 건너뛰는 방법에 대해 고려해 야 하는 중요 한 정보는 [Windows AUTOPILOT EULA 해제](#windows-autopilot-eula-dismissal) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2d797-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="2d797-131">다음 프로필 및 디바이스 관리 사용 권한 및 제한이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="2d797-132">CSP 파트너는 고객이 파트너의 위임된 관리 권한을 제거한 경우에도 재판매인 관계가 있는 기존 고객에 대해 Autopilot 프로필을 계속 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="2d797-133">추가한 고객에 대한 기존 디바이스를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="2d797-134">고객이 비즈니스용 Microsoft Store 또는 Microsoft Intune 포털에 업로드한 디바이스를 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="2d797-135">파트너 센터에서 Autopilot 프로필 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="2d797-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="2d797-136">파트너 센터에서 Windows Autopilot 배포 프로필을 만들어 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="2d797-137">관리자 에이전트만 프로필을 만들고 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="2d797-138">새 Autopilot 프로필 만들기</span><span class="sxs-lookup"><span data-stu-id="2d797-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="2d797-139">파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만들 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="2d797-140">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2d797-141">**Windows Autopilot 프로필** 에서 **추가 새 프로필** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="2d797-142">프로필의 이름과 설명을 입력 하 고 OOBE 설정을 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="2d797-143">다음 중에서 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-143">Choose from:</span></span>  

   - <span data-ttu-id="2d797-144">설치에서 개인 정보 설정 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="2d797-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="2d797-145">설치 프로그램에서 로컬 관리자 계정 사용 안 함</span><span class="sxs-lookup"><span data-stu-id="2d797-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="2d797-146">설치 프로그램에서 자동으로 페이지 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="2d797-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="2d797-147">( *회사 또는 학교에 대 한 설치를 자동으로 선택* 하 고 *Cortana, OneDrive 및 OEM 등록 설정 페이지 건너뛰기*)</span><span class="sxs-lookup"><span data-stu-id="2d797-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="2d797-148">EULA (최종 사용자 사용권 계약) 건너뛰기</span><span class="sxs-lookup"><span data-stu-id="2d797-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="2d797-149">Windows 설치 중에 EULA 페이지를 건너뛰는 방법에 대해 고려해 야 하는 중요 한 정보는 [Windows AUTOPILOT EULA 해제](#windows-autopilot-eula-dismissal) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2d797-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="2d797-150">완료 되 면 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="2d797-151">고객 장치에 Autopilot 프로필 적용</span><span class="sxs-lookup"><span data-stu-id="2d797-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="2d797-152">아래 지침에서는 고객의 장치를 파트너 센터에 이미 추가 했 고 해당 장치 목록에 액세스할 수 있다고 가정 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="2d797-153">고객의 장치를 아직 추가 하지 않은 경우 [고객 계정에 장치 추가](#add-devices-to-a-customers-account) 의 지침에 따라 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="2d797-154">고객에 대 한 Autopilot 프로필을 만든 후 고객의 장치에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="2d797-155">파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만든 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2d797-156">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2d797-157">**장치에 프로필 적용** 에서 프로필을 추가할 장치 또는 장치 그룹을 선택 하 고 **프로필 적용** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="2d797-158">방금 적용 한 프로필이 **프로필** 열에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="2d797-159">아래 단계에 따라 프로필이 장치에 성공적으로 적용 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="2d797-160">a.</span><span class="sxs-lookup"><span data-stu-id="2d797-160">a.</span></span>  <span data-ttu-id="2d797-161">장치를 네트워크에 연결 하 고 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="2d797-162">b.</span><span class="sxs-lookup"><span data-stu-id="2d797-162">b.</span></span>  <span data-ttu-id="2d797-163">적절 한 OOBE 화면 (있는 경우)이 표시 되는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="2d797-164">다.</span><span class="sxs-lookup"><span data-stu-id="2d797-164">c.</span></span>  <span data-ttu-id="2d797-165">OOBE 프로세스가 중지 되 면 장치를 공장 기본 설정으로 다시 설정 하 여 새 사용자에 대해 준비 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="2d797-166">고객의 장치에서 Autopilot 프로필 제거</span><span class="sxs-lookup"><span data-stu-id="2d797-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="2d797-167">파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 만든 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2d797-168">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2d797-169">**장치에 프로필 적용** 에서 프로필을 제거 하려는 장치를 선택 하 고 **프로필 제거** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="2d797-170">장치에서 프로필을 제거 해도 해당 프로필은 목록에서 삭제 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="2d797-171">프로필을 삭제 하려면 [Autopilot 프로필 업데이트 또는 삭제](#update-or-delete-an-autopilot-profile)의 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="2d797-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="2d797-172">Autopilot 프로필 업데이트 또는 삭제</span><span class="sxs-lookup"><span data-stu-id="2d797-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="2d797-173">고객이 장치를 배송 한 후 기본 경험을 변경 하려는 경우 파트너 센터에서 프로필을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="2d797-174">고객의 장치가 인터넷에 연결 되 면 OOBE 프로세스 중에 최신 프로필 버전이 다운로드 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="2d797-175">또한 고객이 공장 기본 설정으로 장치를 복원할 때마다 장치는 OOBE 프로세스 중에 최신 프로필 버전을 다시 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="2d797-176">파트너 센터 메뉴에서 **고객** 을 선택한 다음 Autopilot 프로필을 변경 하려는 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="2d797-177">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2d797-178">**Windows Autopilot 프로필** 아래에서 업데이트 해야 하는 프로필을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="2d797-179">필요한 변경 작업을 수행한 다음 **제출** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="2d797-180">이 프로필을 삭제 하려면 페이지의 오른쪽 위 모서리에서 **프로필 삭제** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="2d797-181">고객 계정에 디바이스 추가</span><span class="sxs-lookup"><span data-stu-id="2d797-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="2d797-182">판매 에이전트 및 관리 에이전트는 고객의 계정에 장치를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="2d797-183">사용자 지정 Autopilot 프로필을 고객 장치에 적용 하려면 먼저 고객의 장치 목록에 액세스할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="2d797-184">OEM 이름, 일련 번호 및 모델 조합을 사용할 계획인 경우 다음 제한 사항에 유의 하세요.</span><span class="sxs-lookup"><span data-stu-id="2d797-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="2d797-185">이 튜플은 최신 장치 (예: 4k 해시)에 대해서만 작동 하며, 128b 해시 (RS2 및 이전 장치)에 대해서는 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="2d797-186">튜플 등록은 대/소문자를 구분 하므로 파일의 데이터는 OEM 공급자 (하드웨어 공급자)에서 제공 하는 모델 및 제조업체 이름과 *_정확히_* 일치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="2d797-187">파트너 센터에서 고객의 계정에 장치를 추가 하려면 아래 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="2d797-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="2d797-188">파트너 센터 메뉴에서 _ \*고객\*\*을 선택 하 고 관리 하려는 장치를 가진 고객을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="2d797-189">고객 세부 정보 페이지에서 **장치** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2d797-190">**장치에 프로필 적용** 에서 **장치 추가** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="2d797-191">장치 목록에 대 한 이름을 입력 하 고 **찾아보기** 를 선택 하 여 고객 목록 (.csv 파일 형식)을 파트너 센터에 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2d797-192">장치를 구입 하 여이 .csv 파일을 수신 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="2d797-193">.Csv 파일을 받지 못한 경우 [Windows Autopilot에 장치 추가](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)의 단계를 수행 하 여 직접 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="2d797-194">.Csv 파일을 업로드 하 고 **저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="2d797-195">.csv 파일을 업로드하는 동안 오류 메시지가 나타나면 파일의 형식을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="2d797-196">하드웨어 해시만 사용하거나 OEM 이름, 일련 번호 및 모델(해당 열 순서로) 또는 Windows 제품 ID를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="2d797-197">장치 **추가** 옆에 있는 링크에서 제공 된 샘플 .csv 파일을 사용 하 여 장치 목록을 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="2d797-198">.Csv 파일의 모양은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="2d797-199">**장치 일련 번호, Windows 제품 ID, 하드웨어 해시, 제조업체 이름, 장치 모델**</span><span class="sxs-lookup"><span data-stu-id="2d797-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="2d797-200">**{,,,) Microsoft Corporation, Surface 노트북**</span><span class="sxs-lookup"><span data-stu-id="2d797-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="2d797-201">"제조업체 이름" 및 "장치 모델"은 대/소문자를 구분 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="2d797-202">제조업체 이름 및 장치 모델에 넣을 값을 모르는 경우 장치에서이를 실행 하 여 올바른 값을 수집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="2d797-203">Windows Autopilot EULA 해제</span><span class="sxs-lookup"><span data-stu-id="2d797-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="2d797-204">중요 정보</span><span class="sxs-lookup"><span data-stu-id="2d797-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="2d797-205">Windows Autopilot를 사용 하면 고객을 위해 관리 하는 장치에서 Windows의 사용자 지정 설치를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="2d797-206">고객이이 작업을 수행할 수 있는 권한이 있는 경우 EULA (최종 사용자 사용권 계약) 승인 화면을 비롯 한 Windows를 설정할 때 일반적으로 사용자에 게 표시 되는 특정 설정 화면을 표시 하거나 숨길 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="2d797-207">이 함수를 사용 하 여 사용자에 게 통지를 제공 하거나 약관에 동의 하도록 디자인 된 화면을 표시 하거나 숨기는 것은 사용자에 게 약관을 숨길 수 있는 충분 한 동의 및 권한 부여를 제공 하는 것을 의미 하 고, 고객을 대신 하 여 (조직이 나 개별 사용자가 될 수 있는지 여부에 관계 없이) 고객에 게 동의 하 고 고객에 게 적용 되는 모든 약관을 수락</span><span class="sxs-lookup"><span data-stu-id="2d797-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="2d797-208">여기에는이 도구를 사용 하 여 표시 하거나 숨기는 경우 사용자에 게 표시 되는 사용권 계약 조건에 대 한 계약이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="2d797-209">고객이 Microsoft 또는 라이선스 대리점에서 소프트웨어에 대 한 라이선스를 합법적으로 취득 하지 않은 경우 고객이 해당 장치에서 Windows 소프트웨어를 사용 하지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d797-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>