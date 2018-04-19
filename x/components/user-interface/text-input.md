#### **Thunkable Cross-Platform **✕

# Text Input ![](/assets/iOSviewIconTextInput.png)

---

The Text Input component allows users to enter text as an input into an app, for anything from filling out forms to passwords

* [Set up](#set-up)
* [Style the Text Input](#style-the-text-input)
* [Edit size](#edit-size)
* [Add spacing](#add-spacing)

![](/assets/text-input-✕-fig-1.png)

---

### Set up

You can customize the Text Input to display the standard keyboard or to have it accept email addresses \(shown on Android phone on left\) or numbers \(shown on the iOS phone on the right\)

![](/assets/text-input-✕-fig-2.png)

| Property | Description |
| :--- | :--- |
| Keyboard Type | Default \(`default`\); default is the default keyboard installed on the phone; numeric accepts numbers and is similar to `phone-pad`; `email-address` is customized to accept email addresses |

You can also set up Text Input for passwords as shown below

![](/assets/text-input-✕-fig-3.png)

| Property | Description |
| :--- | :--- |
| Secure Text Entry `Advanced` | Default \(`false`\); If true, replaces text with \* as users type |

---

### Style the Text Input

| Property | Description |
| :--- | :--- |
| Hint | Default \(`Type Here`\); Optional hint text that disappears when the user starts typing into the Text Input |
| Text | Default \(`none`\); Optional text that first appears in the Text Input |
| Color | Default \(`#007AFF`\); Color of the text that users type |
| Font Bold | Default \(`false`\); If `true`, text font will be **bold** |
| Font Italic | Default \(`false`\);  If `true`, text font will be _italic_ |
| Font Size | Default \(`14`\); Size of the text that users type |
| Background Color | Default \(`none`\); Sets the background color of the text box |
| Border | Default \(`none`\); You can set the `width`, `color` and `style` of the border around the Text Input box. On iOS, bordersor background colors can be useful to make the Text Input box more visible |
| Underline Color Android `Advanced` | Default \(`none`\); Sets the underline color of the Text Input on Android |

---

### Edit size

| Property | Description |
| :--- | :--- |
| Height | Default \(`Fit contents`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |
| Width | Default \(`80%`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |

---

### Add spacing

For more information on adding spacing in your app, please see our [introduction here](/x/create/intro-spacing.md)

To find the spacing properties, you'll have to select the `Advanced` tab

| Property | Description |
| :--- | :--- |
| Margin | Default \(`none`\); Margin is the space outside of the border of a component; You can set space on the `top`, `bottom`, `right` or `left` of the component in both pixels or percent of Screen |
| Padding | Default \(`none`\); Padding is the space between the contents and the border of a component; You can set space on the `top`, `bottom`, `right` or `left` of the component in both pixels or percent of Screen |



