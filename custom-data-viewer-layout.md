---
description: Design a custom layout for displaying your data in a Data Viewer
---

# Custom Data Viewer Layout

## Overview

While the [Data Viewer List](data-viewer-list.md) and [Data Viewer Grid](data-viewer-grid.md) have different layout options, you may want to design a custom layout for your data. This can be achieved with [Row](row.md) and [Column](column.md) components.

## Video Tutorial

{% embed url="https://youtu.be/UIZtLgELGyk" %}

## How To Use a Custom Layout in Your App

### Design your Custom Layout

Use a [Row](row.md) or [Column](column.md) to create the custom layout you want. We will refer to this as the 'Parent Row/Column' for the rest of this doc. 

This layout is a Row that contains two Columns. The first Column contains 3 [Labels](label.md): **TitleLabel**, **DescriptionLabel**, and **PriceLabel**. The second Column contains an [Image](image-1.md), **ProductImage**, and a Rating, called **ProductRating**. These components will be referenced in subsequent screenshots in this document.

{% hint style="info" %}
If you want to set the height or width of your parent row/column to fill the container, we recommend setting it to **Relative Size - 100%** for best results.
{% endhint %}

![](.gitbook/assets/initial-layout%20%282%29.png)

### Save your Custom Layout

Select your Parent Row/Column and click the 'Save as Data Viewer Layout' button.

![](.gitbook/assets/save-as-dv-layout.png)

#### Basic

When you click **Save as Data Viewer Layout**, you will see the following dialog:

![](.gitbook/assets/screen-shot-2020-09-14-at-10.20.08-am.png)

To save a basic Data Viewer Layout:

* Enter a **Layout Name**
* Select if your **Layout Type** is **List** or **Grid**

![](.gitbook/assets/screen-shot-2020-09-14-at-10.20.14-am.png)

* Let **Advanced Binding** be set to **false**
* Click **OK**

#### Advanced

To save an advanced Data Viewer Layout:

* Enter a **Layout Name**
* Select if your **Layout Type** is **List** or **Grid**
* Set **Advanced Binding** to **true**

You can now select which properties of the components in your Parents Row/Column you want to bind to the values in your Data Source.

![](.gitbook/assets/selectprops.png)

Once you have selected all of the properties that you want bound to the values in your Data Source, click **OK** to save your custom Data Viewer layout.

![](.gitbook/assets/boundprops.png)

### Use Your Custom Layout

Once you have saved your custom layout, you can select it as a layout for your Data Viewer. If your layout was saved with the Layout Type List, it can be used with the [Data Viewer List](data-viewer-list.md). If it was saved with the Layout Type Grid, it can be used with the [Data Viewer Grid](data-viewer-grid.md).

![](.gitbook/assets/select-custom-layout.png)

### Bind Your Data to Your Custom Layout

You can bind the properties of your data to a [Data Source](data-sources.md).

#### Basic

With Basic Data Binding, Thunkable will automatically select basic properties of your components to bind to values in your data source.

![](.gitbook/assets/simple-binding%20%281%29.png)

#### Advanced

With Advanced Data Binding, Thunkable will allow you to bind the properties that you specified to your data source:

![](.gitbook/assets/advanced-binding.png)

## Managing your Custom Data Layouts

You can manage your custom data layouts by going to your Thunkable homepage at [x.thunkable.com/projects](https://x.thunkable.com/projects) and clicking on the **My Modules** tab at the top of the page. From here, you can edit and delete your custom data layouts.

![](.gitbook/assets/screen-shot-2020-09-14-at-5.15.24-pm.png)

