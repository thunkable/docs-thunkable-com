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

# Local Table Data Source

## Overview

When a data source powers your app, you can continuously update your app contents without having to republish it. It allows you to build a dynamic app that can create, read, update, and delete data. This doc covers creating a local table as the data source.

## Video Tutorial

### How to Create a Local Table Data Source in Your Thunkable App

In this tutorial, we’ll create a local table data source in a Thunkable app and display the data.

{% embed url="https://youtu.be/2x52CJQsc9M" %}

## Create a Local Data Source

To create your own table as a data source:

1. Click the **data icon** in the left side panel to access your data source library.
2. Click the **plus sign** at the top of the panel.&#x20;
3. You can select from previously added data sources or add a new data source. Click **Create New**.
4. Select **Create your own table**.
5. Give your local data source table a name.
6. Click **Create**.
7. To add data to your local table, copy and paste it from another source or click into a cell and type to input the data.&#x20;
8. To modify the table's columns:
   * To **update** the table’s column headers, click their names and type a new header name.
   * To **add** additional columns, click the **+ New Column** button.
   * To **delete** columns, click the **x** in the column’s title box.
9. To modify the table's rows:
   * To **add** additional rows, with your cursor in the bottom row, press your keyboard’s enter or return key.&#x20;
   * To **delete** a row, right-click on it and select **Remove row**.
10. Select your preferred storage option:
    * **App Data Source** - If the data is changed while the app is open, the table's data resets when a user of your app closes and reopens the app. This reduces the time it takes for the app to load on the user's device.&#x20;
    *   **Stored Data Source** - If the data is changed while the app is open, the table's data persists when a user closes and reopens the app. \


        <div align="left">

        <figure><img src="../../.gitbook/assets/data sources - local table - app vs. stored DS (1).png" alt="" width="563"><figcaption></figcaption></figure>

        </div>
11. When your table is complete, click the **X** in the upper right.
12. The newly created local data source is now listed in your project's list of data sources.
    * Click the pencil icon to **rename** the data source.&#x20;
    * Click the data source's name to review and **edit** the data.
    *   Click the trash can icon to **delete** the data source from your project.\


        <div align="left">

        <img src="../../.gitbook/assets/Screen Shot 2022-02-04 at 12.14.36 PM.png" alt="" width="375">

        </div>

## Display the Data in Your App

Once you've connected a data source, you can display the data in your app with a data viewer component. Learn more about data viewer components here:

{% content-ref url="../../app-design/ui-components/data-components/data-viewers/" %}
[data-viewers](../../app-design/ui-components/data-components/data-viewers/)
{% endcontent-ref %}



{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
