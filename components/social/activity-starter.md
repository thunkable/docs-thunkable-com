#### **Thunkable for Android **❤

# Activity Starter ![](/assets/activity-starter-icon.png)

---

The Activity Starter component lets you combine applications by having one application start up other applications.

To start an application with the Activity Starter, you must supply certain control information to the Android operating system. You do this by setting various properties of Activity Starter before calling the ActivityStarter.StartActivity method.This section gives some examples.

The sample app uses the Activity Starter to open the Facebook and Instagram app if it's installed on a user's device

---

#### Open a deep link to an installed app

The Activity Starter can only open another app if it's installed on a user's device 

|  | Action | Activity Class | DataURI | DataURI Example |
| :--- | :--- | :--- | :--- | :--- |
| Email \(default\) | android.intent.action.VIEW |  |  |  |
| Facebook | android.intent.action.VIEW |  | fb://facewebmodal/f?href={weburl} | fb://facewebmodal/f?href=https://www.facebook.com/newmarketgoods |
| Instagram | android.intent.action.VIEW |  |  |  |
| YouTube | android.intent.action.VIEW |  | vnd.youtube:{youtubeuri} |  |

---

#### Open Facebook page in app if available, website if not

![](/assets/activity-starter-blocks-1.png)



