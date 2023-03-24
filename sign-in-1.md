# Email Sign In by Firebase

* [Set up](sign-in-1.md#set-up)
* [Basic sign in](sign-in-1.md#basic-sign-in-)
* [Manage user access](sign-in-1.md#managing-user-access)

{% hint style="info" %}
To use Sign In, you will need to first create your own Firebase account and project
{% endhint %}

## Set up

### Create your free [Firebase](https://firebase.google.com/) account and create a new project

![](.gitbook/assets/thunkable-documentation-exhibits-70%20%281%29.png)

### Enable Email / Password sign in

In the Firebase console, navigate to Authentication and the tab "Sign-In Method". Enable Email/Password as shown below.

![](.gitbook/assets/firebase-fig-4%20%281%29.png)

### Connect your Firebase account with Thunkable

There are two properties that you need to retrieve from Firebase to connect it with Thunkable which are both retrievable from the Firebase console: `API key` and `database URL`

![](.gitbook/assets/thunkable-documentation-exhibits-67.png)

`API key` and `database URL`

![](.gitbook/assets/thunkable-documentation-exhibits-68%20%281%29.png)

![](.gitbook/assets/thunkable-documentation-exhibits-69.png)

### \(Optional\) Modify the email template you send to verify your users' emails

![](.gitbook/assets/firebase-fig-5.png)

## Sign up

The first step for users is to Sign Up with their email address and a password. They will be sent an email to verify the address that they provided. A sample block that also saves login credentials locally with [stored variables](https://docs.thunkable.com/variables#app-stored-and-cloud-variables) is provided below:

![](.gitbook/assets/docs_signup.png)

| Event | Description |
| :--- | :--- |
| Sign up \( `email`, `password)`\) | Signs up a user for a new account. Returns an `error` if sign up is not successful. A common `error` is "The email address is already in use by another account." |

## Sign in

Users who sign up will be sent an email to verify the email address they provided is valid. You can use the blocks below to check whether they have verified their email before they can proceed further

![](.gitbook/assets/signin.png)

When the user's email and password have been stored locally, the following blocks can be used to sign the user in with these details automatically.

![](.gitbook/assets/docs_signin_saved.png)

| Event | Description |
| :--- | :--- |
| Sign in \( `email`, `password`\) | Signs in an existing user. Returns an `error` if sign in is not successful, either because the email is not registered or the password is incorrect. You can also use the `isEmailVerified`output to limit user to sign in only if they have verified their email |
| Sign out \( `email`\) | Signs out a user from an account, usually to sign in with a different account |
| Reset password \( `email`\) | Sends an email to a user to reset their password |
|  |  |

## Manage user access

On the Firebase console, navigate to the Users tab under Authentication and you'll find a dashboard where you can reset a user's password, disable and delete their accounts.

![](.gitbook/assets/firebase-fig-1.png)

