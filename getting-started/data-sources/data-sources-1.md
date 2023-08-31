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

# Airtable Data Source

## Overview

When a data source powers your app, you can continuously update your app contents without having to republish it. It allows you to build a dynamic app that can create, read, update, and delete data. This doc covers connecting your app to Airtable as the data source.

When using [Airtable](https://www.airtable.com/) as your data source, a base is connected to Thunkable. To connect your Airtable base to your Thunkable project, you have two options:

* API Key (supported until Jan 31, 2024)
* OAuth

## Video Tutorial

### How to Connect Your Thunkable App to an Airtable Data Source

In this tutorial, we’ll connect a Thunkable app to Airtable as a data source and display the data in our app.

{% embed url="https://youtu.be/izoH3t0y2hQ" %}

## Connect Your App to Airtable by API Key

{% hint style="warning" %}
Connecting by API key will be supported until Jan 31, 2024, after which the only option will be connecting by OAuth.
{% endhint %}

1. In Thunkable, click the **data icon** in the left side panel to access your data source library.
2. Click the **plus sign** at the top of the panel.&#x20;
3. You can select from previously added data sources or add a new data source. Click **Create New**.
4. Select **Airtable**.&#x20;
5. Click the **API Key** tab.
6. In a separate browser tab, navigate to your Airtable account page.
7. Copy your API key (a 14-character code beginning with "key").&#x20;
8. Return to your Thunkable tab.&#x20;
9. Paste the copied Airtable API token into the corresponding field.&#x20;
10. Click **Refresh** to see your Airtable bases.&#x20;
11. Select the base you want to use as your data source.
12. Indicate if you'd like to use a custom view. Learn more here: [Use a Custom View](data-sources-1.md#use-a-custom-view).
13. Click **Create**.&#x20;

## Connect Your App to Airtable by OAuth

1. Click **Connect to Airtable**.
2. In Thunkable, click the **data icon** in the left side panel to access your data source library.
3. Click the **plus sign** at the top of the panel.&#x20;
4. You can select from previously added data sources or add a new data source. Click **Create New**.
5. Select **Airtable**.&#x20;
6. Click the **OAuth** tab.
7. An Airtable authorization screen opens.
8. Click **+ Add a base**.
9.  Select the bases you want to authorize access to. \


    {% hint style="info" %}
    Select all the bases you want your Thunkable projects to have access to. This includes any bases you've previously connected by API key, as well as any new bases you want to connect to Thunkable.
    {% endhint %}
10. Click **Grant access**.\


    {% hint style="info" %}
    If you are connecting by OAuth for the sole purpose of migrating your connection from API Key and are not creating a new data source, you are done. The following steps only apply when creating a new data source.&#x20;
    {% endhint %}
11. Select the correct base from the dropdown menu.
12. Indicate if you'd like to use a custom view. Learn more here: [Use a Custom View](data-sources-1.md#use-a-custom-view).
13. Click **Create**.

{% hint style="success" %}
Once you've connected your Airtable account to your Thunkable account via OAuth, API keys are no longer used.
{% endhint %}

### Use a Custom View&#x20;

In Airtable, a table is similar to a sheet in a spreadsheet. You can have multiple tables within your Airtable base, and each table can have multiple views. A view indicates how the data is presented within the table. For example, you can use views to show only specific fields or records and apply other configurations to manage the information in that view. The initial default view for an Airtable table is the grid view.

When connecting an Airtable base as your Thunkable project’s data source, you can select a custom view instead of the default grid view. This will apply only to the first table in your base. For subsequent tables, Thunkable will use the default grid view. If you have a base with two tables and the second table has a custom view, you can reorder the tables within the base in Airtable so that the custom view is applied to the correct table.

## Display the Data in Your App

Once you've connected a data source, you can display the data in your app with a data viewer component. Learn more about data viewer components here:

{% content-ref url="../../app-design/ui-components/data-components/data-viewers/" %}
[data-viewers](../../app-design/ui-components/data-components/data-viewers/)
{% endcontent-ref %}

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
