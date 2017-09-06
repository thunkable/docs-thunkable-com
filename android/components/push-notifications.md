| \*`Push Notifications are only available on our`[`Thunkable for Android beta platform`](http://beta.thunkable.com/)`, our platform for testing out new features on the Thunkable platform. IMPORTANT: Thunkable does not guarantee that features on this platform will always remain available and that apps built on beta will always be supported` |
| :--- |


#### **Thunkable for Android **❤

# Push Notifications by One Signal ![](/assets/one-signal-icon.png)

---

User retention in apps is hard and push notifications can be a very valuable asset to continue to engage with your app audience after they have downloaded your app.![](/assets/push-fig-4.png)

However, like ads, being overly aggressive can backfire and have a negative effect on your users. Annoying notifications--those that are irrelevant and too frequent--are the number one reason why users uninstall mobile apps.

| App type | Frequency | Content |
| :--- | :--- | :--- |
| E-commerce | Sales | Coupon code |
| Game | App updates | Try this new level |

We recommend limiting push notifications to content that will be welcomed by a large majority of your users. Less is more!

Most of the work you do to use push notifications in your app will be on the One Signal interface. On Thunkable, you simply drag and drop the component in and add the One Signal API key.

* [Set up with One Signal](#set-up-with-one-signal)

* [Connect One Signal with your app](#connecting-one-signal-with-your-app)

* [Create a message](#create-a-message)

* [Add your app icon and title accent color](#add-your-app-icon-and-title-accent-color) \(optional\)

* [Specify the launch url](#specify-the-launch-url-optional) \(optional\)

* [Push immediately or schedule the notification](#push-the-notification)

---

#### Set up with One Signal

One Signal is a free service that supports unlimited devices and notifications

* Go to [One Signal](https://onesignal.com/) and login
* Add a new app
* Generate a [Google Server API key](https://documentation.onesignal.com/docs/generate-a-google-server-api-key) and project number
* Select 'Native Android' as target SDK

---

#### Connecting One Signal with your app

After dragging and dropping the Push Notifications component to your app, go to the App Settings page of your app and copy the One Signal App ID into the properties of the Push Notifications component![](/assets/push-fig-1.png)

| Property | Description |
| :--- | :--- |
| One Signal App ID | Corresponds to the One Signal App ID on the App Settings page of One Signal |

---

#### Create a message on One Signal

![](/assets/push-fig-3.png)

---

#### Add your app icon and title accent color \(optional\)

If you want to use your app icon as your notification icon, you simply enter the letters "ya" into the small icon field

![](/assets/push-fig-5.png)

---

#### Specify the launch url \(optional\)

![](/assets/push-fig-6.png)

---

#### Push immediately or schedule the notification

One Signal allows users to send a push notification immediately or schedule one for later. You can also select their more intelligent timing that optimizes for a user's timezone or most likely to click time.

IMPORTANT: It may take a few minutes for your first push notification to go through

![](/assets/push-fig-7.png)

