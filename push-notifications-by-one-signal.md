# Push Notifications by OneSignal

## Overview

Push notifications are one of the biggest advantages of mobile apps over mobile websites since they can send messages to users without the app being open.&#x20;

However, notifications that are irrelevant and too frequent are often dismissed or blocked.  We highly recommend sending notifications only when the content is relevant to the user. Examples include an e-commerce app letting the user know about a sale, or a game app letting the user know about a new level or feature.

Thunkable utilizes the services of [OneSignal](https://onesignal.com/) to facilitate push notifications from your app. OneSignal is a free service that supports unlimited devices and notifications. You can learn more about their features here: [OneSignal pricing page](https://onesignal.com/pricing).

{% hint style="info" %}
**Push Notifications are available on Thunkable Pro, Business, and Team plans.** While all Creators can add Push Notifications to their projects and live test them in their Android apps, only Creators on the previously mentioned plans can download and publish apps with Push Notifications. See our [pricing page](https://thunkable.com/#/pricing) for more details.
{% endhint %}

## Add Push Notifications to your app

To add Push Notifications to your app :

1. Navigate to your project's **Blocks tab**.
2. Locate **Push Notification** under the App Features heading.
3.  Click the **gear icon** next to Push Notification.\


    <div align="left">

    <img src=".gitbook/assets/push-notifications.png" alt="">

    </div>
4.  The Push Notification settings modal opens. This is where you will enter your OneSignal Android App ID and OneSignal iOS App ID to configure the connection between OneSignal and your Thunkable project. \


    <div align="left">

    <img src=".gitbook/assets/push notifications modal in Thunkable.png" alt="" width="563">

    </div>

    {% hint style="info" %}
    **Geolocation Permissions** - OneSignal allows you to push messages to users based on their location. In order to do that, you need permission from your users to register their location. Use the toggle in the Push Notification settings to indicate whether you want to request users share their location with OneSignal.
    {% endhint %}


5. The remainder of this document will assist you with:
   1. [Creating a OneSignal Account](push-notifications-by-one-signal.md#create-a-onesignal-account)
   2. [Creating a OneSignal App](push-notifications-by-one-signal.md#create-a-onesignal-app)
   3. [Configuring for Android](push-notifications-by-one-signal.md#android-configuration)
   4. [Configuring for iOS](push-notifications-by-one-signal.md#ios-configuration)

## Create a OneSignal Account

1. Go to [**OneSignal**](https://onesignal.com/).
2. Click **Sign Up**.
3. Create your account and complete the OneSignal onboarding.

## Create a OneSignal App

1.  If you didn't create an app as part of the OneSignal onboarding, navigate to your OneSignal dashboard and click **+ New App/Website**.\


    ![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.56.19 PM.png>)



    {% hint style="info" %}
    If you intend to send push notifications to your app's users on Android and iOS you will need to create a new app in OneSignal for each, Android and iOS.
    {% endhint %}
2. Enter your **app name**. We recommend including the platform in your app name, for example, Employee Directory - Android or Employee Directory - iOS.&#x20;
3.  Select **Apple iOS (APNs)** or **Google Android (FCM)**.\


    ![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.58.03 PM.png>)
4. Click **Next: Configure Your Platform**.
5. Follow the platform-specific configuration instructions below.
   1. [Android Configuration](push-notifications-by-one-signal.md#android-configuration)
   2. [iOS Configuration](push-notifications-by-one-signal.md#ios-configuration)

## Android Configuration

1. If you don't already have one, create a [**Firebase**](https://firebase.google.com/) account. Instructions for getting started with Firebase are available here: [Firebase Account Setup](https://docs.thunkable.com/sign-in#getting-started).
2. Follow OneSignal's instructions to generate a Firebase Server API key for sending Android App Notifications here: [Android: Firebase Credentials](https://documentation.onesignal.com/docs/generate-a-google-server-api-key).
3. In OneSignal, select **Native Android** as your target SDK.
4.  Click **Save & Continue**.\


    <div align="left">

    <img src=".gitbook/assets/Screen Shot 2022-02-17 at 12.13.24 AM.png" alt="">

    </div>
5.  Copy **Your App ID**.\


    ![](.gitbook/assets/app-id.png)
6. Return to the Blocks tab of your Thunkable project. Do not close the OneSignal tab.&#x20;
7. Click the **gear icon** next to Push Notification.
8. In the **Android App ID** field, paste **Your App ID** that you copied from OneSignal in step 5.&#x20;
9.  Click **Submit**.\


    <div align="left">

    <img src=".gitbook/assets/push notifications modal in Thunkable.png" alt="" width="563">

    </div>
10. Click the **Live Test on Device** icon and open the Thunkable Live app on your device.
11. Return to your **OneSignal** tab.&#x20;
12. Click **Check Subscribed Users.**\


    <figure><img src=".gitbook/assets/OneSignal - Check Subscribed Users.png" alt=""><figcaption></figcaption></figure>
13. If the configuration was successful, you will see a congratulations message.
14. Click **Done**.&#x20;
15. To send push notifications to your app's Android users, see this section: [Send Push Notifications](push-notifications-by-one-signal.md#send-push-notifications).

## &#x20;iOS Configuration

1. Follow OneSignal's instructions to generate a p8 certificate: [iOS: p8 Token-Based Connection to APNs](https://documentation.onesignal.com/docs/establishing-an-apns-authentication-key).
2. In OneSignal, select **Native iOS** as your target SDK.
3.  Click **Save & Continue**.\


    <figure><img src=".gitbook/assets/OneSignal - Native iOS SDK.png" alt=""><figcaption></figcaption></figure>
4.  Copy **Your App ID**.\


    <figure><img src=".gitbook/assets/OneSignal - Apple iOS - Your App ID.png" alt=""><figcaption></figcaption></figure>
5. Return to the Blocks tab of your Thunkable project. Do not close the OneSignal tab.&#x20;
6. Click the **gear icon** next to Push Notification.
7. In the **iOS App ID** field, paste **Your App ID** that you copied from OneSignal in step 4.&#x20;
8.  Click **Submit**.\


    <div align="left">

    <figure><img src=".gitbook/assets/push notifications modal in Thunkable.png" alt="" width="563"><figcaption></figcaption></figure>

    </div>

## Send Push Notifications

Once you have your platforms configured in OneSignal you can create and sent push notifications to your app's users. Follow OneSignal's instructions here: [Sending Messages](https://documentation.onesignal.com/docs/sending-notifications#sending-push-notifications-from-onesignal-dashboard).

## Blocks

### Functions

#### User ID

![](<.gitbook/assets/Screen Shot 2022-01-10 at 1.08.59 PM.png>)

This block returns the unique user ID of the device.
