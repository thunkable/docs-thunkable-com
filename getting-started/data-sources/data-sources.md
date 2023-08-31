---
description: >-
  Connecting your project to a data source allows you to work with the
  information that you have stored in Airtable, Google Sheets, Webflow or a
  local table.
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Google Sheets Data Source

## Overview

When a data source powers your app, you can continuously update your app contents without having to republish it. It allows you to build a dynamic app that can create, read, update, and delete data. This doc covers connecting your app to Google Sheets as the data source.

In Google Sheets, the entire document is considered to be the data source. To use a Google Sheet as a data source, the following must be true:

* The first row in your sheet must be a header row, and every column must have a header.
* Your Google Sheet must be [sharable](https://support.google.com/docs/answer/2494822?hl=en\&co=GENIE.Platform%3DDesktop) so that Thunkable can access the data.&#x20;

## Video Tutorial

### How to Connect Your Thunkable App to a Google Sheets Data Source

In this tutorial, we’ll connect a Thunkable app to Google Sheets as a data source and display the data in our app.

{% embed url="https://youtu.be/0YsorQtDsvc" %}

## Connect Your App to Google Sheets

1. Click the **data icon** in the left side panel to access your data source library.
2. Click the **plus sign** at the top of the panel.&#x20;
3. You can select from previously added data sources or add a new data source. Click **Create New**.
4. Select **Google Sheets**.&#x20;
5.  Sign in to your Google account and grant permission for your Thunkable accoumt to access your Google Drive.\


    <div align="left">

    <img src="../../.gitbook/assets/sign-in.png" alt="" width="563">

    </div>
6. Click **Select a Sheet.**
7.  Select your spreadsheet.\


    <div align="left">

    <img src="../../.gitbook/assets/select-a-file.png" alt="" width="563">

    </div>
8. Click **Select**.
9. Rename the data source, if you’d like.&#x20;
10. Indicate which row your column headers are in and which row is the first to contain data.
11. Click **Create**.&#x20;

{% hint style="warning" %}
If you are using a G Suite for Education account and experience issues connecting to Google Sheets, contact your G Suite administrator to review your security settings.&#x20;
{% endhint %}

### Display the Data in Your App

Once you've connected a data source, you can display the data in your app with a data viewer component. Learn more about data viewer components here:

{% content-ref url="../../app-design/ui-components/data-components/data-viewers/" %}
[data-viewers](../../app-design/ui-components/data-components/data-viewers/)
{% endcontent-ref %}

### .xlsx Files

Connecting to .xlsx files that are hosted on Google Sheets is not supported, but you can convert your .xlsx file to a Google Sheet before connecting it to your Thunkable app project. To do so:

1. Open the .xlsx file on Google Sheets
2. Click **File**.
3. Select **Save as Google Sheets**.

<div align="left">

<img src="../../.gitbook/assets/screen-shot-2020-09-21-at-11.37.46-am.png" alt="">

</div>

## Reset Your Google Sheets Connection

### Reset from Thunkable

1. Login to your Thunkable account.
2. Click the **My Data Sources** tab on your Projects Page.
3. Click the **trash can icon** to delete the Google Sheets data source.

![](<../../.gitbook/assets/image (216) (1).png>)

### Reset from Google

If you are having difficulties connecting your Google Sheets from Thunkable, you may need to reset your Google Sheets connection.

1. Navigate to [https://myaccount.google.com/security](https://myaccount.google.com/security)
2. Scroll to the **Your connections to third-party apps & services** section.
3. Click the **Thunkable** connection.&#x20;
4.  In the **Thunkable has some access to your Google Account section**, click **See details.**\


    <figure><img src="../../.gitbook/assets/Google Sheets connection.png" alt=""><figcaption></figcaption></figure>
5.  Click **Remove Access**.\


    <figure><img src="../../.gitbook/assets/Google Sheets - remove access.png" alt=""><figcaption></figcaption></figure>
6. Return to Thunkable and re-connect to your Google Sheets account.

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
