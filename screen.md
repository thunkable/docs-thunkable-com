---
description: >-
  When building apps on Thunkable, Screens function like blank pages in a book.
  They allow you to display different components and information.
---

# Screen

## Adding a Screen to your Project

{% hint style="warning" %}
This feature is available to users with a Team level subscription only at this time.&#x20;
{% endhint %}

There are two ways to add a new screen to your app:

Click the + icon next to your Screen names in the Screens bar.

![](.gitbook/assets/screen-shot-2021-04-12-at-8.06.10-am.png)

Click **Screens +** at the top of your component tree. \
Select **Create New Screen.**

![](.gitbook/assets/screen-shot-2021-04-08-at-5.11.05-pm.png)

## Screen Properties

### Screen

| Property                           | Description                                                                                                                                                                           | Data Type                                                                                                                                                                                                    |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Scrollable                         | Select whether your user can scroll on this screen. For scrollable to work, the components in your screen must have heights either set in `absolute` pixels or set to `fit contents.` | True/False                                                                                                                                                                                                   |
| Background Color                   | Default (`none`). Select any color using the color picker, RGBA or HEX value                                                                                                          | Color                                                                                                                                                                                                        |
| Background Image                   | The image file to be shown in the tab's background                                                                                                                                    | <p>PNG, JPG, GIF, SVG, etc.<br>Can also use URL that ends in file extension (eg <a href="https://thunkable.com/static/media/logo.ba96eb83.png">https://thunkable.com/static/media/logo.ba96eb83.png</a>)</p> |
| Background Image Resize Mode\*     | Set how image is shown if the file and the tab component have different dimensions/aspect ratio                                                                                       | Select from list `[cover, contain, stretch, repeat, center]`                                                                                                                                                 |
| Orientation (iOS and Android only) | Define the screen's orientation.                                                                                                                                                      | Select from list `[portrait, landscape, auto]`                                                                                                                                                               |

#### \* Background Picture Resize Mode

This determines how to resize the image when the frame doesn't match the raw image dimensions.

![](<.gitbook/assets/image (85).png>)

* **Cover:** Fills the entire screen without changing the height and width ratio of the image\

* **Contain:** The entire image will be scaled down to fit inside the screen, without changing the height and width ratio of the image\

* **Stretch:** The image's height will change to fill the screen length-wise\

* **Repeat:** Repeat the image to cover the screen. The image's height and width ratio will not change  \

* **Center:** Positions the image in the middle of the frame

### Status Bar

| Property                   | Description | Data Type                                               |
| -------------------------- | ----------- | ------------------------------------------------------- |
| Visibility                 |             | True/False                                              |
| Style                      |             | Select from menu (default, light-content, dark-content) |
| Color (Android only)       |             | Color                                                   |
| Translucent (Android only) |             | True/False                                              |



## Save Screen

Thunkable allows you to reuse a screen, and its associated blocks, in multiple projects with the "Save to My Screens" feature. You can find the **Save Screen** button at the top of the properties for every screen component in your app.

![](.gitbook/assets/screen-shot-2021-10-01-at-9.59.01-am.png)

### Name Your Screen

It's important that when you save your screen you use a descriptive and memorable name that describes what your screen does. The example below is for a sign in screen, which is something that often get reused across multiple projects.

![](.gitbook/assets/03\_name\_screen.png)

### Add a New Screen

Once you've saved a screen, any time you click the **`+`** button at the top of your component tree to add a new screen to your project, you will be given the option to add a blank screen or to "Add From Saved Screens".

![](.gitbook/assets/screen-shot-2021-10-01-at-10.00.23-am.png)

### Choose a Saved Screen

Simply choose the screen that you want to add in and click the "Copy" button to proceed.

![](.gitbook/assets/05\_choose\_screen.png)

## Screen Blocks&#x20;

### when Screen1 Starts

![](.gitbook/assets/screen-starts.png)

| Event  | Description                               |
| ------ | ----------------------------------------- |
| Starts | Fires when the Screen is **first** opened |

### when Screen1 Opens

![](.gitbook/assets/screen-opens.png)

| Event | Description                            |
| ----- | -------------------------------------- |
| Opens | Fires **anytime** the Screen is opened |

### when Screen1 BackButtonPressed

![](.gitbook/assets/screen-back-button-pressed.png)

| Event             | Description                                                                 |
| ----------------- | --------------------------------------------------------------------------- |
| BackButtonPressed | Fires when the physical or on-screen back button is pressed. (Android only) |

### in Screen1 call ToggleDrawerMenu

![](.gitbook/assets/screen-toggle-drawer-menu.png)

| Function         | Description                                                                                                                 |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------- |
| ToggleDrawerMenu | Opens or Closes the drawer menu, if available. Must be used in conjunction with the [Drawer Navigator](drawer-navigator.md) |

## Screen-Specific Navigator Properties

When you add a Screen to a Navigator, you will see a new section for **Navigation Options** in your Screen's Properties panel. You can read about these properties in the [Top Tab Navigator](top-tab-navigator.md#screen-specific-tab-navigator-properties), [Bottom Tab Navigator](bottom-tab-navigator.md#screen-specific-tab-navigator-properties), and [Drawer Navigator](drawer-navigator.md#screen-specific-drawer-navigator-properties) docs.
