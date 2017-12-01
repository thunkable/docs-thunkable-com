#### **Thunkable for iOS **

# Step 5 `Publish`

---

For app developers looking to distribute their apps widely, publishing your app to the App Store can be a very rewarding process.

Thunkable has eliminated a few steps from the normal iOS submission process to make it easier for our developers including sending new builds directly to iTunes Connect, Apple's portal for managing App Store submissions, auto-incrementing each new build and enabling building apps from non-Mac computers \(usually a Mac is required\).

Do note that Apple holds a high standard for apps that are approved for distribution in the App Store so please [review Apple's policies and guidelines](https://developer.apple.com/app-store/review/guidelines/) to make sure your app is in compliance before you sign up for the Apple Developer Program.

To publish your app to the App Store:

* On Apple
  * [Enroll in the Apple Developer Program](#1--enroll-in-the-apple-developer-program-currently-99year) \(currently $99 / year\)
  * [Register an App ID in your Apple Developer account ](#2--register-an-app-id-in-your-apple-developer-account-apple-will-automatically-generate-a-team-id----)
  * [Create a new app in iTunes Connect](#3--create-a-new-app-in-itunes-connect-itunes-connect-is-your-portal-for-managing-your-submission-to-the-app-store)
* On Thunkable
  * [Update your App Publish settings](#4--on-thunkable-update-your-app-publish-settings-to-find-it-click-on-the-app-icon-on-the-top-left-and-then-the-properties-tab)
  * [When you are ready, select Publish to submit your latest app to iTunes Connect](#5--when-you-are-ready-to-publish-select----to-submit-your-latest-app-to-itunes-connect-this-does-not-yet-publish-your-app-to-the-app-store). This does _not_ yet publish your app to the App Store
* Back on Apple
  * [Follow the instructions on iTunes Connect to submit your app for review](#6--follow-the-instructions-on-itunesconnect-to-submit-your-app-for-review-there-are-3-main-sections-to-fill-out)

If you are not seeing your app build in iTunes Connect, below are a number of common errors \(currently, our error messaging is still in beta!\)

* Troubleshooting

---

### 1 / Enroll in the [Apple Developer Program](https://developer.apple.com/programs/) \(currently $99/year\)

![](/assets/publish-ios-fig-1.png)

---

### 2 / [Register an App ID](https://developer.apple.com/account/ios/identifier/bundle/create) in your Apple Developer account. Apple will automatically generate a `Team ID` . . .

![](/assets/publish-ios-fig-4.png)

### and you will create a `Bundle ID` \(similar to a package name in Android\)

![](/assets/publish-ios-fig-5.png)

---

### 3 / [Create a new app](https://itunesconnect.apple.com/) in iTunes Connect. iTunes Connect is your portal for managing your submission to the App Store.

### ![](/assets/publish-ios-fig-6.png)

### You will need to link the `Bundle ID` you created earlier

![](/assets/publish-ios-fig-7.png)

---

### 4 / On Thunkable, update your App publish settings. To find it, click on the App Icon on the top left and then the Properties tab.

![](/assets/publish-ios-fig-8.png)

---

### 5 / When you are ready to publish, select ![](/assets/publish-ios.png)  to submit your latest app to iTunes Connect. This does _not_ yet publish your app to the App Store.

### ![](/assets/publish-ios-fig-2.png)

### You will also have to enter your Apple developer login credentials![](/assets/publish-ios-fig-3.png)

### When your app has been successfully uploaded, you will receive an email from iTunes Connect. It will also appear under the Testflight tab in your iTunes Connect dashboard. Testflight is a tool from Apple that allows you to test your app before it is submitted for release in the App Store. You can use the tool to share your app with others.

![](/assets/publish-ios-fig-9.png)

### You may need to answer a question about export compliance. You can select 'no' when asked if you app uses encryption since apps made on Thunkable for iOS do not at the moment.

![](/assets/publish-ios-fig-10.png)

### Your app is now ready for internal testing to be downloaded by you and others and ready to submit to the App Store. We recommend you test your app via Testflight before you submit your app for review to the App Store.

![](/assets/publish-ios-fig-11.png)

---

### 6 / Follow the instructions on iTunesConnect to submit your app for review. There are 3 main sections to fill out.

### First is App Information which is pretty straightforward.

### ![](/assets/publish-ios-fig-12.png)The second section is Pricing and Availability. Also, very straightforward although there may be some strategy involved if you want to slowly release your app to different app stores.

![](/assets/publish-ios-fig-13.png)

### The final section contains the design assets \(Screenshots, App Icon\) which you will need to have ready.

![](/assets/publish-ios-fig-14.png)

### You'll also need to select the build version that you want to submit.

![](/assets/publish-ios-fig-15.png)![](/assets/publish-ios-fig-16.png)

### Congrats! You are not ready to submit to the App Store.

---

### Troubleshooting {#publish-troubleshooting}

Common issues

* _Login_. Apple ID or password were entered incorrectly.  Since we don't store either one, there's no easy way for us to check so enter it slowly
* _Build._ Your app may not be able to build/compile for a variety of reasons.  One good check is to download your app to your phone first to see if there are any errors compiling the app.
* _Two-factor authentication_. You must turn off 2 factor authentication for your Apple Developer ID to publish with Thunkable

* _Certificates_. If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time and Thunkable creates one when it publishes to your account.

* _Provisioning profile_. After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive.  To publish successfully, you'll also need to delete any inactive provisioning profiles.



