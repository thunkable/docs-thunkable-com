# App Settings

To view or change your app settings, click on the **Settings** gear icon in the menu on the left.

![](<.gitbook/assets/App Settings.png>)

## 1. Project Settings

### App Description

This is a description of your app and how you intend it to be used. It is not necessary to fill this out in Thunkable. If you [publish](publish.md) your app you will need to enter this information, whether on Thunkable or the App Store or Play Store.

### App Name

Your app name is the name you choose for your app. It differs from the project name, which displays at the top of your project. While the project name is internal and may include details specific to your team, the app name is user-facing.

The app name is the name that is displayed on the Google Play Store or Apple App Store, and that users see when they install your app on their device. This name is also used to set the page title when you publish as a [web app](publish-as-a-web-app-pro.md).&#x20;

We recommend a short one or two word app name.

{% hint style="warning" %}
Avoid using the character "&" in your app name: at the moment, it prevents your app from being installed on your device
{% endhint %}

### Default App Layout <a href="#default-app-layout" id="default-app-layout"></a>

{% hint style="info" %}
Building an app in **Tablet View** is a Pro feature. [Learn more about Pro.](https://thunkable.com/#/pricing)
{% endhint %}

This is where you can change the default designer layout for your app. Use this dropdown to set the default size of your project, choosing from the following options:&#x20;

* Phone + Portrait
* Phone + Landscape
* Tablet + Portrait
* Tablet + Landscape

{% hint style="warning" %}
We recommend setting your Default App Layout before you start adding components to your app. Your layout will not automatically respond when you change your Default App Layout. Your existing components will not change size, and the distance between components will not change.&#x20;

We recommend choosing a Default App Layout before you start adding components to your screen(s).
{% endhint %}

![](.gitbook/assets/defaultlayoutsettings-2.png)

### Icon

Your app icon is the picture that represents your app on your mobile device. This icon will also appear on your listing in the Google Play Store or App Store, and as your project icon on Thunkable. Users on our personal plans will see the default "Made with Thunkable" icon appear when their apps load.&#x20;

{% hint style="info" %}
If your company needs to remove the Thunkable branding from an app, this option is available as a project setting to Business and Team customers.

[Learn more about our plans.](https://thunkable.com/#/pricing)
{% endhint %}

Please ensure the file you upload does not have the same name as another asset you use in your app. This will cause an error.

#### Best Practices&#x20;

| Property  | Setting                                       |
| --------- | --------------------------------------------- |
| Size      | 192 x 192 px (minimum)                        |
| Shape     | Square (equal height and width)               |
| File Type | Preferably .png (vs. jpg or other file types) |

For publishing to the iOS [App Store](publish-to-app-store-ios/#upload-an-icon-and-enter-your-build-number-and-version-number), you will also need an app icon that does not have any transparency, or it may cause an error.

{% hint style="info" %}
For publishing your app to the Play and App stores, you will need to create a separate icon with a higher resolution. For [Google Play](https://developer.android.com/google-play/resources/icon-design-specifications#creating\_assets), the current requirement is 500 x 500 px. For the [App Store](https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/app-icon#app-icon-sizes), it's 1024 x 1024 px.
{% endhint %}

## 2. Splash Screen Image

To access your app's splash screen image settings:

1. Navigate to the project’s **Design tab**.
2. Click the **Settings** icon in the left menu.
3. Click the **three dots icon** at the bottom of the Project Settings section to access the advanced settings.

![](<.gitbook/assets/splash screen image settings.png>)

### Picture

To customize your app’s splash screen picture:

1. Click in the Picture field.
2. Click **Upload files** and select an image from your computer, or select an image from your app’s current assets.

#### Splash Screen Picture Requirements:

* The picture must be square. Rectangle pictures will not render correctly.
* The ideal dimensions for your splash screen picture are 1152x1152 pixels.&#x20;
* If you want a transparent background, a PNG file is recommended.
* [Android splash screen image dimension guide](https://developer.android.com/develop/ui/views/launch/splash-screen#dimensions)

{% hint style="info" %}
**Note:** If you do not select a custom splash screen picture, your app icon image will be used by default.&#x20;
{% endhint %}

### Background Color

To customize the background color of your app’s splash screen:

1. Click in the Background Color field.
2. Use the color picker or input the HEX or RBGA codes to select your preferred color.

{% hint style="info" %}
**Note:** If you do not select a custom splash screen background color, white will be used by default.&#x20;
{% endhint %}

### Sample Splash Screens

<div align="left">

<figure><img src=".gitbook/assets/splash screen - iOS vs. Android.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

## 3. Publishing Settings

### App (Bundle) ID

A unique identifier for your app on the [App Store](publish-to-app-store-ios/#register-an-app-id-on-app-store-connect) or [Play Store](publish-to-play-store-android.md#the-package-name).&#x20;

This should follow a pattern like `com.domain.creatorname.appname`

Make sure none of the segments of this package name begins with a number.\
﻿Ensure none of the letters in this package name has an accent (e vs ë).

### Public App

PRO Thunkable users have the option to set their app to Private. A private app will not be displayed in the Thunkable Public Gallery. [Learn more about Thunkable PRO here.](https://thunkable.com/#/pricing)

### Auto-increment Version

When you publish to the [App Store](publish-to-app-store-ios/) or the [Play Store](publish-to-play-store-android.md), you will need to increment (increase) your version number each time. If this switch is set to `true,` Thunkable will automatically increment your project's version number each time you publish your app (iOS) or download your app (Android).

### Ignore Notch Area

This property enables you to remove the Safe Area View which Thunkable adds to the app automatically. If you set this property to be `true`, the screen background color will extend to full screen and there won’t be any white area. However, you need to manually take care of the notch in your app design, like adding extra space, in order to avoid the app element being blocked by the notch.

### Notch Area Background Color

This property enables you to set the safe area view color. With this, you can customize the background color of the _white area_. Please note, this is an app level setting and you won’t be able to customize the color at the screen level.

## 4. Android Publishing Details

### Version Name

Set a [version name](publish-to-play-store-android.md#build-and-version-number) for this version of your Android app.

### Version Code

Set a [version code](publish-to-play-store-android.md#build-and-version-number) for this version of your Android app.

## 5. iOS

### Version Number

Set a [version number](publish-to-app-store-ios/#set-a-version-number) for this version of your iOS app.

### Tracking Usage Description (iOS only)

If your app or any external service your app interacts with are gathering any kind of identifiable information, this must be explicitly disclosed to the end user of your app using an in-app prompt. If you do not include this and your app engages in tracking, Apple will reject your submission and ask you to resubmit while including an appropriate tracking string. To learn more about when to include a tracking string,[ click here.](https://intercom.help/thunkable/en/articles/5945318-nsusertrackingusagedescription-messages)

### iOS Permissions

When you add components that require permissions to your app, like the camera or map, you will need to add purpose strings to your app if you want to publish it to the App Store.&#x20;

You must add purpose strings for any component that explicitly requires a purpose string.

## 6. Integrations

If your app uses [translation](speech.md#translation), [image recognition](camera.md#image-recognition), [media upload to the cloud](camera.md#upload-image-to-the-cloud), or requires users to [sign in](sign-in.md), you can enter your personal API keys for these integrations in the app settings.&#x20;

### Firebase Settings

To learn more about the Firebase integration, please see here: [Firebase Sign-in](https://docs.thunkable.com/sign-in#firebase-sign-in).

### Google Map Settings

To learn more about the Google Map integration, please see here: [Map](https://docs.thunkable.com/map).

### AdMob Settings

#### iOS and Android App ID

Enter the AdMob app ID for your iOS and/or Android app. To learn more, see here: [Find your app IDs & ad unit IDs](https://support.google.com/admob/answer/7356431?hl=en).

#### Keystore

Import and export an Android Keystore to/from your app. Learn more about the Android Keystore here: [Publish to Android > Keystore](https://docs.thunkable.com/publish-to-play-store-android#the-keystore-private-key).

### Cloudinary Settings

To learn more about the Cloudinary integration, please see here: [Cloudinary](https://docs.thunkable.com/files#connecting-your-cloudinary-db-to-your-thunkable-project).
