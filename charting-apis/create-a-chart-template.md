# Create a chart template

## What are URL Parameters?&#x20;

One of the quickest and easiest ways to send data to an API is by passing information, which we call _parameters_, in the API URL. One great use case for this is to create graphs and charts with data that has been generated in our app. QuickChart is a no-code solution to automatic chart generation. Create a chart template using the [**chart maker**](https://quickchart.io/chart-maker/) interface. Then use the template endpoint to customize and generate charts automatically.

In this guide, you will learn how to:

1. Create and customize a chart template without any code.
2. Save the chart as a URL (API endpoint) that you can use in emails, Excel, Salesforce, and any other formats.
3. Set the chart’s data by providing special parameters in the URL.

{% embed url="https://youtu.be/lZQJfeepZk4" %}

### Create a chart template <a href="#create-a-chart-template" id="create-a-chart-template"></a>

To create charts online, first go to the [chart maker](https://quickchart.io/chart-maker/). Use the interface to build a chart template. This chart will be the basis of the charts you generate automatically in the future.

#### Add data <a href="#add-data" id="add-data"></a>

To get started, add some dummy or example data. The chart preview will update so you can get an idea of how your visualization will work.

Enter data as comma-separated values (e.g. `10,20,30,40`). Each data value maps to a label (e.g. `Jan, Feb, Mar, Apr`). Edit “Labels” at the top of the Data settings to change this mapping.

![](https://quickchart.io/images/docs/chart-maker/labels\_and\_data.jpeg)

Edit labels and data on the left-hand side of the chart maker



**Using coordinates**

> For more advanced use cases, you may provide your data as (x, y) coordinates.
>
> An example of category-based coordinates: `(Jan, 10), (Feb, 20), (Mar, 30), (Apr, 40)`. These coordinates will give you more power over how your line or scatter plot is displayed.
>
> **Numeric coordinates** are also accepted: `(1, 50), (10, 40), (12, 20), (8, 10)`. This format is most commonly used for scatter plots, and requires you to change your Axes to `linear` or `logarithmic` under settings. In this case, you should clear the “Labels” setting at the top of the Data settings - labels will be automatically generated.
>
> **Time series** use coordinates too. For example: `(2020-01-01, 50), (2020-03-15, 12), (2020-06-05, 40)`. To display time series, change the X-axis to `time` type and clear the “Labels” setting in Data settings, as labels will be generated automatically.

#### Customize look & feel <a href="#customize-look-26-feel" id="customize-look-26-feel"></a>

Now that your data is set, time to make the chart look however you want.

Close the data menu to customize your chart’s axes, ticks, legend, and its overall layout.

![](https://quickchart.io/images/docs/chart-maker/menus.gif)

Customize the chart by expanding different sections

Looking for inspiration? Head over to the [chart gallery](https://quickchart.io/gallery/) - most examples are editable in the chart maker.

### Save the template <a href="#save-the-template" id="save-the-template"></a>

Click **Save as API Template** in the top right.

You’ll be presented with an **API endpoint**. This is the base URL of your chart. If you go to it, you will see a chart image. The URL can be further customized to override properties of your chart.

![](https://quickchart.io/images/docs/chart-maker/chart\_template.png)

Saving as an API template gives you an endpoint you can use to generate unlimited charts.
