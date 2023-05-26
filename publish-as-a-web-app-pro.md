---
description: How to publish your project to the internet as a web app
---

# Publish as a Web App

Publishing as a web app is the fastest way to publish your Thunkable app. This means that you can get user feedback in minutes instead of hours or days. One major advantage to publishing on the internet is that you don't need to pay additional fees to an app marketplace.&#x20;

{% hint style="info" %}
Publishing as a web app is available for Thunkable creators with active pro subscriptions. To upgrade your subscription please visit your [membership page](https://x.thunkable.com/account/membership). If you cancel your pro membership, your app will be unpublished once your pro membership expires.
{% endhint %}

## Mobile Web App

![](<.gitbook/assets/mobile\_web\_app (1).png>)

Mobile web apps are best experienced by opening the link directly on your phone. To make your mobile app feel more like a native app you can add it to the [home screen](https://intercom.help/thunkable/en/articles/3828958-add-to-home-screen) directly from your mobile web browser.

If you preview a mobile web app on a desktop or laptop computer you will see a phone frame around the app. This is to give you a rough idea of its final proportions, but ultimately this will vary from device to device depending on factors such as screen size, aspect ratio, and pixel density.

To get an app that can respond to devices of any size, consider publishing as a [Responsive Web App](publish-as-a-web-app-pro.md#responsive-web-app).

## Responsive Web App

![](.gitbook/assets/responsive\_web\_app.png)

Publishing your app as a responsive web app means that it will scale according to the size of the device that it is being opened on.&#x20;

If your app in designed only to be run on phones, consider publishing as a [Mobile Web App](publish-as-a-web-app-pro.md#mobile-web-app).

## Demo

Here's a 3 minute overview of how "Publish as a Web App" works.

{% embed url="https://www.youtube.com/watch?v=7SgIseIqZWk" %}

## Publish web app

Click the Download and Publish icon and select **Publish web app.**

![](<.gitbook/assets/Download and Publish menu (2).png>)

In the next modal you can:

* open the app in a new tab
* copy the app link
* select whether to publish as a [**Mobile web app**](publish-as-a-web-app-pro.md#mobile-web-app) or a [**Responsive web app**](publish-as-a-web-app-pro.md#responsive-web-app)
* share your app through popular channels like Facebook, Twitter and Reddit&#x20;
* **unpublish** your app by clicking on `Disable published link` text

![](<.gitbook/assets/publish-as-web-app (2).png>)

🎉 Congratulations - your Thunkable project is now live on the internet a published web app.

## Publish to a custom domain

### Configure your domain

You need to configure your domain before you can publish your app to that domain. To do so, add the Thunkable IP address (34.136.177.42) to the A record of your domain which you can usually find in the DNS section of your domain provider.

Here are the instructions from some popular domain name providers:&#x20;

* [Namecheap](https://www.namecheap.com/support/knowledgebase/article.aspx/319/2237/how-can-i-set-up-an-a-address-record-for-my-domain/)
* [AWS](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/ResourceRecordTypes.html#AFormat)
* [Digital Ocean](https://docs.digitalocean.com/products/networking/dns/how-to/manage-records/)
* [Google Domains](https://support.google.com/domains/answer/3290350?hl=en)
* [GoDaddy](https://www.godaddy.com/help/add-an-a-record-19238)

DNS synchronization often takes less than an hour but may take up to 72 hours. If your domain is not connecting within 48 hours, we recommend the following troubleshooting steps:

* Confirm the IP address added to your A record is the correct IP (34.136.177.42).
* Ensure you are using `http://` and not `https://`.

### Publish to a custom domain

**Note:** The windows you see may look slightly different from the ones shown below. The windows and prompts vary based on whether or not you’ve published your app as a web app previously.

To publish your web app to a custom domain:

1. Click the **Download and Publish** icon.\
   \
   ![](<.gitbook/assets/Download and Publish menu (2).png>)\

2. Select **Publish web app**.\

3. Add your custom domain in the provided field and click **Add Domain**. Note: this must be the domain and not the URL.\

4.  Click **Check Status**. \


    <figure><img src=".gitbook/assets/custom domain  check status.png" alt=""><figcaption></figcaption></figure>
5. A green **Connected** tag will appear in the field when there is a successful connection. \

6. Ensure the box next to **Publish web app to this domain** is checked.\

7. Select a web app format (Mobile web app or Responsive web app).\

8.  Click **Get link and publish** or **Publish current version**.\
    \


    <figure><img src=".gitbook/assets/custom domain  connected.png" alt=""><figcaption></figcaption></figure>
9. Click **Done**.

## Updating your App

Each time you press publish it’s similar to creating a new release of your app in one of stores. This means you can make changes and updates to your  without worrying about users seeing a half-finished new feature that you’re still working on.

When you’re ready to release a new version, choose “Publish as a Web App” then click the blue “Publish current version” to update your app. The URL will remain the same, but the project that it links to will be updated.

![](.gitbook/assets/screen-shot-2021-04-12-at-9.25.00-am.png)

## Embed your app in a webpage

If you host a webpage, you can embed your Thunkable web app in an iframe using the syntax

`<iframe src="https://thunkable.site/w/K0XDxMqwl" title="Chop Down the Tree Thunkable App" height = 1000 width = 500></iframe>`

You can read more about iframes [here](https://www.w3schools.com/tags/tag\_iframe.ASP).

## Unsupported Components&#x20;

Not all components are supported on the web at this time so please see the list below of components that are not supported. Please note that some are **`Supported but may not work as expected`**so may not work consistently on every device. Others, such as AdMob **`Can not be supported`**but may be replaced by an alternative in the future. While other are  **`Not supported yet`** but may be made available in future updates.

| Component                | Category       | Status                                                     |
| ------------------------ | -------------- | ---------------------------------------------------------- |
| **Accelerometer**        | Sensors        | **`Supported but may not work as expected`**               |
| **AdMob**                | Monetization   | **`Interstitial and Video ads not supported`**             |
| **Assistant**            | Voice          | **`Not supported yet`**                                    |
| **Barcode Scanner**      | Image          | **`Not supported yet`**                                    |
| **Bluetooth Low Energy** | Sensors        | **`Not supported yet`**                                    |
| **Camera**               | App Features   | `Not supported on browsers on iOS`                         |
| **Gyroscope**            | Sensors        | **`Supported but may not work as expected`**               |
| **Magnetometer**         | Sensors        | **`Supported but may not work as expected`**               |
| **Map**                  | Location       | **`Not supported yet`**                                    |
| **Push Notification**    | Social         | **`Not supported yet`**                                    |
| **Share**                | Social         | **`Email and Phone work, other blocks not supported yet`** |
| **Speech Recognizer**    | Voice          | **`Not supported yet`**                                    |
| **Web Viewer**           | User Interface | **`Some Google sites not supported`**                      |

## Troubleshooting

* **404 Not Found** - This error is seen when a user tries to access a web app that the Creator unpublished.
