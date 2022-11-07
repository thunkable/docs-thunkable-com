# Host your Server Side verification code on Firebase

In order to complete the following actions you need to have a few HTTPS callable functions that live in the cloud. These actions will come in handy when you need to validate that a user should or should not have access to certain areas or content within your app. You'll need this to complete the following in-app processes

To be clear: once a purchase has been made, the only way to get an updated status on that purchase is to set up a backend that listens and waits for incoming data from the to the stores OR to directly ping the store and request the information manually. Our current process covers the later, though in the future documentation will be setup such that developers will bee able to ping their own backend Firebase server for subscription/purchase info which is much faster.&#x20;

These steps are necessary when restoring purchases. Per app store polices, all apps that include IAP must also include a way for the user to restore those in app purchases should they ever need to delete/reinstall an app for any reason.&#x20;

* Acknowledge Android Subscriptions
  * if you don't do this step, subscriptions revert within 3 days of the original purchase
* Verify Android Subscriptions
  * useful to ensure that a subscription is still valid.&#x20;
* Verify Android Purchases
  * useful to ensure users did not request refunds/charge backs after they made the original purchase
* Verify iOS Purchases
* Verify iOS Subscriptions
  * useful to ensure that a subscription is still valid. \
