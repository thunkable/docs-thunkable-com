---
description: >-
  Connecting your project to a data source allows you to work with the
  information that you have stored in Airtable, Google Sheets, Webflow or a
  local table.
---

# Data Sources

The data sources blocks allow you to perform a variety of CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) operations on records you have stored in Airtable, Google Sheets, Weblow or a local tables.

## Connect Your App to a Data Source

There are two ways to connect your app to a source:

1. Add a Data Viewer (list or grid) to your project. More on Data Viewers is available here: [data-viewers.md](data-viewers.md "mention"), OR
2. Click the Data Sources icon in the menu on the far left and click the ⊕ icon.
3. In the modal that appears, select a previously connected Data Source, or add a new one.&#x20;
4. When connecting to a new data source, select from one of the following options: \
   •  [Create your own table](data-sources.md#create-your-own-table)\
   •  [Airtable](data-sources.md#airtable)\
   •  [Google Sheets](data-sources.md#google-sheets)\
   •  [Webflow](data-sources.md#webflow)

<div align="left">

<img src=".gitbook/assets/Screen Shot 2021-11-05 at 9.30.56 AM.png" alt="" width="563">

</div>

## Create your Own Table

{% embed url="https://youtu.be/2x52CJQsc9M" %}

To create your own table as a data source:

1. Follow the steps above: [Connect Your App to a Data Source](data-sources.md#1.-connect-your-app-to-a-data-source) and select **Create your own table**.
2. Give your local data source table a name.
3. Click **Create**.
4.  To add data to your local table, copy and paste it from another source or click into a cell and type to input the data. \


    <div align="left">

    <figure><img src=".gitbook/assets/data sources - local table - app vs. stored DS (1).png" alt="" width="563"><figcaption></figcaption></figure>

    </div>
5. To modify the table's columns:
   * To **update** the table’s column headers, click their names and typ a new header name.
   * To **add** additional columns, click the **+ New Column** button.
   * To **delete** columns, click the **x** in the column’s title box.
6. To modify the table's rows:
   * To **add** additional rows, with your cursor in the bottom row, press your keyboard’s enter or return key.&#x20;
   * To **delete** a row, right-click on it and select **Remove row**.
7. Select your preferred storage option:
   * **App Data Source** - If the data is changed while the app is open, the table's data resets when a user of your app closes and reopens the app. This reduces the time it takes for the app to load on the user's device.&#x20;
   * **Stored Data Source** - If the data is changed while the app is open, the table's data persists when a user closes and reopens the app.&#x20;
8. When your table is complete, click the **X** in the upper right.
9. The newly created local data source is now listed in your project's list of data sources.
   * Click the pencil icon to **rename** the data source.&#x20;
   * Click the data source's name to review and **edit** the data.
   *   Click the trash can icon to **delete** the data source from your project.\


       <div align="left">

       <img src=".gitbook/assets/Screen Shot 2022-02-04 at 12.14.36 PM.png" alt="" width="375">

       </div>

## Airtable&#x20;

{% embed url="https://youtu.be/izoH3t0y2hQ" %}

When using [Airtable](https://www.airtable.com/) as your data source, a base is connected to Thunkable. To connect your Airtable base to your Thunkable project, you have two options:

* API Key (supported until Jan 31, 2024)
* OAuth

#### Connecting by API Key

1. Navigate to your Airtable account page.
2. Copy your API key (a 14-character code beginning with "key").&#x20;
3. Return to your Thunkable tab.&#x20;
4. Paste the copied Airtable API token into the corresponding field.&#x20;
5. Click **Refresh** to see your Airtable bases.&#x20;
6. Select the base you want to use as your data source.
7. Click **Create**.&#x20;

#### Connecting by OAuth

1. Click **Connect to Airtable**.
2. An Airtable authorization screen opens.
3. Click **+ Add a base**.
4. Select the base you want to authorize access to.
5. Click **Grant access**.
6. Select the correct base from the dropdown menu.
7. Click **Create**.

<div align="left">

<figure><img src=".gitbook/assets/Airtable - DS connection modal.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

#### Use a Custom View&#x20;

In Airtable, a table is similar to a sheet in a spreadsheet. You can have multiple tables within your Airtable base, and each table can have multiple views. A view indicates how the data is presented within the table. For example, you can use views to show only specific fields or records and apply other configurations to manage the information in that view. The initial default view for an Airtable table is the grid view.

When connecting an Airtable base as your Thunkable project’s data source, you can select a custom view instead of the default grid view. This will apply only to the first table in your base. For subsequent tables, Thunkable will use the default grid view. If you have a base with two tables and the second table has a custom view, you can reorder the tables within the base in Airtable so that the custom view is applied to the correct table.

## Google Sheets

{% embed url="https://youtu.be/0YsorQtDsvc" %}

In Google Sheets, the entire document is considered to be the data source.

To use a Google Sheet as a data source the following must be true:

* The first row in your sheet must be a header row and every column must have a header.
* Your Google Sheet must be [sharable](https://support.google.com/docs/answer/2494822?hl=en\&co=GENIE.Platform%3DDesktop) so that Thunkable can access the data.&#x20;

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

## Webflow

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

<div align="left">

<figure><img src=".gitbook/assets/data sources - webflow - API Key.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

1. Paste the copied Webflow API token into the corresponding field.&#x20;
2. Click **Refresh** to see your Webflow sites.&#x20;
3. Select the site you want to use as your data source.
4. Click **Create**.&#x20;

{% hint style="info" %}
To protect the quality of its service, the Webflow CMS API default rate limit is 60 requests/minute.  Exceeding this limit will result in an error on the Thunkable platform, so please keep this in mind as you build your app.
{% endhint %}

#### Connecting by OAuth

<div align="left">

<figure><img src=".gitbook/assets/data sources - webflow - OAuth.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

1. Click **Connect to Webflow**.
2. A Webflow authorization screen opens.
3. Select the sites or Workspaces you want to authorize access to.
4.  Click **Authorize app**.\


    <figure><img src=".gitbook/assets/data sources - webflow - authorize.png" alt=""><figcaption></figcaption></figure>

## Data Sources Blocks

![](<.gitbook/assets/Blocks  App Features  Data Sources.png>)

### Create&#x20;

{% embed url="https://youtu.be/mxyjQRv4aDg" %}

The `create row in`block allows you to append new rows to the end of your data tables.&#x20;

![](.gitbook/assets/create\_row.png)

The inputs are dynamic so if you change the name of Column 1 or Column 2 in the designer these changes will be reflected in the block too.

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

{% embed url="https://youtu.be/Ab66agEf3ok" %}

#### Delete Row

You can use the `Delete Row` block to delete a row of data from your Data source. \
The `row id` is passed as an input.\
If there is an `error`, the error message is passed as an output.&#x20;

![](.gitbook/assets/deleterow.png)

#### Delete All Rows

You can use the `delete all rows` block to delete all rows in your data source.\
If there is an `error`, the error message is passed as an output.

![](.gitbook/assets/datasourcedeleteallrows.png)

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://form.asana.com/?k=UQqJPrAV\_0n0bK6mskl2SA\&d=114052394876887). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
