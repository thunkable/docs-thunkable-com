# Bluetooth Low Energy

## Description

Bluetooth Low Energy, or BLE, is used to wirelessly connect two devices to one another. The BLE component allows you to find and connect to BLE devices and to communicate directly with them.

{% hint style="info" %}
BLE functionality can't be tested with the [Thunkable Live](https://docs.thunkable.com/get-started/live-test) app on iOS. \
To test the BLE functionality in your app on iOS, please [download](https://docs.thunkable.com/download#download-and-install-ios-app) your app.
{% endhint %}

## Blocks

### Scan

This function is used to scan for nearby BLE or Bluetooth enabled devices. Scanning happens for 10 seconds. Once scanning has successfully completed then a list of the available device ids and a list of available names will be returned. If the scanning function can not be completed then an error will be returned.

![](.gitbook/assets/bluetooth\_scan.png)

| Parameter    | Type   | Description                                              |
| ------------ | ------ | -------------------------------------------------------- |
| Device Ids   | List   | **Returns** a list of the IDs of the available devices   |
| Device Names | List   | **Returns** a list of the names of the available devices |
| error        | String | **Returns** an error message from the function           |

### Connect to Device Id

The `Connect to Device Id` function allows your app to connect to a BLE enabled device based in the Id of that device.

![](.gitbook/assets/bluetooth\_connecttodeviceid.png)

| Parameter   | Type   | Description                                                         |
| ----------- | ------ | ------------------------------------------------------------------- |
| Device Id   | String | **Expects** a text string with the device id you want to connect to |
| Device Name | String | **Returns** the name of the device you have just connected to       |
| error       | String | **Returns** an error message from the function                      |

### Connect to Device Name

When you know the name of the BLE device that you want to connect to you can use the `Connect to Device Name` block to connect directly to it. Please note that device names are not unique and it is relatively easy to change the name of a BLE device.

![](.gitbook/assets/bluetooth\_connecttodevicename.png)

| Parameter   | Type   | Description                                                        |
| ----------- | ------ | ------------------------------------------------------------------ |
| Device Name | String | **Expects** a text block with the name of the device to connect to |
| Device Id   | String | **Returns** the Id of the device that you have just connected to   |
| error       | String | **Returns** an error message from the function                     |

### Receive

If you have a BLE device that is capable of sending data to another device then you will need to use the `Receive` function in your app in order to listen to, or receive, data coming from the BLE device.

You need to be connected to another Bluetooth device in order to use this block.

You can receive a **String** or a **Byte Array**.

![](.gitbook/assets/bluetooth\_receive.png)

| Parameter           | Type   | Description                                                                               |
| ------------------- | ------ | ----------------------------------------------------------------------------------------- |
| characteristic UUID | String | **Expects** a text block with a 32-bit UUID for the BLE type, service or profile required |
| data                | String | **Returns **a string containing the information received from the BLE device              |
| error               | String | **Returns** an error message from the function                                            |

### Transmit

Should you need to send data to a BLE device then you can use the `Transmit` function to send that information.&#x20;

You need to be connected to another Bluetooth device in order to use this block.

You can transmit a **String** or a **Byte Array**.\


![](.gitbook/assets/bluetooth\_transmit.png)

| Parameter           | Type   | Description                                                                               |
| ------------------- | ------ | ----------------------------------------------------------------------------------------- |
| characteristic UUID | String | **Expects** a text block with a 32-bit UUID for the BLE type, service or profile required |
| data                | String | **Expects** a text block with the message that you want to send to your BLE device        |
| error               | String | **Returns** an error message from the function                                            |
