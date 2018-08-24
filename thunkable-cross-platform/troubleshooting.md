# Troubleshooting

Here are some of the most common issues that our users are running into:

* [Live Test \(iOS\)](troubleshooting.md#live-test-ios)
* [Download \(iOS\)](troubleshooting.md#download-ios)
* [Publish \(iOS\)](troubleshooting.md#publish-ios)
* [Live Test \(Android\)](troubleshooting.md#live-test-android)
* [Download \(Android\)](troubleshooting.md#download-android)
* [Publish \(Android\)](troubleshooting.md#publish-android)

## Live Test \(iOS\)

Common issue

**You see a blank / white screen when you live test \(even if there are items in your app\)**

* If you have a Navigator as the first item in your tree, make sure your screen is dropped within it
* Your have unconnected blocks
* You have an event triggered by a Screen.Start which may be causing the screen to crash
* Your app and desktop may not be logged into the same account

**Image is not showing up on your phone**

* The height or width of the image may be set to 'Fit contents'

## Download \(iOS\)

Common issues

**You receive an email from the hard-working beaver saying that this app will not build**

Common issues

* You uploaded an icon that has the same name as an existing asset that you have uploaded
* Your app icon is not an image file
* We are having trouble with our build servers. Please try again in 30 minutes or chat with us if you are still having problems

**You cannot install your app and get the message "Cannot connect to storage.googleapis.com"**

* You have a special character like "&" in your [App Name](create/app-icon-+-name.md#app-name)

## Publish \(iOS\)

Common issues

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
* Apple ID an privacy terms. You must accept Apple's new Apple ID and privacy terms.

## Live Test \(Android\)

Common issues

**You see a blank / white screen when you live test \(even if there are items in your app\)**

* If you have a Navigator as the first item in your tree, make sure your screen is dropped within it
* Your have unconnected blocks
* You have an event triggered by a Screen.Start which may be causing the screen to crash
* Your app and desktop may not be logged into the same account

**App is crashing because of a bug on our end; we are trying to fix it as soon as we can**

* You are trying to set the value of a Slider in your blocks 
* You are trying to set the latitude and longitude of a Map in your blocks

**Image is not showing up on your phone**

* The height or width of the image may be set to 'Fit contents'

## Download \(Android\)

No issues reported

## Publish \(Android\)

**You cannot update an existing app on the Google Play Store**

* If you updating an existing app on the Google Play Store, your app will need to have the i\) [same package name](create/package-name-+-bundle-id.md), ii\) a higher or incremented version number, and the iii\) same keystore. The first two are easily editable in the App Settings page but the keystore is not yet able to be imported / exported. 
* Copied apps within an account \(using the [Make Copy](create/make-copy.md)\) will keep the same keystore as the original app. Apps that are copied from a [Share copy](share.md#share-a-fully-editable-copy-of-your-app-project) link will not have the same keystore. Apps from the [Thunkable Classic platform](../thunkable-classic-android/) cannot yet be updated since it is not yet possible to import the keystore.  

