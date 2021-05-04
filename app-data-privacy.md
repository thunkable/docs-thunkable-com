# 🔒 App Data Privacy

One of the reasons you may want to create your own app is to keep the data that you often share with apps visible to only people you trust \(and not a big company or hackers\).

Since big companies and hackers often target large repositories of sensitive data, simply using an app that you build and keep secure may be one of the best defenses for keeping data in your own hands.

Here are a few tips on how to keep your data private even and especially from us:

## Store data locally

For simple, personal pieces of data like user login info, you can use the [Local Storage]() component to save data to the phone itself.

{% hint style="info" %}
Data stored locally on the phone is often uploaded to the cloud by a phone's back-up provider.
{% endhint %}

## Create your own private repository of cloud data

Most data today is stored and shared from the cloud so the first step in keeping your data private is to create your own repository that can be linked to your app. This includes [Realtime DB]() powered by Firebase, [Media DB]() powered by Cloudinary, and [Spreadsheet]() \(required by default\) powered by Air Table.

Creating your own repository takes a few more steps to set up but makes data you upload not visible to Thunkable \(We provide a default account for convenience purposes\).

{% hint style="info" %}
Cloud database services like Firebase, Cloudinary and Air Table will often use another 3rd party like Google Cloud or Amazon Web Services to store your data but smaller repositories of data are less likely to be looked at.
{% endhint %}

## Require a password to sign in to your app

You may want to limit access to your app on the initial screen by requiring a unique one-time password that all users must know to proceed further. You can use a [Text Input](text-input.md#set-up-for-passwords) component to create a simple version of this. One challenge of this approach is to communicate securely to your users what this password is.

## Require sign in for your app

If you don't want to require a password, you can use the [Sign In](sign-in.md) component to manage users who have access to the app. Users must first create a password with their email address. You can add an additional level of security by requiring users to verify their email address, which sends them an email at their address before they can sign in to your app.

{% hint style="info" %}
There is currently a bug with email verification. We hope to fix this soon.
{% endhint %}

## Share your app with a specific audience

Any type of sign in creates friction for the user and one way to avoid this is to ensure that your app only reaches the users you specify.

There are several approaches to sharing an app with a shared cloud database. Unfortunately all approaches do require a bit of friction that we are working to reduce.

| Approach | Description |
| :--- | :--- |
| [Share the packaged app](download.md#download-and-install-android-app) | For Android, users will have to follow instructions to [install the Thunkable app on their device](download.md#to-install-allow-apps-from-unknown-sources). This approach is not recommended for iOS since there is a download limit of one app per device and users are not advised to share their download link.  Users will also have to follow these instructions to [install the app on their iOS device](download.md#to-install-trust-thunkable-on-your-device). You will also have to re-share these links if you update your app. |
| [Share a read-only version](share-1.md#share-a-read-only-version-of-your-app-project-by-link) of your app | Users will have to install the Thunkable Live app on their device, sign up for a Thunkable account and select "Live Test" from the Thunkable platform |
| [Share a copy](share-1.md#share-a-copy-of-your-app-project-by-link) of your app | Users will have to install the Thunkable Live app on their device, sign up for a Thunkable account, and for apps powered by Firebase, copy the credentials into their app project \(credentials are cleared with apps are shared\). Users can [Live Preview](get-started/live-test.md#live-preview-android-only) from their app. |

