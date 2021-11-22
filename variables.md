# Variables

## What is a Variable?

In app creation, variables work like containers to hold numbers, phrases, the results of a calculation, a database call, or other important values in the app, in the mobile device itself or in the cloud.

Instead of repeating these values in multiple places, a variable can be used wherever it is needed in your Blocks code.

## `App`, `stored` and `cloud` variables

![](.gitbook/assets/screen-shot-2018-10-11-at-12.26.33-pm.png)

When you create a variable, you'll have the choice between an app, stored and cloud variable. All variable types work across screens and the only difference is where they are stored.

### App Variables

An **app** variable works across screens and is stored in the app itself. \
You can save any data type as an app variable.

### Stored Variables

A **stored** variable also works across screens but is saved to the mobile device itself. This means that a stored variable can be retrieved from a previous session. A stored variable is similar to saving a value to [Local Storage](local-storage.md) and is especially useful for retrieving a user's previous setting. If you use stored variables, you no longer need to add Local Storage to your app.

You can save any data type as a stored variable.

### Cloud Variables

A **cloud** variable also works across screens but is saved to the cloud powered by Firebase. \
\
By default, the cloud variable is saved to the Thunkable default Firebase database. We recommend saving them to your own private Firebase DB by [connecting a private Firebase DB to your app](realtime-db.md#set-up-your-own-firebase-account).&#x20;

Cloud variables can be used similar to saving and retrieving values to a [Realtime DB](realtime-db.md) powered by Firebase and can be used in a number of applications that share data across users in the cloud. If you use cloud variables, you no longer need to add a Realtime DB to your app.

#### Cloud Variables and Data

You can only save a piece of [text](text.md) or an [object](objects.md) as a cloud variable.

To save a list as a cloud variable, use the 'make text from list' block to convert the list to a piece of text.

![](.gitbook/assets/screen-shot-2021-04-08-at-11.21.05-am.png)

\
When you retrieve this text from your cloud variable, you can convert it to a list with the 'make list from text' block to work with it as a list in your app.

![](.gitbook/assets/screen-shot-2021-04-08-at-11.21.42-am.png)

To save media as a cloud variable, use the [Cloudinary Media DB](media-db.md) component to upload your audio to the cloud and get a URL that points to it. You can save this URL as a cloud variable.

## Initialize a Variable When the App Starts

![](.gitbook/assets/screen-shot-2018-10-11-at-1.29.35-pm.png)

To create a variable when the app starts, you can grab the block above, select your variable `scope` (app, stored, cloud) and give the variable a `name` like hello. You'll have to connect a block to give app variables an initial value (in the picture above). We recommend placing these blocks in the initial app screen.

## Set a variable during an app event

![](.gitbook/assets/screen-shot-2021-04-08-at-11.14.34-am.png)

You can also set a variable within a block event like the one above. Simply grab the set variable block and connect it to the value that you want it to be set to.

## Retrieving a variable

![](.gitbook/assets/screen-shot-2021-04-08-at-11.15.40-am.png)

Once you have stored a value to your variable, you can retrieve it any time using a block like the one above.



## Updating when the variable initializes or changes

![](.gitbook/assets/screen-shot-2018-12-18-at-11.17.52-pm.png)

Once you have created your variable, you can set it to update when the variable updates in your app.&#x20;

With Cloud variables, this block will also be triggered when the value of the Cloud variable is changed in your Firebase DB. This block replaces the Add.Listener and DataChanged blocks in the Realtime DB.

## Changing a variable

![](.gitbook/assets/screen-shot-2021-04-08-at-11.19.40-am.png)

Variables do not have to be fixed values and there may be times when you want to change your variable automatically like incrementing it by 1 after an event. To do so, grab a block like the one above.

## Dynamically named variables

The above blocks use hard coded variable names, where you must select a variable from a list of variables that you have initialized.

You can also create **dynamically named **variables. There are variables that you create and name during app runtime, which do not have an initialize block.

You can name these by typing in a name, or by using other variables to name the dynamically created variables.

![](.gitbook/assets/screen-shot-2021-04-23-at-8.29.10-am.png)

You can create dynamically named app, stored or cloud variables.
