# 📰 Release Notes

Looking for what's coming soon to Thunkable's Drag and Drop UI? [Click here](https://docs.thunkable.com/v/drag-and-drop/coming-soon)!

## June 25, 2021

Component Updates:

* Improvements to appearance of colors in [Top Tab Navigator](https://docs.thunkable.com/v/drag-and-drop/top-tab-navigator) and [Bottom Tab Navigator](https://docs.thunkable.com/v/drag-and-drop/bottom-tab-navigator) in [Drag and Drop UI](https://docs.thunkable.com/v/drag-and-drop/)

## June 15, 2021

Platform Updates:

* Introduced ability to generate [AAB file for publishing to Google Play Store](publish-to-play-store-android.md)
* Improvements to behavior of downloaded APKs from projects that contain renamed assets

## June 9, 2021

Platform Updates:

* Improvements to performance of Google Sheets [Data Sources](data-sources.md#google-sheets) picker

## May 27, 2021

Platform Updates:

* No longer auto-select first item in media drop-down menu when selecting media source for components such as [Image](image-1.md) or [Sound](sound.md)
* Drag and Drop platform: [New video tutorials](https://docs.thunkable.com/v/drag-and-drop/get-started/tutorials)

New Components:

* Drag and Drop UI: [Stack Navigator](https://docs.thunkable.com/v/drag-and-drop/stack-navigator)

Component Updates:

* Drag and Drop UI: components that are not [Groups](https://docs.thunkable.com/v/drag-and-drop/groups) will no longer accept "children" in the Component Tree
* Drag and Drop UI: [Data Viewer List](https://docs.thunkable.com/v/drag-and-drop/data-viewer-list)'s Left Swipe Enabled and Right Swipe Enabled properties are restored in Design Tab
* Drag and Drop UI: [Label](https://docs.thunkable.com/v/drag-and-drop/label) and [Button](https://docs.thunkable.com/v/drag-and-drop/button) now have a range of fonts to choose from
* Online [Data Sources](data-sources.md) are no longer disconnected from a project when it is copied within the same account

## May 24, 2021

Platform Updates:

* Drag and Drop: Enable pan-to-scroll in Design tab

Component Updates:

* Improvements to performance of [Push Notifications](push-notifications-by-one-signal.md) on iOS

## May 21, 2021

Component Updates:

* [Stack Navigator](stack-navigator.md) no longer compresses screens when [previewing on web](get-started/live-test.md#live-preview) or in a [published web app](publish-as-a-web-app-pro.md)

## May 19, 2021

Platform Updates

* Style updates to login page
* [Publish as web app](publish-as-a-web-app-pro.md): Instead of automatically publish as a mobile web app, let creator choose mobile or responsive web app as project is first published
* Drag and Drop: Restore guidelines in Design tab

Component Updates

* Duplicated [Screens](screen.md) will be added to the right of the existing Screen
* Drag and Drop: Improve behavior of Navigator properties panel in Design tab

## May 13, 2021

Component Updates

* Improvements to Web Viewer scrolling behavior in Drag and Drop projects on Android and iOS

## May 12, 2021

Platform Updates

* Update platform to Expo 41
  * Built APKs now target Android 11
  * Project Settings includes [AdMob Settings](projects/settings.md#admob-settings) section
  * iOS apps with AdMob now [ask for permission](admob.md#ios-and-admob-permissions) to show personalized ads to users in line with [Apple's AppTrackingTransparency requirements](https://developer.apple.com/news/?id=ecvrtzt2)
* Update style of sign in/sign up page
* Fix top banner position in Snap to Place projects

Component Updates

* Expo 41 update also includes minor updates to the following: [Video Recorder](video-recorder.md), [Audio Recorder](audio-recorder.md), [Barcode Scanner](barcode-scanner.md), [Camera](camera.md), [Photo Library](photo-library.md), [Keep Screen Awake block](device.md#keep-screen-awake), [Location Sensor](location-sensor.md), [Date Input](date-input.md), [Time Input,](time-input.md) [Gyroscope](gyroscope.md), [Accelerometer](accelerometer.md), [Magnetometer](magnetometer.md), [Animation by Lottie](lottie.md)
  * These updates are effective in the Snap to Place UI and the Drag and Drop UI
  * These updates are related to permissions and will not affect the performance of these components in your project

## May 5, 2021

Platform Updates

* Allow [published web apps](publish-as-a-web-app-pro.md) to be [embedded](publish-as-a-web-app-pro.md#embed-your-app-in-a-webpage) in a HTML iframe
* Add alert when [previewing](get-started/live-test.md#live-preview) a project that contains a [Web Viewer](web-viewer.md) or a [Bluetooth Low Energy](bluetooth-low-energy.md) component on the web, advising that performance may not match performance on a device
* Improve visibility of components on Drag and Drop canvas when very zoomed in

Component Updates

* Improve appearance of customized [Switch](switch.md) colors
* Update error message shown when [Web API](web-api.md) fails to fetch data

New Components

## April 30, 2021

Platform Updates

* Remove `legacyExternalStorage` permission from built Android apps in line with Google's [Policy Updates](https://support.google.com/googleplay/android-developer/answer/9934569?visit_id=637554004669617100-3975859313&rd=1)

Component Updates

* Improved performance of [Sound](sound.md) component on iOS 

## April 23, 2021

Component Updates

* Drag and Drop: Added Screen-specific properties to [Top Tab Navigator](https://docs.thunkable.com/v/drag-and-drop/top-tab-navigator#screen-specific-tab-navigator-properties), [Bottom Tab Navigator](https://docs.thunkable.com/v/drag-and-drop/bottom-tab-navigator#screen-specific-tab-navigator-properties), and [Drawer Navigator](https://docs.thunkable.com/v/drag-and-drop/drawer-navigator#screen-specific-drawer-navigator-properties)

## April 22, 2021

Platform Updates

* Fix issue where [downloaded](download.md#download-ios-app) iOS apps showed blank space at top and bottom of screen.
  * Added [Ignore Notch Area](projects/settings.md#ignore-notch-area) and [Notch Area Background Color ](projects/settings.md#notch-area-background-color)as properties in Project Settings.
* Let App Name of [web apps](publish-as-a-web-app-pro.md) set page title instead of project name

## April 20, 2021

Platform Updates

* Add AdMob IDFA to iOS build server
* New phone frame border
* Speed up dragging in large projects
* Snap to Place: Improvements behavior on Android where if the device language is a language that is written right-to-left, the position of the components on the app screen are inverted
* Drag and Drop: Adjustments to spacing between Screens in the Design tab
* Drag and Drop: Reset screen position when switching from preview to editing

Component Updates

* Update style of [Alert](alert.md) component

## April 13, 2021

Platform Updates

* Prevent error when no data is found in Airtable base
* Allow HTTP traffic on Android
* Drag and Drop: improve performance of hidden components on Android

Component Updates

* Allow Objects [Get Property Of](objects.md#get-properties-of-an-object) blocks to handle [nested properties and arrays](objects.md#nested-values-and-values-from-arrays)
* [Airtable](spreadsheet.md) component and [Data Sources](data-viewer-list.md#airtable): Allow rows to be created/updated with non-text values
* Add Text Items Color, Text Items Background Color, and Font Size properties to the [List Viewer](list-viewer.md)
* Drag and Drop: add background image to Groups

New Components

* Drag and Drop: AdMob banner
* Drag and Drop: Switch

## Mar 24, 2021

Platform Updates

* Display default profile picture if one has not been set
* Adjust scroll bar on Drag and Drop UI
* Adjustments to Sort By filter on projects homepage

Component Updates

* Fix tooltip message for Web Viewer
* Updated icons for Google Maps and Lottie components

## Mar 18, 2021

Platform Updates

* Update Image icon
* Add Delete Project confirmation modal
* Increase size of border on web preview phone frame
* Update fonts in left sidebar
* Fix scroll glitch in Add Components section
* Drag and Drop: When component is duplicated, add to top of component tree
* Drag and Drop: Increase screen size on Design tab
* Drag and Drop: Remove auto margin that interferes with centering active screen
* Drag and Drop: Improve appearance of Labels in web apps
* Drag and Drop: Update Component Tree
* Drag and Drop: Update Properties Panel layout

## Mar 15, 2021

Component Updates

* Improve performance of Translator component on the web

## March 8, 2021

Component Updates

* Launch Pickers only if visible
* Improvements to Android build server

## Mar 1, 2021

Platform Updates

* Add security modal to prevent accidental deletion of projects. Modal includes warning that project keystore will be deleted.
* Critical update to Thunkable Live for iOS released
* Set delete buttons to be red

## Feb 22, 2021

Platform updates

* Improved performance of Thunkable Live app for iOS
* Introduced [status page](https://status.thunkable.com/) for Thunkable

## Feb 15, 2021

Platform Updates

* Improve rendering of Screens in Design tab of Drag and Drop projects
* Added the following components to Drag and Drop UI:
  * Time Input
  * Date Input
  * Additional guidelines to guide positioning of components

## Feb 8, 2021

Component Updates

* Added block [get device color scheme](device.md#get-device-color-scheme) to the [Device](device.md) drawer of blocks

## February 3, 2021

Platform Updates

* Improve iOS build process on Drag and Drop UI

Component Updates

* Improve performance of Text Input with 'Secure Text Entry' property enabled on web apps and apps being previewed on the web
* Update text for set/get blocks

## January 26, 2021

Platform Updates

* Improve positioning of imported Figma files in a Screen
* Improve appearance of component tree

## January 8, 2021

Platform updates

* Add a processing indicator when new project is created

Component Updates

* Improve performance of [Sensor]() components

## December 15, 2020

Platform Updates

* Combined Drag and Drop UI and moving invisible components to blocks. These features can now be enabled by checking 'Be the first to try out new drag and drop interface' when creating a new project.

## December 2, 2020

Platform updates

* Removing certain permissions from built Android apps to make publishing to the Play Store easier
* Enable creators to access their project files from the Thunkable Design tab

## November 20, 2020

Platform Updates

* Introduced Drag and Drop as [beta feature](https://x.thunkable.com/account/settings)
* Introduced moving invisible components to Blocks tab as [beta feature](https://x.thunkable.com/account/settings)

Component updates

* Add [PATCH](web-api.md#upload-data) method to [Web API](web-api.md) component

## October 28, 2020

Component Updates

* Fixed error caused by deleting [Sprites](sprites.md) from app project

## October 15, 2020

Component Updates

* Allow creators to add their own [Google Maps API key](map.md#google-maps-add-api-key) to their project settings

## September 22, 2020

Component Updates

* [Delete All Rows](data-sources.md#delete-all-rows) block for [Data Sources ](data-sources.md)
* [Alert](alert.md) now works in [Web Apps](publish-as-a-web-app-pro.md)

## September 18, 2020

Component Updates

* Refresh block for [Data Viewer List](data-viewer-list.md) and [Data Viewer Grid ](data-viewer-grid.md)components

New components

* [Custom Data Viewer Layout](custom-data-viewer-layout.md) for use with [Data Viewer List ](data-viewer-list.md)and [Data Viewer Grid](data-viewer-grid.md)

## September 8, 2020

New components

* [Rating](rating.md) Component

## August 28, 2020

New components

* [Canvas Label](canvas-label.md)

Component Updates

* Add multiple [Stages](canvas.md#the-stage) to a [Canvas](canvas.md)

## August 26, 2020

Platform Update

* Update built Android apps to target API level 29

## August 7, 2020

Component Updates

* Manage [location permissions](web-viewer.md#manage-permissions) for [Web Viewer](web-viewer.md)

## July 17, 2020

Component updates

* New [function](functions.md) with return blocks
* Add opacity property to [Sprites](sprites.md)
* Fix 'set Zoom to' block in [Map](map.md)
* Add ability to add circles, polygons to Canvas with [Looks](looks.md) blocks
* Support landscape mode for [Screens](screen.md) on Android apps
* In web apps, open links in new tab
* [Video Recorder](video-recorder.md) component

## July 9, 2020

Component Updates

* Add Click event to [Lottie Animation](lottie.md) component
* Fixes to [Map](map.md) Region so map does not reset on any event

## July 3, 2020

Component Updates

* Add Go Forward/Go Back blocks to [Web Viewer](web-viewer.md)
* Add 'flip [Sprite](sprites.md)' block to [Canvas](canvas.md) blocks

## June 29, 2020

Platform Updates

* Add creator of original project to [Project Details Page](get-started/your-thunkable-projects-page.md#your-project-detail-page) of remixed projects

## June 18, 2020

Component updates

* Adding click events for [Text Input](text-input.md), [Label](label.md) and [Image](image-1.md) components
* Improving the [Map](map.md) event
* [Data Source](data-sources.md): Google Sheets can now be accessed by index in Data Source blocks 
* [Time Input ](time-input.md)label updated

New components

* [Audio Recorder]()

## June 15, 2020

Platform updates

* Redesign of [Thunkable Projects Page](https://docs.thunkable.com/get-started/your-thunkable-projects-page)

## June 8, 2020

Component updates

* Make appearance of [Text Input](text-input.md) in Design tab more true to how it appears in built app/web app when Number Of Lines is greater than 1
* Add blocks to set Image of [Sprite](sprites.md) to next/previous image in Picture List

## June 5, 2020

Platform updates

* New tutorials panel

## May 7, 2020

New components

* [Data Viewer List ](https://docs.thunkable.com/data-viewer-list)and [Data Viewer Grid](https://docs.thunkable.com/data-viewer-grid): list viewers with extended functionality that can be connected to external [Data Sources](https://docs.thunkable.com/data-sources) \(Google Sheets, Airtable, Local DB\)

## Apr 27, 2020

Component updates

* Ability to fix [Screen Orientation](https://docs.thunkable.com/screen#set-orientation) to `Portrait`, `Landscape` or `auto`

## Mar 26, 2020

Blocks

* Added `if-else` block

Bugs

* Fixed bug in `forever` block

Platform

* Removed deprecated UIWebView component \(ITMS-90809\)

## Mar 13, 2020

Platform updates

* Ability to publish your Thunkable app as a [web app](https://docs.thunkable.com/publish-as-a-web-app-pro)

## Feb 28, 2020

Platform updates

* [Save screens](https://community.thunkable.com/t/latest-thunkable-release-save-screens-is-here-2020-02-27/488296) and use them in different projects 
* Added Z property on sprites
* Save expand/collapse settings in the component tree

## Jan 29, 2020

Bug fixes

* Fixes bugs related to recent blocks speed improvement as detailed in the [community](https://community.thunkable.com/t/thunkable-x-blocks-update-your-feedback/425809?u=jane)

Platform

* Preview your app without your device. Added a web preview to the Live Test modal so creators can preview their app without their device. Just click on the `Live Test` button in the designer to test this feature for yourself. This feature is in beta and [not all components are supported](https://docs.thunkable.com/web-preview)

## Jan 23, 2020

Platform

* Speed improvements for projects with large number of blocks

## Jan 3, 2020

Platform updates

* [Web Preview]() \(Beta\) - see a web preview of your apps on the details page of your project and any project on the Thunkable gallery; some [components are not supported yet]() and projects may appear differently than they do on your device

## Dec 19, 2019

Platform updates

* Project Detail Page - updated styling \([see sample](https://x.thunkable.com/projectPage/5c183d7c7bd8616f60c5a39a)\)

## Dec 10, 2019

Platform updates

* User Profile Page - updated profile pages for all creators, featuring all your projects \([see sample](https://x.thunkable.com/profiles/albert)\); Only `public` projects will be visible to other creators

Component updates

* [Timer](timer.md) - added the ability to set the timer in seconds or milliseconds and to count up

## Nov 18, 2019

Platform updates

* Gallery - added the ability to star your favorite projects

## Oct 29, 2019

New components

* [Barcode Scanner](barcode-scanner.md) - allow apps to read any barcode or QR code with the help of a device camera

Component updates

* [Video](video.md) - added the ability to auto-play videos and pause / play video from blocks

## Oct 25, 2019

Platform updates

* Gallery - added the ability to search public gallery projects by creator username

## Oct 18, 2019

New components

* [Video](video.md) - allow users to play videos in your app

## Oct 4, 2019

Component updates

* [Canvas](canvas.md) - added option to change the color of the frame, or the area surrounding the Canvas
* [Alert](alert.md) - adds default text for the Confirm and Cancel buttons

## Oct 2, 2019

Component updates

* [Assistant](assistant.md) by Dialogflow - upgrades the API to V2 since V1 is retiring on Oct 23, 2019

## Sep 12, 2019

Bug fixes

* Screen - fixes `Scrollable` property on Screen component; still a bug with `Scrollable` property for Row component

## Sep 10, 2019

New components

* [Canvas](canvas.md) and [Sprites](sprites.md) - build simple games like Space Invaders and Pong with our newest version of Canvas which includes among other features, a physics engine to create more engaging games
* [PDF Reader](pdf-reader.md) - allow users to view PDFs from the convenience of an app

Platform updates

* [Importing / exporting Android keystores](publish-to-play-store-android.md#export-keystore-from-thunkable-classic) - update apps published to the Google Play store that were made on Thunkable Classic or another compatible platform

## Sep 4, 2019

New components

* [Date Input](date-input.md) - lets users easily select a specific date using the native Android or iOS date picker
* [Time Input](time-input.md) - lets users easily select a specific time using the native Android or iOS date picker

## Aug 21, 2019

Component updates

* [Web API](web-api.md) - added blocks to support changing headers and query parameters

Bug fixes

* [Share](share.md#send-a-text) - fixes bug to send text messages on iOS devices

## Aug 16, 2019

Platform updates

* Tooltips!
* Ability to duplicate components and their properties!
* Ability to duplicate projects in the project list page!

## Jul 19, 2019

Component updates

* [Webviewer](web-viewer.md) - supports full screen video, geolocation and data detector types
* [Stack Navigator](stack-navigator.md#style-your-screen-color) - supports editing the background color of the header bar
* [Gyroscope](gyroscope.md#properties) - added ability to get `alpha`, `beta` and `gamma` values

Block updates

* Add block to dismiss keyboard in the [Device](device.md#dismiss-keyboard) drawer

## Jul 15, 2019

New blocks

* "[Any Component](any-component-blocks.md)" - create and clone visible components e.g. Labels, Images, Buttons in your app on the fly. Very helpful for data-driven apps where the number of components matches the data that it is linked to e.g. a photo-sharing or chat apps and should reduce the number of blocks in many cases

## Jun 26, 2019

New components

* [Bluetooth Low Energy](bluetooth-low-energy.md) - connect to, receive and send data from a mobile device to any device that has a bluetooth low energy chip installed

Component updates

* Maps - Add [delete markers](map.md#delete-markers) event to Maps component
* [Label](label.md) - More styling options! Adds more options to set the font weight and to align the text in the label 

## Jun 24, 2019

Component updates

* [Drawer Navigator](drawer-navigator.md) - added block to toggle open and close the drawer to enable hamburger menu

Platform updates

* Displays profile photo in the top right corner of platform; update yours on the [account settings page here](https://x.thunkable.com/account/settings)

## Jun 17, 2019

Component updates

* Add heading event for Magnetometer

## Jun 11, 2019

Component updates

* Add [shaking event](accelerometer.md#shaking) to Accelerometer component

## Jun 10, 2019

Platform updates

* Added the ability to change your profile photo and headline on your [account settings](https://x.thunkable.com/account/settings) page
* Made app settings page more discoverable with icon -- edit your app title, description, icon and more!

## Jun 3, 2019

Platform updates

* Added ability to change username from [account settings](https://x.thunkable.com/account/settings) page. Username changes will be reflected on the Thunkable community forum

## May 23, 2019

Bug Fixes

* Fixes asset error during iOS publish
* Fixes component search for a few components

## May 20, 2019

New Components

* [Accelerometer](accelerometer.md) - accesses the mobile device's sensor that measures even tiny forces of acceleration acting on the phone from natural \(in a moving vehicle\) and man-made \(shaking the device\)
* [Gyroscope](gyroscope.md) - accesses the mobile device's sensor that measures even tiny tilts of the phone, often used in gaming apps
* [Magnetometer](magnetometer.md) - accesses the mobile device's sensor that measures magnetic fields from the Earth and other nearby objects 

## May 14, 2019

Component Updates

* [Payment]() by Stripe - New lower fees for ![](.gitbook/assets/pro.png)- 2.9% + $0.30 per transaction \(0% Thunkable fee\)

## May 6, 2019

New Components

* [Push Notification](push-notifications-by-one-signal.md) by One Signal ![](.gitbook/assets/pro.png) - PRO only component for sending push notification to users who have downloaded your app; all Thunkers can add the component to their project and live test on Android

## May 2, 2019

New Components

* [Blockchain Wallet]() and [Smart Contract]() by Oasis - our first two components that secure your app's data in the blockchain, powered by Oasis, a privacy-focused cloud backed by blockchain technology

## Apr 9, 2019

New Components

* [Loading icon](loading-icon.md) - helpful UI component to tell your app users that an activity is happening in the background

## Mar 20, 2019

Platform Updates

* Login - added the ability to login to the platform by email

## Mar 19, 2019

Component Updates

* AdMob ![](.gitbook/assets/pro.png) 
  * Thunkable Live iOS app now supports live testing apps with AdMob

## Mar 12, 2019

New Components

* Ads by AdMob ![](.gitbook/assets/pro.png) - all Thunkers can add to their project and live test but only PRO members can download and publish apps with AdMob
  * [Banner](https://docs.thunkable.com/admob#banner-ad)  **-** displays a rectangular ad at the top of bottom of any screen
  * [Interstitial](https://docs.thunkable.com/admob#interstitial-ad) - full screen ads that display over the current screen
  * [Rewarded Video](https://docs.thunkable.com/admob#rewarded-video-ad) - show a full screen video ad over the current screen and adds event handler to reward user after watching

Platform Updates

* Improved build and deploy times

Bug Fixes

* Fixed broken links to Thunkable docs

## Feb 11, 2019

Block updates

* [Variables](variables.md) - added a [change listener to app and stored variables](variables.md#for-app-and-stored-variables-updating-when-the-variable-initializes-or-changes)

Bug fixes

* Fix bug that causes random block to not work in the variable initialization block

Platform updates

* Updated default Splash Screen beaver on downloaded / published apps to new "Made with Thunkable" logo; Thunkable PRO users substitute the Thunkable branding with their own logo

## Jan 31, 2019

Platform updates

* Downloaded and published apps are now ~8MB smaller than before

Component updates

* [Screen](screen.md), [Row](row.md) and [Column](column.md) - `Justification` and `Alignment` properties renamed to `Horizontal and Vertical Alignment`
* [Label](label.md) - default height set to `fit contents`

Block updates

* [Color](colour.md) - added the ability to [set color by Hue, Saturation and Value](colour.md#set-hsv-color)

## Dec 14, 2018

* [Local DB](local-db.md) - create and retrieve data from a data table directly saved in your app

Component updates

* [Share](share.md) - now enables users to send text messages, emails and make phone calls from mobile's device's default apps

New block category

* [Device](device.md)
  * [Date and time](device.md#get-current-time-and-date) - Get the current time from the device's clock
  * [Vibrate](device.md#set-device-to-vibrate) - sets a device to vibrate 
  * [iOS or Android](device.md#get-mobile-operating-system) - detects which platform the device is on
  * [Online or offline](device.md#get-online-offline-status) - detects if device is connected to Wi-Fi or data network

## Dec 5, 2018

Bug fixes

* Fixes variety of bugs that led to Thunkable Live Android crashes
* Users no longer have to set margins and padding to 0 for columns and rows on Android 
* Improved error messaging and validation for new Publish to IOS workflow

## Nov 20, 2018

Platform updates

* [Publish to iOS](publish-to-app-store-ios.md) - Supports the ability to publish to iOS with two-factor authentication turned on

Component / block updates

* Visible property on components - Support making components visible and invisible from the designer and the blocks

Bug fixes

* Custom launch screen for PRO users - fixes bug that does not show current app's logo
* Thunkable Live app - displays app icons on the project list page

## Nov 15, 2018

Component updates

* Tab Navigator - Supports adding icons to the tab navigator with the introduction of two new components, a [Top Tab Navigator](top-tab-navigator.md) and a [Bottom Tab Navigator](bottom-tab-navigator.md). The original [Tab Navigator]() will continue to be supported in existing projects but we highly encourage creators to adopt the new tab components which will have more features

Bug fixes

* Text Input - automatically resizes screen when keyboard is open
* Publish to iOS - fixes Camera and Photo Library permissions
* Blocks - prevents possible infinite loops when asset block is loaded

## Nov 7, 2018

Bug fixes

* Fixes bug where previewed projects were one step behind the Blocks Editor
* Fixes bug where variables did not work with map methods
* Fixes bug where variables did not work well as list indexes

## Oct 23, 2018

Bug fixes

* Fixes the compatibility issue with the new [variable](), [list](lists.md) and [object](objects.md) blocks

## Oct 22, 2018

Platform updates

* [Thunkable PRO users](https://thunkable.com/#/pricing) can now remove the Thunkable logo from the initial screen of all downloaded and published apps. Thunkable will automatically replace that logo with the app icon that they upload. We will be introducing additional customization options in the future.

## Oct 10, 2018

Platform updates

{% hint style="success" %}
Thunkable has launched the [Public Gallery](public-gallery.md), a public collection apps for anyone to preview, download or remix.

All new apps will be public by default and included in the Public Gallery.

Creators who want to keep their project private can [upgrade to Thunkable PRO](https://thunkable.com/#/pricing).
{% endhint %}

* [Variables](variables.md) can now be of type 'app', stored' and 'cloud'.  Existing uses of variables will continue to work as they did before this change.

## Sep 13, 2018

Bug fixes

* Fix some Android crashes
* Easier drag and drop of Button and Image components
* Fix initial load of app icon

## Aug 30, 2018

Bug fixes

* Fix SignIn method of Sign In component to populate outputs userId & isEmailVerified

## Aug 29, 2018

Bug fixes

* Fix iOS download & publish app icon

## Aug 28, 2018

Platform updates

{% hint style="success" %}
All apps built on Thunkable are now [compatible with Android 8.0](https://developer.android.com/about/versions/oreo/android-8.0-migration) \(aka API 26\)!

Users will be prompted to give permission to allow the use of certain components within an app \(Speech Recognizer, Assistant, Camera, Photo Library, Location Sensor\)
{% endhint %}

* Some app layouts have been updated
  * Hide status bar bug - A blank status bar will still show up even if hide status bar is set to false; we are hoping to fix this soon
  * Heights of visible elements set to 'fit contents' may need to be updated to 'relative size' or another option
  * [Scrollable columns](column.md#enable-scrolling) - height will need to be set to 'fit contents'

Bug fixes

* Android app no longer crashes when [open link](control.md#open-an-installed-app-or-website-by-link) block is triggered
* Downloaded and published iOS apps no longer shows editable blocks

## Aug 8, 2018

Bug fixes

* Stability should be significantly improved on the Live App, especially for Android
* There should generally be fewer crashes on downloaded/published apps, especially for Android
* The WebViewer on Android should scroll properly and be responsive
* The Scrollable feature of the Column component should now work properly
* Column component will now display background images on iOS
* Scrollable screens will now scroll on downloaded or published apps for iOS
* Setting Latitude and Longitude on the Map component on Android via blocks should now work
* Setting the Value property of the Slider component on Android via blocks should now work
* Projects with a huge number of components or blocks should no longer generate errors from backend server

New blocks

* [Shuffle list](lists.md#shuffle-list) - get a copy of a list with the items shuffled in a random order.

Platform updates

* Improvements to the tutorials

## Jul 20, 2018

New components

* [Alert](alert.md) - launches a dialog / notification with a message and one or more buttons

## Jun 12, 2018

Bug fixes

* Solves some issues with Thunkable Live app on Android
* Reduces project saving issues

## Jun 5, 2018

**Thunkable Cross-Platform ✕ launches out of beta!**

Platform updates

* Renaming components is now supported. Click on the top of the properties panel to edit the component name
* Each new project can be set to [public or private](projects/).  Public projects are eligible to be featured in the Thunkable Gallery and can be shared in both [read-only](share-1.md#share-a-read-only-version-of-your-app-project) and fully-editable mode
* Sample apps now featured on the project list page
* Supports iOS usage descriptions for describing to users why certain permissions are needed when they download your app; applies only when you Publish to the iOS App Store

Component updates

* [Switch](switch.md) component no longer needs blocks to set-up

## May 22, 2018

Component updates

* [Map](map.md) - adds new block events e.g. on Map Click, on Marker Click and supports the ability to add markers, polylines and polygons
* [Text to Speech](https://docs.thunkable.com/text-to-speech) - increase supported languages from 6 to 87
* [Share](share.md#share-an-image) - now supports sharing locally stored assets \(does not work on Live Test for iOS\)

New components

* [Location Sensor](location-sensor.md) - gets user's current location
* [Slider](slider.md) - UI element of choice for letting users select a value or range from a fixed set of options, such as setting the brightness of a screen

## May 15, 2018

Platform updates

* [Five new tutorials](get-started/tutorials.md) for Thunkable beginners now located in platform panel on the left
* [Share a read-only version](share-1.md#share-a-read-only-version-of-your-app-project-by-link) of your project is now supported with a public option

Bug fixes

* \(Background\) Image for Screens, Rows, Column and Image components now appear in Live Testing when using a Screen.start block
* Image height or width set to 'fit contents' now appear in Live Testing
* Improvements to Download / Publish for iOS including transparency support for app icons and better error messaging
* Improved messaging for Download for Android

## May 7, 2018

Platform updates [broken link](https://play.google.com/brokenlink) [out-of-bounds link](https://app.gitbook.com/@thunkable/s/thunkable-docs/~/edit/drafts/-LnMymO8dgjVIc_YwQ4R/functions)

* Significant user interface update including a new Design / Blocks switch, add Components shifted to the left panel and Properties shifted to the right panel
* Live app now lets you [live preview](get-started/live-test.md#live-preview-android-only) all your app projects from the comfort of your mobile device \(Android only\)
* [Publish for Android](publish.md#publish-to-the-play-store-android) now supported
* Adds [version support](https://docs.thunkable.com/publish-to-app-store-ios#send-to-app-store-connect) for download / publish for Android and iOS
* Updated [download](download.md#download-and-install-ios-app) and [publish](publish.md#publish-to-the-app-store-ios) emails for iOS

## April 12, 2018

Component updates

* [Button](button.md) - supports a number of new properties including sizing \(height, width\) and adding a background picture

New components

* [Speech Recognizer]() - uses artificial intelligence to recognize and translate spoken language into text in 14 different languages
* [Share](share.md) - allows users to share text or post images using their favorite installed communication app from Slack and Facebook to iMessage and WhatsApp
* [Switch](switch.md) - popular UI element to turn on and off a certain feature in an app, often used in settings pages

Platform updates

* Updated Blocks colors

## Apr 5, 2018

New components

* [Spreadsheet](spreadsheet.md) by Airtable - gets, uploads, updates and deletes data from the popular spreadsheet service
* [Payment]() by Stripe - enable accepting credit card payments in app powered through Stripe; Each payment is subject to a 4.9% + $0.30 per transaction fee

Platform updates

* Supports opening installed app by deep link on Android \(aka Activity Starter\) via a Control block
* Blocks now includes zoom control and a better location for the trash can
* Properties have been re-organized into hopefully easier to use categories

## Mar 20, 2018

Platform updates

* [Custom app package name ](release-notes.md)/ bundle ID now supported for both Android and iOS; app icon also supported for Android
* [Make a copy ](make-copy.md)of your project aka checkpoint in one click
* Tracking of project [shares](share-1.md) now available on project page; share links no longer require a user to be logged in

Component updates

* Properties now set / changeable in blocks including all Text / Background Color properties for visible components and Language properties for [Translator](), [Text to Speech]() and [Assistant](assistant.md)
* Transparent color now available as a color property across all visible components
* Easy select and upload via Picture property for [Image]() component

Bug fixes

* Function blocks now work again
* Blocks strings now accepted as numbers
* Changing dropdown component in blocks or duplicating blocks now keeps the same property

## Mar 6, 2018

New component

* [Sign In](https://github.com/thunkable/thunkable-docs/tree/4a752596e288fca776105e94dc5e863bb9a3e25a/ios/components/screen-layout/authentication/sign-in.md) powered by Firebase - support for email sign-in; set-up requires entering in an API key and database URL into app settings
* [Media Database](media-db.md) powered by Cloudinary - support for image, audio and video upload

Component updates

* Most Visible components \(Screen, TextInput, Label, Column, Row, Image, ListViewer, WebViewer, Maps, Google Maps\) - advanced properties including padding, margin, border & user location \(Maps / Google Maps\) added 
* [Realtime DB](realtime-db.md) powered by Firebase - changes set-up from adding a .plist file to entering in an API key and database URL into app settings

Platform updates

* Installing an Android .apk no longer requires uninstalling the Thunkable companion app
* Easier discoverability of uploading files \(now in the bottom left under the component tree
* Error message when dropping a Navigator or Screen to the Phone previewer; they can only be added to the Visible components section of the tree
* Small updates to sharing by link and notifications during download and publish

## Feb 23, 2018

Start of Thunkable Cross-Platform **✕** public beta

