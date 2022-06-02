# Email Sign In by Firebase

{% hint style="info" %}
To use Sign In, you will need to first create your own Firebase account and project
{% endhint %}

## Video Tutorial

You can watch a video to learn about all of the Sign In blocks here:

{% embed url="https://www.youtube.com/watch?v=tdgVeck-sOI" %}

## Getting Started

### Create your free [Firebase](https://firebase.google.com/) account and create a new project

![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.19.36 PM.png>)

### Enable Email / Password Sign in

In the Firebase console, navigate to Authentication go to the `Sign-in Method` tab.

Find the `Email/Password` item under `Sign-in providers`.&#x20;

![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.23.21 PM.png>)

Click the pen icon to edit configuration. Set the `Email/Password` property to true and save.

![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.26.38 PM.png>)



### Connect your Firebase Account with Thunkable

There are two properties that you need to retrieve from Firebase to connect it with Thunkable which are both retrievable from the Firebase console: `API key` and `database URL.`&#x20;

You can add these values to your Project Settings, which you can access by clicking on the gear icon to the left of the Design tab of your project.

![](.gitbook/assets/screen-shot-2021-04-12-at-9.31.31-am.png)

To get these values from your Firebase project, click on the gear icon next to Project Overview and click `Project Settings`.

![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.29.17 PM.png>)

In the General tab, scroll down to the section called Your Apps.\
You will find your API Key and Database URL in the code snippet provided.

![](.gitbook/assets/fbcon.png)

### (Optional) Modify the email template you send to verify your users' emails

You can modify the default email that is sent to new users in the Templates tab of the Authentication segment of your console.

![](.gitbook/assets/auth.png)

## Using the Sign In Component in your App

Click on the Sign In drawer of blocks to access the Sign In blocks.

![](<.gitbook/assets/sign-in (1).png>)

## Sign up

The first step for users is to Sign Up with their email address and a password. They will be sent an email to verify the address that they provided.&#x20;

![](.gitbook/assets/sign-in-blocks-signup.png)

| Event                           | Description                                                                                                                                                       |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Sign up ( `email`, `password)`) | Signs up a user for a new account. Returns an `error` if sign up is not successful. A common `error` is "The email address is already in use by another account." |

Here is an example of using this block:

![](.gitbook/assets/signup.png)

## Sign in

This block will sign a user in and return their user ID.

![](.gitbook/assets/sign-in-blocks-sign-in.png)

You can use these blocks below to sign a user in:

![](.gitbook/assets/sign-in-example.png)

When the user's email and password have been stored locally, the following blocks can be used to sign the user in with these details automatically.

![](.gitbook/assets/automatic-sign-in.png)

You can also use the User ID as a key for storing user data in the cloud. See the [Cloud Variables video tutorial](variables.md#video-tutorials) for an example of this.

## Sign Out

Signs the user out.

![](.gitbook/assets/sign-in-blocks-sign-out.png)

## Reset Password

Send an email to the specified email address to reset their password

![](.gitbook/assets/sign-in-blocks-reset-password.png)

## Manage User Access

On the Firebase console, navigate to the Users tab under Authentication and you'll find a dashboard where you can reset a user's password, disable and delete their accounts.

![](<.gitbook/assets/Screen Shot 2022-02-16 at 11.43.44 PM.png>)

## See Also

Once you have signed a user in, you can use their user ID as a unique key to store unique user data to the cloud. See the [cloud variables video tutorial](variables.md#cloud-variables) for more information. &#x20;
