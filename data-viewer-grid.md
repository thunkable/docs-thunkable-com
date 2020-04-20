---
description: >-
  Create powerful, no-code, data-driven apps connected directly to Google
  Sheets, Airtable, or stored locally.
---

# Data Viewer Grid

{% hint style="info" %}
This component is currently in beta. To sign up to test the Data Viewer please follow [these instructions](https://community.thunkable.com/t/what-are-data-sources/469342?u=domhnallohanlon).
{% endhint %}

## Overview

The data viewer components allow you to create beautiful user interfaces for your data. All of this is done in just 3 steps, no blocks required!

1. Pick your Data Source
2. Choose your Item Layout
3. Set your Data Bindings

## Data Source

When setting up the Data Viewer, you need to specify the source of your data. You can choose to connect to cloud-based data such as Google Sheets or Airtable, or you can create your own table if you want offline access to your data.

![](.gitbook/assets/create_data_source.png)

### Create your own Table

Start by naming your data source.

![](.gitbook/assets/name_local_data.png)

The next thing to do is edit the placeholder data that is automatically generated. Select the Data Viewer component and click on the link that says `Click here to edit the data` 

![](.gitbook/assets/edit_data.png)

### Airtable 

In Airtable, a base in considered to be the data source. Adding an [Airtable](spreadsheet.md) is really simple. 

To get started, copy your API key from your [account page](https://airtable.com/account). An Airtable API key is a 14 character code that begins with the three letters "key". Paste this key into Thunkable and hit `Refresh` to see a list of your Airtable bases. 

Choose the one you want to use as your data source and click `Create`.

![](.gitbook/assets/airtable_setup.png)

### Google Sheets

In Google Sheets, the entire document is considered to be the data source.

