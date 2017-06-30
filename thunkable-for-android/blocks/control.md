#### **Thunkable for Android **❤

# Blocks: Control

---

Control blocks are frequently used blocks for _adding conditions or logic on when an event happens_ i.e. if this, then and _navigating between screens_

### Popular block snippets

Opens a new screen after button is clicked

---

### Control block types

**Conditional and logic operators for events**

* [if & if else](#if)
* [for each from to](#for-each-from-to)
* [for each in list](#for-each-in-list)
* [while](#while)
* [do](#do-this)
* [evaluate but ignore result](#evaluate-but-ignore)

**Screen navigation**

* [open another screen](#open-screen)
* [open another screen with start value](#open-screen-value)
* [get start value](#get-start-value)
* [close screen](#close-screen)
* [close screen with value](#close-screen-value)
* [close application](#close-app)
* [get plain start text](#get-plain-start-text)
* [close screen with plain text](/close screen with plain text)

---

### if & if else {#if}

![](https://thunkable.com/explore/img/blocks/control/if.png)

Tests a given condition. If the condition is true, performs the actions in a given sequence of blocks; otherwise, the blocks are ignored.

![](https://thunkable.com/explore/img/blocks/control/ifelse.png)

Tests a given condition. If the result is true, performs the actions in the -do sequence of blocks; otherwise, performs the actions in the -else sequence of blocks.

![](https://thunkable.com/explore/img/blocks/control/ifelseif.png)

Tests a given condition. If the result is true, performs the actions in the -do sequence of blocks; otherwise tests the statement in the -else if section. If the result is true, performs the actions in the -do sequence of blocks; otherwise, performs the actions in the -else sequence of blocks.

### for each from to {#for-each-from-to}

![](https://thunkable.com/explore/img/blocks/control/forrange.png)

Great for loops, or repetitions of events. Runs the blocks in the do section for each numeric value in the range and incrementing by a certain range. You can change the `number` to something else if you wish.

### for each in list {#for-each-in-list}

![](https://thunkable.com/explore/img/blocks/control/foreach.png)

Great for loops, or repetitions of events.  Runs the blocks in the do section for each item in the list. You can change the `item` to something else if you wish.

### while {#while}

![](https://thunkable.com/explore/img/blocks/control/while.png)

Tests the -test condition. If true, performs the action given in -do , then tests again. When test is false, the block ends and the action given in -do is no longer performed.

### do {#do-this}

![](https://thunkable.com/explore/img/blocks/control/doreturn.png)

Sometimes in a procedure or another block of code, you may need to do something and return something, but for various reasons you may choose to use this block instead of creating a new procedure.

### evaluate but ignore result {#evaluate-but-ignore}

![](https://thunkable.com/explore/img/blocks/control/evaluate.png)

Use this block when trying to trigger an event but the blocks may not seem to fit together.

Provides a "dummy socket" for fitting a block that has a plug on its left into a place where there is no socket, such as one of the sequence of blocks in the do part of a procedure or an if block. The block you fit in will be run, but its returned result will be ignored. This can be useful if you define a procedure that returns a result, but want to call it in a context that does not accept a result.

### open another screen {#open-screen}

![](https://thunkable.com/explore/img/blocks/control/openscreen.png)

Opens the screen with the provided name.

### open another screen with start value {#open-screen-value}

![](https://thunkable.com/explore/img/blocks/control/openscreenwithvalue.png)

Opens another screen and passes a value to it.

### get start value {#get-start-value}

![](https://thunkable.com/explore/img/blocks/control/getstartvalue.png)

Returns the start value given to the current screen.This value is given from using open another screen with start value or close screen with value

### close screen {#close-screen}

![](https://thunkable.com/explore/img/blocks/control/closescreen.png)

Closes the current screen

### close screen with value {#close-screen-value}

![](https://thunkable.com/explore/img/blocks/control/closescreenwithvalue.png)

Closes the current screen and returns a value to the screen that opened this one

### close application {#close-app}

![](https://thunkable.com/explore/img/blocks/control/closeapp.png)

Closes the application

### get plain start text {#get-plain-start-text}

![](https://thunkable.com/explore/img/blocks/control/getplainstarttext.png)

Returns the plain text that was passed to this screen when it was started by another app. If no value was passed, it returns the empty text. For multiple screen apps, use get start value rather than get plain start text

### close screen with plain text {#close-screen-with-plain-text}

![](https://thunkable.com/explore/img/blocks/control/closescreenwithplaintext.png)

Closes the current screen and passes text to the app that opened this one. This command is for returning text to non-Thunkable activities, not to Thunkable screens. For Thunkable Screens, as in multiple screen apps, use Close Screen with Value, not Close Screen with Plain Text.

