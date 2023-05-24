# Purchase Subscription / Purchase One-Time Item

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrMxDvAEx21XNB81zaoj%2Fuploads%2FemFBph2Q1T5n8N9JBcCT%2FScreen%20Shot%202022-04-13%20at%203.37.18%20PM.png?alt=media&#x26;token=497b5644-78bf-43f7-af18-7c8e122e327a" alt=""><figcaption></figcaption></figure>

### Blocks Explained

{% hint style="warning" %}
The green purchase block should be handled as a[ list/array](https://docs.thunkable.com/v/drag-and-drop/lists). The purchase [object](https://docs.thunkable.com/v/drag-and-drop/objects)  is always item # 1 in the list
{% endhint %}

{% hint style="info" %}
Please note that the one-time items and subscription blocks are handled in a similiar manner.&#x20;
{% endhint %}

1. a 'hider' is shown. We recommend you use a 'waiting' modal to indicate to users they should not interact
   1. This could be a Group with a spinning 'loading' icon in an image component.
2. the purchase is initiated
   1. you must pass in a valid [Android](android-play-store-setup.md) or [Apple](ios-app-store-setup.md) item or subscription id to this purple blocks input
3. If an error does occur, the error is passed on to the [Server Log​](host-your-server-side-verification-code-on-firebase/setup-your-cloud-environment/server-logs.md)
4. If the transaction is successful **and** the property purchaseState from object #1 in the (single item list) of purchase objects,
   1. send the purchase for verification ([iOS](ios-app-store-setup.md)) ([Android](android-play-store-setup.md))
   2. **else, send a** [**server log**](host-your-server-side-verification-code-on-firebase/setup-your-cloud-environment/server-logs.md)**​**
5. Hide the hider/waiting modal after verification

​Learn more about the data these blocks return after you created your IAPs, you're ready to start selling them to your users! Using the corresponding `productID` created above, choose the appropriate block (either `Purchase Subscription` or `Purchase One-Time Item`) and connect it to a user action. Purchases should be very straightforward within your app. Make it clear to your users how much they are paying and provide a brief description of the item. You can include more details in your [app store item setup](purchase-subscription-purchase-one-time-item.md). Once you check there wasn't an error, you should [verify](verify-ios-purchases.md) the `purchase` (the green block). If your users are purchasing a subscription on Android, you MUST complete the step of [verification and acknowledgement](verify-and-acknowledge-android-purchases-and-subscription.md) to complete the transaction.\
