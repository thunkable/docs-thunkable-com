# Sample Apps

##  ![](../../.gitbook/assets/remix-icon.png)

Thunkable is building the world's largest gallery of open sourced apps to help inspire you and save you time.

Below are a few of our favorites with more to come. Feel free to remix!

## Beginner

### Ukulele

Ukulele is a simple soundboard app that plays the ukulele chords for one of our favorite songs of all time \(and of the [best Hawaiian songs of all time](http://www.honolulumagazine.com/Honolulu-Magazine/June-2007/50-Greatest-Songs-of-Hawai-8217i/index.php?cparticle=2&siarticle=1#artanc)\), _Waikiki_, recorded in 1946 by Andy Cummings. The ukulele chords themselves were recorded by an aspiring but very amateur ukulele player / thunker Albert Ching \(originally from Waikiki\)

[**Click to remix**](https://goo.gl/knSQs4)

![Feel free to remix this for your favorite instruments although slower sounds will work better](../../.gitbook/assets/thunkable-docs-exhibits-13.png)

### New Market Goods

New Market Goods is a simple website app with a branding screen and a social media bar that opens a deep link to a user's installed apps that works across platforms. We recommend [URL genius](https://app.urlgeni.us/#/) to find deep links for commonly used apps. No set-up is required.

#### [Click to remix](https://goo.gl/Df56zz)

![If you have a mobile optimised website for your business or organization, this is a simple way to turn what you already have into an app.](../../.gitbook/assets/nmg.png)

### Feelings

Feelings is a swipe-able audio book powered by a Tab Navigator and a Text to Speech component. No set-up is required.

#### [Click to remix](https://goo.gl/xs2ZYn)

![](../../.gitbook/assets/feelings.png)

### Fun with Flags

This simple trivia app will test your user's knowledge of country flags. By building something like this for yourself you will develop your understanding of parallel lists, functions, APIs, incrementers and, string matching. You can find a more detailed tutorial of how to build this app in the [Thunkable Community](https://community.thunkable.com/t/quiz-app-fun-with-flags/32265?u=domhnall).

[**Click to remix**](https://x.thunkable.com/copy/6e09037b4bdc7ac4207521322b433137)

![How well do you know your flags?](../../.gitbook/assets/screen-shot-2018-06-20-at-11.27.50.png)

## **Medium**

### Aloha

Aloha is a private anonymous chat app with a short chat history powered by a [Firebase Realtime Database](../create/components/data/realtime-db.md). To [keep your data as private as possible](../create/app-data-privacy.md#create-your-own-private-repository-of-cloud-data), we recommend creating your own Firebase account and add your own API keys.

#### [Click to remix](https://goo.gl/jPNbTN)

![Forget trusting big companies to comply with GDPR; this is a scary simple way to set up private chat where you own and control your chat history](../../.gitbook/assets/docs-aloha.png)

### **こんにちは \(Kon'nichiwa\)**

こんにちは is an app designed for travel in any country. It uses the newly upgraded [Speech Recognizer](../create/components/voice/speech-recognizer.md) combined with the [Translator](../create/components/voice/translator.md) component powered by Yandex to translate any spoke phrase into one of 87 supported languages. The app also features persistent data using [Local Storage](../create/components/data/local-storage.md), importing a list of data from [Spreadsheet](../create/components/data/spreadsheet.md), and sharing results with the [Share](../create/components/social/share.md) component.

[**Click to remix**](https://goo.gl/DHp6Qv)

![](../../.gitbook/assets/docs-real.png)

### Personal Feed

Personal Feed is an easy to edit feed of your favorite websites, powered by a simple Airtable [spreadsheet](../create/components/data/spreadsheet.md) with descriptions that you can modify at any time. This app can be remixed in a number of ways but this example shares popular men's blogger Mister Ching's favorite products for the summer. This app features a Stack Navigator, a Share component, and custom fonts in Labels as well!

#### [Click to remix](https://goo.gl/3Y9WuD)

![](../../.gitbook/assets/docs-feed.png)

### Social Credit

Social Credit is a team counting app for thankless tasks. The app shares data for the team in a private Firebase realtime database account so Thunkers looking to create one for their team will need to [set one up](https://docs.thunkable.com/x/components/data-storage/realtime-db.html#set-up). The app also features some basic error handling and a for loop block

#### [Click to remix](https://goo.gl/2vCtAh)

![Social Credit has really transformed how our office works at Thunkable -- no longer are thankless tasks thankless. The winner each week gets to pick out our lunch destination on Friday \(which is quite an honor\)](../../.gitbook/assets/docs.png)

### Translator

Translator is an app that translates English text into the 20 most popular languages in the world; features advanced use of ListView and persistent data with Local Storage. No set-up is required although Thunkers can use their own Yandex API key if desired

#### [Click to remix](https://goo.gl/vYQNt2)

![](../../.gitbook/assets/translator%20%281%29.png)

### Dad

Dad is a digital version of Albert's dad, based on a recorded interview and powered by Dialogflow's [Assistant](../create/components/voice/assistant.md) service. Thunkers must create their own Dialogflow account to customize their digital version. You can read more of the story of this app on [our blog](https://blog.thunkable.com/meet-my-dad-in-an-app-8a93ded720e0).

#### [Click to remix](https://goo.gl/P94huP)

![This is one of our favorite apps we&apos;ve ever made on the platform -- it&apos;s a great combination of the latest in A.I. and voice technologies and our human need to keep our loved ones close to us at all times](../../.gitbook/assets/docs-dad.png)

### Weather

Weather is an app that pulls the latest temperature from the [Open Weather Map API](https://www.openweathermap.org/api) and as a bonus the latest traffic from the Google Maps component; Thunkers are encouraged to create a free account to use their own Open Weather Map API key

[**Click to remix**](https://goo.gl/cTaaXQ)

{% hint style="danger" %}
There is currently a bug on Android with loading this map.  We are hoping to fix this soon
{% endhint %}

![](../../.gitbook/assets/thunkable-docs-exhibits-1.png)

## Advanced

### Ride

Ride is a simple uber-like app designed for a single rider and driver that demonstrates some of the more complex possibilities of using the Google Maps APIs with the [Web API](../create/components/data/web-api.md) component including the geocoding, distance matrix and routing APIs.  Developers will have to first create and use their own Google Maps API key and [Realtime DB](../create/components/data/realtime-db.md) with Firebase. This is the first sample app that uses the cool renaming component feature that was just implemented.

{% hint style="danger" %}
This sample app currently crashes on Android but we are hoping to add a bug-free version soon
{% endhint %}

[**Click to remix**](https://goo.gl/hzH5Hz)

![This sample app is inspired by the cycle rickshaws of Dhaka and estimates travel distance by rickshaw/bicycle](../../.gitbook/assets/thunkable-docs-exhibits.png)

### Reservation

Reservation is a demonstration of how to accept credit card payments through your app. Thunkers must create their own Stripe account \(please [follow the documentation](https://docs.thunkable.com/ios/components/monetisation/payments.html) carefully on set-up\). The app also uploads user data to a [spreadsheet](https://docs.thunkable.com/ios/components/data-storage/spreadsheets.html) for proper tracking of user transactions.

#### [**Click to remix**](https://goo.gl/XY9cTx)

![](../../.gitbook/assets/thunkable-documentation-exhibits-97%20%281%29.png)

### Gram

Gram is what photo sharing should be -- ad-free, auto-captioning and secure. This app features the Sign In component with Realtime DB both powered by Firebase, Image Recognizer by Microsoft and a way to "heart" photos. Thunkers must create their own Firebase account and add their own API keys and database url in their account settings.

#### [Click to remix](https://goo.gl/gT6qEm)

![This is our most popular sample app so far -- over 1500 remixes and counting!](../../.gitbook/assets/docs-gram.png)



