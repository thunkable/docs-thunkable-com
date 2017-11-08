#### **Thunkable for iOS **

# Step 5 `Publish`

---

Publishing your app to the App Store can be a lengthy and expensive process.  Apple holds a high standard for apps that are approved for distribution in the App Store so please review Apple's policies and guidelines to make sure your app is in compliance before you sign up for the Apple Developer Program.

To get started publishing your app to the App Store:

* [Enroll in the Apple Developer Program](#1--enroll-in-the-apple-developer-program-currently-99year) \(currently $99 / year\)
* [Register an App ID](#2--register-an-app-id-from-apple-similar-to-package-name-in-android-you-should-be-given-a-team-id) from Apple \(similar to package name in Android\)
* [On Thunkable, navigate to the App Settings Page and enter the Team ID, Bundle ID, and App Name and upload and App Icon](#3--on-thunkable-navigate-to-the-app-settings-page-and-enter-the-team-id-bundle-id-and-app-name-and-upload-and-app-icon) 
* [When you are ready, select Publish and enter your Apple credentials](#4--when-you-are-ready-to-publish-select---and-enter-your-apple-credentials-same-as-your-apple-developer-program-membership-id-you-will-get-an-email-from-itunesconnect-when-the-app-has-been-submitted--if-youre-app-has-been-successfully-uploaded-it-should-appear-in-your-itunesconnect-account-like-below).  You will get an email from iTunesConnect when the app has been uploaded.
* [Follow the instructions on iTunesConnect to submit your app for review](#5--follow-the-instructions-on-itunesconnect-to-submit-your-app-for-review)

---

### 1 / Enroll in the [Apple Developer Program](https://developer.apple.com/programs/) \(currently $99/year\)

![](/assets/publish-ios-fig-1.png)

---

### 2 / [Register an App ID](https://developer.apple.com/account/ios/identifier/bundle/create) from Apple \(similar to package name in Android\). You should be given a Team ID.

![](/assets/publish-ios-fig-4.png)

### After following the steps, you should also get a Bundle ID page like the one below.![](/assets/publish-ios-fig-5.png)

---

### 3 / On Thunkable, navigate to the App Settings Page and enter the Team ID, Bundle ID, and App Name and upload an App Icon

![](/assets/publish-ios-fig-6.png)![](/assets/publish-ios-fig-5.png)

---

### 4 / When you are ready to publish, select ![](/assets/publish-ios.png) and enter your Apple credentials \(same as your Apple Developer Program membership ID\). You will get an email from iTunesConnect when the app has been submitted![](/assets/publish-ios-fig-2.png)![](/assets/publish-ios-fig-3.png)If you're app has been successfully uploaded, it should appear in your iTunesConnect account like below:

---

### 5 / Follow the instructions on iTunesConnect to submit your app for review

---

### Troubleshooting

**Certificates**

If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time and Thunkable creates one when it publishes to your account.

**Provisioning Profile**

After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive.  To publish successfully, you'll also need to delete any inactive provisioning profiles. 

**Two-factor authentication**

You must turn off 2 factor authentication for your Apple Developer ID to publish with Thunkable

