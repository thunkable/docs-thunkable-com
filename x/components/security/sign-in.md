#### T**hunkable Cross-Platform **✕

# Sign In ![](/assets/iOSviewIconFirebaseDB.png) powered by Firebase

---

The Sign In component requires email and password authentication to providing additional security for an app and its contents.

`IMPORTANT To use Sign In, you will need to first create your own Firebase account and project`

* [Set up](#set-up)
* [Basic sign in](#basic-sign-in-)
* [Manage user access](#managing-user-access)

---

### Set up

#### Step ① / Create your free [Firebase](https://firebase.google.com/) account and create a new project

#### ![](/assets/firebase-✕-fig-6.png)

#### Step ② / Enable Email / Password sign in

In the Firebase console, navigate to Authentication and the tab "Sign-In Method".  Enable Email/Password as shown below.

![](/assets/firebase-✕-fig-4.png)

#### Step ③ / Connect your Firebase account with Thunkable

There are two properties that you need to retrieve from Firebase to connect it with Thunkable which are both retrievable from the Firebase console: `API key` and `database URL`

`API key` and `database URL`

![](/assets/firebase-✕-fig-2.png)![](/assets/firebase-✕-fig-3.png)

#### \(Optional\) Modify the email template you send to verify your users' emails

![](/assets/firebase-✕-fig-5.png)

---

### Basic sign in

#### Sign Up, Sign In, Sign out, Reset Password

| Event | Description |
| :--- | :--- |
| Sign up \( `email`, `password)`\) | Signs up a user for a new account. Returns an `error` if sign up is not successful. A common `error` is "The email address is already in use by another account." |
| Sign in \( `email`, `password`\) | Signs in an existing user. Returns an `error` if sign in is not successful, either because the email is not registered or the password is incorrect. You can also use the `isEmailVerified`output to limit user to sign in only if they have verified their email |
| Sign out \( `email`\) | Signs out a user from an account, usually to sign in with a different account |
| Reset password \( `email`\) |  |

---

### 

### Manage user access

On the Firebase console, navigate to the Users tab under Authentication and you'll find a dashboard where you can reset a user's password, disable and delete their accounts.

![](/assets/firebase-✕-fig-1.png)

### 



