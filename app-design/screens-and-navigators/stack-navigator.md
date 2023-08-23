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

# Stack Navigator

## Video Tutorial: How to Use the Thunkable Stack Navigator

In this tutorial, we'll explore what a stack navigator is and provide step-by-step instructions on implementation.

{% embed url="https://youtu.be/bN9W7kxe1Fw" %}

## Stack Navigator Properties

### Set Your Screen Transitions

To enable a Stack transition, add a Screen navigation block like the one below. You can find the Screen navigation block in the Control drawer of blocks:

![](../../.gitbook/assets/btn\_click\_1.png)

| Property | Description                          | Data Type                                                                                                                                        |
| -------- | ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Mode     | Define how your screens will stack.  | <p>Select from list:<br><code>card</code> - new screens slide in from the left<br><code>modal</code> - new screens slide in from the bottom </p> |

### Header Mode

| Property   | Description                                | Data Type                                                                                                                                             |
| ---------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| HeaderMode | Define how the header appears in your app. | <p>Select from list:<br><code>float</code> - headers fade in with the screen change<br><code>screen</code> - headers slide with the screen change</p> |

### Header Shown

It is possible to hide the Header bar and maintain the Stacking transition by using the Stack property below. Hiding the Header bar will also hide the back button that makes it easier to transition to the previous screen.

| Property    | Description                               | Data Type                                                                                                                         |
| ----------- | ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| HeaderShown | Define if the header appears in your app. | <p>Toggle:</p><p><code>true (blue)</code> - show header<br><code>false (grey)</code> - hide header (including the back arrow)</p> |