# Ads by AdMob

![](.gitbook/assets/webp.net-resizeimage.png)

AdMob is the most popular ad network for monetizing mobile apps today. Apps with large audiences can use AdMob to not only generate revenue for the creator but in some cases \(like with AdMob Rewarded Video\), create better user experiences than the alternative \(e.g. in-app purchases to play a new game level\). 

We highly recommend that you only add ads to your app after you have a large audience of users \(otherwise, you won't generate much revenue anyway\).

* [Review guidelines](admob.md#review-guidelines)
* [Sample apps](admob.md#sample-apps)
* [Ad formats](admob.md#ad-formats)
* [Banner ad](admob.md#banner-ad)
* [Interstitial ad](admob.md#interstitial-ad)
* [Rewarded video ad](admob.md#rewarded-video-ad)
* [Live test](admob.md#live-test) \(Android only\)
* [Download and publish](admob.md#download-and-publish) ![](.gitbook/assets/pro.png) ****
  * [Submit for review](admob.md#submit-for-review)
  * [Create `Ad Unit ID`](admob.md#create-an-ad-unit-id)\`\`
  * [Link `Ad Unit ID`](admob.md#link-ad-unit-id)\`\`
  * [Set `test mode = false`](admob.md#set-test-mode-false)\`\`
* [Troubleshooting](admob.md#troubleshooting)

{% hint style="info" %}
**AdMob is our first**  ![](.gitbook/assets/pro.png) **component.** While all Thunkers can add AdMob to their app projects and live test the ads in their apps, only PRO Thunkers can download and publish apps with AdMob.

All apps must be approved by Thunkable subject to our [review guidelines](admob.md#review-guidelines). If you are a PRO Thunker, you can [**submit your app for review here**](https://airtable.com/shr3qok3ARKXY7cBt). Once approved, apps can be downloaded and published without further review.

Thunkable reserves the right to change an app's approval status subject to any violation of our guidelines.

Thunkable also reserves the right to charge up to a 10% maintenance fee for revenue earned via AdMob in the future. \(During the initial period, Thunkable will not charge a maintenance fee\)
{% endhint %}

## Review guidelines

Thunkable has partnered with AdMob to ensure that apps created on our cross-platform use ads to monetize apps in a way that both provides high quality traffic to advertisers and a high quality user experience for end users of apps.

All apps with AdMob must be first approved by Thunkable before they can be downloaded or published. AdMob has its [own policies](https://support.google.com/admob/answer/7313578) that an app must comply with including but not limited to: 

* Inappropriate content that advertisers do not want to be associated with e.g. copyrighted, adult
* Invalid activity that lowers the quality of traffic to advertisers e.g. ad placements that encourage clicks

Thunkable will review apps for compliance with AdMob policies but will specifically **reject apps** that are:

* Earning apps - apps that encourage users to clicks ads in exchange for some form of payment
* Auto-impression apps  - apps that repeatedly load banner ads in the background of apps

Once approved, apps can be downloaded and published without further review.

**Thunkable reserves the right to change an app's approval status subject to any violation of our guidelines.**

## **Sample apps** <a id="sample-apps"></a>

| **Sample App** | Description |
| :--- | :--- |
| [Dad with Ad](https://x.thunkable.com/projects/5c85f9c0bd31e8c4e90f3539/Welcome/designer) | Dad app with AdMob Banner ad on home screen and AdMob Rewarded Video ad that appears after a user has receive an answer from my dad |

## Ad formats

|  | Banner ad | Interstitial ad | Rewarded video ad |
| :--- | :--- | :--- | :--- |
| Description | Banner ads are rectangular image or text ads that occupy a spot within an app's layout. They stay on screen while users are interacting with the app, and can refresh automatically after a certain period of time. If you're new to mobile advertising, they're a great place to start. | Interstitial ads are full-screen ads that cover the interface of their host app. They're typically displayed at natural transition points in the flow of an app, such as between activities or during the pause between levels in a game. When an app shows an interstitial ad, the user has the choice to either tap on the ad and continue to its destination or close it and return to the app. | Full-screen video ads that users have the option of watching in full [in exchange for in-app rewards](https://support.google.com/admob/answer/7313578).  |
| Recommended for | Single-screen apps | Multi-screen apps | Multi-level games |
| Limit | 1 per screen | 1 per app | 1 per app |

## Banner ad

AdMob banner ads are the simplest ad format to implement and are recommended for beginners.

![Drag and drop the component onto any screen. You may need to re-position banner ad to the bottom or top of the screen using the Vertical Alignment property of the Screen.](.gitbook/assets/thunkable-docs-exhibits-10.png)

That's it.  There's no blocks needed. 

The first banner ad will load when ready and will reload a new ad every minute.

## Interstitial ad

Interstitial ads are recommended after a user has completed a task in your app. We don't recommend showing an interstitial ad right after the app opens and the user has not spent any time in your app.

To show an interstitial app, you need to first add the component and then add the `Show Ad` block after the appropriate event in your app

![](.gitbook/assets/screen-shot-2019-03-08-at-8.54.29-am.png)



## R**ewarded video** ad

Rewarded video ads are recommended after a user has completed a heavy task in your app and would be willing to watch a long video to continue. 

To show a rewarded video app, you need to first add the component and then add the `Show Ad` block after the appropriate event in your app. You'll then want to add a `Reward User` event to continue the app. 

![](.gitbook/assets/screen-shot-2019-03-08-at-8.55.38-am.png)

## Live test \(Android only\) <a id="live-test"></a>

At the moment, it is only possible to live test apps on Android devices. \(To view an ad on an iOS device today, you'll need a PRO account, your app to be approved and to download your app to your iOS device\). We hope to lift this restriction soon.

For your convenience, we have provided a test  `Ad Unit ID` for you to see how a particular ad format may appear in your app. 

During live test, all AdMob ads will be set to `test mode = true`, which means clicks and impressions will not be counted. This is true even if you add your own `Ad Unit ID` and set `test mode = false`.

![](.gitbook/assets/admob-on-design-doc-mar-2019.png)

## Download and publish ![](.gitbook/assets/pro.png) 

{% hint style="info" %}
Only ![](.gitbook/assets/pro.png) ****members can download and publish apps with AdMob
{% endhint %}

### **Submit for review**

All apps with AdMob must be approved by the team at Thunkable \([**submit your app here**](https://airtable.com/shr3qok3ARKXY7cBt)\).  
  
Once approved, apps can be downloaded and published without further review.

Thunkable reserves the right to change an app's approval status subject to any violation of our guidelines.

### **Create an `Ad Unit ID`**

To set your ads live, you'll need to first[ create an AdMob account](https://admob.google.com/home/). Once you have created your account, you'll need to set up an app and create an `Ad Unit ID`.  \(It may take up to an hour for `Ad Unit ID` to be activated and start showing ads\)

Below is a visual walkthrough of the steps after you have created your AdMob account:

![](.gitbook/assets/thunkable-docs-exhibits-8.png)

![](.gitbook/assets/thunkable-docs-exhibits-3.png)

![](.gitbook/assets/thunkable-docs-exhibits-4.png)

![](.gitbook/assets/thunkable-docs-exhibits-5.png)

![](.gitbook/assets/thunkable-docs-exhibits-6.png)

![](.gitbook/assets/thunkable-docs-exhibits-7.png)

### Link `Ad Unit ID` 

{% hint style="info" %}
The Ad Unit ID should begin with `ca-app-pub-xxx`
{% endhint %}

![Enter your Ad Unit ID into the properties panel of your AdMob component. Make sure you enter the right Ad Unit ID for the appropriate ad format](.gitbook/assets/thunkable-docs-exhibits-13.png)

### Set `test mode = false` 

To protect the integrity of your account, we have by default set `test mode = true`.

When you are ready activate your ads when you download or publish, you'll simply need to set `test mode = false`.

![](.gitbook/assets/thunkable-docs-exhibits-14.png)

## **Troubleshooting**

If you are not seeing ads appear in your app, it may be due to the following reasons:

* Your AdMob account has been disabled due to a policy violation. Please sign in to your AdMob account
* Your AdMob component property `test mode = true`. To activate, you'll need to flip the switch to `test mode = false`
* Your  `Ad Unit ID` has not yet been activated. This may take up to a few hours
* You have entered the App ID or the Publisher ID instead of the Ad Unit ID which begins with `ca-app-pub-xxx`
* Please check the mobile device internet connectivity or disable ad blockers on the mobile device
* Your setup is correct. The issue is that AdMob does not always have an ad to return for every request. This may happen particularly if you have just registered your AdMob publisher ID, as it takes some time and multiple requests before the new ID starts returning ads
* [Check the community forum for other potential errors](https://community.thunkable.com/)

\*\*\*\*

\*\*\*\*

