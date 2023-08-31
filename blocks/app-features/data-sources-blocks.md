---
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

# Data Sources Blocks

## Overview

The data sources blocks allow you to perform a variety of CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) operations on records you have stored in Airtable, Google Sheets, Weblow, or a local table.

![](<../../.gitbook/assets/Blocks  App Features  Data Sources.png>)

## Create Data

### Video Tutorial

#### How to Create Data in a Thunkable Data Source

In this tutorial, we’ll demonstrate how to create data in a connected data source such as Google Sheets, Airtable, Webflow, or a local table.

{% embed url="https://youtu.be/mxyjQRv4aDg" %}

**Template app:**&#x20;

1. Click: [https://x.thunkable.com/projectPage/64668b45dace620c9c533936](https://x.thunkable.com/projectPage/64668b45dace620c9c533936)
2. Click **Copy Project** in the upper right.

**Copy of spreadsheet:** [Google Sheet - Thunkable Employee Directory](https://docs.google.com/spreadsheets/d/1hMdJ1O-uekCi1\_aT4OpWInk\_bS\_pvU3zouqYYXE2sn4/copy)

### Create Row In Block Overview

The **create row in** block allows you to append new rows to the end of your data tables.&#x20;

![](../../.gitbook/assets/create\_row.png)

The inputs are dynamic, so if you change the name of Column 1 or Column 2 in the data source, these changes will also be reflected in the block.

## Read Data

### Video Tutorial

#### **How to Read Data in a Thunkable Data Source**

In this tutorial, we’ll demonstrate how to read data in a connected data source such as Google Sheets, Airtable, Webflow, or a local table.

{% embed url="https://youtu.be/kXex673U2Aw" %}

### Get Value From Block Overview

The **get value from** block allows you to read a value from a specific cell in your data table. You can specify the column name in the block itself and pass the unique row id as an input.&#x20;

![](../../.gitbook/assets/get\_value.png)

Note that each row has its own unique 24 character ID. You must use this ID to refer to rows of your Airtable and Local data sources in the blocks below.

If your data source is a **Google Sheet**, you can refer to the row by its integer position (1 for the first row, 2 for the second row, etc.)

### Get Row Object From Block Overview

The **get row object from** block returns the row object of the specified row ID. The row object can be used with [Objects Blocks.](../blocks/objects.md)

<div align="left">

<img src="../../.gitbook/assets/darasourcesgetrowobject.png" alt="" width="563">

</div>

### List of Value In Block Overview

The **list of values in** block allows you to read an entire column of data from a table and returns it as a list you can then manipulate with the [List Blocks](../blocks/lists.md).

![](../../.gitbook/assets/list\_of\_values.png)

### Number of Rows In Block Overview

The **number of rows in** block returns an integer corresponding to how many rows are in a given data source.

<div align="left">

<img src="../../.gitbook/assets/number_of_rows.png" alt="" width="563">

</div>

## Update Data

### Video Tutorial

#### How to Update Data in a Thunkable Data Source

In this tutorial, we’ll demonstrate how to update data in a connected data source such as Google Sheets, Airtable, Webflow, or a local table.

{% embed url="https://youtu.be/ZvaW8YON2oU" %}

**Template app:**&#x20;

1. Click: [https://x.thunkable.com/projectPage/64668b079fd0bb4094b4f86f](https://x.thunkable.com/projectPage/64668b079fd0bb4094b4f86f)
2. Click **Copy Project** in the upper right.

**Copy of spreadsheet:** [Google Sheet - Thunkable Employee Directory](https://docs.google.com/spreadsheets/d/1hMdJ1O-uekCi1\_aT4OpWInk\_bS\_pvU3zouqYYXE2sn4/copy)

### Update Value In Block Overview

The **update value in** block allows you to modify or update an existing cell in your data source. The column name is specified in the block itself. The **row id** and new **value** are passed as inputs.&#x20;

<div align="left">

<img src="../../.gitbook/assets/update_value.png" alt="" width="563">

</div>

## Delete Data

### Video Tutorial

#### How to Delete Data in a Thunkable Data Source

In this tutorial, we’ll demonstrate how to delete data in a connected data source such as Google Sheets, Airtable, Webflow, or a local table.

{% embed url="https://youtu.be/Ab66agEf3ok" %}

**Template app:**&#x20;

1. Click: [https://x.thunkable.com/projectPage/64668ac3fa089d0fb2b6ec97](https://x.thunkable.com/projectPage/64668ac3fa089d0fb2b6ec97)
2. Click **Copy Project** in the upper right.

**Copy of spreadsheet:** [Google Sheet - Thunkable Employee Directory](https://docs.google.com/spreadsheets/d/1hMdJ1O-uekCi1\_aT4OpWInk\_bS\_pvU3zouqYYXE2sn4/copy)

### Delete Row In Block Overview

The **delete row in** block allows you to delete a row of data from your data source. The row id is passed as an input. If there is an error, the error message is passed as an output.&#x20;

<div align="left">

<img src="../../.gitbook/assets/deleterow.png" alt="" width="563">

</div>

### Delete All Rows In Block Overview

The **delete all rows in** block allows you to delete all rows in your data source. If there is an error, the error message is passed as an output.

<div align="left">

<img src="../../.gitbook/assets/datasourcedeleteallrows.png" alt="" width="375">

</div>

