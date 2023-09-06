---
description: >-
  Navigate to different screens using a clickable drawer that slides out from
  the side.
---

# Drawer Navigator

## Video Tutorial

### How to Use the Thunkable Drawer Navigator

In this tutorial, we'll explore the benefits of using a drawer navigator and provide step-by-step instructions on implementation.

{% embed url="https://youtu.be/-S-9_VbtI5Y" %}

## Add a Navigator

To add a navigator to your app, click **Screens +** at the top of your component tree. \
Select **Add Navigator** and select the Navigator you want to add.

<figure><img src="../../.gitbook/assets/add screen  add navigator menu.png" alt=""><figcaption></figcaption></figure>

## Add Screens to the Drawer Navigator

Within the component tree, drag and drop screens to nest them under the Drawer Navigator component.

![](<../../.gitbook/assets/2023-02-27\_11-22-07 (1).gif>)



## Screen-Specific Drawer Navigator Properties

Once a screen has been added to the drawer navigator, a new section in the screen's properties panel, **Drawer Navigation Options**, becomes available. This is where you define the screen's label that displays in the user's drawer navigator.

## Drawer Navigator Properties

You have many options for styling your Drawer Navigator, such as changing the background color or tint color. Here are the different options for customization:

| Property                  | Description                                                                                              | Data Type                        |
| ------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------- |
| Drawer Width              | The width of the drawer in pixels. By default, this is 280 pixels for phones and 320 pixels for tablets. | Number                           |
| Drawer Position           | The position the Drawer enters the screen from.                                                          | Select from menu (left or right) |
| Active Tint Color         | Text color of selected drawer.                                                                           | Color                            |
| Active Background Color   | Background color of selected drawer.                                                                     | Color                            |
| Inactive Tint Color       | Text color for unselected drawers.                                                                       | Color                            |
| Inactive Background Color | Background color for unselected drawers.                                                                 | Color                            |

