#### **Thunkable Cross-Platform **✕

# Design Template ![](/assets/template-icon.png)

---

**Almost any design that a modern app developer can make is possible on **Thunkable ✕. Below are some of the most common interfaces that you may want to incorporate into your app.

### Popular

A **Scrollable screen** can be made by setting Scrollable to `false` in a Screen to Column. Elements within the Screen or Column have to be sized with heights in absolute pixels which together exceed the height of the Screen or Column. For example, an iPhone 6 has a Screen height of 648 px so elements within it will have to collectively exceed that number for the elements to scroll. We also set the minWidth to `100%` of the Column in the advanced properties so that the scrolling Column does not move from left to right.

#### [Click to copy](https://goo.gl/LErms2)

![](/assets/design-✕-scrollable.gif)

**Swipeable screens** can be made by dropping Screens within a Tab navigator, setting SwipeEnabled to `false` in the Tab propeties and setting TabVisible to `false` in the Screen properties

#### [**Click to copy**](https://goo.gl/5Gr3E6)

### ![](/assets/design-✕-swipeable-screens.gif)

A **Branding screen** can be made setting a Timer to fire after `3000` milliseconds and navigate to the second screen

#### [**Click to copy**](https://goo.gl/sWaWjQ)

![](/assets/design-✕-branding.gif)

