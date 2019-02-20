# Tiny Web DB

{% hint style="info" %}
Since the introduction of Firebase, we only recommend the Tiny Web DB component for specific cases where you want to own and manage your own database infrastructure
{% endhint %}

### Setting up your own database \(Take a deep breath!\)

By default, the Tiny Web DB component stores data on a test service provided by Thunkable. This service is helpful for testing, but it is shared by all Thunkable users, and it has a limit of 1000 entries. If you use it, your data will be overwritten eventually.

For most apps you write, you'll want to create a custom web service that isn't shared with other Thunkable apps and programmers.

To create your own web service, follow these instructions:

* Download App Engine for Python in Standard environments at [https://cloud.google.com/appengine/downloads](https://cloud.google.com/appengine/downloads). After installing it, run the GoogleAppEngineLauncher by clicking its icon.
* Download this [sample code](http://appinventor.mit.edu/explore/sites/all/files/tinywebdb/customtinywebdb.zip). It is a zip file containing the source code for your custom Tiny Web DB web service
* This code is setup to run with App Engine using Python 2.7, so you’ll need Python 2.7 on your computer. To check your version of Python, open up your Terminal and type in python. If you don't have the right version, you can download it from here
* To make sure that App Engine is configured to use it, in App Engine Launcher, choose Preferences and then put in path to Python2.7 \(On a Mac, this might be something like /usr/local/bin/python2.7 \)
* Unzip the downloaded zip file. It will create a folder named **customtinywebdb**. You can rename it if you want.
* In the GoogleAppEngineLauncher, choose **File \| Add Existing Application**. Browse to set the Path to the

  customtinywebdb folder you just unzipped. Then click the Run button. This will launch a test web service that runs on your local machine.

* You can test the service by opening a browser and entering "localhost:8080" as the URL. \(NOTE: if you've already created a web service, the port number \(8080\) may be different the second time, check the table in Google App Engine Launcher to see what Port number you should use\).
* You'll see the web page interface to your web service. The end-goal of this service is to communicate with a mobile app created with Thunkable. But the service provides a web page interface to the service to help programmers with debugging. You can invoke the get and store operations by hand, view the existing entries, and also delete individual entries. NOTE: If you are having problems creating a web page, click the Logs on the App Engine screen to diagnose the error.

Congrats, you've now made a webpage for your app. But your app is not yet on the web, and thus not yet accessible to an Thunkable app. To get it there, you need to upload it to Google's App Engine servers.

* In the GoogleAppEngineLauncher, choose **Dashboard**. Enter your Google account information and you'll be taken to an App Engine dashboard.
* Choose **Create an Application**. You'll need to specify a globally unique Application Identifier. Remember the Application identifier as you'll need it later. Provide a name to your app and click **Create Application** to submit. If your Identifier was unique, you now have a new, empty app on Google's servers.
* Open a text editor on your local computer and open the file **app.yaml** within the **customtinywebdb** folder you unzipped. Modify the first line so that the application matches the application identifier you set at Google.
* In GoogleAppEngineLauncher, choose **Deploy** and follow the steps for deploying your app.
* Test to see if your app is running on the web. In a browser, enter **&lt;myapp&gt;.appspot.com**, only substitute your application identifier for &lt;myapp&gt;. The app should look the same as when you ran it on the local test server. Only now, it's on the web and you can access it from your Thunkable for Android app.

Your Thunkable apps can store and retrieve data using your new service. Just do the following:

* Drag in a **Tiny Web DB** component into the Component Designer.
* Modify the ServiceURL property from the default [http://appinvtinywebdb.appspot.com/](https://appinvtinywebdb.appspot.com/)

  to your web service.

* Any StoreValue operations \(blocks\) will store data at your service, and any GetValue operations will retrieve from your service.

### Functionality

| Event | Description |
| :--- | :--- |
| Service URL | The URL to the database with which the component should communicate |
| Store Value \(tag, valueToStore\) | Sends a request to the Web service to store the given value under the given tag |
| Value Stored | Indicates that a StoreValue server request has succeeded |
| Get Value \(tag\) | Sends a request to the Web service to get the value stored under the given tag. The Web service must decide what to return if there is no value stored under the tag. This component accepts whatever is returned |
| Got Value \(tagFromWebDB, valueFromWebDB\) | Indicates that a GetValue server request has succeeded |
| Web Service Error \(message\) | Indicates that there was an error communicating with the Web service |

