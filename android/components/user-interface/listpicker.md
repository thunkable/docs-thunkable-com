#### **Thunkable for Android **❤

# ListPicker ![](/assets/listpicker-icon.png) + ListView ![](/assets/listview-icon.png) +  Spinner ![](/assets/spinner-icon.png)  + CheckBox ![](/assets/checkbox-icon.png)

---

|  | ![](/assets/listpicker-icon.png) | ![](/assets/listview-icon.png) | ![](/assets/spinner-icon.png) | ![](/assets/checkbox-icon.png) |
| :--- | :--- | :--- | :--- | :--- |
|  | [ListPicker](#listpicker) | [ListView](#listview) | [Spinner](#spinner) | [CheckBox](#checkbox) |
|  | ![](/assets/listpicker-example.png) | ![](/assets/listview-example.png) | ![](/assets/spinner-example.png) | ![](/assets/checkbox-example.png) |
| Common use case | Drop down menus with a **medium number** of elements users can select by scrolling or searching. **Opens in a new screen** | Drop down menus with a **medium number** of elements users can select by searching in the current screen | Drop down menus with a **small number **of elements \(up to 5\) where user options show next to filter in the current screen | Selections of a **single element or multiple elements **in a small list in the current screen |

---

### ListPicker ![](/assets/listpicker-icon.png) {#listpicker}

The Listpicker is a popular choice for drop down menus with more than 5 choices since the list itself opens in a new screen. A searchable filter bar is also available to make selection in long lists even easier for users.

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

#### **Appearance**

There are two elements to a ListPicker, a button that opens the ListPicker and the ListPicker itself

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Shape | Default \(rectangle\), rounded, rectangular or oval. The shape will not be visible if an Image is being displayed |
| Background Color | Background color of the button. Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Image | You can upload an image to your app or reference an image url for the button. If an image is uploaded, it will negate the background color and shape properties |
| Title | Optional title that will display at the top of the list |
| Text | Optional text that will display on the button |
| Text Color | Text color of the button. Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Item Text Color | The text color of the list items. Default \(White\) |
| Item Background Color | The background color of the list items. Default \(Black\) |
| Text Alignment | Left \(recommended\), center or right |
| Font Bold | If checked, button text is displayed in **bold** |
| Font Italic | If checked, button text is displayed in _italic_ |
| Font Size | Point size for button text |
| Font Typeface | Default \(Roboto\), Roboto Regular, Roboto Thin, Sans Serif, Serif, and Monospace. You can upload your own custom font \(.ttf\) |
| Show Feedback | If checked, shows visual feedback for a button with an image displayed |
| Visible | If checked, the button will be visible on the screen |

---

### ListView ![](/assets/listview-icon.png) {#listview}

The ListView is a less customizable but also simpler drop down menu that can be displayed on the user's current screen

---

#### Functionality

| Event / Property | Description |
| :--- | :--- |
| Elements From String | Comma separated list of choices to use. For example apples, oranges, bananas |
| Elements | List of choices to display \(as a list\) |
| Show Filter Bar | If checked, will display a Search Filter Bar above the Listpicker |
| After Picking | After the user has selected from the list |
| Selection | The selected item |
| Selection Index | The index of the selected item, starting at 1. If no item is selected, the value will be 0 |

---

#### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Background Color | Background color of the list. Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Text Color | Text color of the list. Default \(White\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Visible | If checked, the Listpicker button will be visible on the screen |

---

### Spinner ![](/assets/spinner-icon.png) {#spinner}

The Spinner is a great drop down menu option for shorter lists

---

#### Creating an initial list for the spinner

![](/assets/spinner-blocks-1.png)

---

#### Functionality

| Event / Property | Description |
| :--- | :--- |
| Elements From String | Comma separated list of choices to use. For example apples, oranges, bananas |
| Elements | List of choices to display \(as a list\) |
| After Picking | After the user has selected from the list |
| Selection | The selected item |
| Selection Index | The index of the selected item, starting at 1. If no item is selected, the value will be 0 |
| Display Dropdown | Displays the dropdown list similar to when user clicks on spinner |

---

#### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Prompt | Text to display for the Spinner window |
| Visible | If checked, the Listpicker button will be visible on the screen |

---

### CheckBox ![](/assets/checkbox-icon.png) {#checkbox}

The CheckBox is the simplest of menus because it has a single element that can be selected \(or unselected\)

---

#### Functionality

| Event / Property | Description |
| :--- | :--- |
| Checked | If checked, the element is selected |
| Click | User taps and releases the CheckBox |
| Enabled | If checked, CheckBox functionality is enabled |
| Got Focus | User's finger is over the CheckBox, making it possible to click |
| Lost Focus | User's finger is away from the CheckBox, making it no longer possible to click |

---

#### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Text | Text to display next to the CheckBox. |
| Text Color | Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Outline Color | Default \(Material Light Green\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Visible | If checked, the Listpicker button will be visible on the screen |



