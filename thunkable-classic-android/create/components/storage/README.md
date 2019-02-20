# Storage

Deciding on which storage option can be complex but the key things to consider are i\) the file types you want to store and retrieve, ii\) the amount of data and iii\) the amount of security you want to have on that data. Since most data for your app should be secured, there is often some set up required to use these components.

At Thunkable, we particularly love data storage options like Firebase that require little set-up to get started but provide the option of security once you have your app working.

### Data Storage

|  | ![](../../../../.gitbook/assets/tiny-db-icon.png) | ![](../../../../.gitbook/assets/file-icon%20%281%29.png) | ![](../../../../.gitbook/assets/firebase-icon.png) | ![](../../../../.gitbook/assets/spreadsheets-icon.png) | ![](../../../../.gitbook/assets/fusion-tables-icon.png) | ![](../../../../.gitbook/assets/web-icon.png) | ![](../../../../.gitbook/assets/cloudinary-icon.png) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
|  | [Tiny DB](tiny-db.md) | [File](file.md) | [Firebase DB](firebase-db.md) | [Spreadsheets](spreadsheets.md) | [Fusion Tables](fusion-tables.md) | [Web](web.md) | [Cloudinary](cloudinary-db.md) |
| Description | Store and retrieve one row of data stored locally on the device; ideal for saving data from a previous app session | Store and retrieve files \(e.g. PDFs\) stored locally on the device | Store and retrieve one row of data stored in the cloud that can be set to private | Store and retrieve multiple rows of data stored in a Google or Microsoft spreadsheet | Store, query and delete more than a thousand rows of data secured by Google Service authentication | Query data from a web service \(e.g. Weather information\) | Store and retrieve image, audio or video files |
| Local / cloud | Works offline | Works offline | Can work offline in limited ways | Reliable data connection | Reliable data connection | Reliable data connection | Reliable data connection |
| Sample app types | All | PDF viewers | Messaging | Apps with lists, simple mapping | Complex mapping | Stock quotes, weather info | Images, audio files, videos |

**Important note**: Since the introduction of Firebase, we only recommend the [Tiny Web DB](tiny-web-db.md) component for specific cases where you want to own and manage your own database infrastructure

