---
description: >-
  Possibly the most common style of navigation in mobile apps is tab-based
  navigation.
---

# Top Tab Navigator

The Top Tab Navigator is positioned at the top of your app, and allows users to switch between different screens by clicking. 

![](.gitbook/assets/image%20%28112%29.png)

## Adding Navigators

To add a navigator to your app, click **Screens +** at the top of your component tree.   
Select **Add Navigator** and select the Navigator you want to add.

![](.gitbook/assets/screen-shot-2021-04-08-at-5.06.23-pm.png)

## Tab Navigator Properties

You have many options for styling your Top Tab Navigator, such as changing the background color or tint color. Here are the different options for customization:

#### Simple Properties

* **SwipeEnabled:** Allow the user to swipe between screens.
* **AnimationEnabled:** Select whether to animate the transitions between screens.
* **Lazy:** If `true`, tabs are only loaded once the tab is opened. If `false`, all tabs are loaded when the Tab Navigator is first opened.
* **Background Color:** Select a color for the top tab navigator. 
* **Tab Indicator Color:** An underline will appear underneath the tab you select. You can select a color for the underline. 
* **Active Tint Color:** Select a font color for the tab currently in use.
* **Inactive Tint Color:** Select a color for the text of the tabs that are not in use. 
* **ShowIcon:** Toggle whether to show icons in the Tab Navigator.
* **ShowLabel:** Toggle whether to show tab labels in the Tab Navigator.

#### Advanced Properties

* **Upper Case Label:** Make the text for all the tabs upper case. 
* **PressColor:** Color of material ripple as a tab is pressed
* **PressOpacity:** Opacity of material ripple as a tab is pressed
* **ScrollEnabled:** Toggle whether to enable scrollable tabs
* **Tab Indicator Height:** An underline will appear underneath the tab you select. This section will allow you to choose how tall the underline is.

## Adding Labels and Icons to Your Tabs 

When designing a tab, you can use words or images to guide users to different screens. 

![Using Words](.gitbook/assets/image%20%28112%29.png)

![Using Images](.gitbook/assets/image%20%2854%29.png)

## Step by Step Instructions

Step 1. Add screens to a Navigator by dragging and dropping them on top of a Navigator.

Step 2. Select the Top Tab Navigator. Decide if you would like to display icons or labels by clicking on these switches:

![](.gitbook/assets/image%20%2844%29.png)

Step 3. Depending on if you are adding icons or labels, select the screen you would like to style and upload an image or add content:

![](.gitbook/assets/image%20%2872%29.png)

Additional descriptions are below:

**Tab Bar Label** -- The name of your tab label

**Active Tab Icon** -- Icon that appears when tab is selected; You can upload an image for this icon.

**Inactive Tab Icon** --  Icon that appears when tab is not selected; You can upload an image for this icon.

## Enable Swiping

Swiping is a popular way to move through screens and is enabled by the Tab Navigator. You can enable the swipe feature by clicking the "SwipeEnabled' switch. 

![](.gitbook/assets/image%20%2864%29.png)

