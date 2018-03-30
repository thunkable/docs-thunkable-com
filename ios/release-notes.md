#### **Thunkable for iOS **

# Release Notes

---

#### Apr 2, 2018 

New components

* [Location Sensor](/android/components/location/location-sensor.md) - gets a user's current location and with permission of the user, can track a user's location history, both when the app is open and when it is in the background
* [Spreadsheet](/ios/components/data-storage/spreadsheets.md) by Airtable - gets, uploads, updates and deletes data from the popular spreadsheet service
* [Payment](/ios/components/monetisation/payments.md) by Stripe - enable accepting credit card payments in app powered through Stripe; Each payment is subject to a 4.9% + $0.30 per transaction fee

Platform updates

* Blocks now includes zoom control and a better location for the trash can
* Properties have been re-organized into hopefully easier to use categories

---

#### Mar 20, 2018 `v32`

Platform updates

* [Make a copy](/ios/components/make-copy.md) of your project aka checkpoint in one click
* Tracking of project [shares](/ios/6-share.md) now available on project page; share links no longer require a user to be logged in

Component updates

* Properties now set / changeable in blocks including all Text / Background Color properties for visible components and Language properties for [Translator](/ios/components/voice/translator.md), [Text to Speech](/ios/components/voice/text-to-speech.md) and [Assistant](/ios/components/voice/assistant.md)
* Transparent color now available as a color property across all visible components
* Easy select and upload via Picture property for [Image](/android/components/image/README.md) component

Bug fixes

* [Function](/ios/blocks/functions.md) blocks now work again
* Blocks strings now accepted as numbers
* Changing dropdown component in blocks or duplicating blocks now keeps the same property

---

#### Mar 6, 2018 `v31`

New component

* [Sign In](/ios/components/screen-layout/authentication/sign-in.md) powered by Firebase - support for email sign-in; set-up requires entering in an API key and database URL into app settings
* [Media Database](/ios/components/data-storage/media-db.md) powered by Cloudinary - support for image, audio and video upload

Component updates

* Most Visible components \(Screen, TextInput, Label, Column, Row, Image, ListViewer, WebViewer, Maps, Google Maps\) - advanced properties including padding, margin, border & user location \(Maps / Google Maps\) added 
* [Realtime DB](/ios/components/data-storage/realtime-db.md) powered by Firebase - changes set-up from adding a .plist file to entering in an API key and database URL into app settings

Platform updates

* Easier discoverability of uploading files \(now in the bottom left under the component tree\)

* Error message when dropping a Navigator or Screen to the Phone previewer; they can only be added to the Visible components section of the tree

* Small updates to sharing by link and notifications during download and publish

---

#### Feb 23, 2018 `v30`

New component

* [Lottie](/ios/components/image/lottie.md) - support for very popular component that renders After Effects animations in real time, allowing apps to use animations as easily as they use static images

Platform updates

* More descriptive email messages for download and publish

---

#### Feb 2, 2018 `v28`

New component

* [Google Maps](/ios/components/location/google-maps.md) - basic support for Google Maps; more features to be added in the future

Bug fix

* Enables invisible components to be blocked on other screens besides Screen 1
* Fixes some issues with disappearing blocks

---

#### Jan 14, 2018 `v27`

Bug fix

* Live app now supports login from iOS 9 and 10

---

#### Jan 10, 2018 `v26`

Component updates

* [Translator](/ios/components/voice/translator.md) powered by Yandex - adds supports for all 84 languages supported by Yandex from 14
* [Realtime Database](/ios/components/data-storage/realtime-db.md) powered by Firebase - adds support for a user's private database instance
* [Screen](/ios/components/screen-layout/screen.md) -- adds support for background color, picture, scrolling and hiding status bar
* [Row](/ios/components/screen-layout/layout/row.md) -- adds support background color and picture
* [Column](/ios/components/screen-layout/layout/column.md) -- adds support background color and picture

Live testing updates \(please download the latest version\)

* To [live test](/ios/live-test.md), user first logins to their app and then clicks Live Test on the platform; there is no longer any need to scan a QR code

Platform improvements

