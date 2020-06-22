---
description: How to publish your Thunkable Project to the Apple App Store
---

# Publish to App Store \(iOS\)

Publishing your app to the App Store can be a rewarding process.

Apple requires a lot information for apps that are available in their App Store. As a result, the publishing process can feel long and will require at least 20 minutes to complete the necessary steps, which currently requires information from 4 different Apple websites.

Thunkable is continually looking for ways to streamline the publishing process and has made it possible for creators to publish from a non-Mac computer, which is normally required from the standard publishing process.

### Table of Contents

* [Minimum requirements](publish-to-app-store-ios.md#minimum-requirements)
* [Register your app](publish-to-app-store-ios.md#register-your-app)
* [Two-factor authentication](publish-to-app-store-ios.md#two-factor-authentication)
* [App Store Connect](publish-to-app-store-ios.md#app-store-connect)
* [App info](publish-to-app-store-ios.md#app-info)
* [Troubleshooting](publish-to-app-store-ios.md#troubleshooting)
* [Submit your app for review](publish-to-app-store-ios.md#submit-your-app-for-review)
* [Adding Push Notifications](publish-to-app-store-ios.md#adding-push-notifications)

## Minimum requirements

{% hint style="info" %}
Apple holds a high standard for apps that are approved for distribution in the App Store so please [review Apple's policies and guidelines](https://developer.apple.com/app-store/review/guidelines/) to make sure your app is in compliance before you sign up for the Apple Developer Program
{% endhint %}

* Apple Developer Program membership \($100/year\). Don't have one? [**Sign up here**](https://developer.apple.com/programs/).

## Overview

![](.gitbook/assets/pubish_step_by_step.gif)

1. [ ] [Sign into you Apple Developer Account](publish-to-app-store-ios.md#sign-into-your-apple-developer-account)
2. [ ] [Register your App ID](publish-to-app-store-ios.md#register-your-app-id)
3. [ ] [Create a Distribution Certificate](publish-to-app-store-ios.md#create-a-distribution-certificate)
4. [ ] [Generate a Mobile Provisioning Profile](publish-to-app-store-ios.md#provision-your-app)
5. [ ] [Set an app-specific password](publish-to-app-store-ios.md#generate-an-app-specific-password)
6. [ ] [Create an app on App Store Connect](publish-to-app-store-ios.md#appstore-connect)
7. [ ] [Send to App Store Connect](publish-to-app-store-ios.md#send-to-app-store-connect)

## Sign into your Apple Developer Account

The first, and probably most important, piece of information you will need is an Apple Developer Account. To obtain a developer account you must enrol in the [Apple Developer Program](https://developer.apple.com/programs/).

### Developer Accounts for Schools

Certain educational institutions qualify for free Apple developer accounts. To check if your school or university if eligible, please visit this Apple site.

### Apple

### Thunkable

Thunkable enables you to send your project directly to the App Store without the need for any specialized software or hardware. To begin the process, click on the **Publish** icon and choose the **Publish to App Store \(iOS\)** option from the drop-down menu.

![](.gitbook/assets/screenshot-2019-10-07-at-15.54.16.png)

A publishing dialog will pop-up on screen to guide you through the publication process. Please take a moment to read all the instructions on screen the click the **Get Started** button to proceed. 

![](.gitbook/assets/01_get_started.png)

Enter the Apple ID and password that are associated with your Apple Developer account. Since Two Factor Authentication \(2FA\) is now the default for Apple accounts, it is assumed that you have this enabled, and the rest of this guide shows the steps for publishing with 2FA enabled. Click the **Next** button to log in and continue to the next step.

![](.gitbook/assets/02_sign_in.png)

## Register your App ID

Every app published on the App Store must have a unique name. For example, there can only ever be one app called `Thunkable Sample App`. 

### Apple

Go to the [**Apple Developer website**](https://developer.apple.com/account) ****to ****register a new App ID. Click through the tabs below to see each screen in the ID creation process.

Step 6 in the tabs below shows you where to find your App Name, Team ID, and Bundle ID.

{% tabs %}
{% tab title="Step 1" %}
![](.gitbook/assets/dev_01.png)

Open your Apple Developer account page and choose the **Certificates, IDs & Profiles** option from the menu on the left hand side of the screen.
{% endtab %}

{% tab title="Step 2" %}
![](.gitbook/assets/dev_02.png)

From the menu on the left, click on the **Identifiers** menu item
{% endtab %}

{% tab title="Step 3" %}
![](.gitbook/assets/dev_03.png)

Click on the blue **+** icon to add a new ID to your account.
{% endtab %}

{% tab title="Step 4" %}
![](.gitbook/assets/dev_04.png)

Choose **App IDs** from the list of options and then click on the blue **Continue** button to go to the next screen.
{% endtab %}

{% tab title="Step 5" %}
![](.gitbook/assets/dev_05.png)

For the app **Description** enter the name you want to give your app and for the **Bundle ID** enter the bundle ID from your Thunkable project settings. Click **Continue** to review these details.
{% endtab %}

{% tab title="Step 6" %}
![](.gitbook/assets/dev_06a.png)

Once you are happy with these detail, click **Register** to confirm your app ID.
{% endtab %}

{% tab title="Step 7" %}
![](.gitbook/assets/dev_07.png)

This new app ID is added to your list of app IDs. 
{% endtab %}
{% endtabs %}

### Thunkable

Back in Thunkable, you will be prompted for your App Name, Team ID and Bundle ID. If you are unsure of what these are, please refer to Step 6, above. 

* **App Name:** The app Name must be unique to the App Store and is what appears next to the app icon when it is downloaded on a user's phone.
* **Team ID:**  A unique account identifier that is linked to your Apple Developer Program membership. Apple will automatically create this for you, and it can be used for every app you publish.
* **Bundle ID:** Also unique to your app, but not visible to your app users. Otherwise, a single Explicit App ID should work. Apple recommends reversing your domain name to create your bundle ID i.e. _com.yourDomainName.yourAppName_ to avoid conflicts with other apps.
  * _Note: Starting June 16, 2020, uploading apps to the App Store requires an explicit bundle ID. Wildcard bundle IDs are no longer available when creating app records._

![](.gitbook/assets/03_registerapp-1.png)

## Create a Distribution Certificate

Two-factor authentication helps to keep your account secure and Apple has made it mandatory for new developers to turn two-factor authentication on. If you do have 2FA turned on, you'll need to complete the following steps to confirm your identity with Apple.

### Thunkable

In the publishing dialog, click the link that says **Click to Download CSR.** This is your Certificate Signing Request file and you will need it to generate an iOS Distribution Certificate. 



![](.gitbook/assets/download_csr.png)

### Apple 

Go to the [Certificates page](https://developer.apple.com/account/resources/certificates/list) in your Apple Developer account to generate an iOS Distribution Certificate. Two-factor authentication helps to keep your account secure and Apple is making it mandatory for new developers to turn two-factor authentication on.

{% hint style="warning" %}
You may already have an account certificate in your account. You can only have two certificates per account so you may need to revoke a certificate before you can create a new one.
{% endhint %}

{% tabs %}
{% tab title="Step 1" %}
![](.gitbook/assets/cert_01.png)

Click on the blue **+** icon to create a new iOS distribution certificate.
{% endtab %}

{% tab title="Step 2" %}
![](.gitbook/assets/cert_02.png)

Choose **iOS Distribution \(App Store and Ad Hoc\)** from the next list and click **Continue.**
{% endtab %}

{% tab title="Step 3" %}
![](.gitbook/assets/cert_03.png)

Upload the [Certificate Signing Request](publish-to-app-store-ios.md#thunkable-2) you download from Thunkable and click **Continue** to get your certificate.
{% endtab %}

{% tab title="Step 4" %}
![](.gitbook/assets/cert_04.png)

Click the blue **Download** button to save a copy of this certificate to your computer.
{% endtab %}

{% tab title="Step 5" %}
![](.gitbook/assets/04_csr_cer.png)

Back in Thunkable, click the **Upload Certificate** button and choose the `.cer` file that you have just created. 
{% endtab %}
{% endtabs %}

## Provision your App

Provisioning profiles are required by Apple to install an app on a device. You need to create a `.mobileprovision` file in your Apple account and then return to Thunkable to upload this file.

### Apple

{% tabs %}
{% tab title="Step 1" %}
![](.gitbook/assets/prof_01.png)

Open up the [Profiles list](https://developer.apple.com/account/resources/profiles/list) in your Apple Developer account and click the blue **+** button to get started. 
{% endtab %}

{% tab title="Step 2" %}
![](.gitbook/assets/prof_02.png)

Make sure you are creating a **Distribution** profile and that the **App Store** option \(highlighted above\) is selected. Click **Continue** to choose an App ID.
{% endtab %}

{% tab title="Step 3" %}
![](.gitbook/assets/prof_03.png)

From the drop down menu, choose the ID for the app that you are trying to publish. Click **Continue** to go to the next page.
{% endtab %}

{% tab title="Step 4" %}
![](.gitbook/assets/prof_04.png)

Choose a certificate and click **Continue.**
{% endtab %}

{% tab title="Step 5" %}
![](.gitbook/assets/prof_05.png)

Finally, give your provisioning profile a meaningful name and hit the **Generate** button.
{% endtab %}

{% tab title="Step 6" %}
![](.gitbook/assets/prof_06.png)

Once the provisioning profile has been generated you can then **Download** it to your computer. 
{% endtab %}

{% tab title="Step 7" %}
![](.gitbook/assets/prof_07.png)

The profile has a `.mobileprovision`file type. You now need to go back to Thunkable and upload this file. 
{% endtab %}
{% endtabs %}

### Thunkable

Back in Thunkable, upload your `.mobileprovision` file and click the **Next** button to go to the next step; [Generating an app-specific password.](publish-to-app-store-ios.md#generate-an-app-specific-password)

![](.gitbook/assets/05_provisioning.png)

## App-specific passwords

Apple requires app-specific passwords to sign-in securely from Thunkable. 

{% hint style="info" %}
You only need **one** app-specific password for your Thunkable account.   
You do **not** need a separate app-specific password for separate apps.
{% endhint %}

You will need this password to update your app in the future, so make sure to record it securely.

### Generate an app-specific password

Go to the [Apple ID account website](https://appleid.apple.com/#!&page=signin) and create an app-specific password.

{% tabs %}
{% tab title="Step 1" %}
![](.gitbook/assets/appid_01.png)

**Step 1:** Enter your Apple ID and Password
{% endtab %}

{% tab title="Step 2" %}
![](.gitbook/assets/appid_02.png)

**Step 2:** If prompted, enter your 6 digit authentication code.
{% endtab %}

{% tab title="Step 3" %}
![](.gitbook/assets/appid_03.png)

**Step 3:** Once signed in, click on the **Generate password...** link highlighted above.
{% endtab %}

{% tab title="Step 4" %}
![](.gitbook/assets/docspublishasp.png)

**Step 4:** Give your password a meaningful name so you will be able to recognise it later.
{% endtab %}

{% tab title="Step 5" %}
![](.gitbook/assets/appid_05.png)

**Step 5:** You will not be able to retrieve this password once you click **Done** so make sure you save it some place safe.
{% endtab %}
{% endtabs %}

### Changing an App-specific password

To change an app-specific password, you will need to 1\) revoke your old password and 2\) generate a new password using the steps above.   
  
To revoke an app-specific password:

1. Sign into your [Apple ID account page](https://appleid.apple.com/#!&page=signin)
2. In the **Security** section, click **Edit**
3. Go to the **App-Specific Passwords** section and click **View History**
4. Click the ⓧ next to an individual password to revoke it, or click 'Revoke All' to revoke all of your app-specific passwords

### Thunkable 

Paste your app-specific password into the empty text box and click the **Next** button to send your project to [App Store Connect](publish-to-app-store-ios.md#appstore-connect). 

![](.gitbook/assets/06_app_specific_password.png)

## App Store Connect  <a id="appstore-connect"></a>

App Store Connect is where you'll prepare your app store listing

### Thunkable

At this point in the process the publishing dialog will prompt your to crate a new app on App Store Connect. Simply click the link to open this site in a new tab.

![](.gitbook/assets/07_appstore_connect.png)

### Apple

#### Go to the [App Store Connect website](https://appstoreconnect.apple.com/login)

App Store Connect is your portal for managing your submission to the App Store.

{% tabs %}
{% tab title="Step 1" %}
![](.gitbook/assets/store_01.png)
{% endtab %}

{% tab title="Step 2" %}
![](.gitbook/assets/store_02.png)
{% endtab %}

{% tab title="Step 3" %}
![](.gitbook/assets/store_03.png)
{% endtab %}

{% tab title="Step 4" %}
![](.gitbook/assets/store_04.png)

You will need to use the same **App Name** and **Bundle ID** you registered earlier. If you registered an 'Explicit App ID', you will enter it into the Bundle ID field above.
{% endtab %}

{% tab title="Step 5" %}
![](.gitbook/assets/store_05.png)
{% endtab %}
{% endtabs %}

## App info

You're almost there.

![](.gitbook/assets/08_app_info-1.png)

### Upload an app icon

This app icon appears when a user downloads your app from the App Store. Our recommended size is 192 x 192 px. This icon must not have any transparent pixels.

### Set a build and version number

The version number is visible to your users when they download a new version of your app. The build number needs to increase with each version and is only visible to you. You can opt to let Thunkable automatically increment your build and version numbers.

### Permissions

Apple requires that you explain to users why you may need access to a sensitive services like a camera, photo library and microphone. You can add these explanations in the App Settings panel.

![](.gitbook/assets/app_settings.png)

### Congratulations

You should shortly receive an email from Thunkable to let you know that your app is being sent to the App Store. There are still a number of steps that Apple need to take before your app can be downloaded, but that's everything completed from the Thunkable side of things - congrats!

![](.gitbook/assets/app_sent.png)

## **Send to App Store Connect**

You should receive an email from Apple that says your app is ready in the App Store Connect website. **This may take up to an hour.**

If your app is submitted successfully, it should appear under the Testflight tab in your App Store Connect dashboard. Testflight is a tool from Apple that allows you to test your app before it is submitted for release in the App Store.

\(If there are any issues, you’ll get an email from us telling you what you’ll need to fix.\)

![If your app is sent successfully, you&apos;ll see a new build under the TestFlight tab in your App Store Connect dashboard. Testflight allows you to invite beta testers to your app before you release it in the App Store.](.gitbook/assets/thunkable-docs-exhibits-85.png)

## Troubleshooting

**You do not see your app uploaded to App Store Connect**

* Download. One way to check if your app is build-able is to download it to your phone first. Two common download errors are:
  * You uploaded an icon that has the same name as an existing asset that you have uploaded
  * Your app icon is not an image file
* Icons. Apple additionally does not allow you to have any icons with any transparent colors. We recommend app icons to be 192 x 192 px
* Membership. To publish to the App Store, you'll need to sign up for [Apple Developer Program Membership](https://developer.apple.com/programs/). This currently costs $99 / year.
* App Store Connect. Make sure to [follow this step](publish.md#step-③--create-a-new-app-in-itunes-connect) on creating a new app on iTunes Connect
* Certificates. If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time and Thunkable creates one when it publishes to your account
* Provisioning profile. After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive.  To publish successfully, you'll also need to delete any inactive provisioning profiles
* Two-factor authentication. You must turn off two-factor authentication for your Apple Developer ID to publish with Thunkable. Please [click here](https://community.thunkable.com/t/important-two-factor-authentication-publishing-to-ios-app-store-on-thunkable-cross-platform/42504) to see our recommendations for turning off two-factor authentication 
* Login. Apple ID or password were entered incorrectly.  Since we don't store either one, there's no easy way for us to check so enter it slowly
* Apple ID and privacy terms. You must accept Apple's new Apple ID and privacy terms.
* You see a message saying "ITMS-90809: Deprecated API Usage - Apple will stop accepting submissions of apps that use UIWebView APIs". This is a warning, but you can still publish your app. See the [Web Viewer](https://docs.thunkable.com/web-viewer) documentation for more details.

## Submit your app for review

Congrats. You're so close.

There are three main steps that are required before you can submit your app for review. To complete the steps, you will need:

* Design assets
  * Icon \(1024 x 1024 px\)
  * iPhone and iPad screenshots
* Privacy policy url for all apps

### App information

The App Information section is straightforward but does include a privacy policy url, which is required for all apps

![](.gitbook/assets/thunkable-docs-exhibits-72.png)

### Pricing and availability

![](.gitbook/assets/thunkable-docs-exhibits-73.png)

### Design assets

The final section requires screenshots for both iPhone and iPad and a high resolution icon.

The high resolution icon will be featured in the App Store listing and must be 1024 x 1024 px with no transparency. To generate this icon, we recommend a tool [like this](https://makeappicon.com/).

You can see the screenshots you need in Apple's [screenshot specifications document](https://help.apple.com/app-store-connect/#/devd274dd925).

{% hint style="info" %}
 You can create your own iOS screenshots in your browser. Learn more here: [Generate Screenshots](generate-screenshots.md)
{% endhint %}

![](.gitbook/assets/thunkable-docs-exhibits-74.png)

You'll also need to select the build version that you want to submit.

![](.gitbook/assets/thunkable-documentation-exhibits-73.png)

![](.gitbook/assets/thunkable-documentation-exhibits-74.png)

### Export compliance

{% hint style="info" %}
You may need to answer a question about **export compliance**. You can select 'no' when asked if you app uses encryption since apps made on Thunkable for iOS do not at the moment.
{% endhint %}

![](.gitbook/assets/thunkable-docs-exhibits-86.png)

![](.gitbook/assets/thunkable-docs-exhibits-87.png)

### Advertising identifier

{% hint style="info" %}
After submitting your app for review, you may asked, "Does this app use the Advertising Identifier \(IDFA\)?"

The app will still be able to be published but you will want to **check** **the following three boxes**:

* Attribute this app installation to a previously served advertisement”
* “Attribute an action taken within this app to a previously served advertisement”
* “I, YOUR\_NAME, confirm that this app, and any third party…”

Note, you should _not_ check the box labeled “Serve advertisements within the app”.
{% endhint %}

## Adding Push Notifications

If you are adding Push Notifications to an app that is already published, you will need to create a new **.mobileprovision** file. Here's a quick overview of what that process looks like.

Click on _Provisioning Profiles &gt; All_ to see your current iOS provisioning profiles. Notice that the app you just created is now **invalid** so we need to generate a new one.

![](.gitbook/assets/inactive.png)

Open the inactive profile and click on **Edit** to generate a new one.

![](.gitbook/assets/edit.png)

Scroll to the bottom of the page and click **Generate.**

![](.gitbook/assets/generate.png)

On the next screen, click the **Download** button and the .mobileprovision file will be saved to your downloads folder.

![](.gitbook/assets/download.png)

 



