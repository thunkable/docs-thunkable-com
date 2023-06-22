# Layout Component

The Layout component is currently being beta-tested.

## Overview

Thunkable’s Layout component allows for more precise positioning of UI components on an app screen, by allowing you to position UI components dependent on other UI components on the screen. For example, in a typical sign-in screen, if a user inputs an incorrect email address or password, a screen built with a Layout component allows you to shift the UI components on the screen to display the error messaging to the user.&#x20;

## Add a Layout to a Screen

To add a Layout to a screen:

1. Drag and drop the Layout UI component onto a screen. You’ll notice it is composed of two Containers, one on top of the other.&#x20;
2. Click and drag the sizing handles in the corners to resize the Layout UI component.&#x20;
3. Click and drag to reposition it.

<figure><img src=".gitbook/assets/add Layout component gif.gif" alt=""><figcaption></figcaption></figure>

## Insert Additional Containers

By default, a newly added Layout has two horizontal Containers arranged vertically, one on top of the other. To insert additional Containers to a Layout:

1. Click to select the Layout UI component in the component tree or within the screen.
2. At the top of the Layout’s properties panel, select whether you want to insert a Horizontal or Vertical Container.\
   ∙ **Horizontal Container** - UI components within the Container are aligned horizontally, side by side\
   ∙ **Vertical Container** - UI components within the Container are aligned vertically, on top of each other
3. Identify into which Layout or Container you want to insert the new Container.
4. Click **Add**. &#x20;

## Add UI Components

To add UI components to a Layout:

1. Drag and drop UI components into a Container on a screen.&#x20;
2.  Once UI components are in a Container, rearrange their order by dragging and dropping their component names in the component tree.\
    \


    <figure><img src=".gitbook/assets/move components in tree.gif" alt=""><figcaption></figcaption></figure>

## Layout Properties

The following properties are configured on the right in the Layout's properties panel.&#x20;

{% tabs %}
{% tab title="Alignment " %}
| Property                        | Value         | Description                                                                                                                                                                                                                                                      |
| ------------------------------- | ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Direction                       | vertical      | The elements directly within the Layout (could be a UI component or a Container) are aligned vertically, on top of each other.                                                                                                                                   |
| Direction                       | horizontal    | The elements directly within the Layout (could be a UI component or a Container) are aligned horizontally, side by side.                                                                                                                                         |
| Vertical / Horizontal Alignment | top           | The elements directly within the Layout (could be a UI component or a Container) are positioned at the top of the Layout.                                                                                                                                        |
| Vertical / Horizontal Alignment | bottom        | The elements directly within the Layout (could be a UI component or a Container) are positioned at the bottom of the Layout.                                                                                                                                     |
| Vertical / Horizontal Alignment | left          | The elements directly within the Layout (could be a UI component or a Container) are positioned at the left of the Layout.                                                                                                                                       |
| Vertical / Horizontal Alignment | right         | The elements directly within the Layout (could be a UI component or a Container) are positioned at the right of the Layout.                                                                                                                                      |
| Vertical / Horizontal Alignment | center        | The elements directly within the Layout (could be a UI component or a Container) are positioned in the center of the Layout (either top to bottom or left to right, depending on the selected direction).                                                        |
| Vertical / Horizontal Alignment | space-between | The elements directly within the Layout (could be a UI component or a Container) are positioned with an equal amount of space between them.                                                                                                                      |
| Vertical / Horizontal Alignment | space-around  | The elements directly within the Layout (could be a UI component or a Container) are positioned with an equal amount of space between them, including at the top and bottom for a vertical direction Layout or left and right for a horizontal direction Layout. |
| Scrollable                      | true/on       | The user can scroll within the Layout.                                                                                                                                                                                                                           |
| Scrollable                      | false/off     | The user cannot scroll within the Layout.                                                                                                                                                                                                                        |
| Scroll Bar Visible              | true/on       | The scroll bar is visible to the user.                                                                                                                                                                                                                           |
| Scroll Bar Visible              | false/off     | The scroll bar is not visible to the user.                                                                                                                                                                                                                       |

**Horizontal Alignment Examples**

<figure><img src=".gitbook/assets/layout-horizontal alignment-v2.png" alt=""><figcaption></figcaption></figure>

**Vertical Alignment Examples**

