---
title: "Troubleshoot issues for the Power Apps mobile app | MicrosoftDocs"
description: Troubleshooting and known issues for the Power Apps mobile app 
author: mduelae
manager: kvivek
ms.service: powerapps
ms.component: pa-user
ms.topic: conceptual
ms.date: 04/28/2021
ms.author: mkaur
ms.custom: ""
ms.reviewer: ""
ms.assetid: 
search.audienceType: 
  - enduser
search.app: 
  - PowerApps
---

# Troubleshoot issues for Power Apps mobile app

This troubleshooting article helps fix common issues for the [Power Apps mobile app](../mobile/run-powerapps-on-mobile.md).

If you don't find the answer to your issue, then email us at [pamobsup@microsoft.com](mailto:pamobsup@microsoft.com?subject=Power%20Mobile%20issues) and include your device make and model, session ID, and provide the exact error message that you get.


## Unable to sign in on an Android device using Authenticator or Company Portal

There is an intermittent issue with Microsoft Authenticator app version 6.2104.2518 and Company Portal version 5.0.5123.0, which causes sign-in to fail with no error message in the Power Apps mobile app.

A fix will be released shortly. Regularly check the Authenticator app or the Company Portal mobile app for updates. Until then, try this workaround:

1.	Make sure you have a good internet connection.
2.	Wait for one minute and then try signing in again.

If you still can't sign in after several attempts, try launching your app in the web browser as a temporary solution until the Authenticator or Company Portal apps are updated.

## Unable to open an app

There is an intermittent issue with Microsoft Authenticator app version 6.2104.2518 and Company Portal version 5.0.5123.0, which prevents apps opening in the Power Apps mobile app.

A fix will be released shortly. Regularly check the Authenticator app or the Company Portal mobile app for updates. Until then, try this workaround:

1.	Make sure you have a good internet connection.
2.	Wait for one minute and then try opening the app again.

If you still can't open the app after several attempts, try launching your app in the web browser as a temporary solution until the Authenticator or Company Portal apps are updated.

## Error: There was a problem signing you in

You are unable to sign in due to issues with the Microsoft Authenticator app. 

If you don’t have the Microsoft Authenticator app, download the app from the App Store or Play Store and then sign in to Power Apps mobile again.

If you already have the Microsoft Authenticator app installed and you're having sign in issues, then try these steps:

1. Back up your Microsoft Authenticator account. For more information, see [Back up and recover account credentials using the Microsoft Authenticator app](/azure/active-directory/user-help/user-help-auth-app-backup-recovery)
2. Uninstall the Microsoft Authenticator app.
3. Uninstall Power Apps mobile.
4. Reinstall the Microsoft Authenticator app and add your back up account.
5. Reinstall [Power Apps mobile](../mobile/run-powerapps-on-mobile.md#install-power-apps-mobile-app).
6. Open Power Apps mobile and then sign in.


## Error: Your device configuration is preventing sign in

If you get this error messages, it means your company's IT department requires Microsoft Intune or an authentication app to sign in securely. However, your device setup is blocking Power Apps mobile from launching the authentication app that's installed on your device.

Microsoft authentication apps are Authenticator and Company Portal. Your company may use a third-party authentication app. If you're not sure, ask your IT department or help desk which authentication app to use. Once you have the correct authentication app, then follow the steps below.

 > [!NOTE]
 > Power Apps requires a valid license to sign in. For more information, see [Licensing overview](/power-platform/admin/pricing-billing-skus).

Sometimes, updating and manually opening the authentication app on your device before signing in to Power Apps mobile can fix the problem. If this doesn't fix the issue, then follow the next steps depending on your device manufacturer and authentication app. 

**Huawei or Honor device**

1. Go to **Settings** > **Battery** > **App launch**. 

    > [!NOTE]
    > The **App launch** menu can have different names depending on the model and the operating version of your mobile device. If you   don’t see the **App launch** menu option, then look for one of the following menu options:
    > - **Close apps after screen lock** 
    > - **Applications** 
    > - **Background applications**

2. Under **Manage automatically**, on the authenticator app set the toggle switch to **OFF**.
3. On the **Manage manually** screen ensure that **Secondary launch / Can be launched by other apps** is enabled. To allow the Power Apps mobile app to launch the app.

**Vivo device**

1. Go to **Settings** > **More Settings** > **Applications** > **Autostart**.
2. Set the toggle switch to **ON** for the authenticator app.

If the issue is still not fixed, then try these steps:

1. Back up your Microsoft Authenticator accounts. For more info, see [Back up and recover account credentials using the Microsoft Authenticator app](/azure/active-directory/user-help/user-help-auth-app-backup-recovery) 
2. Uninstall the Microsoft Authenticator app.
3. Uninstall Power Apps mobile.
4. Install Microsoft Authenticator again and add your back up accounts again.
5. Install [Power Apps mobile](../mobile/run-powerapps-on-mobile.md#install-power-apps-mobile-app).
6. Open Power Apps mobile and sign in.

If you still can't sign in, then email us at pamobsup@microsoft.com and include your device make and model, session ID, and provide the exact error message that you get.


## Pin to Home does not work on iOS 14

**iOS device running iOS 14**: The Safari browser no longer supports the **Pin to Home** functionality for Power Apps mobile. You need to use the Siri Shortcuts app to pin an app to the Home screen. For more information, see [Use Siri Shortcuts (iOS 14 or later)](../mobile/run-powerapps-on-mobile.md#use-siri-shortcuts-to-add-a-shortcut-to-the-home-screen-ios-14-or-later).

**iOS 13**: You can still use the Safari browser to pin an app to the Home screen. For more information, see [Pin an app to the home screen](../mobile/run-powerapps-on-mobile.md#use-safari-to-add-a-shortcut-ios-13-or-earlier)

## App list is empty

The app list in the Power Apps mobile app may appear empty when you lose internet connection before the app list has completely downloaded. This can happen in any of the following scenarios:

-	It's the first time you're signing in to the mobile app.
-	When you pull down to refresh the app list.
-	When you come back online after a period of being offline. The app list is automatically refreshed.

To resolve connection related issues, ensure you remain connected to the internet while the app list is fully downloaded.


### See also  

[Power Apps portals known issues](../maker/portals/known-issues.md) <br/>
[Power Automate known issues](/power-automate/process-advisor-issues)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
