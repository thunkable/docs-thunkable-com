#### **Thunkable for Android **❤

# Components: Screen

---

Screens are natural ways to break up your apps so that they are more digestible to your users. On Thunkable, there is a limit of 10 screens per app.

Screens are where you set layouts and program navigation. Screen1 is also where you set many of your app level properties.

---

### How to add a screen

![](https://lh6.googleusercontent.com/1oEzLB4YgohJ9xkkqyOox_Ljr9gbVxreM8EfuVqC0LX0jni6rhmNbBvZzbrqCCng0dHfeKh_g2bPthx2pfKrTpHZx3jOpAel5K_zXQPs3UyabZ1dYzq0VD4ikRJ0krCWMPZkpJZg)

---

### App settings\* \(Screen1 Only\)

| Property | Description |
| :--- | :--- |
| App Name | Name of the app as it appears below the icon on the phone. Will be set to the project name initially. |
| Icon | App icon -- the recommended app icon size is 96 px by 96 px |
| Sizing | If set to responsive \(recommended\), screen layouts will autoscale to the size of the screen. Components should be sized to 'percent' height and width. If set to fixed, screen layouts will be created for a single fixed-sized screen and components should be sized to 'pixels' height and width |
| Version Name | Description which helps users distinguish between different versions of your app on the Google Play Store |
| Version Code | An integer value which must be incremented each time a new .apk is created for the Google Play Store |

\*Can only be set in the Designer

---

### Appearance, layout & animations

| Property | Description |
| :--- | :--- |
| Title |  |
| Title |  |
|  |  |
| About Screen | Appears when "About this Application" is selected from the system menu. The title must be visib |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |

TitleVisible

The title bar is the top gray bar on the screen. This property reports whether the title bar is visible.

Title

The caption for the form, which appears in the title bar.

ShowStatusBar

The status bar is the topmost bar on the screen. This property reports whether the status bar is visible.



Align Horizontal

A number that encodes how contents of the screen are aligned horizontally. The choices are: 1 = left aligned, 2 = horizontally centered, 3 = right aligned.

Align Vertical

A number that encodes how the contents of the arrangement are aligned vertically. The choices are: 1 = aligned at the top, 2 = vertically centered, 3 = aligned at the bottom. Vertical alignment has no effect if the screen is scrollable.

Background Image

The screen background image.

Close Screen Animation

The animation for closing current screen and returning to the previous screen. Valid options are default, fade, zoom, slidehorizontal, slidevertical, and none.

OpenScreenAnimation

The animation for switching to another screen. Valid options are default, fade, zoom, slidehorizontal, slidevertical, and none.

ScreenOrientation

The requested screen orientation, specified as a text value. Commonly used values are landscape, portrait, sensor, user and unspecified. See the Android developer documentation for ActivityInfo.Screen\_Orientation for the complete list of possible settings.

Scrollable

When checked, there will be a vertical scrollbar on the screen, and the height of the application can exceed the physical height of the device. When unchecked, the application height is constrained to the height of the device.