<figure><img src=".gitbook/assets/layout-vertical alignment.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Layout" %}
<table><thead><tr><th width="158.66666666666666">Property</th><th width="186">Value</th><th>Description</th></tr></thead><tbody><tr><td>X</td><td>coordinate value</td><td>Position of the upper left corner of the Layout on the X-axis, where the left side of the screen is X=0.</td></tr><tr><td>Y</td><td>coordinate value</td><td>Position of the upper left corner of the Layout on the Y-axis, where the top of the screen is Y=0.</td></tr><tr><td>Height</td><td>number in pixels</td><td>The Layout’s height is defined by a custom number of pixels.</td></tr><tr><td>Width</td><td>number in pixels</td><td>The Layout’s width is defined by a custom number of pixels.</td></tr><tr><td>Resize Mode</td><td>Stretch</td><td>Stretches the Layout to fit the dimensions of the device's screen.</td></tr><tr><td>Resize Mode</td><td>Float in Place</td><td>Renders the Layout in the same aspect ratio as the design, regardless of the device size.</td></tr></tbody></table>
{% endtab %}

{% tab title="Image" %}
| Property                       | Value        | Description                                                                                                         |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------------------------------------------- |
| Background Picture             | Upload files | Click to upload an image file.                                                                                      |
| Background Picture             | Type in URL  | Type in an image URL.                                                                                               |
| Background Picture Resize Mode | cover        | Fills the entire Layout without changing the height and width ratio of the image.                                   |
| Background Picture Resize Mode | contain      | The entire image is scaled down to fit inside the Layout, without changing the height and width ratio of the image. |
| Background Picture Resize Mode | stretch      | The image's height will change to fill the Layout length-wise.                                                      |
| Background Picture Resize Mode | repeat       | The image repeats to cover the Layout. The image's height and width ratio do not change.                            |
| Background Picture Resize Mode | center       | The image is positioned in the middle of the Layout.                                                                |
{% endtab %}

{% tab title="Style" %}
<table><thead><tr><th width="196">Property</th><th width="183.66666666666666">Value</th><th>Description</th></tr></thead><tbody><tr><td>Visible</td><td>visible</td><td>Users can see the Layout.</td></tr><tr><td>Visible</td><td>invisible</td><td>Users cannot see the Layout.</td></tr><tr><td>Background Color</td><td>color</td><td>The background color of the Layout.</td></tr><tr><td>Border: Style</td><td>solid</td><td>The Layout’s border is a solid line.</td></tr><tr><td>Border: Style</td><td>dotted</td><td>The Layout’s border is a dotted line.</td></tr><tr><td>Border: Style</td><td>dashed</td><td>The Layout’s border is a dashed line.</td></tr><tr><td>Border: Color</td><td>color</td><td>The Layout’s border is the color selected. </td></tr><tr><td>Border: Width</td><td>number in pixels</td><td>The width of the Layout’s border is defined by a custom number of pixels.</td></tr><tr><td>Border: Radius</td><td>number in pixels</td><td>The radius of the Layout border’s corners is defined by a custom number of pixels.</td></tr><tr><td>Shadow: Color</td><td>color</td><td>The Layout’s shadow is the color selected. </td></tr><tr><td>Shadow: Opacity</td><td>number between 0 and 100</td><td>The opacity of the Layout’s shadow. </td></tr><tr><td>Shadow: Radius</td><td>number in pixels</td><td>The radius of the Layout shadow’s corners is defined by a custom number of pixels.</td></tr><tr><td>Shadow: Offset</td><td>number in pixels</td><td>How far the Layout’s shadow should be offset, in height and width, is defined by a custom number of pixels.</td></tr></tbody></table>
{% endtab %}

{% tab title="Spacing" %}
<table><thead><tr><th width="166">Property</th><th width="101.66666666666666">Value</th><th>Description</th></tr></thead><tbody><tr><td>Margin</td><td>top</td><td>The margin between the Layout’s top border and the next UI component as defined by a custom number of pixels.</td></tr><tr><td>Margin</td><td>bottom</td><td>The margin between the Layout’s bottom border and the next UI component as defined by a custom number of pixels.</td></tr><tr><td>Margin</td><td>left</td><td>The margin between the Layout’s left border and the next UI component as defined by a custom number of pixels.</td></tr><tr><td>Margin</td><td>right</td><td>The margin between the Layout’s right border and the next UI component as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>top</td><td>The padding between the Layout and its top border as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>bottom</td><td>The padding between the Layout and its bottom border as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>left</td><td>The padding between the Layout and its left border as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>right</td><td>The padding between the Layout and its right border as defined by a custom number of pixels.</td></tr></tbody></table>
{% endtab %}
{% endtabs %}

