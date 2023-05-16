# Get Products Info

<details>

<summary>Learn more about the data this block returns</summary>

The following is an example of the formatting for data you can expect from the green data blocks

```javascript
[{
"type":0,
"priceAmountMicros": 4990000,
"title":"This is a purchase",
"productId": "one_time_purchase",
"description": "Purchase this once, remove ads forever",
"priceCurrencyCode": "USD",
"price":"$4.99",
"subscriptionPeriod":"P0D"
}]


```

Note on item type:&#x20;

* Note that this is not very accurate on iOS as this data is only available on iOS 11.2 and higher and non-renewable subscriptions always return IAPItemType.PURCHASE.

<!---->

* IAP Item Type's PURCHASE - One time purchase or consumable. IAPItemType.PURCHASE ＝ 0

<!---->

* SUBSCRIPTION - Subscription. IAPItemType.SUBSCRIPTION ＝ 1

None on priceAmountMicros&#x20;

* The price in micro-units, where 1,000,000 micro-units equal one unit of the currency. Use this for calculations.

Note on subscription period&#x20;

* The length of a subscription period specified in ISO 8601 format.&#x20;
  * In-app purchases return P0D.&#x20;
  * On iOS, non-renewable subscriptions also return P0D.&#x20;
  * Examples:&#x20;
    * P0D - in-app purchase or (0 day subscription length)&#x20;
    * P6W - 6 weeks&#x20;
    * P3M - 3 months&#x20;
    * P1Y - 1 Year

</details>

This block will allow you to list the items that you have included in the app for sale. In order to use this block properly, your apps IAP component should always have an up-to-date IAP list of items and subscriptions.&#x20;

<div align="left">

<figure><img src="../.gitbook/assets/product info.png" alt=""><figcaption></figcaption></figure>

</div>
