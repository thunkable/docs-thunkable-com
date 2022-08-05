---
description: Navigate to different screens using a bottom tab navigator.
---

# Bottom Tab Navigator

![Bottom tabs are a popular way to navigate an app today](.gitbook/assets/thunkable-docs-exhibits-81.png)

## Video Tutorial

You can watch a video tutorial for using Navigators in your Thunkable app here:

{% embed url="https://www.youtube.com/watch?v=0NrkKiCGaxk&list=PLB89L9PPGIrxGeViKhkRvHVD7yFc4q_Np&index=2" %}

## Adding Navigators

To add a navigator to your app, click **Screens +** at the top of your component tree. \
Select **Add Navigator** and select the Navigator you want to add.

![](.gitbook/assets/screen-shot-2021-04-08-at-5.06.23-pm.png)

## Bottom Tab Navigator Properties

You have many options for styling your Bottom Tab Navigator, such as changing the background color or tint color. Here are the different options for customization:

| Property                  | Description                                                         | Data Type        |
| ------------------------- | ------------------------------------------------------------------- | ---------------- |
| Active Tint Color         | Select a text color for the tab currently in use.                   | Color            |
| Active Background Color   | Select a background color for the tab currently in use.             | Color            |
| Inactive Tint Color       | Select a color for the text of the tabs that are not in use.        | Color            |
| Inactive Background Color | Select a color for the tab not currently in use.                    | Color            |
| Show Label Icon           | Select whether to show icons, labels, or both in the Tab Navigator. | Select from menu |

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

