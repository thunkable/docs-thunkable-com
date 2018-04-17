#### **Thunkable Cross-Platform **✕

# Publish ![](/assets/iOSviewIconPublish_TR.png)

---

If you want your app to reach a large audience, we recommend publishing it to the Google Play or App Store. To do so, you will need to enroll in their developer programs and submit your app for approval.

* [Publish to the App Store \(iOS\)](#publish-to-the-app-store-ios)
* Publish to Play Store \(Android\) - not yet available

---

### Publish to the App Store \(iOS\)

For app developers looking to distribute their apps widely, publishing your app to the App Store can be a very rewarding process.

Thunkable has eliminated a few steps from the normal iOS submission process to make it easier for our developers. We send new versions of your app directly to iTunes Connect, Apple's portal for managing App Store submissions, auto-increment each new version and enabling building apps from non-Mac computers \(usually a Mac is required\).

Do note that Apple holds a high standard for apps that are approved for distribution in the App Store so please [review Apple's policies and guidelines](https://developer.apple.com/app-store/review/guidelines/) to make sure your app is in compliance before you sign up for the Apple Developer Program.

To publish your app to the App Store:

* [① / Enroll in the Apple Developer Program](#step-①---enroll-in-the-apple-developer-program-currently-99year) \(currently $99 / year\)
* [② / Register an App ID](#step ② --register-an-app-id-in-your-apple-developer-account) 
* [③ / Create a new app in iTunes Connect](#step-③--create-a-new-app-in-itunes-connect-)
* [④ / Update your App Publish settings on Thunkable](#step-④--update-your-app-publish-settings-on-thunkable)
* [⑤ / Send your app to iTunes Connect on Thunkable](#step-⑤--send-your-app-to-itunes-connect-on-thunkable)

* [⑥ / Submit your app for review](#step-⑥--submit-your-app-for-review)

---

#### Step ①  / Enroll in the [Apple Developer Program](https://developer.apple.com/programs/) \(currently $99/year\)

![](/assets/publish-ios-fig-1.png)

---

#### Step ②  / [Register an App ID](https://developer.apple.com/account/ios/identifier/bundle/create) in your Apple Developer account

Apple will automatically generate a `Team ID` . . .

![](/assets/publish-ios-✕-fig-1.png)

and you will create a `Bundle ID`

![](/assets/publish-ios-✕-fig-2.png)

---

#### Step ③ / [Create a new app](https://itunesconnect.apple.com/) in iTunes Connect

iTunes Connect is your portal for managing your submission to the App Store

### ![](/assets/publish-ios-fig-6.png)

You will need to link the `Bundle ID` you created earlier

![](/assets/publish-ios-✕-fig-3.png)

---

#### Step ④ / Update your App Publish settings on Thunkable

To find the App settings, click on the App Icon on the top left.

**IMPORTANT Make sure your icon does not have any transparency in it otherwise Apple will not be able to accept it. **For more recommendations on App Name and Icons, please [visit this page](/x/create/app-icon-+-name.md)

![](/assets/publish-ios-✕-fig-4.png)

---

#### Step ⑤ / Send your app to iTunes Connect on Thunkable

Before you send your app to iTunes Connect, make sure you set the appropriate Build and Version Number. Apple requires each new version of your app to have a unique and sequentially higher Build and Version Number. You can also let Thunkable auto-increment \(or automatically increase\) the build and version numbers for you.

![](/assets/publish-ios-✕-fig-6.png)

To send your app to iTunes Connect, you'll simply select Publish to App Store and enter your Apple developer login credentials

#### ![](/assets/publish-ios-✕-fig-5.gif)

#### Wait \(up to an hour\)

You may have to wait up to an hour for the app to be successfully sent to iTunes Connect since we have to build the app and it must go through the Apple submission process.

#### Success!

If your app has been successfully uploaded, you will receive an email from iTunes Connect.

Your latest build will appear under the Testflight tab in your iTunes Connect dashboard. Testflight is a tool from Apple that allows you to test your app before it is submitted for release in the App Store. You can use the tool to share your app with others.

![](/assets/publish-ios-✕-fig-7.png)

You may need to answer a question about export compliance. You can select 'no' when asked if you app uses encryption since apps made on Thunkable for iOS do not at the moment.

![](/assets/publish-ios-✕-fig-8.png)

Your app is now ready for internal testing to be downloaded by you and others and ready to submit to the App Store. We recommend you test your app via Testflight before you submit your app for review to the App Store.

#### ![](/assets/publish-ios-fig-11.png)

#### Troubleshooting

**You do not see your app uploaded to iTunes Connect**

* Download. One way to check if your app is build-able is to download it to your phone first. Two common download errors are:
  * You uploaded an icon that has the same name as an existing asset that you have uploaded
  * Your app icon is not an image file
* Icons. Apple additionally does not allow you to have any icons with any transparent colors. We recommend app icons to be 192 x 192 px
* Membership. To publish to the App Store, you'll need to sign up for [Apple Developer Program Membership](https://developer.apple.com/programs/). This currently costs $99 / year.
* Login. Apple ID or password were entered incorrectly.  Since we don't store either one, there's no easy way for us to check so enter it slowly
* Certificates. If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time and Thunkable creates one when it publishes to your account
* Provisioning profile. After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive.  To publish successfully, you'll also need to delete any inactive provisioning profiles
* Two-factor authentication. You must turn off 2 factor authentication for your Apple Developer ID to publish with Thunkable

---

#### Step ⑥ / Submit your app for review

There are 3 main sections to fill out.

**App Information **which is pretty straightforward.

![](/assets/publish-ios-fig-12.png)The second section is **Pricing and Availability**. Also, very straightforward although there may be some strategy involved if you want to slowly release your app to different app stores \(New Zealand is a popular first country to launch in\).

![](/assets/publish-ios-fig-13.png)

The final section contains the design assets \(**Screenshots, App Icon**\) which you will need to have ready.

**IMPORTANT For the App Store, iOS requires you to submit an additional app icon with no transparency at sized at 1024 x 1024 px. **To generate this icon, we recommend a tool [like this](https://makeappicon.com/) to generate this icon

**Also, by default, Thunkable submits your app to be available for both iPhone and iPad so you'll have to submit screenshots for both iPhone and iPad. ** For generating screenshots, we recommend a tool [like this](https://shotbot.io/?utm_source=makeappicon&utm_medium=web&utm_campaign=makeappicon)

![](/assets/publish-ios-fig-14.png)

You'll also need to select the build version that you want to submit.

#### ![](/assets/publish-ios-fig-15.png)![](/assets/publish-ios-fig-16.png)

#### Congrats! You are now ready to submit to the App Store.

### 



