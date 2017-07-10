#### **Thunkable for Android **❤

# Fusion Tables ![](/assets/fusion-tables-icon.png)

---

Fusion Tables is a powerful database component that lets you store, share and query big data sets in a cloud powered by Google. With the power of Fusion Tables does come consider set-up -- up to an hour at our last estimate. 

This component uses the [Fusion Tables API V2.0.]()

---

#### Set up

Applications using Fusion Tables must authenticate with Google's servers. 

To get set up, please follow [these instructions from our friends at MIT App Inventor](https://docs.google.com/document/d/1HifuZqz5xu0KPS-e4oUv-t-nQoUQ8VMNyh_y6OjZkc0/edit). It will take you through the 5 steps of set-up including creating a Google Developers account, a new project under that account, connecting that project to the Fusion Tables API, a service account for the project, and a new Fusion Table.

**Important note**: Initial set up time can take up to one hour \(due to changes from Google with the latest API\)

| Property | Description |
| :--- | :--- |
| API Key Your Google API Key. See above for details on obtaining an API key. |  |
| Key File Specifies the path of the private key file. This key file is used to get access to the FusionTables API through Service Authentication. |  |
|  |  |



  


Query

The query to send to the Fusion Tables API.

For legal query formats and examples, see the[Fusion Tables API V2.0 reference manual]().

  


Note that you do not need to worry about UTF-encoding the query. You must make sure the query follows the syntax described in the reference manual. Note that capitalization for names of columns is necessary and that single quotes must be used around column names if there are spaces in them.

  


ServiceAccountEmail

The Service Account Email Address used for Service Authentication.

  


UseServiceAuthentication

Indicates whether a service account should be used for authentication.

• Methods

GotResult\(text result\)

Indicates that the Fusion Tables query has finished processing and returned with a result. The result of the query will generally be returned in CSV format, and can be converted to list format using the "list from csv table" or "list from csv row" blocks.

  


![](https://thunkable.com/reference/components/images/user_interface/u155.png)

FusionTablesControl

  


#### Functionality

| Event | Description |
| :--- | :--- |
| Service URL | The URL to the database with which the component should communicate |
| Store Value \(tag, valueToStore\) | Sends a request to the Web service to store the given value under the given tag |
| Value Stored | Indicates that a StoreValue server request has succeeded |
| Get Value \(tag\) | Sends a request to the Web service to get the value stored under the given tag. The Web service must decide what to return if there is no value stored under the tag. This component accepts whatever is returned |
| Got Value \(tagFromWebDB, valueFromWebDB\) | Indicates that a GetValue server request has succeeded |
| Web Service Error \(message\) | Indicates that there was an error communicating with the Web service |



#### Functionality

| Event | Description |
| :--- | :--- |
| Service URL | The URL to the database with which the component should communicate |
| Store Value \(tag, valueToStore\) | Sends a request to the Web service to store the given value under the given tag |
| Value Stored | Indicates that a StoreValue server request has succeeded |
| Get Value \(tag\) | Sends a request to the Web service to get the value stored under the given tag. The Web service must decide what to return if there is no value stored under the tag. This component accepts whatever is returned |
| Got Value \(tagFromWebDB, valueFromWebDB\) | Indicates that a GetValue server request has succeeded |
| Web Service Error \(message\) | Indicates that there was an error communicating with the Web service |



