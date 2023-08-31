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

# Custom Data Viewer

## Overview

Thunkable provides various default [data viewer list](data-viewer-list.md) and [data viewer grid](data-viewer-grid.md) templates, but saving a customized layout component as a data viewer allows you to display your data in a way that reflects your brand design and preferences.&#x20;

## Video Tutorial

### How to Customize a Data Viewer in Thunkable

In this tutorial, we’ll show you how to customize a Thunkable data viewer so you can display your data in a way that meets your user’s needs and reflects your brand design.

{% embed url="https://www.youtube.com/watch?v=O6ohIj0ZfMg" %}

## To Save a Layout as a Data Viewer:

1. When you're happy with the layout you have customized, ensure it is selected in the component tree.
2. Click the **vertical ellipsis** next to the layout's name in the properties panel.
3.  Select **Save as Data Viewer Layout**.\


    <div align="left">

    <figure><img src="../../../../.gitbook/assets/Layout - Save as Data Viewer Layout.png" alt="" width="563"><figcaption></figcaption></figure>

    </div>
4. Give your data viewer layout a detailed **name**.
5. Select the **Layout Type** you want to create. \
   \- List for a data viewer list\
   \- Grid for a data viewer grid
6. Click **OK**.

### To Use a Saved Layout as a Data Viewer:

1. Click the **Create New Screen** icon at the top of the component tree in the Designer. &#x20;
2. Drag a **Data Viewer Lis**t or **Data Viewer Grid** component onto your screen.
3. Reposition and resize as necessary.
4. Connect your project to a data source. See here for instructions on connecting a data source: [Data Sources](../../../../getting-started/data-sources/).
5.  Click the sample template to access the data viewer templates available to you.\


    <div align="left">

    <figure><img src="../../../../.gitbook/assets/Data Viewer List - properties panel - design template.png" alt="" width="290"><figcaption></figcaption></figure>

    </div>
6. Click to select the layout you saved as a data viewer from the bottom of the template library.&#x20;
7.  Map your data source columns to components within your custom data viewer layout. \


    <div align="left">

    <figure><img src="../../../../.gitbook/assets/Data Viewer - properites panel - map column data.png" alt="" width="279"><figcaption></figcaption></figure>

    </div>

## Related Docs

### Layout Component

Custom data viewers are created using Thunkable’s layout component, which allow for more precise positioning of UI components on an app screen.

{% content-ref url="../../basic-components/layout.md" %}
[layout.md](../../basic-components/layout.md)
{% endcontent-ref %}

### Data Sources Blocks

By incorporating the data source blocks into your app, you can allow users to create, read, update, and delete data in your data source when they interact with the data viewer.

{% content-ref url="../../../../blocks/app-features/data-sources-blocks.md" %}
[data-sources-blocks.md](../../../../blocks/app-features/data-sources-blocks.md)
{% endcontent-ref %}
