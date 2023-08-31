# App Data Privacy

One of the reasons you may want to create your own app is to keep the data that you often share with apps visible to only people you trust (and not a big company or hackers).

Since big companies and hackers often target large repositories of sensitive data, simply using an app that you build and keep secure may be one of the best defences for keeping data in your own hands.

## Recommendations for keeping your data private

### Store data locally

For simple personal data like user login info, you can use a [local table data source](../../getting-started/data-sources.md#create-your-own-table) to save data directly to the device.

{% hint style="info" %}
Data stored locally on the phone is often uploaded to the cloud by a phone's back-up provider.
{% endhint %}

### Create your own private repository of cloud data

Most data today is stored and shared from the cloud, so the first step in keeping your data private is to create your own repository that can be linked to your app. This includes databases powered by [Firebase](https://firebase.google.com/), [Cloudinary](https://cloudinary.com/), and  [Airtable](https://www.airtable.com/).

Creating your own repository takes a few more steps to set up but makes data you upload not visible to Thunkable (We provide a default account for convenience purposes).

{% hint style="info" %}
Cloud database services like Firebase, Cloudinary and Air Table will often use another 3rd party like Google Cloud or Amazon Web Services to store your data but smaller repositories of data are less likely to be looked at.
{% endhint %}

### Require a password to sign in to your app

You may want to limit access to your app on the initial screen by requiring a unique one-time password that all users must know to proceed further. You can use a [Text Input](../../app-design/ui-components/basic-components/text-input.md#set-up-for-passwords) component to create a simple version of this. One challenge of this approach is to communicate securely to your users what this password is.

### Require sign in for your app

If you don't want to require a password, you can use the [Sign In](../../blocks/app-features/sign-in.md) component to manage users who have access to the app. Users must first create a password with their email address. You can add an additional level of security by requiring users to verify their email address, which sends them an email at their address before they can sign in to your app.

### Share your app with a specific audience

Any type of sign in creates friction for the user and one way to avoid this is to ensure that your app only reaches the users you specify.

There are several approaches to sharing an app with a shared cloud database.&#x20;

| Approach                                                                                                                     | Description                                                                                                                                                                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Share the packaged app](download-and-share/download.md#download-and-install-android-app)                                    | For Android, users must follow these instructions to [install the Thunkable app on their device](download-and-share/download.md#to-install-allow-apps-from-unknown-sources).                                                                                                                                                             |
| [Share a read-only version](download-and-share/share-1.md#share-a-read-only-version-of-your-app-project-by-link) of your app | Users will have to install the Thunkable Live app on their device, sign up for a Thunkable account and select "Live Test" from the Thunkable platform                                                                                                                                                                                    |
| [Share a copy](download-and-share/share-1.md#share-a-copy-of-your-app-project-by-link) of your app                           | Users will have to install the Thunkable Live app on their device, sign up for a Thunkable account, and for apps powered by Firebase, copy the credentials into their app project (credentials are cleared with apps are shared). Users can [Live Preview](../../getting-started/live-test.md#live-preview-android-only) from their app. |
