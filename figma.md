# Figma Integration

## Figma Integration

{% hint style="info" %}
Figma integration is a beta feature, so there will be some bugs and snags as you use it. We would love any [feedback](https://community.thunkable.com/t/report-bugs-and-submit-feature-requests-in-our-public-github-repository/31760?page=2) you have to give!
{% endhint %}

## Importing a file

You can import a Figma file into your Thunkable project. 

Click on the Assets tab and click the + icon next to the text **Figma Files**.

![](.gitbook/assets/screen-shot-2021-06-23-at-10.38.24-am.png)

You will be asked to Authenticate with your Figma account. Follow the steps. You will only need to do this once.

Paste in the URL of your Figma Project and select a Page in the dropdown menu. 

{% hint style="info" %}
At the moment, we are only supporting imports for mobile designs at 375x669 px in portrait mode. 
{% endhint %}

The Figma importer will add all Artboards in a single page, so we recommend creating a separate Page in Figma with the Artboards you intend on importing.  

![Remember to select the Page you want to import](.gitbook/assets/figma-importmodal.png)

### What gets imported?

Thunkable will recognize imported items as either Figma components or Groups. 

A Figma component will allow us to know that it has been imported and will be recognized when a file is re-synced when the original Figma file is updated. Figma components can be recognized as either a Text component or a Vector component. 

![](.gitbook/assets/figma-imported.png)

![](.gitbook/assets/figma-blocks%20%281%29.png)

## Updating a file

As you change and update your original designs, keep Thunkable up to date by re-syncing a Screen.

{% hint style="info" %}
There might be a few differences with your Figma file and the output in Thunkable. Re-syncing your Screen with Figma may improve your imported Screen's appearance!
{% endhint %}

![](.gitbook/assets/figma-sync.png)

## Blocks

Imported Figma components have basic Blocks available. 

![](.gitbook/assets/figma-blocks.png)

