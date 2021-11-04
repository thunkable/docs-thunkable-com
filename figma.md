# Figma Integration

## Figma Integration

{% hint style="info" %}
Figma integration is a beta feature. We would love any [feedback](https://community.thunkable.com/t/report-bugs-and-submit-feature-requests-in-our-public-github-repository/31760?page=2) you have to give!
{% endhint %}

## Importing a file

You can import a Figma file into your Thunkable project.&#x20;

Click on the Assets tab and click the + icon next to the text **Figma Files**.

![](.gitbook/assets/screen-shot-2021-06-23-at-10.38.24-am.png)

You will be asked to Authenticate with your Figma account. You will only need to do this once.

Paste in the URL of your Figma Project and select a Page in the dropdown menu.&#x20;

{% hint style="info" %}
At the moment, we are only supporting imports for mobile designs at 375x669 px in portrait mode.&#x20;
{% endhint %}

The Figma importer will add all Artboards in a single page, so we recommend creating a designated Page in Figma with the Artboards you intend on importing. &#x20;

![Remember to select the Page you want to import](.gitbook/assets/figma-importmodal.png)

### What gets imported?

Thunkable imports your Figma files in a way that best preserves your original designs.&#x20;

Shapes such as rectangle or a circle will be imported as a shape. You can continue to edit its style within Thunkable. Images and text will be imported as a png. We have done this intentionally to preserve the original font styles. If you want text to be editable, we recommend you replace that image with a Thunkable [label](label.md).&#x20;

![](<.gitbook/assets/figma main screen.png>)

## Updating a file

As you change and update your original designs, keep Thunkable up to date by re-syncing a Screen.

Find your imported Screen name in the Design tab and click the 🔄 icon.

{% hint style="info" %}
There might be a few differences with your Figma file and the output in Thunkable. Re-syncing your Screen with Figma may improve your imported Screen's appearance!
{% endhint %}

![](.gitbook/assets/figma\_refresh.png)

## Blocks

All imported Figma items will have some standard blocks.&#x20;

You can use these imported components as a button by adding a `Click` block. You can also choose to change its background color, or add text or a picture, among other actions.

![ ](<.gitbook/assets/figma component blocks.png>)
