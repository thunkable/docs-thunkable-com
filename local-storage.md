# Local Storage

## Local Storage Overview

{% hint style="warning" %}
You should now use [stored variables](variables.md#app-stored-and-cloud-variables) instead of adding a Local Storage component. This will work the same way in the background but will save you a lot of blocks. To work with tabular data in your app please use the [local DB](local-db.md) component in your app.
{% endhint %}

* [Save Data](local-storage.md#save-data)
* [Get Data](local-storage.md#get-data)

This storage option is useful for saving simple info on the device, especially helpful for remembering user's setting from a previous session.

## Save Data

To save data locally to your phone, simple name a `key` to store a `value` under. If you have a previous `value` in your `key`, saving it will override that `value`

![](.gitbook/assets/local-storage-fig-1.png)

## Get Data

![](.gitbook/assets/local-storage-fig-2.png)

