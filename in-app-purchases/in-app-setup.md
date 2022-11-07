# In-App Setup

### App Infrastructure Planning

Developers should plan to store purchase information in the app for quick retrieval. Purchases are associated with transaction ID's which are associated with the Apple ID of the phone. These Transaction ID's are used like a receipt to verify purchases or to validate subscription status's. \


We recommend you setup Stored Variables to hold this information locally for now if you are unfamiliar with NodeJS or Javascript programming.&#x20;

The following is an example of saving information related to a Subscription and 1-Time purchase. The expiry time or T/F value is saved along with the corresponding transaction ID.&#x20;

<figure><img src="../.gitbook/assets/Screen Shot 2022-04-05 at 10.48.16 AM.png" alt=""><figcaption></figcaption></figure>

