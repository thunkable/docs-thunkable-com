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

### List Viewer

| Property                      | Description                                           | Data Type          |
| ----------------------------- | ----------------------------------------------------- | ------------------ |
| Text Items                    | Set text items of List Viewer                         | List of text items |
| Color                         | Set font color of Text Items                          | Color              |
| Background Color (text items) | Set background color for the items in the List Viewer | Color              |
| Font Size                     | Set font size of Text Items                           | Number             |
| Show Arrow                    | Toggle whether arrow is shown beside text items       | True/False         |

### Advanced Properties

| Property                                 | Description                                            | Data Type                           |
| ---------------------------------------- | ------------------------------------------------------ | ----------------------------------- |
| Writing Direction (iOS and web app only) | Set writing direction of text items                    | Select from list `[auto, ltr, rtl]` |
| Background Color (container)             | Set the background color of the List Viewer container. | Color                               |

### Layout

| Property    | Description                                                  | Data Type                                    |
| ----------- | ------------------------------------------------------------ | -------------------------------------------- |
| X           | Set the location of your List Viewer on the X-axis in pixels | Number                                       |
| Y           | Set the location of your List Viewer on the Y-axis in pixels | Number                                       |
| Height      | Set the Height of your List Viewer in pixels                 | Number                                       |
| Width       | Set the Width of your List Viewer in pixels                  | Number                                       |
| Resize Mode | Define dimensions of the list viewer component/container     | Select from list `[Stretch, Float in Place]` |

### Style

| Property       | Description                                                                   | Data Type                                  |
| -------------- | ----------------------------------------------------------------------------- | ------------------------------------------ |
| Visible        | Toggle whether your end users can see the List Viewer                         | True/False                                 |
| Border Style   | Set style of List Viewer's border                                             | Select from list `[solid, dotted, dashed]` |
| Border Color   | Set color of List Viewer's border                                             | Color                                      |
| Border Width   | Set width of List Viewer's border in pixels                                   | Number                                     |
| Border Radius  | Set radius of corners for List Viewer's border in pixels                      | Number                                     |
| Shadow Color   | Color of List Viewer's shadow                                                 | Color                                      |
| Shadow Opacity | Opacity of List Viewer's shadow                                               | Number between 0 and 100                   |
| Shadow Radius  | Radius of corners of List Viewer's shadow in pixels                           | Number                                     |
| Shadow Offset  | How far List Viewer's shadow should be offset, in Height and Width, in pixels | Number                                     |

## Blocks

### Functions

#### When Item Click

![](.gitbook/assets/select\_from\_lv.png)

Performs an action when the user clicks on an item of the List Viewer.

Outputs

| Item  | Text of selected item                             | String |
| ----- | ------------------------------------------------- | ------ |
| Index | Position of item in List Viewer (starting with 1) | Number |

### Properties

Set and get [properties](list-viewer.md#properties) of the List Viewer.

#### Text Items

Set the text items displayed in your List Viewer. Works with [list](lists.md) blocks:

!['set List Viewer's text items' block used with create list block](.gitbook/assets/short\_list.png)

!['set List Viewer's text items' block used with make list from text block](.gitbook/assets/medium\_list.png)

This block also works with blocks to retrieve columns from [Data Sources](data-sources.md):

![Fetching data from a Local Table](.gitbook/assets/local-table.png)

![Getting data from an Airtable Table](.gitbook/assets/airtable\_col.png)

![Reading data from a Google Sheet](<.gitbook/assets/spreadsheet (1).png>)

Choosing Airtable or Google Sheets allows you to create dynamic list viewers. This is where the information displayed to the user changes whenever you change your cloud-based data in Airtable or Google Sheets. Either of these options are ideal for when you need to store thousands of items, or you need to work with items that change frequently.&#x20;

Performs an action when the user clicks on any one of the list items.

#### Text Items Color

![](<.gitbook/assets/text items color.png>)

Set and get font color of the List Viewer's text items.

#### Text Items Background Color

![](.gitbook/assets/lvbg.png)

Set and get background color of the List Viewer's text items.

#### Text Items Font Size

![](.gitbook/assets/lvfs.png)

Set and get font size of the List Viewer's text items.

#### Show Arrow

![](.gitbook/assets/lvsa.png)

Choose whether or not the arrow is displayed next to every item in the list viewer.

#### Height

![](.gitbook/assets/lvh.png)

The `Computed Height`block returns the height of the List Viewer in pixels after it has been rendered on-screen.

#### Width

![](.gitbook/assets/lvw.png)



The `Computed Width`block returns the width of the List Viewer in pixels after it has been rendered on-screen.

#### Visible

![](.gitbook/assets/lvv.png)

Set and get the visibility of the List Viewer.
