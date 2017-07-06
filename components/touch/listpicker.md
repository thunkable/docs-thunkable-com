#### **Thunkable for Android **❤

# ListPicker, ListView, Spinner and CheckBox

---

|  | ListPicker | ListView | Spinner | CheckBox |
| :--- | :--- | :--- | :--- | :--- |
|  | ![](/assets/listpicker-example.png) | ![](/assets/listview-example.png) | ![](/assets/spinner-example.png) | ![](/assets/checkbox-example.png) |
| Common use case | Drop down menus with a **medium number of elements** \(up to 20\) where users select by scrolling | Drop down menus with a **large number of elements **since users can filter through them via search | Drop down menus with a **small number of elements** \(up to 5\) where user options show next to item | Selections of a **single element or multiple elements in a small list** |

---

### ListPicker

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Click | User tapped and releases the button |
| Long Click | User holds the button down |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finger is away from the button, making it no longer possible to click |

BackgroundColor

The color of the listview background.

Elements

List of text elements to build your list.

ElementsFromString

Build a list with a series of text elements separated by commas such as: Cheese,Fruit,Bacon,Radish. Each word before the comma will be an element in the list.

Height

Determines the height of the list on the view.

Selection

Returns the text last selected in the ListView.

SelectionIndex

The index of the currently selected item, starting at 1. If no item is selected, the value will be 0. If an attempt is made to set this to a number less than 1 or greater than the number of items in the ListView, SelectionIndex will be set to 0, and Selection will be set to the empty text.

ShowFilterBar

Sets visibility of ShowFilterBar. True will show the bar, False will hide it.

TextColor

The text color of the listview items.

Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

Width

Determines the width of the list on the view.

• Events

AfterPicking\(\)

Simple event to be raised after the an element has been chosen in the list. The selected element is available in the Selection property.

### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Shape\* | Default \(rectangle\), rounded, rectangular or oval. The shape will not be visible if an Image is being displayed |
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
| Visible | If checked, the button will be visible on the screen |

\*Can only be set in the Designer

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Click | User tapped and releases the button |
| Long Click | User holds the button down |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finger is away from the button, making it no longer possible to click |



