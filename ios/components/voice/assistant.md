#### **Thunkable for iOS **

# Assistant aka Voice Assistant ![](/assets/dialogflow-assistant-ios-icon.png) powered by Dialogflow

---

The Assistant component powered by Dialogflow, an Alphabet company, enables real-time voice responses to user questions asked by voice. The Assistant understands a user's natural language and the developer simply programs the questions and responses to return to the user.![](/assets/assistant-ios-fig-5.png)

---

#### Set up

Since you are setting up your own assistant, also known as an agent, you will first need to create an account with [Dialogflow](https://dialogflow.com/).

**Step 1** **Create an intent\(s\)**. After you create our account, you will be asked to create an intent, which is simply _a user expression that will prompt a given text response_![](/assets/assistant-ios-fig-1.png)![](/assets/assistant-ios-fig-2.png)**Step 2 Find your agent's client access token.** After you've found it, you can copy it into the properties of the Assistant component in Thunkable

![](/assets/assistant-ios-fig-3.png)

| Property | Description |
| :--- | :--- |
| Dialogflow Client Access Token | Please generate your own account with Dialogflow. Each agent will have its own unique client access token |

---

#### Select language

Amazingly, the Assistant speaks multiple languages--13 in fact with an additional 5 accents

| Property | Description |
| :--- | :--- |
| Language | Refers to both the language recognized by the Assistant and the language which it speaks aloud. Currently available: `ENGLISH`,`ENGLISH_GB`, `ENGLISH_US`,`CHINESE_CHINA`,`CHINESE_HONGKONG`,`CHINESE_TAIWAN`,`DUTCH`, `FRENCH`,`GERMAN`,`GREEK`,`ITALIAN`,`JAPANESE`,`KOREAN`,`PORTUGUESE`,`PORTUGUESE_BRAZIL`,`RUSSIAN`,`SPANISH`,`UKRANIAN` |

---

#### Triggering the Assistant

The Assistant can be triggered both by voice or a text query.  The result is a text `value` that you can convert to speech with a Text to Speech component

![](/assets/assistant-ios-fig-4.png)

| Event | Description |
| :--- | :--- |
| Start Listening | Asks the Assistant to start listening to a voice query. You must use both the Start Listening and Stop Listening events to |
| Stop Listening | Asks the Assistant to stop listening to a voice query |
| Query \(`text`\) | Submits a query to the Assistant in text form |