## Container Properties

The following properties are configured on the right in the Container's properties panel.&#x20;

{% tabs %}
{% tab title="Alignment" %}
<table><thead><tr><th width="212">Property</th><th width="123.66666666666666">Value</th><th>Description</th></tr></thead><tbody><tr><td>Direction</td><td>vertical</td><td>UI components within the Container are aligned vertically, on top of each other.</td></tr><tr><td>Direction</td><td>horizontal</td><td>UI components within the Container are aligned horizontally, side by side.</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>top</td><td>UI components are positioned at the top of the Container</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>bottom</td><td>UI components are positioned at the bottom of the Container</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>left</td><td>UI components are positioned at the left of the Container</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>right</td><td>UI components are positioned at the right of the Container</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>center</td><td>UI components are positioned in the center of the Container (either top to bottom or left to right depending on the selected direction)</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>space-between</td><td>UI components are positioned with an equal amount of space between them</td></tr><tr><td>Vertical / Horizontal Alignment</td><td>space-around</td><td>UI components are positioned with an equal amount of space between them, including at the top and bottom for vertical direction Containers or left and right for horizontal direction Containers</td></tr><tr><td>Scrollable</td><td>true/on</td><td><p>The user can scroll within the Container. </p><p>Note: When setting a Container as scrollable, we recommend the size of the UI components within it are set to an absolute pixel value or Fit Contents.</p></td></tr><tr><td>Scrollable</td><td>false/off</td><td>The user cannot scroll within the Container. </td></tr><tr><td>Scroll Bar Visible</td><td>true/on</td><td>The scroll bar is visible to the user.</td></tr><tr><td>Scroll Bar Visible</td><td>false/off</td><td>The scroll bar is not visible to the user.</td></tr></tbody></table>

**Horizontal Alignment Examples**

<figure><img src=".gitbook/assets/layout-horizontal alignment-v2.png" alt=""><figcaption></figcaption></figure>

**Vertical Alignment Examples**

<figure><img src=".gitbook/assets/layout-vertical alignment.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Layout" %}
<table><thead><tr><th width="128.33333333333334">Property</th><th width="138">Value</th><th>Description</th></tr></thead><tbody><tr><td>Height</td><td>Fit contents</td><td>The Container’s height is the same as the tallest UI component or Container within it (horizontal direction) or the stacked UI components or Containers within it (vertical direction).</td></tr><tr><td>Height</td><td>Fill container</td><td>The elements directly within the Container (could be a UI component or another Container) fill the Container vertically. </td></tr><tr><td>Height</td><td>Size (e.g. 50px or 50%)</td><td>The Container’s height is defined by a custom number of pixels or percentage of the screen.</td></tr><tr><td>Width</td><td>Fit contents</td><td>The Container’s width is the same as the widest UI component or Container within it (vertical direction) or the side-by-side UI components or Containers within it (horizontal direction).</td></tr><tr><td>Width</td><td>Fill container</td><td>The elements directly within the Container (could be a UI component or another Container) fill the Container horizontally. </td></tr><tr><td>Width</td><td>Size (e.g. 50px or 50%)</td><td>The Container’s width is defined by a custom number of pixels or percentage of the screen.</td></tr></tbody></table>
{% endtab %}

{% tab title="Image" %}
| Property                       | Value        | Description                                                                                                         |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------------------------------------------- |
| Background Picture             | Upload files | Click to upload an image file.                                                                                      |
| Background Picture             | Type in URL  | Type in an image URL.                                                                                               |
| Background Picture Resize Mode | cover        | Fills the entire screen without changing the height and width ratio of the image.                                   |
| Background Picture Resize Mode | contain      | The entire image is scaled down to fit inside the screen, without changing the height and width ratio of the image. |
| Background Picture Resize Mode | stretch      | The image's height will change to fill the screen length-wise.                                                      |
| Background Picture Resize Mode | repeat       | The image repeats to cover the screen. The image's height and width ratio do not change.                            |
| Background Picture Resize Mode | center       | The image is positioned in the middle of the frame.                                                                 |
{% endtab %}