* Add ability to rename projects from project page
* Improved component hierarchy with collapsible trees
* Improved add component organization with component categories
* Improved top right header including links to documentation, tutorials and community forum
* Removed the ability to add assets by dragging and dropping anywhere; Users can still add assets by [following these directions](/ios/components/app-settings/upload-media.md)

---

#### Dec 18, 2017 `v25`

Platform improvements

* Users in blocks view stay in blocks view when selecting a component

---

#### Dec 13, 2017 `v24`

Platform improvements

* [Share](/ios/6-share.md) your app project by link
* Added Blocks tab when selecting invisible components
* Alert users who don't have cookies enabled during login

Bug fix

* Fixed bug that prevented events within a single block from triggering in sequence

---

#### Dec 5, 2017 `v23`

Bug fix

* Fixed bug that disabled function blocks

---

#### Dec 1, 2017 `v22`

Platform

* Add any component by dragging and dropping them onto the phone OR in the appropriate part of the app hierarchy
* Remove a component by selecting the trash can within each component
* View your custom app icon on the project page or on the app setting of the Designer; custom app icon must be uploaded into the app project settings
* Separate entrance for Hour of Code \([code.thunkable.com](http://code.thunkable.com)\)

---

#### Nov 22, 2017 `v21`

New components

* [Sound](/ios/components/voice/sound.md) to play your favorite sounds
* [Timer](/ios/components/user-interface/sensors/timer.md) to trigger events at certain times
* [Text to Speech](/ios/components/voice/text-to-speech.md) to speak aloud text in a variety of languages
* [Translator](/ios/components/voice/translator.md) powered by Yandex to translate text between a number of languages
* [Assistant](/ios/components/voice/assistant.md) powered by Dialogflow to speak aloud pre-determined answers to users natural language questions
* [Image Recognizer](/ios/components/image/image-recognizer.md) powered by Microsoft to describe the content of photos

Platform

* [Publish](/ios/publish.md) your app to the App Store; requires an Apple Program Developer membership \(currently costs $99/year\)

---

#### Nov 6, 2017 `v19`

New components

* [Web API](/ios/components/storage/web-api.md) to retrieve and post data to your favorite web services

Component updates

* [Button](/android/components/user-interface/button.md)  - additional styling options like background color, text size; also adds long click, touch up and touch down events
* [Text Input](/ios/components/user-interface/text-input.md) - hides keyboard when user hits return or clicks outside the keyboard; also adds ability to accept numbers only, email addresses or open the phone keypad

---

#### Nov 2, 2017 `v18`

Platform improvements

* Tablet and smartphone support for drag and drop of components and blocks
* [Upload media](/ios/components/app-settings/upload-media.md) by dragging and dropping files to any part of Thunkable platform screen

New components

* [Camera](/ios/components/media/camera.md) to take photos
* [Photo Library](/ios/components/media/photo-library.md) aka Image Picker to select photos from the device
* [Realtime DB](/ios/components/storage/realtime-db.md) powered by Firebase to save and retrieve data in a cloud database and update data in realtime 

New blocks

* [Objects](/ios/blocks/objects.md) blocks to format data retrieved from outside Web services APIs

---

#### Sep 25, 2017 `v16`

Platform updates

* [Download to phone](https://docs.thunkable.com/ios/download.html#step-4-download) - link only active for 24 hours

New blocks

* Screen Starts - triggers events when a screen first opens \(similar to Screen.Initialize in Android\)

---

#### Sep 15, 2017 `v15`

Platform updates

* [Custom icon and app name](/ios/components/app-settings/custom-icon-+-app-name.md)

---

#### Sep 13, 2017 `v14`

Platform updates

* [Drag and drop to add components](https://docs.thunkable.com/ios/create.html#step-5：-add-app-components)
* [Download to phone](//ios/download.md#step-4-download)
* [Thunkable live testing app](http://appstore.com/thunkablelive) on the App Store
* Ability to [add multiple Screens](https://docs.thunkable.com/ios/components/user-interface/screen.html#add-multiple-screens-under-a-navigator)
* Remove whitelist requirement

New components

* [Navigators](/ios/components/navigators/README.md) - Drawer, Tab, Stack
* [List Viewer](/ios/components/user-interface/list-view.md)
* [Local Storage](/ios/components/storage/local-storage.md) - our first Invisible component



