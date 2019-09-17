# Push Notifications by One Signal

## PLEASE NOTE: 

**At this time Push Notifications can only be tested on Android Devices.**

**You can add Push Notifications to iOS apps but testing can only be done after an app is published to the App Store.** 

![One Signal is the world leader in push notifications and they offer their service for free. ](.gitbook/assets/onesignaldemo.png)

Push notifications are one of the biggest advantages that mobile apps have over  mobile websites, since they can send messages to users without the app being open. 

However, annoying notifications---those that are irrelevant and too frequent---can be dismissed or blocked easily.  We highly recommend sending notifications only when the content is relevant to the user. 

**Good examples**:

| App type | Frequency | Content |
| :--- | :--- | :--- |
| E-commerce | Sales | Coupon code |
| Game | App updates | Try this new level |

{% hint style="info" %}
**Push Notifications are a**  ![](.gitbook/assets/pro.png) **component.** While all Thunkers can add Push Notifications to their app projects and live test them in their apps \(Android only\), only PRO Thunkers can download and publish apps with Push Notifications.
{% endhint %}

{% hint style="danger" %}
Live Testing on Push Notifications is currently \(Sept. 2019\) not working as expected for all users. We're working to fix this, but for now please download your app to test and verify your OneSignal account.
{% endhint %}

{% hint style="info" %}
**Availability**

|  | Add to Project | Live Test | Download | Publish |
| :--- | :--- | :--- | :--- | :--- |
| Android | All Thunkers | All Thunkers | \*\*\*\*![](.gitbook/assets/pro.png) only | \*\*\*\*![](.gitbook/assets/pro.png) only |
| iOS | All Thunkers | Not available | Not available | ![](.gitbook/assets/pro.png) only |
{% endhint %}

## Sign up with One Signal

One Signal is a free service that supports unlimited devices and notifications. They make money by selling your users' data to 3rd parties.

* Go to [One Signal](https://onesignal.com/) and sign up for an account

![](.gitbook/assets/image%20%2873%29.png)

After you have signed up, click Add App and enter in your app name:

![](.gitbook/assets/image%20%2894%29.png)

![](.gitbook/assets/image%20%2837%29.png)

After adding your app, OneSignal will ask you to select a platform. Below, we have created guides for both Android and iOS.

**At this time Push Notifications can only be tested on Android Devices.**

**You can add Push Notifications to iOS apps but testing can only be done after an app is published to the App Store.** 

![](.gitbook/assets/screen-shot-2019-04-30-at-9.47.44-am.png)

## Android Setup

Setting up push notifications for Android is relatively straightforward. Here's a quick overview of the steps, followed by a more detailed walk-through.

1. [Select Your Platform](push-notifications-by-one-signal.md#1-choose-the-android-platform)
2. [Configure Your Platform](push-notifications-by-one-signal.md#2-set-up-a-firebase-project)
3. [Select Your SDK](push-notifications-by-one-signal.md#3-select-your-sdk)
4. [Install Your SDK](push-notifications-by-one-signal.md#5-install-your-sdk)

### 1. Select Your Platform

After you have added an app and given it a name, select the Google Android option.

![Click on &quot;Google Android&quot; to set up an Android app.](.gitbook/assets/screen-shot-2019-04-30-at-9.47.44-am.png)

### 2. Configure Your Platform

For this next step, you will need a [Firebase](https://firebase.google.com/) account. 

For instructions on how to set up a Firebase account, please click [here](https://docs.thunkable.com/realtime-db#set-up-your-own-firebase-account).

Once you are signed in with Firebase, create a new project.

![](.gitbook/assets/image%20%2819%29.png)

Once you have created a new project, click on the gear icon beside Project Overview and select **Project settings**.

![](.gitbook/assets/screenshot-2019-05-01-at-11.23.28.png)

Select the Cloud Messaging option:

![](.gitbook/assets/image%20%2856%29.png)

There are two things that you will need to copy and paste back into One Signal:

1. Server Key
2. Sender ID

![](.gitbook/assets/image%20%2888%29.png)

Go back to the **One Signal** platform.

Earlier you should have selected the Android option on One Signal, and your screen should look like this:

![](.gitbook/assets/image%20%284%29.png)

Copy and paste the Firebase Server Key and the Firebase Sender ID sections into One Signal.

### 3. Select Your SDK

The last thing you need to do in OneSignal is choose your target SDK. Select **Native Android** and click next to continue. 

![](.gitbook/assets/screenshot-2019-05-01-at-11.32.34.png)

### 4. Install Your SDK

Copy the alpha numeric code that OneSignal generates called **Your App ID** in the image below.

![](.gitbook/assets/screenshot-2019-05-01-at-11.34.39.png)

On Thunkable, drag and drop the Push Notifications component into your app.

On the right hand side, paste the code from One Signal into the Android App ID section. 

![](.gitbook/assets/android.png)

Click the Live Test button. Once the app is on your phone, go back to One Signal. Click the "Check Subscribed Users" button.

![](.gitbook/assets/image%20%2897%29.png)

If you are live testing or have downloaded your Android app, you should see a congratulations message. Click "DONE".

Select the "MESSAGES" option and then select "NEW PUSH". You will now be able to create push notifications and send them to your app users.

![](.gitbook/assets/image%20%28106%29.png)

##  iOS Setup

Setting up push notifications involves a few more steps on iOS than on Android, but every step is covered in detail below. 

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

When you are ready to send your first push notification, select the "MESSAGES" option and then select "NEW PUSH". You will now be able to create push notifications and send them to your app users.



![](.gitbook/assets/image%20%28106%29.png)

