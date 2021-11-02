---
description: >-
  The List Viewer component allows you to add, view and click on items in a
  list.
---

# List Viewer

## List Viewer Overview

![](.gitbook/assets/list-viewer-fig-1.png)

## Properties

You can customize the List Viewer with the following properties:

### Properties

* **Text Items: **set text items of List Viewer&#x20;
* **Text Items Color: **Set color of Text Items font
* **Text Items Background Color: **Set background color for List Viewer
* **Text Items Font Size: **Set font size of Text Items
* **Show Arrow: **To see an arrow beside each item in the list, set the switch to true

### Advanced Properties

* **Writing Direction (iOS and web only):** set writing direction of text items
* **Background Color: **set background color of List Viewer&#x20;

### Layout

* **X: **set the location of your List Viewer on the X-axis in pixels
* **Y: **set the location of your List Viewer on the Y-axis in pixels
* **Height: **set the Height of your List Viewer in pixels
* **Width: **set the Width of your List Viewer in pixels
* **Visible: **To see the text input in your app, set the switch to true

### Style

* **Border Width: **Enter how wide you want the border outline of the List Viewer to be
* **Border Color: **Pick a color for the border of the List Viewer
* **Border Style: **Select if you want the border to be a dotted, dashed or solid line
* **Border Radius: **Enter how round you want the edges of the border for the List Viewer to be

## Blocks

### Set Items of a List Viewer

#### Short Lists

We recommend adding a short [list](lists.md) of items within the app itself as the Screen starts. Although the list block itself can handle a large number of items, practically speaking you probably only want to use this approach if your project has tens of items.

![](.gitbook/assets/short\_list.png)

#### Medium Lists

If you need longer lists of information in your app you can use delimited data. This is very similar to using something like a .csv file. You can have hundreds of items in your list viewer using this method.&#x20;

![](.gitbook/assets/medium\_list.png)

#### Long Lists

For longer lists where you need hundreds or thousands of items in your list, we recommend using the [Data Sources](data-sources.md) component. This gives you three different options for storing your data.&#x20;

1. Local Table
2. Airtable
3. Google Sheets

![Fetching data from a Local Table](.gitbook/assets/local-table.png)

![Getting data from an Airtable Table](.gitbook/assets/airtable\_col.png)

![Reading data from a Google Sheet](<.gitbook/assets/spreadsheet (1).png>)

Choosing Airtable or Google Sheets allows you to create dynamic list viewers. This is where the information displayed to the user changes whenever you change your cloud-based data in Airtable or Google Sheets. Either of these options are ideal for when you need to store thousands of items, or you need to work with items that change frequently.&#x20;

| Property   | Description                                    |
| ---------- | ---------------------------------------------- |
| Text Items | Default (`none`); items must be in list format |

### When Item Click

![](.gitbook/assets/select\_from\_lv.png)

Performs an action when the user clicks on any one of the list items.

#### Outputs

| Name  | Data Type | Description                                       |
| ----- | --------- | ------------------------------------------------- |
| Item  | String    | Text of selected item                             |
| Index | Number    | Position of item in List Viewer (starting with 1) |

### Properties

#### Height

![](<.gitbook/assets/height (3).png>)

The set and get height blocks work with the Height property of the list viewer component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

The `Computed Height`block returns the on-screen dimensions of the list viewer, after it has been rendered on-screen. The value returned is an integer, representing the size of the list viewer in pixels.

#### Show Arrow

![](.gitbook/assets/show\_arrow.png)

Choose whether or not the arrow is displayed next to every item in the list viewer.

#### Text Items

![](.gitbook/assets/text\_items.png)

Set or get the list of text items that are displayed in the List Viewer. You must use a [list](lists.md) of data here - either locally stored or stored in the cloud.

#### Visible

![](<.gitbook/assets/visible (5).png>)



The set and get visible blocks are used to show or hide the entire list viewer component. Acceptable values are:

* True
* False

#### Width

![](<.gitbook/assets/width (4).png>)

The `Computed Width`block returns the on-screen dimensions of the list viewer, after it has been rendered on-screen. The value returned is an integer, representing the size of the list viewer in pixels.

The list viewer doesn't currently support pixel or percentage values for the `width` property.
