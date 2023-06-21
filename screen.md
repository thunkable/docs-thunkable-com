---
description: >-
  When building apps on Thunkable, Screens function like blank pages in a book.
  They allow you to display different components and information.
---

# Screen

## Adding a Screen to your Project

There are two ways to add a new screen to your app:

Click the + icon next to your Screen names in the Screens bar.

<figure><img src=".gitbook/assets/Add screen from top header.png" alt=""><figcaption></figcaption></figure>

Click **New Screen** icon at the top of your components tree. \
Select **Create New Screen.**

<div align="left">

<figure><img src=".gitbook/assets/Create new screen icon.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

### Copy and paste components&#x20;

Once you’ve perfected the design of a screen on the Design tab of a drag and drop project you can duplicate it using copy and paste keyboard shortcuts.

To copy and paste a screen:&#x20;

1.  Click on a screen name in the component tree (A) or the screen itself within your workspace (B).

    <figure><img src="https://lh3.googleusercontent.com/aVVH2nMfdTb2fyerNLzn4HktWL-hv50diVzP90PQvpSbbB45FGWUwj1OF9chxAoR1iVJV813LPP3nL8Yd95Av6EAw5NEG1oOktoM1GXqDg8LyLCraIKV-zXSHmtBXHJp-LNdDX_446vqo7028JI4o9IrQYPDTPo4aIkhwA-ZakAejpB0DctUGreUVA" alt=""><figcaption></figcaption></figure>
2. Type **ctrl+c** or **command+c** on Mac, and **ctrl+c** on PC, to copy the screen.&#x20;
3. Type **ctrl+v** or **command+v** on Mac, and **ctrl+v** on PC, to paste a duplicate of the screen.
4. The new screen will be added to the right of the existing screen.

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

The status bar is located at the top of a phone's screen. The status bar displays information regarding signal strength, battery, and whether or not things like the alarm or wi-fi are enabled.

| Property                   | Description                                                                                                                    | Data Type                                               |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------- |
| Visibility                 | Decide whether you want the status bar visible on the screen.                                                                  | True/False                                              |
| Style                      | Default is best practice, but you can select light-content or dark-content to potentially override the user's phone settings.  | Select from menu (default, light-content, dark-content) |
| Color (Android only)       | Color of the status bar.                                                                                                       | Color                                                   |
| Translucent (Android only) | When translucent is set to true, the app will appear under the status bar.                                                     | True/False                                              |



## Save and Resuse Screens

Thunkable allows you to reuse a screen, and its associated blocks, in multiple projects.&#x20;

{% hint style="warning" %}
This feature is available with the Thunkable Teams plan. See here for more information: [Thunkable pricing](https://thunkable.com/#/pricing).
{% endhint %}

{% embed url="https://youtu.be/-gIH6tV7Yfs" %}

### Save Screen

1. Select the screen in the Designer.
2. Click the vertical elipses at the top of the screen's properties pane.
3. Click **Save Screen**.\
   ![](<.gitbook/assets/Save Screen menu.png>)
4. Give your screen a descriptive name.&#x20;
5. Click **Save**.

### Add Screen to Another Project

1. Open the project in which you'd like to add the saved screen.
2.  Click the upside-down arrow at the top of the Designer's component tree.\


    <div align="left">

    <figure><img src=".gitbook/assets/Add From Saved Screens.png" alt="" width="563"><figcaption></figcaption></figure>

    </div>
3. Click **Add From Saved Screens**.
4. Select the screen you want to add.
5.  Click **Copy**.\


    ![](.gitbook/assets/05\_choose\_screen.png)

### Errors&#x20;

When a saved screen is added to a new project, you may notice some errors in the blocks that you’ll need to address. This is because the app you have added the screen to doesn’t necessarily have the same features. For example, the blocks may navigate the user to a screen that doesn’t exist in the new app. Another example of an error that would need to be addressed is if the screen had a data viewer, but the data source wasn’t connected to this project.

### View All Saved Screens

1. Navigate to your Projects Page.
2.  Click **My Screens** in the upper left.\


    <div align="left">

    <figure><img src=".gitbook/assets/Projects Screen  My Screens.png" alt="" width="563"><figcaption></figcaption></figure>

    </div>
3. On you My Screens page you can view your screens, rename them, and delete screens you no longer need.

## Disable app screen preview

You can disable screen preview for apps with many screens to improve platform performance and load time. When enabled, the project only loads the screen you're working on, and the others are paused.&#x20;

<figure><img src=".gitbook/assets/disable app screen preview - Designer.png" alt=""><figcaption></figcaption></figure>

To disable app screen preview:

1. Click your **account avatar or icon** in the upper right corner.&#x20;
2. Select **Settings**.&#x20;
3. Click the **FEATURES** tab.
4. Toggle on **Disable app screen preview**.

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
