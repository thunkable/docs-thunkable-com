---
description: >-
  Layout components allow you to organize your screen into a more readable and
  navigable interface
---

# Layout

####  ![](../../../.gitbook/assets/hor-arrange-icon%20%281%29.png)  ![](../../../.gitbook/assets/ver-arrange-icon.png)  ![](../../../.gitbook/assets/table-arrange-icon%20%282%29.png)

Vertical arrangements are often used as a substitute for screens by turning their visibility to 'true' and 'false'. Horizontal arrangements are often used for arranging content that goes across the screen like a top navigation menu or for creating padding on a screen \(empty labels can also be used\). Scrollable arrangements can be useful for apps where there is a lot of content like images that you may not fit within a fixed space. Table arrangements are useful when the content should be spaced consistently like in a bottom tabbed menu

The sample app [Thunkableagram: AI-powered Instagram](layout.md) uses all of these types of arrangements

|  | ![](../../../.gitbook/assets/ver-arrange-icon%20%281%29.png) | ![](../../../.gitbook/assets/hor-arrange-icon.png) |  | ![](../../../.gitbook/assets/table-arrange-icon%20%281%29.png) |
| :--- | :--- | :--- | :--- | :--- |
| Component | Vertical Arrangement | Horizontal Arrangement | Vertical or Horizontal Scroll Arrangement | Table Arrangement |
| Common use case | Screen substitute | Top navigation menu or padding | Scrollable vertical content | Bottom tabbed menu |

#### Pro-tip: Vertical arrangements as Screen substitutes

Screens are natural ways to organize an app but they have two limitations that make Vertical \(or Horizontal\) Arrangements a good substitute:

* The maximum screen limit is 10 on Thunkable
* They do not allow passing more than one value between screens

To use Vertical Arrangements as screens:

1. Add a Vertical Arrangement
2. Set the Height and Width to 'Fill Parent'
3. Set the Visible property to 'true' or 'false' depending on the event

![](../../../.gitbook/assets/screen-shot-2017-07-14-at-3.23.32-pm.png)

### **Vertical, Horizontal or Scroll Arrangements** ![](../../../.gitbook/assets/ver-arrange-icon%20%282%29.png)![](../../../.gitbook/assets/hor-arrange-icon%20%282%29.png)

#### Appearance

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill'. For most cases, we recommend setting to 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill'. For most cases, we recommend setting to 'Automatic' or 'Fill' |
| Align Horizontal | 'Center' \(default\), 'Left, 'Right' |
| Align Vertical | 'Top' \(default\), 'Center', 'Bottom' |
| Background Color | Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks edito |
| Image | You can upload an image to your app or reference an image url. If an image is uploaded, it will negate the background color |
| Visible | If checked, arrangement will be visible |

### Table Arrangement ![](../../../.gitbook/assets/table-arrange-icon.png)

#### Appearance

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill'. For most cases, we recommend setting to 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill'. For most cases, we recommend setting to 'Automatic' or 'Fill' |
| Columns | Number of columns |
| Rows | Number of rows |
| Visible | If checked, arrangement will be visible |

