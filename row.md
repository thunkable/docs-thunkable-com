---
description: >-
  A row is horizontal container that allows you to position components side by
  side.
---

# Row

* [Set the size of the row](row.md#set-size-of-the-row)
* [Space the elements horizontally](row.md#space-the-elements-horizontally)
* [Space the elements vertically](row.md#space-the-elements-vertically)
* [Add a background color or picture](row.md#add-a-background-color-or-picture)

![](.gitbook/assets/row-fig-1.png)

## **Set the size of the row**

**For more information on sizing in your app, please see our introduction here​**  


<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Property</b>
      </th>
      <th style="text-align:left"><b>Description</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Height</td>
      <td style="text-align:left">
        <ul>
          <li>Fill container - The row fills the entire screen vertically</li>
          <li>Fit contents - The row&#x2019;s height changes to fit the components it
            contains</li>
          <li>Relative size - The row fills the specified percentage of the screen</li>
          <li>Absolute size - Sizes the row to a specified number of pixels</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Width</td>
      <td style="text-align:left">
        <ul>
          <li>Fill container - The row fills the entire screen horizontally</li>
          <li>Fit contents - The row&#x2019;s width changes to fit the components it
            contains</li>
          <li>Relative size - The row fills the specified percentage of the screen</li>
          <li>Absolute - Sizes the row to a specified number of pixels</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Space the elements horizontally

The `Horizontal Alignment` property allows you to space elements in a Row horizontally

![](.gitbook/assets/image%20%2862%29.png)

![](.gitbook/assets/thunkable-documentation-exhibits-64.png)

## Space the elements vertically

The `Vertical Alignment` property allows you to space elements in a Row vertically

![](.gitbook/assets/spacing-fig-2.png)

## Add a background color or picture

| Property | Description |
| :--- | :--- |
| Background Color | Default \(`none`\). Select any color using the color picker, RGBA or HEX value |
| Background Picture | You can upload a background image to your app or reference an image url e.g.`beaver-yellow.png` |
|  |  |

**Background Picture Resize Mode** 

* Cover: Fills the entire screen without changing the height and width ratio of the image 
* Contain: The entire image will be scaled down to fit inside the screen, without changing the height and width ratio of the image 
* Stretch: The image's height will change to fill the screen length-wise 
* Repeat: Repeat the image to cover the screen. The image's height and width ratio

   will not change    

* Center: Positions the image in the middle of the frame

