# Charting in Thunkable

## Setting URL Parameters in Thunkable

Now that we know what URL parameters are, we can start creating blocks in our project to dynamically update the parameters. To do this we'll use the Text blocks, and in particular the Join block, to change out each of our variables.

### Overview

{% hint style="success" %}
**Remix Link:** [**https://x.thunkable.com/projectPage/6227740a29e8cb0010e04e5d**](https://x.thunkable.com/projectPage/6227740a29e8cb0010e04e5d)
{% endhint %}

To recreate the UI for this app you can add an image and a button - click on the remix button to add the UI and blocks for this project to your Thunkable account.

### Block it Out

Drag an image component onto the screen. The chart URL will be used as the image source. The URL should be set in your blocks unless you plan to have a static chart image, in which case you may set the image source on the design screen.&#x20;

* Drag an image component to the screen
* Go to your blocks
* Following some user or system generated action, set the url for the image component using the Quickchart API **base URL** provided while saving your chart
* All chart updates will be made by appending text `join blocks` to the image source URL.&#x20;

<figure><img src="../../.gitbook/assets/Charting in Thunkable  Blocking it out.png" alt=""><figcaption></figcaption></figure>

## Use the no-code chart API <a href="#use-the-no-code-chart-api" id="use-the-no-code-chart-api"></a>

Currently, three aspects of your chart can be overriden with custom values:

1. Chart title
2. Dataset labels
3. Data

These customizations are passed as URL parameters. For example, to override chart title, take the base URL and add the following:

```
?title=New title
```

<figure><img src="../../.gitbook/assets/Charting in Thunkable  use no code 1.png" alt=""><figcaption></figcaption></figure>

You can join URL parameters together using the **&** symbol. For example:

```
?title=New title&labels=Q1,Q2,Q3,Q4
```

<figure><img src="../../.gitbook/assets/Charting in Thunkable  use no code 2.png" alt=""><figcaption></figcaption></figure>

To override data, use **data1**, **data2**, **data3**, …, for each dataset on the chart.

For example, to override the first (primary) dataset:

```
?data1=40,60,80,100
```

<figure><img src="../../.gitbook/assets/Charting in Thunkable  use no code 3.png" alt=""><figcaption></figcaption></figure>

To override multiple datasets and the chart title:

```
?data1=40,60,80,100&data2=5,6,7,8&title=Updated chart

```

<figure><img src="../../.gitbook/assets/Charting in Thunkable  use no code 4.png" alt=""><figcaption></figcaption></figure>
