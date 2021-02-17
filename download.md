# 📥 Download

{% hint style="info" %}
Before you download, we recommend first [adding an App Icon and Name](projects/settings.md) to your app
{% endhint %}

* [Download limits](download.md#download-limits)
* [Download and install Android app](download.md#download-and-install-android-app)
* [Download and install iOS app](download.md#download-and-install-ios-app)

## Download limits

Due to special circumstances from Apple, there is a limit of one downloaded app per phone on iOS. Download wait times will also be a bit longer.

When there is a queue of iOS apps waiting to be built, [PRO](https://thunkable.com/#/pricing) creators will be given priority in the queue.

|  | Android | iOS |
| :--- | :--- | :--- |
| Download app limit | No limit | One app per phone |

### Select Download Android app

To download your Android app, select Download Android App and an .apk file will be generated on your desktop

![](.gitbook/assets/thunkable-documentation-exhibits-95%20%281%29.png)

### Keep your .apk file

If you are using the latest version of Chrome you might see a notification that your app "_is not commonly downloaded and may be dangerous_". While some .apk files can potentially contain malicious software you are downloading an app that you have created yourself so there is no danger here. You can click on the "More Options" menu and choose the "Keep" option as highlighted below to complete your download.

![](.gitbook/assets/screen-shot-2018-06-28-at-19.33.13.png)

### To install, allow apps from Unknown sources

Anyone installing your app directly, instead of from the Play Store, will need to change the setting on their phone to allow installation of apps from Unknown sources

![](.gitbook/assets/download-fig-4.png)

## Download and install iOS app

### Select Download iOS app and enter your email address

You will receive an email when your app is ready to download. This usually takes 15-20 minutes but can take up to an hour

![](.gitbook/assets/downloadandroid.png)

### Click on the download link in your email

{% hint style="info" %}
The link to download the app is only intended for your own use and will expire after 24 hours
{% endhint %}

![](.gitbook/assets/thunkable-documentation-exhibits-86.png)

### To install, trust Thunkable on your device

On your first time downloading apps for iOS, you will need to open your `Settings` app, navigate to `General` and `Device Management` and then `Trust "Thunkable, Inc."` \(the business name of Thunkable\)

![](.gitbook/assets/assets_-lan5scxl2uqujuoqkjo_-lan5weceranwag7ig2g_-lan671msr8pjsfhbvj7_download-fig-3.png)

### Troubleshooting

Common issues

**You receive an email from the hard-working beaver saying that this app will not build**

* You uploaded an icon that has the same name as an existing asset that you have uploaded
* Your app icon is not an image file
* Your app icon contains transparent pixels. Apple does not allow you to have any icons with any transparent colors
* We are having trouble with our build servers. Please try again in 30 minutes or chat with us if you are still having problems
* App \(Bundle\) ID. Your App \(Bundle\) ID is a series of short strings of text that are separated by periods, such as **com.thunkable.creator.app**. These string of text must i\) be lowercase, ii\) begin with a letter.
  * Examples of App \(Bundle\) IDs that can cause errors: com.thunkable.creator.1app, Com.Thunkable.Creator.APP
* Asset names. We recommend that asset names **only** contain Roman alphabet characters with no accents, and numbers.
  * Examples of asset names that could cause errors: image\(1\).jpg, imãge.jpg
  * Examples of asset names that won't cause errors: image1.jpg, image.jpg

**You cannot install your app and get the message "Cannot connect to storage.googleapis.com"**

* You have a special character like "&" in your [App Name](projects/settings.md#app-name)

**When you install your app on Android, you see the message "There was a problem parsing the Package"**

* This is caused by your package name, also known in your project as your App \(Bundle\) ID. Your App \(Bundle\) ID is a series of short strings of text that are separated by periods, such as **com.thunkable.creator.app**. These string of text must i\) be lowercase, ii\) begin with a letter.
  * Examples of App \(Bundle\) IDs that can cause errors: com.thunkable.creator.1app, Com.Thunkable.Creator.APP

