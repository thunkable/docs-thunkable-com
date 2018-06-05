---
description: >-
  Stack navigators provides a way for your app to transition between screens
  where the new screen is stacked on top of the original screen
---

# Stack Navigator

{% hint style="warning" %}
Navigators are the only component that you cannot drag and drop into your phone at the moment. You'll have to drag it left to the tree hierarchy. Make sure that screens are fully contained within your navigator.
{% endhint %}

![](../../../../.gitbook/assets/thunkable-documentation-exhibits-85.png)

![](../../../../.gitbook/assets/thunkable-documentation-exhibits-84.png)

## Name your screens

The Stack navigator creates a header bar across all screens. You can add a title to this bar by navigating to the Screen properties

| Property | Description |
| --- | --- | --- |
| Header Title | Title of your header |
| Header Back Title | Title of the back button on a stacked screen; if `blank`, will use the `Header Title` |

## Set your screen transitions

To enable a Stack transition, you will have to add a Screen navigation block like the one below. You can find the Screen navigation block in the pre-built Control category:

![](../../../../.gitbook/assets/blocks-control-fig-8%20%281%29.png)

Screens can Stack from left to right or from top to bottom. You can set the transition style with the Stack property below:

| Property | Description |
| --- | --- |
| Mode | Default \(`card`\); `Card` mode stacks screens from left to right while `modal` stacks screens from top to bottom |

## Hide your header

It is possible to hide the Header bar and maintain the Stacking transition by using the Stack property below. Hiding the Header bar will also hide the back button that makes it easier to transition to your original screen

| Property | Description |
| --- | --- |
| Header Mode | Default \(`Screen`\); If you want to hide the header, set to `none` |

## Style your screen color

By default, when you add a Stack, the Screens contained within it change their background color to a light gray. If you want to change it to another color, find the Screen property below:

| Property | Description |
| --- | --- |
| Background Color | Default \(`Light gray`\). Select any color using the color picker, RGBA or HEX value |

