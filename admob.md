# Ads by AdMob

{% hint style="info" %}
**AdMob is a**  <img src=".gitbook/assets/pro.png" alt="" data-size="line"> **component.** All Thunkers can add AdMob to their projects and live test the ads in their apps. Only PRO Thunkers can download and publish apps that contain ads. To get started, [join our MCM network](https://docs.google.com/forms/d/e/1FAIpQLSf3DSZ\_Uon406Demqt\_pxJb1fiQRc6IT49CYf19bJr8VG40SQ/viewform?pli=1).
{% endhint %}

## 1. AdMob Overview&#x20;

<div align="left">

<img src=".gitbook/assets/webp.net-resizeimage.png" alt="">

</div>

AdMob is the most popular ad network for monetizing mobile apps today.&#x20;

Apps with large audiences can use AdMob to not only generate revenue for the creator, but in some cases, create better user experiences. For example, users may prefer to watch a [Rewarded Video Ad](admob.md#rewarded-video-a-d) to unlock extra content than pay money to unlock extra content.

We **highly recommend** that you only add ads to your app after it has been completed and you have a good idea of how users will move through your app. Once your app is complete, you can go back in find natural points to add the different types of ads for your users.

## 2. Setup Your AdMob Account

You need an [AdMob account](https://admob.google.com/home/get-started/) to show ads in your project.

Once you have an AdMob account, you will need to paste the following into the [AdMob section of your Project Settings](settings/project-settings/#admob-settings):

* [iOS app ID](https://support.google.com/admob/answer/7356431?hl=en) (if publishing to App Store)
* [Android app ID](https://support.google.com/admob/answer/7356431?hl=en) (if publishing to Play Store)
* [Tracking Usage Description](https://developer.apple.com/app-store/user-privacy-and-data-use/) (if publishing to App Store)
  * Default value: "This identifier will be used to deliver personalized ads to you."

![](<.gitbook/assets/Screenshot 2023-02-16 at 4.29.28 PM.png>)

Once you have published your app, you will also need individual [Ad Unit IDs](https://support.google.com/admob/answer/7356431?hl=en) for each AdMob component in your project. To add an Ad Unit ID:

1. Click on the Apps tab in your AdMob Sidebar
2. Click View All Apps
3. Click the name of the app associated with the ad unit.
4. Click on the Add Ad Unit button
5. Select the type of ad you wish to add (Note: Thunkable only currently supports Banner, Interstitial, or Rewarded Ads).
6. Add a name for your Ad Unit (e.g. "Banner Ad")
7. Click the Create Ad Unit button

![](<.gitbook/assets/Screenshot 2023-02-16 at 2.55.32 PM.png>)

### 3. Join Thunkable's MCM Network

To download and publish Thunkable apps that contain ads, you must first be a member of Thunkable's MCM (Multiple Customer Management) network.&#x20;

An invitation to this network will be sent to you the first time you submit your app for review. If you do not change AdMob accounts, this only needs to be done once, when you [submit your first app for review](https://docs.google.com/forms/d/e/1FAIpQLSf3DSZ\_Uon406Demqt\_pxJb1fiQRc6IT49CYf19bJr8VG40SQ/viewform?pli=1).

By joining this network, you consent to sharing 10% of your AdMob revenue for all apps you have currently on AdMob with Thunkable to support maintenance costs.

### 4. Submit Your App For Review

Thunkable has partnered with AdMob to ensure that apps created on our cross-platform use ads to monetize apps in a way that both provides high quality traffic to advertisers and a high quality user experience for end users of apps.

All apps with AdMob must be first approved by Thunkable before they can be downloaded or published. AdMob has its [own policies](https://support.google.com/admob/answer/7313578) that an app must comply with including but not limited to:&#x20;

* Inappropriate content that advertisers do not want to be associated with e.g. copyrighted, adult
* Invalid activity that lowers the quality of traffic to advertisers e.g. ad placements that encourage clicks

Thunkable will review apps for compliance with AdMob policies but will specifically **reject apps** that are:

* Incomplete apps - apps that are still in their early stages and won't show how ads will be used in the app
* Earning apps - apps that encourage users to clicks ads in exchange for some form of payment
* Auto-impression apps  - apps that repeatedly load banner ads in the background of apps
* Apps that show an Interstitial ad or Video ad on startup - these ads must be implemented properly in your app

**Thunkable reserves the right to change an app's approval status subject to any violation of our guidelines.**

If your app is rejected, the Thunkable AdMob team will send an email to the address used in your submission and you will be provided with an explanation and a recommendation for changes to make to get your app approved upon re-submission.

You are welcome to submit the same app for approval multiple times.

## 5. Types of Ads

### Banner ad

The Banner ad is a rectangular image or text ads that occupy a spot within an app's layout.&#x20;

AdMob banner ads are the simplest ad format to implement and are recommended for beginners. No blocks are needed to show your Banner ad to your end users.

The first banner ad will load when ready and will reload a new ad every minute.

There is a maximum of 1 Banner ad allowed per screen. You can show multiple banners in a single multi-screen app. You can learn more about best practices for implementing and using banners [here](https://support.google.com/admob/answer/6128877?hl=en).

<figure><img src=".gitbook/assets/Screenshot 2023-02-16 at 4.46.12 PM.png" alt=""><figcaption></figcaption></figure>

### Properties

#### AdMob Banner

| Name                 | Description                                                                                                                                | Data Type  |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------- |
| Ad Unit ID (Android) | Ad Unit ID for showing your ad on Android devices                                                                                          | Text       |
| Ad Unit ID (iOS)     | Ad Unit ID for showing your ad on iOS devices                                                                                              | Text       |
| Test Mode            | <p>Toggle whether real ads or sample ads should display in your app. <br><strong>Set this to true while testing your own app.</strong></p> | True/False |

#### Layout

| Name    | Description                                                                   | Data Type  |
| ------- | ----------------------------------------------------------------------------- | ---------- |
| Y       | Location of top left corner of Banner ad on Y-axis, where the top side is Y=0 | Number     |
| Visible | Set whether the Banner ad component is visible                                | True/False |

### Interstitial Ad

Interstitial ads are full-screen ads that cover the interface of their host app.&#x20;

These should displayed at natural transition points in the flow of an app, eg. between activities, between levels in a game. The user can click on or close the ad.

There is a limit of one interstitial ad component per app, but you can show the ad multiple times.

To show an interstitial app, you need to first add the component and then add the [Show Ad block ](admob.md#blocks)after the appropriate event in your app.

### Adding an Interstitial ad to your app

To add an Interstitial ad to your app:

1. Go to your Blocks tab&#x20;
2. Click on the icon next to the Ads drawer of blocks
3. Select **AdMob Interstitial**

![](<.gitbook/assets/Screenshot 2023-02-16 at 5.13.27 PM.png>)

### Properties

You will see a dialog where you can set the following properties:

| Name                 | Description                                                                                                                                | Data Type  |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------- |
| Ad Unit ID (Android) | Ad Unit ID for showing your ad on Android devices                                                                                          | Text       |
| Ad Unit ID (iOS)     | Ad Unit ID for showing your ad on iOS devices                                                                                              | Text       |
| Test Mode            | <p>Toggle whether real ads or sample ads should display in your app. <br><strong>Set this to true while testing your own app.</strong></p> | True/False |

### Blocks

<div align="center">

<figure><img src=".gitbook/assets/Screenshot 2023-02-16 at 3.36.44 PM.png" alt=""><figcaption></figcaption></figure>

</div>

#### Events

Use the **when Ad Open** and **when Ad Close** blocks to trigger events to happen when the interstitial ad opens or closes.

![](.gitbook/assets/admob-inter-blocks-events.png)

#### Functions

Use the **Show Ad** block to show an interstitial ad in your app. If there is an error, the **error** block will catch and return it.

![](.gitbook/assets/screen-shot-2021-04-08-at-4.00.50-pm.png)

#### Properties

Set and get [properties](admob.md#properties-1) of your Interstitial ad.

Ad Unit ID (Android):

<figure><img src=".gitbook/assets/Screen Shot 2021-04-08 at 4.01.14 PM copy.jpg" alt=""><figcaption></figcaption></figure>

Ad Unit ID (iOS):

![](.gitbook/assets/screen-shot-2021-04-08-at-4.01.14-pm-copy.jpg)

Test Mode:

![](.gitbook/assets/screen-shot-2021-04-08-at-4.01.14-pm.png)

## 6. R**ewarded Video** Ad <a href="#rewarded-video-a-d" id="rewarded-video-a-d"></a>

Rewarded Video Ads are full-screen video ads that users have the option of watching in full [in exchange for in-app rewards](https://support.google.com/admob/answer/7313578).&#x20;

Rewarded video ads are recommended after a user has completed a heavy task in your app and would be willing to watch a long video to continue.&#x20;

There is a limit of one rewarded video ad component per app, but you can show the ad multiple times.

To show a rewarded video app, you need to first add the component and then add the [`Show Ad` block ](admob.md#rewarded-video-ad-blocks)after the appropriate event in your app.&#x20;

You'll then want to add a [`Reward User` event](admob.md#rewarded-video-ad-blocks) to reward your user in the app. You can learn more about best practices for implementing and using Rewarded Video ads [here](https://support.google.com/admob/answer/7313578?hl=en).

### Adding a Rewarded Video ad to your app

To add an Rewarded Video ad to your app:

1. Go to your Blocks tab&#x20;
2. Click on the icon next to the Ads drawer of blocks
3. Select **AdMob Rewarded Video**

### Properties

You will see a dialogue where you can set the following properties:

| Name                 | Description                                                                                                                                | Data Type  |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------- |
| Ad Unit ID (Android) | Ad Unit ID for showing your ad on Android devices                                                                                          | Text       |
| Ad Unit ID (iOS)     | Ad Unit ID for showing your ad on iOS devices                                                                                              | Text       |
| Test Mode            | <p>Toggle whether real ads or sample ads should display in your app. <br><strong>Set this to true while testing your own app.</strong></p> | True/False |

### Blocks

#### Events

Use the **when Ad Close** block to trigger events to happen when the Rewarded Video ad closes.

![](<.gitbook/assets/admob-video-blocks-events (1).png>)

#### Functions

Use the **Show Ad** block to show the ad video, and the **Reward User** block to reward the user after displaying the video.

![](.gitbook/assets/screen-shot-2019-03-08-at-8.55.38-am.png)

#### Properties

Set and get [properties](admob.md#properties-2) of your Rewarded Video ad.

Ad Unit ID (Android):

![](.gitbook/assets/admob-video-blocks-android.png)

Ad Unit ID (iOS):

![](.gitbook/assets/admob-video-blocks-ios.png)

Test Mode:

![](.gitbook/assets/admob-video-blocks-testmode.png)

## 7. Live Test <a href="#live-test" id="live-test"></a>

For your convenience, we have provided a test  `Ad Unit ID` for you to see how a particular ad format may appear in your app. _You must change this to your own Publisher and Ad Unit ID before publishing._

During live test, all AdMob ads will be set to `test mode = true`, which means clicks and impressions will not be counted.&#x20;

This is true even if you add your own `Ad Unit ID` and set `test mode = false`.

## 8. Download and Publish&#x20;

### Set `test mode = false`&#x20;

To protect the integrity of your account, we have by default set `test mode = true`.

When you are ready activate your ads when you publish, you'll simply need to set `test mode = false`.

<figure><img src=".gitbook/assets/Screenshot 2023-02-16 at 4.54.46 PM.png" alt=""><figcaption></figcaption></figure>

Downloading your app with `test mode = false` to generate more impressions/clicks for your ads is considered [invalid traffic](https://support.google.com/admob/answer/3342054?hl=en\&ref\_topic=9756841) and may lead to your AdMob account being suspended or disabled.

### **Build Your App!**

Once approved, apps can be downloaded and published without further review.

* [Publish to App Store (iOS)](https://docs.thunkable.com/publish-to-app-store-ios)
* [Publish to Play Store (Android) with AAB](https://docs.thunkable.com/publish-to-play-store-android)

## 9. iOS and AdMob Permissions

With iOS 14.5 and above, your app users will be asked if they consent to an advertising identifier being used to show them personalized ads. This is what the dialog looks like:

![](<.gitbook/assets/tracking-dialog (1).png>)

\
You can set a personalized Tracking Usage Description in your [Project Settings](settings/project-settings/).‌ All characters in your Tracking Usage Description must be alphanumeric or an underscore \[a-z A-Z 0-9 \_]\
\
If this permission is declined, your app will still show ads. These will be more generic ads and won't be targeted at the user.\
\
﻿If the user has turned off the `Allow Apps to Request to Track` property in their device settings, this permission will be declined by default and they will not see this dialog.

{% hint style="info" %}
## **Troubleshooting**

If you are not seeing ads appear in your app, it may be due to the following reasons:

* Your AdMob account has been disabled due to a policy violation. Please sign in to [your AdMob account](https://admob.google.com/home/)
* Your AdMob component property `test mode = true`. To activate, you'll need to flip the switch to `test mode = false`
* Your `Ad Unit ID` has not yet been activated. This may take up to a few hours
* You have entered the App ID or the Publisher ID instead of the Ad Unit ID which begins with `ca-app-pub-xxx`
* Please check the mobile device internet connectivity or disable ad blockers on the mobile device
* Check your app's [Readiness Status](https://support.google.com/admob/answer/10564477?hl=en). Only apps with a _Ready_ status will be served ads.
* Your setup is correct. The issue is that AdMob does not always have an ad to return for every request. This may happen particularly if you have just registered your AdMob publisher ID, as it takes some time and multiple requests before the new ID starts returning ads
* [Check the community forum for other potential errors](https://community.thunkable.com/)

Adding error handling to your AdMob blocks can better help troubleshoot issues

![](<.gitbook/assets/Screenshot 2023-02-16 at 3.36.44 PM.png>)
{% endhint %}

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
