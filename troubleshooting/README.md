# 🔎 Troubleshooting

Here are some of the most common issues that our users are running into:

## Live Test

**Issue:** You see a blank / white screen when you live test (even if there are items in your app)

* If you have a Navigator as the first item in your tree, make sure your screen is dropped within it
* Your have unconnected blocks
* You have an event triggered by a Screen.Start which may be causing the screen to crash
* Your app and desktop may not be logged into the same account

**Issue:** Image is not showing up on your phone

* The height or width of the image may be set to 'Fit contents'

## Download Android

**Issue:** Trouble downloading AAB and APK files from Google Chrome

* The Google Chrome browser blocks downloads for your safety. If you open the email with a download link for your APK or AAB file in Google Chrome, you may not be able to download your file. \
  You can try one of these options:
  1. Open the email in another browser, like Firefox or Safari, and download the file.
  2. Change your Google Chrome settings to allow you to download files. \
     [You can find instructions to do this here. ](https://www.businessinsider.com/how-to-stop-chrome-from-blocking-downloads)\
     Please note that changing your browser security settings can make you more vulnerable as you use the web, and Google Chrome does not recommend disabling this setting.

## Publish iOS

**Issue:** You don't see your app uploaded to App Store Connect

* **Icons**. Ensure your icon is 192 x 192 px and has no transparencies.&#x20;
* **Membership**. You require an active [Apple Developer Program Membership](https://developer.apple.com/programs/) to publish to the App Store.&#x20;
* **Certificates**. If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time, and Thunkable creates one when it publishes to your account
* **Provisioning profile**. After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive. To publish successfully, you need to delete any inactive provisioning profiles.
* **Login**. Ensure your Apple ID and password are entered correctly. Thunkable cannot access your credentials, so save them somewhere safe.
* **Apple ID and privacy terms**. You must accept Apple's new Apple ID and privacy terms.

### Android

**Issue:** You cannot update an existing app on the Google Play Store

* If you want to update an existing app on the Google Play Store, your app will need to have:&#x20;
  * the same package name
  * a higher or incremented version number
  * the same keystore
* The first two are easily editable in your App Settings, but the keystore cannot be imported/exported.&#x20;
* Copied apps within an account ([Duplicate Your Project](../make-copy.md)) will keep the same keystore as the original app. Apps copied from a [Share](../share-1.md#share-a-fully-editable-copy-of-your-app-project) link will not have the same Keystore.&#x20;

## Data Sources

### How can I reset my Google Sheets connection in Thunkable?

#### A. Reset from Thunkable

1. Login to your Thunkable account.
2. Click the **My Data Sources** tab on your Projects Page.
3. Click the **trash can icon** to delete the Google Sheets data source.

![](<../.gitbook/assets/image (216) (1).png>)

#### B. Reset from Google

If you are having difficulties connecting to your Google Sheets from Thunkable, you may need to reset your Google Sheets connection.

1. Navigate to [https://myaccount.google.com/security](https://myaccount.google.com/security)
2. Scroll to the **Your connections to third-party apps & services** section.
3. Click the **Thunkable** connection.&#x20;
4.  Click **See details** in the **Thunkable has some access to your Google Account section**.\


    <figure><img src="../.gitbook/assets/Google Sheets connection.png" alt=""><figcaption></figcaption></figure>
5.  Click **Remove Access**.\


    <figure><img src="../.gitbook/assets/Google Sheets - remove access.png" alt=""><figcaption></figcaption></figure>
6. Return to Thunkable and re-connect to your Google Sheets account.
