---
description: >-
  The Data Sources blocks allow you work with the information that you have
  stored in your connected Airtable Bases, Google Sheets or Local Tables.
---

# Data Sources

The Data Sources blocks allow you to perform a variety of CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) operations on records that you have stored in Airtable, Google Sheets or Local Tables.

## Add a Data Source to your App

To access the Data Sources blocks you need to add a Data Source to your app. There are two ways to do this:

* Add a [Data Viewer List](data-viewer-list.md) or a [Data Viewer Grid](data-viewer-grid.md) to your project
* Click on the ⊕ icon in the Data Sources section of your component tree:

![](.gitbook/assets/screen-shot-2021-03-26-at-2.46.24-pm.png)

In the modal that appears, you can choose a previously connected Data Source, or add a new Data Source.&#x20;

### Adding a New Data Source

When adding a new Data Source, you can choose a source of your data:

* [Create your own table](data-sources.md#create-your-own-table)
* [Airtable](data-sources.md#airtable)
* [Google Sheets](data-sources.md#google-sheets)
* [Webflow](data-sources.md#webflow)

![](<.gitbook/assets/Screen Shot 2021-11-05 at 9.30.56 AM.png>)



### Create your Own Table

{% embed url="https://youtu.be/2x52CJQsc9M" %}

Start by naming your data source.

![](.gitbook/assets/name\_local\_data2.png)

You can now see this Data Source from your Data Sources section.\
Click on the pen to rename the Data Source. \
Click on the Data Source name to edit the data.

![](<.gitbook/assets/Screen Shot 2022-02-04 at 12.14.36 PM.png>)

The data editor allows you to edit, add, and delete columns of information. To change any of the individual values simply click on the cell and type whatever you like.&#x20;

![](.gitbook/assets/edit\_table2.png)

### Airtable&#x20;

{% embed url="https://youtu.be/izoH3t0y2hQ" %}

In Airtable, a base in considered to be the data source. Adding an [Airtable](https://www.airtable.com/) database is simple.&#x20;

To start, copy your API key from your Airtable account page. An Airtable API key is a 14 character code that begins with the three letters "key". Paste this key into Thunkable and click the `Refresh` button to see a list of your Airtable bases.&#x20;

Choose the base you want to use as your data source and click `Create`.

![](.gitbook/assets/airtable\_setup.png)

### Google Sheets

{% embed url="https://youtu.be/0YsorQtDsvc" %}

In Google Sheets, the entire document is considered to be the data source.

In order to use a Google Sheet as a data source, the first row in your Sheet must be a **header** row.

Your Google Sheet must be [sharable](https://support.google.com/docs/answer/2494822?hl=en\&co=GENIE.Platform%3DDesktop) for Thunkable to access its data.&#x20;

To connect a Google Sheet, sign in and grant permission for your Thunkable project to access your Google Drive.

![](.gitbook/assets/sign-in.png)

{% hint style="warning" %}
Some users have reported issues connecting to Google Sheets if they are using G Suite for Education accounts. You may need to contact your G Suite administrator to review your security settings.&#x20;
{% endhint %}

Once you have allowed this, you will see a list of spreadsheets in your Google Drive. If you don't see the sheet you are looking for you can switch to list view, sort alphabetically or search for the one you need. Click `Select` to return to your Thunkable project.

![](.gitbook/assets/select-a-file.png)

At this time, connecting to **.xlsx** files that are hosted on Google Sheets is not supported. You can convert your .xlsx file to a Google Sheet before connecting it to your Thunkable app project. Simply open your .xlsx file on Google Sheets, then click **File > Save as Google Sheets**.

![](.gitbook/assets/screen-shot-2020-09-21-at-11.37.46-am.png)

{% hint style="info" %}
Looking to reset your Google Sheets connection? [Click here](troubleshooting/#how-can-i-reset-my-google-sheets-connection-in-thunkable) for instructions
{% endhint %}

### Webflow

{% embed url="https://www.youtube.com/watch?v=4WLOPIP_WuY/?1" %}

When using Weblow as the data source for your Thunkable app, you’ll connect to a Webflow CMS or Content Management System collection.&#x20;

To connect your Webflow CMS to your Thunkable project, you have two options:

* API Key
* OAuth

#### Connecting by API Key

Within the Webflow platform:

1. Navigate to your site settings.
2. Click the Integrations tab
3. Under the **API access** header, click Generate API token.&#x20;
4. Copy the Webflow API token.

Within the Thunkable platform:

![](<.gitbook/assets/data sources - webflow - API Key.png>)

1. Paste the copied Webflow API token into the corresponding field.&#x20;
2. Click **Refresh** to see your Webflow sites.&#x20;
3. Select the site you want to use as your data source.
4. Click Create.&#x20;

{% hint style="info" %}
To protect the quality of its service, the Webflow CMS API default rate limit is 60 requests/minute.  Exceeding this limit will result in an error on the Thunkable platform, so please keep this in mind as you build your app.
{% endhint %}

#### Connecting by OAuth

![](<.gitbook/assets/data sources - webflow - OAuth.png>)

1. Click **Connect to Webflow**.
2. A Webflow authorization screen opens.
3. Select the sites or Workspaces you want to authorize access to.
4.  Click **Authorize app**.\


    <figure><img src=".gitbook/assets/data sources - webflow - authorize.png" alt=""><figcaption></figcaption></figure>

## Data Source blocks

![](.gitbook/assets/data\_sources\_drawer.png)

### Create&#x20;

{% embed url="https://youtu.be/mxyjQRv4aDg" %}

The `create row in`block allows you to append new rows to the end of your data tables.&#x20;

![](.gitbook/assets/create\_row.png)

The inputs are dynamic so if you change the name of Column 1 or Column 2 in the designer these changes will be reflected in the block too.

![](.gitbook/assets/edit\_table2.png)

### Read&#x20;

{% embed url="https://youtu.be/kXex673U2Aw" %}

The `get value from` blocks allows you get read one value from a specific cell in your data table. You can specify the column name in the block itself and pass the unique row id as an input.&#x20;

Note that each row has its own unique 24 character ID. You must use this ID to refer to rows of your Airtable and Local data sources in the blocks below.

If your data source is a **Google Sheet**, you can refer to the row by its integer position (1 for the first row, 2 for the second row, etc.)

![](.gitbook/assets/get\_value.png)

`Get row object` will return the row object of the specified row ID. The row object can be used with [Objects blocks.](objects.md)

![](.gitbook/assets/darasourcesgetrowobject.png)

The `list of values in` block allows you to read an entire column of data from a table and returns it as a list that you can then manipulate with the built-in [List blocks](lists.md).

![](.gitbook/assets/list\_of\_values.png)

The `number of rows in` block returns an integer corresponding to how many rows are in a given table.

![](.gitbook/assets/number\_of\_rows.png)

### Update&#x20;

{% embed url="https://youtu.be/ZvaW8YON2oU" %}

You can use the `update value in` block to modify or update an existing cell in your data table. The column name is specified in the block itself. Both the **row id** and new **value** are passed as inputs.&#x20;

![](.gitbook/assets/update\_value.png)



### Delete

#### Delete Row

You can use the `Delete Row` block to delete a row of data from your Data source. \
The `row id` is passed as an input.\
If there is an `error`, the error message is passed as an output.&#x20;

![](.gitbook/assets/deleterow.png)

#### Delete All Rows

You can use the `delete all rows` block to delete all rows in your data source.\
If there is an `error`, the error message is passed as an output.

![](.gitbook/assets/datasourcedeleteallrows.png)