{% tab title="Style" %}
<table><thead><tr><th width="191.66666666666666">Property</th><th width="158">Value</th><th>Description</th></tr></thead><tbody><tr><td>Visible</td><td>visible</td><td>Users can see the Container.</td></tr><tr><td>Visible</td><td>invisible</td><td>Users cannot see the Container.</td></tr><tr><td>Background Color</td><td>color</td><td>The background color of the Container.</td></tr><tr><td>Visible</td><td>solid</td><td>The Container’s border is a solid line.</td></tr><tr><td>Visible</td><td>dotted</td><td>The Container’s border is a dotted line.</td></tr><tr><td>Visible</td><td>dashed</td><td>The Container’s border is a dashed line.</td></tr><tr><td>Border: Color</td><td>color</td><td>The Container’s border is the color selected. </td></tr><tr><td>Border: Width</td><td>number in pixels</td><td>The width of the Container’s border is defined by a custom number of pixels.</td></tr><tr><td>Border: Radius</td><td>number in pixels</td><td>The radius of the Container border’s corners is defined by a custom number of pixels.</td></tr><tr><td>Shadow: Color</td><td>color</td><td>The Container’s shadow is the color selected. </td></tr><tr><td>Shadow: Opacity</td><td>number between 0 and 100</td><td>The opacity of the Container’s shadow. </td></tr><tr><td>Shadow: Radius</td><td>number in pixels</td><td>The radius of the Container shadow’s corners is defined by a custom number of pixels.</td></tr><tr><td>Shadow: Offset</td><td>number in pixels</td><td>How far the Container’s shadow should be offset, in height and width, is defined by a custom number of pixels.</td></tr></tbody></table>
{% endtab %}

{% tab title="Spacing" %}
<table><thead><tr><th width="135.66666666666666">Property</th><th width="116">Value</th><th>Description</th></tr></thead><tbody><tr><td>Margin</td><td>top</td><td>The margin between the Container’s top border and the next Container as defined by a custom number of pixels.</td></tr><tr><td>Margin</td><td>bottom</td><td>The margin between the Container’s bottom border and the next Container as defined by a custom number of pixels.</td></tr><tr><td>Margin</td><td>left</td><td>The margin between the Container’s left border and the next Container as defined by a custom number of pixels.</td></tr><tr><td>Margin</td><td>right</td><td>The margin between the Container’s right border and the next Container as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>top</td><td>The padding between the Container and its top border as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>bottom</td><td>The padding between the Container and its bottom border as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>left</td><td>The padding between the Container and its left border as defined by a custom number of pixels.</td></tr><tr><td>Padding</td><td>right</td><td>The padding between the Container and its right border as defined by a custom number of pixels.</td></tr></tbody></table>
{% endtab %}
{% endtabs %}

## Layout Blocks

To access the blocks specific to the Layout component:

1. Navigate to the **Blocks** tab.
2. In the component tree on the left, click the **Layout component**.
3. A drawer of Layout-specific blocks opens.

