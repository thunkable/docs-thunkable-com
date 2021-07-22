---
description: Enable your apps to read barcodes and QR codes
---

# Barcode Scanner

## Barcode Scanner Overview

Barcodes and QR codes can be useful features in many types of apps from social apps like WeChat and Venmo to connect friends together or location-based games like scavenger hunts. The Barcode Scanner component uses the camera to read any barcode or QR code.

![](.gitbook/assets/thunkable-play-store-screenshots-1080-x-1920-17.png)

## Blocks

The Barcode Scanner is among the easiest components to set-up and use. After adding the component to your app, you can connect it with a button and a label like the blocks below.

### Scan

![](.gitbook/assets/screen-shot-2021-04-19-at-10.32.23-am.png)

#### Outputs

| Name | Data Type | Data |
| :--- | :--- | :--- |
| value | text | value from scanned barcode/QR code |
| type | text | `barcode` or `QR code` |
| was cancelled | True/False | If user cancelled action, returns `true`; else returns `false` |
| error | Text | If error, returns error; else returns `null` |

In most cases you'll use the default `back` camera in your mobile device but you also have the option to specify the front camera in certain cases.

![](.gitbook/assets/screen-shot-2019-10-24-at-1.43.37-pm.png)

