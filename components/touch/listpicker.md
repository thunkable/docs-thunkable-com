#### **Thunkable for Android **❤

# ListPicker, ListView, Spinner and CheckBox

---

|  | [ListPicker](#listpicker) | ListView | Spinner | CheckBox |
| :--- | :--- | :--- | :--- | :--- |
|  | ![](/assets/listpicker-example.png) | ![](/assets/listview-example.png) | ![](/assets/spinner-example.png) | ![](/assets/checkbox-example.png) |
| Common use case | Drop down menus with a **medium number of elements** \(up to 20\) where users select by scrolling | Drop down menus with a **large number of elements **since users can filter through them via search | Drop down menus with a **small number of elements** \(up to 5\) where user options show next to item | Selections of a **single element or multiple elements in a small list** |

---

### ListPicker

---

#### Functionality

| Event / Property | Description |
| :--- | :--- |
| Elements From String | Comma separated list of choices to use. For example apples, oranges, bananas |
| Elements | List of choices to display \(as a list\) |
| Show Filter Bar | If checked, will display a Search Filter Bar above the Listpicker |
| Open | Opens the Listpicker similar to if a user clicked on it |
| Before Picking | Before the list is displayed and can be used to prepare the list before it is shown |
| After Picking | After the user has selected from the list |
| Selection | The selected item |
| Selection Index | The index of the selected item, starting at 1. If no item is selected, the value will be 0 |
| Enabled | If checked, Listpicker functionality is enabled |
| Got Focus | User's finger is over the Listpicker, making it possible to click |
| Lost Focus | User's finger is away from the Listpicker, making it no longer possible to click |

---

### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Shape | Default \(rectangle\), rounded, rectangular or oval. The shape will not be visible if an Image is being displayed |
| Background Color | Background color of the Listpicker button. Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Image | You can upload an image to your app or reference an image url. If an image is uploaded, it will negate the background color and shape properties |
| Title | Optional title that will display at the top of the list |
| Text | Optional text that will display on the ListPicker button |
| Text Color | Text color of the Listpicker button. Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Item Text Color | The text color of the list items. Default \(White\) |
| Item Background Color | The background color of the list items. Default \(Black\) |
| Text Alignment | Left \(recommended\), center or right |
| Font Bold | If checked, Listpicker button text is displayed in **bold** |
| Font Italic | If checked, Listpicker button text is displayed in _italic_ |
| Font Size | Point size for Listpicker button text |
| Font Typeface | Default \(Roboto\), Roboto Regular, Roboto Thin, Sans Serif, Serif, and Monospace. You can upload your own custom font \(.ttf\) |
| Show Feedback | If checked, shows visual feedback for a button with an image displayed |
| Visible | If checked, the Listpicker button will be visible on the screen |



