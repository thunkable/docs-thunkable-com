#### **Thunkable for Android **❤

# App Limits

---

| Element | Limit |
| :--- | :--- |
| App size | 10 MB |
| App icon size | 96 x 96 px \(recommended\) |
| Screens | Up to 10 \(recommended\)\* |

\*Thunkable will not prevent you from creating an app with more than 10 screens.  But be aware that if you do that, you are in danger of exceeding the processing and memory limitations of many Android devices as well as your browser.   The precise limits depend on several different factors such as the size of your app, the storage taken up by sounds and images, the speed of your network connection, and the configuration of your Web browser.  But as you keep adding screens, you’ll run across one or more of these factors, and the consequences could be very unpleasant.  This could include the Blocks editor running more and more slowly, and the inability of Thunkable to build your project.  In extreme cases, you could exceed the capacity of App Inventor to save or load your project: you would be stuck with no way to view or even fix your project and you’d have to ask for help on the forum, and even the people there might be unable to help.

If you’re building an app with more than 10 screens, save your project \(aia file\) to your local computer -- not just the Thunkable server -- each time you make a significant change.   It’s a good idea to save the versions of the project under different names, like MyAppV1, MyAppV2, and so on.   That way, if you do run into a problem, you have a history of versions to examine.  Be especially careful if you add a lot of screens to a project at once.  That’s a likely time to run into problems.

Making a series of backups like this is a good idea, not only in the case of multiple screens, but any time you are working on large and complex projects.   There is always a risk of losing your work, and it’s worth the effort to make backups as a precaution.

---

#### Most common causes of apps not building or crashes

* [Extensions](/Android/extensions.md)
  * Extensions are created by the community and many of them work wonderfully on Thunkable.  A few of them do lead to more frequent app crashes
* Images
  * App icon too large \(we recommend 96 px by 96 px\)
  * Too many / too large images \(the app size limit is 10MB\)
  * Some users have detected that Thunkable works better with .pngs than .jpgs
* Too many screens \(there is not a hard limit on 10 screens but performance reduces beyond that\)
* Blocks
  * Errors in blocks \(usually this will prevent the app from building\)
  * Too many blocks \(we have seen a few cases where a lot of blocks create performance issues\)



