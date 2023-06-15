# Get Most Recent Active Purchase

<details>

<summary>Learn more about the data this block returns</summary>

This block will return the users most recent purchase that is still valid/active.

```

//iOS
[{
"purchaseState":3,
"orderId":"20000002342",
"purchaseTime":23434234234
"acknowledged": true,
"productId":"app_store_product_id",
"originalOrderId":"20000002034234", 
"originalPurchaseTime":234234234234, 
"transactionReceipt":"LONG STRING", 
}]


//Android
[{
"packageName": "com.thunkable.testapp",
"productId": "new_sub",
"acknowledged": true,
"purchaseToken":"LONG STRING",
"purchaseState":1,
"orderId":"GPA.2345-2345-2345-23456",
"purchaseTime":234234234234134
}]
```

</details>

