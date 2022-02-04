---
description: >-
  Create powerful, no-code, data-driven apps connected directly to Google
  Sheets, Airtable, or stored locally.
---

# Data Viewer Grid

{% hint style="info" %}
If you have any feedback for us about the Data Viewer components please let us know over in the [Thunkable Community](https://community.thunkable.com/t/latest-thunkable-release-new-components-data-viewer-list-and-data-viewer-grid-2020-05-05/564204?u=domhnallohanlon).
{% endhint %}

## Overview

The data viewer components allow you to create beautiful user interfaces for your data. All of this is done in just 3 steps, no blocks required!

1. [Pick your Data Source](data-viewer-grid.md#data-source)
2. [Choose your Item Layout](data-viewer-grid.md#layout)
3. [Set your Data Bindings](data-viewer-grid.md#data-bindings)

You can add additional functionality to the Data Viewer Grid by using the included [component blocks](data-viewer-grid.md#blocks) or you can work directly with your raw data by using the [Data Sources blocks](data-sources.md).

## Properties

### Data Viewer Grid

| Property          | Description                                                                                                 | Data Type                                |
| ----------------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Data Source       | The [Data Source](data-sources.md#add-a-data-source-to-your-app) your data is to be pulled from             | Reference to chosen data source          |
| Table             | Table from your Data Source to show data from                                                               | Reference to chosen table in Data Source |
| Layout            | Format of how your data will be displayed in your app                                                       | Select from list                         |
| Bindings          | Select what items of data from your Data Source to show in which aspects of yoru layout                     | Select from lists                        |
| Horizontal Scroll | Toggle whether your Data Viewer should scroll horizontally (if `false`, Data Viewer will scroll vertically) | True/False                               |
| Empty Text        | Text that will be displayed if there is no data to fill a string in your Data Viewer                        | Text                                     |

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

The entire Data Viewer can be completely hidden or shown by setting the `Visible`property to false or true, respectively.&#x20;

![](<.gitbook/assets/grid\_visible (1).png>)



### Data Sources

When you connect a Data Source to your project you will also have access to a second block drawer. These Data Source blocks allow you to perform a variety of CRUD (**C**reate, **R**ead, **U**pdate, **D**elete) operations on your data.&#x20;

Click on the link below to learn how to use the Data Sources blocks in your project.&#x20;

{% content-ref url="data-sources.md" %}
[data-sources.md](data-sources.md)
{% endcontent-ref %}



