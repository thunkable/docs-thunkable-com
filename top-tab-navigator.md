---
description: >-
  Possibly the most common style of navigation in mobile apps is tab-based
  navigation.
---

# Top Tab Navigator

The Top Tab Navigator is positioned at the top of your app, and allows users to switch between different screens by clicking.&#x20;

![](<.gitbook/assets/image (112).png>)

## Adding Navigators

To add a navigator to your app, you will need to drag the navigator component into your component tree, and then drag a screen on top of the navigator component.&#x20;

![](<.gitbook/assets/ezgif.com-video-to-gif-6 (1).gif>)

## Tab Navigator Properties

You have many options for styling your Top Tab Navigator, such as changing the background color or tint color. Here are the different options for customization:

#### Simple Properties

* **SwipeEnabled:** Allow the user to swipe between screens.
* **AnimationEnabled:** Select whether to animate the transitions between screens.
* **Lazy:** If `true`, tabs are only loaded once the tab is opened. If `false`, all tabs are loaded when the Tab Navigator is first opened.
* **Background Color:** Select a color for the top tab navigator.&#x20;
* **Tab Indicator Color:** An underline will appear underneath the tab you select. You can select a color for the underline.&#x20;
* **Active Tint Color:** Select a font color for the tab currently in use.
* **Inactive Tint Color:** Select a color for the text of the tabs that are not in use.&#x20;
* **ShowIcon:** Toggle whether to show icons in the Tab Navigator.
* **ShowLabel:** Toggle whether to show tab labels in the Tab Navigator.

#### Advanced Properties

* **Upper Case Label:** Make the text for all the tabs upper case.&#x20;
* **PressColor:** Color of material ripple as a tab is pressed
* **PressOpacity:** Opacity of material ripple as a tab is pressed
* **ScrollEnabled:** Toggle whether to enable scrollable tabs
* **Tab Indicator Height:** An underline will appear underneath the tab you select. This section will allow you to choose how tall the underline is.

## Adding Labels and Icons to Your Tabs&#x20;

When designing a tab, you can use words or images to guide users to different screens.&#x20;

![Using Words](<.gitbook/assets/image (112).png>)

![Using Images](<.gitbook/assets/image (54).png>)

## Step by Step Instructions

Step 1. Add screens to a Navigator by dragging and dropping them on top of a Navigator.

Step 2. Select the Top Tab Navigator. Decide if you would like to display icons or labels by clicking on these switches:

![](<.gitbook/assets/image (44).png>)

Step 3. Depending on if you are adding icons or labels, select the screen you would like to style and upload an image or add content:

![](<.gitbook/assets/image (72).png>)

Additional descriptions are below:

**Tab Bar Label** -- The name of your tab label

**Active Tab Icon** -- Icon that appears when tab is selected; You can upload an image for this icon.

**Inactive Tab Icon** --  Icon that appears when tab is not selected; You can upload an image for this icon.

## Enable Swiping

Swiping is a popular way to move through screens and is enabled by the Tab Navigator. You can enable the swipe feature by clicking the "SwipeEnabled' switch.&#x20;

![](<.gitbook/assets/image (64).png>)
