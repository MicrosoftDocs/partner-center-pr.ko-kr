---
title: Simplify device setup with Windows Autopilot | Partner Center
description: Add a Windows AutoPilot deployment profile in Partner Center to simplify device setup with Windows Autopilot
author: KPacquer
keywords: autopilot, windows autopilot, microsoft autopilot, zero-touch deployment, oobe, login screens
ms.openlocfilehash: 72cf8a8361a12c545501a452788d231f930c4928
ms.sourcegitcommit: d9f3e4e8115c0ad44f97041d352b703cda7ba9e5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/28/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>Simplify device setup with Windows Autopilot 

Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps. To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).

## <a name="features"></a>Features

*  **Disable local administrator permissions** for the end users setting up devices
*  **Show an organization's login page**. The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.
*  **Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.
*  **Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile. 

## <a name="requirements"></a>Requirements

*  Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later) or Windows 10 Pro for Advanced PCs.
*  Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM. You'll use identifiers to assign organization profiles in Partner Center. After September 2017 you will no longer need the hardware hash. 
*  The devices must have access to the internet. When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.
*  Enrolling the device into an MDM requires Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Add organization login pages to OOBE

To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Remove Windows pages from OOBE with a Windows AutoPilot deployment profile

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a>Examples of settings in a Windows AutoPilot deployment profile
*  Skip Privacy Settings in setup
*  Disable local admin account in setup
*  Automatically skip pages in setup
   *  Automatically select setup for work or school
   *  Skip Cortana, OneDrive, and OEM registration setup pages

### <a name="add-devices-and-apply-a-profile"></a>Add devices and apply a profile

In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.

To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.

1.  Add the list of devices into Partner Center.

    Sales agents and admin agents have access to add the list of devices into Partner Center.
    
    Indirect resellers can work with their indirect provider to add this.

    a.  Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot). This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier. 

    b.  From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.

    c.  Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.” 

    d.  Click **Browse** > select the device info file > **Validate**.

    **Note:** If you get an error message after trying to upload the .csv file, check the format of the file. After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID. You can also use the sample .csv file provided from the link next to **Add devices**.

2.  Create a profile that you can apply to the devices. (Only admin agents have access to create and apply profiles in Partner Center.)

    a.  From **Devices**, click **Add new profile**.

    b.  Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.

    c.  Configure the OOBE settings. For example, check **Skip Express Settings in setup**.

    d.  Click **Submit**.

3.  Apply the profile.

    a.  From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure. To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).

    b.  Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”). The devices will show the profile in the Profile column.

4.  Optional: Test to see that your profile works.

    a.  Connect a device to the network, and turn it on.

    b.  Verify that the appropriate OOBE screens (if any) appear.

    c.  To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.


## <a name="to-update-or-delete-a-profile"></a>To update or delete a profile 

Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer. When the device connects to the internet, it downloads the latest version of your profile during the OOBE process. If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile. 

### <a name="you-can-remove-a-profile-from-a-device"></a>You can remove a profile from a device
1. Select the device (or batch of devices) you want to remove the profile from. 

2. In **Assign and delete devices** pane, select **Remove profile**.

3. Go to the profile you want to remove and delete it. The profile will be deleted from all devices.

From **Devices**, select the profile. From here, you can modify the existing settings.

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Windows Autopilot EULA 철회 – 중요한 정보

이 도구를 사용하면 고객을 위해 관리하는 장치에서 Windows 개별 설치를 구성할 수 있습니다. 고객이 승인한 경우 EULA 동의 화면 등 Windows를 설정할 때 일반적으로 사용자에게 제시되는 일부 설정 화면을 표시하지 않거나 숨길 수 있습니다. 

이 기능을 사용함으로써 귀하는 약관의 고지 또는 동의를 사용자에게 제공하도록 고안된 화면을 표시하지 않거나 숨기는 데 동의합니다. 이는 약관을 숨기기 위해 고객으로부터 충분한 동의와 승인을 얻었으며 고객(경우에 따라 조직 또는 개별 사용자)을 대신하여 고지에 동의하고 고객에게 적용되는 약관에 동의함을 의미합니다. 여기에는 이 도구를 사용하여 표시하거나 숨기지 않는 경우, 사용자에게 제시되는 라이선스 약관 또는 고지에 대한 동의가 포함됩니다. 귀하의 고객이 Microsoft 또는 사용권이 허용된 배포자로부터 유효하게 소프트웨어 라이선스를 취득하지 않은 경우, 고객은 이러한 장치에서 Windows 소프트웨어를 사용할 수 없습니다.


