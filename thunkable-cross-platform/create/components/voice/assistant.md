# Assistant

* [Set up](assistant.md#set-up)
* [Select listening language](assistant.md#select-listening-language)
* [Activate the Assistant](assistant.md#activate-the-assistant)

## Set up

### **Create a** [**free Dialogflow**](https://dialogflow.com/) **account**

![](../../../../.gitbook/assets/assistant-dialogflow-fig-1.png)

### Connect your Dialogflow agent with Thunkable

To connect your Dialogflow agent to Thunkable, you'll have to find the `Client Access Token`

![](../../../../.gitbook/assets/assistant-dialogflow-fig-2.png)

To find the `Client Access Token`, you'll have to first create an agent and then navigate to the General tab with the Settings page. Each agent has a unique Client Access Token

![](../../../../.gitbook/assets/assistant-dialogflow-fig-3.png)

### Create Intents with Text Responses

After you create our account, you will be asked to create an intent, which is simply a user expression that will prompt a given text response. The more intents that you create, the more commands or questions the Assistant will be able to respond to. Since the Assistant is powered by a breakthrough technology called natural language processing, the user won't have to always say exactly what is specified in the intents \(although the more expressions the better\)![](../../../../.gitbook/assets/assistant-ios-fig-1.png)![](../../../../.gitbook/assets/assistant-ios-fig-2.png)

## Select listening language

Amazingly, the Assistant understands multiple languages--13 in fact with an additional 5 accents

| Property | Description |
| :--- | :--- |
| Language | Refers to both the language recognized by the Assistant and the language which it speaks aloud. Currently available: `ENGLISH`,`ENGLISH_GB`, `ENGLISH_US`,`CHINESE_CHINA`,`CHINESE_HONGKONG`,`CHINESE_TAIWAN`,`DUTCH`, `FRENCH`,`GERMAN`,`GREEK`,`ITALIAN`,`JAPANESE`,`KOREAN`,`PORTUGUESE`,`PORTUGUESE_BRAZIL`,`RUSSIAN`,`SPANISH`,`UKRANIAN` |

## Activate the Assistant

The Assistant is powered by a speech recognizer which listens to a voice query. It's important to make sure the Assistant has enough time to listen to a voice query and return a response. The blocks below illustrate one way of implementing the Assistant Start and Stop procedures.

If the query is successful, it will return a text `value` that you can use to speak aloud or play a given sound as illustrated below

![](../../../../.gitbook/assets/assistant-dialogflow-fig-4.png)

| Event | Description |
| :--- | :--- |
| Start Listening | Asks the Assistant to start listening to a voice query. You must use both the Start Listening and Stop Listening events to |
| Stop Listening | Asks the Assistant to stop listening to a voice query |
| Query \(`text`\) | Submits a query to the Assistant in text form |

