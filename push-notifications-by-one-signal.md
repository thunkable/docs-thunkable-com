# Push Notifications by One Signal

![One Signal is the world leader in push notifications and they offer their service for free. They make money by selling your users&apos; data to third parties](.gitbook/assets/onesignaldemo.png)

Push notifications are one of the biggest advantages that mobile apps have over their mobile website counterparts since they can send a message to a user without an app being open. However, annoying notifications, those that are irrelevant and too frequent, can be dismissed our block easily so we highly recommend sending notifications only when the content is relevant to the user.

| App type | Frequency | Content |
| :--- | :--- | :--- |
| E-commerce | Sales | Coupon code |
| Game | App updates | Try this new level |

{% hint style="info" %}
**Push Notifications are a** ![](.gitbook/assets/pro.png) **component.** While all Thunkers can add Push Notifications to their app projects and live test them in their apps, only PRO Thunkers can download and publish apps with Push Notifications.
{% endhint %}

Most of the work you do to use push notifications in your app will be on the One Signal interface. On Thunkable, you simply drag and drop the component in and add the One Signal Android and/or iOS key\(s\).

## Sign up with One Signal

One Signal is a free service that supports unlimited devices and notifications. They make money by selling your users' data to 3rd parties.

* Go to [One Signal](https://onesignal.com/) and sign up for an account
* Add a new app

After you have added a new app, you'll likely see a screen like the one below:

![](.gitbook/assets/screen-shot-2019-04-30-at-9.47.44-am.png)

Thunkable currently supports Apple iOS and Google Android.

## Android Set Up

Setting  up push notifications for Android is relatively straightforward. Here's a quick overview of the steps, followed by a more detailed walk-through.

![By the end of this tutorial you should have an Android\_AppID to add to your Thunkable project.](.gitbook/assets/android.png)

1. [Select Your Platform](push-notifications-by-one-signal.md#1-choose-the-android-platform)
2. [Configure Your Platform](push-notifications-by-one-signal.md#2-set-up-a-firebase-project)
3. [Select Your SDK](push-notifications-by-one-signal.md#3-select-your-sdk)
4. [Install Your SDK](push-notifications-by-one-signal.md#5-install-your-sdk)

### 1. Select Your Platform

When you create a new OneSignal project it ask you what platform your want are using. In this dialog choose "Android"

![Create a new app and give it a name.](.gitbook/assets/screenshot-2019-05-01-at-11.20.30.png)

![Click on &quot;Google Android&quot; to set up an Android app.](.gitbook/assets/screen-shot-2019-04-30-at-9.47.44-am.png)

### 2. Configure Your Platform

We you go to configure your platform you will be prompted for a **Firebase Server Key** and a **Firebase Sender ID.** As the name implies, you will need a firebase account to provide this information.

![](.gitbook/assets/screenshot-2019-05-01-at-11.21.33.png)

We have more extensive documentation on setting up a Firebase account, if you don't have one already you can read that [here](realtime-db.md#set-up-your-own-firebase-account).

Once you have created a new project click on the gear icon beside Project Overview and open your **Project settings**.

![](.gitbook/assets/screenshot-2019-05-01-at-11.23.28.png)

In your project settings, click on the **Cloud Messaging** tab where you can find both your server key and sender ID. Copy both of these and go back to OneSignal.

### 3. Select Your SDK

The last thing you need to do in OneSignal is choose your target SDK. Select **Native Android** and click next to continue. 

![](.gitbook/assets/screenshot-2019-05-01-at-11.32.34.png)

### 4. Install Your SDK

Copy the alpha numeric code that OneSignal Generates called **Your App ID** in the image below.

![](.gitbook/assets/screenshot-2019-05-01-at-11.34.39.png)

Paste this ID into your Thunkable project and download your .apk. You're now ready to start sending Push Notifications to your Android users.

![](.gitbook/assets/android.png)

##  iOS Set Up

Setting up push notifications involves a few more steps on iOS than on Android, but every step is covered in detail below. 

![By the end of the walk through you will have and IOS\_AppID you can use in your app.](.gitbook/assets/ios.png)

1. [Select Platform](push-notifications-by-one-signal.md#1-select-platform)
2. [Configure Platform](push-notifications-by-one-signal.md#2-configure-platform)
3. [Select SDK](push-notifications-by-one-signal.md#3-select-sdk)
4. [Install SDK](push-notifications-by-one-signal.md#4-install-sdk)

### 1. Select Platform

Get started by creating a new app. You need to do this even if your Thunkable project is intended for both iOS and Android. 

![](.gitbook/assets/newapp.png)

After that, choose **Apple iOS** as your platform.

![](.gitbook/assets/screenshot-2019-05-01-at-13.13.07.png)

### 2. Configure Platform

OneSignal have provided [extensive documentation](https://documentation.onesignal.com/docs/generate-an-ios-push-certificate) on how to find your **Production Certificate .p12 file** as well as your **Production Private Key Password**. The most important steps are outlined below.

To begin, open the [OneSignal Provisionator](https://onesignal.com/provisionator) webpage. This tool will generate a .p12 file and the accompanying password for you.

![](.gitbook/assets/onesignalportal.png)

Follow the on screen instructions. Enter your Apple Developer ID and password. This portal works with 2FA enabled as well. If prompted, enter your 2FA code. Choose your team and the relevant Bundle ID and click generate. 

{% hint style="warning" %}
You must be a Team Administrator to generate the files
{% endhint %}

You can now download the .p12, .cer and .pem files that are generated for you.

{% hint style="warning" %}
Don't forget to save your password somewhere safe.
{% endhint %}

Click on **Apple iOS** 

![](.gitbook/assets/screenshot-2019-05-01-at-13.31.08.png)

With that completed you can upload your .p12 file and enter the password in OneSignal. Click **Save** to proceed to the next step.

![](.gitbook/assets/screenshot-2019-05-01-at-13.17.37.png)

### 3. Select SDK

Click on **Native iOS**  to choose the SDK you wish to target. Then click **Next** to generate your App ID.

![](.gitbook/assets/screenshot-2019-05-01-at-13.17.49.png)

### 4. Install SDK

Copy the alpha-numeric code labeled **Your App ID** and head back to Thunkable.

![](.gitbook/assets/screenshot-2019-05-01-at-13.19.03.png)

Paste your ID in the **IOS\_AppID** field and you're almost done. In order to now publish your app your will have to create a .mobileprovision profile. You can find details of how to do this on the ["Publish to App Store" page](publish-to-app-store-ios.md#adding-push-notifications).

![](.gitbook/assets/screenshot-2019-05-01-at-13.19.25.png)

