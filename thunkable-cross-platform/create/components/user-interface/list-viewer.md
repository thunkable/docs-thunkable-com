# List Viewer

* [Add items to a List Viewer](list-viewer.md#add-items-to-a-list-viewer)
* [Select item from a List Viewer](list-viewer.md#select-item-from-a-list-viewer)
* [Style the List Viewer](list-viewer.md#style-the-list-viewer)
* [Edit the List Viewer height](list-viewer.md#edit-the-listviewer-height)
* [Add spacing](list-viewer.md#add-spacing)

![](../../../../.gitbook/assets/list-viewer-fig-1.png)

## Add items to a List Viewer

We recommend adding a short list of items within the app itself as the Screen starts

![](../../../../.gitbook/assets/list-viewer-fig-2.png)

For longer lists, we recommend using the [Spreadsheet](../data/spreadsheet.md) component

![](../../../../.gitbook/assets/list-viewer-fig-3.png)

| Property | Description |
| :--- | :--- |
| Text Items | Default \(`none`\); items must be in list format |

## Select item from a List Viewer

![](../../../../.gitbook/assets/list-viewer-fig-4.png)

| Property | Description |
| :--- | :--- |
| Item Click | Returns an `item` value and a numeric `index` number when an item is selected |

## Style the List Viewer

| Property | Description |
| :--- | :--- |
| Show Arrow | Default \(`true`\); If `true,`shows an arrow with each list item |
| Background Color | Default \(`none`\); Sets the background color of the List Viewer |
| Background Picture | Default \(`none`\); Optional background picture that appears in the List Viewer |

## Edit the ListViewer height

A List Viewer automatically fill 100% of the Screen width

For more information on sizing in your app, please see our [introduction here​](../../intro-to-sizing.md)

| Property | Description |
| :--- | :--- |
| Height | Default \(`Fill container`\); Four options: 1\)`Fit contents`which auto-sizes to the content size or 2\)`Fill container`which auto-sizes to the container 3\)`Relative size`in percent of Screen, 4\)`Absolute size`in pixels |

## Add spacing

For more information on adding spacing in your app, please see our [introduction here](../../intro-to-spacing.md)

To find the spacing properties, you'll have to select the `Advanced` tab

| Property | Description |
| :--- | :--- |
| Margin `Advanced` | Default \(`none`\); Margin is the space outside of the border of a component; You can set space on the `top`, `bottom`, `right` or `left` of the component in both pixels or percent of Screen |
| Padding `Advanced` | Default \(`none`\); Padding is the space between the contents and the border of a component; You can set space on the `top`, `bottom`, `right` or `left` of the component in both pixels or percent of Screen |

