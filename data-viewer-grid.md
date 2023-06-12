---
description: >-
  Create powerful, no-code, data-driven apps connected directly to Google
  Sheets, Airtable, or stored locally.
---

# Data Viewer Grid

## Overview

The Data Viewer Grid lets you connect to a Data Source and view your data as a grid. This layout works well with data that includes images.

<div align="left">

<img src=".gitbook/assets/Screen Shot 2022-02-04 at 12.44.53 PM.png" alt="Example of a Data viewer Grid. Data is dummy data from Webflow." width="375">

</div>

## Properties

### Data Viewer Grid

| Property          | Description                                                                                                 | Data Type                                |
| ----------------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Data Source       | The [Data Source](data-sources.md#add-a-data-source-to-your-app) your data is to be pulled from             | Reference to chosen data source          |
| Table             | Table from your Data Source to show data from                                                               | Reference to chosen table in Data Source |
| Grid Appearance   | How your data will be displayed in your app                                                                 | Select from list                         |
| Populate Data     | Select what items of data from your Data Source to show in which aspects of your layout                     | Select from lists                        |
| Horizontal Scroll | Toggle whether your Data Viewer should scroll horizontally (if `false`, Data Viewer will scroll vertically) | True/False                               |
| Empty Text        | Text that will be displayed if there is no data to fill a string in your Data Viewer                        | Text                                     |

### Layout

| Property    | Description                                                                         | Data Type                                    |
| ----------- | ----------------------------------------------------------------------------------- | -------------------------------------------- |
| X           | Location of top left corner of component on X-axis, where the left hand side is X=0 | Number                                       |
| Y           | Location of top left corner of component on Y-axis, where the top side is Y=0       | Number                                       |
| Height      | Height of component in pixels                                                       | Number                                       |
| Width       | Width of component in pixels                                                        | Number                                       |
| Resize Mode | Define dimensions of the Data Viewer Grid component/container                       | Select from list `[Stretch, Float in Place]` |

## Blocks

### Events

The `Item Click` event is fired when any card in the Data Viewer is clicked.&#x20;

Returns a `row id` which corresponds to the unique Thunkable Id of the card that was clicked.&#x20;

The row id is particularly useful when used with the the [Data Source](data-sources.md) blocks.

![](.gitbook/assets/grid\_click.png)

### Functions

#### Refresh

Refresh the Data Viewer Grid to sync with the Data Source.

![](.gitbook/assets/dvg\_refresh.png)

### Properties

Set and get [properties](data-viewer-grid.md#properties) of the Data Viewer Grid.

#### Computed Height & Width

Get the computed Height and Width of the Data Viewer Grid as it appears on-screen.

#### Visible

Set and get the Visible property of the Data Viewer Grid

#### Horizontal Scroll

Set and get the Horizontal Scroll property of the Data Viewer Grid

#### Empty Text

Set and get the Empty Text property of the Data Viewer Grid

### Data Sources

When you connect a Data Source to your project you will also have access to a second block drawer. These Data Source blocks allow you to perform a variety of CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) operations on your data.&#x20;

Click on the link below to learn how to use the Data Sources blocks in your project.&#x20;

{% content-ref url="data-sources.md" %}
[data-sources.md](data-sources.md)
{% endcontent-ref %}
