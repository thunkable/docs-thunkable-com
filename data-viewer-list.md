---
description: >-
  Create powerful, no-code, data-driven apps connected directly to Google
  Sheets, Airtable, or stored locally.
---

# Data Viewer List

## Overview

The Data Viewer List lets you connect to a Data Source and view your data as a list.

![Example of a Data viewer List. Data is dummy data from Webflow.](<.gitbook/assets/Screen Shot 2022-02-04 at 12.47.54 PM.png>)

## Properties

### Data Viewer Grid

| Property                      | Description                                                                                                                                        | Data Type                                |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Data Source                   | The [Data Source](data-sources.md#add-a-data-source-to-your-app) your data is to be pulled from                                                    | Reference to chosen data source          |
| Table                         | Table from your Data Source to show data from                                                                                                      | Reference to chosen table in Data Source |
| Layout                        | Format of how your data will be displayed in your app                                                                                              | Select from list                         |
| Bindings                      | Select what items of data from your Data Source to show in which aspects of yoru layout                                                            | Select from lists                        |
| Left Swipe                    | Toggle whether your end user can swipe a list item to the left to view an additional Button. Reveals Left Swipe Button settings if set to `true`   | True/False                               |
| Left Swipe Button Text        | Text of Button visible when user swipes list item to the left                                                                                      | Text                                     |
| Left Swipe Button Text Color  | Text Color of Button visible when user swipes list item to the left                                                                                | Color                                    |
| Left Swipe Background Color   | Background Color of Button visible when user swipes list item to the left                                                                          | Color                                    |
| Right Swipe                   | Toggle whether your end user can swipe a list item to the right to view an additional Button. Reveals Right Swipe Button settings if set to `true` | True/False                               |
| Right Swipe Button Text       | Text of Button visible when user swipes list item to the right                                                                                     | Text                                     |
| Right Swipe Button Text Color | Text Color of Button visible when user swipes list item to the right                                                                               | Color                                    |
| Right Swipe Background Color  | Background Color of Button visible when user swipes list item to the right                                                                         | Color                                    |
| Empty Text                    | Text that will be displayed if there is no data to fill a string in your Data Viewer                                                               | Text                                     |

### Layout

| Property | Description                                                                         | Data Type  |
| -------- | ----------------------------------------------------------------------------------- | ---------- |
| X        | Location of top left corner of component on X-axis, where the left hand side is X=0 | Number     |
| Y        | Location of top left corner of component on Y-axis, where the top side is Y=0       | Number     |
| Height   | Height of component in pixels                                                       | Number     |
| Width    | Width of component in pixels                                                        | Number     |
| Visible  | Toggle whether your end users can see the component                                 | True/False |

## Blocks

### Events

#### Click&#x20;

The Item Click event is fired when any list item in the Data Viewer is clicked. It returns a `row id` which corresponds to the unique Thunkable Id of the item that was clicked. The row id is most useful when used with the the Data Source blocks.

![](.gitbook/assets/item\_click.png)

#### Swipe Click

The left and right swipe click events are fired when these buttons are clicked. Both return a `row id` to quickly identify which row was clicked when using the Data Source blocks

![](.gitbook/assets/left\_swipe.png)

![](.gitbook/assets/right\_swipe.png)

### Functions

#### Refresh

Refresh the Data Viewer List to sync with the Data Source.

![](.gitbook/assets/dvl\_refresh.png)



### Properties

Set and get [properties](data-viewer-list.md#properties) of the Data Viewer List.

#### Computed Height & Width

Get the computed Height and Width of the Data Viewer List as it appears on-screen.

#### Visible

Set and get the Visible property of the Data Viewer List

#### Empty Text

Set and get the Empty Text property of the Data Viewer List

### Data Sources

When you connect a Data Source to your project you will also have access to a second block drawer. These Data Source blocks allow you to perform a variety of CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) operations on your data.&#x20;

Click on the link below to learn how to use the Data Sources blocks in your project.&#x20;

{% content-ref url="data-sources.md" %}
[data-sources.md](data-sources.md)
{% endcontent-ref %}
