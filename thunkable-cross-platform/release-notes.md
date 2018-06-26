# Release Notes

### TBD

New components

* [Alert](create/components/user-interface/alert.md) - launches a dialog / notification with a message and one or more buttons

### June 12, 2018

Bug fixes

* Solves some issues with Thunkable Live app on Android
* Reduces project saving issues

### June 5, 2018

**Thunkable Cross-Platform ✕ launches out of beta!**

Platform updates

* Renaming components is now supported. Click on the top of the properties panel to edit the component name
* Each new project can be set to [public or private](create/public-vs-private-projects.md).  Public projects are eligible to be featured in the Thunkable Gallery and can be shared in both [read-only](share.md#share-a-read-only-version-of-your-app-project) and fully-editable mode
* Sample apps now featured on the project list page
* Supports iOS usage descriptions for describing to users why certain permissions are needed when they download your app; applies only when you Publish to the iOS App Store

Component updates

* Switch component no longer needs blocks to set-up

### May 22, 2018

Component updates

* [Map](create/components/location/map.md) - adds new block events e.g. on Map Click, on Marker Click and supports the ability to add markers, polylines and polygons
* [Text to Speech](https://docs.thunkable.com/x/components/artificial-intelligence/text-to-speech.html) - increase supported languages from 6 to 87
* [Share](create/components/social/share.md#share-an-image) - now supports sharing locally stored assets \(does not work on Live Test for iOS\)

New components

* [Location Sensor](create/components/location/location-sensor.md) - gets user's current location
* [Slider](create/components/user-interface/slider.md) - UI element of choice for letting users select a value or range from a fixed set of options, such as setting the brightness of a screen

### May 15, 2018

Platform updates

* [Five new tutorials](get-started/tutorials.md) for Thunkable beginners now located in platform panel on the left
* [Share a read-only version](share.md#share-a-read-only-version-of-your-app-project-by-link) of your project is now supported with a public option

Bug fixes

* \(Background\) Image for Screens, Rows, Column and Image components now appear in Live Testing when using a Screen.start block
* Image height or width set to 'fit contents' now appear in Live Testing
* Improvements to Download / Publish for iOS including transparency support for app icons and better error messaging
* Improved messaging for Download for Android

### May 7, 2018

Platform updates

* Significant user interface update including a new Design / Blocks switch, add Components shifted to the left panel and Properties shifted to the right panel
* Live app now lets you [live preview](live-test.md#live-preview-android-only) all your app projects from the comfort of your mobile device \(Android only\)
* [Publish for Android](publish.md#publish-to-the-play-store-android) now supported
* Adds [version support](https://docs.thunkable.com/x/5-publish.html#step-⑤--send-your-app-to-itunes-connect-on-thunkable) for download / publish for Android and iOS
* Updated [download](download.md#download-and-install-ios-app) and [publish](publish.md#publish-to-the-app-store-ios) emails for iOS

### April 12, 2018

Component updates

* [Button](create/components/user-interface/button.md) - supports a number of new properties including sizing \(height, width\) and adding a background picture

New components

* [Speech Recognizer](create/components/voice/speech-recognizer.md) - uses artificial intelligence to recognize and translate spoken language into text in 14 different languages
* [Share](create/components/social/share.md) - allows users to share text or post images using their favorite installed communication app from Slack and Facebook to iMessage and WhatsApp
* [Switch](create/components/user-interface/switch.md) - popular UI element to turn on and off a certain feature in an app, often used in settings pages

Platform updates

* Updated Blocks colors

### Apr 5, 2018

New components

* [Spreadsheet](create/components/data/spreadsheet.md) by Airtable - gets, uploads, updates and deletes data from the popular spreadsheet service
* [Payment](create/components/monetization/payment.md) by Stripe - enable accepting credit card payments in app powered through Stripe; Each payment is subject to a 4.9% + $0.30 per transaction fee

Platform updates

* Supports opening installed app by deep link on Android \(aka Activity Starter\) via a Control block
* Blocks now includes zoom control and a better location for the trash can
* Properties have been re-organized into hopefully easier to use categories

### Mar 20, 2018

Platform updates

* [Custom app package name ](create/package-name-+-bundle-id.md)/ bundle ID now supported for both Android and iOS; app icon also supported for Android
* [Make a copy ](create/make-copy.md)of your project aka checkpoint in one click
* Tracking of project [shares](share.md) now available on project page; share links no longer require a user to be logged in

Component updates

* Properties now set / changeable in blocks including all Text / Background Color properties for visible components and Language properties for [Translator](create/components/voice/translator.md), [Text to Speech](create/components/voice/text-to-speech.md) and [Assistant](create/components/voice/assistant.md)
* Transparent color now available as a color property across all visible components
* Easy select and upload via Picture property for [Image](../thunkable-classic-android/create/components/image/) component

Bug fixes

* Function blocks now work again
* Blocks strings now accepted as numbers
* Changing dropdown component in blocks or duplicating blocks now keeps the same property

### Mar 6, 2018

New component

* [Sign In](https://github.com/thunkable/thunkable-docs/tree/4a752596e288fca776105e94dc5e863bb9a3e25a/ios/components/screen-layout/authentication/sign-in.md) powered by Firebase - support for email sign-in; set-up requires entering in an API key and database URL into app settings
* [Media Database](create/components/data/media-db.md) powered by Cloudinary - support for image, audio and video upload

Component updates

* Most Visible components \(Screen, TextInput, Label, Column, Row, Image, ListViewer, WebViewer, Maps, Google Maps\) - advanced properties including padding, margin, border & user location \(Maps / Google Maps\) added 
* [Realtime DB](create/components/data/realtime-db.md) powered by Firebase - changes set-up from adding a .plist file to entering in an API key and database URL into app settings

Platform updates

* Installing an Android .apk no longer requires uninstalling the Thunkable companion app
* Easier discoverability of uploading files \(now in the bottom left under the component tree
* Error message when dropping a Navigator or Screen to the Phone previewer; they can only be added to the Visible components section of the tree
* Small updates to sharing by link and notifications during download and publish

### Feb 23, 2018

Start of Thunkable Cross-Platform **✕** public beta

