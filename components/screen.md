#### **Thunkable for Android **❤

# Components: Screen

---

Screens are natural ways to break up your apps so that they are more digestible to your users. On Thunkable, there is a limit of 10 screens per app.

Screens are where you set layouts and program navigation. Screen1 is also where you set many of your app level properties.

---

### App settings \(Screen 1 Only\)

| Property | Description |
| :--- | :--- |
|  |  |
|  |  |

### Appearance and layout

| Property | Description |
| :--- | :--- |
| Height | Button height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Button width in pixels, percent, 'Automatic' or 'Fill' |
| Shape\* | Default \(rectangle\), rounded, rectangular or oval.  The shape will not be visible if an Image is being displayed |
| Background Color | Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Image | You can upload an image to your app or reference an image url. If an image is uploaded, it will negate the background color and shape properties |
| Text | Optional text that will display on the button |
| Text Color | Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Text Alignment\* | Left, center \(recommended\) or right |
| Font Bold | If checked, button text is displayed in **bold** |
| Font Italic | If checked, button text is displayed in _italic_ |
| Font Size | Point size for button text |
| Font Typeface\* | Default \(Roboto\), Roboto Regular, Roboto Thin, Sans Serif, Serif, and Monospace. You can upload your own custom font \(.ttf\) |
| Show Feedback | If checked, shows visual feedback for a button with an image displayed |
| Visible | If checked, the button will be visible on the screen. |

\*Can only be set in the Designer



About Screen

Information about the screen. It appears when "About this Application" is selected from the system menu. Use it to tell users about your app. In multiple screen apps, each screen has its own AboutScreen info.

Align Horizontal

A number that encodes how contents of the screen are aligned horizontally. The choices are: 1 = left aligned, 2 = horizontally centered, 3 = right aligned.

Align Vertical

A number that encodes how the contents of the arrangement are aligned vertically. The choices are: 1 = aligned at the top, 2 = vertically centered, 3 = aligned at the bottom. Vertical alignment has no effect if the screen is scrollable.

App Name\* \(designer only\)

This is the display name of the installed application in the phone. If the AppName is blank, it will be set to the name of the project when the project is built.

BackgroundImage

The screen background image.

CloseScreenAnimation

The animation for closing current screen and returning to the previous screen. Valid options are default, fade, zoom, slidehorizontal, slidevertical, and none.

Height

Screen height \(y-size\).

Icon \(designer only\)

OpenScreenAnimation

The animation for switching to another screen. Valid options are default, fade, zoom, slidehorizontal, slidevertical, and none.

ScreenOrientation

The requested screen orientation, specified as a text value. Commonly used values are landscape, portrait, sensor, user and unspecified. See the Android developer documentation for ActivityInfo.Screen\_Orientation for the complete list of possible settings.

Scrollable

When checked, there will be a vertical scrollbar on the screen, and the height of the application can exceed the physical height of the device. When unchecked, the application height is constrained to the height of the device.

ShowStatusBar

The status bar is the topmost bar on the screen. This property reports whether the status bar is visible.

Sizing \(designer only\)

If set to fixed, screen layouts will be created for a single fixed-size screen and autoscaled. If set to responsive, screen layouts will use the actual resolution of the device. See the documentation on responsive design in Thunkable for more information. This property appears on Screen1 only and controls the sizing for all screens in the app.

TitleVisible

The title bar is the top gray bar on the screen. This property reports whether the title bar is visible.

Title

The caption for the form, which appears in the title bar.

VersionCode \(designer only\)

An integer value which must be incremented each time a new Android Application Package File \(APK\) is created for the Google Play Store.

VersionName \(designer only\)

A string which can be changed to allow Google Play Store users to distinguish between different versions of the App.

Width

Screen width \(x-size\).

