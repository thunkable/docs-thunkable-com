---
description: >-
  Possibly the most common style of navigation in mobile apps is tab-based
  navigation.
---

# Top Tab Navigator

The Top Tab Navigator is positioned at the top of your app, and allows users to switch between different screens by clicking.&#x20;

![](<.gitbook/assets/image (112).png>)

## Video Tutorial

You can watch a video tutorial that explains all of the Navigators here:

{% embed url="https://www.youtube.com/watch?v=TqIVHGYdi54" %}

## Adding Navigators

To add a navigator to your app, click **Screens +** at the top of your component tree. \
Select **Add Navigator** and select the Navigator you want to add.

![](.gitbook/assets/screen-shot-2021-04-08-at-5.06.23-pm.png)

## Top Tab Navigator Properties

You have many options for styling your Top Tab Navigator, such as changing the background color or tint color. Here are the different options for customization:

| Property            | Description                                                                                                                     | Data Type        |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| Swipe Enabled       | Allow the user to swipe between screens.                                                                                        | True/False       |
| Animation Enabled   | Select whether to animate the transitions between screens.                                                                      | True/False       |
| Lazy                | If `true`, tabs are only loaded once the tab is opened. If `false`, all tabs are loaded when the Tab Navigator is first opened. | True/False       |
| Background Color    | Select a color for the top tab navigator.                                                                                       | Color            |
| Tab Indicator Color | An underline will appear underneath the tab you select. You can select a color for the underline                                | Color            |
| Active Tint Color   | Select a text color for the tab currently in use.                                                                               | Color            |
| Inactive Tint Color | Select a color for the text of the tabs that are not in use.                                                                    | Color            |
| Show Label Icon     | Select whether to show icons, labels, or both in the Tab Navigator.                                                             | Select from menu |

### Advanced Properties <a href="#data-viewer-list" id="data-viewer-list"></a>

| Property                     | Description                                                                                                              | Data Type  |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------ | ---------- |
| Uppercase Label              | Make the text for all the tabs upper case.                                                                               | True/False |
| Press Color (Android only)   | Color of material ripple as a tab is pressed.                                                                            | Color      |
| Press Opacity (Android only) | Opacity of material ripple as a tab is pressed.                                                                          | Number     |
| Tab Indicator Height         | An underline will appear underneath the tab you select. This section will allow you to choose how tall the underline is. | Number     |



## Adding Labels and Icons to Your Tabs&#x20;

When designing a tab, you can use words or images to guide users to different screens.&#x20;

![Using Words](<.gitbook/assets/image (112).png>)

![Using Images](<.gitbook/assets/image (54).png>)

## Tab-Specific Properties

Click on a tab in your design to access the properties panel for that specific tab.

### Screen

| Property                           | Description                                                                                                                                      | Data Type                                                                                                                                                                                                    |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Navigation Button Name             | Text that appears in the top tab navigator.                                                                                                      | Text                                                                                                                                                                                                         |
| Scrollable                         | Select whether your user can scroll on this screen.                                                                                              | True/False                                                                                                                                                                                                   |
| Background Color                   | Select the tab's background color.                                                                                                               | Color                                                                                                                                                                                                        |
| Background Image                   | The image file to be shown in the tab's background                                                                                               | <p>PNG, JPG, GIF, SVG, etc.<br>Can also use URL that ends in file extension (eg <a href="https://thunkable.com/static/media/logo.ba96eb83.png">https://thunkable.com/static/media/logo.ba96eb83.png</a>)</p> |
| Background Image Resize Mode       | Set how image is shown if the file and the tab component have different dimensions/aspect ratio                                                  | <p>Select from list <code>[cover, contain, stretch, repeat, center]</code><br></p>                                                                                                                           |
| Orientation (iOS and Android only) | Toggle whether your end user can swipe a list item to the left to view an additional Button. Reveals Left Swipe Button settings if set to `true` | True/False                                                                                                                                                                                                   |

### Tab Navigation Options

| Property          | Description                                                                            | Data Type                                                                                                                                                                                                    |
| ----------------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Tab Bar Label     | Set the Label of this Screen's tab in the Tab Navigator                                | Text                                                                                                                                                                                                         |
| Active Tab Icon   | Set the Icon of this Screen's tab in the Tab Navigator for when the Screen is active   | <p>PNG, JPG, GIF, SVG, etc.<br>Can also use URL that ends in file extension (eg <a href="https://thunkable.com/static/media/logo.ba96eb83.png">https://thunkable.com/static/media/logo.ba96eb83.png</a>)</p> |
| Inactive Tab Icon | Set the Icon of this Screen's tab in the Tab Navigator for when the Screen is inactive | <p>PNG, JPG, GIF, SVG, etc.<br>Can also use URL that ends in file extension (eg <a href="https://thunkable.com/static/media/logo.ba96eb83.png">https://thunkable.com/static/media/logo.ba96eb83.png</a>)</p> |
| Tab Bar Visible   | Set whether the Tab Navigator is visible when this Screen is open                      | True/False                                                                                                                                                                                                   |

### Status Bar

| Property                   | Description | Data Type                                               |
| -------------------------- | ----------- | ------------------------------------------------------- |
| Visibility                 |             | True/False                                              |
| Style                      |             | Select from menu (default, light-content, dark-content) |
| Color (Android only)       |             | Color                                                   |
| Translucent (Android only) |             | True/False                                              |

