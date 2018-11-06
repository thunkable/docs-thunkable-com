# Publish to Play Store \(Android\)

Publishing your app to the Play Store is a relatively straightforward process and will help your app reach 2 billion active Android devices.

{% hint style="info" %}
Success on Google Play starts with quality. The best apps and games have higher ratings, more installs, and more engagement. We recommend visiting the [Play Store Developer Policy Center](https://play.google.com/about/developer-content-policy/#!?modal_active=none) before you submit your app to the Play Store
{% endhint %}

* [Minimum requirements](publish-to-play-store-android.md#minimum-requirements)
* [App info](publish-to-play-store-android.md#app-info)
* [Download your Android app](publish-to-play-store-android.md#download-your-android-app)
* [Submit your app for review](publish-to-play-store-android.md#submit-your-app-for-review)
* [Troubleshooting](publish-to-play-store-android.md#troubleshooting)

## Minimum requirements

* Google Play Developer Account \($25 one-time fee\). Don't have an account? [**Sign up here**](https://play.google.com/apps/publish/signup/)\*\*\*\*

There are a few additional requirements for the Play Store submission that do take time to create:

* Design assets
  * Icon \(512 x 512 px\)
  * App screenshots
  * Feature graphic \(1024 x 500 px\)
* Privacy policy \(for certain apps that require sensitive information e.g. access to phone camera\)



## App info

To publish your app on Android, you'll need to add an `app icon`, a `name`, a `package name` and an app `version`. To find the App settings, click on the App Icon on the top left.

![](../../.gitbook/assets/ezgif.com-video-to-gif-31%20%281%29.gif)

For recommendations on your `app icon` and `name`, [please see this guide](../create/app-icon-+-name.md).

Each Android app that is published to the Play Store has a unique `package name`. Currently, you can enter this in the App \(Bundle\) ID field. 

{% hint style="info" %}
If you are only publishing to the Play Store, you do not need to enter a Team ID to publish to the Play Store \(this is for iOS only\)
{% endhint %}

Before you download your app, make sure you set the appropriate Build and Version Number. Google Play requires each new version of your app to have a unique and sequentially higher Build and Version Number. You can also let Thunkable auto-increment \(or automatically increase\) the build and version numbers for you.

![](../../.gitbook/assets/thunkable-documentation-exhibits-94.png)

## Download your Android app

![Select Download or Publish Android App and an .apk file will be generated on your desktop](../../.gitbook/assets/thunkable-documentation-exhibits-95.png)

## Submit your app for review

### Create a new app on the Google Play Developer Console

![](../../.gitbook/assets/thunkable-documentation-exhibits-98.png)

![](../../.gitbook/assets/thunkable-documentation-exhibits-99.png)

Next, create a new release. This is where you'll upload the latest version of your app \(.apk\)

![](../../.gitbook/assets/thunkable-documentation-exhibits-96%20%281%29.png)

![](../../.gitbook/assets/thunkable-documentation-exhibits-97.png)

{% hint style="info" %}
Enable Google Play App signing. This is an optional program but we recommend it for most use cases.
{% endhint %}

![Drag and drop your app \(.apk\) to the console](../../.gitbook/assets/thunkable-documentation-exhibits-100%20%281%29.png)

### Update your Play store listing

To complete your Play Store listing, you will have to fill out a content rating questionnaire and set pricing and availability. In addition you will need to add a minimum of 4 design assets - two screenshots, a higher resolution icon \(512 x 512 px\) and a feature graphic \(1024 x 500 px\) that shows up on the Play Store app.

![](blob:https://docs.thunkable.com/fb130b9d-e9ee-4ef9-86d8-e265361e07b2)

![](../../.gitbook/assets/thunkable-documentation-exhibits-94%20%281%29.png)

![](../../.gitbook/assets/thunkable-background-image-1080-x-1920-px-11.png)

![App screenshots](../../.gitbook/assets/thunkable-background-image-1080-x-1920-px-12%20%281%29.png)

![High resolution app icon \(512 x 512 px\)](../../.gitbook/assets/d-icon-dark.png)

![Feature Graphic \(1024 x 500 px\)](../../.gitbook/assets/webp.net-resizeimage-11.png)

### Add a privacy policy

{% hint style="info" %}
Apps that request access to sensitive permissions or data \(as defined in the [user data policies](https://play.google.com/about/privacy-security-deception/user-data/)\) are required by the Google Play Store to include a privacy policy. Currently all apps made on Thunkable request access to sensitive permissions or data, which means you will need to provide a privacy policy
{% endhint %}

**Congrats! You are now ready to submit to the Play Store.**

## Troubleshooting

**You cannot update an existing app on the Google Play Store**

{% hint style="warning" %}
Apps originally built on the [Thunkable Classic platform](../../thunkable-classic-android/) cannot be updated since it is not yet possible to import the keystore
{% endhint %}

* If you updating an existing app on the Google Play Store, your app will need to have the i\) same package name, ii\) a higher or incremented version number, and the iii\) same keystore. The first two are easily editable in the App Settings page but the keystore is not yet able to be imported / exported. 
* Copied apps within an account \(using the [Make Copy](../make-copy.md)\) will keep the same keystore as the original app. Apps that are copied from a [Share copy](../share.md#share-a-fully-editable-copy-of-your-app-project) link will not have the same keystore. Apps from the [Thunkable Classic platform](../../thunkable-classic-android/) cannot yet be updated since it is not yet possible to import the keystore. 



