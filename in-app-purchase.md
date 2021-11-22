# In-App Purchase



{% hint style="info" %}
In-App Purchases is available to Thunkers on PRO, Business and Enterprise plans.&#x20;

[Sign up for a plan on our pricing page.](https://thunkable.com/#/pricing)
{% endhint %}

## Compatibility

* The IAP component works on the Android platform and iOS platform.
* Currently, there is no support for IAP on web apps
* The IAP component doesn’t work on the Thunkable live apps (Android/iOS)

## **Initial Setup**

Before you set up your IAP blocks in Thunkable, you need to establish a set of product IDs. Each product ID is associated with the item being paid for.&#x20;

If you are developing for both Android & iOS, we suggest you use the same product ID for similar items in both stores.

Product IDs need to start with a number or lower case letter, and be 148 characters or less. They can contain  any of the following characters: numbers (0-9), lowercase letters (a-z), underscores (\_), and periods (.)

### Google Play Store (Monetize → Products)

Select your product type:

* In-App Product - a one-time purchase
* Subscription - recurring purchases

[Read: Earn | Google Play | Android Developers](https://developer.android.com/distribute/best-practices/earn)

### Apple App Store (In-App Purchase → Manage)

Before you can create your In-App Purchases, you are required by Apple to request and fill out their Paid Applications contract.

To do so, log into your App Store Connect account, and go to the Agreements, Tax, and Banking section. In this section, you will see the ability to request the Paid Applications contract towards the top of the page.

After this is complete, you will now be able to add your In-App Purchases.

* Consumable - a one-off purchase which can be repeated and keeps no history&#x20;
* Non-Consumable - a product that can only be purchased once and keeps history in your apple account. If you try and buy a second time, it reports you have already purchased and offers a free download
* Auto-Renewable Subscription
* Non-Renewing Subscription

[Read: In-App Purchase - App Store](https://developer.apple.com/in-app-purchase/)

## Properties

To add IAP to your project, navigate to Add Components and enter “IAP” into the search bar. Drag the In-App Purchase component to the Invisible Components section above.

![](<.gitbook/assets/image (221).png>)

Next, you will need to add the product IDs on the Properties panel on the right. These strings must match what you have in the App Store or Play Store. Make sure you double-check that you add Items as Items, and Subscriptions as Subscriptions.

![](<.gitbook/assets/image (216).png>)

## Blocks

### For Sale

If you need to pull the product/subscription info from the Play Store or App Store, you can use the following block. For the fields in the return object, you can reference them here.

![](broken-reference)

### Purchasing

You can use the following blocks to start the one-time purchase or subscription. For the fields in the return object, you can reference them here.

![](broken-reference)

![](broken-reference)

###

### Purchase History&#x20;

You can use the following block to get the purchase history and you can verify the purchase from the return list. This block is helpful when you need to restore an existing purchase either on a new device or a new app installation. For the fields in the return object, you can reference them here.

![](broken-reference)

![](broken-reference)

{% hint style="warning" %}
The "Get Most Recent Active Purchase" block may crash your iOS app.&#x20;
{% endhint %}

## Testing

To test the IAP component, you have to publish it to the Google Play Store or App Store. You will not be able to test IAP with the Thunkable Live App or through Web Preview.

{% hint style="warning" %}
Be mindful to leave extra time for testing in your app development cycle to allow time for each respective store to review your apps. Depending on your stage of app development, a review could take anywhere from an hour to 4 days.
{% endhint %}

### App Store (iOS):

On iOS you need to submit to the App Store via Testflight to test the features.&#x20;

Testflight sets up a sandbox environment automatically. When you send your update to the app store, you are able to test without having it go to the live version.

[Read more about Testflight here. ](https://developer.apple.com/testflight/)

### Play Store (Android):

On Android publish to the Play Store via internal beta testing. You can read more about internal beta testing in the Play Store here.

You have to upload the APK or AAB file to the Play Store console before you can add any In-App Purchases.

There are two ways you can test how a pre-release app functions on the Google Play store: You can publish an app to the alpha or beta distribution channels. This makes the app available on the Google Play store, but only to the testers you put on a "whitelist."

&#x20;In a few cases, you can test Google Play functionality with an unpublished app. For example, you can test an unpublished app's in-app billing support by using static responses, special reserved product IDs that always return a specific result (like "purchased" or "refunded").