<table><thead><tr><th width="347">Block Image</th><th>Description</th></tr></thead><tbody><tr><td><img src=".gitbook/assets/Layout scroll to end (frame 470x40x2).png" alt=""></td><td>If the Layout is scrollable, you can use this block to scroll the user to the end of the Layout. For example, a user clicks a button in a chat app, and the Layout scrolls to the end of the chat history to see the most recent messages.</td></tr><tr><td><img src=".gitbook/assets/Layout scroll to start (frame 470x40x2).png" alt=""></td><td>If the Layout is scrollable, you can use this block to scroll the user to the start of the Layout.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s height (frame 470x40x2).png" alt=""></td><td>Sets the Layout’s height to a custom number of pixels.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s height (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s height in pixels.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s computed height (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s computed height, the on-screen dimensions of the Layout, after it has been rendered on-screen. The value returned is an integer, representing the height of the Layout in pixels.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s width (frame 470x40x2).png" alt=""></td><td>Sets the Layout’s width to a custom number of pixels.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s width (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s width in pixels.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s computed width (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s computed width, the on-screen dimensions of the Layout, after it has been rendered on-screen. The value returned is an integer, representing the width of the Layout in pixels.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s visible (frame 470x40x2).png" alt=""></td><td><p>When set to true, sets the Layout to visible, meaning the Layout is visible to users.</p><p>When set to false, sets the Layout to invisible, meaning the Layout is not visible to users.</p></td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s visible (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s visibility status. Returns true (visible) or false (invisible).</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s X (frame 470x40x2).png" alt=""></td><td>Set the position of the upper left corner of the Layout on the X-axis, where the left side of the screen is X=0.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s X (frame 470x40x2).png" alt=""></td><td>Get the position of the upper left corner of the Layout on the X-axis, where the left side of the screen is X=0.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s Y (frame 470x40x2).png" alt=""></td><td>Set the position of the upper left corner of the Layout on the Y-axis, where the top of the screen is Y=0.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s Y (frame 470x40x2).png" alt=""></td><td>Get the position of the upper left corner of the Layout on the Y-axis, where the top of the screen is Y=0.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s background color (frame 470x40x2).png" alt=""></td><td>Set the Layout’s background color.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s background color (frame 470x40x2).png" alt=""></td><td>Get the Layout’s background color.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s background picture (frame 470x40x2).png" alt=""></td><td>Set the Layout's background picture. Click the dropdown menu to select an image from your computer.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s background picture (frame 470x40x2).png" alt=""></td><td>Get the Layout's background picture.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s background picture resize (frame 470x40x2).png" alt=""></td><td>Set the Layout’s background picture resize mode. See the Layout Properties section for definitions of the acceptable values.</td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s background picture resize (frame 470x40x2).png" alt=""></td><td>Get the Layout’s background picture resize mode.</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s scrollable (frame 470x40x2).png" alt=""></td><td><p>When set to true, sets the Layout to scrollable for users.</p><p>When set to false, sets the Layout to scrollable for users.</p></td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s scrollable (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s scrollable status. Returns true (scrollable) or false (not scrollable).</td></tr><tr><td><img src=".gitbook/assets/set Layout&#x27;s scroll bar visible (frame 470x40x2).png" alt=""></td><td><p>When set to true, sets the Layout’s scroll bar to visible for users.</p><p>When set to false, sets the Layout’s scroll bar to invisible for users.</p></td></tr><tr><td><img src=".gitbook/assets/get Layout&#x27;s scroll bar visible (frame 470x40x2).png" alt=""></td><td>Gets the Layout’s scroll bar visibility status. Returns true (visible) or false (invisible).</td></tr></tbody></table>

## Container Blocks

To access the blocks specific to the Container component:

1. Navigate to the **Blocks** tab.
2. In the component tree on the left, click the **Container component** that is nested under the Layout component.
3. A drawer of Container-specific blocks opens.
4. The blocks are the same as the ones above in the [Layout Blocks section](layout.md#7.-layout-blocks), but specific to the Container instead of the Layout.

## Create a Custom Data Viewer&#x20;

Thunkable provides a variety of default [Data Viewer List](data-viewer-list.md) and [Data Viewer Grid](data-viewer-grid.md) templates, but saving a customized Layout component as a Data Viewer allows you to display your data in a way that reflects your brand design and preferences.&#x20;

### To save a Layout as a Data Viewer:

1. When you're happy with the Layout you have customized, ensure it is selected in the component tree.
2. Click the **vertical ellipsis** next to the Layout's name in the properties panel.
3.  Select **Save as Data Viewer Layout**.\


    <div align="left">

    <figure><img src=".gitbook/assets/Layout - Save as Data Viewer Layout.png" alt="" width="563"><figcaption></figcaption></figure>

    </div>
4. Give your Data Viewer Layout a detailed **name**.
5. Select the **Layout Type** you want to create. \
   \- List for a Data Viewer List\
   \- Grid for a Data Viewer List.
6. Click **OK**.

### To use a saved Layout as a Data Viewer:

1. Click the **Create New Screen** icon at the top of the component tree in the Designer. &#x20;
2. Drag a **Data Viewer Lis**t or **Data Viewer Grid** onto your screen.
3. Reposition and resize as necessary.
4. Connect you project to a data source. See here for instructions on connecting a data source: [Data Sources](data-sources.md).
5.  Click the sample template to access the Data Viewer templates available to you.\


    <div align="left">

    <figure><img src=".gitbook/assets/Data Viewer List - properties panel - design template.png" alt="" width="290"><figcaption></figcaption></figure>

    </div>
6. Click to select the Layout you saved as a Data Viewer from the bottom of the template library.&#x20;
7.  Map your data source columns to components within your custom Data Viewer Layout. \


    <div align="left">

    <figure><img src=".gitbook/assets/Data Viewer - properites panel - map column data.png" alt="" width="279"><figcaption></figcaption></figure>

    </div>

See here for more on working with Data Viewers and Data Sources: [Data Viewers and Data Sources](data-viewers.md).
