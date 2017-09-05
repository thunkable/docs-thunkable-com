| `AdMob is only available on our `[`Thunkable for Android beta platform`](http://beta.thunkable.com/)`, our platform for testing out new features on the Thunkable platform. For AdMob, Thunkable also reserves the right to charge a maintenance fee of 5% of the ad revenue generated for use of the AdMob component. IMPORTANT: Thunkable does not guarantee that features on this platform will always remain available and that apps built on beta will always be supported` |
| :--- |


#### **Thunkable for Android **❤

# AdMob ![](/assets/admob-icon.png)

---

The AdMob components tap into one of the largest mobile ad networks currently available to help app developers maximize revenue from their apps. We have a [section on our community forum](https://community.thunkable.com/c/professional/admob) dedicated to helping users use this component effectively.

* [Set up](#set-up)
* [Loading an Ad](#loading-an-ad)
* [Troubleshooting](#troubleshooting)

**Important**: We recommend that app developers audience first before implementing ads both because it takes away from the user experience and without a sufficient audience, you won't generate much revenue anyway. Google will also refund advertisers and debit developers if there are too many accidental or fraudulent clicks and even disable an ad or an account where it detects there are.

AdMob offers two types of ads:

| Interstitial | Banner |
| :--- | :--- |
| ![](/assets/admob-fig-1.png) | ![](/assets/admob-fig-2.png) |
| Full screen | 320 x 50 fixed ratio |
| Best suited for apps with linear user experiences with clear starts and stops.  For a gaming app, a good time for an interstitial is after a level is complete.  For a non-gaming app, interstitials may be effective after a number of actions have been completed | Works well with most apps but avoid placing in the middle of screen esp in between interactive content as this may reduce the likelihood of users to engage with the ad or lead to accidental clicks |

---

#### Set up

There is a bit of set-up required to start making money with AdMob.  The step that usually confuses users is the waiting period between when an account is created and when ads are ready to go live, which sometimes may take a day.

1. [Go to AdMob](https://www.google.com/admob/) and create an account 
2. Add an existing app on Google Play or one that is not yet published ![](/assets/admob-fig-3.png)![](/assets/admob-fig-4.png)![](/assets/admob-fig-5.png)![](/assets/admob-fig-6.png)
3. Create an ad unit and find your Ad Unit ID to copy into Thunkable  ![](/assets/admob-fig-7.png)![](/assets/admob-fig-8.png)![](/assets/admob-fig-9.png)
4. Go to the beta Set the Screen Size on Thunkable Screen1 to 'Responsive' ![](/assets/admob-fig-10.png)
5. Import your existing project \(.aia\) onto the Beta platform ![](/assets/admob-fig-11.png)
6. \(Optional\) If you are updating an app already uploaded to the Google Play Store, you will have to 'Export keystore' from your current app and 'Import keystore' into your new app

---

#### Loading an Ad

Loads your AdMob banner ad after the user has been in your app for 20 seconds.  You can adjust the timer to vary the time before the ad loads but it may actually be both better for the user experience and for your earnings to wait a little bit of time before you trigger the ads to prevent app users from bouncing too quickly

![](/assets/admob-blocks-1.png)

| Property / Event | Description |
| :--- | :--- |
| Ad unit ID | ID retrieved from your AdMob account \(see set-up above\) after you create a new ad unit and select ad format |
| Test mode | If 'true', ad clicks will not count. We recommend that you select 'true' when testing and then set to 'false' when you publish your app live |
| Load Ad | Loads the ad |
| Visible | If 'true', ad will be visible on the screen |

---

#### Troubleshooting

Common issues

* Ads are not showing up
  * AdMob account created very recently. Usually it takes at least a few hours for the account to be activated
  * For Banner Ads, Screen set to 'Fixed'. Screen needs to be set to 'Responsive'
  * Load Ad block not called in Blocks Editor
  * Account has been suspended by AdMob. Clicking ads on your own app can lead to suspensions as can one or more users repeatedly clicking the ads on your app. Accounts can also be suspended for deceptive ad placement that generates accidental clicks
  * [Check the AdMob forum for more potential errors](https://community.thunkable.com/c/professional/admob)



