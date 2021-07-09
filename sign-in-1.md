# Email Sign In by Firebase

{% hint style="info" %}
To use Sign In, you will need to first create your own Firebase account and project
{% endhint %}

## Getting Started

### Create your free [Firebase](https://firebase.google.com/) account and create a new project

![](.gitbook/assets/thunkable-documentation-exhibits-70%20%281%29.png)

### Enable Email / Password Sign in

In the Firebase console, navigate to Authentication and the tab "Sign-In Method". Enable Email/Password as shown below.

![](.gitbook/assets/firebase-fig-4%20%281%29.png)

### Connect your Firebase Account with Thunkable

There are two properties that you need to retrieve from Firebase to connect it with Thunkable which are both retrievable from the Firebase console: `API key` and `database URL`

![](.gitbook/assets/thunkable-documentation-exhibits-67.png)

`API key` and `database URL`

![](.gitbook/assets/thunkable-documentation-exhibits-68%20%281%29.png)

![](.gitbook/assets/thunkable-documentation-exhibits-69.png)

### \(Optional\) Modify the email template you send to verify your users' emails

![](.gitbook/assets/firebase-fig-5.png)

## Using the Sign In Component in your App

Click on the Sign In drawer of blocks to access the Sign In blocks.

![](.gitbook/assets/sign-in%20%281%29.png)

## Sign up

The first step for users is to Sign Up with their email address and a password. They will be sent an email to verify the address that they provided. 

![](.gitbook/assets/screen-shot-2021-04-19-at-11.53.48-am.png)

| Event | Description |
| :--- | :--- |
| Sign up \( `email`, `password)`\) | Signs up a user for a new account. Returns an `error` if sign up is not successful. A common `error` is "The email address is already in use by another account." |

Here is an example of using this block:

![](.gitbook/assets/screen-shot-2021-04-19-at-11.55.16-am.png)

## Sign in

This block will sign a user in and return their user ID.

![](.gitbook/assets/screen-shot-2021-04-19-at-11.57.04-am.png)

| Name | Data Type | Data |
| :--- | :--- | :--- |
| error | Text | If error, returns error; else, returns `null` |
| userId | Text | Returns unique ID for each account |
| isEmailVerified | True/False | If email has been verified, returns `true`; else, returns `false` |

When the user's email and password have been stored locally, the following blocks can be used to sign the user in with these details automatically.

![](.gitbook/assets/screen-shot-2021-04-19-at-12.01.03-pm.png)

## Sign Out

Signs the user out.

![](.gitbook/assets/screen-shot-2021-04-19-at-12.01.33-pm.png)

## Reset Password

Send an email to the specified email address to reset their password

![](.gitbook/assets/screen-shot-2021-04-19-at-12.02.37-pm.png)

## Manage User Access

On the Firebase console, navigate to the Users tab under Authentication and you'll find a dashboard where you can reset a user's password, disable and delete their accounts.

![](.gitbook/assets/firebase-fig-1.png)

