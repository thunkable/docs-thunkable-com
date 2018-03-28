#### **Thunkable for iOS **

# Sign In ![](blob:https://www.gitbook.com/4da21b52-8ab1-4fb5-90a3-f43c0860d6c8) powered by Firebase

---

The Sign In component supports email and password for any app where a developer wants users to sign in to an app before proceeding further.

IMPORTANT To use Sign In, you'll need to first create your own Firebase account and project

* [Set up](#set-up)
* [Basic sign up / sign in](#basic-sign-up--sign-in-)
* [Sign up / sign in with persistent login](#sign-up--sign-in-with-persistent-login)

![](/assets/sign-in-firebase-fig-1.png)

---

### Set up

#### Step ① / Create an account with [Firebase](https://firebase.google.com/) for free \(you can upgrade to a paid plan later\)

#### Step ② / After creating your project, retrieve the API key and database URL for your project from the Firebase console.  One way to retrieve those values is illustrated below.

#### ![](/assets/firebase-ios-fig-3.png)![](/assets/firebase-ios-fig-4.png)

#### Step ③ / On Thunkable, you can simply copy the API key and database URL into App Settings \(which you can find by clicking on your project app icon on the top left. ![](/assets/firebase-ios-fig-5.png)

#### Step ④ / On Firebase, navigate the Authentication section and the "Sign In method" tab and "Enable" Email/Password sign in. ![](/assets/firebase-ios-fig-8.png)

#### In the "Templates" tab, you can edit the template you send to verify emails from your app users.

![](/assets/firebase-ios-fig-9.png)

#### In the "Users" tab, you can disable or delete a user's account as well as reset their password.

![](/assets/firebase-ios-fig-10.png)

---

### Basic sign up / sign in![](/assets/sign-in-firebase-fig-2.png)

---

### Sign up / sign In with persistent login

#### Persistent login is the simple idea that you save a user's email and password from the last session in local storage on their device so they don't have to type it in again ![](/assets/sign-in-firebase-fig-3.png)

#### Sign Up, Sign In, Sign out, Reset Password

| Event | Description |
| :--- | :--- |
| Sign up \( `email`, `password)`\) | Signs up a user for a new account. Returns an `error` if sign up is not successful. A common `error` is "The email address is already in use by another account." |
| Sign in \( `email`, `password`\) | Signs in an existing user. Returns an `error` if sign in is not successful, either because the email is not registered or the password is incorrect. You can also use the `isEmailVerified`output to limit user to sign in only if they have verified their email |
| Sign out \( `email`\) | Signs out a user from an account, usually to sign in with a different account |
| Reset password \( `email`\) | Resets a user's password and asks users for a new password via email |



