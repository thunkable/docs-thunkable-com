#### **Thunkable for iOS **

# Screen

---

Screens are the pages of an app. We designed Thunkable for iOS to support simple one screen apps and complex, multi-screen apps which take advantage of a new component in Thunkable called [Navigators](/ios/components/navigators/README.md), which manage how multiple Screens of an app are linked together

* [Add a Screen](#add-a-screen)
* [Add multiple Screens under a Navigator](#add-multiple-screens-under-a-navigator)
* [Edit appearance of Screens within a Navigator](#edit-appearance-of-screens-within-a-navigator)

---

#### Add a screen

![](/assets/add-screen-ios-1.gif)

---

#### **Add multiple screens under a Navigator**

![](/assets/multi-screen-ios-1.gif)

---

#### Edit appearance of Screens within a Navigator

##### Drawer Navigator

| Property | Description |
| :--- | :--- |
| Title | Title of the Screen; serves as the visible label of the Drawer if the 'drawer label' is blank |
| Drawer Label | Title of the visible label of the Drawer |

##### Tab Navigator

| Property | Description |
| :--- | :--- |
| Title | Title of the Screen; serves as the visible label of the Tab if the 'tab bar label' is blank |
| Tab Bar Label | Title of the visible label on the Tab bar |
| Tab Bar Visible | If `false`, hides the Screen from the Tab bar |

##### Stack Navigator

| Properties | Description |
| :--- | :--- |
| Title | Title of the Screen; serves as the visible header of the Screen if 'header title' is blank |
| Header Title | Title of the visible header on the Screen |
| Header Back Title |  |
| Header Truncated Back Title |  |
| Header Tint Color | Color of the text in the header |
| Gestures Enabled | If `true`, you can use gestures to dismiss the Screen |



