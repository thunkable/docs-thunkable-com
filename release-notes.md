# 📰 Release Notes

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
* BLE: Added ListenForDisconnection block
* Files drawer: fixed behavior where 'convert to base64' block appeared multiple times
* Any Component drawer: Fixed generic event block
* Google Sheets Data Sources: Fixed behavior where Google Sheet Data Source could be dropped when a project was remixed
* Group: Improve handling of moving children when Group is moved
* Web Viewer: Improved ability to interact with Web Viewer contained in a Group

## July 15, 2022

Platform Updates

* Updated wording in pop-up that asks new creators about occupation
* Fixed crashing seen with clone block
* Improved handling of uploading large files to the cloud

## July 14, 2022

Component Updates

* Screen: Fix z-index reversal

## July 6, 2022

Platform Updates

* Enabled Drag and Drop by default for creators who create Drag and Drop projects
* Keep component selection when clicked twice

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

* Restored appearance of Label's 'TextAlign' property on Android/iOS

## June 8, 2022

Component Updates

* Improvements to In-App Purchases component

## June 3, 2022

Component Updates

* Figma: Fixed checkbox import
* Label: Added Font Family property back to Label component

## June 1, 2022

Platform Updates

* Built iOS apps now positioned better relative to device notch area
* Improve appearance of projects page at x.thunkable.com

Component Updates

* [Bottom Tab Navigator](bottom-tab-navigator.md): Remove unwanted white space underneath navigator on iOS
* [Stack Navigator](stack-navigator.md): Fix 'Header Mode: None' on web apps
* [Groups](https://docs.thunkable.com/v/drag-and-drop/group): Can now be positioned relative to device
* [Lottie Animation](lottie.md): Show message if invalid file type uploaded to component
* [Label](label.md): Fix Label.Click block
* [Label](label.md): Fix Number of Lines property
* [AdMob](admob.md): Fix error shown in console when mouse hovers over AdMob Banner in Design tab

New Components

* [Camera](https://docs.thunkable.com/v/drag-and-drop/camera): Upload Video from photo library

## May 31, 2022

Updates

* [Data Viewer Grid](data-viewer-grid.md): Prevent unwanted vertical scrolling on iOS when Horizontal Scrolling is enabled
* [In-App Purchases](in-app-purchase.md): Improve error messaging

## May 25, 2022

Updates

* [Data Viewer List](data-viewer-list.md): Fix scrolling on Android when Screen is scrollable

## May 14, 2022

Updates

* Add [information to platform concerning changes to testing your iOS app on an iOS device](https://blog.thunkable.com/update-on-ios-downloading-with-thunkable)

## May 13, 2022

Updates

* [Groups](https://docs.thunkable.com/v/drag-and-drop/group): Allow custom touch opacity

## May 6, 2022

Updates

* [Bluetooth Low Energy](https://docs.thunkable.com/v/drag-and-drop/bluetooth-low-energy): Fix ReceiveByteArray block

## May 2, 2022

New Components

* [File Picker for Snap to Place UI](https://docs.thunkable.com/file-picker)

## April 27, 2022

Platform Updates

* Fixes to UI inconsistencies

New Components

* [Checkbox](https://docs.thunkable.com/v/drag-and-drop/checkbox) (Drag and Drop UI)

Component Updates

* Switch: Improve positioning on Thunkable Live companion app
* Screen: Add Computed Height and Computed Width blocks
* Groups: Add relative positioning for child components
* Firebase Sign In: Added Delete User block
* Visible Components: Fix unintended shadows/borders

## March 11, 2022

New Components

* [File Picker blocks](https://docs.thunkable.com/v/drag-and-drop/files#file-from-device)

## March 3, 2022

Platform Updates

* Add 'Published as Web App' as filter on project home screen

Component Updates

* Fix z-index for Video player on web
* Improve scrolling for non-editable Text Input
* Improve Text Input autofocus on web

## February 24, 2022

Platform Updates

* Improvements to location of pasted blocks in Firefox browser
* Reduce iOS build time from 40 minutes to 20 minutes

Component Updates

* Upgrade Airtable version to 0.7.2
* Fix Airtable handling of zero values
* Improve behavior of 'when Screen Opens' block on screens with Loading Icon

## February 17, 2022

Platform Updates

* Improvements to appearance of projects on larger screens

## February 15, 2022

Platform Updates

* Reduce build times for iOS apps from 40 minutes to 20 minutes

## February 7, 2022

Platform Updates

* DND UI: improvements to relative positioning
* Updates to rendering fonts on the web
* Blocks: Blocks that have been copied and pasted will always be pasted within view
* Android Build Server: Escape Maps and AdMob API keys to improve Android build process

Component Updates

* Canvas: Improvements to Canvas as rendered in the Design tab
* Web Viewer: Improvements to showing offline HTML files

## February 4, 2022

Component Updates

* Web Viewer: Updates to requesting end user permission

## February 3, 2022

Platform Updates

* **Upgraded to** [**Expo 43**](https://blog.expo.dev/expo-sdk-43-aa9b3c7d5541)****
* Thunkable Live App: UI updates
* Thunkable Live: Reset app testing local storage when local data source is updated
* Figma: Import assets as regular Thunkable assets
* For components with text, ensured default text color is consistent across Android, iOS and Web
* DND UI: X/Y properties are relative to the container

Component Updates

* Data Sources: Added rename button for local Data Sources
* Data Viewer Grid: Added horizontal scroll
* Labels: Improvements to appearance on wider screens
* Image: Enable rendering of SVG image files
* Button: Added ability to set properties when Button is part of a custom Data Viewer List
* Video: Editing properties of hidden video player no longer crashes the app
* Canvas: Improved appearance when height is relative or absolute value
* Canvas: Fixed 'next sprite image number' block
* Map: Width of marker description box better fits descriptions of different lengths

## January 31, 2022

Platform Updates

* Improvements to layout of permissions in project settings panel

## January 28, 2022

Platform Updates

* Fix titles of imported [Figma](https://docs.thunkable.com/v/drag-and-drop/figma) screens
* Rename [saved screen](screen.md#choose-a-saved-screen) and its children if Screen/components with these names already exist in the project

## January 24, 2022

Platform Updates

* Improve performance of blocks tab
* Reduce how frequently creators need to sign in again

Component Updates

* Video: Improvements to play/stop blocks performance

## January 21, 2022

Platform Updates

* [Figma Import](https://docs.thunkable.com/v/drag-and-drop/figma): Improvements to screen and artboard naming
* Fix behavior where deleting all screens in a project caused the browser screen to go blank

Component Updates

* Data Viewer: Move 'empty string' property to bottom of main properties panel
* Label: Add default border styles
* Push Notifications: Location Permissions now cross-platform (were previously Android-only)
* Video Player: Update to give end user more control over video playback

## January 14, 2022

Platform Updates

* Update scrollbar width for consistency across platforms
* Update how long component names are handled

Component Updates

* Text input: Added support for changing hint text color on web

## January 13, 2022

Platform Updates

* Improve appearance of imported Figma files when project is in read-only mode

Component Updates

* Web Viewer: Add tracking permissions
* Web Viewer: Performance Improvements

## January 12, 2022

Platform Updates

* Fixed behavior where some data sources could not be deleted

## January 7, 2022

Platform Updates

* Fixed date and time on 'Copy from My Screens' modal
