#### **Thunkable for Android **❤

# Components: Screen

---

Screens are natural ways to break up your apps so that they are more digestible to your users. On Thunkable, there is a limit of 10 screens per app.

Screens are where you set layouts, program the initial opening of the app and the navigation. Screen1 is also where you set many of your app level properties.

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
| Title | Displayed on title bar |
| Title Visible | If checked, shows a default \(gray\) title bar on the screen |
| About Screen | Appears when "About this Application" is selected from the system menu. The title must be visible for this screen to be visible |
| Show Status Bar | If checked, shows the top most bar on the screen which displays time, battery etc |
| Alight Horizontal | Center, Left or Right |
| Alight Vertical | Center, Top or Bottom |
| Background Image | You can upload an image to your app or reference an image url |
| Background Color | Default \(White\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
|  |  |
|  |  |
|  |  |
|  |  |

Close Screen Animation

The animation for closing current screen and returning to the previous screen. Valid options are default, fade, zoom, slidehorizontal, slidevertical, and none.

OpenScreenAnimation

The animation for switching to another screen. Valid options are default, fade, zoom, slidehorizontal, slidevertical, and none.

ScreenOrientation

The requested screen orientation, specified as a text value. Commonly used values are landscape, portrait, sensor, user and unspecified. See the Android developer documentation for ActivityInfo.Screen\_Orientation for the complete list of possible settings.

Scrollable

When checked, there will be a vertical scrollbar on the screen, and the height of the application can exceed the physical height of the device. When unchecked, the application height is constrained to the height of the device.

