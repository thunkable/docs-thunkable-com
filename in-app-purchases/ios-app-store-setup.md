# iOS App Store Setup

## Setup your account

Before you can create your In-App Purchases, you are required by Apple to request and fill out their Paid Applications contract.

To do so, log into your App Store Connect account, and go to the Agreements, Tax, and Banking section. In this section, you will see the ability to request the Paid Applications contract towards the top of the page.

After this is complete, you will now be able to add your In-App Purchases.

* Consumable - a one-off purchase which can be repeated and keeps no history&#x20;
* Non-Consumable - a product that can only be purchased once and keeps history in your apple account. If you try and buy a second time, it reports you have already purchased and offers a free download
* Auto-Renewable Subscription
* Non-Renewing Subscription

## Create the item or subscription to purchase

{% tabs %}
{% tab title="Consumable, Non-Consumable, or Non-Renewing Subscriptions" %}
**Required role:** You must have the [Account Holder](https://help.apple.com/app-store-connect/#/dev1d7b9bccf), [Admin](https://help.apple.com/app-store-connect/#/devf3ef59c83), [App Manager](https://help.apple.com/app-store-connect/#/dev26fb1aeb8), [Developer](https://help.apple.com/app-store-connect/#/deveb40aa0cc), or [Marketing](https://help.apple.com/app-store-connect/#/dev6ce96c97a) role to add and edit in-app purchases. See [Role permissions](https://help.apple.com/app-store-connect/#/deve5f9a89d7).

1. From My Apps, select your app.
2. In the sidebar under In-App Purchases, click Manage.
3.  To add an in-app purchase, go to In-App Purchases and click the Add button (+).

    ![App Details Menu](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/InApp\_AppDetails-menu-5\_2x.png)
4. Select Consumable, Non-Consumable, or Non-Renewing Subscriptions and click Create. For auto-renewable subscriptions, see [Create an auto-renewable subscription](https://help.apple.com/app-store-connect/#/dev06f89ce98).
5. Add the reference name, product ID, and a localized display name.
6.  Click Save, or Submit for Review.

    You can enter all your metadata when you create your in-app purchases, or enter your in-app purchase information later.

{% hint style="info" %}
All in-app purchase metadata can be edited, except the Product ID and in-app purchase type. If your in-app purchase has never been submitted to Apple for review, you can make changes to your metadata. If your in-app purchase has already been submitted, some changes require approval by App Review.
{% endhint %}
{% endtab %}

{% tab title="Auto Renewable Subscriptions" %}
## Create an auto-renewable subscription <a href="#dev06f89ce98" id="dev06f89ce98"></a>

To offer auto-renewable subscriptions within your app, you must first create auto-renewable subscription products in App Store Connect. When you create your first subscription product, the App Store Connect flow will guide you to create your first subscription group. When you create additional subscription products, you'll be able to add these products to the subscriptions groups you've already created, or create a new group. Before creating subscriptions, ensure that you understand the right subscription setup for your business model. See [Overview of auto-renewable subscription group setup](https://help.apple.com/app-store-connect/#/dev75708c031).

To learn more about the subscription business model for your app, read [Offering Subscriptions](https://developer.apple.com/app-store/subscriptions/whats-new).

**Required role:** [Account Holder](https://help.apple.com/app-store-connect/#/dev1d7b9bccf), [Admin](https://help.apple.com/app-store-connect/#/devf3ef59c83), [App Manager](https://help.apple.com/app-store-connect/#/dev26fb1aeb8), [Developer](https://help.apple.com/app-store-connect/#/deveb40aa0cc), or [Marketing](https://help.apple.com/app-store-connect/#/dev6ce96c97a). See [Role permissions](https://help.apple.com/app-store-connect/#/deve5f9a89d7).

### Create a subscription product

1. From My Apps, select your app.
2. In the sidebar under In-App Purchases, click Manage.
3.  Scroll to the In-App Purchases section and click the Add button (+).

    ![App Details Menu](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/InApp\_Create\_an\_auto-renewable\_subscription\_Create\_a\_subscription\_group\_Step3.png)
4.  Select auto-renewable subscription, then click create.

    _Note:_ If you'd like your subscription to be accessible from more than one app, create an equivalent subscription product for each app. For more information, see [Offering Subscription Products Across Multiple Apps](https://developer.apple.com/documentation/storekit/in-app\_purchase/offering\_a\_subscription\_across\_multiple\_apps).
5.  Add your in-app purchase reference name and product ID, then click Next.

    ![Create Auto-Renewable Subscription](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/InApp\_Create\_Subscription.png)
6.  If this is the first auto-renewable subscription product you are creating, you'll need to also create a subscription group (you'll be able to add details to it later), by selecting Choose New Subscription Group. If you've already created subscription products and groups before, add your subscription product to an existing group or create a new subscription group. Then click Create.

    **Important:** How you set up your subscription group or groups will determine how customers can subscribe to your content or services, how they move between subscriptions, when they are billed, and your proceeds. See \[\<Overview of setting up auto-renewable subscriptions>] and ensure that you understand the right subscription setup for your business model. Keep in mind that a subscription cannot belong to more than one group and cannot switch groups after it’s been created.

    ![Create Subscription Group](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/InApp\_Create\_Subscription\_Group.png)

    The Subscription Group page will open.
7. Once you've created your subscription product, you'll be taken to its information page to add more details. Under Subscription Duration, choose a duration from the pop-up menu.
8. Under Subscription Prices, [set a price for your auto-renewable subscription](https://help.apple.com/app-store-connect/#/devc9870599e).
9. Under Localizations, click on the Add button (+) to add a language for your localized display name.
10. Enter your localized information.

    ![Understanding Subscription Group Display Name](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/InApp\_Understanding\_Subscription\_Groups4\_2x.png)
11. Under App Store Promotion, optionally add a promotional image. Learn more about [Promoting In-App Purchases](https://developer.apple.com/app-store/promoting-in-app-purchases/).
12. Under Review Information, provide any additional information that may help the App Review team review your in-app purchase.
13. Click Save.
{% endtab %}
{% endtabs %}

<details>

<summary>The difference between Consumable, Non-Consumable, or Non-Renewing Subscriptions, and auto-renewable Subscriptions. </summary>

**Consumable**

[Products](http://initech.co.il/definition-and-analysis/) that are used one time, after which they become depleted and need to be purchased again, are usually implemented as consumables. For example, fish food in a fishing app could be implemented as a consumable product.

**Non-Consumable**

Non-consumable products are purchased once by users and do not expire or decrease with use. For example, new race tracks for a game could be implemented as non-consumable products.

Apple can host your non-consumable products for you.

**Auto-Renewable Subscription**

Auto-renewable subscriptions allow users to purchase dynamic content, such as magazine subscriptions, for a set duration of time. Subscriptions renew automatically unless the user opts out of the renewal. If the content you want offer doesn’t fit what’s outlined in the[ App Review Guidelines](https://developer.apple.com/appstore/guidelines.html), consider offering the content through a non-renewing subscription.

Auto-renewable subscriptions can include an incentive to customers who share their contact information with you.

**Free Subscription**

Free subscriptions allow users to download dynamic content, such as magazine subscriptions, for a set duration of time. Free subscriptions are a way for developers to put free content in the Newsstand in the App Store. After a user signs up for a free subscription, the subscription content will be available on all devices associated with the user’s Apple ID. Note that free subscriptions do not expire and can be offered only in Newsstand-enabled apps.

Free subscriptions don’t offer a marketing opt-in incentive as do auto-renewable subscriptions, but users are prompted to share their information.

Free Subscriptions are not available for Mac apps.

**Non-Renewing Subscription**

Non-renewing subscriptions allow the sale of items with a limited duration. They are used for products that offer time-based access to static content.

If you use non-renewing subscriptions, your app is responsible for delivering the subscription to all devices associated with the user’s Apple ID.

Because a non-renewing subscription requires a user to renew each time the subscription ends, your [app](http://initech.co.il/mobile-app-development/) must contain code that recognizes when the subscription is due to expire and prompt the user to purchase a new subscription.

Source: [Apple Official In-App Purchase Guide](https://developer.apple.com/library/ios/documentation/LanguagesUtilities/Conceptual/iTunesConnectInAppPurchase\_Guide/Chapters/CreatingInAppPurchaseProducts.html#//apple\_ref/doc/uid/TP40013727-CH3-SW1)

</details>



## Setup in-app purchase testers  <a href="#dev7e89e149d" id="dev7e89e149d"></a>

{% tabs %}
{% tab title="Setup Test Users" %}
You can test your app and in-app purchases without creating financial transactions by using sandbox, a test environment that uses the infrastructure of the App Store but doesn’t process actual payments. Instead, it returns transactions as if payments were processed successfully.&#x20;



1.  From [Users and Access](https://help.apple.com/app-store-connect/#/devd2fe02057), click Testers under Sandbox.


2. Click the Add icon (+).
3. Enter the tester information, then click Invite.

![](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/users\_and\_roles\_sandbox\_testers.png)

Account information cannot be edited once a Sandbox Apple ID is created.
{% endtab %}

{% tab title="Clearing test purchase history" %}
You can clear the purchase history for a tester so that you can continue to use the same sandbox Apple ID for ongoing testing. Clearing purchase history will delete all past auto-renewable subscriptions and non-consumables purchased by the selected testers in the sandbox environment. In-app purchases made by customers on the App Store are not affected.

To clear tester purchase history:

1. From Users and Access, under Sandbox, click Testers.
2.  Click Edit.


3.  Select the checkbox for each tester you want to modify and click Clear Purchase History.


4.  Click Clear Purchase History in the dialog that appears.



    Sandbox Apple IDs with a high number of purchases may take longer to clear. This action cannot be reversed.

![](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/sandbox\_edit.png)

![](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/sandbox\_clear\_history.png)

![](https://help.apple.com/app-store-connect/en.lproj/GlobalArt/sandbox\_clear\_confirm.png)

##
{% endtab %}

{% tab title="Subscription Renewal Rate" %}
### Subscription Renewal Rate

You can choose a subscription renewal rate for each tester to speed up or slow down how often subscriptions renew. Subscriptions are automatically canceled after 12 renewals.

By default, a one month renewal lasts 5 minutes. If you wish to speed up the renewal period, you can choose 3 minutes. If you wish to slow down the renewal period, you can choose 15 minutes, 30 minutes, or an hour.

The columns in the chart below represent each of the accelerated renewal rates you can select for a tester in App Store Connect. The corresponding test durations are listed underneath the accelerated rates for each product duration.

<table data-header-hidden><thead><tr><th></th><th width="177"></th><th></th><th></th><th></th><th></th></tr></thead><tbody><tr><td>Actual Duration</td><td>Monthly renewal every 3 minutes</td><td>Monthly renewal every 5 minutes (default)</td><td>Monthly renewal every 15 minutes</td><td>Monthly renewal every 30 minutes</td><td>Monthly renewal every hour</td></tr><tr><td>1 week</td><td>3 minutes</td><td>3 minutes</td><td>5 minutes</td><td>10 minutes</td><td>15 minutes</td></tr><tr><td>1 month</td><td>3 minutes</td><td>5 minutes</td><td>15 minutes</td><td>30 minutes</td><td>1 hour</td></tr><tr><td>2 months</td><td>6 minutes</td><td>10 minutes</td><td>30 minutes</td><td>1 hour</td><td>2 hours</td></tr><tr><td>3 months</td><td>9 minutes</td><td>15 minutes</td><td>45 minutes</td><td>1 hour 30 minutes</td><td>3 hours</td></tr><tr><td>6 months</td><td>18 minutes</td><td>30 minutes</td><td>1 hour 30 minutes</td><td>3 hours</td><td>6 hours</td></tr><tr><td>1 year</td><td>36 minutes</td><td>1 hour</td><td>3 hours</td><td>6 hours</td><td>12 hours</td></tr></tbody></table>

###
{% endtab %}

{% tab title="Interrupted Purchases" %}
You can test interrupted purchase scenarios on a device running iOS 14 or later by enabling interrupted purchases in App Store Connect for a specific tester Sandbox Apple ID. If this option is selected, on-device purchase attempts by that Sandbox Apple ID will be interrupted in the sandbox environment and continue to be interrupted until the option is deselected or the tester agrees to terms and conditions on their iOS device. This allows you to test your app’s handling of an interruption to ensure a seamless customer experience.

In general, an interrupted purchase is experienced anytime a customer needs to address an issue with their Apple ID. Some example scenarios include:

* The user needs to agree to updated terms and conditions.
* The user needs to update an expired payment method.

When interrupted purchase is enabled for a sandbox tester, all purchases will be interrupted for that Sandbox Apple ID, preventing the transaction from completing until resolved. In sandbox, the tester will need to agree to terms and conditions in order to complete the purchase. Purchases will continue to be interrupted on the Sandbox Apple ID until you disable the option in App Store Connect or the tester agrees to terms and conditions on their iOS device.

Follow the steps outlined in [Testing In-App Purchases with Sandbox](https://developer.apple.com/documentation/storekit/original\_api\_for\_in-app\_purchase/testing\_in-app\_purchases\_with\_sandbox) to understand what to test and how to use your device in a testing environment.
{% endtab %}

{% tab title="App Store Country or Region" %}
You can change the account region for a tester to any of the 175 different regions for the App Store. This allows you to continue testing on different storefronts using the same Sandbox Apple ID, without having to create new testers.

You will need to sign in again with your Sandbox Apple ID on your device to complete this change.
{% endtab %}
{% endtabs %}

## Create an app password

#### Create an App Password: used to verify purchases

1. Navigate to [Appleid.apple.com](https://appleid.apple.com/) from your web browser and sign in with your Apple ID and Password.
2. Verify your identity with two-factor authentication.
3.  Under the Security section, select **Generate Passwords**.

    If you don't see the option to generate app-specific passwords, you'll need to [enable two-factor authentication](https://www.imore.com/how-enable-2-factor-authentication-iphone-and-ipad), which is [different than two-step verification](https://www.imore.com/two-factor-authentication).
4. Enter a **label** for the password. Be sure the name relates to the app for which you are generating the password, like "Outlook" or "Thunderbird."
5. Select **Create**.
6.  Copy the **app-specific password** you generated and save it in a file on your local system such that you may reference it as needed while building your app.&#x20;



![](https://www.imore.com/sites/imore.com/files/styles/xlarge/public/field/image/2017/05/generate-app-specific-password-01.jpg?itok=oX08V5e7)

![](https://www.imore.com/sites/imore.com/files/styles/xlarge/public/field/image/2017/05/generate-app-specific-password-02.jpg?itok=2zxkCWt\_)

![](https://www.imore.com/sites/imore.com/files/styles/xlarge/public/field/image/2017/05/generate-app-specific-password-03.jpg?itok=8ddj1IIs)

###
