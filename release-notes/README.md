---
description: Keep up to date with our releases!
---

# 📰 Release Notes

## September 28, 2022

Platform Updates

* Add ability to [copy and paste components](../ui-components.md#copy-and-paste-components) with hotkey commands
* Add pop-up to confirm deletion of large (7+) groups of blocks

## September 27, 2022

Platform Updates

* Upgrade to [Expo 45](https://blog.expo.dev/expo-sdk-45-f4e332954a68)
* [Android Download](../download.md#download-android-app), [Android Publish](../publish-to-play-store-android.md): Fix 'missing keystore' error

## September 24, 2022

Component Updates

* [Bluetooth Low Energy](../bluetooth-low-energy.md): fix permissions for Android 11 devices&#x20;

## September 22, 2022

Platform Updates

* Fix issue with signing in seen with new accounts
* [Android Download](../download.md#download-android-app), [Android Publish](../publish-to-play-store-android.md): Remove option to build Android apps with Android API 30 - all Android apps now built with Android API 31/targeting Android 12
* Web Preview: Hide blocks when previewing a read-only app
* Fix opening the project detail page

## September 16, 2022

Platform Updates

* Improve speed in snap-to-place projects

## September 13, 2022

Platform Updates

* [iOS Publish](../publish-to-app-store-ios/): Change how build numbers are generated

Component Updates

* [Data Sources](../data-sources.md): Improve updating display of data in Local Data Source when viewing project

## September 7, 2022

Platform Updates

* [Android download](../download.md#download-android-app), [Android publish](../publish-to-play-store-android.md): built Android apps will target Android API 31 by default

Component Updates

* [Speech blocks](../speech.md): restored Amharic option in language drop-down

## September 6, 2022

Platform Updates

* Improve quality of project backups

## September 3, 2022

Platform Updates

* Background updates to improve stability of platform

## August 30, 2022

Platform Updates

* Improve appearance of read-only projects
* Remove URL redirect for web apps
* Improve appearance of account icon in project view

Component Updates

* [Date Input](../date-input.md): improve positioning on web apps

## August 27, 2022

Platform Updates

* Frontend security update

## August 25, 2022

Platform Updates

* [Download Android](../download.md#download-android-app), [Publish Android](../publish-to-play-store-android.md): added option to build Android app to target Android API 31/Android 12
  * New apps to the Google Play Store must target at least Android API 31/Android 12
  * Updates to existing apps on the Google Play Store must target Android API 31/Android 12 from **November 1, 2022**
  * All existing apps on the Google Play Store must target Android API 31/Android 12 by **November 1, 2023**

## August 24, 2022

Platform Updates

* Infrastructure upgrades
* Increased frequency of project backups

Component Updates

* [AdMob](../admob.md): Improved error handling
* [Group](../group.md):  improved appearance of Button inside nested Groups



## August 17, 2022

Platform Updates

* Preparation for upgrading to React Navigation 5 with Expo 45
* Improve analytics for causes of projects not saving

## August 15, 2022

Platform Updates

* Fix issue with displaying assets in web apps
* Show accurate publish date for web apps
* Drop support for iOS 12 as part of preparation for using Expo 45
  * Will be adding support for iOS 16

Component Updates

* [Web API](../web-api.md): Allow form data to be submitted to API
* [Sound](../sound.md): Play sound even if device is set to silent
* [Logic blocks](../logic.md), [variables](../variables.md): Fix errors seen when trying to compare null variable to empty text or empty list

## August 10, 2022

Platform Updates

* Updated navigation to prepare for Expo upgrade

Component Updates

* [Button](../button.md): Improve appearance of border

## August 9, 2022

Platform Updates

* Improved consistency of naming copied projects
* Updated project page icons

Component Updates

* [Airtable Data Sources](../data-sources.md#airtable): fix error when syncing with Airtable DB containing tables which have been deleted externally to the Thunkable project&#x20;
* Updated Firebase used for [cloud variables](../variables.md#cloud-variables) and [Sign In](../sign-in.md)

## August 3, 2022

Platform Updates

* Project workspace: Close Download/Actions menus when item is clicked
* Membership page: Added Upgrade Account button

Component Updates

* Screen: When new Screen is selected, center that screen in the Design workspace
* Text Input: Fix handling newlines with \n character for Hint text
* Button: Fixed style of Button in nested Group on the web
* Figma import: Fix importing text boxes with newline characters

## July 27, 2022

Platform Updates

* Added pop-up with warning if project is not saved before leaving/refreshing Thunkable project page
* Updated wording on membership page
* Updated Design tab UI
* Fixed icons in project Settings panel
* Adjusted the style of star box on the project detail page&#x20;
* iOS Publish: Updated with Apple Sign In Entitlement&#x20;

Component Updates

* Google Sheets Data Source: Updated 'Delete Row' block so that row is deleted and not just cleared of values
* Share block: made compatible with any file type
* Files drawer: fixed behavior where 'convert to base64' block appeared multiple times
* Any Component drawer: Fixed generic event block
* Google Sheets Data Sources: Fixed behavior where Google Sheet Data Source could be dropped when a project was remixed
* Group: Improve handling of moving children when Group is moved
* Web Viewer: Improved ability to interact with Web Viewer contained in a Group

## July 15, 2022

Platform Updates

New Components

* Drag and Drop UI: Added create and clone blocks
* Drag and Drop UI: Added Relative X/Y and height/width blocks

Component Updates

* Data Sources: Added 'Get All Rows' block for Airtable Data Sources
* Data Viewer: fixed bug seen when trying to add null value to Data Source

## June 16, 2022

Platform Updates

* Added 'Delete Account' section to Thunkable Live app

## June 10, 2022

Component Updates

* Improvements to In-App Purchases component
* Restored appearance of Label's 'TextAlign' property on Android/iOS

## June 3, 2022

Component Updates

* Figma: Fixed checkbox import
* Label: Added Font Family property back to Label component

## June 1, 2022 <a href="#june-1-2022" id="june-1-2022"></a>

Platform Updates

* Built iOS apps now positioned better relative to device notch area
* Improve appearance of projects page at x.thunkable.com

Component Updates

* ​[Bottom Tab Navigator](../bottom-tab-navigator.md): Remove unwanted white space underneath navigator on iOS
* ​[Stack Navigator](../stack-navigator.md): Fix 'Header Mode: None' on web apps
* ​[Groups](../group.md): Can now be positioned relative to device
* ​[Lottie Animation](../lottie.md): Show message if invalid file type uploaded to component
* ​[Label](../label.md): Fix Label.Click block
* ​[Label](../label.md): Fix Number of Lines property
* ​[AdMob](../admob.md): Fix error shown in console when mouse hovers over AdMob Banner in Design tab

New Components

* ​[Camera](../camera.md): Upload Video from photo library

## May 31, 2022 <a href="#may-31-2022" id="may-31-2022"></a>

Updates

* ​[Data Viewer Grid](../data-viewer-grid.md): Prevent unwanted vertical scrolling on iOS when Horizontal Scrolling is enabled
* ​[In-App Purchases](../in-app-purchase.md): Improve error messaging

## May 25, 2022

Updates

* [Data Viewer List](../data-viewer-list.md): Fix scrolling on Android when Screen is scrollable

## Previous Releases

See an archive [here](https://docs.thunkable.com/v/snap-to-place/release-notes).&#x20;

