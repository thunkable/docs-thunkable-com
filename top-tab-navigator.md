---
description: >-
  Possibly the most common style of navigation in mobile apps is tab-based
  navigation.
---

# Top Tab Navigator

The Top Tab Navigator is positioned at the top of your app, and allows users to switch between different screens by clicking.&#x20;

<div align="left">

<img src=".gitbook/assets/image (112).png" alt="">

</div>

## Video Tutorial

{% embed url="https://youtu.be/ZkxI53wF3UE" %}

## Adding Navigators

To add a navigator to your app, click the dropdown arrow at the top of your component tree.\
Select **Add Navigator** and select the Navigator you want to add.

<figure><img src=".gitbook/assets/Navigator menu.png" alt=""><figcaption></figcaption></figure>

## Top Tab Navigator Properties

You have many options for styling your Top Tab Navigator, such as changing the background color or tint color. To access the navigator's properties panel, click the Top Tab Navigator's name in the component tree. Here are the different options for customization:

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

<div align="left">

<img src=".gitbook/assets/image (112).png" alt="Using Words">

</div>

<div align="left">

<img src=".gitbook/assets/image (54).png" alt="Using Images">

</div>

## Tab-Specific Properties

To access the properties panel for a specific tab, click the screen name in the component tree.&#x20;

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

The status bar is located at the top of a phone's screen. The status bar displays information regarding signal strength, battery, and whether or not things like the alarm or wi-fi are enabled.

| Property                   | Description                                                                                                                    | Data Type                                               |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------- |
| Visibility                 | Decide whether you want the status bar visible on the screen.                                                                  | True/False                                              |
| Style                      | Default is best practice, but you can select light-content or dark-content to potentially override the user's phone settings.  | Select from menu (default, light-content, dark-content) |
| Color (Android only)       | Color of the status bar.                                                                                                       | Color                                                   |
| Translucent (Android only) | When translucent is set to true, the app will appear under the status bar.                                                     | True/False                                              |

