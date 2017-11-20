#### **Thunkable for iOS **

# Troubleshooting

---

### `Download`

Common issues

* You uploaded an icon that has the same name as an existing asset that you have uploaded

Custom icon not showing

* We recommend uploading an icon asset that is at least 200 px by 200 px

---

### `Publish`

Common issues

* _Login_. Apple ID or password were entered incorrectly.  Since we don't store either one, there's no easy way for us to check so enter it slowly
* _Certificates_. If you have an existing Apple Developer Program account with 2 iOS certificates, you'll have to revoke one. Apple only allows developers to have 2 iOS certificates at a time and Thunkable creates one when it publishes to your account.

* _Provisioning profile_. After you revoke your certificate, it is possible that one or more of your provisioning profiles will become inactive.  To publish successfully, you'll also need to delete any inactive provisioning profiles.

* _Two-factor authentication_. You must turn off 2 factor authentication for your Apple Developer ID to publish with Thunkable



