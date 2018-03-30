#### Thunkable **Cross-Platform **✕ \(Beta\)

# Troubleshooting

---

### `Live Testing`

Common issues

**You see a blank / white screen when you live test \(even if there are items in your app\)**

* If you have a Navigator as the first item in your tree, make sure your screen is dropped within it
* Your have unconnected blocks
* You have an event triggered by a Screen.Start which may be causing the screen to crash
* You may not be logged in to the same account as your 

**Image is not showing up on your phone**

* The height or width of the image may be set to 'Fit contents'

---

### `Download for iOS`

Common issues

**You receive an email from the hard-working beaver saying that this app will not build**

* You uploaded an icon that has the same name as an existing asset that you have uploaded
* Your app icon is not an image file

### `Download for Android`

Common issues not yet reported

---

### `Publish for iOS`

Common issues

**You do not see your app uploaded to iTunes Connect**

* Download. Your app cannot build for reasons stated above. One way to check if your app is build-able is to download it to your phone first
* Icons. Apple doesn't allow you to have any icons with any transparent colors. We recommend app icons to be 192 x 192 px
* Membership. To publish to the App Store, you'll need to sign up for [Apple Developer Program Membership](https://developer.apple.com/programs/). This currently costs $99 / year.
* Login. Apple ID or password were entered incorrectly.  Since we don't store either one, there's no easy way for us to check so enter it slowly
* Certificates. If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time and Thunkable creates one when it publishes to your account
* Provisioning profile. After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive.  To publish successfully, you'll also need to delete any inactive provisioning profiles
* Two-factor authentication. You must turn off 2 factor authentication for your Apple Developer ID to publish with Thunkable

### `Publish for Android`

This feature is not yet available

