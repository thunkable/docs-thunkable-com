---
description: Create interactive gaming apps with the canvas component.
---

# Canvas

The canvas component is a touch-sensitive panel that enables the movement of items. 

You can use this component to create a variety of games and experiences that involve different methods of touching a screen.

* [Adding a Canvas](canvas.md#adding-a-canvas)
* [The Stage](canvas.md#the-stage)
  * [Gravity](canvas.md#gravity)
  * [Touch Drawing](canvas.md#touch-drawing)

## Adding a Canvas 

To add a canvas to your app, drag and drop the canvas component into the app builder. 

When you click on the Canvas in your component tree, Canvas tab will appear. Click on this tab to customize your canvas

![Screenshot of Canvas tab in your Thunkable project editor](.gitbook/assets/canvastab.png)

The three elements of a Canvas are the **Stage,** the **Sprites**, and the **Canvas Label**.

## The Stage

The Stage is the background of your Canvas. You can set a background color or background picture, a border color, and the stage's Height and Width. You can click and drag your **Sprites** on the stage in the Canvas tab.

### Gravity

You can set **Gravity** of the Stage along the X and Y axis. The Sprites on the stage can be toggled to **ignore** gravity or not. If a Sprite is affected by gravity, it will be pulled in the direction of the gravity. 

{% tabs %}
{% tab title="Y Gravity" %}
![Behavior of Sprite when Y Gravity = 100, X Gravity = 0](.gitbook/assets/y-axis-gravity.gif)
{% endtab %}

{% tab title="X Gravity" %}
![Behavior of Sprite when Y Gravity = 0, X Gravity = 100](.gitbook/assets/x-axis-gravity.gif)
{% endtab %}

{% tab title="Y and X Gravity" %}
![Behavior of Sprite when Y Gravity = 100, X Gravity = 100](.gitbook/assets/x-y-axis-gravity-1-.gif)
{% endtab %}
{% endtabs %}

### Touch Drawing

You can enable **Touch Drawing** on your Screen.   
You can set the **Drawing Color** to choose the color you draw in.   
You can set the **Drawing Width** to choose the thickness of the line you draw on the stage.

### Multiple Stages

You can add multiple stages to a Canvas component, in the same way you can add multiple Screens to an app project. when you have selected your Canvas tab, click on the + next to your Stage name to add another Stage to the Canvas.

![](.gitbook/assets/addstage.png)

Each Stage has its own Sprites, background color, gravity, etc. 

