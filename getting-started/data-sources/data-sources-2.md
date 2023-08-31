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

# Webflow Data Source

## Overview

When a data source powers your app, you can continuously update your app contents without having to republish it. It allows you to build a dynamic app that can create, read, update, and delete data. This doc covers connecting your app to Webflow as the data source.

When using Weblow as the data source for your Thunkable app, you’ll connect to a Webflow CMS or Content Management System collection. To connect your Webflow CMS to your Thunkable project, you have two options:

* API Key
* OAuth

## Video Tutorial

### How to Connect Your Thunkable App to a Webflow Data Source

In this tutorial, we’ll connect a Thunkable app to Webflow as a data source and display the data in our app.

{% embed url="https://www.youtube.com/watch?v=4WLOPIP_WuY/?1" %}

## Connect Your App to Webflow by API Key

1. In Thunkable, click the **data icon** in the left side panel to access your data source library.
2. Click the **plus sign** at the top of the panel.&#x20;
3. You can select from previously added data sources or add a new data source. Click **Create New**.
4. Select **Webflow**.&#x20;
5. Click the **API Key** tab.
6. In a separate browser tab, navigate to your Webflow site settings.
7. Click the **Integrations** tab.
8. Under the **API access** header, click **Generate API token**.&#x20;
9. Copy the Webflow API token.
10. Return to your Thunkable tab. \


    <div align="left">

    <figure><img src="../../.gitbook/assets/data sources - webflow - API Key.png" alt="" width="375"><figcaption></figcaption></figure>

    </div>
11. Paste the copied Webflow API token into the corresponding field.&#x20;
12. Click **Refresh** to see your Webflow sites.&#x20;
13. Select the site you want to use as your data source.
14. Click **Create**.&#x20;

{% hint style="info" %}
To protect the quality of its service, the Webflow CMS API default rate limit is 60 requests/minute. Exceeding this limit will result in an error on the Thunkable platform, so please keep this in mind as you build your app.
{% endhint %}

## Connect Your App to Webflow by OAuth

1. In Thunkable, click the **data icon** in the left side panel to access your data source library.
2. Click the **plus sign** at the top of the panel.&#x20;
3. You can select from previously added data sources or add a new data source. Click **Create New**.
4. Select **Webflow**.&#x20;
5.  Click the **OAuth** tab.\


    <div align="left">

    <figure><img src="../../.gitbook/assets/data sources - webflow - OAuth.png" alt="" width="375"><figcaption></figcaption></figure>

    </div>
6. Click **Connect to Webflow**.
7. A Webflow authorization screen opens.
8. Select the sites or Workspaces you want to authorize access to.
9.  Click **Authorize app**.\


    <figure><img src="../../.gitbook/assets/data sources - webflow - authorize.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
To protect the quality of its service, the Webflow CMS API default rate limit is 60 requests/minute. Exceeding this limit will result in an error on the Thunkable platform, so please keep this in mind as you build your app.
{% endhint %}

## Display the Data in Your App

Once you've connected a data source, you can display the data in your app with a data viewer component. Learn more about data viewer components here:

{% content-ref url="../../app-design/ui-components/data-components/data-viewers/" %}
[data-viewers](../../app-design/ui-components/data-components/data-viewers/)
{% endcontent-ref %}

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
