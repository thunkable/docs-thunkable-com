# Group

A Group is a container component.

You can place [User Interface](ui-components.md) components inside a Group to make changing the appearance of your app easier.

## Add Components to Group

To add components to a Group, simply drag and drop the components inside the Group.

You will see the components you added to the Group are now nestled inside the Group in the component tree.

## Moving Groups in Your Project

When a group that contains UI Component(s) is moved, its content are moved with it as a unit.

This makes it easier to design complex layouts.

## Properties

### Layout

| Property    | Description                                                                         | Data Type                                                   |
| ----------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| Position    | Set whether the Group is positioned Relative to the Screen or Relative to Device ¹  | Select from menu: \[Relative to Screen, Relative to Device] |
| Height      | Height of Group in pixels                                                           | Number                                                      |
| Width       | Width of Group in pixels                                                            | Number                                                      |
| X           | Position of top left corner of Group on X-axis                                      | Number                                                      |
| Y           | Position of top left corner of Group on Y-axis                                      | Number                                                      |
| Visible     | Set whether Group is shown on screen                                                | True/False                                                  |
| Resize Mode | Set how Group is resized on wider screens - Stretch or Float in Place ²             | Select from menu: \[Resize, Float in Place]                 |

¹ Relative to Screen: Group moves as end user scrolls\
Relative to Device: Group stays in place as end user scrolls

² Stretch: Resize Group in proportion with wider Screen\
Float in Place: Keep same dimensions for Group on larger screens

### Image

| Property                       | Description                                                                                         | Data Type                                                                                                                                                                                                    |
| ------------------------------ | --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Background Picture             | The image file to be shown in the Image component                                                   | <p>PNG, JPG, GIF, SVG, etc.<br>Can also use URL that ends in file extension (eg <a href="https://thunkable.com/static/media/logo.ba96eb83.png">https://thunkable.com/static/media/logo.ba96eb83.png</a>)</p> |
| Background Picture Resize Mode | Set how picture is shown if the file and the Image component have different dimensions/aspect ratio | Select from list `[cover, contain, stretch, repeat, center]`                                                                                                                                                 |

### Style

| Property         | Description                                                             | Data Type                                  |
| ---------------- | ----------------------------------------------------------------------- | ------------------------------------------ |
| Background Color | Color of Group's background                                             | Color                                      |
| Border Width     | Width of Group's border in pixels                                       | Number                                     |
| Border Radius    | Radius of corners of Group's border in pixels                           | Number                                     |
| Border Color     | Color of Group's border                                                 | Color                                      |
| Border Style     | Style of Group's border                                                 | Select from list `[solid, dotted, dashed]` |
| Shadow Color     | Color of Group's shadow                                                 | Color                                      |
| Shadow Opacity   | Opacity of Group's shadow                                               | Number between 0 and 100                   |
| Shadow Radius    | Radius of corners of Group's shadow in pixels                           | Number                                     |
| Shadow Offset    | How far Group's shadow should be offset, in Height and Width, in pixels | Number                                     |
| Touch Opacity    | Set opacity of Group when user clicks on Group                          | Number between 0-100                       |

## Blocks

### Events

You can use the following blocks to listen for when a specific event occurs

#### Click

Performs an action when the user taps the Group.

### Properties

Set and get the [properties](group.md#properties) of the Group.

#### Background Color

Set and get the Background Color of the Group.

#### Background Picture

Set and get the Background Picture of the Group.

#### Background Picture Resize Mode

Set and get the Background Picture Resize Mode of the Group.

#### Computed Height

Get the height of the of the Group as it appears in-screen in pixels.

#### Visible

Set and get the Visible property of the Group.

#### Computed Width

Get the width of the of the Group as it appears in-screen in pixels.

